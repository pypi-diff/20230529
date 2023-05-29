# Comparing `tmp/pretix-saferpay-1.4.0.tar.gz` & `tmp/pretix-saferpay-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-saferpay-1.4.0.tar", last modified: Mon Jan 30 14:19:45 2023, max compression
+gzip compressed data, was "pretix-saferpay-1.4.1.tar", last modified: Mon May 29 07:31:03 2023, max compression
```

## Comparing `pretix-saferpay-1.4.0.tar` & `pretix-saferpay-1.4.1.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-01-30 14:19:45.388349 pretix-saferpay-1.4.0/
--rw-r--r--   0 raphael   (1000) raphael   (1000)      555 2022-02-19 19:26:48.000000 pretix-saferpay-1.4.0/LICENSE
--rw-r--r--   0 raphael   (1000) raphael   (1000)      132 2022-02-19 19:26:48.000000 pretix-saferpay-1.4.0/MANIFEST.in
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1209 2023-01-30 14:19:45.388349 pretix-saferpay-1.4.0/PKG-INFO
--rw-r--r--   0 raphael   (1000) raphael   (1000)      931 2022-02-19 19:26:48.000000 pretix-saferpay-1.4.0/README.rst
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-01-30 14:19:45.388349 pretix-saferpay-1.4.0/pretix_saferpay/
--rw-r--r--   0 raphael   (1000) raphael   (1000)       22 2023-01-30 14:19:38.000000 pretix-saferpay-1.4.0/pretix_saferpay/__init__.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)      742 2023-01-30 14:19:38.000000 pretix-saferpay-1.4.0/pretix_saferpay/apps.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-01-30 14:19:45.388349 pretix-saferpay-1.4.0/pretix_saferpay/locale/
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-01-30 14:19:45.385015 pretix-saferpay-1.4.0/pretix_saferpay/locale/de/
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-01-30 14:19:45.388349 pretix-saferpay-1.4.0/pretix_saferpay/locale/de/LC_MESSAGES/
--rw-r--r--   0 raphael   (1000) raphael   (1000)     6292 2022-03-31 20:30:12.000000 pretix-saferpay-1.4.0/pretix_saferpay/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 raphael   (1000) raphael   (1000)    10800 2022-03-31 20:05:26.000000 pretix-saferpay-1.4.0/pretix_saferpay/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-01-30 14:19:45.388349 pretix-saferpay-1.4.0/pretix_saferpay/locale/de_Informal/
--rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-02-19 19:26:48.000000 pretix-saferpay-1.4.0/pretix_saferpay/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-01-30 14:19:45.388349 pretix-saferpay-1.4.0/pretix_saferpay/locale/de_Informal/LC_MESSAGES/
--rw-r--r--   0 raphael   (1000) raphael   (1000)     6239 2022-03-31 20:30:12.000000 pretix-saferpay-1.4.0/pretix_saferpay/locale/de_Informal/LC_MESSAGES/django.mo
--rw-r--r--   0 raphael   (1000) raphael   (1000)    10741 2022-03-31 20:05:26.000000 pretix-saferpay-1.4.0/pretix_saferpay/locale/de_Informal/LC_MESSAGES/django.po
--rw-r--r--   0 raphael   (1000) raphael   (1000)     6971 2022-03-24 16:46:30.000000 pretix-saferpay-1.4.0/pretix_saferpay/locale/django.pot
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-01-30 14:19:45.385015 pretix-saferpay-1.4.0/pretix_saferpay/locale/hr/
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-01-30 14:19:45.388349 pretix-saferpay-1.4.0/pretix_saferpay/locale/hr/LC_MESSAGES/
--rw-r--r--   0 raphael   (1000) raphael   (1000)     6946 2023-01-30 14:18:39.000000 pretix-saferpay-1.4.0/pretix_saferpay/locale/hr/LC_MESSAGES/django.po
--rw-r--r--   0 raphael   (1000) raphael   (1000)    28125 2023-01-30 14:18:39.000000 pretix-saferpay-1.4.0/pretix_saferpay/payment.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1741 2022-10-11 15:58:05.000000 pretix-saferpay-1.4.0/pretix_saferpay/signals.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-01-30 14:19:45.385015 pretix-saferpay-1.4.0/pretix_saferpay/static/
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-01-30 14:19:45.388349 pretix-saferpay-1.4.0/pretix_saferpay/static/pretix_saferpay/
--rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-02-19 19:26:48.000000 pretix-saferpay-1.4.0/pretix_saferpay/static/pretix_saferpay/.gitkeep
--rw-r--r--   0 raphael   (1000) raphael   (1000)     3674 2022-03-24 16:46:30.000000 pretix-saferpay-1.4.0/pretix_saferpay/static/pretix_saferpay/logo.svg
--rw-r--r--   0 raphael   (1000) raphael   (1000)      300 2022-10-11 15:58:02.000000 pretix-saferpay-1.4.0/pretix_saferpay/tasks.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-01-30 14:19:45.385015 pretix-saferpay-1.4.0/pretix_saferpay/templates/
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-01-30 14:19:45.388349 pretix-saferpay-1.4.0/pretix_saferpay/templates/pretix_saferpay/
--rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-02-19 19:26:48.000000 pretix-saferpay-1.4.0/pretix_saferpay/templates/pretix_saferpay/.gitkeep
--rw-r--r--   0 raphael   (1000) raphael   (1000)      342 2022-02-19 19:26:48.000000 pretix-saferpay-1.4.0/pretix_saferpay/templates/pretix_saferpay/checkout_payment_confirm.html
--rw-r--r--   0 raphael   (1000) raphael   (1000)      227 2022-02-19 19:26:48.000000 pretix-saferpay-1.4.0/pretix_saferpay/templates/pretix_saferpay/checkout_payment_form.html
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1050 2022-02-19 19:26:48.000000 pretix-saferpay-1.4.0/pretix_saferpay/templates/pretix_saferpay/control.html
--rw-r--r--   0 raphael   (1000) raphael   (1000)      629 2022-02-19 19:26:48.000000 pretix-saferpay-1.4.0/pretix_saferpay/templates/pretix_saferpay/pending.html
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1044 2022-10-11 15:58:24.000000 pretix-saferpay-1.4.0/pretix_saferpay/templates/pretix_saferpay/redirect.html
--rw-r--r--   0 raphael   (1000) raphael   (1000)      739 2022-12-17 17:14:45.000000 pretix-saferpay-1.4.0/pretix_saferpay/urls.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)    10511 2022-10-11 15:58:05.000000 pretix-saferpay-1.4.0/pretix_saferpay/views.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-01-30 14:19:45.388349 pretix-saferpay-1.4.0/pretix_saferpay.egg-info/
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1209 2023-01-30 14:19:45.000000 pretix-saferpay-1.4.0/pretix_saferpay.egg-info/PKG-INFO
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1217 2023-01-30 14:19:45.000000 pretix-saferpay-1.4.0/pretix_saferpay.egg-info/SOURCES.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)        1 2023-01-30 14:19:45.000000 pretix-saferpay-1.4.0/pretix_saferpay.egg-info/dependency_links.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)       67 2023-01-30 14:19:45.000000 pretix-saferpay-1.4.0/pretix_saferpay.egg-info/entry_points.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)       16 2023-01-30 14:19:45.000000 pretix-saferpay-1.4.0/pretix_saferpay.egg-info/top_level.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)      363 2023-01-30 14:19:45.388349 pretix-saferpay-1.4.0/setup.cfg
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1082 2022-12-17 17:15:15.000000 pretix-saferpay-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:31:03.047279 pretix-saferpay-1.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-05-29 07:27:55.000000 pretix-saferpay-1.4.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-05-29 07:27:55.000000 pretix-saferpay-1.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1971 2023-05-29 07:31:03.047279 pretix-saferpay-1.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-29 07:27:55.000000 pretix-saferpay-1.4.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:31:03.043279 pretix-saferpay-1.4.1/pretix_saferpay/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-29 07:27:55.000000 pretix-saferpay-1.4.1/pretix_saferpay/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      742 2023-05-29 07:27:55.000000 pretix-saferpay-1.4.1/pretix_saferpay/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:31:03.047279 pretix-saferpay-1.4.1/pretix_saferpay/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:31:03.043279 pretix-saferpay-1.4.1/pretix_saferpay/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:31:03.047279 pretix-saferpay-1.4.1/pretix_saferpay/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10800 2023-05-29 07:27:55.000000 pretix-saferpay-1.4.1/pretix_saferpay/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:31:03.047279 pretix-saferpay-1.4.1/pretix_saferpay/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 07:30:36.000000 pretix-saferpay-1.4.1/pretix_saferpay/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:31:03.047279 pretix-saferpay-1.4.1/pretix_saferpay/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10741 2023-05-29 07:27:55.000000 pretix-saferpay-1.4.1/pretix_saferpay/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     6971 2023-05-29 07:27:55.000000 pretix-saferpay-1.4.1/pretix_saferpay/locale/django.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:31:03.043279 pretix-saferpay-1.4.1/pretix_saferpay/locale/hr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:31:03.047279 pretix-saferpay-1.4.1/pretix_saferpay/locale/hr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     6946 2023-05-29 07:27:55.000000 pretix-saferpay-1.4.1/pretix_saferpay/locale/hr/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)    28691 2023-05-29 07:27:55.000000 pretix-saferpay-1.4.1/pretix_saferpay/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1741 2023-05-29 07:27:55.000000 pretix-saferpay-1.4.1/pretix_saferpay/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:31:03.043279 pretix-saferpay-1.4.1/pretix_saferpay/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:31:03.047279 pretix-saferpay-1.4.1/pretix_saferpay/static/pretix_saferpay/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 07:30:36.000000 pretix-saferpay-1.4.1/pretix_saferpay/static/pretix_saferpay/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     3674 2023-05-29 07:27:55.000000 pretix-saferpay-1.4.1/pretix_saferpay/static/pretix_saferpay/logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-05-29 07:27:55.000000 pretix-saferpay-1.4.1/pretix_saferpay/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:31:03.043279 pretix-saferpay-1.4.1/pretix_saferpay/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:31:03.047279 pretix-saferpay-1.4.1/pretix_saferpay/templates/pretix_saferpay/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 07:30:36.000000 pretix-saferpay-1.4.1/pretix_saferpay/templates/pretix_saferpay/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-05-29 07:27:55.000000 pretix-saferpay-1.4.1/pretix_saferpay/templates/pretix_saferpay/checkout_payment_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-05-29 07:27:55.000000 pretix-saferpay-1.4.1/pretix_saferpay/templates/pretix_saferpay/checkout_payment_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2023-05-29 07:27:55.000000 pretix-saferpay-1.4.1/pretix_saferpay/templates/pretix_saferpay/control.html
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-05-29 07:27:55.000000 pretix-saferpay-1.4.1/pretix_saferpay/templates/pretix_saferpay/pending.html
+-rw-rw-rw-   0 root         (0) root         (0)     1044 2023-05-29 07:27:55.000000 pretix-saferpay-1.4.1/pretix_saferpay/templates/pretix_saferpay/redirect.html
+-rw-rw-rw-   0 root         (0) root         (0)      739 2023-05-29 07:27:55.000000 pretix-saferpay-1.4.1/pretix_saferpay/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    10511 2023-05-29 07:27:55.000000 pretix-saferpay-1.4.1/pretix_saferpay/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:31:03.043279 pretix-saferpay-1.4.1/pretix_saferpay.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1971 2023-05-29 07:31:03.000000 pretix-saferpay-1.4.1/pretix_saferpay.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-05-29 07:31:03.000000 pretix-saferpay-1.4.1/pretix_saferpay.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 07:31:03.000000 pretix-saferpay-1.4.1/pretix_saferpay.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      135 2023-05-29 07:31:03.000000 pretix-saferpay-1.4.1/pretix_saferpay.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-29 07:31:03.000000 pretix-saferpay-1.4.1/pretix_saferpay.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      918 2023-05-29 07:27:55.000000 pretix-saferpay-1.4.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      797 2023-05-29 07:31:03.047279 pretix-saferpay-1.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-29 07:27:55.000000 pretix-saferpay-1.4.1/setup.py
```

### Comparing `pretix-saferpay-1.4.0/LICENSE` & `pretix-saferpay-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-saferpay-1.4.0/README.rst` & `pretix-saferpay-1.4.1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 1. Make sure that you have a working `pretix development setup`_.
 
 2. Clone this repository, eg to ``local/pretix-saferpay``.
 
 3. Activate the virtual environment you use for pretix development.
 
-4. Execute ``python setup.py develop`` within this directory to register this application with pretix's plugin registry.
+4. Execute ``pip install -e .`` within this directory to register this application with pretix's plugin registry.
 
 5. Execute ``make`` within this directory to compile translations.
 
 6. Restart your local pretix server. You can now use the plugin from this repository for your events by enabling it in
    the 'plugins' tab in the settings.
```

### Comparing `pretix-saferpay-1.4.0/pretix_saferpay/apps.py` & `pretix-saferpay-1.4.1/pretix_saferpay/apps.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,13 +13,13 @@
         category = "PAYMENT"
         description = gettext_lazy(
             "Accept payments through Saferpay, a payment method offered by Worldline (formerly SIX Payment Services)."
         )
         visible = True
         picture = "pretix_saferpay/logo.svg"
         version = __version__
-        compatibility = "pretix>=4.16.0"
+        compatibility = "pretix>=4.20.0"
 
     def ready(self):
         from . import signals, tasks  # NOQA
```

### Comparing `pretix-saferpay-1.4.0/pretix_saferpay/locale/de/LC_MESSAGES/django.po` & `pretix-saferpay-1.4.1/pretix_saferpay/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-saferpay-1.4.0/pretix_saferpay/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-saferpay-1.4.1/pretix_saferpay/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-saferpay-1.4.0/pretix_saferpay/locale/django.pot` & `pretix-saferpay-1.4.1/pretix_saferpay/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-saferpay-1.4.0/pretix_saferpay/locale/hr/LC_MESSAGES/django.po` & `pretix-saferpay-1.4.1/pretix_saferpay/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-saferpay-1.4.0/pretix_saferpay/payment.py` & `pretix-saferpay-1.4.1/pretix_saferpay/payment.py`

 * *Files 1% similar despite different names*

```diff
@@ -425,14 +425,26 @@
                 "pretix.event.order.refund.failed",
                 {
                     "local_id": refund.local_id,
                     "provider": refund.provider,
                     "data": refund.info_data,
                 },
             )
+            if "ProcessorMessage" in refund.info_data:
+                raise PaymentException(
+                    _(
+                        "Saferpay returned the following error: {error}"
+                    ).format(error=refund.info_data.get('ProcessorMessage'))
+                )
+            elif "ErrorMessage" in refund.info_data:
+                raise PaymentException(
+                    _(
+                        "Saferpay returned the following error: {error}"
+                    ).format(error=refund.info_data.get('ErrorMessage'))
+                )
             raise PaymentException(
                 _(
                     "We had trouble communicating with Saferpay. Please try again and get in touch "
                     "with us if this problem persists."
                 )
             )
         except RequestException as e:
```

### Comparing `pretix-saferpay-1.4.0/pretix_saferpay/signals.py` & `pretix-saferpay-1.4.1/pretix_saferpay/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-saferpay-1.4.0/pretix_saferpay/static/pretix_saferpay/logo.svg` & `pretix-saferpay-1.4.1/pretix_saferpay/static/pretix_saferpay/logo.svg`

 * *Files identical despite different names*

### Comparing `pretix-saferpay-1.4.0/pretix_saferpay/templates/pretix_saferpay/control.html` & `pretix-saferpay-1.4.1/pretix_saferpay/templates/pretix_saferpay/control.html`

 * *Files identical despite different names*

### Comparing `pretix-saferpay-1.4.0/pretix_saferpay/templates/pretix_saferpay/pending.html` & `pretix-saferpay-1.4.1/pretix_saferpay/templates/pretix_saferpay/pending.html`

 * *Files identical despite different names*

### Comparing `pretix-saferpay-1.4.0/pretix_saferpay/templates/pretix_saferpay/redirect.html` & `pretix-saferpay-1.4.1/pretix_saferpay/templates/pretix_saferpay/redirect.html`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 <html>
 <head>
     <title>{{ settings.PRETIX_INSTANCE_NAME }}</title>
     {% compress css %}
         <link rel="stylesheet" type="text/x-scss" href="{% static "pretixbase/scss/cachedfiles.scss" %}"/>
     {% endcompress %}
     {% compress js %}
-        <script type="text/javascript" src="{% static "jquery/js/jquery-2.1.1.min.js" %}"></script>
+        <script type="text/javascript" src="{% static "jquery/js/jquery-3.6.4.min.js" %}"></script>
     {% endcompress %}
 </head>
 <body>
     <div class="container">
         <h1>{% trans "The payment process has started in a new window." %}</h1>
 
         <p>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% load compress %} {% load i18n %} {% load static %}
 {% compress css %}
 css/cachedfiles.scss" %}"/> {% endcompress %} {% compress js %}
-s/jquery-2.1.1.min.js" %}">
+s/jquery-3.6.4.min.js" %}">
 {% endcompress %}
 ****** {% trans "The payment process has started in a new window." %} ******
 {% trans "The window to enter your payment data was not opened or was closed?"
 %}
 _{%_trans_"Click_here_in_order_to_open_the_window."_%}
```

### Comparing `pretix-saferpay-1.4.0/pretix_saferpay/urls.py` & `pretix-saferpay-1.4.1/pretix_saferpay/urls.py`

 * *Files identical despite different names*

### Comparing `pretix-saferpay-1.4.0/pretix_saferpay/views.py` & `pretix-saferpay-1.4.1/pretix_saferpay/views.py`

 * *Files identical despite different names*

### Comparing `pretix-saferpay-1.4.0/pretix_saferpay.egg-info/SOURCES.txt` & `pretix-saferpay-1.4.1/pretix_saferpay.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 pretix_saferpay/__init__.py
 pretix_saferpay/apps.py
 pretix_saferpay/payment.py
 pretix_saferpay/signals.py
 pretix_saferpay/tasks.py
@@ -12,18 +13,16 @@
 pretix_saferpay/views.py
 pretix_saferpay.egg-info/PKG-INFO
 pretix_saferpay.egg-info/SOURCES.txt
 pretix_saferpay.egg-info/dependency_links.txt
 pretix_saferpay.egg-info/entry_points.txt
 pretix_saferpay.egg-info/top_level.txt
 pretix_saferpay/locale/django.pot
-pretix_saferpay/locale/de/LC_MESSAGES/django.mo
 pretix_saferpay/locale/de/LC_MESSAGES/django.po
 pretix_saferpay/locale/de_Informal/.gitkeep
-pretix_saferpay/locale/de_Informal/LC_MESSAGES/django.mo
 pretix_saferpay/locale/de_Informal/LC_MESSAGES/django.po
 pretix_saferpay/locale/hr/LC_MESSAGES/django.po
 pretix_saferpay/static/pretix_saferpay/.gitkeep
 pretix_saferpay/static/pretix_saferpay/logo.svg
 pretix_saferpay/templates/pretix_saferpay/.gitkeep
 pretix_saferpay/templates/pretix_saferpay/checkout_payment_confirm.html
 pretix_saferpay/templates/pretix_saferpay/checkout_payment_form.html
```

