# Comparing `tmp/nautobot_circuit_maintenance-0.6.2.tar.gz` & `tmp/nautobot_circuit_maintenance-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_circuit_maintenance-0.6.2.tar", max compression
+gzip compressed data, was "nautobot_circuit_maintenance-1.0.0.tar", max compression
```

## Comparing `nautobot_circuit_maintenance-0.6.2.tar` & `nautobot_circuit_maintenance-1.0.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0    10174 2023-01-30 19:49:41.829177 nautobot_circuit_maintenance-0.6.2/LICENSE
--rw-r--r--   0        0        0    18707 2023-01-30 19:49:41.829177 nautobot_circuit_maintenance-0.6.2/README.md
--rw-r--r--   0        0        0     4493 2023-01-30 19:49:41.833177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/__init__.py
--rw-r--r--   0        0        0      658 2023-01-30 19:49:41.833177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/admin.py
--rw-r--r--   0        0        0       54 2023-01-30 19:49:41.833177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/api/__init__.py
--rw-r--r--   0        0        0     1800 2023-01-30 19:49:41.833177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/api/serializers.py
--rw-r--r--   0        0        0      493 2023-01-30 19:49:41.833177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/api/urls.py
--rw-r--r--   0        0        0     2104 2023-01-30 19:49:41.833177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/api/views.py
--rw-r--r--   0        0        0     1498 2023-01-30 19:49:41.833177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/choices.py
--rw-r--r--   0        0        0     2298 2023-01-30 19:49:41.833177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/custom_validators.py
--rw-r--r--   0        0        0      616 2023-01-30 19:49:41.833177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/enum.py
--rw-r--r--   0        0        0     4226 2023-01-30 19:49:41.833177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/filters.py
--rw-r--r--   0        0        0     2922 2023-01-30 19:49:41.833177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/fixtures/handle_notifications_job.yaml
--rw-r--r--   0        0        0     2190 2023-01-30 19:49:41.833177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/fixtures/source_gmail_api.yaml
--rw-r--r--   0        0        0     1800 2023-01-30 19:49:41.833177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/fixtures/source_imap.yaml
--rw-r--r--   0        0        0     7262 2023-01-30 19:49:41.833177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/forms.py
--rw-r--r--   0        0        0       27 2023-01-30 19:49:41.833177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/handle_notifications/__init__.py
--rw-r--r--   0        0        0    18672 2023-01-30 19:49:41.833177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/handle_notifications/handler.py
--rw-r--r--   0        0        0    26888 2023-01-30 19:49:41.833177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/handle_notifications/sources.py
--rw-r--r--   0        0        0      355 2023-01-30 19:49:41.833177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/jobs/__init__.py
--rw-r--r--   0        0        0     6863 2023-01-30 19:49:41.833177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/jobs/site_search.py
--rw-r--r--   0        0        0     3044 2023-01-30 19:49:41.833177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/metrics_app.py
--rw-r--r--   0        0        0     9788 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/migrations/0001_initial.py
--rw-r--r--   0        0        0     1479 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/migrations/0002_notification_secrets_out_of_db.py
--rw-r--r--   0        0        0     1648 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/migrations/0003_improve_rawnotification.py
--rw-r--r--   0        0        0     2006 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/migrations/0004_raw_md5.py
--rw-r--r--   0        0        0      406 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/migrations/0005_notificationsource__token.py
--rw-r--r--   0        0        0      302 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/migrations/0006_fake_migration_to_update_custom_fields.py
--rw-r--r--   0        0        0      455 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/migrations/0007_notificationsource_attach_all_providers.py
--rw-r--r--   0        0        0     1424 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/migrations/0008_raw_binary.py
--rw-r--r--   0        0        0      548 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/migrations/0009_auto_20210916_1519.py
--rw-r--r--   0        0        0     1875 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/migrations/0010_rawnotification_stamp.py
--rw-r--r--   0        0        0      573 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/migrations/0011_mysql.py
--rw-r--r--   0        0        0        0 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/migrations/__init__.py
--rw-r--r--   0        0        0    11121 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/models.py
--rw-r--r--   0        0        0     1831 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/navigation.py
--rw-r--r--   0        0        0     2381 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/tables.py
--rw-r--r--   0        0        0      705 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/template_content.py
--rw-r--r--   0        0        0     1343 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/circuit_extension.html
--rw-r--r--   0        0        0     5914 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/circuit_maintenance_overview.html
--rw-r--r--   0        0        0     2618 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/circuitimpact.html
--rw-r--r--   0        0        0    11188 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/circuitmaintenance.html
--rw-r--r--   0        0        0     2151 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/note.html
--rw-r--r--   0        0        0     2812 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/notificationsource.html
--rw-r--r--   0        0        0     1575 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/parsednotification.html
--rw-r--r--   0        0        0     2313 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/rawnotification.html
--rw-r--r--   0        0        0       35 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/tests/__init__.py
--rw-r--r--   0        0        0     3512 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/tests/test_api.py
--rw-r--r--   0        0        0     4231 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/tests/test_app_metrics.py
--rw-r--r--   0        0        0      611 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/tests/test_basics.py
--rw-r--r--   0        0        0     4015 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/tests/test_graphql.py
--rw-r--r--   0        0        0    33322 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/tests/test_handler.py
--rw-r--r--   0        0        0     2623 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/tests/test_jobs.py
--rw-r--r--   0        0        0     3414 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/tests/test_models.py
--rw-r--r--   0        0        0    30744 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/tests/test_sources.py
--rw-r--r--   0        0        0    23182 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/tests/test_views.py
--rw-r--r--   0        0        0     5250 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/urls.py
--rw-r--r--   0        0        0    22471 2023-01-30 19:49:41.837177 nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/views.py
--rw-r--r--   0        0        0     2952 2023-01-30 19:49:51.537315 nautobot_circuit_maintenance-0.6.2/pyproject.toml
--rw-r--r--   0        0        0    20502 1970-01-01 00:00:00.000000 nautobot_circuit_maintenance-0.6.2/setup.py
--rw-r--r--   0        0        0    20034 1970-01-01 00:00:00.000000 nautobot_circuit_maintenance-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-05-29 05:52:42.796839 nautobot_circuit_maintenance-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4803 2023-05-29 05:52:42.796839 nautobot_circuit_maintenance-1.0.0/README.md
+-rw-r--r--   0        0        0     4618 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/__init__.py
+-rw-r--r--   0        0        0      658 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/admin.py
+-rw-r--r--   0        0        0       54 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/api/__init__.py
+-rw-r--r--   0        0        0     1800 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/api/serializers.py
+-rw-r--r--   0        0        0      493 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/api/urls.py
+-rw-r--r--   0        0        0     2104 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/api/views.py
+-rw-r--r--   0        0        0     1498 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/choices.py
+-rw-r--r--   0        0        0     2298 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/custom_validators.py
+-rw-r--r--   0        0        0      616 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/enum.py
+-rw-r--r--   0        0        0     4226 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/filters.py
+-rw-r--r--   0        0        0     2922 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/fixtures/handle_notifications_job.yaml
+-rw-r--r--   0        0        0     2190 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/fixtures/source_gmail_api.yaml
+-rw-r--r--   0        0        0     1800 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/fixtures/source_imap.yaml
+-rw-r--r--   0        0        0     7358 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/forms.py
+-rw-r--r--   0        0        0       27 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/handle_notifications/__init__.py
+-rw-r--r--   0        0        0    18672 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/handle_notifications/handler.py
+-rw-r--r--   0        0        0    26888 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/handle_notifications/sources.py
+-rw-r--r--   0        0        0      355 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/jobs/__init__.py
+-rw-r--r--   0        0        0     6814 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/jobs/site_search.py
+-rw-r--r--   0        0        0     3044 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/metrics_app.py
+-rw-r--r--   0        0        0     9788 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1479 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/migrations/0002_notification_secrets_out_of_db.py
+-rw-r--r--   0        0        0     1648 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/migrations/0003_improve_rawnotification.py
+-rw-r--r--   0        0        0     2006 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/migrations/0004_raw_md5.py
+-rw-r--r--   0        0        0      406 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/migrations/0005_notificationsource__token.py
+-rw-r--r--   0        0        0      302 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/migrations/0006_fake_migration_to_update_custom_fields.py
+-rw-r--r--   0        0        0      455 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/migrations/0007_notificationsource_attach_all_providers.py
+-rw-r--r--   0        0        0     1424 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/migrations/0008_raw_binary.py
+-rw-r--r--   0        0        0      548 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/migrations/0009_auto_20210916_1519.py
+-rw-r--r--   0        0        0     1875 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/migrations/0010_rawnotification_stamp.py
+-rw-r--r--   0        0        0      573 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/migrations/0011_mysql.py
+-rw-r--r--   0        0        0        0 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/migrations/__init__.py
+-rw-r--r--   0        0        0    11137 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/models.py
+-rw-r--r--   0        0        0     2657 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/navigation.py
+-rw-r--r--   0        0        0     2381 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/tables.py
+-rw-r--r--   0        0        0      705 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/template_content.py
+-rw-r--r--   0        0        0     1343 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/circuit_extension.html
+-rw-r--r--   0        0        0     5914 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/circuit_maintenance_overview.html
+-rw-r--r--   0        0        0      845 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/circuitimpact.html
+-rw-r--r--   0        0        0     9205 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/circuitmaintenance.html
+-rw-r--r--   0        0        0     1209 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/note.html
+-rw-r--r--   0        0        0     2515 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/notificationsource.html
+-rw-r--r--   0        0        0     1443 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/parsednotification.html
+-rw-r--r--   0        0        0     1893 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/rawnotification.html
+-rw-r--r--   0        0        0       35 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/tests/__init__.py
+-rw-r--r--   0        0        0     3512 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/tests/test_api.py
+-rw-r--r--   0        0        0     4231 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/tests/test_app_metrics.py
+-rw-r--r--   0        0        0     1533 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/tests/test_basic.py
+-rw-r--r--   0        0        0      611 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/tests/test_basics.py
+-rw-r--r--   0        0        0     4015 2023-05-29 05:52:42.808839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/tests/test_graphql.py
+-rw-r--r--   0        0        0    33322 2023-05-29 05:52:42.812839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/tests/test_handler.py
+-rw-r--r--   0        0        0     2623 2023-05-29 05:52:42.812839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/tests/test_jobs.py
+-rw-r--r--   0        0        0     3414 2023-05-29 05:52:42.812839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/tests/test_models.py
+-rw-r--r--   0        0        0    30768 2023-05-29 05:52:42.812839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/tests/test_sources.py
+-rw-r--r--   0        0        0    23584 2023-05-29 05:52:42.812839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/tests/test_views.py
+-rw-r--r--   0        0        0     5250 2023-05-29 05:52:42.812839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/urls.py
+-rw-r--r--   0        0        0    22471 2023-05-29 05:52:42.812839 nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/views.py
+-rw-r--r--   0        0        0     3989 2023-05-29 05:52:59.808799 nautobot_circuit_maintenance-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6147 1970-01-01 00:00:00.000000 nautobot_circuit_maintenance-1.0.0/PKG-INFO
```

### Comparing `nautobot_circuit_maintenance-0.6.2/LICENSE` & `nautobot_circuit_maintenance-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/__init__.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,21 +73,21 @@
     NotificationSource.objects.exclude(name__in=desired_notification_sources_names).delete()
 
 
 class CircuitMaintenanceConfig(PluginConfig):
     """Plugin configuration for the Circuit Maintenance plugin."""
 
     name = "nautobot_circuit_maintenance"
-    verbose_name = "Circuit Maintenance"
+    verbose_name = "Circuit Maintenance Management"
     version = __version__
     author = "Network to Code, LLC"
     author_email = "opensource@networktocode.com"
-    description = "Automatically handle network circuit maintenance notifications."
+    description = "Nautobot App that automatically manages network circuit maintenance notifications. Dynamically reads email inboxes (or APIs) and updates Nautobot mapping circuit maintenances to devices."
     base_url = "circuit-maintenance"
-    min_version = "1.0.0-beta.4"
+    min_version = "1.4"
     max_version = "1.999"
     required_settings = []
     default_settings = {
         "raw_notification_initial_days_since": 7,
         "raw_notification_size": 8192,
         "dashboard_n_days": 30,
         "overlap_job_exclude_no_impact": False,
```

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/admin.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/admin.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/api/serializers.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/api/serializers.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/api/views.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/api/views.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/choices.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/choices.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/custom_validators.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/custom_validators.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/enum.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/enum.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/filters.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/fixtures/handle_notifications_job.yaml` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/fixtures/handle_notifications_job.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/fixtures/source_gmail_api.yaml` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/fixtures/source_gmail_api.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/fixtures/source_imap.yaml` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/fixtures/source_imap.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/forms.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,16 @@
 
 
 class NoteCSVForm(CustomFieldModelCSVForm):
     """Form for creating bulk Notes."""
 
     class Meta:  # noqa: D106 "Missing docstring in public nested class"
         model = Note
-        fields = Note.csv_headers
+        # Omit the `last_updated` field from the CSV form, as it can't be set by the user.
+        fields = Note.csv_headers[:-1]
 
 
 class RawNotificationFilterSetForm(BootstrapMixin, CustomFieldFilterForm):
     """Form for filtering Raw Notification instances."""
 
     model = RawNotification
```

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/handle_notifications/handler.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/handle_notifications/handler.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/handle_notifications/sources.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/handle_notifications/sources.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/jobs/site_search.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/jobs/site_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 PLUGIN_SETTINGS = settings.PLUGINS_CONFIG.get("nautobot_circuit_maintenance", {})
 CIRCUIT_MAINTENANCE_TAG_COLOR = "Purple"
 
 name = "Circuit Maintenance"  # pylint: disable=invalid-name
 
 
-def check_for_overlap(record1: CircuitMaintenance, record2: CircuitMaintenance):
+def check_for_overlap(record1: CircuitMaintenance, record2: CircuitMaintenance) -> bool:
     """Checks for the overlap of two circuit maintenance records.
 
     Args:
         record1 (CircuitMaintenance): First maintenance record
         record2 (CircuitMaintenance): Second maintenance record
 
     Returns:
@@ -45,15 +45,15 @@
     for term in [circuit.termination_a, circuit.termination_z]:
         if term is not None and getattr(term, "provider_network") is None:
             site_set.add(term.site)
 
     return site_set
 
 
-def build_sites_to_maintenance_mapper(maintenance_queryset):
+def build_sites_to_maintenance_mapper(maintenance_queryset) -> dict:
     """Build a site to circuit maintenance mapper so the data can be quickly accessed of what possible overlaps.
 
     Leverages defaultdict to provide the default value of an empty set to each key that will be added. Then adds each
     particular circuit maintenance object to the dictionary to be used as a map of maintenances going on at the site.
     Build a data dictionary that maps sites to circuit maintenances:
 
     data_dict = {
@@ -90,17 +90,14 @@
     """Nautobot Job definition for finding sites without redundant circuit for impactful maintenance.
 
     Current iteration of this job assumes that many sites will be only dual carrier connected. The searches are going
     to search for a single overlap in this first iteration.
 
     Future iterations may include the ability to search for multiple circuit overlaps that would allow for just a single
     circuit to be available.
-
-    Args:
-        Job (Nautobot Job): Nautobot Job parent class
     """
 
     job_debug = BooleanVar(description="Enable for more verbose debug logging")
 
     class Meta:
         """Meta definition for the Job."""
```

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/metrics_app.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/metrics_app.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/migrations/0001_initial.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/migrations/0002_notification_secrets_out_of_db.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/migrations/0002_notification_secrets_out_of_db.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/migrations/0003_improve_rawnotification.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/migrations/0003_improve_rawnotification.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/migrations/0004_raw_md5.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/migrations/0004_raw_md5.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/migrations/0008_raw_binary.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/migrations/0008_raw_binary.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/migrations/0009_auto_20210916_1519.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/migrations/0009_auto_20210916_1519.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/migrations/0010_rawnotification_stamp.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/migrations/0010_rawnotification_stamp.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/migrations/0011_mysql.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/migrations/0011_mysql.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/models.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         max_length=50,
         choices=NoteLevelChoices,
         null=True,
         blank=True,
     )
     comment = models.TextField()
 
-    csv_headers = ["maintenance", "title", "level", "comment"]
+    csv_headers = ["maintenance", "title", "level", "comment", "last_updated"]
 
     class Meta:  # noqa: D106 "Missing docstring in public nested class"
         ordering = ["last_updated"]
         unique_together = ["maintenance", "title"]
 
     def __str__(self):
         """String value for HTML rendering."""
```

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/tables.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/tables.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/template_content.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/template_content.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/circuit_extension.html` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/circuit_extension.html`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/circuit_maintenance_overview.html` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/circuit_maintenance_overview.html`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/circuitmaintenance.html` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/circuitmaintenance.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,104 +1,60 @@
-{% extends 'base.html' %}
-{% load buttons %}
-{% load custom_links %}
+{% extends 'generic/object_detail.html' %}
 {% load helpers %}
-{% load plugins %}
 
-{% block title %}{{ object }}{% endblock %}
+{% block masthead %}
+    <h1>Maintenance ID: {% block title %}{{ object }}{% endblock %}</h1>
+{% endblock masthead %}
 
-{% block header %}
-
-    <div class="row noprint">
-        <div class="col-sm-8 col-md-9">
-            <ol class="breadcrumb">
-                <li><a href="{% url 'plugins:nautobot_circuit_maintenance:circuitmaintenance_list' %}">Circuit Maintenances</a></li>
-                <li><a>{{ object.name }}</a></li>
-            </ol>
+{% block content_left_page %}
+    <div class="panel panel-default">
+        <div class="panel-heading">
+            <strong>Info</strong>
         </div>
+        <table class="table table-hover panel-body attr-table">
+            <tr>
+                <td>Name</td>
+                <td>
+                    <span class="">{{ object.name }}</span>
+                </td>
+            </tr>
+            <tr>
+                <td>Description</td>
+                <td>{{ object.description }}</td>
+            </tr>
+            <tr>
+                <td>Status</td>
+                <td>{{ object.status }}</td>
+            </tr>
+            <tr>
+                <td>Start Time</td>
+                <td>{{ object.start_time }}</td>
+            </tr>
+            <tr>
+                <td>End Time</td>
+                <td>{{ object.end_time }}</td>
+            </tr>
+            <tr>
+                <td>Acknowledged</td>
+                <td>{{ object.ack }}</td>
+            </tr>
+            <tr>
+                <td>Notifying Provider</td>
+                {% with object.parsednotification_set.first.raw_notification.provider as provider %}
+                    {% if provider %}
+                        <td><a href="{{ provider.get_absolute_url }}">{{ provider }}</a></td>
+                    {% else %}
+                        <td>{{ provider | placeholder }}</td>
+                    {% endif %}
+                {% endwith %}
+        </table>
     </div>
-
-    <div class="pull-right noprint">
-        {% plugin_buttons object %}
-        {% if perms.nautobot_circuit_maintenance.edit_circuitmaintenance %}
-            {% edit_button object %}
-        {% endif %}
-        {% if perms.nautobot_circuit_maintenance.delete_circuitmaintenance %}
-            {% delete_button object %}
-        {% endif %}
-    </div>
-
-    <h1>Maintenance ID: {{ object }}</h1>
-    {% include 'inc/created_updated.html' %}
-    <div class="pull-right noprint">
-        {% custom_links object %}
-    </div>
-    <ul class="nav nav-tabs">
-        <li role="presentation"{% if not active_tab %} class="active"{% endif %}>
-            <a href="{{ object.get_absolute_url }}">Circuit Maintenance</a>
-        </li>
-        {% if perms.extras.view_objectchange %}
-            <li role="presentation"{% if active_tab == 'changelog' %} class="active"{% endif %}>
-                <a href="{% url 'plugins:nautobot_circuit_maintenance:circuitmaintenance_changelog' pk=object.pk %}">Change Log</a>
-            </li>
-        {% endif %}
-    </ul>
-
 {% endblock %}
 
-{% block content %}
-
-    <div class="row">
-        <div class="col-md-6">
-            <div class="panel panel-default">
-                <div class="panel-heading">
-                    <strong>Info</strong>
-                </div>
-                <table class="table table-hover panel-body attr-table">
-                    <tr>
-                        <td>Name</td>
-                        <td>
-                            <span class="">{{ object.name }}</span>
-                        </td>
-                    </tr>
-                    <tr>
-                        <td>Description</td>
-                        <td>{{ object.description }}</td>
-                    </tr>
-                    <tr>
-                        <td>Status</td>
-                        <td>{{ object.status }}</td>
-                    </tr>
-                    <tr>
-                        <td>Start Time</td>
-                        <td>{{ object.start_time }}</td>
-                    </tr>
-                    <tr>
-                        <td>End Time</td>
-                        <td>{{ object.end_time }}</td>
-                    </tr>
-                    <tr>
-                        <td>Acknowledged</td>
-                        <td>{{ object.ack }}</td>
-                    </tr>
-                    <tr>
-                        <td>Notifying Provider</td>
-                        {% with object.parsednotification_set.first.raw_notification.provider as provider %}
-                            {% if provider %}
-                                <td><a href="{{ provider.get_absolute_url }}">{{ provider }}</a></td>
-                            {% else %}
-                                <td>{{ provider | placeholder }}</td>
-                            {% endif %}
-                        {% endwith %}
-                </table>
-            </div>
-        </div>
-    </div>
-
-
+{% block content_full_width_page %}
     <div class="panel panel-default">
         <div class="panel-heading">
             <strong>Circuits</strong>
             <div class="pull-right noprint">
             {% if perms.nautobot_circuit_maintenance.add_circuitmaintenance %}
                 <a href="{% url 'plugins:nautobot_circuit_maintenance:circuitimpact_add' %}?maintenance={{ object.id }}&return_url={{ object.get_absolute_url }}" >
                     <span class="mdi mdi-plus" aria-hidden="true"></span> Add
@@ -166,16 +122,14 @@
                 </tr>
                 {% endfor %}
             </tbody>
         </table>
         {% endif %}
     </div>
 
-
-
     <div class="panel panel-default">
         <div class="panel-heading">
             <strong>Notes</strong>
             <div class="pull-right noprint">
             {% if perms.nautobot_circuit_maintenance.add_circuitmaintenance %}
                 <a href="{% url 'plugins:nautobot_circuit_maintenance:note_add' %}?maintenance={{ object.id }}&return_url={{ object.get_absolute_url }}" >
                     <span class="mdi mdi-plus" aria-hidden="true"></span> Add
@@ -226,15 +180,14 @@
                 </tr>
                 {% endfor %}
             </tbody>
         </table>
         {% endif %}
     </div>
 
-
     <div class="panel panel-default">
         <div class="panel-heading">
             <strong>Notifications</strong>
         </div>
         {% if not parsednotification %}
         <div class="panel-body">
             <span class="text-muted">None</span>
@@ -261,12 +214,8 @@
                     </td>
                 </tr>
                 {% endfor %}
             </tbody>
         </table>
         {% endif %}
     </div>
-    {% include 'inc/custom_fields_panel.html' %}
-    {% include 'inc/relationships_panel.html' %}
-    {% include 'extras/inc/tags_panel.html' with tags=object.tags.all url='nautobot_circuit_maintenance:circuitmaintenance_list' %}
-
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,33 +1,20 @@
-{% extends 'base.html' %} {% load buttons %} {% load custom_links %} {% load
-helpers %} {% load plugins %} {% block title %}{{ object }}{% endblock %} {%
-block header %}
-   1. Circuit_Maintenances
-   2. {{ object.name }}
-{% plugin_buttons object %} {% if
-perms.nautobot_circuit_maintenance.edit_circuitmaintenance %} {% edit_button
-object %} {% endif %} {% if
-perms.nautobot_circuit_maintenance.delete_circuitmaintenance %} {%
-delete_button object %} {% endif %}
-****** Maintenance ID: {{ object }} ******
-{% include 'inc/created_updated.html' %}
-{% custom_links object %}
-    * % if not active_tab %} class="active"{% endif %}> Circuit_Maintenance
-{% if perms.extras.view_objectchange %}
-% if active_tab == 'changelog' %} class="active"{% endif %}> Change_Log
-{% endif %}
-{% endblock %} {% block content %}
+{% extends 'generic/object_detail.html' %} {% load helpers %} {% block masthead
+%}
+****** Maintenance ID: {% block title %}{{ object }}{% endblock %} ******
+{% endblock masthead %} {% block content_left_page %}
 Info
 Name               {{ object.name }}
 Description        {{ object.description }}
 Status             {{ object.status }}
 Start Time         {{ object.start_time }}
 End Time           {{ object.end_time }}
 Acknowledged       {{ object.ack }}
 Notifying Provider {{_provider_}}           {{ provider | placeholder }}
+{% endblock %} {% block content_full_width_page %}
 Circuits
 {% if perms.nautobot_circuit_maintenance.add_circuitmaintenance %} _Add {%
 endif %}
 {% if not circuits %}
 None
 {% else %}
 ID                  Impact         Provider                 Type                 Status                             A Side                                         Z Side                                         Description
@@ -61,11 +48,8 @@
 {% else %}
 Subject                                      Date                                       JSON
 {                                            {                                          {
 {                                            {                                          {
 parsed_notification.raw_notification.subject parsed_notification.raw_notification.stamp parsed_notification.json
 }}                                           }}                                         | render_json }}
 {% endif %}
-{% include 'inc/custom_fields_panel.html' %} {% include 'inc/
-relationships_panel.html' %} {% include 'extras/inc/tags_panel.html' with
-tags=object.tags.all url='nautobot_circuit_maintenance:circuitmaintenance_list'
-%} {% endblock %}
+{% endblock %}
```

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/note.html` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/parsednotification.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,45 @@
-{% extends 'base.html' %}
-{% load buttons %}
+{% extends 'generic/object_detail.html' %}
 {% load custom_links %}
-{% load helpers %}
-{% load plugins %}
 
-{% block title %}{{ object }}{% endblock%}
 {% block header %}
 
-
 <div class="row noprint">
-    <div class="col-sm-8 col-md-9">
-        <ol class="breadcrumb">
-            <li><a href="{% url 'plugins:nautobot_circuit_maintenance:note_list' %}">Notes</a></li>
-            <li><a>{{ object }}</a></li>
-        </ol>
-    </div>
+  <div class="col-sm-8 col-md-9">
+    <ol class="breadcrumb">
+      <li><a href="{% url 'plugins:nautobot_circuit_maintenance:rawnotification_list' %}">Raw Notifications</a></li>
+      <li><a href="{{ object.raw_notification.get_absolute_url }}">{{ object.raw_notification }}</a></li>
+      <li><a>{{ object }}</a></li>
+    </ol>
+  </div>
 </div>
 
-<h1>{{ object.title }}</h1>
-
-{% include 'inc/created_updated.html' with obj=object %}
-
+<h1>{{ object }}</h1>
 <div class="pull-right noprint">{% custom_links object %}</div>
 
-<ul class="nav nav-tabs">
-  <li role="presentation"{% if not active_tab %} class="active"{% endif %}>
-      <a href="{{ object.get_absolute_url }}">Note</a>
-  </li>
-  {% if perms.extras.view_objectchange %}
-      <li role="presentation"{% if active_tab == 'changelog' %} class="active"{% endif %}>
-          <a href="{% url 'plugins:nautobot_circuit_maintenance:note_changelog' pk=object.pk %}">Change Log</a>
-      </li>
-  {% endif %}
-</ul>
-
-{% endblock %} {% block content %}
+{% endblock %}
 
-<div class="row">
-  <div class="col-md-6">
+{% block content_left_page %}
     <div class="panel panel-default">
-      <div class="panel-heading">
-        <strong>Info</strong>
-      </div>
-      <table class="table table-hover panel-body attr-table">
-        <tr>
-          <td>Title</td>
-          <td>
-            <span class="">{{ object.title }}</span>
-          </td>
-        </tr>
-        <tr>
-          <td>Level</td>
-          <td>{{ object.level }}</td>
-        </tr>
-        <tr>
-            <td>Maintenance</td>
-            <td>
-                <a href="{% url 'plugins:nautobot_circuit_maintenance:circuitmaintenance' pk=object.maintenance.id %}"
-                  >{{ object.maintenance }}</a
-                >
-              </td>
-        </tr>
-        <tr>
-            <td>Comment</td>
-            <td>{{ object.comment }}</td>
-        </tr>
-        <tr>
-            <td>Last Updated</td>
-            <td>{{ object.last_updated }}</td>
-        </tr>
-      </table>
+        <div class="panel-heading">
+            <strong>Info</strong>
+        </div>
+        <table class="table table-hover panel-body attr-table">
+            <tr>
+                <td>Maintenance</td>
+                <td><a href="{{ object.maintenance.get_absolute_url }}">{{ object.maintenance.name }}</a></td>
+            </tr>
+            <tr>
+                <td>Raw Notification</td>
+                <td><a href="{{ object.raw_notification.get_absolute_url }}">{{ object.raw_notification }}</a></td>
+            </tr>
+            <tr>
+                <td>Last Updated</td>
+                <td>{{ object.last_updated }}</td>
+            </tr>
+            <tr>
+                <td>JSON</td>
+                <td>{{ object.json|linebreaks }}</td>
+            </tr>
+        </table>
     </div>
-  </div>
-</div>
-{% include 'inc/custom_fields_panel.html' %}
-{% include 'inc/relationships_panel.html' %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,21 +1,14 @@
-{% extends 'base.html' %} {% load buttons %} {% load custom_links %} {% load
-helpers %} {% load plugins %} {% block title %}{{ object }}{% endblock%} {%
-block header %}
-   1. Notes
-   2. {{ object }}
-****** {{ object.title }} ******
-{% include 'inc/created_updated.html' with obj=object %}
+{% extends 'generic/object_detail.html' %} {% load custom_links %} {% block
+header %}
+   1. Raw_Notifications
+   2. {{_object.raw_notification_}}
+   3. {{ object }}
+****** {{ object }} ******
 {% custom_links object %}
-    * % if not active_tab %} class="active"{% endif %}> Note
-{% if perms.extras.view_objectchange %}
-% if active_tab == 'changelog' %} class="active"{% endif %}> Change_Log
-{% endif %}
-{% endblock %} {% block content %}
+{% endblock %} {% block content_left_page %}
 Info
-Title        {{ object.title }}
-Level        {{ object.level }}
-Maintenance  {{_object.maintenance_}}
-Comment      {{ object.comment }}
-Last Updated {{ object.last_updated }}
-{% include 'inc/custom_fields_panel.html' %} {% include 'inc/
-relationships_panel.html' %} {% endblock %}
+Maintenance      {{_object.maintenance.name_}}
+Raw Notification {{_object.raw_notification_}}
+Last Updated     {{ object.last_updated }}
+JSON             {{ object.json|linebreaks }}
+{% endblock %}
```

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/notificationsource.html` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/templates/nautobot_circuit_maintenance/rawnotification.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,56 @@
-{% extends 'base.html' %}
-{% load buttons %}
-{% load custom_links %}
-{% load helpers %}
-{% load plugins %}
+{% extends 'generic/object_detail.html' %}
 
-{% block title %}{{ object }}{% endblock%}
-{% block header %}
+{% block buttons %}{% endblock %}
 
-<div class="row noprint">
-    <div class="col-sm-8 col-md-9">
-        <ol class="breadcrumb">
-            <li><a href="{% url 'plugins:nautobot_circuit_maintenance:notificationsource_list' %}">Notification Sources</a></li>
-            <li><a>{{ object.name }}</a></li>
-        </ol>
-    </div>
-</div>
-
-<h1>{{ object.name }}</h1>
-
-{% include 'inc/created_updated.html' with obj=object %}
-
-<div class="pull-right noprint">{% custom_links object %}</div>
-
-{% endblock %} {% block content %}
-
-<div class="row">
-  <div class="col-md-6">
+{% block content_left_page %}
     <div class="panel panel-default">
-      <div class="panel-heading">
-        <strong>Info</strong>
-      </div>
-      <table class="table table-hover panel-body attr-table">
-      <tr>
-        <td>Name</td>
-        <td>
-          <span class="">{{ object.name }}</span>
-        </td>
-      </tr>
-      <tr>
-      <td>Slug</td>
-      <td>{{ object.slug }}</td>
-      </tr>
-      <tr>
-      <td>Type</td>
-      <td>{{ source_type }}</td>
-      </tr>
-      <tr>
-      <td>Account ID</td>
-      <td>{{ account }}</td>
-      </tr>
-      <tr>
-      <td>Providers</td>
-      <td>
-          <ul>
-              {% for provider in providers %}
-                  <li><a href="{{ provider.get_absolute_url }}">{{ provider.name }}</a></li>
-              {% endfor %}
-          </ul>
-      </td>
-      </tr>
-      <td>Attach all providers</td>
-      <td>
-        {% if object.attach_all_providers %}
-            <span class="text-success"><i class="mdi mdi-check-bold"></i></span>
-        {% else %}
-            <span class="text-danger"><i class="mdi mdi-close"></i></span>
-        {% endif %}
-      </td>
-      </tr>
-      {% if authentication_message %}
-      <tr>
-      <td>Authentication Status</td>
-      <td>{{ authentication_message }}</td>
-      </tr>
-      {% endif %}
-
-      </table>
+        <div class="panel-heading">
+            <strong>Info</strong>
+        </div>
+        <table class="table table-hover panel-body attr-table">
+            <tr>
+                <td>Subject</td>
+                <td>
+                    <span class="">{{ object.subject }}</span>
+                </td>
+            </tr>
+            <tr>
+                <td>Provider</td>
+                <td><a href="{{ object.provider.get_absolute_url }}">{{ object.provider }}</a></td>
+            </tr>
+            <tr>
+                <td>Sender</td>
+                <td>{{ object.sender }}</td>
+            </tr>
+            <tr>
+                <td>Source</td>
+                <td><a href="{{ object.source.get_absolute_url }}">{{ object.source }}</a></td>
+            </tr>
+            <tr>
+                <td>Parsed</td>
+                <td>
+                    {% if parsed_notification %}
+                        <a href="{{ parsed_notification.get_absolute_url }}">{{ object.parsed }}</a>,
+                        leading to maintenance <a href="{{ parsed_notification.maintenance.get_absolute_url }}">
+                            {{ parsed_notification.maintenance }}
+                        </a>
+                    {% else %}
+                        {{ object.parsed }}
+                    {% endif %}
+                </td>
+            </tr>
+            <tr>
+                <td>Stamp</td>
+                <td>{{ object.stamp }}</td>
+            </tr>
+            <tr>
+                <td>Last Updated</td>
+                <td>{{ object.last_updated }}</td>
+            </tr>
+            <tr>
+                <td>Raw</td>
+                <td><pre>{{ raw_repr|linebreaks }}</pre></td>
+            </tr>
+        </table>
     </div>
-    <div class="btn-group">
-      <a href="{% url 'plugins:nautobot_circuit_maintenance:notificationsource_validate' slug=object.slug %}?return_url={{ object.get_absolute_url }}" class="btn  btn-xs">
-        <button type="submit" name="_validate" class="btn btn-primary">Validate Authentication</button>
-      </a>
-      {% if perms.nautobot_circuit_maintenance.add_circuitmaintenance %}
-      <a href="{% url 'plugins:nautobot_circuit_maintenance:notificationsource_edit' slug=object.slug %}?return_url={{ object.get_absolute_url }}" class="btn  btn-xs">
-        <button type="submit" name="_validate" class="btn btn-primary btn-warning">Edit</button>
-      </a>
-      {% endif %}
-  </div>
-  </div>
-</div>
-{% include 'inc/custom_fields_panel.html' %}
-{% include 'inc/relationships_panel.html' %}
-
-
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,22 +1,14 @@
-{% extends 'base.html' %} {% load buttons %} {% load custom_links %} {% load
-helpers %} {% load plugins %} {% block title %}{{ object }}{% endblock%} {%
-block header %}
-   1. Notification_Sources
-   2. {{ object.name }}
-****** {{ object.name }} ******
-{% include 'inc/created_updated.html' with obj=object %}
-{% custom_links object %}
-{% endblock %} {% block content %}
+{% extends 'generic/object_detail.html' %} {% block buttons %}{% endblock %} {%
+block content_left_page %}
 Info
-Name                  {{ object.name }}
-Slug                  {{ object.slug }}
-Type                  {{ source_type }}
-Account ID            {{ account }}
-                          * {% for provider in providers %}
-Providers                 * {{_provider.name_}}
-                          * {% endfor %}
-Authentication Status {{ authentication_message }}
-Validate_Authentication {% if
-perms.nautobot_circuit_maintenance.add_circuitmaintenance %} Edit {% endif %}
-{% include 'inc/custom_fields_panel.html' %} {% include 'inc/
-relationships_panel.html' %} {% endblock %}
+Subject      {{ object.subject }}
+Provider     {{_object.provider_}}
+Sender       {{ object.sender }}
+Source       {{_object.source_}}
+             {% if parsed_notification %} {{_object.parsed_}}, leading to
+Parsed       maintenance {{_parsed_notification.maintenance_}} {% else %} {
+             { object.parsed }} {% endif %}
+Stamp        {{ object.stamp }}
+Last Updated {{ object.last_updated }}
+Raw          {{ raw_repr|linebreaks }}
+{% endblock %}
```

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/tests/test_api.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/tests/test_app_metrics.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/tests/test_app_metrics.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/tests/test_basics.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/tests/test_graphql.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/tests/test_handler.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/tests/test_jobs.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/tests/test_models.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/tests/test_sources.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/tests/test_sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,16 +329,17 @@
     @parameterized.expand(
         [
             ["name_1", "url1", "user_1", "password_1", "imap_server", 993, False],
             ["name_1", "url1", None, "password_1", "imap_server", 993, True],
             ["name_1", "url1", "user_1", None, "imap_server", 993, True],
             ["name_1", "url1", "user_1", "password_1", None, 993, True],
             ["name_1", "url1", "user_1", "password_1", "imap_server", None, False],
-        ]  # pylint: disable=too-many-arguments
+        ]
     )
+    # pylint: disable-next=too-many-arguments
     def test_imap_init(self, name, url, account, password, imap_server, imap_port, exception):
         """Test IMAP class init."""
         kwargs = {}
         if name:
             kwargs["name"] = name
         if url:
             kwargs["url"] = url
@@ -545,16 +546,17 @@
         self.logger.log_warning.assert_not_called()
 
     @parameterized.expand(
         [
             ["name_1", "url1", "user_1", "credentials_file", False],
             ["name_1", "url1", None, "credentials_file", True],
             ["name_1", "url1", "user_1", None, True],
-        ]  # pylint: disable=too-many-arguments
+        ]
     )
+    # pylint: disable-next=too-many-arguments
     def test_gmail_api_service_account_init(self, name, url, account, credentials_file, exception):
         """Test Gmail API class init."""
         kwargs = {}
         if name:
             kwargs["name"] = name
         if url:
             kwargs["url"] = url
@@ -643,16 +645,17 @@
             [
                 datetime.datetime(2021, 9, 20, 17, 49, 50, 0),
                 "X-Original-Sender",
                 ["email1@example.com", "email2@example.com"],
                 ["mailinglist1@example.com", "mailinglist2@example.com"],
                 "after:2021/09/20 {from:mailinglist1@example.com from:mailinglist2@example.com}",
             ],
-        ]  # pylint: disable=too-many-arguments
+        ]
     )
+    # pylint: disable-next=too-many-arguments
     def test_get_search_criteria(
         self, since_timestamp, source_header, emails_to_fetch, limit_emails_with_not_header_from, result
     ):
         """Test the get_search_criteria method."""
         source = GmailAPI(
             name="whatever",
             url="https://accounts.google.com/o/oauth2/auth",
```

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/tests/test_views.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/tests/test_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,36 +35,43 @@
     def test_has_advanced_tab(self):
         pass
 
     @skip("Not implemented yet.")
     def test_get_object_notes(self):
         pass
 
+    @skip("Issue https://github.com/nautobot/nautobot/issues/3419")
+    def test_queryset_to_csv(self):
+        pass
+
     @classmethod
     def setUpTestData(cls):
         """Setup environment for testing."""
         CircuitMaintenance.objects.create(
-            name="UT-TEST-1", start_time="2020-10-04 10:00:00", end_time="2020-10-04 12:00:00"
+            name="UT-TEST-1", start_time="2020-10-04T10:00:00", end_time="2020-10-04 12:00:00"
         )
         CircuitMaintenance.objects.create(
-            name="UT-TEST-2", start_time="2020-10-05 10:00:00", end_time="2020-10-05 12:00:00"
+            name="UT-TEST-2", start_time="2020-10-05T10:00:00", end_time="2020-10-05 12:00:00"
+        )
+        CircuitMaintenance.objects.create(
+            name="UT-TEST-3", start_time="2020-10-06 10:00:00", end_time="2020-10-06 12:00:00"
         )
 
         cls.form_data = {
             "name": "UT-TEST-10",
             "start_time": "2020-10-06 10:00:00",
             "end_time": "2020-10-06 12:00:00",
             "description": "TEST 0 descr",
         }
 
         cls.csv_data = (
             "name,start_time,end_time,description",
-            "UT-TEST-20, 2020-10-06 10:00:00, 2020-10-06 12:00:00, TEST 20 descr",
-            "UT-TEST-21, 2020-10-06 10:00:00, 2020-10-06 12:00:00, TEST 21 descr",
-            "UT-TEST-22, 2020-10-06 10:00:00, 2020-10-06 12:00:00, TEST 22 descr",
+            "UT-TEST-20, 2020-10-06T10:00:00, 2020-10-06T12:00:00, TEST 20 descr",
+            "UT-TEST-21, 2020-10-06T10:00:00, 2020-10-06T12:00:00, TEST 21 descr",
+            "UT-TEST-22, 2020-10-06T10:00:00, 2020-10-06T12:00:00, TEST 22 descr",
         )
 
         cls.bulk_edit_data = {
             "status": "CANCELLED",
         }
 
 
@@ -181,31 +188,35 @@
     def test_list_objects_unknown_filter_strict_filtering(self):
         pass
 
     @skip("Not Implemented")
     def test_get_object_notes(self):
         pass
 
+    @skip("Issue https://github.com/nautobot/nautobot/issues/3419")
+    def test_queryset_to_csv(self):
+        pass
+
     @classmethod
     def setUpTestData(cls):
         """Setup environment for testing."""
 
         maintenance = CircuitMaintenance.objects.create(
             name="UT-TEST-1", start_time="2020-10-04 10:00:00", end_time="2020-10-04 12:00:00"
         )
 
         Note.objects.create(maintenance=maintenance, title="Note 1", comment="comment 1")
         Note.objects.create(maintenance=maintenance, title="Note 2", comment="comment 2")
 
         cls.form_data = {"maintenance": maintenance, "title": "Note 3", "level": "INFO", "comment": "comment 3"}
 
         cls.csv_data = (
-            "maintenance,title,comment",
-            f"{maintenance.pk}, Note 4, comment 4",
-            f"{maintenance.pk}, Note 5, comment 5",
+            "maintenance,title,level,comment",
+            f"{maintenance.pk}, Note 4, INFO, comment 4",
+            f"{maintenance.pk}, Note 5, INFO, comment 5",
         )
 
         cls.bulk_edit_data = {"level": "WARNING"}
 
     def test_list_objects_with_constrained_permission(self):
         """TODO: fix because it's checking the get_absolute_url() in a wrong page."""
```

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/urls.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/nautobot_circuit_maintenance/views.py` & `nautobot_circuit_maintenance-1.0.0/nautobot_circuit_maintenance/views.py`

 * *Files identical despite different names*

### Comparing `nautobot_circuit_maintenance-0.6.2/pyproject.toml` & `nautobot_circuit_maintenance-1.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-circuit-maintenance"
-version = "v0.6.2"
+version = "v1.0.0"
 description = "Nautobot plugin to automatically handle Circuit Maintenances Notifications"
 authors = ["Network to Code, LLC <opensource@networktocode.com>"]
 
 license = "Apache-2.0"
 
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-plugin-circuit-maintenance"
@@ -21,37 +21,48 @@
 [[tool.poetry.source]]
 name = "pypi-legacy"
 url = "https://pypi.org/simple/"
 secondary = true
 
 [tool.poetry.dependencies]
 python = "^3.7"
-nautobot = "*"
+nautobot = "^1.4.0"
 nautobot-capacity-metrics = {version = "*", optional = true }
 bs4 = "^0.0.1"
 circuit-maintenance-parser = "^2.0.0"
 google-api-python-client = "^2.9.0"
 google-oauth = { version = "^1.0.0", source = "pypi-legacy" }
 google-auth-httplib2 = "^0.1.0"
 google-auth-oauthlib = "^0.5.0"
 # Added due an issue with Markdown 3.3.5
 markdown = "!=3.3.5"
 
 [tool.poetry.dev-dependencies]
 invoke = "*"
-black = "*"
+# Black 23.x.x configuration changes and migration files are taken into account
+black = "^22.6.0"
 django-debug-toolbar = "*"
 yamllint = "*"
 bandit = "*"
 pylint = "*"
 pylint-django = "*"
 pydocstyle = "*"
 flake8 = "*"
 parameterized = "*"
 mysqlclient = "*"
+# Rendering docs to HTML
+mkdocs = "1.3.1"
+# Material for MkDocs theme
+mkdocs-material = "8.4.2"
+# Render custom markdown for version added/changed/remove notes
+mkdocs-version-annotations = "1.0.0"
+# Automatic documentation from sources, for MkDocs
+mkdocstrings = "0.19"
+mkdocstrings-python = "0.7.1"
+towncrier = "^22.12.0"
 
 
 [tool.poetry.extras]
 metrics = ["nautobot-capacity-metrics"]
 
 [tool.black]
 line-length = 120
@@ -79,32 +90,36 @@
 [tool.pylint.master]
 # Include the pylint_django plugin to avoid spurious warnings about Django patterns
 load-plugins="pylint_django"
 
 # Don't cache data for later comparisons
 persistent="no"
 
+# Ignore migrations and tests
+ignore = ".*/tests/*,.*/migrations/*"
+
 # Don't raise alarms if args/kwargs has an issue, as may be required, just as a decorator
 ignored-argument-names="args|kwargs"
 
 [tool.pylint.basic]
 # No docstrings required for private methods (Pylint default), or for test_ functions, or for inner Meta classes.
 no-docstring-rgx="^(_|test_|Meta$)"
 
 [tool.pylint.messages_control]
 # Line length is enforced by Black, so pylint doesn't need to check it.
 # Pylint and Black disagree about how to format multi-line arrays; Black wins.
 disable = """,
     line-too-long,
-    bad-continuation,
     too-few-public-methods,
     duplicate-code,
     too-many-ancestors,
+    useless-option-value,
     """
 
+
 [tool.pylint.miscellaneous]
 # Don't flag TODO as a failure, let us commit with things that still need to be done in the code
 notes = """,
     FIXME,
     XXX,
     """
 
@@ -113,7 +128,22 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests"
 ]
 adopts = "-vv"
+
+[tool.towncrier]
+package = "nautobot_circuit_maintenance"
+directory = "changes"
+filename = "docs/admin/release_notes/version_1.0.md"
+template = "development/towncrier_template.j2"
+start_string = "<!-- towncrier release notes start -->"
+issue_format = "[#{issue}](https://github.com/nautobot/nautobot-plugin-circuit-maintenance/issues/{issue})"
+
+[tool.towncrier.fragment.added]
+[tool.towncrier.fragment.changed]
+[tool.towncrier.fragment.deprecated]
+[tool.towncrier.fragment.fixed]
+[tool.towncrier.fragment.removed]
+[tool.towncrier.fragment.security]
```

