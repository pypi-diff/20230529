# Comparing `tmp/pretix-bitpay-1.5.1.tar.gz` & `tmp/pretix-bitpay-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-bitpay-1.5.1.tar", last modified: Mon Jan 30 14:42:35 2023, max compression
+gzip compressed data, was "pretix-bitpay-1.5.2.tar", last modified: Sun May 28 23:05:17 2023, max compression
```

## Comparing `pretix-bitpay-1.5.1.tar` & `pretix-bitpay-1.5.2.tar`

### file list

```diff
@@ -1,122 +1,126 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.906243 pretix-bitpay-1.5.1/
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1220 2023-01-30 14:42:35.906243 pretix-bitpay-1.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      890 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.894243 pretix-bitpay-1.5.1/pretix_bitpay/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-30 14:13:10.000000 pretix-bitpay-1.5.1/pretix_bitpay/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      890 2023-01-30 14:13:10.000000 pretix-bitpay-1.5.1/pretix_bitpay/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.894243 pretix-bitpay-1.5.1/pretix_bitpay/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.882242 pretix-bitpay-1.5.1/pretix_bitpay/locale/ar/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.894243 pretix-bitpay-1.5.1/pretix_bitpay/locale/ar/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5256 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.882242 pretix-bitpay-1.5.1/pretix_bitpay/locale/ca/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.894243 pretix-bitpay-1.5.1/pretix_bitpay/locale/ca/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5256 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.882242 pretix-bitpay-1.5.1/pretix_bitpay/locale/cs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.894243 pretix-bitpay-1.5.1/pretix_bitpay/locale/cs/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5256 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.882242 pretix-bitpay-1.5.1/pretix_bitpay/locale/da/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.894243 pretix-bitpay-1.5.1/pretix_bitpay/locale/da/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5256 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.886242 pretix-bitpay-1.5.1/pretix_bitpay/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.894243 pretix-bitpay-1.5.1/pretix_bitpay/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10846 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.894243 pretix-bitpay-1.5.1/pretix_bitpay/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.894243 pretix-bitpay-1.5.1/pretix_bitpay/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10762 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     5281 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/django.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.886242 pretix-bitpay-1.5.1/pretix_bitpay/locale/el/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.894243 pretix-bitpay-1.5.1/pretix_bitpay/locale/el/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     7098 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.886242 pretix-bitpay-1.5.1/pretix_bitpay/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.898243 pretix-bitpay-1.5.1/pretix_bitpay/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     6261 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.886242 pretix-bitpay-1.5.1/pretix_bitpay/locale/fi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.898243 pretix-bitpay-1.5.1/pretix_bitpay/locale/fi/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     6378 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.886242 pretix-bitpay-1.5.1/pretix_bitpay/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.898243 pretix-bitpay-1.5.1/pretix_bitpay/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     8984 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.886242 pretix-bitpay-1.5.1/pretix_bitpay/locale/it/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.898243 pretix-bitpay-1.5.1/pretix_bitpay/locale/it/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5669 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.886242 pretix-bitpay-1.5.1/pretix_bitpay/locale/ja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.898243 pretix-bitpay-1.5.1/pretix_bitpay/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5256 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.886242 pretix-bitpay-1.5.1/pretix_bitpay/locale/lv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.898243 pretix-bitpay-1.5.1/pretix_bitpay/locale/lv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5763 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.886242 pretix-bitpay-1.5.1/pretix_bitpay/locale/nl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.898243 pretix-bitpay-1.5.1/pretix_bitpay/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10536 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.886242 pretix-bitpay-1.5.1/pretix_bitpay/locale/nl_BE/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.898243 pretix-bitpay-1.5.1/pretix_bitpay/locale/nl_BE/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5259 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/nl_BE/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.886242 pretix-bitpay-1.5.1/pretix_bitpay/locale/nl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.898243 pretix-bitpay-1.5.1/pretix_bitpay/locale/nl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     8175 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/nl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.886242 pretix-bitpay-1.5.1/pretix_bitpay/locale/pl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.898243 pretix-bitpay-1.5.1/pretix_bitpay/locale/pl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5503 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.886242 pretix-bitpay-1.5.1/pretix_bitpay/locale/pl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.898243 pretix-bitpay-1.5.1/pretix_bitpay/locale/pl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5265 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/pl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.886242 pretix-bitpay-1.5.1/pretix_bitpay/locale/pt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.898243 pretix-bitpay-1.5.1/pretix_bitpay/locale/pt/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5256 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.886242 pretix-bitpay-1.5.1/pretix_bitpay/locale/pt_BR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.898243 pretix-bitpay-1.5.1/pretix_bitpay/locale/pt_BR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5259 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.886242 pretix-bitpay-1.5.1/pretix_bitpay/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.898243 pretix-bitpay-1.5.1/pretix_bitpay/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5256 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.886242 pretix-bitpay-1.5.1/pretix_bitpay/locale/si/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.902243 pretix-bitpay-1.5.1/pretix_bitpay/locale/si/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     6411 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/si/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.886242 pretix-bitpay-1.5.1/pretix_bitpay/locale/sl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.902243 pretix-bitpay-1.5.1/pretix_bitpay/locale/sl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5256 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.890242 pretix-bitpay-1.5.1/pretix_bitpay/locale/sv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.902243 pretix-bitpay-1.5.1/pretix_bitpay/locale/sv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5427 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.890242 pretix-bitpay-1.5.1/pretix_bitpay/locale/tr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.902243 pretix-bitpay-1.5.1/pretix_bitpay/locale/tr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10406 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.890242 pretix-bitpay-1.5.1/pretix_bitpay/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.902243 pretix-bitpay-1.5.1/pretix_bitpay/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5643 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.902243 pretix-bitpay-1.5.1/pretix_bitpay/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/migrations/0002_referencedbitpayobject_payment.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      336 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/models.py
--rw-rw-rw-   0 root         (0) root         (0)    11373 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/payment.py
--rw-rw-rw-   0 root         (0) root         (0)     1427 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.890242 pretix-bitpay-1.5.1/pretix_bitpay/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.902243 pretix-bitpay-1.5.1/pretix_bitpay/static/pretix_bitpay/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/static/pretix_bitpay/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     4759 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/static/pretix_bitpay/bitpay-logo.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.890242 pretix-bitpay-1.5.1/pretix_bitpay/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.906243 pretix-bitpay-1.5.1/pretix_bitpay/templates/pretix_bitpay/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/templates/pretix_bitpay/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      668 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/templates/pretix_bitpay/action_overpaid.html
--rw-rw-rw-   0 root         (0) root         (0)      557 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/templates/pretix_bitpay/action_refund.html
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/templates/pretix_bitpay/checkout_payment_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/templates/pretix_bitpay/checkout_payment_form.html
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/templates/pretix_bitpay/control.html
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/templates/pretix_bitpay/control_refund.html
--rw-rw-rw-   0 root         (0) root         (0)      210 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/templates/pretix_bitpay/pending.html
--rw-rw-rw-   0 root         (0) root         (0)     1044 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/templates/pretix_bitpay/redirect.html
--rw-rw-rw-   0 root         (0) root         (0)      787 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     9350 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/pretix_bitpay/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:42:35.894243 pretix-bitpay-1.5.1/pretix_bitpay.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1220 2023-01-30 14:42:35.000000 pretix-bitpay-1.5.1/pretix_bitpay.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2493 2023-01-30 14:42:35.000000 pretix-bitpay-1.5.1/pretix_bitpay.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-30 14:42:35.000000 pretix-bitpay-1.5.1/pretix_bitpay.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-01-30 14:42:35.000000 pretix-bitpay-1.5.1/pretix_bitpay.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-01-30 14:42:35.000000 pretix-bitpay-1.5.1/pretix_bitpay.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-01-30 14:42:35.000000 pretix-bitpay-1.5.1/pretix_bitpay.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-01-30 14:42:35.910243 pretix-bitpay-1.5.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1155 2023-01-30 13:14:57.000000 pretix-bitpay-1.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.748228 pretix-bitpay-1.5.2/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-05-28 23:05:17.748228 pretix-bitpay-1.5.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.728227 pretix-bitpay-1.5.2/pretix_bitpay/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      910 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.732227 pretix-bitpay-1.5.2/pretix_bitpay/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.720227 pretix-bitpay-1.5.2/pretix_bitpay/locale/ar/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.732227 pretix-bitpay-1.5.2/pretix_bitpay/locale/ar/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5256 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.720227 pretix-bitpay-1.5.2/pretix_bitpay/locale/ca/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.732227 pretix-bitpay-1.5.2/pretix_bitpay/locale/ca/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5256 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.720227 pretix-bitpay-1.5.2/pretix_bitpay/locale/cs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.732227 pretix-bitpay-1.5.2/pretix_bitpay/locale/cs/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     8237 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.720227 pretix-bitpay-1.5.2/pretix_bitpay/locale/da/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.732227 pretix-bitpay-1.5.2/pretix_bitpay/locale/da/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5256 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.720227 pretix-bitpay-1.5.2/pretix_bitpay/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.732227 pretix-bitpay-1.5.2/pretix_bitpay/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10846 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.732227 pretix-bitpay-1.5.2/pretix_bitpay/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:04:49.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.732227 pretix-bitpay-1.5.2/pretix_bitpay/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10762 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     5281 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/django.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.720227 pretix-bitpay-1.5.2/pretix_bitpay/locale/el/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.732227 pretix-bitpay-1.5.2/pretix_bitpay/locale/el/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     7098 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.720227 pretix-bitpay-1.5.2/pretix_bitpay/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.732227 pretix-bitpay-1.5.2/pretix_bitpay/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     6261 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.724227 pretix-bitpay-1.5.2/pretix_bitpay/locale/fi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.732227 pretix-bitpay-1.5.2/pretix_bitpay/locale/fi/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     6378 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.724227 pretix-bitpay-1.5.2/pretix_bitpay/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.732227 pretix-bitpay-1.5.2/pretix_bitpay/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     9280 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.724227 pretix-bitpay-1.5.2/pretix_bitpay/locale/hr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.732227 pretix-bitpay-1.5.2/pretix_bitpay/locale/hr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5256 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.724227 pretix-bitpay-1.5.2/pretix_bitpay/locale/it/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.736227 pretix-bitpay-1.5.2/pretix_bitpay/locale/it/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5666 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.724227 pretix-bitpay-1.5.2/pretix_bitpay/locale/ja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.736227 pretix-bitpay-1.5.2/pretix_bitpay/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5256 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.724227 pretix-bitpay-1.5.2/pretix_bitpay/locale/lv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.736227 pretix-bitpay-1.5.2/pretix_bitpay/locale/lv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5763 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.724227 pretix-bitpay-1.5.2/pretix_bitpay/locale/nl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.736227 pretix-bitpay-1.5.2/pretix_bitpay/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10536 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.724227 pretix-bitpay-1.5.2/pretix_bitpay/locale/nl_BE/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.736227 pretix-bitpay-1.5.2/pretix_bitpay/locale/nl_BE/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5259 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/nl_BE/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.724227 pretix-bitpay-1.5.2/pretix_bitpay/locale/nl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.736227 pretix-bitpay-1.5.2/pretix_bitpay/locale/nl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     8175 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/nl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.724227 pretix-bitpay-1.5.2/pretix_bitpay/locale/pl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.736227 pretix-bitpay-1.5.2/pretix_bitpay/locale/pl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.724227 pretix-bitpay-1.5.2/pretix_bitpay/locale/pl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.736227 pretix-bitpay-1.5.2/pretix_bitpay/locale/pl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5265 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/pl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.724227 pretix-bitpay-1.5.2/pretix_bitpay/locale/pt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.736227 pretix-bitpay-1.5.2/pretix_bitpay/locale/pt/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5256 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.724227 pretix-bitpay-1.5.2/pretix_bitpay/locale/pt_BR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.736227 pretix-bitpay-1.5.2/pretix_bitpay/locale/pt_BR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5259 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.724227 pretix-bitpay-1.5.2/pretix_bitpay/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.740228 pretix-bitpay-1.5.2/pretix_bitpay/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5256 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.724227 pretix-bitpay-1.5.2/pretix_bitpay/locale/si/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.740228 pretix-bitpay-1.5.2/pretix_bitpay/locale/si/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     6411 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/si/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.724227 pretix-bitpay-1.5.2/pretix_bitpay/locale/sl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.740228 pretix-bitpay-1.5.2/pretix_bitpay/locale/sl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5256 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.724227 pretix-bitpay-1.5.2/pretix_bitpay/locale/sv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.740228 pretix-bitpay-1.5.2/pretix_bitpay/locale/sv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5427 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.724227 pretix-bitpay-1.5.2/pretix_bitpay/locale/tr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.740228 pretix-bitpay-1.5.2/pretix_bitpay/locale/tr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10406 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.724227 pretix-bitpay-1.5.2/pretix_bitpay/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.740228 pretix-bitpay-1.5.2/pretix_bitpay/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5643 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.740228 pretix-bitpay-1.5.2/pretix_bitpay/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/migrations/0002_referencedbitpayobject_payment.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:04:49.000000 pretix-bitpay-1.5.2/pretix_bitpay/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      350 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    13195 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1428 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.724227 pretix-bitpay-1.5.2/pretix_bitpay/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.740228 pretix-bitpay-1.5.2/pretix_bitpay/static/pretix_bitpay/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:04:49.000000 pretix-bitpay-1.5.2/pretix_bitpay/static/pretix_bitpay/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     4759 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/static/pretix_bitpay/bitpay-logo.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.724227 pretix-bitpay-1.5.2/pretix_bitpay/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.748228 pretix-bitpay-1.5.2/pretix_bitpay/templates/pretix_bitpay/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:04:49.000000 pretix-bitpay-1.5.2/pretix_bitpay/templates/pretix_bitpay/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      668 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/templates/pretix_bitpay/action_overpaid.html
+-rw-rw-rw-   0 root         (0) root         (0)      557 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/templates/pretix_bitpay/action_refund.html
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/templates/pretix_bitpay/checkout_payment_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/templates/pretix_bitpay/checkout_payment_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/templates/pretix_bitpay/control.html
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/templates/pretix_bitpay/control_refund.html
+-rw-rw-rw-   0 root         (0) root         (0)      210 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/templates/pretix_bitpay/pending.html
+-rw-rw-rw-   0 root         (0) root         (0)     1044 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/templates/pretix_bitpay/redirect.html
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    10256 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pretix_bitpay/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:17.728227 pretix-bitpay-1.5.2/pretix_bitpay.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-05-28 23:05:17.000000 pretix-bitpay-1.5.2/pretix_bitpay.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2554 2023-05-28 23:05:17.000000 pretix-bitpay-1.5.2/pretix_bitpay.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 23:05:17.000000 pretix-bitpay-1.5.2/pretix_bitpay.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      131 2023-05-28 23:05:17.000000 pretix-bitpay-1.5.2/pretix_bitpay.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-28 23:05:17.000000 pretix-bitpay-1.5.2/pretix_bitpay.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-28 23:05:17.000000 pretix-bitpay-1.5.2/pretix_bitpay.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      983 2023-05-28 08:29:08.000000 pretix-bitpay-1.5.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      857 2023-05-28 23:05:17.748228 pretix-bitpay-1.5.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-28 23:04:49.000000 pretix-bitpay-1.5.2/setup.py
```

### Comparing `pretix-bitpay-1.5.1/LICENSE` & `pretix-bitpay-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/PKG-INFO` & `pretix-bitpay-1.5.2/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,22 @@
-Metadata-Version: 2.1
-Name: pretix-bitpay
-Version: 1.5.1
-Summary: This plugin allows accepting crypto currency payments in pretix via BitPay-compatible payment providers.
-Home-page: https://github.com/pretix/pretix-bitpay
-Author: Raphael Michel
-Author-email: michel@rami.io
-License: Apache Software License
-License-File: LICENSE
-
 BitPay payments
 ==========================
 
 This is a plugin for `pretix`_. 
 
 Development setup
 -----------------
 
 1. Make sure that you have a working `pretix development setup`_.
 
 2. Clone this repository, eg to ``local/pretix-bitpay``.
 
 3. Activate the virtual environment you use for pretix development.
 
-4. Execute ``python setup.py develop`` within this directory to register this application with pretix's plugin registry.
+4. Execute ``pip install -e .`` within this directory to register this application with pretix's plugin registry.
 
 5. Execute ``make`` within this directory to compile translations.
 
 6. Restart your local pretix server. You can now use the plugin from this repository for your events by enabling it in
    the 'plugins' tab in the settings.
```

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/apps.py` & `pretix-bitpay-1.5.2/pretix_bitpay/apps.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 from django.utils.functional import cached_property
 from django.utils.translation import gettext_lazy as _
 
 from . import __version__
 
 
 class BitpayApp(AppConfig):
-    name = 'pretix_bitpay'
+    name = "pretix_bitpay"
     verbose_name = _("BitPay")
 
     class PretixPluginMeta:
         name = _("BitPay")
         author = "Raphael Michel"
-        category = 'PAYMENT'
+        category = "PAYMENT"
         version = __version__
         compatibility = "pretix>=4.16.0"
-        description = _("Receive Crypto payments via BitPay-compatible payment providers.")
+        description = _(
+            "Receive Crypto payments via BitPay-compatible payment providers."
+        )
         picture = "pretix_bitpay/bitpay-logo.svg"
 
     def ready(self):
         from . import signals  # NOQA
 
     @cached_property
     def compatibility_errors(self):
         errs = []
         try:
             import btcpay  # NOQA
         except ImportError:
             errs.append("Python package 'btcpay' is not installed.")
         return errs
-
-
```

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/ar/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/ca/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/cs/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/nl_BE/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-03-21 15:17+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: cs\n"
+"Language: nl_BE\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_bitpay/__init__.py:10 pretix_bitpay/__init__.py:13
 #: pretix_bitpay/payment.py:32
 msgid "BitPay"
```

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/da/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/de/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/django.pot` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/el/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/es/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/fi/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/fr/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/fr/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,33 +4,35 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-03-21 15:17+0100\n"
-"PO-Revision-Date: 2019-10-01 01:00+0000\n"
-"Last-Translator: Fabian Rodriguez <magicfab@legoutdulibre.com>\n"
-"Language-Team: French <https://translate.pretix.eu/projects/pretix/pretix-"
-"plugin-bitpay/fr/>\n"
+"PO-Revision-Date: 2023-01-16 23:00+0000\n"
+"Last-Translator: Maurice Kaag <maurice@kaag.me>\n"
+"Language-Team: French <https://translate.pretix.eu/projects/pretix/"
+"pretix-plugin-bitpay/fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 3.5.1\n"
+"X-Generator: Weblate 4.15\n"
 
 #: pretix_bitpay/__init__.py:10 pretix_bitpay/__init__.py:13
 #: pretix_bitpay/payment.py:32
 msgid "BitPay"
 msgstr "BitPay"
 
 #: pretix_bitpay/__init__.py:17
 msgid "Receive Crypto payments via BitPay-compatible payment providers."
 msgstr ""
+"Recevez des paiements en crypto-monnaies via des fournisseurs de paiement "
+"compatibles avec BitPay."
 
 #: pretix_bitpay/payment.py:36
 msgid "Crypto"
 msgstr "Crypto"
 
 #: pretix_bitpay/payment.py:54
 msgid ""
@@ -49,18 +51,14 @@
 msgstr "Connecter avec BitPay"
 
 #: pretix_bitpay/payment.py:66
 msgid "Connect with test.bitpay.com"
 msgstr "Se connecter avec test.bitpay.com"
 
 #: pretix_bitpay/payment.py:67
-#, fuzzy
-#| msgid ""
-#| "Alternatively, you can connect with a third-party provider using a BitPay-"
-#| "compatible API. Enterthe URL here you want to connect to."
 msgid ""
 "Alternatively, you can connect with a third-party provider using a BitPay-"
 "compatible API. Enter the URL here you want to connect to."
 msgstr ""
 "Vous pouvez aussi vous connecter avec un fournisseur tiers utilisant une API "
 "compatible avec BitPay. Entrez l'URL à laquelle vous souhaitez vous "
 "connecter."
@@ -75,52 +73,57 @@
 
 #: pretix_bitpay/payment.py:94
 msgid "API URL"
 msgstr "URL API"
 
 #: pretix_bitpay/payment.py:98
 msgid "Payment method name"
-msgstr ""
+msgstr "Nom du mode de paiement"
 
 #: pretix_bitpay/payment.py:101
 msgid ""
 "Since you can accept a variety of different Crypto coins with BitPay and "
 "BitPay-compatible services, you can set the name of the payment method here "
 "to reflect the coins you are actually accepting."
 msgstr ""
+"Étant donné que vous pouvez accepter plusieurs crypto-monnaies avec BitPay "
+"et les services compatibles BitPay, vous pouvez définir le nom de la méthode "
+"de paiement ici pour refléter la monnaie que vous acceptez réellement."
 
 #: pretix_bitpay/payment.py:142
 msgid ""
 "The BitPay plugin is operating in test mode. No money will actually be "
 "transferred."
 msgstr ""
+"Le plugin BitPay fonctionne en mode test. Aucune somme d'argent ne sera "
+"réellement transférée."
 
 #: pretix_bitpay/payment.py:171 pretix_bitpay/payment.py:215
 msgid ""
 "We had trouble communicating with BitPay. Please try again and get in touch "
 "with us if this problem persists."
 msgstr ""
 "Nous avons eu du mal à communiquer avec BitPay. Veuillez réessayer et "
 "prendre contact avec nous si le problème persiste."
 
 #: pretix_bitpay/payment.py:224
 msgid "BitPay reported an error: {}"
-msgstr "BitPay a signalé une erreur: {}"
+msgstr "BitPay a signalé une erreur : {}"
 
 #: pretix_bitpay/payment.py:231
 msgid ""
 "We had trouble communicating with BitPay. Please try again and contact "
 "support if the problem persists."
 msgstr ""
 "Nous avons eu du mal à communiquer avec BitPay. Veuillez réessayer et "
 "prendre contact avec nous si le problème persiste."
 
 #: pretix_bitpay/signals.py:25
 msgid "BitPay reported an event: {}"
-msgstr "BitPay a rapporté un événement: {}"
+msgstr "BitPay a rapporté un événement : {}"
 
 #: pretix_bitpay/templates/pretix_bitpay/action_overpaid.html:5
 #, python-format
 msgid ""
 "The BitPay invoice <a %(bp_href)s>%(charge)s</a> has succeeded, but the "
 "order %(order)s is expired and the product was sold out in the meantime. "
 "Therefore, the payment could not be accepted. Please contact the user and "
@@ -187,16 +190,16 @@
 #: pretix_bitpay/templates/pretix_bitpay/redirect.html:17
 msgid "The payment process has started in a new window."
 msgstr "Le processus de paiement a démarré dans une autre fenêtre."
 
 #: pretix_bitpay/templates/pretix_bitpay/redirect.html:20
 msgid "The window to enter your payment data was not opened or was closed?"
 msgstr ""
-"La fenêtre de saisie de vos données de paiement n' a pas été ouverte ou a "
-"été fermée"
+"La fenêtre de saisie de vos données de paiement a-t-elle été fermée ou ne "
+"s'est pas ouverte ?"
 
 #: pretix_bitpay/templates/pretix_bitpay/redirect.html:24
 msgid "Click here in order to open the window."
 msgstr "Cliquez ici pour ouvrir la fenêtre."
 
 #: pretix_bitpay/views.py:125
 msgid "Your BitPay account has been disconnected."
```

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/it/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/pl/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-03-21 15:17+0100\n"
-"PO-Revision-Date: 2020-06-24 15:00+0000\n"
-"Last-Translator: Frank <webappconcept@gmail.com>\n"
-"Language-Team: Italian <https://translate.pretix.eu/projects/pretix/pretix-"
-"plugin-bitpay/it/>\n"
-"Language: it\n"
+"PO-Revision-Date: 2022-11-06 06:00+0000\n"
+"Last-Translator: Maciej Szymczak <maciej+github@szymczak.at>\n"
+"Language-Team: Polish <https://translate.pretix.eu/projects/pretix/"
+"pretix-plugin-bitpay/pl/>\n"
+"Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 3.10.3\n"
+"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
+"|| n%100>=20) ? 1 : 2;\n"
+"X-Generator: Weblate 4.14.1\n"
 
 #: pretix_bitpay/__init__.py:10 pretix_bitpay/__init__.py:13
 #: pretix_bitpay/payment.py:32
 msgid "BitPay"
 msgstr ""
 
 #: pretix_bitpay/__init__.py:17
@@ -126,19 +127,19 @@
 "After you submitted your order, we will redirect you to a payment partner to "
 "complete your payment. You will then be redirected back here to get your "
 "tickets."
 msgstr ""
 
 #: pretix_bitpay/templates/pretix_bitpay/control.html:6
 msgid "Invoice ID"
-msgstr ""
+msgstr "Numer faktury"
 
 #: pretix_bitpay/templates/pretix_bitpay/control.html:8
 msgid "Status"
-msgstr "Stato"
+msgstr ""
 
 #: pretix_bitpay/templates/pretix_bitpay/control.html:14
 msgid "Error message"
 msgstr ""
 
 #: pretix_bitpay/templates/pretix_bitpay/control_refund.html:5
 msgid ""
@@ -151,36 +152,33 @@
 msgid ""
 "We're waiting for an answer from the payment provider regarding your "
 "payment. Please contact us if this takes more than a few hours."
 msgstr ""
 
 #: pretix_bitpay/templates/pretix_bitpay/redirect.html:17
 msgid "The payment process has started in a new window."
-msgstr "Il processo di pagamento è stato inziato in una nuova finestra."
+msgstr ""
 
 #: pretix_bitpay/templates/pretix_bitpay/redirect.html:20
 msgid "The window to enter your payment data was not opened or was closed?"
 msgstr ""
-"La finestra di inserimento dati di PayPal non è stata aperta o si è chiusa?"
 
 #: pretix_bitpay/templates/pretix_bitpay/redirect.html:24
 msgid "Click here in order to open the window."
 msgstr ""
 
 #: pretix_bitpay/views.py:125
 msgid "Your BitPay account has been disconnected."
 msgstr ""
 
 #: pretix_bitpay/views.py:175
 msgid ""
 "Sorry, there was an error in the payment process. Please check the link in "
 "your emails to continue."
 msgstr ""
-"Spiacenti, c'è stato un problema durante il pagamento. Segui il link "
-"nell'email per continuare."
 
 #: pretix_bitpay/views.py:190
 msgid "You are already connected to BitPay."
 msgstr ""
 
 #: pretix_bitpay/views.py:216 pretix_bitpay/views.py:225
 msgid "Communication with BitPay was not successful."
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/ja/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/lv/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/nl/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/nl_BE/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/ru/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-03-21 15:17+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: nl_BE\n"
+"Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_bitpay/__init__.py:10 pretix_bitpay/__init__.py:13
 #: pretix_bitpay/payment.py:32
 msgid "BitPay"
```

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/nl_Informal/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/nl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/pl/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/pl_Informal/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,21 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-03-21 15:17+0100\n"
-"PO-Revision-Date: 2022-11-06 06:00+0000\n"
-"Last-Translator: Maciej Szymczak <maciej+github@szymczak.at>\n"
-"Language-Team: Polish <https://translate.pretix.eu/projects/pretix/"
-"pretix-plugin-bitpay/pl/>\n"
-"Language: pl\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: Automatically generated\n"
+"Language-Team: none\n"
+"Language: pl_Informal\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
-"|| n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.14.1\n"
 
 #: pretix_bitpay/__init__.py:10 pretix_bitpay/__init__.py:13
 #: pretix_bitpay/payment.py:32
 msgid "BitPay"
 msgstr ""
 
 #: pretix_bitpay/__init__.py:17
@@ -127,15 +123,15 @@
 "After you submitted your order, we will redirect you to a payment partner to "
 "complete your payment. You will then be redirected back here to get your "
 "tickets."
 msgstr ""
 
 #: pretix_bitpay/templates/pretix_bitpay/control.html:6
 msgid "Invoice ID"
-msgstr "Numer faktury"
+msgstr ""
 
 #: pretix_bitpay/templates/pretix_bitpay/control.html:8
 msgid "Status"
 msgstr ""
 
 #: pretix_bitpay/templates/pretix_bitpay/control.html:14
 msgid "Error message"
```

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/pl_Informal/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/sl/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-03-21 15:17+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: pl_Informal\n"
+"Language: sl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_bitpay/__init__.py:10 pretix_bitpay/__init__.py:13
 #: pretix_bitpay/payment.py:32
 msgid "BitPay"
```

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/pt/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/pt_BR/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/ru/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/hr/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-03-21 15:17+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: ru\n"
+"Language: hr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_bitpay/__init__.py:10 pretix_bitpay/__init__.py:13
 #: pretix_bitpay/payment.py:32
 msgid "BitPay"
```

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/si/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/si/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/sl/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/sv/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-03-21 15:17+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: Automatically generated\n"
-"Language-Team: none\n"
-"Language: sl\n"
+"PO-Revision-Date: 2020-09-19 18:00+0000\n"
+"Last-Translator: Tobias Sundgren <syrgas@gmail.com>\n"
+"Language-Team: Swedish <https://translate.pretix.eu/projects/pretix/pretix-"
+"plugin-bitpay/sv/>\n"
+"Language: sv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 3.10.3\n"
 
 #: pretix_bitpay/__init__.py:10 pretix_bitpay/__init__.py:13
 #: pretix_bitpay/payment.py:32
 msgid "BitPay"
 msgstr ""
 
 #: pretix_bitpay/__init__.py:17
@@ -127,15 +130,15 @@
 
 #: pretix_bitpay/templates/pretix_bitpay/control.html:6
 msgid "Invoice ID"
 msgstr ""
 
 #: pretix_bitpay/templates/pretix_bitpay/control.html:8
 msgid "Status"
-msgstr ""
+msgstr "Status"
 
 #: pretix_bitpay/templates/pretix_bitpay/control.html:14
 msgid "Error message"
 msgstr ""
 
 #: pretix_bitpay/templates/pretix_bitpay/control_refund.html:5
 msgid ""
```

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/sv/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/it/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-03-21 15:17+0100\n"
-"PO-Revision-Date: 2020-09-19 18:00+0000\n"
-"Last-Translator: Tobias Sundgren <syrgas@gmail.com>\n"
-"Language-Team: Swedish <https://translate.pretix.eu/projects/pretix/pretix-"
-"plugin-bitpay/sv/>\n"
-"Language: sv\n"
+"PO-Revision-Date: 2023-05-18 01:00+0000\n"
+"Last-Translator: M C <micasadmail@gmail.com>\n"
+"Language-Team: Italian <https://translate.pretix.eu/projects/pretix/"
+"pretix-plugin-bitpay/it/>\n"
+"Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 3.10.3\n"
+"X-Generator: Weblate 4.17\n"
 
 #: pretix_bitpay/__init__.py:10 pretix_bitpay/__init__.py:13
 #: pretix_bitpay/payment.py:32
 msgid "BitPay"
 msgstr ""
 
 #: pretix_bitpay/__init__.py:17
@@ -130,15 +130,15 @@
 
 #: pretix_bitpay/templates/pretix_bitpay/control.html:6
 msgid "Invoice ID"
 msgstr ""
 
 #: pretix_bitpay/templates/pretix_bitpay/control.html:8
 msgid "Status"
-msgstr "Status"
+msgstr "Stato"
 
 #: pretix_bitpay/templates/pretix_bitpay/control.html:14
 msgid "Error message"
 msgstr ""
 
 #: pretix_bitpay/templates/pretix_bitpay/control_refund.html:5
 msgid ""
@@ -151,33 +151,37 @@
 msgid ""
 "We're waiting for an answer from the payment provider regarding your "
 "payment. Please contact us if this takes more than a few hours."
 msgstr ""
 
 #: pretix_bitpay/templates/pretix_bitpay/redirect.html:17
 msgid "The payment process has started in a new window."
-msgstr ""
+msgstr "Il processo di pagamento è stato inziato in una nuova finestra."
 
 #: pretix_bitpay/templates/pretix_bitpay/redirect.html:20
+#, fuzzy
 msgid "The window to enter your payment data was not opened or was closed?"
 msgstr ""
+"La finestra per inserire i dati di pagamento non era aperta o era chiusa?"
 
 #: pretix_bitpay/templates/pretix_bitpay/redirect.html:24
 msgid "Click here in order to open the window."
 msgstr ""
 
 #: pretix_bitpay/views.py:125
 msgid "Your BitPay account has been disconnected."
 msgstr ""
 
 #: pretix_bitpay/views.py:175
 msgid ""
 "Sorry, there was an error in the payment process. Please check the link in "
 "your emails to continue."
 msgstr ""
+"Spiacenti, c'è stato un errore durante il pagamento. Segui il link "
+"nell'email per continuare."
 
 #: pretix_bitpay/views.py:190
 msgid "You are already connected to BitPay."
 msgstr ""
 
 #: pretix_bitpay/views.py:216 pretix_bitpay/views.py:225
 msgid "Communication with BitPay was not successful."
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/tr/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/locale/zh_Hans/LC_MESSAGES/django.po` & `pretix-bitpay-1.5.2/pretix_bitpay/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/migrations/0002_referencedbitpayobject_payment.py` & `pretix-bitpay-1.5.2/pretix_bitpay/migrations/0002_referencedbitpayobject_payment.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,20 +3,24 @@
 from __future__ import unicode_literals
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ('pretixbase', '0097_auto_20180722_0804'),
-        ('pretix_bitpay', '0001_initial'),
+        ("pretixbase", "0097_auto_20180722_0804"),
+        ("pretix_bitpay", "0001_initial"),
     ]
 
     operations = [
         migrations.AddField(
-            model_name='referencedbitpayobject',
-            name='payment',
-            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.CASCADE, to='pretixbase.OrderPayment'),
+            model_name="referencedbitpayobject",
+            name="payment",
+            field=models.ForeignKey(
+                blank=True,
+                null=True,
+                on_delete=django.db.models.deletion.CASCADE,
+                to="pretixbase.OrderPayment",
+            ),
         ),
     ]
```

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/payment.py` & `pretix-bitpay-1.5.2/pretix_bitpay/payment.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Union
 
 import hashlib
 import json
 import logging
 import requests
-import urllib
 from collections import OrderedDict
 from django import forms
 from django.core import signing
 from django.http import HttpRequest
 from django.template.loader import get_template
 from django.urls import reverse
 from django.utils.functional import cached_property
@@ -23,20 +22,22 @@
 
 from .models import ReferencedBitPayObject
 
 logger = logging.getLogger(__name__)
 
 
 class BitPay(BasePaymentProvider):
-    identifier = 'bitpay'
-    verbose_name = _('BitPay')
+    identifier = "bitpay"
+    verbose_name = _("BitPay")
 
     @property
     def public_name(self):
-        return str(self.settings.get('public_name', as_type=LazyI18nString) or _('Crypto'))
+        return str(
+            self.settings.get("public_name", as_type=LazyI18nString) or _("Crypto")
+        )
 
     def settings_content_render(self, request):
         if not self.settings.token:
             return (
                 "<p>{}</p>"
                 "<p>"
                 "<a href='{}' target='_blank' class='btn btn-primary btn-lg'>{}</a> "
@@ -46,212 +47,313 @@
                 "</form>"  # This is a hell of a hack, sorry…
                 "<form class='form-inline' action='{}' method='GET' target='_blank'>"
                 "<input type='text' name='url' class='form-control' value='https://btcpay.lightbo.lt'> "
                 "<button class='btn btn-default'>{}</button>"
                 "</form>"
                 "<form>"
             ).format(
-                _('To accept payments via BitPay, you will need an account at BitPay. By clicking on the '
-                  'following button, you can connect pretix to your BitPay account. A BitPay site will open in a new '
-                  'tab. Return to this page and refresh it after you authorized the token at BitPay.'),
-                reverse('plugins:pretix_bitpay:auth.start', kwargs={
-                    'organizer': self.event.organizer.slug,
-                    'event': self.event.slug,
-                }),
-                _('Connect with BitPay'),
-                reverse('plugins:pretix_bitpay:auth.start', kwargs={
-                    'organizer': self.event.organizer.slug,
-                    'event': self.event.slug,
-                }) + '?test=1',
-                _('Connect with test.bitpay.com'),
-                _('Alternatively, you can connect with a third-party provider using a BitPay-compatible API. Enter '
-                  'the URL here you want to connect to.'),
-                reverse('plugins:pretix_bitpay:auth.start', kwargs={
-                    'organizer': self.event.organizer.slug,
-                    'event': self.event.slug,
-                }),
-                _('Start pairing')
+                _(
+                    "To accept payments via BitPay, you will need an account at BitPay. By clicking on the "
+                    "following button, you can connect pretix to your BitPay account. A BitPay site will open in a new "
+                    "tab. Return to this page and refresh it after you authorized the token at BitPay."
+                ),
+                reverse(
+                    "plugins:pretix_bitpay:auth.start",
+                    kwargs={
+                        "organizer": self.event.organizer.slug,
+                        "event": self.event.slug,
+                    },
+                ),
+                _("Connect with BitPay"),
+                reverse(
+                    "plugins:pretix_bitpay:auth.start",
+                    kwargs={
+                        "organizer": self.event.organizer.slug,
+                        "event": self.event.slug,
+                    },
+                )
+                + "?test=1",
+                _("Connect with test.bitpay.com"),
+                _(
+                    "Alternatively, you can connect with a third-party provider using a BitPay-compatible API. Enter "
+                    "the URL here you want to connect to."
+                ),
+                reverse(
+                    "plugins:pretix_bitpay:auth.start",
+                    kwargs={
+                        "organizer": self.event.organizer.slug,
+                        "event": self.event.slug,
+                    },
+                ),
+                _("Start pairing"),
             )
         else:
             return (
                 "<button formaction='{}' class='btn btn-danger'>{}</button>"
             ).format(
-                reverse('plugins:pretix_bitpay:auth.disconnect', kwargs={
-                    'organizer': self.event.organizer.slug,
-                    'event': self.event.slug,
-                }),
-                _('Disconnect from BitPay')
+                reverse(
+                    "plugins:pretix_bitpay:auth.disconnect",
+                    kwargs={
+                        "organizer": self.event.organizer.slug,
+                        "event": self.event.slug,
+                    },
+                ),
+                _("Disconnect from BitPay"),
             )
 
     @property
     def settings_form_fields(self):
         if not self.settings.token:
             return {}
         d = OrderedDict(
             [
-                ('url',
-                 forms.CharField(
-                     label=_('API URL'),
-                     disabled=True
-                 )),
-                ('public_name', I18nFormField(
-                    label=_('Payment method name'),
-                    widget=I18nTextInput,
-                    help_text=_(
-                        'Since you can accept a variety of different Crypto coins with BitPay and BitPay-compatible '
-                        'services, you can set the name of the payment method here to reflect the coins you are '
-                        'actually accepting.'
-                    )
-                )),
-            ] + list(super().settings_form_fields.items())
+                ("url", forms.CharField(label=_("API URL"), disabled=True)),
+                (
+                    "public_name",
+                    I18nFormField(
+                        label=_("Payment method name"),
+                        widget=I18nTextInput,
+                        help_text=_(
+                            "Since you can accept a variety of different Crypto coins with BitPay and BitPay-compatible "
+                            "services, you can set the name of the payment method here to reflect the coins you are "
+                            "actually accepting."
+                        ),
+                    ),
+                ),
+            ]
+            + list(super().settings_form_fields.items())
         )
 
-        d.move_to_end('public_name', last=False)
-        d.move_to_end('_enabled', last=False)
+        d.move_to_end("public_name", last=False)
+        d.move_to_end("_enabled", last=False)
         return d
 
     def redirect(self, request, url):
-        if request.session.get('iframe_session', False):
+        if request.session.get("iframe_session", False):
             return (
-                build_absolute_uri(request.event, 'plugins:pretix_bitpay:redirect') +
-                '?data=' + signing.dumps({
-                    'url': url,
-                    'session': {
-                        'payment_bitpay_order_secret': request.session['payment_bitpay_order_secret'],
+                build_absolute_uri(request.event, "plugins:pretix_bitpay:redirect")
+                + "?data="
+                + signing.dumps(
+                    {
+                        "url": url,
+                        "session": {
+                            "payment_bitpay_order_secret": request.session[
+                                "payment_bitpay_order_secret"
+                            ],
+                        },
                     },
-                }, salt='safe-redirect')
+                    salt="safe-redirect",
+                )
             )
         else:
             return str(url)
 
     def payment_form_render(self, request) -> str:
-        template = get_template('pretix_bitpay/checkout_payment_form.html')
-        ctx = {'request': request, 'event': self.event, 'settings': self.settings}
+        template = get_template("pretix_bitpay/checkout_payment_form.html")
+        ctx = {"request": request, "event": self.event, "settings": self.settings}
         return template.render(ctx)
 
     def checkout_confirm_render(self, request) -> str:
-        template = get_template('pretix_bitpay/checkout_payment_confirm.html')
-        ctx = {'request': request, 'event': self.event, 'settings': self.settings}
+        template = get_template("pretix_bitpay/checkout_payment_confirm.html")
+        ctx = {"request": request, "event": self.event, "settings": self.settings}
         return template.render(ctx)
 
     def checkout_prepare(self, request, total):
         return True
 
     def payment_is_valid_session(self, request):
         return True
 
     @property
     def test_mode_message(self):
-        if '//test.bitpay.com' in self.settings.url:
-            return _('The BitPay plugin is operating in test mode. No money will actually be transferred.')
+        if "//test.bitpay.com" in self.settings.url:
+            return _(
+                "The BitPay plugin is operating in test mode. No money will actually be transferred."
+            )
         return None
 
     @cached_property
     def client(self):
         from btcpay import BTCPayClient
-        return BTCPayClient(host=self.settings.url, pem=self.settings.pem, tokens={'merchant': self.settings.token})
+
+        return BTCPayClient(
+            host=self.settings.url,
+            pem=self.settings.pem,
+            tokens={"merchant": self.settings.token},
+        )
 
     def execute_payment(self, request: HttpRequest, payment: OrderPayment):
-        request.session['payment_bitpay_order_secret'] = payment.order.secret
+        request.session["payment_bitpay_order_secret"] = payment.order.secret
 
         try:
-            inv = self.client.create_invoice({
-                "price": float(payment.amount),
-                "currency": self.event.currency,
-                "orderId": payment.order.full_code,
-                "transactionSpeed": "medium",
-                "extendedNotifications": "true",
-                "notificationURL": build_absolute_uri(self.event, "plugins:pretix_bitpay:webhook"),
-                "redirectURL": build_absolute_uri(self.event, "plugins:pretix_bitpay:return", kwargs={
-                    'order': payment.order.code,
-                    'payment': payment.pk,
-                    'hash': hashlib.sha1(payment.order.secret.lower().encode()).hexdigest(),
-                }),
-                # "buyer": {"email": "test@customer.com"},
-                "token": self.settings.token
-            })
+            inv = self.client.create_invoice(
+                {
+                    "price": float(payment.amount),
+                    "currency": self.event.currency,
+                    "orderId": payment.order.full_code,
+                    "transactionSpeed": "medium",
+                    "extendedNotifications": "true",
+                    "notificationURL": build_absolute_uri(
+                        self.event, "plugins:pretix_bitpay:webhook"
+                    ),
+                    "redirectURL": build_absolute_uri(
+                        self.event,
+                        "plugins:pretix_bitpay:return",
+                        kwargs={
+                            "order": payment.order.code,
+                            "payment": payment.pk,
+                            "hash": hashlib.sha1(
+                                payment.order.secret.lower().encode()
+                            ).hexdigest(),
+                        },
+                    ),
+                    # "buyer": {"email": "test@customer.com"},
+                    "token": self.settings.token,
+                }
+            )
         except RequestException:
-            logger.exception('Failure during bitpay payment.')
-            raise PaymentException(_('We had trouble communicating with BitPay. Please try again and get in touch '
-                                     'with us if this problem persists.'))
-        ReferencedBitPayObject.objects.get_or_create(order=payment.order, payment=payment, reference=inv['id'])
+            logger.exception("Failure during bitpay payment.")
+            raise PaymentException(
+                _(
+                    "We had trouble communicating with BitPay. Please try again and get in touch "
+                    "with us if this problem persists."
+                )
+            )
+        ReferencedBitPayObject.objects.get_or_create(
+            order=payment.order, payment=payment, reference=inv["id"]
+        )
         payment.info = json.dumps(inv)
-        payment.save(update_fields=['info'])
-        return self.redirect(request, inv['url'])
+        payment.save(update_fields=["info"])
+        return self.redirect(request, inv["url"])
 
     def payment_pending_render(self, request: HttpRequest, payment: OrderPayment):
-        template = get_template('pretix_bitpay/pending.html')
-        ctx = {'request': request, 'event': self.event, 'settings': self.settings,
-               'order': payment.order}
+        template = get_template("pretix_bitpay/pending.html")
+        ctx = {
+            "request": request,
+            "event": self.event,
+            "settings": self.settings,
+            "order": payment.order,
+        }
         return template.render(ctx)
 
     def payment_control_render(self, request: HttpRequest, payment: OrderPayment):
-        template = get_template('pretix_bitpay/control.html')
-        ctx = {'request': request, 'event': self.event, 'settings': self.settings,
-               'payment_info': payment.info_data, 'order': payment.order, 'provname': self.verbose_name}
+        template = get_template("pretix_bitpay/control.html")
+        ctx = {
+            "request": request,
+            "event": self.event,
+            "settings": self.settings,
+            "payment_info": payment.info_data,
+            "order": payment.order,
+            "provname": self.verbose_name,
+        }
         return template.render(ctx)
 
     abort_pending_allowed = True
 
     def payment_refund_supported(self, payment: OrderPayment):
         return True
 
     def payment_partial_refund_supported(self, payment: OrderPayment):
         return True
 
     def _refund(self, refund):
         from btcpay import crypto
-        payload = json.dumps({
-            'token': refund.payment.info_data.get('token'),
-            'amount': refund.payment.info_data.get('price'),
-            'currency': refund.payment.info_data.get('currency'),
-            'refundEmail': refund.order.email
-        })
-        uri = self.client.host + "/invoices/" + refund.payment.info_data.get('id') + "/refunds"
+
+        payload = json.dumps(
+            {
+                "token": refund.payment.info_data.get("token"),
+                "amount": refund.payment.info_data.get("price"),
+                "currency": refund.payment.info_data.get("currency"),
+                "refundEmail": refund.order.email,
+            }
+        )
+        uri = (
+            self.client.host
+            + "/invoices/"
+            + refund.payment.info_data.get("id")
+            + "/refunds"
+        )
         xidentity = crypto.get_compressed_public_key_from_pem(self.client.pem)
         xsignature = crypto.sign(uri + payload, self.client.pem)
-        headers = {"content-type": "application/json", 'accept': 'application/json', 'X-Identity': xidentity,
-                   'X-Signature': xsignature, 'X-accept-version': '2.0.0'}
+        headers = {
+            "content-type": "application/json",
+            "accept": "application/json",
+            "X-Identity": xidentity,
+            "X-Signature": xsignature,
+            "X-accept-version": "2.0.0",
+        }
         try:
-            response = requests.post(uri, data=payload, headers=headers, verify=self.client.verify)
+            response = requests.post(
+                uri, data=payload, headers=headers, verify=self.client.verify
+            )
         except Exception:
-            logger.exception('Failure during bitpay refund.')
-            raise PaymentException(_('We had trouble communicating with BitPay. Please try again and get in touch '
-                                     'with us if this problem persists.'))
+            logger.exception("Failure during bitpay refund.")
+            raise PaymentException(
+                _(
+                    "We had trouble communicating with BitPay. Please try again and get in touch "
+                    "with us if this problem persists."
+                )
+            )
         if not response.ok:
             try:
-                e = response.json()['error']
+                e = response.json()["error"]
             except JSONDecodeError:
                 e = response
 
-            logger.exception('Failure during bitpay refund: {}'.format(e))
-            raise PaymentException(_('BitPay reported an error: {}').format(e))
+            logger.exception("Failure during bitpay refund: {}".format(e))
+            raise PaymentException(_("BitPay reported an error: {}").format(e))
 
     def execute_refund(self, refund: OrderRefund):
         try:
             self._refund(refund)
         except requests.exceptions.RequestException as e:
-            logger.exception('BitPay error: %s' % str(e))
-            raise PaymentException(_('We had trouble communicating with BitPay. Please try again and contact '
-                                     'support if the problem persists.'))
+            logger.exception("BitPay error: %s" % str(e))
+            raise PaymentException(
+                _(
+                    "We had trouble communicating with BitPay. Please try again and contact "
+                    "support if the problem persists."
+                )
+            )
         else:
             refund.done()
 
     def shred_payment_info(self, obj: Union[OrderPayment, OrderRefund]):
         d = obj.info_data
         for k, v in list(d.items()):
-            if v not in ('id', 'status', 'price', 'currency', 'invoiceTime', 'paymentSubtotals',
-                         'paymentTotals', 'transactionCurrency', 'amountPaid'):
-                d[k] = '█'
+            if v not in (
+                "id",
+                "status",
+                "price",
+                "currency",
+                "invoiceTime",
+                "paymentSubtotals",
+                "paymentTotals",
+                "transactionCurrency",
+                "amountPaid",
+            ):
+                d[k] = "█"
         obj.info_data = d
         obj.save()
 
-        for le in obj.order.all_logentries().filter(action_type="pretix_bitpay.event").exclude(data=""):
+        for le in (
+            obj.order.all_logentries()
+            .filter(action_type="pretix_bitpay.event")
+            .exclude(data="")
+        ):
             d = le.parsed_data
-            if 'data' in d:
-                for k, v in list(d['data'].items()):
-                    if v not in ('id', 'status', 'price', 'currency', 'invoiceTime', 'paymentSubtotals',
-                                 'paymentTotals', 'transactionCurrency', 'amountPaid'):
-                        d['data'][k] = '█'
+            if "data" in d:
+                for k, v in list(d["data"].items()):
+                    if v not in (
+                        "id",
+                        "status",
+                        "price",
+                        "currency",
+                        "invoiceTime",
+                        "paymentSubtotals",
+                        "paymentTotals",
+                        "transactionCurrency",
+                        "amountPaid",
+                    ):
+                        d["data"][k] = "█"
                 le.data = json.dumps(d)
                 le.shredded = True
-                le.save(update_fields=['data', 'shredded'])
+                le.save(update_fields=["data", "shredded"])
```

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/signals.py` & `pretix-bitpay-1.5.2/pretix_bitpay/signals.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,34 +8,35 @@
     requiredaction_display,
 )
 
 
 @receiver(register_payment_providers, dispatch_uid="payment_bitpay")
 def register_payment_provider(sender, **kwargs):
     from .payment import BitPay
+
     return BitPay
 
 
 @receiver(signal=logentry_display, dispatch_uid="bitpay_logentry_display")
 def pretixcontrol_logentry_display(sender, logentry, **kwargs):
-    if logentry.action_type != 'pretix_bitpay.event':
+    if logentry.action_type != "pretix_bitpay.event":
         return
 
     data = json.loads(logentry.data)
-    event_type = data.get('event', {}).get('name', '?')
-    return _('BitPay reported an event: {}').format(event_type)
+    event_type = data.get("event", {}).get("name", "?")
+    return _("BitPay reported an event: {}").format(event_type)
 
 
 @receiver(signal=requiredaction_display, dispatch_uid="bitpay_requiredaction_display")
 def pretixcontrol_action_display(sender, action, request, **kwargs):
-    if not action.action_type.startswith('pretix_bitpay'):
+    if not action.action_type.startswith("pretix_bitpay"):
         return
 
     data = json.loads(action.data)
 
-    if action.action_type == 'pretix_bitpay.refund':
-        template = get_template('pretix_bitpay/action_refund.html')
-    elif action.action_type == 'pretix_bitpay.overpaid':
-        template = get_template('pretix_bitpay/action_overpaid.html')
+    if action.action_type == "pretix_bitpay.refund":
+        template = get_template("pretix_bitpay/action_refund.html")
+    elif action.action_type == "pretix_bitpay.overpaid":
+        template = get_template("pretix_bitpay/action_overpaid.html")
 
-    ctx = {'data': data, 'event': sender, 'action': action}
+    ctx = {"data": data, "event": sender, "action": action}
     return template.render(ctx, request)
```

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/static/pretix_bitpay/bitpay-logo.svg` & `pretix-bitpay-1.5.2/pretix_bitpay/static/pretix_bitpay/bitpay-logo.svg`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/templates/pretix_bitpay/action_overpaid.html` & `pretix-bitpay-1.5.2/pretix_bitpay/templates/pretix_bitpay/action_overpaid.html`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/templates/pretix_bitpay/action_refund.html` & `pretix-bitpay-1.5.2/pretix_bitpay/templates/pretix_bitpay/action_refund.html`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/templates/pretix_bitpay/control.html` & `pretix-bitpay-1.5.2/pretix_bitpay/templates/pretix_bitpay/control.html`

 * *Files identical despite different names*

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay/templates/pretix_bitpay/redirect.html` & `pretix-bitpay-1.5.2/pretix_bitpay/templates/pretix_bitpay/redirect.html`

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

### Comparing `pretix-bitpay-1.5.1/pretix_bitpay.egg-info/SOURCES.txt` & `pretix-bitpay-1.5.2/pretix_bitpay.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 pretix_bitpay/__init__.py
 pretix_bitpay/apps.py
 pretix_bitpay/models.py
 pretix_bitpay/payment.py
 pretix_bitpay/signals.py
@@ -24,14 +25,15 @@
 pretix_bitpay/locale/de/LC_MESSAGES/django.po
 pretix_bitpay/locale/de_Informal/.gitkeep
 pretix_bitpay/locale/de_Informal/LC_MESSAGES/django.po
 pretix_bitpay/locale/el/LC_MESSAGES/django.po
 pretix_bitpay/locale/es/LC_MESSAGES/django.po
 pretix_bitpay/locale/fi/LC_MESSAGES/django.po
 pretix_bitpay/locale/fr/LC_MESSAGES/django.po
+pretix_bitpay/locale/hr/LC_MESSAGES/django.po
 pretix_bitpay/locale/it/LC_MESSAGES/django.po
 pretix_bitpay/locale/ja/LC_MESSAGES/django.po
 pretix_bitpay/locale/lv/LC_MESSAGES/django.po
 pretix_bitpay/locale/nl/LC_MESSAGES/django.po
 pretix_bitpay/locale/nl_BE/LC_MESSAGES/django.po
 pretix_bitpay/locale/nl_Informal/LC_MESSAGES/django.po
 pretix_bitpay/locale/pl/LC_MESSAGES/django.po
```

### Comparing `pretix-bitpay-1.5.1/setup.cfg` & `pretix-bitpay-1.5.2/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -30,15 +30,17 @@
 	der __repr__
 	if settings.DEBUG
 	NOQA
 	NotImplementedError
 
 [check-manifest]
 ignore = 
+	.update-locales
 	.update-locales.sh
+	.gitlab-ci.yml
 	.install-hooks.sh
 	pretixplugin.toml
 	Makefile
 	manage.py
 	tests/*
 
 [egg_info]
```

