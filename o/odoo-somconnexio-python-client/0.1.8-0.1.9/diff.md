# Comparing `tmp/odoo-somconnexio-python-client-0.1.8.tar.gz` & `tmp/odoo-somconnexio-python-client-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/odoo-somconnexio-python-client-0.1.8.tar", last modified: Tue Dec 29 07:53:13 2020, max compression
+gzip compressed data, was "dist/odoo-somconnexio-python-client-0.1.9.tar", last modified: Thu Jan  7 10:48:53 2021, max compression
```

## Comparing `odoo-somconnexio-python-client-0.1.8.tar` & `odoo-somconnexio-python-client-0.1.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-29 07:53:13.000000 odoo-somconnexio-python-client-0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)     6342 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/README.md
--rw-r--r--   0 root         (0) root         (0)     8872 2020-12-29 07:53:13.000000 odoo-somconnexio-python-client-0.1.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-29 07:53:13.000000 odoo-somconnexio-python-client-0.1.8/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-29 07:53:13.000000 odoo-somconnexio-python-client-0.1.8/tests/tryton_mappers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/tests/tryton_mappers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2358 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/tests/tryton_mappers/test_subscription_request_from_partner_form.py
--rw-rw-rw-   0 root         (0) root         (0)     9931 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/tests/tryton_mappers/test_crm_lead_from_contract_form.py
--rw-rw-rw-   0 root         (0) root         (0)     7880 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/tests/tryton_mappers/tryton_factories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-29 07:53:13.000000 odoo-somconnexio-python-client-0.1.8/tests/resources/
--rw-rw-rw-   0 root         (0) root         (0)     1792 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/tests/resources/test_providers.py
--rw-rw-rw-   0 root         (0) root         (0)     2569 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/tests/resources/test_subscription_request.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/tests/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      971 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/tests/resources/test_address.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/tests/resources/test_partner.py
--rw-rw-rw-   0 root         (0) root         (0)     3703 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/tests/resources/test_crm_lead.py
--rw-rw-rw-   0 root         (0) root         (0)      453 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/tests/resources/test_discovery_channel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-29 07:53:13.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/
--rw-rw-rw-   0 root         (0) root         (0)     3092 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/client.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      193 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-29 07:53:13.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/tryton_mappers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/tryton_mappers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10027 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/tryton_mappers/crm_lead_from_contract_form.py
--rw-rw-rw-   0 root         (0) root         (0)     4391 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/tryton_mappers/subscription_request_from_partner_form.py
--rw-rw-rw-   0 root         (0) root         (0)      728 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-29 07:53:13.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/resources/
--rw-rw-rw-   0 root         (0) root         (0)      975 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/resources/crm_lead.py
--rw-rw-rw-   0 root         (0) root         (0)      769 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/resources/address.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      629 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/resources/discovery_channel.py
--rw-rw-rw-   0 root         (0) root         (0)     1033 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/resources/provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1912 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/resources/partner.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/resources/crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1390 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/resources/subscription_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1177 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/resources/broadband_isp_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/resources/mobile_isp_info.py
--rw-r--r--   0 root         (0) root         (0)       38 2020-12-29 07:53:13.000000 odoo-somconnexio-python-client-0.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1942 2020-12-29 07:53:05.000000 odoo-somconnexio-python-client-0.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-29 07:53:13.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2020-12-29 07:53:13.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     8872 2020-12-29 07:53:13.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1750 2020-12-29 07:53:13.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-12-29 07:53:13.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2020-12-29 07:53:13.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2020-12-29 07:53:13.000000 odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-07 10:48:53.000000 odoo-somconnexio-python-client-0.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)     6342 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/README.md
+-rw-r--r--   0 root         (0) root         (0)     8872 2021-01-07 10:48:53.000000 odoo-somconnexio-python-client-0.1.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-07 10:48:53.000000 odoo-somconnexio-python-client-0.1.9/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-07 10:48:53.000000 odoo-somconnexio-python-client-0.1.9/tests/tryton_mappers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/tests/tryton_mappers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2358 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/tests/tryton_mappers/test_subscription_request_from_partner_form.py
+-rw-rw-rw-   0 root         (0) root         (0)     9931 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/tests/tryton_mappers/test_crm_lead_from_contract_form.py
+-rw-rw-rw-   0 root         (0) root         (0)     7880 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/tests/tryton_mappers/tryton_factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-07 10:48:53.000000 odoo-somconnexio-python-client-0.1.9/tests/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/tests/resources/test_providers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2569 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/tests/resources/test_subscription_request.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/tests/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      971 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/tests/resources/test_address.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/tests/resources/test_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)     3703 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/tests/resources/test_crm_lead.py
+-rw-rw-rw-   0 root         (0) root         (0)      453 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/tests/resources/test_discovery_channel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-07 10:48:53.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/
+-rw-rw-rw-   0 root         (0) root         (0)     3092 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/client.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      193 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-07 10:48:53.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/tryton_mappers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/tryton_mappers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10027 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/tryton_mappers/crm_lead_from_contract_form.py
+-rw-rw-rw-   0 root         (0) root         (0)     4391 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/tryton_mappers/subscription_request_from_partner_form.py
+-rw-rw-rw-   0 root         (0) root         (0)      728 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-07 10:48:53.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      975 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/resources/crm_lead.py
+-rw-rw-rw-   0 root         (0) root         (0)      769 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/resources/address.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      629 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/resources/discovery_channel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/resources/provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/resources/partner.py
+-rw-rw-rw-   0 root         (0) root         (0)      523 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/resources/crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1390 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/resources/subscription_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/resources/broadband_isp_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/resources/mobile_isp_info.py
+-rw-r--r--   0 root         (0) root         (0)       38 2021-01-07 10:48:53.000000 odoo-somconnexio-python-client-0.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1942 2021-01-07 10:48:45.000000 odoo-somconnexio-python-client-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-07 10:48:53.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2021-01-07 10:48:53.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     8872 2021-01-07 10:48:53.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1750 2021-01-07 10:48:53.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-01-07 10:48:53.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2021-01-07 10:48:53.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2021-01-07 10:48:53.000000 odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client.egg-info/top_level.txt
```

### Comparing `odoo-somconnexio-python-client-0.1.8/README.md` & `odoo-somconnexio-python-client-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `odoo-somconnexio-python-client-0.1.8/PKG-INFO` & `odoo-somconnexio-python-client-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-somconnexio-python-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python wrapper for SomConnexio's Odoo (using REST API)
 Home-page: https://gitlab.com/coopdevs/odoo-somconnexio-python-client
 Author: Coopdevs
 Author-email: info@coopdevs.org
 Maintainer: Daniel Palomar
 License: UNKNOWN
 Description: [![pipeline status](https://gitlab.com/coopdevs/odoo-somconnexio-python-client/badges/master/pipeline.svg)](https://gitlab.com/coopdevs/odoo-somconnexio-python-client/commits/master)
```

### Comparing `odoo-somconnexio-python-client-0.1.8/tests/tryton_mappers/test_subscription_request_from_partner_form.py` & `odoo-somconnexio-python-client-0.1.9/tests/tryton_mappers/test_subscription_request_from_partner_form.py`

 * *Files identical despite different names*

### Comparing `odoo-somconnexio-python-client-0.1.8/tests/tryton_mappers/test_crm_lead_from_contract_form.py` & `odoo-somconnexio-python-client-0.1.9/tests/tryton_mappers/test_crm_lead_from_contract_form.py`

 * *Files identical despite different names*

### Comparing `odoo-somconnexio-python-client-0.1.8/tests/tryton_mappers/tryton_factories.py` & `odoo-somconnexio-python-client-0.1.9/tests/tryton_mappers/tryton_factories.py`

 * *Files identical despite different names*

### Comparing `odoo-somconnexio-python-client-0.1.8/tests/resources/test_providers.py` & `odoo-somconnexio-python-client-0.1.9/tests/resources/test_providers.py`

 * *Files identical despite different names*

### Comparing `odoo-somconnexio-python-client-0.1.8/tests/resources/test_subscription_request.py` & `odoo-somconnexio-python-client-0.1.9/tests/resources/test_subscription_request.py`

 * *Files identical despite different names*

### Comparing `odoo-somconnexio-python-client-0.1.8/tests/resources/test_address.py` & `odoo-somconnexio-python-client-0.1.9/tests/resources/test_address.py`

 * *Files identical despite different names*

### Comparing `odoo-somconnexio-python-client-0.1.8/tests/resources/test_partner.py` & `odoo-somconnexio-python-client-0.1.9/tests/resources/test_partner.py`

 * *Files identical despite different names*

### Comparing `odoo-somconnexio-python-client-0.1.8/tests/resources/test_crm_lead.py` & `odoo-somconnexio-python-client-0.1.9/tests/resources/test_crm_lead.py`

 * *Files identical despite different names*

### Comparing `odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/client.py` & `odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/client.py`

 * *Files identical despite different names*

### Comparing `odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/tryton_mappers/crm_lead_from_contract_form.py` & `odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/tryton_mappers/crm_lead_from_contract_form.py`

 * *Files identical despite different names*

### Comparing `odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/tryton_mappers/subscription_request_from_partner_form.py` & `odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/tryton_mappers/subscription_request_from_partner_form.py`

 * *Files identical despite different names*

### Comparing `odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/exceptions.py` & `odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/resources/crm_lead.py` & `odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/resources/crm_lead.py`

 * *Files identical despite different names*

### Comparing `odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/resources/address.py` & `odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/resources/address.py`

 * *Files identical despite different names*

### Comparing `odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/resources/discovery_channel.py` & `odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/resources/discovery_channel.py`

 * *Files identical despite different names*

### Comparing `odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/resources/provider.py` & `odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/resources/provider.py`

 * *Files identical despite different names*

### Comparing `odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/resources/partner.py` & `odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/resources/partner.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         email,
         phone,
         mobile,
         cooperator_register_number,
         cooperator_end_date,
         coop_agreement_code,
         sponsor_id,
+        coop_candidate,
         **kwargs
     ):
         self.id = id
         self.name = name
         self.firstname = firstname
         self.lastname = lastname
         self.ref = ref
@@ -37,14 +38,15 @@
         self.email = email
         self.phone = phone
         self.mobile = mobile
         self.cooperator_register_number = cooperator_register_number
         self.cooperator_end_date = cooperator_end_date
         self.sponsor_id = sponsor_id
         self.coop_agreement_code = coop_agreement_code
+        self.coop_candidate = coop_candidate
 
     @classmethod
     def get(cls, ref):
         """
         Get ResPartner using the ref param.
 
         :return: Partner object if exists
```

### Comparing `odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/resources/crm_lead_line.py` & `odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/resources/crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/resources/subscription_request.py` & `odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/resources/subscription_request.py`

 * *Files identical despite different names*

### Comparing `odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/resources/broadband_isp_info.py` & `odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/resources/broadband_isp_info.py`

 * *Files identical despite different names*

### Comparing `odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client/resources/mobile_isp_info.py` & `odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client/resources/mobile_isp_info.py`

 * *Files identical despite different names*

### Comparing `odoo-somconnexio-python-client-0.1.8/setup.py` & `odoo-somconnexio-python-client-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import sys
 
 with open("README.md") as f:
     README = f.read()
 
 
-VERSION = "0.1.8"
+VERSION = "0.1.9"
 
 
 ########
 # Copied from https://github.com/kennethreitz/setup.py
 here = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client.egg-info/PKG-INFO` & `odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-somconnexio-python-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python wrapper for SomConnexio's Odoo (using REST API)
 Home-page: https://gitlab.com/coopdevs/odoo-somconnexio-python-client
 Author: Coopdevs
 Author-email: info@coopdevs.org
 Maintainer: Daniel Palomar
 License: UNKNOWN
 Description: [![pipeline status](https://gitlab.com/coopdevs/odoo-somconnexio-python-client/badges/master/pipeline.svg)](https://gitlab.com/coopdevs/odoo-somconnexio-python-client/commits/master)
```

### Comparing `odoo-somconnexio-python-client-0.1.8/odoo_somconnexio_python_client.egg-info/SOURCES.txt` & `odoo-somconnexio-python-client-0.1.9/odoo_somconnexio_python_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

