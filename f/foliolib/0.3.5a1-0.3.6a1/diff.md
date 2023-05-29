# Comparing `tmp/foliolib-0.3.5a1.tar.gz` & `tmp/foliolib-0.3.6a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foliolib-0.3.5a1.tar", last modified: Sat May 20 15:30:27 2023, max compression
+gzip compressed data, was "foliolib-0.3.6a1.tar", last modified: Mon May 29 06:17:20 2023, max compression
```

## Comparing `foliolib-0.3.5a1.tar` & `foliolib-0.3.6a1.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-20 15:30:27.142341 foliolib-0.3.5a1/
--rw-r--r--   0 tobi      (1000) tobi      (1000)    35146 2020-10-11 07:41:52.000000 foliolib-0.3.5a1/COPYING
--rw-r--r--   0 tobi      (1000) tobi      (1000)       43 2020-11-07 12:13:21.000000 foliolib-0.3.5a1/MANIFEST.in
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2459 2023-05-20 15:30:27.142341 foliolib-0.3.5a1/PKG-INFO
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1719 2023-02-21 11:23:02.000000 foliolib-0.3.5a1/README.rst
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-20 15:30:27.134341 foliolib-0.3.5a1/foliolib/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1031 2023-03-24 13:25:47.000000 foliolib-0.3.5a1/foliolib/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      396 2023-05-20 15:30:26.000000 foliolib-0.3.5a1/foliolib/__version__.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-20 15:30:27.134341 foliolib-0.3.5a1/foliolib/apiBuilder/
--rw-r--r--   0 tobi      (1000) tobi      (1000)      351 2022-10-11 12:37:16.000000 foliolib-0.3.5a1/foliolib/apiBuilder/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1288 2022-03-13 04:11:25.000000 foliolib-0.3.5a1/foliolib/apiBuilder/build_api.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1586 2022-05-04 20:18:39.000000 foliolib-0.3.5a1/foliolib/apiBuilder/cli.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-20 15:30:27.134341 foliolib-0.3.5a1/foliolib/cli/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3821 2023-04-21 06:17:59.000000 foliolib-0.3.5a1/foliolib/cli/__init__.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-20 15:30:27.134341 foliolib-0.3.5a1/foliolib/cli/folio/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1461 2022-05-09 17:53:56.000000 foliolib-0.3.5a1/foliolib/cli/folio/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      229 2022-04-05 13:20:51.000000 foliolib-0.3.5a1/foliolib/cli/folio/inventory.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      634 2022-02-21 04:57:32.000000 foliolib-0.3.5a1/foliolib/cli/main.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      374 2022-02-21 04:57:41.000000 foliolib-0.3.5a1/foliolib/cli/main_err.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      895 2022-02-21 04:57:36.000000 foliolib-0.3.5a1/foliolib/cli/main_noauth.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4591 2023-04-15 04:58:38.000000 foliolib-0.3.5a1/foliolib/cli/module.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3495 2023-04-01 07:43:09.000000 foliolib-0.3.5a1/foliolib/cli/okapi.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      446 2022-02-21 04:57:17.000000 foliolib-0.3.5a1/foliolib/cli/orderedGroup.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3680 2023-02-15 15:06:27.000000 foliolib-0.3.5a1/foliolib/cli/platform.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2759 2023-04-21 05:25:46.000000 foliolib-0.3.5a1/foliolib/cli/server.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    12868 2022-10-06 05:29:03.000000 foliolib-0.3.5a1/foliolib/cli/tenant.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    12406 2023-05-20 05:12:45.000000 foliolib-0.3.5a1/foliolib/config.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      801 2022-05-09 17:52:49.000000 foliolib-0.3.5a1/foliolib/exceptions.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-20 15:30:27.134341 foliolib-0.3.5a1/foliolib/folio/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1870 2022-10-06 05:35:01.000000 foliolib-0.3.5a1/foliolib/folio/__init__.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-20 15:30:27.142341 foliolib-0.3.5a1/foliolib/folio/api/
--rw-r--r--   0 tobi      (1000) tobi      (1000)        0 2021-11-15 08:23:39.000000 foliolib-0.3.5a1/foliolib/folio/api/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9675 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/audit.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2643 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/authtoken.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6783 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/bulkOperations.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8152 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/calendar.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    40174 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/circulation.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    73691 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/circulationStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6506 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/configuration.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    10526 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/consortia.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4913 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/copycat.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    54009 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/courses.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    19883 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/dataExport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6349 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/dataExportSpring.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    10066 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/dataExportWorker.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    13485 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/dataImport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    37645 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/dataImportConverterStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    41060 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/diConverterStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2213 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/ebsconet.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     7884 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/email.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4984 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/entitiesLinks.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    25152 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/ermUsage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4482 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/ermUsageHarvester.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8498 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/eusageReports.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4273 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/eventConfig.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    80620 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/feesfines.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    76479 2023-05-20 04:20:10.000000 foliolib-0.3.5a1/foliolib/folio/api/finance.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    79172 2023-05-20 04:20:10.000000 foliolib-0.3.5a1/foliolib/folio/api/financeStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    51717 2023-05-20 04:20:10.000000 foliolib-0.3.5a1/foliolib/folio/api/fincConfig.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6999 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/folioCustomFields.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1342 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/folioSpringBase.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1787 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/folioVertxLib.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8283 2023-05-20 04:20:10.000000 foliolib-0.3.5a1/foliolib/folio/api/gobi.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     7801 2023-05-20 04:20:10.000000 foliolib-0.3.5a1/foliolib/folio/api/idmConnect.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    74110 2023-05-20 04:20:28.000000 foliolib-0.3.5a1/foliolib/folio/api/innReach.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    22929 2023-05-20 04:20:28.000000 foliolib-0.3.5a1/foliolib/folio/api/inventory.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)   220610 2023-05-20 04:20:29.000000 foliolib-0.3.5a1/foliolib/folio/api/inventoryStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6001 2023-05-20 04:20:29.000000 foliolib-0.3.5a1/foliolib/folio/api/inventoryUpdate.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    45051 2023-05-20 04:20:29.000000 foliolib-0.3.5a1/foliolib/folio/api/invoice.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    47143 2023-05-20 04:20:29.000000 foliolib-0.3.5a1/foliolib/folio/api/invoiceStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    54294 2023-05-20 04:20:29.000000 foliolib-0.3.5a1/foliolib/folio/api/kbEbscoJava.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3051 2023-05-20 04:20:29.000000 foliolib-0.3.5a1/foliolib/folio/api/ldp.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1332 2023-05-20 04:20:29.000000 foliolib-0.3.5a1/foliolib/folio/api/licenses.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8538 2023-05-20 04:20:29.000000 foliolib-0.3.5a1/foliolib/folio/api/login.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4260 2023-05-20 04:20:29.000000 foliolib-0.3.5a1/foliolib/folio/api/loginSaml.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17932 2023-05-20 04:20:29.000000 foliolib-0.3.5a1/foliolib/folio/api/marccat.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    20533 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/metaStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8754 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/notes.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8870 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/notify.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    12105 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/oaiPmh.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    63105 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/orders.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    78262 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/ordersStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4978 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/organizations.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    45825 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/organizationsStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3632 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/passwordValidator.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5893 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/patron.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    15601 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/patronBlocks.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    14392 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/permissions.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9093 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/pubsub.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4214 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/quickMarc.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17165 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/remoteStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    21731 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/reservoir.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1928 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/rtac.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17672 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/search.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      732 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/sender.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5419 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/settings.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    11215 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/sharedIndex.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    23625 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/sourceRecordManager.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    28052 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/sourceRecordStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3187 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/tags.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4091 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/templateEngine.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      870 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/userImport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    24002 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/users.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    11127 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/usersBl.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5803 2022-05-31 09:32:11.000000 foliolib-0.3.5a1/foliolib/folio/config.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8495 2021-02-25 09:49:29.000000 foliolib-0.3.5a1/foliolib/folio/dataImport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      436 2022-03-17 02:39:17.000000 foliolib-0.3.5a1/foliolib/folio/exceptions.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      945 2022-04-08 08:56:47.000000 foliolib-0.3.5a1/foliolib/folio/inventory.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    24355 2023-05-09 16:17:52.000000 foliolib-0.3.5a1/foliolib/folio/inventoryReferenceData.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9397 2023-05-20 07:12:08.000000 foliolib-0.3.5a1/foliolib/folio/users.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-20 15:30:27.142341 foliolib-0.3.5a1/foliolib/helper/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1207 2023-04-21 05:23:46.000000 foliolib-0.3.5a1/foliolib/helper/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9311 2023-04-21 05:23:46.000000 foliolib-0.3.5a1/foliolib/helper/database.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3636 2022-10-11 03:50:00.000000 foliolib-0.3.5a1/foliolib/helper/folio.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3055 2023-02-09 19:10:16.000000 foliolib-0.3.5a1/foliolib/helper/modules.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3935 2023-04-01 06:20:04.000000 foliolib-0.3.5a1/foliolib/helper/okapi.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5714 2023-02-18 17:54:00.000000 foliolib-0.3.5a1/foliolib/helper/platform.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1517 2022-10-11 03:48:54.000000 foliolib-0.3.5a1/foliolib/helper/tenant.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-20 15:30:27.142341 foliolib-0.3.5a1/foliolib/okapi/
--rw-r--r--   0 tobi      (1000) tobi      (1000)    14520 2022-10-13 08:48:51.000000 foliolib-0.3.5a1/foliolib/okapi/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2399 2022-07-24 04:45:10.000000 foliolib-0.3.5a1/foliolib/okapi/exceptions.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    16267 2023-04-21 05:23:46.000000 foliolib-0.3.5a1/foliolib/okapi/kubeClient.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      542 2022-03-22 15:04:58.000000 foliolib-0.3.5a1/foliolib/okapi/misc.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    38800 2023-04-21 05:23:46.000000 foliolib-0.3.5a1/foliolib/okapi/okapiClient.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    10030 2023-02-02 10:53:21.000000 foliolib-0.3.5a1/foliolib/okapi/okapiModule.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17121 2023-04-21 05:23:46.000000 foliolib-0.3.5a1/foliolib/okapi/okapiModuleKubernetes.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-20 15:30:27.134341 foliolib-0.3.5a1/foliolib.egg-info/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2459 2023-05-20 15:30:27.000000 foliolib-0.3.5a1/foliolib.egg-info/PKG-INFO
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3790 2023-05-20 15:30:27.000000 foliolib-0.3.5a1/foliolib.egg-info/SOURCES.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)        1 2023-05-20 15:30:27.000000 foliolib-0.3.5a1/foliolib.egg-info/dependency_links.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)       46 2023-05-20 15:30:27.000000 foliolib-0.3.5a1/foliolib.egg-info/entry_points.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)      130 2023-05-20 15:30:27.000000 foliolib-0.3.5a1/foliolib.egg-info/requires.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)      126 2023-05-20 15:30:27.000000 foliolib-0.3.5a1/foliolib.egg-info/top_level.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)      305 2023-02-21 08:41:56.000000 foliolib-0.3.5a1/requirements.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1182 2023-05-20 15:30:27.142341 foliolib-0.3.5a1/setup.cfg
--rw-r--r--   0 tobi      (1000) tobi      (1000)      117 2022-10-11 12:39:31.000000 foliolib-0.3.5a1/setup.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-29 06:17:20.421483 foliolib-0.3.6a1/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    35146 2020-10-11 07:41:52.000000 foliolib-0.3.6a1/COPYING
+-rw-r--r--   0 tobi      (1000) tobi      (1000)       43 2020-11-07 12:13:21.000000 foliolib-0.3.6a1/MANIFEST.in
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2459 2023-05-29 06:17:20.421483 foliolib-0.3.6a1/PKG-INFO
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1719 2023-02-21 11:23:02.000000 foliolib-0.3.6a1/README.rst
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-29 06:17:20.409483 foliolib-0.3.6a1/foliolib/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1031 2023-03-24 13:25:47.000000 foliolib-0.3.6a1/foliolib/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      396 2023-05-29 06:17:20.000000 foliolib-0.3.6a1/foliolib/__version__.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-29 06:17:20.409483 foliolib-0.3.6a1/foliolib/apiBuilder/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      351 2022-10-11 12:37:16.000000 foliolib-0.3.6a1/foliolib/apiBuilder/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1288 2022-03-13 04:11:25.000000 foliolib-0.3.6a1/foliolib/apiBuilder/build_api.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1586 2022-05-04 20:18:39.000000 foliolib-0.3.6a1/foliolib/apiBuilder/cli.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-29 06:17:20.413483 foliolib-0.3.6a1/foliolib/cli/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3821 2023-04-21 06:17:59.000000 foliolib-0.3.6a1/foliolib/cli/__init__.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-29 06:17:20.413483 foliolib-0.3.6a1/foliolib/cli/folio/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1461 2022-05-09 17:53:56.000000 foliolib-0.3.6a1/foliolib/cli/folio/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      229 2022-04-05 13:20:51.000000 foliolib-0.3.6a1/foliolib/cli/folio/inventory.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      634 2022-02-21 04:57:32.000000 foliolib-0.3.6a1/foliolib/cli/main.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      374 2022-02-21 04:57:41.000000 foliolib-0.3.6a1/foliolib/cli/main_err.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      895 2022-02-21 04:57:36.000000 foliolib-0.3.6a1/foliolib/cli/main_noauth.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4591 2023-04-15 04:58:38.000000 foliolib-0.3.6a1/foliolib/cli/module.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3495 2023-04-01 07:43:09.000000 foliolib-0.3.6a1/foliolib/cli/okapi.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      446 2022-02-21 04:57:17.000000 foliolib-0.3.6a1/foliolib/cli/orderedGroup.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3892 2023-05-29 05:12:42.000000 foliolib-0.3.6a1/foliolib/cli/platform.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2759 2023-04-21 05:25:46.000000 foliolib-0.3.6a1/foliolib/cli/server.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    12868 2022-10-06 05:29:03.000000 foliolib-0.3.6a1/foliolib/cli/tenant.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    12652 2023-05-26 13:04:01.000000 foliolib-0.3.6a1/foliolib/config.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      801 2022-05-09 17:52:49.000000 foliolib-0.3.6a1/foliolib/exceptions.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-29 06:17:20.413483 foliolib-0.3.6a1/foliolib/folio/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1870 2022-10-06 05:35:01.000000 foliolib-0.3.6a1/foliolib/folio/__init__.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-29 06:17:20.421483 foliolib-0.3.6a1/foliolib/folio/api/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)        0 2021-11-15 08:23:39.000000 foliolib-0.3.6a1/foliolib/folio/api/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9675 2023-05-20 04:20:08.000000 foliolib-0.3.6a1/foliolib/folio/api/audit.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2643 2023-05-20 04:20:08.000000 foliolib-0.3.6a1/foliolib/folio/api/authtoken.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6783 2023-05-20 04:20:08.000000 foliolib-0.3.6a1/foliolib/folio/api/bulkOperations.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8152 2023-05-20 04:20:08.000000 foliolib-0.3.6a1/foliolib/folio/api/calendar.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    40174 2023-05-20 04:20:08.000000 foliolib-0.3.6a1/foliolib/folio/api/circulation.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    73691 2023-05-20 04:20:08.000000 foliolib-0.3.6a1/foliolib/folio/api/circulationStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6506 2023-05-20 04:20:08.000000 foliolib-0.3.6a1/foliolib/folio/api/configuration.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    10526 2023-05-20 04:20:08.000000 foliolib-0.3.6a1/foliolib/folio/api/consortia.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4913 2023-05-20 04:20:08.000000 foliolib-0.3.6a1/foliolib/folio/api/copycat.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    54009 2023-05-20 04:20:08.000000 foliolib-0.3.6a1/foliolib/folio/api/courses.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    19883 2023-05-20 04:20:09.000000 foliolib-0.3.6a1/foliolib/folio/api/dataExport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6349 2023-05-20 04:20:09.000000 foliolib-0.3.6a1/foliolib/folio/api/dataExportSpring.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    10066 2023-05-20 04:20:09.000000 foliolib-0.3.6a1/foliolib/folio/api/dataExportWorker.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    13485 2023-05-20 04:20:09.000000 foliolib-0.3.6a1/foliolib/folio/api/dataImport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    37645 2023-05-20 04:20:09.000000 foliolib-0.3.6a1/foliolib/folio/api/dataImportConverterStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    41060 2023-05-20 04:20:09.000000 foliolib-0.3.6a1/foliolib/folio/api/diConverterStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2213 2023-05-20 04:20:09.000000 foliolib-0.3.6a1/foliolib/folio/api/ebsconet.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     7884 2023-05-20 04:20:09.000000 foliolib-0.3.6a1/foliolib/folio/api/email.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4984 2023-05-20 04:20:09.000000 foliolib-0.3.6a1/foliolib/folio/api/entitiesLinks.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    25152 2023-05-20 04:20:09.000000 foliolib-0.3.6a1/foliolib/folio/api/ermUsage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4482 2023-05-20 04:20:09.000000 foliolib-0.3.6a1/foliolib/folio/api/ermUsageHarvester.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8498 2023-05-20 04:20:09.000000 foliolib-0.3.6a1/foliolib/folio/api/eusageReports.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4273 2023-05-20 04:20:09.000000 foliolib-0.3.6a1/foliolib/folio/api/eventConfig.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    80620 2023-05-20 04:20:09.000000 foliolib-0.3.6a1/foliolib/folio/api/feesfines.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    76479 2023-05-20 04:20:10.000000 foliolib-0.3.6a1/foliolib/folio/api/finance.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    79172 2023-05-20 04:20:10.000000 foliolib-0.3.6a1/foliolib/folio/api/financeStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    51717 2023-05-20 04:20:10.000000 foliolib-0.3.6a1/foliolib/folio/api/fincConfig.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6999 2023-05-20 04:20:08.000000 foliolib-0.3.6a1/foliolib/folio/api/folioCustomFields.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1342 2023-05-20 04:20:08.000000 foliolib-0.3.6a1/foliolib/folio/api/folioSpringBase.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1787 2023-05-20 04:20:08.000000 foliolib-0.3.6a1/foliolib/folio/api/folioVertxLib.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8283 2023-05-20 04:20:10.000000 foliolib-0.3.6a1/foliolib/folio/api/gobi.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     7801 2023-05-20 04:20:10.000000 foliolib-0.3.6a1/foliolib/folio/api/idmConnect.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    74110 2023-05-20 04:20:28.000000 foliolib-0.3.6a1/foliolib/folio/api/innReach.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    22929 2023-05-20 04:20:28.000000 foliolib-0.3.6a1/foliolib/folio/api/inventory.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)   220610 2023-05-20 04:20:29.000000 foliolib-0.3.6a1/foliolib/folio/api/inventoryStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6001 2023-05-20 04:20:29.000000 foliolib-0.3.6a1/foliolib/folio/api/inventoryUpdate.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    45051 2023-05-20 04:20:29.000000 foliolib-0.3.6a1/foliolib/folio/api/invoice.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    47143 2023-05-20 04:20:29.000000 foliolib-0.3.6a1/foliolib/folio/api/invoiceStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    54294 2023-05-20 04:20:29.000000 foliolib-0.3.6a1/foliolib/folio/api/kbEbscoJava.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3051 2023-05-20 04:20:29.000000 foliolib-0.3.6a1/foliolib/folio/api/ldp.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1332 2023-05-20 04:20:29.000000 foliolib-0.3.6a1/foliolib/folio/api/licenses.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8538 2023-05-20 04:20:29.000000 foliolib-0.3.6a1/foliolib/folio/api/login.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4260 2023-05-20 04:20:29.000000 foliolib-0.3.6a1/foliolib/folio/api/loginSaml.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    17932 2023-05-20 04:20:29.000000 foliolib-0.3.6a1/foliolib/folio/api/marccat.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    20533 2023-05-20 04:20:30.000000 foliolib-0.3.6a1/foliolib/folio/api/metaStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8754 2023-05-20 04:20:30.000000 foliolib-0.3.6a1/foliolib/folio/api/notes.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8870 2023-05-20 04:20:30.000000 foliolib-0.3.6a1/foliolib/folio/api/notify.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    12105 2023-05-20 04:20:30.000000 foliolib-0.3.6a1/foliolib/folio/api/oaiPmh.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    63105 2023-05-20 04:20:30.000000 foliolib-0.3.6a1/foliolib/folio/api/orders.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    78262 2023-05-20 04:20:30.000000 foliolib-0.3.6a1/foliolib/folio/api/ordersStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4978 2023-05-20 04:20:30.000000 foliolib-0.3.6a1/foliolib/folio/api/organizations.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    45825 2023-05-20 04:20:30.000000 foliolib-0.3.6a1/foliolib/folio/api/organizationsStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3632 2023-05-20 04:20:30.000000 foliolib-0.3.6a1/foliolib/folio/api/passwordValidator.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5893 2023-05-20 04:20:30.000000 foliolib-0.3.6a1/foliolib/folio/api/patron.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    15601 2023-05-20 04:20:30.000000 foliolib-0.3.6a1/foliolib/folio/api/patronBlocks.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    14392 2023-05-20 04:20:30.000000 foliolib-0.3.6a1/foliolib/folio/api/permissions.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9093 2023-05-20 04:20:30.000000 foliolib-0.3.6a1/foliolib/folio/api/pubsub.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4214 2023-05-20 04:20:30.000000 foliolib-0.3.6a1/foliolib/folio/api/quickMarc.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    17165 2023-05-20 04:20:31.000000 foliolib-0.3.6a1/foliolib/folio/api/remoteStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    21731 2023-05-20 04:20:31.000000 foliolib-0.3.6a1/foliolib/folio/api/reservoir.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1928 2023-05-20 04:20:31.000000 foliolib-0.3.6a1/foliolib/folio/api/rtac.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    17672 2023-05-20 04:20:31.000000 foliolib-0.3.6a1/foliolib/folio/api/search.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      732 2023-05-20 04:20:31.000000 foliolib-0.3.6a1/foliolib/folio/api/sender.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5419 2023-05-20 04:20:31.000000 foliolib-0.3.6a1/foliolib/folio/api/settings.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    11215 2023-05-20 04:20:31.000000 foliolib-0.3.6a1/foliolib/folio/api/sharedIndex.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    23625 2023-05-20 04:20:31.000000 foliolib-0.3.6a1/foliolib/folio/api/sourceRecordManager.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    28052 2023-05-20 04:20:31.000000 foliolib-0.3.6a1/foliolib/folio/api/sourceRecordStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3187 2023-05-20 04:20:31.000000 foliolib-0.3.6a1/foliolib/folio/api/tags.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4091 2023-05-20 04:20:31.000000 foliolib-0.3.6a1/foliolib/folio/api/templateEngine.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      870 2023-05-20 04:20:31.000000 foliolib-0.3.6a1/foliolib/folio/api/userImport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    24002 2023-05-20 04:20:31.000000 foliolib-0.3.6a1/foliolib/folio/api/users.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    11127 2023-05-20 04:20:31.000000 foliolib-0.3.6a1/foliolib/folio/api/usersBl.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5803 2022-05-31 09:32:11.000000 foliolib-0.3.6a1/foliolib/folio/config.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8495 2021-02-25 09:49:29.000000 foliolib-0.3.6a1/foliolib/folio/dataImport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      436 2022-03-17 02:39:17.000000 foliolib-0.3.6a1/foliolib/folio/exceptions.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      945 2022-04-08 08:56:47.000000 foliolib-0.3.6a1/foliolib/folio/inventory.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    24355 2023-05-09 16:17:52.000000 foliolib-0.3.6a1/foliolib/folio/inventoryReferenceData.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9397 2023-05-20 07:12:08.000000 foliolib-0.3.6a1/foliolib/folio/users.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-29 06:17:20.421483 foliolib-0.3.6a1/foliolib/helper/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1207 2023-04-21 05:23:46.000000 foliolib-0.3.6a1/foliolib/helper/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9311 2023-04-21 05:23:46.000000 foliolib-0.3.6a1/foliolib/helper/database.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3636 2022-10-11 03:50:00.000000 foliolib-0.3.6a1/foliolib/helper/folio.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3055 2023-02-09 19:10:16.000000 foliolib-0.3.6a1/foliolib/helper/modules.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3935 2023-04-01 06:20:04.000000 foliolib-0.3.6a1/foliolib/helper/okapi.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6637 2023-05-27 07:21:39.000000 foliolib-0.3.6a1/foliolib/helper/platform.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1517 2022-10-11 03:48:54.000000 foliolib-0.3.6a1/foliolib/helper/tenant.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-29 06:17:20.421483 foliolib-0.3.6a1/foliolib/okapi/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    14520 2022-10-13 08:48:51.000000 foliolib-0.3.6a1/foliolib/okapi/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2399 2022-07-24 04:45:10.000000 foliolib-0.3.6a1/foliolib/okapi/exceptions.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    16267 2023-04-21 05:23:46.000000 foliolib-0.3.6a1/foliolib/okapi/kubeClient.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      542 2022-03-22 15:04:58.000000 foliolib-0.3.6a1/foliolib/okapi/misc.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    38800 2023-04-21 05:23:46.000000 foliolib-0.3.6a1/foliolib/okapi/okapiClient.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    10030 2023-02-02 10:53:21.000000 foliolib-0.3.6a1/foliolib/okapi/okapiModule.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    17123 2023-05-24 12:23:18.000000 foliolib-0.3.6a1/foliolib/okapi/okapiModuleKubernetes.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-29 06:17:20.409483 foliolib-0.3.6a1/foliolib.egg-info/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2459 2023-05-29 06:17:20.000000 foliolib-0.3.6a1/foliolib.egg-info/PKG-INFO
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3790 2023-05-29 06:17:20.000000 foliolib-0.3.6a1/foliolib.egg-info/SOURCES.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)        1 2023-05-29 06:17:20.000000 foliolib-0.3.6a1/foliolib.egg-info/dependency_links.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)       46 2023-05-29 06:17:20.000000 foliolib-0.3.6a1/foliolib.egg-info/entry_points.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      130 2023-05-29 06:17:20.000000 foliolib-0.3.6a1/foliolib.egg-info/requires.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      126 2023-05-29 06:17:20.000000 foliolib-0.3.6a1/foliolib.egg-info/top_level.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      305 2023-02-21 08:41:56.000000 foliolib-0.3.6a1/requirements.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1182 2023-05-29 06:17:20.421483 foliolib-0.3.6a1/setup.cfg
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      117 2022-10-11 12:39:31.000000 foliolib-0.3.6a1/setup.py
```

### Comparing `foliolib-0.3.5a1/COPYING` & `foliolib-0.3.6a1/COPYING`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/PKG-INFO` & `foliolib-0.3.6a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foliolib
-Version: 0.3.5a1
+Version: 0.3.6a1
 Summary: Okapi/Folio Manager and Library
 Home-page: https://github.com/tobi-weber/foliolib
 Author: Tobias Weber
 Author-email: tobi-weber@gmx.de
 License: GPL-3.0 License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `foliolib-0.3.5a1/README.rst` & `foliolib-0.3.6a1/README.rst`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/__init__.py` & `foliolib-0.3.6a1/foliolib/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/apiBuilder/build_api.py` & `foliolib-0.3.6a1/foliolib/apiBuilder/build_api.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/apiBuilder/cli.py` & `foliolib-0.3.6a1/foliolib/apiBuilder/cli.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/cli/__init__.py` & `foliolib-0.3.6a1/foliolib/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/cli/folio/__init__.py` & `foliolib-0.3.6a1/foliolib/cli/folio/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/cli/main.py` & `foliolib-0.3.6a1/foliolib/cli/main.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/cli/main_noauth.py` & `foliolib-0.3.6a1/foliolib/cli/main_noauth.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/cli/module.py` & `foliolib-0.3.6a1/foliolib/cli/module.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/cli/okapi.py` & `foliolib-0.3.6a1/foliolib/cli/okapi.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/cli/platform.py` & `foliolib-0.3.6a1/foliolib/cli/platform.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 def platform():
     """Commands to manage Folio platforms.
     """
 
 
 @platform.command()
 @click.argument("tenantid")
-@click.option("-p", "--platform", default="R3-2022-GA",
-              help="Path to platform directory, tgz file, zip file or platform version")
+@click.option("-p", "--platform", default="R1-2023-GA",
+              help="Platform version (e.g. R1-2023 or path to platform directory or platform tgz file")
 @click.option("-n", "--node", default=get_node(),
               help="node id", show_default=True)
 @click.option("-a", "--deployAsync",  help="", is_flag=True)
 @click.option("--loadSample",  help="", is_flag=True)
 @click.option("--loadReference",  help="", is_flag=True)
 @click.option(
     "--ignoreErrors", is_flag=True, help="Ignore errors during the install operation")
@@ -31,14 +31,15 @@
     "--no-npmSnapshot", is_flag=True, help="Not include NPM module snapshots")
 @click.option(
     "--no-preRelease", is_flag=True, help="Pre-releases should be considered for installation")
 @click.option(
     "--simulate", is_flag=True, help="Simulate the installation")
 def install(**kwargs):
     """Install a folio platform.
+    This can be called multiple times, to setup different tenants.
 
     TENANTID\ttenant id.
     """
     _kwargs = {}
     if kwargs["ignoreerrors"]:
         _kwargs["ignoreErrors"] = True
     if kwargs["simulate"]:
@@ -54,15 +55,15 @@
                      loadReference=kwargs["loadreference"],
                      deploy_async=kwargs["deployasync"],
                      **_kwargs)
 
 
 @platform.command()
 @click.option("-t", "--tenant", default="ALL",
-              help="Tenant id to upgrade. Default all tenants will be upgraded")
+              help="Tenant id to upgrade. Default all tenants will be upgraded, except the supertenant")
 @click.option("-p", "--platform", required=True,
               help="Path to platform directory, tgz file, zip file or platform version")
 @click.option("-n", "--node", default=get_node(),
               help="node id", show_default=True)
 @click.option("-a", "--deployAsync",  help="", is_flag=True)
 @click.option("-e", "--exclude",  help="Exclude module from upgrade, e.g. mod-authtoken",
               multiple=True)
@@ -74,14 +75,16 @@
     "--no-npmSnapshot", is_flag=True, help="Not include NPM module snapshots")
 @click.option(
     "--no-preRelease", is_flag=True, help="Pre-releases should be considered for installation")
 @click.option(
     "--simulate", is_flag=True, help="Simulate the installation")
 def upgrade(**kwargs):
     """Upgrade folio tenants.
+    It is recommended to unsecure okapi before upgrading.
+    It may be necessary to update okapi before.
     """
     _kwargs = {}
     if kwargs["ignoreerrors"]:
         _kwargs["ignoreErrors"] = True
     if kwargs["simulate"]:
         _kwargs["simulate"] = True
     if kwargs["no_invoke"]:
```

### Comparing `foliolib-0.3.5a1/foliolib/cli/server.py` & `foliolib-0.3.6a1/foliolib/cli/server.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/cli/tenant.py` & `foliolib-0.3.6a1/foliolib/cli/tenant.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/config.py` & `foliolib-0.3.6a1/foliolib/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,14 +280,17 @@
             self.__foliolibcfg["PullNode"]["host"] = "folio-registry.dev.folio.org"
             self.__foliolibcfg["PullNode"]["port"] = "443"
             self.__foliolibcfg["PullNode"]["ssl"] = str(True)
             self.__foliolibcfg["Cache"] = {}
             self.__foliolibcfg["Cache"]["descriptors"] = os.path.join(self.get_confdir(),
                                                                       "cache",
                                                                       "descriptors")
+            self.__foliolibcfg["Cache"]["platforms"] = os.path.join(self.get_confdir(),
+                                                                    "cache",
+                                                                    "platforms")
             self.__foliolibcfg["GitHub"] = {}
             self.__foliolibcfg["GitHub"]["access-token"] = ""
             with open(fpath, "w") as f:
                 self.__foliolibcfg.write(f)
         else:
             log.debug("%s already exists.", fpath)
```

### Comparing `foliolib-0.3.5a1/foliolib/exceptions.py` & `foliolib-0.3.6a1/foliolib/exceptions.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/__init__.py` & `foliolib-0.3.6a1/foliolib/folio/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/audit.py` & `foliolib-0.3.6a1/foliolib/folio/api/audit.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/authtoken.py` & `foliolib-0.3.6a1/foliolib/folio/api/authtoken.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/bulkOperations.py` & `foliolib-0.3.6a1/foliolib/folio/api/bulkOperations.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/calendar.py` & `foliolib-0.3.6a1/foliolib/folio/api/calendar.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/circulation.py` & `foliolib-0.3.6a1/foliolib/folio/api/circulation.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/circulationStorage.py` & `foliolib-0.3.6a1/foliolib/folio/api/circulationStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/configuration.py` & `foliolib-0.3.6a1/foliolib/folio/api/configuration.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/consortia.py` & `foliolib-0.3.6a1/foliolib/folio/api/consortia.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/copycat.py` & `foliolib-0.3.6a1/foliolib/folio/api/copycat.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/courses.py` & `foliolib-0.3.6a1/foliolib/folio/api/courses.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/dataExport.py` & `foliolib-0.3.6a1/foliolib/folio/api/dataExport.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/dataExportSpring.py` & `foliolib-0.3.6a1/foliolib/folio/api/dataExportSpring.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/dataExportWorker.py` & `foliolib-0.3.6a1/foliolib/folio/api/dataExportWorker.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/dataImport.py` & `foliolib-0.3.6a1/foliolib/folio/api/dataImport.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/dataImportConverterStorage.py` & `foliolib-0.3.6a1/foliolib/folio/api/dataImportConverterStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/diConverterStorage.py` & `foliolib-0.3.6a1/foliolib/folio/api/diConverterStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/ebsconet.py` & `foliolib-0.3.6a1/foliolib/folio/api/ebsconet.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/email.py` & `foliolib-0.3.6a1/foliolib/folio/api/email.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/entitiesLinks.py` & `foliolib-0.3.6a1/foliolib/folio/api/entitiesLinks.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/ermUsage.py` & `foliolib-0.3.6a1/foliolib/folio/api/ermUsage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/ermUsageHarvester.py` & `foliolib-0.3.6a1/foliolib/folio/api/ermUsageHarvester.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/eusageReports.py` & `foliolib-0.3.6a1/foliolib/folio/api/eusageReports.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/eventConfig.py` & `foliolib-0.3.6a1/foliolib/folio/api/eventConfig.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/feesfines.py` & `foliolib-0.3.6a1/foliolib/folio/api/feesfines.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/finance.py` & `foliolib-0.3.6a1/foliolib/folio/api/finance.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/financeStorage.py` & `foliolib-0.3.6a1/foliolib/folio/api/financeStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/fincConfig.py` & `foliolib-0.3.6a1/foliolib/folio/api/fincConfig.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/folioCustomFields.py` & `foliolib-0.3.6a1/foliolib/folio/api/folioCustomFields.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/folioSpringBase.py` & `foliolib-0.3.6a1/foliolib/folio/api/folioSpringBase.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/folioVertxLib.py` & `foliolib-0.3.6a1/foliolib/folio/api/folioVertxLib.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/gobi.py` & `foliolib-0.3.6a1/foliolib/folio/api/gobi.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/idmConnect.py` & `foliolib-0.3.6a1/foliolib/folio/api/idmConnect.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/innReach.py` & `foliolib-0.3.6a1/foliolib/folio/api/innReach.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/inventory.py` & `foliolib-0.3.6a1/foliolib/folio/api/inventory.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/inventoryStorage.py` & `foliolib-0.3.6a1/foliolib/folio/api/inventoryStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/inventoryUpdate.py` & `foliolib-0.3.6a1/foliolib/folio/api/inventoryUpdate.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/invoice.py` & `foliolib-0.3.6a1/foliolib/folio/api/invoice.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/invoiceStorage.py` & `foliolib-0.3.6a1/foliolib/folio/api/invoiceStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/kbEbscoJava.py` & `foliolib-0.3.6a1/foliolib/folio/api/kbEbscoJava.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/ldp.py` & `foliolib-0.3.6a1/foliolib/folio/api/ldp.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/licenses.py` & `foliolib-0.3.6a1/foliolib/folio/api/licenses.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/login.py` & `foliolib-0.3.6a1/foliolib/folio/api/login.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/loginSaml.py` & `foliolib-0.3.6a1/foliolib/folio/api/loginSaml.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/marccat.py` & `foliolib-0.3.6a1/foliolib/folio/api/marccat.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/metaStorage.py` & `foliolib-0.3.6a1/foliolib/folio/api/metaStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/notes.py` & `foliolib-0.3.6a1/foliolib/folio/api/notes.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/notify.py` & `foliolib-0.3.6a1/foliolib/folio/api/notify.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/oaiPmh.py` & `foliolib-0.3.6a1/foliolib/folio/api/oaiPmh.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/orders.py` & `foliolib-0.3.6a1/foliolib/folio/api/orders.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/ordersStorage.py` & `foliolib-0.3.6a1/foliolib/folio/api/ordersStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/organizations.py` & `foliolib-0.3.6a1/foliolib/folio/api/organizations.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/organizationsStorage.py` & `foliolib-0.3.6a1/foliolib/folio/api/organizationsStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/passwordValidator.py` & `foliolib-0.3.6a1/foliolib/folio/api/passwordValidator.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/patron.py` & `foliolib-0.3.6a1/foliolib/folio/api/patron.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/patronBlocks.py` & `foliolib-0.3.6a1/foliolib/folio/api/patronBlocks.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/permissions.py` & `foliolib-0.3.6a1/foliolib/folio/api/permissions.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/pubsub.py` & `foliolib-0.3.6a1/foliolib/folio/api/pubsub.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/quickMarc.py` & `foliolib-0.3.6a1/foliolib/folio/api/quickMarc.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/remoteStorage.py` & `foliolib-0.3.6a1/foliolib/folio/api/remoteStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/reservoir.py` & `foliolib-0.3.6a1/foliolib/folio/api/reservoir.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/rtac.py` & `foliolib-0.3.6a1/foliolib/folio/api/rtac.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/search.py` & `foliolib-0.3.6a1/foliolib/folio/api/search.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/sender.py` & `foliolib-0.3.6a1/foliolib/folio/api/sender.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/settings.py` & `foliolib-0.3.6a1/foliolib/folio/api/settings.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/sharedIndex.py` & `foliolib-0.3.6a1/foliolib/folio/api/sharedIndex.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/sourceRecordManager.py` & `foliolib-0.3.6a1/foliolib/folio/api/sourceRecordManager.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/sourceRecordStorage.py` & `foliolib-0.3.6a1/foliolib/folio/api/sourceRecordStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/tags.py` & `foliolib-0.3.6a1/foliolib/folio/api/tags.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/templateEngine.py` & `foliolib-0.3.6a1/foliolib/folio/api/templateEngine.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/userImport.py` & `foliolib-0.3.6a1/foliolib/folio/api/userImport.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/users.py` & `foliolib-0.3.6a1/foliolib/folio/api/users.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/api/usersBl.py` & `foliolib-0.3.6a1/foliolib/folio/api/usersBl.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/config.py` & `foliolib-0.3.6a1/foliolib/folio/config.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/dataImport.py` & `foliolib-0.3.6a1/foliolib/folio/dataImport.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/inventory.py` & `foliolib-0.3.6a1/foliolib/folio/inventory.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/inventoryReferenceData.py` & `foliolib-0.3.6a1/foliolib/folio/inventoryReferenceData.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/folio/users.py` & `foliolib-0.3.6a1/foliolib/folio/users.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/helper/__init__.py` & `foliolib-0.3.6a1/foliolib/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/helper/database.py` & `foliolib-0.3.6a1/foliolib/helper/database.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/helper/folio.py` & `foliolib-0.3.6a1/foliolib/helper/folio.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/helper/modules.py` & `foliolib-0.3.6a1/foliolib/helper/modules.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/helper/okapi.py` & `foliolib-0.3.6a1/foliolib/helper/okapi.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/helper/platform.py` & `foliolib-0.3.6a1/foliolib/helper/platform.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 import sys
 import tarfile
 import tempfile
 import zipfile
 
 import requests
+from foliolib.config import Config
 from foliolib.exceptions import FoliolibError
 from foliolib.helper import split_modid
 from foliolib.helper.modules import (add_modules, deploy_modules,
                                      deploy_modules_async, enable_modules,
                                      load_install_file)
 from foliolib.helper.okapi import clean_okapi
 from foliolib.okapi.okapiClient import OkapiClient
@@ -34,27 +35,38 @@
     elif platform.endswith(".zip"):
         print("platform is zipfile")
         with zipfile.ZipFile(platform, "r") as z:
             z.extractall(tmp)
             print(z.filelist())
             return "ZIP"
     else:
-        url = f"https://api.github.com/repos/folio-org/platform-complete/tags"
-        response = requests.get(url)
-        tags = response.json()
-        tarball_url = None
-        for t in tags:
-            if t["name"] == platform.strip():
-                tarball_url = t["tarball_url"]
-        if tarball_url is None:
-            raise FoliolibError("Unknown platform %s" % platform)
-        response = requests.get(tarball_url)
-        fname = os.path.join(tmp, "folio-platform.tar.gz")
-        with open(fname, "bw") as f:
-            f.write(response.content)
+        cache_dir = os.path.join(Config().foliolibcfg()[
+                                 "Cache"]["platforms"])
+        if not os.path.exists(cache_dir):
+            os.mkdir(cache_dir)
+        fname = os.path.join(cache_dir, f"folio-platform-{platform}.tar.gz")
+        if not os.path.exists(fname):
+            print("Download folio platform %s" % platform)
+            url = f"https://api.github.com/repos/folio-org/platform-complete/tags"
+            response = requests.get(url)
+            tags = response.json()
+            tarball_url = None
+            for t in tags:
+                if t["name"] == platform.strip():
+                    tarball_url = t["tarball_url"]
+            if tarball_url is None:
+                print("Available folio platforms:")
+                names = [t["name"] for t in tags]
+                for name in sorted(names):
+                    print(name)
+                raise FoliolibError("Unknown platform %s" % platform)
+            response = requests.get(tarball_url)
+            with open(fname, "bw") as f:
+                f.write(response.content)
+
         with tarfile.open(fname, "r:gz") as f:
             f.extractall(tmp)
             return os.path.join(tmp,
                                 f.getmembers()[0].name)
 
 
 def install_platform(platform: str, node: str, tenantid: str,
@@ -114,16 +126,22 @@
     Args:
         platform (str): Path to the folder of the folio platform.
         node (str): node id
         tenantid (str): tenant id
         loadSample (bool, optional): load samples. Defaults to False.
     """
     def upgrade(tid):
+        okapi = OkapiClient()
+        for m in okapi_modules:
+            if m.get_id().startswith("mod-authtoken"):
+                print("Upgrade %s for tenant %s" % (m.get_id(), tid))
+                msg = okapi.upgrade_modules(tid, [m.get_id()], invoke=False)
+                print(json.dumps(msg, indent=2))
         print("Upgrade modules for tenant %s ..." % tid)
-        msg = OkapiClient().upgrade_modules(tid, **kwargs)
+        msg = okapi.upgrade_modules(tid, **kwargs)
         print(json.dumps(msg, indent=2))
     platform = __process_platform(platform)
 
     okapi_install = os.path.join(platform, "okapi-install.json")
     okapi_modules = load_install_file(okapi_install)
     stripes_install = os.path.join(platform, "stripes-install.json")
     stripes_modules = load_install_file(stripes_install)
@@ -136,19 +154,21 @@
         for mod_name in exclude:
             stripes_modules = [m for m in stripes_modules
                                if not mod_name == split_modid(m.get_id())[0]]
             okapi_modules = [m for m in okapi_modules
                              if not mod_name == split_modid(m.get_id())[0]]
 
     add_modules(okapi_modules + stripes_modules)
+
     if deploy_async:
         deploy_modules_async(node, okapi_modules)
     else:
         deploy_modules(node, okapi_modules)
 
     if tenantid == "ALL":
         tenants = OkapiClient().get_tenants()
         for tenant in tenants:
-            upgrade(tenant["id"])
+            if not tenant["id"] == "supertenant":
+                upgrade(tenant["id"])
     else:
         upgrade(tenantid)
     clean_okapi()
```

### Comparing `foliolib-0.3.5a1/foliolib/helper/tenant.py` & `foliolib-0.3.6a1/foliolib/helper/tenant.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/okapi/__init__.py` & `foliolib-0.3.6a1/foliolib/okapi/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/okapi/exceptions.py` & `foliolib-0.3.6a1/foliolib/okapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/okapi/kubeClient.py` & `foliolib-0.3.6a1/foliolib/okapi/kubeClient.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/okapi/misc.py` & `foliolib-0.3.6a1/foliolib/okapi/misc.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/okapi/okapiClient.py` & `foliolib-0.3.6a1/foliolib/okapi/okapiClient.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/okapi/okapiModule.py` & `foliolib-0.3.6a1/foliolib/okapi/okapiModule.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/foliolib/okapi/okapiModuleKubernetes.py` & `foliolib-0.3.6a1/foliolib/okapi/okapiModuleKubernetes.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,21 +25,21 @@
         self._memory = docker_args["memory"]
         self._port = docker_args["port"]
         self._protocol = docker_args["protocol"]
         self._env = module.get_env()
         self.healthCheck = True
         self.podAntiAffinity = True
         modcfg = Config().modulescfg(modId)
-        okapicfg = Config().servercfg()
-        self._namespace = okapicfg.get(
-            "Kubernetes", "namespace", fallback="default")
-        self.imagePullSecret = okapicfg.get(
+        servercfg = Config().servercfg()
+        self._namespace = servercfg.get(
+            "Kubernetes", "namespace", fallback="folio")
+        self.imagePullSecret = servercfg.get(
             "Kubernetes", "imagePullSecret", fallback=None)
 
-        self._replicas = okapicfg.getint("Kubernetes", "replicas", fallback=1)
+        self._replicas = servercfg.getint("Kubernetes", "replicas", fallback=1)
 
         if self._modId.startswith("mod-authtoken"):
             self._replicas = 1
 
         if self._modId.startswith("mod-data-import"):
             self._replicas = 1
```

### Comparing `foliolib-0.3.5a1/foliolib.egg-info/PKG-INFO` & `foliolib-0.3.6a1/foliolib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foliolib
-Version: 0.3.5a1
+Version: 0.3.6a1
 Summary: Okapi/Folio Manager and Library
 Home-page: https://github.com/tobi-weber/foliolib
 Author: Tobias Weber
 Author-email: tobi-weber@gmx.de
 License: GPL-3.0 License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `foliolib-0.3.5a1/foliolib.egg-info/SOURCES.txt` & `foliolib-0.3.6a1/foliolib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.5a1/setup.cfg` & `foliolib-0.3.6a1/setup.cfg`

 * *Files identical despite different names*

