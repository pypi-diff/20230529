# Comparing `tmp/django-vendor-promo-0.2.2.tar.gz` & `tmp/django-vendor-promo-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-vendor-promo-0.2.2.tar", last modified: Fri May 26 13:22:47 2023, max compression
+gzip compressed data, was "django-vendor-promo-0.2.3.tar", last modified: Mon May 29 10:54:50 2023, max compression
```

## Comparing `django-vendor-promo-0.2.2.tar` & `django-vendor-promo-0.2.3.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.460409 django-vendor-promo-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/LICENSE.mit.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-26 13:22:47.456410 django-vendor-promo-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 13:22:47.460409 django-vendor-promo-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.440410 django-vendor-promo-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.444410 django-vendor-promo-0.2.2/src/django_vendor_promo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-26 13:22:47.000000 django-vendor-promo-0.2.2/src/django_vendor_promo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-26 13:22:47.000000 django-vendor-promo-0.2.2/src/django_vendor_promo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:22:47.000000 django-vendor-promo-0.2.2/src/django_vendor_promo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-26 13:22:47.000000 django-vendor-promo-0.2.2/src/django_vendor_promo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 13:22:47.000000 django-vendor-promo-0.2.2/src/django_vendor_promo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.448410 django-vendor-promo-0.2.2/src/vendorpromo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.448410 django-vendor-promo-0.2.2/src/vendorpromo/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.448410 django-vendor-promo-0.2.2/src/vendorpromo/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     9047 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/api/v1/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.448410 django-vendor-promo-0.2.2/src/vendorpromo/api/v1/vouchery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/api/v1/vouchery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/api/v1/vouchery/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/api/v1/vouchery/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/integrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.452410 django-vendor-promo-0.2.2/src/vendorpromo/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/migrations/0002_affiliate_couponcode_promotionalcampaign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/migrations/0003_auto_20230524_1701.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.452410 django-vendor-promo-0.2.2/src/vendorpromo/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/processors/DummyProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/processors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/processors/stripe.py
--rw-r--r--   0 runner    (1001) docker     (123)    17456 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/processors/vouchery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.440410 django-vendor-promo-0.2.2/src/vendorpromo/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.456410 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/affiliate_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/affiliate_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/coupon_code_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/coupon_code_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.456410 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/includes/promocode_apply.html
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/processor_site_config.html
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/processor_site_config_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/promo.html
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/promo_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/promocode_formset.html
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/promotional_campaign_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/promotional_campaign_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/vouchery_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/vouchery_integration.html
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/vouchery_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.456410 django-vendor-promo-0.2.2/src/vendorpromo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/tests/test_affiliate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/tests/test_coupon_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    21273 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/tests/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/tests/test_promo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/tests/test_promotional_campaign.py
--rw-r--r--   0 runner    (1001) docker     (123)    20938 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/tests/test_stripe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:54:50.990148 django-vendor-promo-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/LICENSE.mit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-29 10:54:50.990148 django-vendor-promo-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 10:54:50.990148 django-vendor-promo-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:54:50.974148 django-vendor-promo-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:54:50.978148 django-vendor-promo-0.2.3/src/django_vendor_promo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-29 10:54:50.000000 django-vendor-promo-0.2.3/src/django_vendor_promo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-29 10:54:50.000000 django-vendor-promo-0.2.3/src/django_vendor_promo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:54:50.000000 django-vendor-promo-0.2.3/src/django_vendor_promo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-29 10:54:50.000000 django-vendor-promo-0.2.3/src/django_vendor_promo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 10:54:50.000000 django-vendor-promo-0.2.3/src/django_vendor_promo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:54:50.978148 django-vendor-promo-0.2.3/src/vendorpromo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:54:50.978148 django-vendor-promo-0.2.3/src/vendorpromo/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:54:50.982148 django-vendor-promo-0.2.3/src/vendorpromo/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9047 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/api/v1/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:54:50.982148 django-vendor-promo-0.2.3/src/vendorpromo/api/v1/vouchery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/api/v1/vouchery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/api/v1/vouchery/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/api/v1/vouchery/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/integrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:54:50.982148 django-vendor-promo-0.2.3/src/vendorpromo/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/migrations/0002_affiliate_couponcode_promotionalcampaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/migrations/0003_auto_20230524_1701.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/migrations/0004_affiliate_name_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:54:50.982148 django-vendor-promo-0.2.3/src/vendorpromo/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/processors/DummyProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/processors/stripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17456 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/processors/vouchery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:54:50.974148 django-vendor-promo-0.2.3/src/vendorpromo/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:54:50.986148 django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/affiliate_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/affiliate_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/coupon_code_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/coupon_code_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:54:50.986148 django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/includes/promocode_apply.html
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/processor_site_config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/processor_site_config_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/promo.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/promo_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/promocode_formset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/promotional_campaign_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/promotional_campaign_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/vouchery_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/vouchery_integration.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/vouchery_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:54:50.990148 django-vendor-promo-0.2.3/src/vendorpromo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/tests/test_affiliate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/tests/test_coupon_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21273 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/tests/test_promo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/tests/test_promotional_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20938 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/tests/test_stripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-05-29 10:53:50.000000 django-vendor-promo-0.2.3/src/vendorpromo/views.py
```

### Comparing `django-vendor-promo-0.2.2/PKG-INFO` & `django-vendor-promo-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vendor-promo
-Version: 0.2.2
+Version: 0.2.3
 Summary: Extension to Django Vendor to add Promo Code capabilities
 Author: Roberto Himmelbauer
 Author-email: Grant Viklund <renderbox@gmail.com>
 Project-URL: Homepage, https://github.com/renderbox/django-vendor-promo/
 Project-URL: Bug Tracker, https://github.com/renderbox/django-vendor-promo/issues
 Keywords: django,app
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `django-vendor-promo-0.2.2/pyproject.toml` & `django-vendor-promo-0.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 [project]
 name = "django-vendor-promo"
-version = "0.2.2"
+version = "0.2.3"
 
 authors = [
   { name="Grant Viklund", email="renderbox@gmail.com" },
   { name="Roberto Himmelbauer" }
 ]
 description = "Extension to Django Vendor to add Promo Code capabilities"
 readme = "README.md"
```

### Comparing `django-vendor-promo-0.2.2/src/django_vendor_promo.egg-info/PKG-INFO` & `django-vendor-promo-0.2.3/src/django_vendor_promo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vendor-promo
-Version: 0.2.2
+Version: 0.2.3
 Summary: Extension to Django Vendor to add Promo Code capabilities
 Author: Roberto Himmelbauer
 Author-email: Grant Viklund <renderbox@gmail.com>
 Project-URL: Homepage, https://github.com/renderbox/django-vendor-promo/
 Project-URL: Bug Tracker, https://github.com/renderbox/django-vendor-promo/issues
 Keywords: django,app
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `django-vendor-promo-0.2.2/src/django_vendor_promo.egg-info/SOURCES.txt` & `django-vendor-promo-0.2.3/src/django_vendor_promo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 src/vendorpromo/api/v1/views.py
 src/vendorpromo/api/v1/vouchery/__init__.py
 src/vendorpromo/api/v1/vouchery/urls.py
 src/vendorpromo/api/v1/vouchery/views.py
 src/vendorpromo/migrations/0001_initial.py
 src/vendorpromo/migrations/0002_affiliate_couponcode_promotionalcampaign.py
 src/vendorpromo/migrations/0003_auto_20230524_1701.py
+src/vendorpromo/migrations/0004_affiliate_name_type.py
 src/vendorpromo/migrations/__init__.py
 src/vendorpromo/processors/DummyProcessor.py
 src/vendorpromo/processors/__init__.py
 src/vendorpromo/processors/base.py
 src/vendorpromo/processors/stripe.py
 src/vendorpromo/processors/vouchery.py
 src/vendorpromo/templates/vendorpromo/affiliate_detail.html
```

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/admin.py` & `django-vendor-promo-0.2.3/src/vendorpromo/admin.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/api/v1/urls.py` & `django-vendor-promo-0.2.3/src/vendorpromo/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/api/v1/views.py` & `django-vendor-promo-0.2.3/src/vendorpromo/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/api/v1/vouchery/views.py` & `django-vendor-promo-0.2.3/src/vendorpromo/api/v1/vouchery/views.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/config.py` & `django-vendor-promo-0.2.3/src/vendorpromo/config.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/forms.py` & `django-vendor-promo-0.2.3/src/vendorpromo/forms.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/integrations.py` & `django-vendor-promo-0.2.3/src/vendorpromo/integrations.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/migrations/0001_initial.py` & `django-vendor-promo-0.2.3/src/vendorpromo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/migrations/0002_affiliate_couponcode_promotionalcampaign.py` & `django-vendor-promo-0.2.3/src/vendorpromo/migrations/0002_affiliate_couponcode_promotionalcampaign.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/migrations/0003_auto_20230524_1701.py` & `django-vendor-promo-0.2.3/src/vendorpromo/migrations/0003_auto_20230524_1701.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/models.py` & `django-vendor-promo-0.2.3/src/vendorpromo/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,16 @@
 
 class Affiliate(CreateUpdateModelBase):
     '''
     Class to link Customer Profiles or a general contact to a Promo
     '''
     uuid = models.UUIDField(default=uuid.uuid4, editable=False, unique=True)
     slug = AutoSlugField(unique_with=('customer_profile__site'), editable=True, blank=True, null=True, verbose_name=_("Affiliate Code"))
+    name = models.CharField(max_length=120, blank=True, null=True, verbose_name=_("Name"))
+    type = models.CharField(max_length=80, blank=True, null=True, verbose_name=_("Type"))
     contact_name = models.CharField(max_length=120, blank=True, null=True, verbose_name=_("Contact Name"))
     email = models.EmailField(blank=True, null=True, verbose_name=_("Email"))
     company = models.CharField(max_length=120, blank=True, null=True, verbose_name=_("Company"))
     customer_profile = models.ForeignKey(CustomerProfile, blank=True, null=True, on_delete=models.CASCADE, verbose_name=_("Customer Profile"))
     promo = models.ManyToManyField(PromotionalCampaign, blank=True, verbose_name=_("Promotion Campaign"))
     site = models.ForeignKey(Site, on_delete=models.CASCADE, blank=False, null=False, verbose_name=_("Site"))
```

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/processors/base.py` & `django-vendor-promo-0.2.3/src/vendorpromo/processors/base.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/processors/stripe.py` & `django-vendor-promo-0.2.3/src/vendorpromo/processors/stripe.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/processors/vouchery.py` & `django-vendor-promo-0.2.3/src/vendorpromo/processors/vouchery.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/affiliate_detail.html` & `django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/affiliate_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/affiliate_list.html` & `django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/affiliate_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/coupon_code_detail.html` & `django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/coupon_code_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/coupon_code_list.html` & `django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/coupon_code_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/includes/promocode_apply.html` & `django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/includes/promocode_apply.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/processor_site_config_list.html` & `django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/processor_site_config_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/promo.html` & `django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/promo.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/promo_list.html` & `django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/promo_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/promocode_formset.html` & `django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/promocode_formset.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/promotional_campaign_detail.html` & `django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/promotional_campaign_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/promotional_campaign_list.html` & `django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/promotional_campaign_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/vouchery_detail.html` & `django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/vouchery_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/vouchery_integration.html` & `django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/vouchery_integration.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/vouchery_list.html` & `django-vendor-promo-0.2.3/src/vendorpromo/templates/vendorpromo/vouchery_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/tests/test_affiliate.py` & `django-vendor-promo-0.2.3/src/vendorpromo/tests/test_affiliate.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/tests/test_api.py` & `django-vendor-promo-0.2.3/src/vendorpromo/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/tests/test_coupon_code.py` & `django-vendor-promo-0.2.3/src/vendorpromo/tests/test_coupon_code.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/tests/test_processor.py` & `django-vendor-promo-0.2.3/src/vendorpromo/tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/tests/test_promo.py` & `django-vendor-promo-0.2.3/src/vendorpromo/tests/test_promo.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/tests/test_promotional_campaign.py` & `django-vendor-promo-0.2.3/src/vendorpromo/tests/test_promotional_campaign.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/tests/test_stripe.py` & `django-vendor-promo-0.2.3/src/vendorpromo/tests/test_stripe.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/urls.py` & `django-vendor-promo-0.2.3/src/vendorpromo/urls.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.2/src/vendorpromo/views.py` & `django-vendor-promo-0.2.3/src/vendorpromo/views.py`

 * *Files identical despite different names*

