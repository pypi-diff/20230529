# Comparing `tmp/sloth-framework-0.1.6.tar.gz` & `tmp/sloth-framework-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sloth-framework-0.1.6.tar", last modified: Wed May 24 23:12:28 2023, max compression
+gzip compressed data, was "sloth-framework-0.1.7.tar", last modified: Mon May 29 02:52:45 2023, max compression
```

## Comparing `sloth-framework-0.1.6.tar` & `sloth-framework-0.1.7.tar`

### file list

```diff
@@ -1,311 +1,311 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.821168 sloth-framework-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-24 23:12:28.821168 sloth-framework-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 23:12:28.821168 sloth-framework-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.785169 sloth-framework-0.1.6/sloth/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.785169 sloth-framework-0.1.6/sloth/actions/
--rw-r--r--   0 runner    (1001) docker     (123)    40271 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/actions/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/actions/inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.785169 sloth-framework-0.1.6/sloth/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20587 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.785169 sloth-framework-0.1.6/sloth/api/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.785169 sloth-framework-0.1.6/sloth/api/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.785169 sloth-framework-0.1.6/sloth/api/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.785169 sloth-framework-0.1.6/sloth/api/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/management/commands/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/management/commands/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/management/commands/reset_passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/management/commands/selenium.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/management/commands/send_web_push_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/management/commands/startserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/management/commands/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/management/commands/sync_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.789168 sloth-framework-0.1.6/sloth/api/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0002_role_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0003_alter_application_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0004_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0005_task_stopped_alter_task_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0009_pushnotification.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0010_alter_pushnotification_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0011_alter_application_client_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0012_authcode.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0013_task_partial_task_total.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0014_email.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.781169 sloth-framework-0.1.6/sloth/api/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.789168 sloth-framework-0.1.6/sloth/api/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/all.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/bootstrap-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    33038 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/bpmn.css
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/colorpick.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.789168 sloth-framework-0.1.6/sloth/api/static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   107280 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   116316 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   112880 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   111976 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/fonts/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    83304 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/fonts/bootstrap-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    47832 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/fonts/bpmn.eot
--rw-r--r--   0 runner    (1001) docker     (123)   133048 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/fonts/bpmn.svg
--rw-r--r--   0 runner    (1001) docker     (123)    47680 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/fonts/bpmn.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    16004 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/fonts/bpmn.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/fonts/bpmn.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    30702 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/icons.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.789168 sloth-framework-0.1.6/sloth/api/static/css/images/
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/images/ui-icons_444444_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/images/ui-icons_555555_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    35973 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/jquery-ui.css
--rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/leaflet.css
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/sloth.css
--rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/trumbowyg.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.781169 sloth-framework-0.1.6/sloth/api/static/icons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.789168 sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/
--rw-r--r--   0 runner    (1001) docker     (123)   100170 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/fontawesome.min.css
--rw-r--r--   0 runner    (1001) docker     (123)  1726692 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/fontawesome.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.793168 sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   181852 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105536 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    60520 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.793168 sloth-framework-0.1.6/sloth/api/static/icons/materialicons/
--rw-r--r--   0 runner    (1001) docker     (123)   174176 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   127220 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   155604 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/materialicons/materialicons.css
--rw-r--r--   0 runner    (1001) docker     (123)   135988 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.793168 sloth-framework-0.1.6/sloth/api/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    57420 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/click.png
--rw-r--r--   0 runner    (1001) docker     (123)    55448 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/hand.png
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.797168 sloth-framework-0.1.6/sloth/api/static/images/images/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/images/badge.png
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/images/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    45136 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/login.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    22817 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21495 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/no-image.png
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/sloth.png
--rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/user.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.801168 sloth-framework-0.1.6/sloth/api/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/api.js
--rw-r--r--   0 runner    (1001) docker     (123)    78743 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)  1665279 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/bpmn.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     4098 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/colorpick.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.801168 sloth-framework-0.1.6/sloth/api/static/js/i18n/
--rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/i18n/pt-BR.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   520714 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/jquery-ui.js
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/jquery.binarytransport.js
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/jquery.mask.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    80794 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/jquery.timepicker.js
--rw-r--r--   0 runner    (1001) docker     (123)   147555 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/leaflet.js
--rw-r--r--   0 runner    (1001) docker     (123)    24103 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/masonry.pkgd.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    43994 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/qr-scanner-worker.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/qr-scanner.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/qrcode.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/select2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    17257 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/sloth.js
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/sw.js
--rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/tests.js
--rw-r--r--   0 runner    (1001) docker     (123)    28280 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/trumbowyg.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/wpn.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.801168 sloth-framework-0.1.6/sloth/api/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.785169 sloth-framework-0.1.6/sloth/api/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.801168 sloth-framework-0.1.6/sloth/api/templates/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/actions/execute_query.html
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/actions/execute_script.html
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/actions/show_icons.html
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/actions/workflow.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.801168 sloth-framework-0.1.6/sloth/api/templates/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/api/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.801168 sloth-framework-0.1.6/sloth/api/templates/charts/
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/charts/bar.html
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/charts/column.html
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/charts/donut.html
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/charts/legend.html
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/charts/pie.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.805168 sloth-framework-0.1.6/sloth/api/templates/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/apps.html
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/cards.html
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/dashboards.html
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/default.html
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/form.html
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/grids.html
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/header.html
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/links.html
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/messages.html
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/modal.html
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/plus.html
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/report.html
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/settings.html
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/shortcuts.html
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/tasks.html
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/tools.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.805168 sloth-framework-0.1.6/sloth/api/templates/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/inputs/picker.html
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/inputs/qrcode.html
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/inputs/select.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.809168 sloth-framework-0.1.6/sloth/api/templates/queryset/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/accordion.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.809168 sloth-framework-0.1.6/sloth/api/templates/queryset/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/actions/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/actions/batch.html
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/actions/global.html
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/calendar.html
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/cards.html
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/datatable.html
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/filter.html
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/filters.html
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/queryset.html
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/rows.html
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/scroll.html
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/statistics.html
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/timeline.html
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/tree.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.785169 sloth-framework-0.1.6/sloth/api/templates/renderers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.809168 sloth-framework-0.1.6/sloth/api/templates/renderers/badges/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/badges/badge.html
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/badges/boolean.html
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/badges/danger.html
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/badges/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/badges/status.html
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/badges/warning.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.809168 sloth-framework-0.1.6/sloth/api/templates/renderers/boolean/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/boolean/thumb.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.809168 sloth-framework-0.1.6/sloth/api/templates/renderers/calendar/
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/calendar/calendar.html
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/calendar/events.html
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/calendar/legend.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.809168 sloth-framework-0.1.6/sloth/api/templates/renderers/documents/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/documents/document.html
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/documents/popup.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.809168 sloth-framework-0.1.6/sloth/api/templates/renderers/images/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/images/banner.html
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/images/group.html
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/images/image.html
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/images/round.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.809168 sloth-framework-0.1.6/sloth/api/templates/renderers/links/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/links/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/links/url.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.809168 sloth-framework-0.1.6/sloth/api/templates/renderers/maps/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/maps/geolocation.html
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/maps/map.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.813168 sloth-framework-0.1.6/sloth/api/templates/renderers/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/messages/custom.html
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/messages/danger.html
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/messages/message.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/messages/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/messages/success.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/messages/warning.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.813168 sloth-framework-0.1.6/sloth/api/templates/renderers/photos/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/photos/photo.html
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/photos/round.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.813168 sloth-framework-0.1.6/sloth/api/templates/renderers/programing/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/programing/strtable.html
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/programing/terminal.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.813168 sloth-framework-0.1.6/sloth/api/templates/renderers/progress/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/progress/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/progress/success.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.813168 sloth-framework-0.1.6/sloth/api/templates/renderers/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/steps/check.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.813168 sloth-framework-0.1.6/sloth/api/templates/renderers/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/tags/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/tags/tags.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.813168 sloth-framework-0.1.6/sloth/api/templates/renderers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/utils/formatted.html
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/utils/progress.html
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/utils/qrcode.html
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/utils/steps.html
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/utils/table.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.813168 sloth-framework-0.1.6/sloth/api/templates/themes/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/themes/dark.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.813168 sloth-framework-0.1.6/sloth/api/templates/valueset/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/valueset/2-column.html
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/valueset/field.html
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/valueset/fieldset-group.html
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/valueset/fieldset-list.html
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/valueset/fieldset-tab.html
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/valueset/fieldset.html
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/valueset/primitive.html
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/valueset/value.html
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/valueset/valueset.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/api/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templatetags/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/cloud/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/cloud/printer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6116 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/cloud/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/conf/local_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/conf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21773 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    42840 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/core/queryset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/core/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/core/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21103 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/core/valueset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/db/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/test/selenium/
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/test/selenium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/test/selenium/browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/utils/formatter/
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/utils/formatter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/utils/http/
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/utils/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/utils/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/utils/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28753 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/utils/icons/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    53105 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/utils/icons/fontawesome.py
--rw-r--r--   0 runner    (1001) docker     (123)    20959 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/utils/icons/materialicons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.821168 sloth-framework-0.1.6/sloth/utils/log/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/utils/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/utils/log/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.821168 sloth-framework-0.1.6/sloth_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-24 23:12:28.000000 sloth-framework-0.1.6/sloth_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-05-24 23:12:28.000000 sloth-framework-0.1.6/sloth_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 23:12:28.000000 sloth-framework-0.1.6/sloth_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-24 23:12:28.000000 sloth-framework-0.1.6/sloth_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 23:12:28.000000 sloth-framework-0.1.6/sloth_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.432301 sloth-framework-0.1.7/sloth/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.432301 sloth-framework-0.1.7/sloth/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)    40271 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/actions/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/actions/inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.432301 sloth-framework-0.1.7/sloth/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20928 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.432301 sloth-framework-0.1.7/sloth/api/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16913 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.432301 sloth-framework-0.1.7/sloth/api/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.432301 sloth-framework-0.1.7/sloth/api/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.432301 sloth-framework-0.1.7/sloth/api/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/management/commands/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/management/commands/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/management/commands/reset_passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/management/commands/selenium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/management/commands/send_web_push_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/management/commands/startserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/management/commands/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/management/commands/sync_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.436301 sloth-framework-0.1.7/sloth/api/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0002_role_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0003_alter_application_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0004_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0005_task_stopped_alter_task_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0009_pushnotification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0010_alter_pushnotification_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0011_alter_application_client_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0012_authcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0013_task_partial_task_total.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0014_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.428301 sloth-framework-0.1.7/sloth/api/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.436301 sloth-framework-0.1.7/sloth/api/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/all.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/bootstrap-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    33038 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/bpmn.css
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/colorpick.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.440301 sloth-framework-0.1.7/sloth/api/static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   107280 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   116316 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   112880 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   111976 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/fonts/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    83304 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/fonts/bootstrap-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    47832 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/fonts/bpmn.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   133048 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/fonts/bpmn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    47680 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/fonts/bpmn.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    16004 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/fonts/bpmn.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/fonts/bpmn.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    30702 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/icons.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.440301 sloth-framework-0.1.7/sloth/api/static/css/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35973 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/jquery-ui.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/leaflet.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/sloth.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/trumbowyg.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.428301 sloth-framework-0.1.7/sloth/api/static/icons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.440301 sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/
+-rw-r--r--   0 runner    (1001) docker     (123)   100170 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/fontawesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)  1726692 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/fontawesome.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.444301 sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   181852 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105536 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    60520 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.444301 sloth-framework-0.1.7/sloth/api/static/icons/materialicons/
+-rw-r--r--   0 runner    (1001) docker     (123)   174176 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   127220 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   155604 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/materialicons/materialicons.css
+-rw-r--r--   0 runner    (1001) docker     (123)   135988 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.444301 sloth-framework-0.1.7/sloth/api/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    57420 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/click.png
+-rw-r--r--   0 runner    (1001) docker     (123)    55448 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/hand.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.444301 sloth-framework-0.1.7/sloth/api/static/images/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/images/badge.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/images/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45136 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/login.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    22817 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21495 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/no-image.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/sloth.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/user.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.452302 sloth-framework-0.1.7/sloth/api/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    78743 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1665279 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/bpmn.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4098 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/colorpick.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.452302 sloth-framework-0.1.7/sloth/api/static/js/i18n/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/i18n/pt-BR.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   520714 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/jquery-ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/jquery.binarytransport.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/jquery.mask.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    80794 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/jquery.timepicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)   147555 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/leaflet.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24103 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/masonry.pkgd.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43994 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/qr-scanner-worker.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/qr-scanner.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/qrcode.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/select2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17790 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/sloth.js
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/sw.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/tests.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28280 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/trumbowyg.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/wpn.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.452302 sloth-framework-0.1.7/sloth/api/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.428301 sloth-framework-0.1.7/sloth/api/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.452302 sloth-framework-0.1.7/sloth/api/templates/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/actions/execute_query.html
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/actions/execute_script.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/actions/show_icons.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/actions/workflow.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.452302 sloth-framework-0.1.7/sloth/api/templates/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/api/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.452302 sloth-framework-0.1.7/sloth/api/templates/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/charts/bar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/charts/column.html
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/charts/donut.html
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/charts/legend.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/charts/pie.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.456302 sloth-framework-0.1.7/sloth/api/templates/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/apps.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/dashboards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/default.html
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/grids.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/links.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/messages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/plus.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/report.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/shortcuts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/tasks.html
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/tools.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.456302 sloth-framework-0.1.7/sloth/api/templates/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/inputs/picker.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/inputs/qrcode.html
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/inputs/select.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.456302 sloth-framework-0.1.7/sloth/api/templates/queryset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/accordion.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.456302 sloth-framework-0.1.7/sloth/api/templates/queryset/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/actions/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/actions/batch.html
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/actions/global.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/calendar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/datatable.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/filters.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/queryset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/rows.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/scroll.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/statistics.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/timeline.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/tree.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.428301 sloth-framework-0.1.7/sloth/api/templates/renderers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.456302 sloth-framework-0.1.7/sloth/api/templates/renderers/badges/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/badges/badge.html
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/badges/boolean.html
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/badges/danger.html
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/badges/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/badges/status.html
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/badges/warning.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.456302 sloth-framework-0.1.7/sloth/api/templates/renderers/boolean/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/boolean/thumb.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.456302 sloth-framework-0.1.7/sloth/api/templates/renderers/calendar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/calendar/calendar.html
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/calendar/events.html
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/calendar/legend.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.456302 sloth-framework-0.1.7/sloth/api/templates/renderers/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/documents/document.html
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/documents/popup.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.456302 sloth-framework-0.1.7/sloth/api/templates/renderers/images/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/images/banner.html
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/images/group.html
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/images/image.html
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/images/round.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.456302 sloth-framework-0.1.7/sloth/api/templates/renderers/links/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/links/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/links/url.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.456302 sloth-framework-0.1.7/sloth/api/templates/renderers/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/maps/geolocation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/maps/map.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/api/templates/renderers/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/messages/custom.html
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/messages/danger.html
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/messages/message.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/messages/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/messages/success.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/messages/warning.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/api/templates/renderers/photos/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/photos/photo.html
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/photos/round.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/api/templates/renderers/programing/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/programing/strtable.html
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/programing/terminal.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/api/templates/renderers/progress/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/progress/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/progress/success.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/api/templates/renderers/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/steps/check.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/api/templates/renderers/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/tags/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/tags/tags.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/api/templates/renderers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/utils/formatted.html
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/utils/progress.html
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/utils/qrcode.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/utils/steps.html
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/utils/table.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/api/templates/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/themes/dark.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/api/templates/valueset/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/valueset/2-column.html
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/valueset/field.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/valueset/fieldset-group.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/valueset/fieldset-list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/valueset/fieldset-tab.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/valueset/fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/valueset/primitive.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/valueset/value.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/valueset/valueset.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/api/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templatetags/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/cloud/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/cloud/printer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6116 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/cloud/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/conf/local_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/conf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21773 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42840 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/core/queryset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/core/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/core/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21103 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/core/valueset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/sloth/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/sloth/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/sloth/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/sloth/test/selenium/
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/test/selenium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/test/selenium/browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/sloth/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/sloth/utils/formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/utils/formatter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/sloth/utils/http/
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/utils/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/sloth/utils/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/utils/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28753 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/utils/icons/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53105 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/utils/icons/fontawesome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20959 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/utils/icons/materialicons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/sloth/utils/log/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/utils/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/utils/log/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/sloth_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 02:52:45.000000 sloth-framework-0.1.7/sloth_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-05-29 02:52:45.000000 sloth-framework-0.1.7/sloth_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 02:52:45.000000 sloth-framework-0.1.7/sloth_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-29 02:52:45.000000 sloth-framework-0.1.7/sloth_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 02:52:45.000000 sloth-framework-0.1.7/sloth_framework.egg-info/top_level.txt
```

### Comparing `sloth-framework-0.1.6/PKG-INFO` & `sloth-framework-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sloth-framework
-Version: 0.1.6
+Version: 0.1.7
 Summary: Metadata-based web framework for the development of management information systems
 Home-page: http://sloth.aplicativo.click/
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `sloth-framework-0.1.6/setup.py` & `sloth-framework-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open(os.path.join(root_dir, 'sloth/requirements.txt')) as file:
     requirements = file.read().strip().splitlines()
 
 os.chdir(root_dir)
 
 setup(
     name='sloth-framework',
-    version='0.1.6',
+    version='0.1.7',
     packages=find_packages(),
     install_requires=requirements,
     extras_require={
         'dev': [],
         'production': [],
     },
     include_package_data=True,
```

### Comparing `sloth-framework-0.1.6/sloth/Dockerfile` & `sloth-framework-0.1.7/sloth/Dockerfile`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/__init__.py` & `sloth-framework-0.1.7/sloth/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/__main__.py` & `sloth-framework-0.1.7/sloth/__main__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/actions/__init__.py` & `sloth-framework-0.1.7/sloth/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/actions/fields.py` & `sloth-framework-0.1.7/sloth/actions/fields.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/actions/inputs.py` & `sloth-framework-0.1.7/sloth/actions/inputs.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/__init__.py` & `sloth-framework-0.1.7/sloth/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/actions.py` & `sloth-framework-0.1.7/sloth/api/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
 import json
+import sys
+
 import onetimepass
 import base64
 import requests
 import io
 import subprocess
 from django.core.cache import cache
 from django.core.exceptions import ValidationError
@@ -570,7 +572,22 @@
                     content = file.read()
             else:
                 content = Workflow.INITIAL_CONTENT
         return self.render('actions/workflow.html', title='Fluxograma', content=content)
 
     def has_permission(self, user):
         return user.is_superuser
+
+
+class TestLogger(actions.ActionView):
+    class Meta:
+        verbose_name = 'Log de Teste'
+        modal = True
+        style = 'primary'
+
+    def view(self):
+        command = self.request.GET.get('command')
+        print(command)
+        return command
+
+    def has_permission(self, user):
+        return 'test' in sys.argv
```

### Comparing `sloth-framework-0.1.6/sloth/api/backends/__init__.py` & `sloth-framework-0.1.7/sloth/api/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/dashboard.py` & `sloth-framework-0.1.7/sloth/api/dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,30 +380,31 @@
                 menu[item['label']] = item
                 icons[item['label']] = item['icon'] or 'record-circle'
 
         if not render:
             return dict(icons=icons, items=menu)
 
         html = []
-        def append_html(label, item, level=0):
+        def append_html(label, item, level=0, hierarchy=None):
             ident = '\t' * level
             nbsp = '&nbsp;' * level * 3
             html.append('{}<li>'.format(ident))
             icon = '<i class="bi bi-{} menu-item-icon"></i> '.format(icons[label]) if level == 0 else ''
             if 'url' in item:
-                html.append('{}\t<a href="{}">{}{}{}</a>'.format(ident, item['url'], icon, nbsp, item['label']))
+                html.append('{}\t<a class="menu-subitem" data-hierarchy="({})" href="{}">{}{}{}</a>'.format(ident, ', '.join([f"'{text}'" for text in hierarchy]), item['url'], icon, nbsp, item['label']))
             else:
-                html.append('{}\t<a href="javascript:">{}{}{}<i class="bi bi-chevron-down chevron"></i></a>'.format(ident, icon, nbsp, label))
+                html.append('{}\t<a class="menu-item" href="javascript:">{}{}{}<i class="bi bi-chevron-down chevron"></i></a>'.format(ident, icon, nbsp, label))
                 html.append('{}<ul>'.format(ident))
                 for sublabel, subitem in item.items():
-                    append_html(sublabel, subitem, level+1)
+                    hierarchy.insert(0, sublabel)
+                    append_html(sublabel, subitem, level+1, hierarchy)
                 html.append('{}</ul>'.format(ident))
             html.append('{}</li>'.format(ident))
         for label, item in menu.items():
-            append_html(label, item, 0)
+            append_html(label, item, 0, [label])
         return mark_safe('\n'.join(html))
 
     def serialize(self, data):
         for k, v in data.items():
             pass # print(k, v)
         for k, v in data.get('append', {}).items():
             self.data[k].append(v)
```

### Comparing `sloth-framework-0.1.6/sloth/api/management/commands/cloud.py` & `sloth-framework-0.1.7/sloth/api/management/commands/cloud.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/management/commands/query.py` & `sloth-framework-0.1.7/sloth/api/management/commands/query.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/management/commands/send_web_push_notification.py` & `sloth-framework-0.1.7/sloth/api/management/commands/send_web_push_notification.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/management/commands/startserver.py` & `sloth-framework-0.1.7/sloth/api/management/commands/startserver.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/management/commands/sync.py` & `sloth-framework-0.1.7/sloth/api/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/migrations/0001_initial.py` & `sloth-framework-0.1.7/sloth/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/migrations/0002_role_user.py` & `sloth-framework-0.1.7/sloth/api/migrations/0002_role_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/migrations/0003_alter_application_user.py` & `sloth-framework-0.1.7/sloth/api/migrations/0003_alter_application_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/migrations/0004_task.py` & `sloth-framework-0.1.7/sloth/api/migrations/0004_task.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/migrations/0005_task_stopped_alter_task_message.py` & `sloth-framework-0.1.7/sloth/api/migrations/0005_task_stopped_alter_task_message.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py` & `sloth-framework-0.1.7/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py` & `sloth-framework-0.1.7/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py` & `sloth-framework-0.1.7/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/migrations/0009_pushnotification.py` & `sloth-framework-0.1.7/sloth/api/migrations/0009_pushnotification.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/migrations/0010_alter_pushnotification_user.py` & `sloth-framework-0.1.7/sloth/api/migrations/0010_alter_pushnotification_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/migrations/0011_alter_application_client_secret.py` & `sloth-framework-0.1.7/sloth/api/migrations/0011_alter_application_client_secret.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/migrations/0012_authcode.py` & `sloth-framework-0.1.7/sloth/api/migrations/0012_authcode.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/migrations/0013_task_partial_task_total.py` & `sloth-framework-0.1.7/sloth/api/migrations/0013_task_partial_task_total.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/migrations/0014_email.py` & `sloth-framework-0.1.7/sloth/api/migrations/0014_email.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/models.py` & `sloth-framework-0.1.7/sloth/api/models.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/all.min.css` & `sloth-framework-0.1.7/sloth/api/static/css/all.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/bootstrap-icons.css` & `sloth-framework-0.1.7/sloth/api/static/css/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/bootstrap.min.css` & `sloth-framework-0.1.7/sloth/api/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/bpmn.css` & `sloth-framework-0.1.7/sloth/api/static/css/bpmn.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/colorpick.min.css` & `sloth-framework-0.1.7/sloth/api/static/css/colorpick.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf` & `sloth-framework-0.1.7/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf` & `sloth-framework-0.1.7/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf` & `sloth-framework-0.1.7/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/fonts/bootstrap-icons.woff` & `sloth-framework-0.1.7/sloth/api/static/css/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/fonts/bootstrap-icons.woff2` & `sloth-framework-0.1.7/sloth/api/static/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/fonts/bpmn.eot` & `sloth-framework-0.1.7/sloth/api/static/css/fonts/bpmn.eot`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/fonts/bpmn.svg` & `sloth-framework-0.1.7/sloth/api/static/css/fonts/bpmn.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/fonts/bpmn.ttf` & `sloth-framework-0.1.7/sloth/api/static/css/fonts/bpmn.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/fonts/bpmn.woff` & `sloth-framework-0.1.7/sloth/api/static/css/fonts/bpmn.woff`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/fonts/bpmn.woff2` & `sloth-framework-0.1.7/sloth/api/static/css/fonts/bpmn.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/icons.svg` & `sloth-framework-0.1.7/sloth/api/static/css/icons.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/images/ui-icons_444444_256x240.png` & `sloth-framework-0.1.7/sloth/api/static/css/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/images/ui-icons_555555_256x240.png` & `sloth-framework-0.1.7/sloth/api/static/css/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/jquery-ui.css` & `sloth-framework-0.1.7/sloth/api/static/css/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/leaflet.css` & `sloth-framework-0.1.7/sloth/api/static/css/leaflet.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/select2.min.css` & `sloth-framework-0.1.7/sloth/api/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/sloth.css` & `sloth-framework-0.1.7/sloth/api/static/css/sloth.css`

 * *Files 2% similar despite different names*

```diff
@@ -48,18 +48,21 @@
     color: white !important;
 }
 .img-circle{
     border-radius: 50%;
 }
 .queryset-title {
     display: inline-block;
+    margin-top: 10px;
 }
 .queryset-action-bar {
     float: right;
     display: inline-block;
+    margin-right: 10px;
+    margin-top: 10px;
 }
 .queryset-data{
     overflow-x:auto;
     max-width:100%;
     clear: both;
     padding: 1px;
 }
@@ -124,14 +127,16 @@
 }
 .fieldset-tab .queryset-title h2{
     font-size: 1.25rem;
 }
 .fieldset-action-bar{
     float: right;
     display: inline-block;
+    margin-right: 10px;
+    margin-top: 10px;
 }
 .fieldet-tab{
     padding-top: 1rem;
 }
 @keyframes slideInFromLeft {
   0% {
     transform: translateX(-100%);
@@ -465,15 +470,15 @@
 .admin-queryset .queryset-data, .admin-queryset .search-and-filters form.with-filter,
 .fieldset-inline-action, .action-wrapper fieldset, .cards-wrapper,
 .shortcut-wrapper, .fieldset-list, .fieldset-group, .box,
 .valueset-fieldsets > reloadable-fieldset:not(.box){
 	background-color: white;
 	box-shadow: 0px 16px 32px 0px #001E3C0A;
 	border-radius: 8px;
-	padding: 20px;
+	padding-left: 20px;
 }
 .search-and-filters form, .action-wrapper, .cards-wrapper, .shortcut-wrapper, .fieldset-list, .fieldset-inline-action{
     margin-bottom: 20px;
 }
 
 .progress{
     height: 1.5rem;
```

### Comparing `sloth-framework-0.1.6/sloth/api/static/css/trumbowyg.min.css` & `sloth-framework-0.1.7/sloth/api/static/css/trumbowyg.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/fontawesome.min.css` & `sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/fontawesome.min.js` & `sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/fontawesome.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf` & `sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2` & `sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf` & `sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2` & `sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf` & `sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2` & `sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2` & `sloth-framework-0.1.7/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2` & `sloth-framework-0.1.7/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2` & `sloth-framework-0.1.7/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/icons/materialicons/materialicons.css` & `sloth-framework-0.1.7/sloth/api/static/icons/materialicons/materialicons.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2` & `sloth-framework-0.1.7/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/images/click.png` & `sloth-framework-0.1.7/sloth/api/static/images/click.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/images/hand.png` & `sloth-framework-0.1.7/sloth/api/static/images/hand.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/images/icon.png` & `sloth-framework-0.1.7/sloth/api/static/images/icon.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/images/icon.svg` & `sloth-framework-0.1.7/sloth/api/static/images/icon.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/images/images/badge.png` & `sloth-framework-0.1.7/sloth/api/static/images/images/badge.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/images/images/icon.png` & `sloth-framework-0.1.7/sloth/api/static/images/images/icon.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/images/login.jpeg` & `sloth-framework-0.1.7/sloth/api/static/images/login.jpeg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/images/logo.png` & `sloth-framework-0.1.7/sloth/api/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/images/logo.svg` & `sloth-framework-0.1.7/sloth/api/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/images/no-image.png` & `sloth-framework-0.1.7/sloth/api/static/images/no-image.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/images/sloth.png` & `sloth-framework-0.1.7/sloth/api/static/images/sloth.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/images/user.png` & `sloth-framework-0.1.7/sloth/api/static/images/user.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/js/api.js` & `sloth-framework-0.1.7/sloth/api/static/js/api.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/js/bootstrap.bundle.min.js` & `sloth-framework-0.1.7/sloth/api/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/js/bpmn.js` & `sloth-framework-0.1.7/sloth/api/static/js/bpmn.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/js/colorpick.min.js` & `sloth-framework-0.1.7/sloth/api/static/js/colorpick.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/js/i18n/pt-BR.js` & `sloth-framework-0.1.7/sloth/api/static/js/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/js/jquery-3.6.0.min.js` & `sloth-framework-0.1.7/sloth/api/static/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/js/jquery-ui.js` & `sloth-framework-0.1.7/sloth/api/static/js/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/js/jquery.binarytransport.js` & `sloth-framework-0.1.7/sloth/api/static/js/jquery.binarytransport.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/js/jquery.mask.min.js` & `sloth-framework-0.1.7/sloth/api/static/js/jquery.mask.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/js/jquery.timepicker.js` & `sloth-framework-0.1.7/sloth/api/static/js/jquery.timepicker.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/js/leaflet.js` & `sloth-framework-0.1.7/sloth/api/static/js/leaflet.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/js/masonry.pkgd.min.js` & `sloth-framework-0.1.7/sloth/api/static/js/masonry.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/js/popper.min.js` & `sloth-framework-0.1.7/sloth/api/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/js/qr-scanner-worker.min.js` & `sloth-framework-0.1.7/sloth/api/static/js/qr-scanner-worker.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/js/qr-scanner.min.js` & `sloth-framework-0.1.7/sloth/api/static/js/qr-scanner.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/js/qrcode.min.js` & `sloth-framework-0.1.7/sloth/api/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/js/select2.min.js` & `sloth-framework-0.1.7/sloth/api/static/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/js/sloth.js` & `sloth-framework-0.1.7/sloth/api/static/js/sloth.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -83,14 +83,15 @@
                     for (k in vals) {
                         $('#' + k).val(vals[k]).trigger('change')
                     }
                 } else $('#modal').find('.modal-body').html('');
             });
             $('#modal').on('shown.bs.modal', function(e) {
                 $('#modal').responsive();
+                testlogger("self.look_at_popup_window()");
             });
         }
         if ($('#modal').find('.modal-body').html().trim()) {
             $('#modal').find('.modal-body').css('visibility', 'hidden');
             $('#modal .modal-body .select2-hidden-accessible').select2("destroy");
             window['POPUP_STACK'].push($('#modal').find('.modal-body').clone());
             var vals = {};
@@ -105,45 +106,14 @@
                     //$('.modal-body').find('input[type=text], input[type=number]').first().focus();
                 }, 200);
             }
             $('#modal').modal('show');
             $('#modal').find('.modal-body').css('visibility', 'visible');
         });
     },
-    reloadAreas(areas) {
-        if (areas != null) {
-            $('.reloadable-fieldset').map(function(i, item) {
-                if (areas.indexOf(item.id) >= 0 || areas.length == 0) {
-                    $.get($(item).data('path'), function(html) {
-                        if ($(item).find('.bi-chevron-right').length) {
-                            html = html.replace('bi-chevron-down', 'bi-chevron-right');
-                        }
-                        $(item).html(html).initialize();
-                    })
-                }
-            });
-            $('.reloadable-queryset').map(function(i, item) {
-                window['reload' + this.id]();
-            });
-        } else {
-            var url = document.location.pathname;
-            if ($(document).getCookie('current_tab')) url += '?tab=' + $(document).getCookie('current_tab');
-            $(document).open(url);
-        }
-        return this;
-    },
-    reload: function(id) {
-        if (id) {
-            $(this).request($(id).data('url'), 'GET', {}, function(html) {
-                $(id).html($(html).find(id).html()).initialize();
-            });
-        } else {
-            document.location.reload();
-        }
-    },
     redirect: function(url) {
         $('#modal').modal('hide');
         document.location.href = url;
     },
     download: function(url) {
         alert(url);
         var a = document.createElement("a");
@@ -224,15 +194,14 @@
             var widgets = $('.' + this.name);
             $(this).on('click', function(e) {
                 $(widgets).prop('disabled', !this.checked);
             });
             $(widgets).prop('disabled', !this.checked);
         });
         $(this).find('textarea.html-input').each(function(index) {
-            console.log(this);
             $(this).trumbowyg({
                 lang: 'pt_br'
             });
         });
         $(this).find('select').not('.select2-hidden-accessible').each(function(index) {
             var element = $(this);
             var url = $(this).data('choices-url');
@@ -264,14 +233,17 @@
                 },
                 templateSelection: function(data) {
                     return data.text;
                 }
             }
             if (url == null) ajax = null;
             $(this).select2({
+                ajax: {
+                    delay: 3000
+                },
                 width: '100%',
                 language: 'pt-BR',
                 allowClear: true,
                 placeholder: '',
                 ajax: ajax,
                 templateResult: function(item) {
                     return item.html ? $(item.html) : item.text
@@ -318,50 +290,82 @@
             });
         });
         $(document).on('select2:open', () => {
             $(this).closest('.select2-search__field').focus();
         });
         $('.fieldset-tab').map(function(i, item) {
             var fieldsets = $(this).find('.reloadable-fieldset, .reloadable-queryset');
-            if (fieldsets.length == 1) fieldsets.find('.queryset-title, fieldset-title').hide();
+            if (fieldsets.length == 1) fieldsets.find('.queryset-title, .fieldset-title').hide();
         });
+
+        if (window.testlogger) {
+            function formatValue(value) {
+                if (value && value.length == 10 && value.indexOf('-') == 4) {
+                    var tokens = value.split('-');
+                    if (tokens.length == 3) return tokens[2] + '/' + tokens[1] + '/' + tokens[0];
+                }
+                return value;
+            }
+            $(this).find('input, textarea').not('input[type=checkbox]').blur(function() {
+                testlogger("self.enter('" + $(this).parent().find('label').html().trim().replace('*', '') + "', '" + formatValue($(this).val()) + "')")
+            });
+            $(this).find('select').change(function() {
+                testlogger("self.choose('" + $(this).parent().find('label').html().trim().replace('*', '') + "', '" + $(this).find('option:selected').html() + "')")
+            });
+            $(this).find('a:not(.btn):not(.nav-link):not(.menu-item):not(.menu-subitem):not(.search-menu-item)').click(function() {
+                testlogger("self.click_link('" + $(this).text().replace("Loading...", "").trim() + "')")
+            });
+            $(this).find('a.nav-link').click(function() {
+                testlogger("self.click_tab('" + $(this).find('.nav-link-text').text().trim() + "')")
+            });
+            $(this).find('a.menu-subitem').click(function() {
+                testlogger("self.click_menu" + $(this).data("hierarchy") + "")
+            });
+            $(this).find('a.search-menu-item').click(function() {
+                testlogger("self.search_menu('" + $(this).text().trim() + "')")
+            });
+            $(this).find('a.btn').click(function() {
+                testlogger("self.click_button('" + $(this).text().trim() + "')")
+            });
+            $(this).find('button').click(function() {
+                testlogger("self.click_button('" + $(this).text().replace("Loading...", "").trim() + "')")
+            });
+            $(this).find('input[type=checkbox]').click(function() {
+                testlogger("self.check('" + $(this).parent().find('label').html().trim().replace('*', '') + "')")
+            });
+            $(this).find('btn i.bi').click(function() {
+                testlogger("self.click_icon('" + $(this).attr('class').replace("bi ", "").replace("bi-", "") + "')")
+            });
+        }
         return this;
     },
-    areas: function() {
-        return $('.reloadable-fieldset').map(function(i, item) {
-            return item.id
-        }).get()
-    },
     refresh: function(areas) {
-        if (areas.length == 0) areas = $(this).areas();
-        if (areas.length > 0) {
-            var url = '?only=' + areas.join(',');
-            $.get({
-                url: url,
-                success: function(html) {
-                    $('.valueset-header').html($(html).find('.valueset-header'));
-                    areas.forEach(function(attrName) {
-                        var remote = $(html).find('#' + attrName);
-                        var local = $('#' + attrName);
-                        var arrow = local.find('fieldset-title').find('i');
-                        if (arrow.hasClass('bi-chevron-down')) {
-                            arrow.addClass('bi-chevron-down').removeClass('bi-chevron-right');
-                        } else {
-                            arrow.removeClass('bi-chevron-down').addClass('bi-chevron-right');
+        function reloadAreas() {
+            $('.reloadable-fieldset, .reloadable-queryset').map(
+                function(i, item) {
+                    var querystring = '';
+                    var qsform = $('#form-' + item.id);
+                    if (qsform.length > 0) querystring = '?' + qsform.serialize();
+                    var url = $(item).data('path') + querystring;
+                    if (areas && areas.length > 0 && areas.indexOf(item.id) < 0) return;
+                    $.get(url, function(html) {
+                        if ($(item).find('.bi-chevron-right').length) {
+                            html = html.replace('bi-chevron-down', 'bi-chevron-right');
                         }
-                        remote.find('.fieldset-data').css('display', local.find('.fieldset-data').css('display'));
-                        local.html(remote.html()).initialize();
-                    });
+                        $(item).html($(html).html()).initialize();
+                    })
+                    //console.log(item.id + ' : ' + url);
+                    return {
+                        id: item.id,
+                        url: url
+                    }
                 }
-            });
+            ).get();
         }
-        // reload all querysets
-        $('.reloadable-queryset').map(function(i, item) {
-            window['reload' + this.id]();
-        });
+        setTimeout(reloadAreas, 1000);
     },
     dynamic: function(name, initial) {
         var form = $(this);
         var lastChangedValue = {};
         initial.hide.forEach(function(name) {
             form.find("input[name=" + name + "], select[name=" + name + "], textarea[name=" + name + "]").closest('.form-field').hide();
         });
```

### Comparing `sloth-framework-0.1.6/sloth/api/static/js/sw.js` & `sloth-framework-0.1.7/sloth/api/static/js/sw.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/js/tests.js` & `sloth-framework-0.1.7/sloth/api/static/js/tests.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -71,15 +71,27 @@
     var lastScrooledElement = null;
     if (element.offset() && !isIntoView(element)) {
         var scrollData = {
             scrollTop: element.offset().top - $(window).height() / 2
         };
         if (window['display_fake_mouse']) var scroolSpeed = 1200;
         else var scroolSpeed = 0;
-        $([document.documentElement, document.body]).animate(scrollData, scroolSpeed, 'swing', function() {
+        // $([document.documentElement, document.body]).animate(scrollData, scroolSpeed, 'swing', function (){
+        if ($('#modal:visible').length > 0) {
+            var container = '#modal';
+            var scrollData = {
+                scrollTop: element.offset().top - (window.innerHeight * 0.25) + $(container).scrollTop()
+            };
+        } else {
+            var container = 'body';
+            var scrollData = {
+                scrollTop: element.offset().top - (window.innerHeight * 0.25)
+            };
+        }
+        $(container).animate(scrollData, scroolSpeed, 'swing', function() {
             if (lastScrooledElement != element) callback();
             lastScrooledElement = element;
         });
     } else {
         callback();
     }
     return element
@@ -109,15 +121,15 @@
     var link = type == null || type == 'link';
     var button = type == null || type == 'button';
     var tab = type == 'tab';
     var icon = type == 'icon';
     if (icon) {
         element = $(cursor || document).find('.bi-' + name + ':visible').parent();
     } else if (tab) {
-        element = $(document).find('a.nav-link').filter(function() {
+        element = $(cursor || document).find('a.nav-link').filter(function() {
             return $(this).find('.nav-link-text').text().trim() == name;
         }).first();
     } else {
         if (element.length == 0 && (link || button)) element = $(cursor || document).find("button:visible").filter(function() {
             return $(this).text().replace('Loading...', '').trim() === name;
         }).first();
         if (element.length == 0 && (link || button)) element = $(cursor || document).find("a:visible").filter(function() {
@@ -258,21 +270,21 @@
             }
             return scroolToElement(element, afterScrool);
         }
         throw Error('Not found.')
     }
 }
 
-function check(name, radio) {
-    lookAt(name);
+function check(name, radio, look) {
+    if (look == null) lookAt(name);
     if (radio) tipo = 'radio';
     else tipo = 'checkbox';
     var element = $(cursor || document).find('input[type=' + tipo + ']');
     if (recursively(element)) {
-        return check(name, radio);
+        return check(name, radio, false);
     } else if (element.length > 0) {
         element.trigger('click');
         return element;
     }
     throw Error('Not found.')
 }
 
@@ -303,26 +315,29 @@
 
     if (recursively(element)) {
         return choose(name, value, headless);
     } else if (element.length > 0) {
         if (headless) {
             $(element).val(element.find("option:contains(" + value + ")").val());
         } else {
-            element.select2("open");
-            var $search = element.data('select2').dropdown.$search || element.data('select2').selection.$search;
-            $search.val(value);
-            $search.trigger('keyup');
-            var lookup = "option:contains(" + value + ")";
-
-            function waitValue() {
-                var value = element.find(lookup).val();
-                element.val(value).trigger('change');
-                element.select2('close');
+            function afterScrool() {
+                element.select2("open");
+                var $search = element.data('select2').dropdown.$search || element.data('select2').selection.$search;
+                $search.val(value);
+                $search.trigger('keyup');
+                var lookup = "option:contains(" + value + ")";
+
+                function waitValue() {
+                    var value = element.find(lookup).val();
+                    element.val(value).trigger('change');
+                    element.select2('close');
+                }
+                setTimeout(waitValue, '2000');
             }
-            setTimeout(waitValue, '2000');
+            return scroolToElement(element, afterScrool);
         }
         return element.parent()[0]
     }
     throw Error('Not found.')
 }
 
 function seeMessage(text) {
```

### Comparing `sloth-framework-0.1.6/sloth/api/static/js/trumbowyg.min.js` & `sloth-framework-0.1.7/sloth/api/static/js/trumbowyg.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/static/js/wpn.js` & `sloth-framework-0.1.7/sloth/api/static/js/wpn.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/tasks/__init__.py` & `sloth-framework-0.1.7/sloth/api/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/actions/execute_query.html` & `sloth-framework-0.1.7/sloth/api/templates/actions/execute_query.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/actions/show_icons.html` & `sloth-framework-0.1.7/sloth/api/templates/actions/show_icons.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/actions/workflow.html` & `sloth-framework-0.1.7/sloth/api/templates/actions/workflow.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/api/index.html` & `sloth-framework-0.1.7/sloth/api/templates/api/index.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/charts/bar.html` & `sloth-framework-0.1.7/sloth/api/templates/charts/bar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/charts/column.html` & `sloth-framework-0.1.7/sloth/api/templates/charts/column.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/charts/pie.html` & `sloth-framework-0.1.7/sloth/api/templates/charts/pie.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/dashboard/actions.html` & `sloth-framework-0.1.7/sloth/api/templates/dashboard/actions.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/dashboard/apps.html` & `sloth-framework-0.1.7/sloth/api/templates/dashboard/apps.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/dashboard/base.html` & `sloth-framework-0.1.7/sloth/api/templates/dashboard/base.html`

 * *Files 16% similar despite different names*

```diff
@@ -70,9 +70,13 @@
       </main>
     {% block footer %}
     {% include "dashboard/footer.html" %}
     {% endblock %}
     {% include "dashboard/modal.html" %}
     {% include "dashboard/bottom.html" %}
   </body>
+  <script>
+    var display_fake_mouse = false;
+    function testlogger(command){return;$.get('/app/dashboard/test_logger/?command='+command);};
+  </script>
 </html>
 {% endif %}
```

### Comparing `sloth-framework-0.1.6/sloth/api/templates/dashboard/bottom.html` & `sloth-framework-0.1.7/sloth/api/templates/dashboard/bottom.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/dashboard/cards.html` & `sloth-framework-0.1.7/sloth/api/templates/dashboard/cards.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/dashboard/footer.html` & `sloth-framework-0.1.7/sloth/api/templates/dashboard/footer.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/dashboard/form.html` & `sloth-framework-0.1.7/sloth/api/templates/dashboard/form.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/dashboard/grids.html` & `sloth-framework-0.1.7/sloth/api/templates/dashboard/grids.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/dashboard/header.html` & `sloth-framework-0.1.7/sloth/api/templates/dashboard/header.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/dashboard/links.html` & `sloth-framework-0.1.7/sloth/api/templates/dashboard/links.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/dashboard/menu.html` & `sloth-framework-0.1.7/sloth/api/templates/dashboard/menu.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/dashboard/messages.html` & `sloth-framework-0.1.7/sloth/api/templates/dashboard/messages.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/dashboard/modal.html` & `sloth-framework-0.1.7/sloth/api/templates/dashboard/modal.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/dashboard/plus.html` & `sloth-framework-0.1.7/sloth/api/templates/dashboard/plus.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/dashboard/report.html` & `sloth-framework-0.1.7/sloth/api/templates/dashboard/report.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/dashboard/search.html` & `sloth-framework-0.1.7/sloth/api/templates/dashboard/search.html`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   {% for item in dashboard.data.search %}
   <li class="list-group-item d-flex justify-content-between align-items-start">
     <div class="ms-2 me-auto">
       <div>
         {% if item.subitems %}
           {{ item.label }}
         {% else %}
-        <a class="item" href="{{ item.url }}">
+        <a class="item search-menu-item" href="{{ item.url }}">
           {{ item.label }}
         </a>
         {% endif %}
       </div>
       {% for subitem in item.subitems %}
         <div><a class="subitem" href="{{ subitem.url }}">{{ subitem.label }}</a></div>
       {% endfor %}
```

### Comparing `sloth-framework-0.1.6/sloth/api/templates/dashboard/settings.html` & `sloth-framework-0.1.7/sloth/api/templates/dashboard/settings.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/dashboard/shortcuts.html` & `sloth-framework-0.1.7/sloth/api/templates/dashboard/shortcuts.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/dashboard/tasks.html` & `sloth-framework-0.1.7/sloth/api/templates/dashboard/tasks.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/dashboard/tools.html` & `sloth-framework-0.1.7/sloth/api/templates/dashboard/tools.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/inputs/picker.html` & `sloth-framework-0.1.7/sloth/api/templates/inputs/picker.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/inputs/qrcode.html` & `sloth-framework-0.1.7/sloth/api/templates/inputs/qrcode.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/inputs/select.html` & `sloth-framework-0.1.7/sloth/api/templates/inputs/select.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/queryset/accordion.html` & `sloth-framework-0.1.7/sloth/api/templates/queryset/accordion.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/queryset/calendar.html` & `sloth-framework-0.1.7/sloth/api/templates/queryset/calendar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/queryset/cards.html` & `sloth-framework-0.1.7/sloth/api/templates/queryset/cards.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/queryset/datatable.html` & `sloth-framework-0.1.7/sloth/api/templates/queryset/datatable.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/queryset/filter.html` & `sloth-framework-0.1.7/sloth/api/templates/queryset/filter.html`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
           language: 'pt-BR',
           allowClear: true,
           placeholder: 'Selecione uma opção',
           {% if metadata.choices is None %}
           ajax: {
             url: function () {return "{{ data.path|start_querystring }}"+$('#form-{{ data.uuid }}').serialize()+'&choices={{ metadata.key }}';},
             dataType: 'json',
-            delay: 250,
+            delay: 3000,
             minimumInputLength: 3,
             data: function (params) {
               return { term: params.term };
             },
             processResults: function (data) {
               return { results: data.items };
             },
```

### Comparing `sloth-framework-0.1.6/sloth/api/templates/queryset/filters.html` & `sloth-framework-0.1.7/sloth/api/templates/queryset/filters.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/queryset/queryset.html` & `sloth-framework-0.1.7/sloth/api/templates/queryset/queryset.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 {% load tags %}
-<div>
 <div class="reloadable-queryset {% if not data.metadata.is_admin%}box{% endif %}" id="{{ data.key }}" data-path="{{ data.path }}">
     <div class="queryset {% if data.metadata.is_admin %}admin-queryset{% endif %}" id="queryset-{{ data.uuid }}">
         {% if data.name %}
             {% if data.metadata.is_admin %}
                 <div class="queryset-title">
                     <h2>{{ data.icon|icontag }} {{ data.name }}</h2>
                 </div>
@@ -56,15 +55,15 @@
                     $('#subset-{{ data.uuid }}').val(subset);
                     $('#tabs-container-{{ data.uuid }}').find('.nav-item.'+subset).find('.spinner-border').removeClass('d-none');
                     var data = $('#form-{{ data.uuid }}').serialize();
                     $.ajax({
                         url:'{{ data.path|safe }}?{{ request|post_querystring }}',
                         data: data,
                         success:function( html ) {
-                            $('#{{ data.key }}').html($(html).find('#{{ data.key }}').html()).initialize();
+                            $('#{{ data.key }}').html($(html).html()).initialize();
                             $(document.body).removeClass('page-loading');
                         }
                     });
                 }
                 function toggleActions{{ data.uuid }}(input){
                     if(input.value=='') $('#queryset-{{ data.uuid }}').find('.action-checkbox').prop('checked', input.checked);
                     if($('#queryset-{{ data.uuid }}').find('.action-checkbox:checked').length>0){
@@ -201,12 +200,13 @@
         {% endfor %}
       </ul>
     </nav>
     {% endif %}
         </div>
         </div>
     </div>
+    {% if data.metadata.scrollable %}
+        {% include "queryset/scroll.html" %}
+    {% endif %}
 </div>
-{% if data.metadata.scrollable %}
-    {% include "queryset/scroll.html" %}
-{% endif %}
-</div>
+
+
```

### Comparing `sloth-framework-0.1.6/sloth/api/templates/queryset/rows.html` & `sloth-framework-0.1.7/sloth/api/templates/queryset/rows.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/queryset/scroll.html` & `sloth-framework-0.1.7/sloth/api/templates/queryset/scroll.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/queryset/statistics.html` & `sloth-framework-0.1.7/sloth/api/templates/queryset/statistics.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% load tags %}
-<div class="reloadable-fieldset box" id="{{ data.key }}" data-path="{{ data.path }}">
+<div class="{% if unreloadable %}un{% endif %}reloadable-fieldset box" id="{{ data.key }}" data-path="{{ data.path }}">
 <div id="statistics-{{ data.uuid }}">
 {% if uuid is None or request.GET.uuid is None %}
     {% if data.name %}
         <div class="fieldset-title" onclick="$(this).parent().find('.toogle-data').slideToggle();$(this).find('i').toggleClass('bi-chevron-down').toggleClass('bi-chevron-right');">
           <h5><i class="bi bi-chevron-down"></i> {{ data.name }}</h5>
         </div>
     {% endif %}
```

### Comparing `sloth-framework-0.1.6/sloth/api/templates/queryset/timeline.html` & `sloth-framework-0.1.7/sloth/api/templates/queryset/timeline.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/queryset/tree.html` & `sloth-framework-0.1.7/sloth/api/templates/queryset/tree.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/renderers/calendar/calendar.html` & `sloth-framework-0.1.7/sloth/api/templates/renderers/calendar/calendar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/renderers/maps/map.html` & `sloth-framework-0.1.7/sloth/api/templates/renderers/maps/map.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/renderers/programing/strtable.html` & `sloth-framework-0.1.7/sloth/api/templates/renderers/programing/strtable.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/renderers/steps/check.html` & `sloth-framework-0.1.7/sloth/api/templates/renderers/steps/check.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/renderers/utils/steps.html` & `sloth-framework-0.1.7/sloth/api/templates/renderers/utils/steps.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% load tags %}
+<div>
 <style>
     .steps-horizontal-{{ key }}{
         overflow-x: hidden;
         min-width: {{ value|length|add:2 }}00;
     }
 	.steps-horizontal-{{ key }} .step{
 		vertical-align: top;
@@ -78,7 +79,8 @@
         <div class="step">
             <div class="cicle {% if date %}active bg-primary border border-primary{% endif %}">{{ forloop.counter }}</div>
             <div class="text">{{ step }} {% if date %}<div class="text-date">{{ date }}</div>{% endif %}</div>
         </div>
     {% endfor %}
 </div>
 {% endif %}
+</div>
```

### Comparing `sloth-framework-0.1.6/sloth/api/templates/renderers/utils/table.html` & `sloth-framework-0.1.7/sloth/api/templates/renderers/utils/table.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/themes/dark.html` & `sloth-framework-0.1.7/sloth/api/templates/themes/dark.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/valueset/fieldset-group.html` & `sloth-framework-0.1.7/sloth/api/templates/valueset/fieldset-group.html`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
                 {% include 'valueset/fieldset.html' with data=fieldset %}
             {% endfor %}
         {% else %}
             {% include 'valueset/fieldset.html' with data=item %}
         {% endif %}
     {% endfor %}
 {% else %}
-    <div class="fieldset-group">
+    <div class="fieldset-group" id="{{ item.key }}" data-path="{{ item.path }}" data-tab="">
         <div class="fieldset-title">
             <h5>{{ item.name }}</h5>
         </div>
         <div class="fieldset-action-bar" style="margin-right:18px">
               {% if item.actions %}
                   {% include "dashboard/actions.html" with uuid=item.uuid target="model" actions=item.actions   %}
               {% endif %}
@@ -33,14 +33,15 @@
         </ul>
         <script>
             function hideTitles{{ item.uuid }}(){
                 $('#fieldset-group-{{ item.uuid }}-tab').find('.fieldset-title,.queryset-title').hide();
             }
             function reloadFieldsetGroup{{ item.uuid }}(tab, path, type){
                 // $(document).setCookie('current_tab', tab);
+                $('#{{ item.key }}').data('tab', tab);
                 $(document.body).addClass('page-loading');
                 $('#fieldset-group-{{ item.uuid }}').find('.nav-link.'+tab).find('.spinner-border').removeClass('d-none');
                 $.ajax({
                     url:path,
                     data:{tab:1},
                     success:function( html ) {
                         $('#fieldset-group-{{ item.uuid }}-tab').html(html).initialize();
```

### Comparing `sloth-framework-0.1.6/sloth/api/templates/valueset/fieldset-list.html` & `sloth-framework-0.1.7/sloth/api/templates/valueset/fieldset-list.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/valueset/fieldset.html` & `sloth-framework-0.1.7/sloth/api/templates/valueset/fieldset.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/valueset/value.html` & `sloth-framework-0.1.7/sloth/api/templates/valueset/value.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templates/valueset/valueset.html` & `sloth-framework-0.1.7/sloth/api/templates/valueset/valueset.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/templatetags/tags.py` & `sloth-framework-0.1.7/sloth/api/templatetags/tags.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/urls.py` & `sloth-framework-0.1.7/sloth/api/urls.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/api/views.py` & `sloth-framework-0.1.7/sloth/api/views.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/cloud/printer.py` & `sloth-framework-0.1.7/sloth/cloud/printer.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/cloud/server.py` & `sloth-framework-0.1.7/sloth/cloud/server.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/conf/settings.py` & `sloth-framework-0.1.7/sloth/conf/settings.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/core/base.py` & `sloth-framework-0.1.7/sloth/core/base.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/core/queryset.py` & `sloth-framework-0.1.7/sloth/core/queryset.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/core/statistics.py` & `sloth-framework-0.1.7/sloth/core/statistics.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/core/validation.py` & `sloth-framework-0.1.7/sloth/core/validation.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/core/valueset.py` & `sloth-framework-0.1.7/sloth/core/valueset.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/db/models/__init__.py` & `sloth-framework-0.1.7/sloth/db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/test/__init__.py` & `sloth-framework-0.1.7/sloth/test/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/test/selenium/__init__.py` & `sloth-framework-0.1.7/sloth/test/selenium/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 from django.conf import settings
 from django.core.management import call_command
 from django.contrib.staticfiles.testing import LiveServerTestCase
 from django.contrib.staticfiles.handlers import StaticFilesHandler
 from django.contrib.auth.models import User
 from sloth.test.selenium.browser import Browser
 from subprocess import DEVNULL, check_call
+from django.core.servers.basehttp import WSGIServer
+
+
+WSGIServer.handle_error = lambda *args, **kwargs: None
 
 
 class TestStaticFilesHandler(StaticFilesHandler):
     def _middleware_chain(self, request):
         from django.http import HttpResponse
         return HttpResponse()
 
@@ -122,21 +126,31 @@
         cls.browser.close()
         cls.browser.quit()
         cls.browser.service.stop()
         # len(self._resultForDoCleanups.errors)>0
 
     def save(self, name='state'):
         dbname = settings.DATABASES['default']['NAME']
-        cmd = 'pg_dump -U postgres -d {} --inserts --data-only --no-owner --file={}.sql'.format(dbname, name)
-        check_call(cmd.split(), stdout=DEVNULL, stderr=DEVNULL)
+        if 'sqlite3' in settings.DATABASES['default']['ENGINE']:
+            cmd = 'sqlite3 {} ".dump" > {}.sql'.format(dbname, name)
+            os.system(cmd)
+        else:
+            cmd = 'pg_dump -U postgres -d {} --inserts --data-only --no-owner --file={}.sql'.format(dbname, name)
+            check_call(cmd.split(), stdout=DEVNULL, stderr=DEVNULL)
 
     def resume(self, name='state'):
         dbname = settings.DATABASES['default']['NAME']
         cursor = connection.cursor()
-        tables = [m._meta.db_table for c in apps.get_app_configs() for m in c.get_models()]
-        for table in tables:
-            cursor.execute('truncate table {} cascade;'.format(table))
-        cmd = 'psql -U postgres -d {} --file={}.sql'.format(dbname, name)
-        check_call(cmd.split(), stdout=DEVNULL, stderr=DEVNULL)
+        if 'sqlite3' in settings.DATABASES['default']['ENGINE']:
+            cmd = 'sqlite3 {} "PRAGMA writable_schema = 1;DELETE FROM sqlite_master;PRAGMA writable_schema = 0;VACUUM;PRAGMA integrity_check;"'.format(dbname)
+            os.system(cmd)
+            cmd = 'cat {}.sql | sqlite3 {}'.format(name, dbname)
+            os.system(cmd)
+        else:
+            tables = [m._meta.db_table for c in apps.get_app_configs() for m in c.get_models()]
+            for table in tables:
+                cursor.execute('truncate table {} cascade;'.format(table))
+            cmd = 'psql -U postgres -d {} --file={}.sql'.format(dbname, name)
+            check_call(cmd.split(), stdout=DEVNULL, stderr=DEVNULL)
 
     def loaddata(self, fixture_path):
         call_command('loaddata', '--skip-checks', fixture_path)
```

### Comparing `sloth-framework-0.1.6/sloth/test/selenium/browser.py` & `sloth-framework-0.1.7/sloth/test/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/utils/__init__.py` & `sloth-framework-0.1.7/sloth/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/utils/formatter/__init__.py` & `sloth-framework-0.1.7/sloth/utils/formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/utils/http/__init__.py` & `sloth-framework-0.1.7/sloth/utils/http/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/utils/icons/bootstrap.py` & `sloth-framework-0.1.7/sloth/utils/icons/bootstrap.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/utils/icons/fontawesome.py` & `sloth-framework-0.1.7/sloth/utils/icons/fontawesome.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/utils/icons/materialicons.py` & `sloth-framework-0.1.7/sloth/utils/icons/materialicons.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth/utils/log/sql.py` & `sloth-framework-0.1.7/sloth/utils/log/sql.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.6/sloth_framework.egg-info/PKG-INFO` & `sloth-framework-0.1.7/sloth_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sloth-framework
-Version: 0.1.6
+Version: 0.1.7
 Summary: Metadata-based web framework for the development of management information systems
 Home-page: http://sloth.aplicativo.click/
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `sloth-framework-0.1.6/sloth_framework.egg-info/SOURCES.txt` & `sloth-framework-0.1.7/sloth_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

