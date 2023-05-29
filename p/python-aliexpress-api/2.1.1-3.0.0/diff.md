# Comparing `tmp/python-aliexpress-api-2.1.1.tar.gz` & `tmp/python-aliexpress-api-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-aliexpress-api-2.1.1.tar", last modified: Sat Nov 20 11:16:44 2021, max compression
+gzip compressed data, was "python-aliexpress-api-3.0.0.tar", last modified: Mon May 29 18:43:02 2023, max compression
```

## Comparing `python-aliexpress-api-2.1.1.tar` & `python-aliexpress-api-3.0.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-20 11:16:44.912442 python-aliexpress-api-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2857 2021-11-20 11:16:44.912442 python-aliexpress-api-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2367 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-20 11:16:44.908442 python-aliexpress-api-2.1.1/aliexpress_api/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10117 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-20 11:16:44.908442 python-aliexpress-api-2.1.1/aliexpress_api/errors/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/errors/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-20 11:16:44.908442 python-aliexpress-api-2.1.1/aliexpress_api/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)      204 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      754 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/helpers/arguments.py
--rw-r--r--   0 runner    (1001) docker     (121)      800 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/helpers/categories.py
--rw-r--r--   0 runner    (1001) docker     (121)      287 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/helpers/products.py
--rw-r--r--   0 runner    (1001) docker     (121)      857 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/helpers/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-20 11:16:44.908442 python-aliexpress-api-2.1.1/aliexpress_api/models/
--rw-r--r--   0 runner    (1001) docker     (121)      289 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/models/affiliate_link.py
--rw-r--r--   0 runner    (1001) docker     (121)      121 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/models/category.py
--rw-r--r--   0 runner    (1001) docker     (121)      256 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/models/currencies.py
--rw-r--r--   0 runner    (1001) docker     (121)      193 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/models/hotproducts.py
--rw-r--r--   0 runner    (1001) docker     (121)      310 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/models/languages.py
--rw-r--r--   0 runner    (1001) docker     (121)      968 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/models/product.py
--rw-r--r--   0 runner    (1001) docker     (121)      298 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/models/request_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-20 11:16:44.908442 python-aliexpress-api-2.1.1/aliexpress_api/skd/
--rw-r--r--   0 runner    (1001) docker     (121)      375 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/skd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-20 11:16:44.908442 python-aliexpress-api-2.1.1/aliexpress_api/skd/api/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/skd/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10619 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/skd/api/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-20 11:16:44.912442 python-aliexpress-api-2.1.1/aliexpress_api/skd/api/rest/
--rw-r--r--   0 runner    (1001) docker     (121)      314 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/skd/api/rest/AliexpressAffiliateCategoryGetRequest.py
--rw-r--r--   0 runner    (1001) docker     (121)      345 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/skd/api/rest/AliexpressAffiliateFeaturedpromoGetRequest.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/skd/api/rest/AliexpressAffiliateFeaturedpromoProductsGetRequest.py
--rw-r--r--   0 runner    (1001) docker     (121)      555 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/skd/api/rest/AliexpressAffiliateHotproductDownloadRequest.py
--rw-r--r--   0 runner    (1001) docker     (121)      696 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/skd/api/rest/AliexpressAffiliateHotproductQueryRequest.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/skd/api/rest/AliexpressAffiliateLinkGenerateRequest.py
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/skd/api/rest/AliexpressAffiliateOrderGetRequest.py
--rw-r--r--   0 runner    (1001) docker     (121)      472 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/skd/api/rest/AliexpressAffiliateOrderListRequest.py
--rw-r--r--   0 runner    (1001) docker     (121)      473 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/skd/api/rest/AliexpressAffiliateOrderListbyindexRequest.py
--rw-r--r--   0 runner    (1001) docker     (121)      690 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/skd/api/rest/AliexpressAffiliateProductQueryRequest.py
--rw-r--r--   0 runner    (1001) docker     (121)      626 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/skd/api/rest/AliexpressAffiliateProductSmartmatchRequest.py
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/skd/api/rest/AliexpressAffiliateProductdetailGetRequest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/skd/api/rest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-20 11:16:44.912442 python-aliexpress-api-2.1.1/aliexpress_api/tools/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      522 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/aliexpress_api/tools/get_product_id.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-20 11:16:44.912442 python-aliexpress-api-2.1.1/python_aliexpress_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2857 2021-11-20 11:16:44.000000 python-aliexpress-api-2.1.1/python_aliexpress_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1919 2021-11-20 11:16:44.000000 python-aliexpress-api-2.1.1/python_aliexpress_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-20 11:16:44.000000 python-aliexpress-api-2.1.1/python_aliexpress_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-11-20 11:16:44.000000 python-aliexpress-api-2.1.1/python_aliexpress_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-11-20 11:16:44.000000 python-aliexpress-api-2.1.1/python_aliexpress_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-20 11:16:44.912442 python-aliexpress-api-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      729 2021-11-20 11:16:35.000000 python-aliexpress-api-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:43:02.009710 python-aliexpress-api-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-29 18:43:02.009710 python-aliexpress-api-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:43:02.005710 python-aliexpress-api-3.0.0/aliexpress_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:43:02.005710 python-aliexpress-api-3.0.0/aliexpress_api/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/errors/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:43:02.005710 python-aliexpress-api-3.0.0/aliexpress_api/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/helpers/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/helpers/categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/helpers/products.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/helpers/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:43:02.005710 python-aliexpress-api-3.0.0/aliexpress_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/models/affiliate_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/models/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/models/currencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/models/hotproducts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/models/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/models/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/models/request_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:43:02.009710 python-aliexpress-api-3.0.0/aliexpress_api/skd/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/skd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:43:02.009710 python-aliexpress-api-3.0.0/aliexpress_api/skd/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/skd/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11042 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/skd/api/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:43:02.009710 python-aliexpress-api-3.0.0/aliexpress_api/skd/api/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/skd/api/rest/AliexpressAffiliateCategoryGetRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/skd/api/rest/AliexpressAffiliateFeaturedpromoGetRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/skd/api/rest/AliexpressAffiliateFeaturedpromoProductsGetRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/skd/api/rest/AliexpressAffiliateHotproductDownloadRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/skd/api/rest/AliexpressAffiliateHotproductQueryRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/skd/api/rest/AliexpressAffiliateLinkGenerateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/skd/api/rest/AliexpressAffiliateOrderGetRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/skd/api/rest/AliexpressAffiliateOrderListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/skd/api/rest/AliexpressAffiliateOrderListbyindexRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/skd/api/rest/AliexpressAffiliateProductQueryRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/skd/api/rest/AliexpressAffiliateProductSmartmatchRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/skd/api/rest/AliexpressAffiliateProductdetailGetRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/skd/api/rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:43:02.009710 python-aliexpress-api-3.0.0/aliexpress_api/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/aliexpress_api/tools/get_product_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:43:02.009710 python-aliexpress-api-3.0.0/python_aliexpress_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-29 18:43:01.000000 python-aliexpress-api-3.0.0/python_aliexpress_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-29 18:43:01.000000 python-aliexpress-api-3.0.0/python_aliexpress_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 18:43:01.000000 python-aliexpress-api-3.0.0/python_aliexpress_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 18:43:01.000000 python-aliexpress-api-3.0.0/python_aliexpress_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-29 18:43:01.000000 python-aliexpress-api-3.0.0/python_aliexpress_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 18:43:02.009710 python-aliexpress-api-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-29 18:42:50.000000 python-aliexpress-api-3.0.0/setup.py
```

### Comparing `python-aliexpress-api-2.1.1/LICENSE` & `python-aliexpress-api-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-aliexpress-api-2.1.1/PKG-INFO` & `python-aliexpress-api-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: python-aliexpress-api
-Version: 2.1.1
+Version: 3.0.0
 Summary: AliExpress API wrapper for Python
 Home-page: https://github.com/sergioteula/python-aliexpress-api
 Author: Sergio Abad
 Author-email: sergio.abad@bytelix.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -72,9 +71,7 @@
 parent_categories = aliexpress.get_parent_categories()
 child_categories = aliexpress.get_child_categories(parent_categories[0].category_id)
 ```
 
 ## License
 
 Copyright © 2020 Sergio Abad. See [license](https://github.com/sergioteula/python-aliexpress-api/blob/master/LICENSE) for details.
-
-
```

### Comparing `python-aliexpress-api-2.1.1/README.md` & `python-aliexpress-api-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `python-aliexpress-api-2.1.1/aliexpress_api/api.py` & `python-aliexpress-api-3.0.0/aliexpress_api/api.py`

 * *Files identical despite different names*

### Comparing `python-aliexpress-api-2.1.1/aliexpress_api/errors/exceptions.py` & `python-aliexpress-api-3.0.0/aliexpress_api/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-aliexpress-api-2.1.1/aliexpress_api/helpers/arguments.py` & `python-aliexpress-api-3.0.0/aliexpress_api/helpers/arguments.py`

 * *Files identical despite different names*

### Comparing `python-aliexpress-api-2.1.1/aliexpress_api/helpers/categories.py` & `python-aliexpress-api-3.0.0/aliexpress_api/helpers/categories.py`

 * *Files identical despite different names*

### Comparing `python-aliexpress-api-2.1.1/aliexpress_api/helpers/requests.py` & `python-aliexpress-api-3.0.0/aliexpress_api/helpers/requests.py`

 * *Files identical despite different names*

### Comparing `python-aliexpress-api-2.1.1/aliexpress_api/models/product.py` & `python-aliexpress-api-3.0.0/aliexpress_api/models/product.py`

 * *Files identical despite different names*

### Comparing `python-aliexpress-api-2.1.1/aliexpress_api/skd/api/base.py` & `python-aliexpress-api-3.0.0/aliexpress_api/skd/api/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,295 +1,332 @@
 # -*- coding: utf-8 -*-
-'''
+"""
 Created on 2012-7-3
 
 @author: lihao
-'''
+"""
 
 
-import http.client as httplib
-import urllib
-import time
 import hashlib
-import json
+import http.client as httplib
 import itertools
+import json
 import mimetypes
+import time
+import urllib
 
-'''
+"""
 定义一些系统变量
-'''
+"""
 
 SYSTEM_GENERATE_VERSION = "taobao-sdk-python-20200924"
 
 P_APPKEY = "app_key"
 P_API = "method"
 P_SESSION = "session"
 P_ACCESS_TOKEN = "access_token"
 P_VERSION = "v"
 P_FORMAT = "format"
 P_TIMESTAMP = "timestamp"
 P_SIGN = "sign"
 P_SIGN_METHOD = "sign_method"
 P_PARTNER_ID = "partner_id"
 
-P_CODE = 'code'
-P_SUB_CODE = 'sub_code'
-P_MSG = 'msg'
-P_SUB_MSG = 'sub_msg'
+P_CODE = "code"
+P_SUB_CODE = "sub_code"
+P_MSG = "msg"
+P_SUB_MSG = "sub_msg"
+
 
+N_REST = "/sync"
 
-N_REST = '/router/rest'
 
 def sign(secret, parameters):
-    #===========================================================================
+    # ===========================================================================
     # '''签名方法
     # @param secret: 签名需要的密钥
     # @param parameters: 支持字典和string两种
     # '''
-    #===========================================================================
+    # ===========================================================================
     # 如果parameters 是字典类的话
     if hasattr(parameters, "items"):
         keys = parameters.keys()
         keys = list(keys)
         keys.sort()
 
-        parameters = "%s%s%s" % (secret,
-            str().join('%s%s' % (key, parameters[key]) for key in keys),
-            secret)
-    parameters = parameters.encode('utf-8')
+        parameters = "%s%s%s" % (
+            secret,
+            str().join("%s%s" % (key, parameters[key]) for key in keys),
+            secret,
+        )
+    parameters = parameters.encode("utf-8")
     sign = hashlib.md5(parameters).hexdigest().upper()
     return sign
 
+
 def mixStr(pstr):
-    if(isinstance(pstr, str)):
+    if isinstance(pstr, str):
         return pstr
-    elif(isinstance(pstr, str)):
-        return pstr.encode('utf-8')
+    elif isinstance(pstr, str):
+        return pstr.encode("utf-8")
     else:
         return str(pstr)
 
+
 class FileItem(object):
-    def __init__(self,filename=None,content=None):
+    def __init__(self, filename=None, content=None):
         self.filename = filename
         self.content = content
 
+
 class MultiPartForm(object):
     """Accumulate the data to be used when posting a form."""
 
     def __init__(self):
         self.form_fields = []
         self.files = []
         self.boundary = "PYTHON_SDK_BOUNDARY"
         return
 
     def get_content_type(self):
-        return 'multipart/form-data; boundary=%s' % self.boundary
+        return "multipart/form-data; boundary=%s" % self.boundary
 
     def add_field(self, name, value):
         """Add a simple field to the form data."""
         self.form_fields.append((name, str(value)))
         return
 
     def add_file(self, fieldname, filename, fileHandle, mimetype=None):
         """Add a file to be uploaded."""
         body = fileHandle.read()
         if mimetype is None:
-            mimetype = mimetypes.guess_type(filename)[0] or 'application/octet-stream'
-        self.files.append((mixStr(fieldname), mixStr(filename), mixStr(mimetype), mixStr(body)))
+            mimetype = mimetypes.guess_type(filename)[0] or "application/octet-stream"
+        self.files.append(
+            (mixStr(fieldname), mixStr(filename), mixStr(mimetype), mixStr(body))
+        )
         return
 
     def __str__(self):
         """Return a string representing the form data, including attached files."""
         # Build a list of lists, each containing "lines" of the
         # request.  Each part is separated by a boundary string.
         # Once the list is built, return a string where each
         # line is separated by '\r\n'.
         parts = []
-        part_boundary = '--' + self.boundary
+        part_boundary = "--" + self.boundary
 
         # Add the form fields
         parts.extend(
-            [ part_boundary,
-              'Content-Disposition: form-data; name="%s"' % name,
-              'Content-Type: text/plain; charset=UTF-8',
-              '',
-              value,
+            [
+                part_boundary,
+                'Content-Disposition: form-data; name="%s"' % name,
+                "Content-Type: text/plain; charset=UTF-8",
+                "",
+                value,
             ]
             for name, value in self.form_fields
-            )
+        )
 
         # Add the files to upload
         parts.extend(
-            [ part_boundary,
-              'Content-Disposition: file; name="%s"; filename="%s"' % \
-                 (field_name, filename),
-              'Content-Type: %s' % content_type,
-              'Content-Transfer-Encoding: binary',
-              '',
-              body,
+            [
+                part_boundary,
+                'Content-Disposition: file; name="%s"; filename="%s"'
+                % (field_name, filename),
+                "Content-Type: %s" % content_type,
+                "Content-Transfer-Encoding: binary",
+                "",
+                body,
             ]
             for field_name, filename, content_type, body in self.files
-            )
+        )
 
         # Flatten the list and add closing boundary marker,
         # then return CR+LF separated data
         flattened = list(itertools.chain(*parts))
-        flattened.append('--' + self.boundary + '--')
-        flattened.append('')
-        return '\r\n'.join(flattened)
+        flattened.append("--" + self.boundary + "--")
+        flattened.append("")
+        return "\r\n".join(flattened)
+
 
 class TopException(Exception):
-    #===========================================================================
+    # ===========================================================================
     # 业务异常类
-    #===========================================================================
+    # ===========================================================================
     def __init__(self):
         self.errorcode = None
         self.message = None
         self.subcode = None
         self.submsg = None
         self.application_host = None
         self.service_host = None
 
     def __str__(self, *args, **kwargs):
-        sb = "errorcode=" + mixStr(self.errorcode) +\
-            " message=" + mixStr(self.message) +\
-            " subcode=" + mixStr(self.subcode) +\
-            " submsg=" + mixStr(self.submsg) +\
-            " application_host=" + mixStr(self.application_host) +\
-            " service_host=" + mixStr(self.service_host)
+        sb = (
+            "errorcode="
+            + mixStr(self.errorcode)
+            + " message="
+            + mixStr(self.message)
+            + " subcode="
+            + mixStr(self.subcode)
+            + " submsg="
+            + mixStr(self.submsg)
+            + " application_host="
+            + mixStr(self.application_host)
+            + " service_host="
+            + mixStr(self.service_host)
+        )
         return sb
 
+
 class RequestException(Exception):
-    #===========================================================================
+    # ===========================================================================
     # 请求连接异常类
-    #===========================================================================
+    # ===========================================================================
     pass
 
+
 class RestApi(object):
-    #===========================================================================
+    # ===========================================================================
     # Rest api的基类
-    #===========================================================================
+    # ===========================================================================
 
-    def __init__(self, domain='gw.api.taobao.com', port = 80):
-        #=======================================================================
+    def __init__(self, domain="api-sg.aliexpress.com", port=80):
+        # =======================================================================
         # 初始化基类
         # Args @param domain: 请求的域名或者ip
         #      @param port: 请求的端口
-        #=======================================================================
+        # =======================================================================
         self.__domain = domain
         self.__port = port
         self.__httpmethod = "POST"
         from .. import getDefaultAppInfo
-        if(getDefaultAppInfo()):
+
+        if getDefaultAppInfo():
             self.__app_key = getDefaultAppInfo().appkey
             self.__secret = getDefaultAppInfo().secret
 
     def get_request_header(self):
         return {
-                 'Content-type': 'application/x-www-form-urlencoded;charset=UTF-8',
-                 "Cache-Control": "no-cache",
-                 "Connection": "Keep-Alive",
+            "Content-type": "application/x-www-form-urlencoded;charset=UTF-8",
+            "Cache-Control": "no-cache",
+            "Connection": "Keep-Alive",
         }
 
     def set_app_info(self, appinfo):
-        #=======================================================================
+        # =======================================================================
         # 设置请求的app信息
         # @param appinfo: import top
         #                 appinfo aliexpress.top.appinfo(appkey,secret)
-        #=======================================================================
+        # =======================================================================
         self.__app_key = appinfo.appkey
         self.__secret = appinfo.secret
 
     def getapiname(self):
         return ""
 
     def getMultipartParas(self):
-        return [];
+        return []
 
     def getTranslateParas(self):
-        return {};
+        return {}
 
     def _check_requst(self):
         pass
 
     def getResponse(self, authrize=None, timeout=30):
-        #=======================================================================
+        # =======================================================================
         # 获取response结果
-        #=======================================================================
-        if(self.__port == 443):
-            connection = httplib.HTTPSConnection(self.__domain, self.__port, timeout=timeout)
+        # =======================================================================
+        if self.__port == 443:
+            connection = httplib.HTTPSConnection(
+                self.__domain, self.__port, timeout=timeout
+            )
         else:
-            connection = httplib.HTTPConnection(self.__domain, self.__port, timeout=timeout)
+            connection = httplib.HTTPConnection(
+                self.__domain, self.__port, timeout=timeout
+            )
         timestamp_temp = "%.2f" % (float(time.time()))
         timestamp_temp = str(int(float(timestamp_temp) * 1000))
 
         sys_parameters = {
-            P_FORMAT: 'json',
+            P_FORMAT: "json",
             P_APPKEY: self.__app_key,
             P_SIGN_METHOD: "md5",
-            P_VERSION: '2.0',
+            P_VERSION: "2.0",
             P_TIMESTAMP: timestamp_temp,
             P_PARTNER_ID: SYSTEM_GENERATE_VERSION,
             P_API: self.getapiname(),
         }
         if authrize is not None:
             sys_parameters[P_SESSION] = authrize
         application_parameter = self.getApplicationParameters()
         sign_parameter = sys_parameters.copy()
         sign_parameter.update(application_parameter)
         sys_parameters[P_SIGN] = sign(self.__secret, sign_parameter)
         connection.connect()
 
-        header = self.get_request_header();
-        if(self.getMultipartParas()):
+        header = self.get_request_header()
+        if self.getMultipartParas():
             form = MultiPartForm()
             for key, value in application_parameter.items():
                 form.add_field(key, value)
             for key in self.getMultipartParas():
-                fileitem = getattr(self,key)
-                if(fileitem and isinstance(fileitem,FileItem)):
-                    form.add_file(key,fileitem.filename,fileitem.content)
+                fileitem = getattr(self, key)
+                if fileitem and isinstance(fileitem, FileItem):
+                    form.add_file(key, fileitem.filename, fileitem.content)
             body = str(form)
-            header['Content-type'] = form.get_content_type()
+            header["Content-type"] = form.get_content_type()
         else:
             body = urllib.parse.urlencode(application_parameter)
 
         url = N_REST + "?" + urllib.parse.urlencode(sys_parameters)
         connection.request(self.__httpmethod, url, body=body, headers=header)
-        response = connection.getresponse();
+        response = connection.getresponse()
         if response.status != 200:
-            raise RequestException('invalid http status ' + str(response.status) + ',detail body:' + response.read())
+            raise RequestException(
+                "invalid http status "
+                + str(response.status)
+                + ",detail body:"
+                + response.read()
+            )
         result = response.read()
         jsonobj = json.loads(result)
         if "error_response" in jsonobj:
             error = TopException()
-            if P_CODE in jsonobj["error_response"] :
+            if P_CODE in jsonobj["error_response"]:
                 error.errorcode = jsonobj["error_response"][P_CODE]
-            if P_MSG in jsonobj["error_response"] :
+            if P_MSG in jsonobj["error_response"]:
                 error.message = jsonobj["error_response"][P_MSG]
-            if P_SUB_CODE in jsonobj["error_response"] :
+            if P_SUB_CODE in jsonobj["error_response"]:
                 error.subcode = jsonobj["error_response"][P_SUB_CODE]
-            if P_SUB_MSG in jsonobj["error_response"] :
+            if P_SUB_MSG in jsonobj["error_response"]:
                 error.submsg = jsonobj["error_response"][P_SUB_MSG]
             error.application_host = response.getheader("Application-Host", "")
             error.service_host = response.getheader("Location-Host", "")
             raise error
         return jsonobj
 
-
     def getApplicationParameters(self):
         application_parameter = {}
         for key in self.__dict__:
             value = self.__dict__[key]
-            if not key.startswith("__") and not key in self.getMultipartParas() and not key.startswith("_RestApi__") and value is not None :
-                if(key.startswith("_")):
+            if (
+                not key.startswith("__")
+                and not key in self.getMultipartParas()
+                and not key.startswith("_RestApi__")
+                and value is not None
+            ):
+                if key.startswith("_"):
                     application_parameter[key[1:]] = value
                 else:
                     application_parameter[key] = value
-        #查询翻译字典来规避一些关键字属性
+        # 查询翻译字典来规避一些关键字属性
         translate_parameter = self.getTranslateParas()
         for key in application_parameter:
             value = application_parameter[key]
             if key in translate_parameter:
-                application_parameter[translate_parameter[key]] = application_parameter[key]
+                application_parameter[translate_parameter[key]] = application_parameter[
+                    key
+                ]
                 del application_parameter[key]
         return application_parameter
```

### Comparing `python-aliexpress-api-2.1.1/aliexpress_api/skd/api/rest/__init__.py` & `python-aliexpress-api-3.0.0/aliexpress_api/skd/api/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `python-aliexpress-api-2.1.1/aliexpress_api/tools/get_product_id.py` & `python-aliexpress-api-3.0.0/aliexpress_api/tools/get_product_id.py`

 * *Files identical despite different names*

### Comparing `python-aliexpress-api-2.1.1/python_aliexpress_api.egg-info/PKG-INFO` & `python-aliexpress-api-3.0.0/python_aliexpress_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: python-aliexpress-api
-Version: 2.1.1
+Version: 3.0.0
 Summary: AliExpress API wrapper for Python
 Home-page: https://github.com/sergioteula/python-aliexpress-api
 Author: Sergio Abad
 Author-email: sergio.abad@bytelix.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -72,9 +71,7 @@
 parent_categories = aliexpress.get_parent_categories()
 child_categories = aliexpress.get_child_categories(parent_categories[0].category_id)
 ```
 
 ## License
 
 Copyright © 2020 Sergio Abad. See [license](https://github.com/sergioteula/python-aliexpress-api/blob/master/LICENSE) for details.
-
-
```

### Comparing `python-aliexpress-api-2.1.1/python_aliexpress_api.egg-info/SOURCES.txt` & `python-aliexpress-api-3.0.0/python_aliexpress_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-aliexpress-api-2.1.1/setup.py` & `python-aliexpress-api-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='python-aliexpress-api',
-    version='2.1.1',
+    version='3.0.0',
     author='Sergio Abad',
     author_email='sergio.abad@bytelix.com',
     description='AliExpress API wrapper for Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/sergioteula/python-aliexpress-api',
```

