# Comparing `tmp/pingdatautil-0.0.3.tar.gz` & `tmp/pingdatautil-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pingdatautil-0.0.3.tar", last modified: Wed Apr 12 03:12:21 2023, max compression
+gzip compressed data, was "pingdatautil-0.0.4.tar", last modified: Mon May 29 06:15:08 2023, max compression
```

## Comparing `pingdatautil-0.0.3.tar` & `pingdatautil-0.0.4.tar`

### file list

```diff
@@ -1,47 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 03:12:21.235404 pingdatautil-0.0.3/
--rw-rw-rw-   0        0        0     1090 2023-04-02 15:02:53.000000 pingdatautil-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      331 2023-04-12 03:11:58.000000 pingdatautil-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      142 2023-04-12 03:12:21.234404 pingdatautil-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       59 2023-04-12 03:04:56.000000 pingdatautil-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 03:12:21.219642 pingdatautil-0.0.3/pingdatautil/
--rw-rw-rw-   0        0        0     6939 2023-04-02 17:34:55.000000 pingdatautil-0.0.3/pingdatautil/AzureStorage.py
--rw-rw-rw-   0        0        0     6272 2023-04-09 09:04:38.000000 pingdatautil-0.0.3/pingdatautil/DataConnection.py
--rw-rw-rw-   0        0        0    20872 2023-04-09 10:39:11.000000 pingdatautil-0.0.3/pingdatautil/DataExport.py
--rw-rw-rw-   0        0        0     2294 2023-04-02 15:51:17.000000 pingdatautil-0.0.3/pingdatautil/EngineHelper.py
--rw-rw-rw-   0        0        0     7118 2023-04-09 10:55:36.000000 pingdatautil-0.0.3/pingdatautil/ExcelFormatter.py
--rw-rw-rw-   0        0        0     6294 2023-04-02 16:21:41.000000 pingdatautil-0.0.3/pingdatautil/GoogleDrive.py
--rw-rw-rw-   0        0        0     5602 2023-04-02 16:20:58.000000 pingdatautil-0.0.3/pingdatautil/GoogleSheet.py
--rw-rw-rw-   0        0        0    22769 2023-04-07 07:52:34.000000 pingdatautil-0.0.3/pingdatautil/HyperClass.py
--rw-rw-rw-   0        0        0     8710 2023-04-02 17:03:36.000000 pingdatautil-0.0.3/pingdatautil/JDBCExport.py
--rw-rw-rw-   0        0        0     4187 2023-04-02 16:59:49.000000 pingdatautil-0.0.3/pingdatautil/JDBCHelper.py
--rw-rw-rw-   0        0        0     2291 2023-04-02 15:47:17.000000 pingdatautil-0.0.3/pingdatautil/LineNotify.py
--rw-rw-rw-   0        0        0     4087 2023-04-02 15:47:31.000000 pingdatautil-0.0.3/pingdatautil/Logger.py
--rw-rw-rw-   0        0        0    15750 2023-04-02 16:44:54.000000 pingdatautil-0.0.3/pingdatautil/ODBCExport.py
--rw-rw-rw-   0        0        0     3756 2023-04-09 08:31:37.000000 pingdatautil-0.0.3/pingdatautil/ODBCHelper.py
--rw-rw-rw-   0        0        0     3835 2023-04-10 02:37:54.000000 pingdatautil-0.0.3/pingdatautil/ODBCHelper1.py
--rw-rw-rw-   0        0        0    14299 2023-04-11 09:13:14.000000 pingdatautil-0.0.3/pingdatautil/UnitTest.py
--rw-rw-rw-   0        0        0      484 2023-04-10 02:36:27.000000 pingdatautil-0.0.3/pingdatautil/_LogUtil.py
--rw-rw-rw-   0        0        0      566 2023-04-11 07:58:05.000000 pingdatautil-0.0.3/pingdatautil/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 03:12:21.224926 pingdatautil-0.0.3/pingdatautil.egg-info/
--rw-rw-rw-   0        0        0      142 2023-04-12 03:12:21.000000 pingdatautil-0.0.3/pingdatautil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      985 2023-04-12 03:12:21.000000 pingdatautil-0.0.3/pingdatautil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 03:12:21.000000 pingdatautil-0.0.3/pingdatautil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-04-12 03:12:21.000000 pingdatautil-0.0.3/pingdatautil.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-12 03:12:21.000000 pingdatautil-0.0.3/pingdatautil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 03:12:21.235404 pingdatautil-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      365 2023-04-12 03:09:33.000000 pingdatautil-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 03:12:21.233399 pingdatautil-0.0.3/test/
--rw-rw-rw-   0        0        0      903 2023-04-09 08:49:13.000000 pingdatautil-0.0.3/test/test-data-connection.py
--rw-rw-rw-   0        0        0      503 2023-04-09 09:58:44.000000 pingdatautil-0.0.3/test/test-data-export-2.py
--rw-rw-rw-   0        0        0      661 2023-04-11 03:47:54.000000 pingdatautil-0.0.3/test/test-data-export-jdbc.py
--rw-rw-rw-   0        0        0     1246 2023-04-10 04:00:25.000000 pingdatautil-0.0.3/test/test-data-export.py
--rw-rw-rw-   0        0        0      557 2023-04-11 03:48:18.000000 pingdatautil-0.0.3/test/test-excel-format.py
--rw-rw-rw-   0        0        0      414 2023-04-07 07:38:37.000000 pingdatautil-0.0.3/test/test-hyper1.py
--rw-rw-rw-   0        0        0      958 2023-04-02 17:22:59.000000 pingdatautil-0.0.3/test/test-hyper2.py
--rw-rw-rw-   0        0        0      756 2023-04-05 07:30:16.000000 pingdatautil-0.0.3/test/test1.py
--rw-rw-rw-   0        0        0      356 2023-04-07 02:52:52.000000 pingdatautil-0.0.3/test/test1a.py
--rw-rw-rw-   0        0        0      428 2023-04-09 11:53:27.000000 pingdatautil-0.0.3/test/test1m.py
--rw-rw-rw-   0        0        0      779 2023-04-03 04:07:43.000000 pingdatautil-0.0.3/test/test2.py
--rw-rw-rw-   0        0        0     1375 2023-04-02 17:35:00.000000 pingdatautil-0.0.3/test/test3.py
--rw-rw-rw-   0        0        0      276 2023-04-05 07:30:30.000000 pingdatautil-0.0.3/test/test4.py
--rw-rw-rw-   0        0        0      123 2023-04-10 02:30:50.000000 pingdatautil-0.0.3/test/test5.py
+drwxrwxrwx   0        0        0        0 2023-05-29 06:15:08.271664 pingdatautil-0.0.4/
+-rw-rw-rw-   0        0        0     1090 2023-04-02 15:02:53.000000 pingdatautil-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      329 2023-04-12 03:30:14.000000 pingdatautil-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      142 2023-05-29 06:15:08.270316 pingdatautil-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2023-04-12 03:04:56.000000 pingdatautil-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 06:15:08.266417 pingdatautil-0.0.4/pingdatautil/
+-rw-rw-rw-   0        0        0     6939 2023-04-02 17:34:55.000000 pingdatautil-0.0.4/pingdatautil/AzureStorage.py
+-rw-rw-rw-   0        0        0     6272 2023-04-12 03:37:18.000000 pingdatautil-0.0.4/pingdatautil/DataConnection.py
+-rw-rw-rw-   0        0        0    20872 2023-04-09 10:39:11.000000 pingdatautil-0.0.4/pingdatautil/DataExport.py
+-rw-rw-rw-   0        0        0     2294 2023-04-02 15:51:17.000000 pingdatautil-0.0.4/pingdatautil/EngineHelper.py
+-rw-rw-rw-   0        0        0     7118 2023-04-09 10:55:36.000000 pingdatautil-0.0.4/pingdatautil/ExcelFormatter.py
+-rw-rw-rw-   0        0        0     6294 2023-04-02 16:21:41.000000 pingdatautil-0.0.4/pingdatautil/GoogleDrive.py
+-rw-rw-rw-   0        0        0     5602 2023-04-02 16:20:58.000000 pingdatautil-0.0.4/pingdatautil/GoogleSheet.py
+-rw-rw-rw-   0        0        0     2553 2023-05-29 06:10:01.000000 pingdatautil-0.0.4/pingdatautil/GoogleStorage.py
+-rw-rw-rw-   0        0        0    22769 2023-04-07 07:52:34.000000 pingdatautil-0.0.4/pingdatautil/HyperClass.py
+-rw-rw-rw-   0        0        0     8710 2023-04-02 17:03:36.000000 pingdatautil-0.0.4/pingdatautil/JDBCExport.py
+-rw-rw-rw-   0        0        0     4187 2023-04-02 16:59:49.000000 pingdatautil-0.0.4/pingdatautil/JDBCHelper.py
+-rw-rw-rw-   0        0        0     2291 2023-04-02 15:47:17.000000 pingdatautil-0.0.4/pingdatautil/LineNotify.py
+-rw-rw-rw-   0        0        0     4087 2023-04-02 15:47:31.000000 pingdatautil-0.0.4/pingdatautil/Logger.py
+-rw-rw-rw-   0        0        0    15750 2023-04-02 16:44:54.000000 pingdatautil-0.0.4/pingdatautil/ODBCExport.py
+-rw-rw-rw-   0        0        0     3756 2023-04-09 08:31:37.000000 pingdatautil-0.0.4/pingdatautil/ODBCHelper.py
+-rw-rw-rw-   0        0        0    14299 2023-04-11 09:13:14.000000 pingdatautil-0.0.4/pingdatautil/UnitTest.py
+-rw-rw-rw-   0        0        0      482 2023-04-12 03:36:51.000000 pingdatautil-0.0.4/pingdatautil/_Util.py
+-rw-rw-rw-   0        0        0      566 2023-04-11 07:58:05.000000 pingdatautil-0.0.4/pingdatautil/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 06:15:08.270316 pingdatautil-0.0.4/pingdatautil.egg-info/
+-rw-rw-rw-   0        0        0      142 2023-05-29 06:15:08.000000 pingdatautil-0.0.4/pingdatautil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2023-05-29 06:15:08.000000 pingdatautil-0.0.4/pingdatautil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 06:15:08.000000 pingdatautil-0.0.4/pingdatautil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-29 06:15:08.000000 pingdatautil-0.0.4/pingdatautil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-29 06:15:08.000000 pingdatautil-0.0.4/pingdatautil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 06:15:08.271664 pingdatautil-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      409 2023-05-29 06:13:54.000000 pingdatautil-0.0.4/setup.py
```

### Comparing `pingdatautil-0.0.3/LICENSE` & `pingdatautil-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.3/pingdatautil/AzureStorage.py` & `pingdatautil-0.0.4/pingdatautil/AzureStorage.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.3/pingdatautil/DataConnection.py` & `pingdatautil-0.0.4/pingdatautil/DataConnection.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.3/pingdatautil/DataExport.py` & `pingdatautil-0.0.4/pingdatautil/DataExport.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.3/pingdatautil/EngineHelper.py` & `pingdatautil-0.0.4/pingdatautil/EngineHelper.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.3/pingdatautil/ExcelFormatter.py` & `pingdatautil-0.0.4/pingdatautil/ExcelFormatter.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.3/pingdatautil/GoogleDrive.py` & `pingdatautil-0.0.4/pingdatautil/GoogleDrive.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.3/pingdatautil/GoogleSheet.py` & `pingdatautil-0.0.4/pingdatautil/GoogleSheet.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.3/pingdatautil/HyperClass.py` & `pingdatautil-0.0.4/pingdatautil/HyperClass.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.3/pingdatautil/JDBCExport.py` & `pingdatautil-0.0.4/pingdatautil/JDBCExport.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.3/pingdatautil/JDBCHelper.py` & `pingdatautil-0.0.4/pingdatautil/JDBCHelper.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.3/pingdatautil/LineNotify.py` & `pingdatautil-0.0.4/pingdatautil/LineNotify.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.3/pingdatautil/Logger.py` & `pingdatautil-0.0.4/pingdatautil/Logger.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.3/pingdatautil/ODBCExport.py` & `pingdatautil-0.0.4/pingdatautil/ODBCExport.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.3/pingdatautil/ODBCHelper.py` & `pingdatautil-0.0.4/pingdatautil/ODBCHelper.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.3/pingdatautil/UnitTest.py` & `pingdatautil-0.0.4/pingdatautil/UnitTest.py`

 * *Files identical despite different names*

### Comparing `pingdatautil-0.0.3/pingdatautil/__init__.py` & `pingdatautil-0.0.4/pingdatautil/__init__.py`

 * *Files identical despite different names*

