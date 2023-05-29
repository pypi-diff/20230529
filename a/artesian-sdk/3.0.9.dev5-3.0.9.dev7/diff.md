# Comparing `tmp/artesian-sdk-3.0.9.dev5.tar.gz` & `tmp/artesian-sdk-3.0.9.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artesian-sdk-3.0.9.dev5.tar", last modified: Fri Mar 10 12:36:55 2023, max compression
+gzip compressed data, was "artesian-sdk-3.0.9.dev7.tar", last modified: Tue May  9 13:57:11 2023, max compression
```

## Comparing `artesian-sdk-3.0.9.dev5.tar` & `artesian-sdk-3.0.9.dev7.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:36:55.524239 artesian-sdk-3.0.9.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:36:55.512238 artesian-sdk-3.0.9.dev5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:36:55.512238 artesian-sdk-3.0.9.dev5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/.github/workflows/python-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:36:55.512238 artesian-sdk-3.0.9.dev5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22765 2023-03-10 12:36:55.524239 artesian-sdk-3.0.9.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20757 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:36:55.516238 artesian-sdk-3.0.9.dev5/samples/
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/samples/TestActual.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/samples/TestAuction.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/samples/TestBidAsk.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/samples/TestGMEOffers.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/samples/TestMarketDataService.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/samples/TestMas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/samples/TestVersioned.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/samples/TestWriteDataAndQueryActual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/samples/TestWriteDataAndQueryAuction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/samples/TestWriteDataAndQueryBidAsk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/samples/TestWriteDataAndQueryMas.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 12:36:55.524239 artesian-sdk-3.0.9.dev5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:36:55.512238 artesian-sdk-3.0.9.dev5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:36:55.516238 artesian-sdk-3.0.9.dev5/src/Artesian/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/ArtesianConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/ArtesianPolicyConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:36:55.516238 artesian-sdk-3.0.9.dev5/src/Artesian/GMEPublicOffers/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/GMEPublicOffers/ExtractionRangeConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    15089 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/GMEPublicOffers/GMEPublicOfferQuery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/GMEPublicOffers/GMEPublicOfferQueryParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/GMEPublicOffers/GMEPublicOfferService.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:36:55.516238 artesian-sdk-3.0.9.dev5/src/Artesian/GMEPublicOffers/_Enum/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/GMEPublicOffers/_Enum/BaType.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/GMEPublicOffers/_Enum/GenerationType.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/GMEPublicOffers/_Enum/Market.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/GMEPublicOffers/_Enum/Purpose.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/GMEPublicOffers/_Enum/Scope.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/GMEPublicOffers/_Enum/Status.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/GMEPublicOffers/_Enum/UnitType.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/GMEPublicOffers/_Enum/Zone.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/GMEPublicOffers/_Enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/GMEPublicOffers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Granularity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:36:55.516238 artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/
--rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/MarketDataService.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:36:55.516238 artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/_Dto/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/_Dto/CurveRangeEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/_Dto/MarketDataEntityInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/_Dto/MarketDataEntityOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/_Dto/MarketDataIdentifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/_Dto/PagedResult.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/_Dto/UpsertData.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/_Dto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:36:55.520238 artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/_Enum/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/_Enum/AggregationRule.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/_Enum/MarketDataType.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/_Enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:36:55.520238 artesian-sdk-3.0.9.dev5/src/Artesian/Query/
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/ActualQuery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/AuctionQuery.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/BidAskQuery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/DefaultPartitionStrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/MasQuery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/QueryService.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/RelativeInterval.py
--rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/VersionedQuery.py
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/_Query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:36:55.520238 artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/ActualQueryParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/AuctionQueryParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/BidAskQueryParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/ExtractionRangeConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/ExtractionRangeType.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/MasQueryParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/MostRecentSelectionConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/QueryParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/VersionSelectionConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/VersionSelectionType.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/VersionedQueryParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/VersionsRangeSelectionConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/Query/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:36:55.520238 artesian-sdk-3.0.9.dev5/src/Artesian/_ClientsExecutor/
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/_ClientsExecutor/ArtesianJsonSerializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/_ClientsExecutor/Client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/_ClientsExecutor/RequestExecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/_ClientsExecutor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/src/Artesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-10 12:36:55.000000 artesian-sdk-3.0.9.dev5/src/Artesian/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:36:55.520238 artesian-sdk-3.0.9.dev5/src/artesian_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22765 2023-03-10 12:36:55.000000 artesian-sdk-3.0.9.dev5/src/artesian_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-03-10 12:36:55.000000 artesian-sdk-3.0.9.dev5/src/artesian_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 12:36:55.000000 artesian-sdk-3.0.9.dev5/src/artesian_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-10 12:36:55.000000 artesian-sdk-3.0.9.dev5/src/artesian_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-10 12:36:55.000000 artesian-sdk-3.0.9.dev5/src/artesian_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:36:55.524239 artesian-sdk-3.0.9.dev5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/tests/TestActual.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/tests/TestBidAsk.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/tests/TestClientErrorHandling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/tests/TestMarketDataService.py
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/tests/TestMarketDataUpsertData.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/tests/TestMas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/tests/TestVersioned.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-10 12:36:44.000000 artesian-sdk-3.0.9.dev5/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:57:11.800051 artesian-sdk-3.0.9.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:57:11.788050 artesian-sdk-3.0.9.dev7/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:57:11.788050 artesian-sdk-3.0.9.dev7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/.github/workflows/python-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:57:11.788050 artesian-sdk-3.0.9.dev7/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22765 2023-05-09 13:57:11.800051 artesian-sdk-3.0.9.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20757 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:57:11.788050 artesian-sdk-3.0.9.dev7/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/samples/TestActual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/samples/TestAuction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/samples/TestBidAsk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/samples/TestGMEOffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/samples/TestMarketDataService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/samples/TestMas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/samples/TestVersioned.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/samples/TestWriteDataAndQueryActual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/samples/TestWriteDataAndQueryAuction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/samples/TestWriteDataAndQueryBidAsk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/samples/TestWriteDataAndQueryMas.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 13:57:11.800051 artesian-sdk-3.0.9.dev7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:57:11.784050 artesian-sdk-3.0.9.dev7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:57:11.792050 artesian-sdk-3.0.9.dev7/src/Artesian/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/ArtesianConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/ArtesianPolicyConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:57:11.792050 artesian-sdk-3.0.9.dev7/src/Artesian/GMEPublicOffers/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/GMEPublicOffers/ExtractionRangeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15089 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/GMEPublicOffers/GMEPublicOfferQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/GMEPublicOffers/GMEPublicOfferQueryParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/GMEPublicOffers/GMEPublicOfferService.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:57:11.792050 artesian-sdk-3.0.9.dev7/src/Artesian/GMEPublicOffers/_Enum/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/GMEPublicOffers/_Enum/BaType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/GMEPublicOffers/_Enum/GenerationType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/GMEPublicOffers/_Enum/Market.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/GMEPublicOffers/_Enum/Purpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/GMEPublicOffers/_Enum/Scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/GMEPublicOffers/_Enum/Status.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/GMEPublicOffers/_Enum/UnitType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/GMEPublicOffers/_Enum/Zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/GMEPublicOffers/_Enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/GMEPublicOffers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Granularity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:57:11.792050 artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/
+-rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/MarketDataService.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:57:11.792050 artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/_Dto/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/_Dto/CurveRangeEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/_Dto/MarketDataEntityInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/_Dto/MarketDataEntityOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/_Dto/MarketDataIdentifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/_Dto/PagedResult.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/_Dto/UpsertData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/_Dto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:57:11.796051 artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/_Enum/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/_Enum/AggregationRule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/_Enum/MarketDataType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/_Enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:57:11.796051 artesian-sdk-3.0.9.dev7/src/Artesian/Query/
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/ActualQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/AuctionQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/BidAskQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/DefaultPartitionStrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/MasQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/QueryService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/RelativeInterval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/VersionedQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/_Query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:57:11.796051 artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/ActualQueryParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/AuctionQueryParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/BidAskQueryParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/ExtractionRangeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/ExtractionRangeType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/MasQueryParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/MostRecentSelectionConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/QueryParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/VersionSelectionConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/VersionSelectionType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/VersionedQueryParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/VersionsRangeSelectionConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/Query/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:57:11.800051 artesian-sdk-3.0.9.dev7/src/Artesian/_ClientsExecutor/
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/_ClientsExecutor/ArtesianJsonSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/_ClientsExecutor/Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/_ClientsExecutor/RequestExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/_ClientsExecutor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/src/Artesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-09 13:57:11.000000 artesian-sdk-3.0.9.dev7/src/Artesian/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:57:11.800051 artesian-sdk-3.0.9.dev7/src/artesian_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22765 2023-05-09 13:57:11.000000 artesian-sdk-3.0.9.dev7/src/artesian_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-09 13:57:11.000000 artesian-sdk-3.0.9.dev7/src/artesian_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:57:11.000000 artesian-sdk-3.0.9.dev7/src/artesian_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-09 13:57:11.000000 artesian-sdk-3.0.9.dev7/src/artesian_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 13:57:11.000000 artesian-sdk-3.0.9.dev7/src/artesian_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:57:11.800051 artesian-sdk-3.0.9.dev7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/tests/TestActual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/tests/TestBidAsk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/tests/TestClientErrorHandling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/tests/TestMarketDataService.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/tests/TestMarketDataUpsertData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/tests/TestMas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/tests/TestVersioned.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-09 13:56:55.000000 artesian-sdk-3.0.9.dev7/tests/helpers.py
```

### Comparing `artesian-sdk-3.0.9.dev5/.github/workflows/python-tests.yml` & `artesian-sdk-3.0.9.dev7/.github/workflows/python-tests.yml`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/.gitignore` & `artesian-sdk-3.0.9.dev7/.gitignore`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/.vscode/launch.json` & `artesian-sdk-3.0.9.dev7/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/LICENSE` & `artesian-sdk-3.0.9.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/PKG-INFO` & `artesian-sdk-3.0.9.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artesian-sdk
-Version: 3.0.9.dev5
+Version: 3.0.9.dev7
 Summary: Library provides read access to the Artesian API
 Author-email: ARK Lab <arklab@ark-energy.eu>
 Maintainer-email: ARK Lab <arklab@ark-energy.eu>
 License: MIT License
         
         Copyright (c) 2022 Ark Energy S.r.l.
```

### Comparing `artesian-sdk-3.0.9.dev5/README.md` & `artesian-sdk-3.0.9.dev7/README.md`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/pyproject.toml` & `artesian-sdk-3.0.9.dev7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/samples/TestActual.py` & `artesian-sdk-3.0.9.dev7/samples/TestActual.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/samples/TestAuction.py` & `artesian-sdk-3.0.9.dev7/samples/TestAuction.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/samples/TestVersioned.py` & `artesian-sdk-3.0.9.dev7/samples/TestVersioned.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/samples/TestWriteDataAndQueryActual.py` & `artesian-sdk-3.0.9.dev7/samples/TestWriteDataAndQueryActual.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/samples/TestWriteDataAndQueryAuction.py` & `artesian-sdk-3.0.9.dev7/samples/TestWriteDataAndQueryAuction.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/samples/TestWriteDataAndQueryBidAsk.py` & `artesian-sdk-3.0.9.dev7/samples/TestWriteDataAndQueryBidAsk.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/samples/TestWriteDataAndQueryMas.py` & `artesian-sdk-3.0.9.dev7/samples/TestWriteDataAndQueryMas.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/ArtesianConfig.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/ArtesianConfig.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/ArtesianPolicyConfig.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/ArtesianPolicyConfig.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/Exceptions.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/Exceptions.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/GMEPublicOffers/GMEPublicOfferQuery.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/GMEPublicOffers/GMEPublicOfferQuery.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/GMEPublicOffers/GMEPublicOfferQueryParameters.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/GMEPublicOffers/GMEPublicOfferQueryParameters.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/GMEPublicOffers/GMEPublicOfferService.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/GMEPublicOffers/GMEPublicOfferService.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/GMEPublicOffers/__init__.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/GMEPublicOffers/__init__.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/MarketDataService.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/MarketDataService.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/_Dto/CurveRangeEntity.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/_Dto/CurveRangeEntity.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/_Dto/MarketDataEntityInput.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/_Dto/MarketDataEntityInput.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/_Dto/MarketDataEntityOutput.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/_Dto/MarketDataEntityOutput.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/_Dto/PagedResult.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/_Dto/PagedResult.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/_Dto/UpsertData.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/_Dto/UpsertData.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/_Dto/__init__.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/_Dto/__init__.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/MarketData/__init__.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/MarketData/__init__.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/Query/ActualQuery.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/Query/ActualQuery.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/Query/AuctionQuery.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/Query/AuctionQuery.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/Query/BidAskQuery.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/Query/BidAskQuery.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/Query/DefaultPartitionStrategy.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/Query/DefaultPartitionStrategy.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/Query/MasQuery.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/Query/MasQuery.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/Query/QueryService.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/Query/QueryService.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/Query/VersionedQuery.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/Query/VersionedQuery.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/Query/_Query.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/Query/_Query.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/ActualQueryParameters.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/ActualQueryParameters.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/AuctionQueryParameters.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/AuctionQueryParameters.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/BidAskQueryParameters.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/BidAskQueryParameters.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/ExtractionRangeConfig.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/ExtractionRangeConfig.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/MasQueryParameters.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/MasQueryParameters.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/MostRecentSelectionConfig.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/MostRecentSelectionConfig.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/QueryParameters.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/QueryParameters.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/VersionSelectionConfig.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/VersionSelectionConfig.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/VersionedQueryParameters.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/VersionedQueryParameters.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/Query/_QueryParameters/VersionsRangeSelectionConfig.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/Query/_QueryParameters/VersionsRangeSelectionConfig.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/_ClientsExecutor/ArtesianJsonSerializer.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/_ClientsExecutor/ArtesianJsonSerializer.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/_ClientsExecutor/Client.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/_ClientsExecutor/Client.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/_ClientsExecutor/RequestExecutor.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/_ClientsExecutor/RequestExecutor.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/Artesian/__init__.py` & `artesian-sdk-3.0.9.dev7/src/Artesian/__init__.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/src/artesian_sdk.egg-info/PKG-INFO` & `artesian-sdk-3.0.9.dev7/src/artesian_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artesian-sdk
-Version: 3.0.9.dev5
+Version: 3.0.9.dev7
 Summary: Library provides read access to the Artesian API
 Author-email: ARK Lab <arklab@ark-energy.eu>
 Maintainer-email: ARK Lab <arklab@ark-energy.eu>
 License: MIT License
         
         Copyright (c) 2022 Ark Energy S.r.l.
```

### Comparing `artesian-sdk-3.0.9.dev5/src/artesian_sdk.egg-info/SOURCES.txt` & `artesian-sdk-3.0.9.dev7/src/artesian_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/tests/TestActual.py` & `artesian-sdk-3.0.9.dev7/tests/TestActual.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/tests/TestBidAsk.py` & `artesian-sdk-3.0.9.dev7/tests/TestBidAsk.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/tests/TestClientErrorHandling.py` & `artesian-sdk-3.0.9.dev7/tests/TestClientErrorHandling.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/tests/TestMarketDataService.py` & `artesian-sdk-3.0.9.dev7/tests/TestMarketDataService.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/tests/TestMarketDataUpsertData.py` & `artesian-sdk-3.0.9.dev7/tests/TestMarketDataUpsertData.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/tests/TestMas.py` & `artesian-sdk-3.0.9.dev7/tests/TestMas.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/tests/TestVersioned.py` & `artesian-sdk-3.0.9.dev7/tests/TestVersioned.py`

 * *Files identical despite different names*

### Comparing `artesian-sdk-3.0.9.dev5/tests/helpers.py` & `artesian-sdk-3.0.9.dev7/tests/helpers.py`

 * *Files identical despite different names*

