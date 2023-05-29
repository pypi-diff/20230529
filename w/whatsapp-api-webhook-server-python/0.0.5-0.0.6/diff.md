# Comparing `tmp/whatsapp-api-webhook-server-python-0.0.5.tar.gz` & `tmp/whatsapp-api-webhook-server-python-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-api-webhook-server-python-0.0.5.tar", last modified: Sun Oct 23 13:12:28 2022, max compression
+gzip compressed data, was "whatsapp-api-webhook-server-python-0.0.6.tar", last modified: Mon May 29 11:40:42 2023, max compression
```

## Comparing `whatsapp-api-webhook-server-python-0.0.5.tar` & `whatsapp-api-webhook-server-python-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 13:12:28.449168 whatsapp-api-webhook-server-python-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-10-23 13:12:19.000000 whatsapp-api-webhook-server-python-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5897 2022-10-23 13:12:28.449168 whatsapp-api-webhook-server-python-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5304 2022-10-23 13:12:19.000000 whatsapp-api-webhook-server-python-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-23 13:12:28.449168 whatsapp-api-webhook-server-python-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      863 2022-10-23 13:12:19.000000 whatsapp-api-webhook-server-python-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 13:12:28.445168 whatsapp-api-webhook-server-python-0.0.5/whatsapp_api_webhook_server_python/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-23 13:12:19.000000 whatsapp-api-webhook-server-python-0.0.5/whatsapp_api_webhook_server_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-10-23 13:12:19.000000 whatsapp-api-webhook-server-python-0.0.5/whatsapp_api_webhook_server_python/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1598 2022-10-23 13:12:19.000000 whatsapp-api-webhook-server-python-0.0.5/whatsapp_api_webhook_server_python/webhooksHandler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 13:12:28.449168 whatsapp-api-webhook-server-python-0.0.5/whatsapp_api_webhook_server_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5897 2022-10-23 13:12:28.000000 whatsapp-api-webhook-server-python-0.0.5/whatsapp_api_webhook_server_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-10-23 13:12:28.000000 whatsapp-api-webhook-server-python-0.0.5/whatsapp_api_webhook_server_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-23 13:12:28.000000 whatsapp-api-webhook-server-python-0.0.5/whatsapp_api_webhook_server_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-23 13:12:28.000000 whatsapp-api-webhook-server-python-0.0.5/whatsapp_api_webhook_server_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-10-23 13:12:28.000000 whatsapp-api-webhook-server-python-0.0.5/whatsapp_api_webhook_server_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 11:40:42.287552 whatsapp-api-webhook-server-python-0.0.6/
+-rw-rw-rw-   0        0        0    18829 2023-05-29 11:34:04.000000 whatsapp-api-webhook-server-python-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     7668 2023-05-29 11:40:42.287552 whatsapp-api-webhook-server-python-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6594 2023-05-29 11:35:26.000000 whatsapp-api-webhook-server-python-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-29 11:40:42.287552 whatsapp-api-webhook-server-python-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1434 2023-05-29 11:34:04.000000 whatsapp-api-webhook-server-python-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 11:40:42.278537 whatsapp-api-webhook-server-python-0.0.6/tests/
+-rw-rw-rw-   0        0        0      518 2023-05-29 10:36:08.000000 whatsapp-api-webhook-server-python-0.0.6/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2023-05-29 11:40:42.281536 whatsapp-api-webhook-server-python-0.0.6/whatsapp_api_webhook_server_python/
+-rw-rw-rw-   0        0        0        0 2023-05-29 10:36:08.000000 whatsapp-api-webhook-server-python-0.0.6/whatsapp_api_webhook_server_python/__init__.py
+-rw-rw-rw-   0        0        0      255 2023-05-29 10:36:08.000000 whatsapp-api-webhook-server-python-0.0.6/whatsapp_api_webhook_server_python/webhooks.py
+-rw-rw-rw-   0        0        0     1643 2023-05-29 10:36:08.000000 whatsapp-api-webhook-server-python-0.0.6/whatsapp_api_webhook_server_python/webhooksHandler.py
+drwxrwxrwx   0        0        0        0 2023-05-29 11:40:42.286550 whatsapp-api-webhook-server-python-0.0.6/whatsapp_api_webhook_server_python.egg-info/
+-rw-rw-rw-   0        0        0     7668 2023-05-29 11:40:42.000000 whatsapp-api-webhook-server-python-0.0.6/whatsapp_api_webhook_server_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-05-29 11:40:42.000000 whatsapp-api-webhook-server-python-0.0.6/whatsapp_api_webhook_server_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 11:40:42.000000 whatsapp-api-webhook-server-python-0.0.6/whatsapp_api_webhook_server_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-29 11:40:42.000000 whatsapp-api-webhook-server-python-0.0.6/whatsapp_api_webhook_server_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       35 2023-05-29 11:40:42.000000 whatsapp-api-webhook-server-python-0.0.6/whatsapp_api_webhook_server_python.egg-info/top_level.txt
```

