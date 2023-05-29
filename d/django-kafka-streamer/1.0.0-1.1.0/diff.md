# Comparing `tmp/django-kafka-streamer-1.0.0.tar.gz` & `tmp/django-kafka-streamer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-kafka-streamer-1.0.0.tar", last modified: Sat Jan 14 18:59:20 2023, max compression
+gzip compressed data, was "django-kafka-streamer-1.1.0.tar", last modified: Mon May 29 13:57:53 2023, max compression
```

## Comparing `django-kafka-streamer-1.0.0.tar` & `django-kafka-streamer-1.1.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-01-14 18:59:20.400300 django-kafka-streamer-1.0.0/
-drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-01-14 18:59:20.384300 django-kafka-streamer-1.0.0/.github/
-drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-01-14 18:59:20.388300 django-kafka-streamer-1.0.0/.github/workflows/
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1176 2023-01-13 17:59:53.000000 django-kafka-streamer-1.0.0/.github/workflows/tests.yml
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      212 2023-01-12 08:21:00.000000 django-kafka-streamer-1.0.0/.gitignore
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1348 2023-01-14 13:54:08.000000 django-kafka-streamer-1.0.0/LICENSE
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1445 2023-01-14 18:59:20.400300 django-kafka-streamer-1.0.0/PKG-INFO
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      310 2023-01-13 19:09:43.000000 django-kafka-streamer-1.0.0/README.rst
-drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-01-14 18:59:20.388300 django-kafka-streamer-1.0.0/django_kafka_streamer.egg-info/
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1445 2023-01-14 18:59:20.000000 django-kafka-streamer-1.0.0/django_kafka_streamer.egg-info/PKG-INFO
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1156 2023-01-14 18:59:20.000000 django-kafka-streamer-1.0.0/django_kafka_streamer.egg-info/SOURCES.txt
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)        1 2023-01-14 18:59:20.000000 django-kafka-streamer-1.0.0/django_kafka_streamer.egg-info/dependency_links.txt
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)       90 2023-01-14 18:59:20.000000 django-kafka-streamer-1.0.0/django_kafka_streamer.egg-info/requires.txt
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)       20 2023-01-14 18:59:20.000000 django-kafka-streamer-1.0.0/django_kafka_streamer.egg-info/top_level.txt
-drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-01-14 18:59:20.392300 django-kafka-streamer-1.0.0/kafkastreamer/
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      218 2023-01-14 18:55:31.000000 django-kafka-streamer-1.0.0/kafkastreamer/__init__.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      226 2023-01-12 15:04:45.000000 django-kafka-streamer-1.0.0/kafkastreamer/apps.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      337 2023-01-12 15:04:45.000000 django-kafka-streamer-1.0.0/kafkastreamer/constants.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     2079 2023-01-13 11:36:25.000000 django-kafka-streamer-1.0.0/kafkastreamer/context.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      864 2023-01-13 17:30:19.000000 django-kafka-streamer-1.0.0/kafkastreamer/decorators.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     3908 2023-01-13 11:37:52.000000 django-kafka-streamer-1.0.0/kafkastreamer/handlers.py
-drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-01-14 18:59:20.392300 django-kafka-streamer-1.0.0/kafkastreamer/management/
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)        0 2023-01-11 14:08:36.000000 django-kafka-streamer-1.0.0/kafkastreamer/management/__init__.py
-drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-01-14 18:59:20.392300 django-kafka-streamer-1.0.0/kafkastreamer/management/commands/
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)        0 2023-01-11 14:08:36.000000 django-kafka-streamer-1.0.0/kafkastreamer/management/commands/__init__.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1623 2023-01-12 15:06:59.000000 django-kafka-streamer-1.0.0/kafkastreamer/management/commands/kafkastreamer_refresh.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     4026 2023-01-13 15:57:21.000000 django-kafka-streamer-1.0.0/kafkastreamer/registry.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1026 2023-01-14 14:56:22.000000 django-kafka-streamer-1.0.0/kafkastreamer/serializers.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      310 2023-01-14 15:43:24.000000 django-kafka-streamer-1.0.0/kafkastreamer/settings.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)    20887 2023-01-14 15:50:29.000000 django-kafka-streamer-1.0.0/kafkastreamer/stream.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1130 2023-01-13 16:27:46.000000 django-kafka-streamer-1.0.0/kafkastreamer/tasks.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      110 2023-01-11 14:51:15.000000 django-kafka-streamer-1.0.0/pyproject.toml
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)       38 2023-01-14 15:13:50.000000 django-kafka-streamer-1.0.0/pytest.ini
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1418 2023-01-14 18:59:20.400300 django-kafka-streamer-1.0.0/setup.cfg
-drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-01-14 18:59:20.396300 django-kafka-streamer-1.0.0/tests/
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)        0 2023-01-11 14:58:50.000000 django-kafka-streamer-1.0.0/tests/__init__.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      461 2023-01-14 15:43:49.000000 django-kafka-streamer-1.0.0/tests/conftest.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      753 2023-01-13 17:30:19.000000 django-kafka-streamer-1.0.0/tests/test_admin_site.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1321 2023-01-13 16:45:24.000000 django-kafka-streamer-1.0.0/tests/test_command_refresh.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     2146 2023-01-14 15:49:18.000000 django-kafka-streamer-1.0.0/tests/test_context.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1025 2023-01-14 15:50:59.000000 django-kafka-streamer-1.0.0/tests/test_real_kafka.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     2363 2023-01-13 16:46:56.000000 django-kafka-streamer-1.0.0/tests/test_registry.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1770 2023-01-14 15:06:48.000000 django-kafka-streamer-1.0.0/tests/test_serializers.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     3205 2023-01-14 15:07:57.000000 django-kafka-streamer-1.0.0/tests/test_stream_from_signals.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     3746 2023-01-14 15:09:04.000000 django-kafka-streamer-1.0.0/tests/test_stream_manual.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)    12612 2023-01-14 15:10:15.000000 django-kafka-streamer-1.0.0/tests/test_streamer.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1250 2023-01-13 16:47:57.000000 django-kafka-streamer-1.0.0/tests/test_tasks.py
-drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-01-14 18:59:20.400300 django-kafka-streamer-1.0.0/tests/testapp/
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)        0 2023-01-12 09:37:20.000000 django-kafka-streamer-1.0.0/tests/testapp/__init__.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      281 2023-01-13 16:59:01.000000 django-kafka-streamer-1.0.0/tests/testapp/admin.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      379 2023-01-12 15:50:11.000000 django-kafka-streamer-1.0.0/tests/testapp/models.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      588 2023-01-13 16:44:58.000000 django-kafka-streamer-1.0.0/tests/testapp/streamers.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      303 2023-01-12 15:07:04.000000 django-kafka-streamer-1.0.0/tests/utils.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      735 2023-01-14 14:22:12.000000 django-kafka-streamer-1.0.0/tox.ini
+drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-05-29 13:57:53.229700 django-kafka-streamer-1.1.0/
+drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-05-29 13:57:53.209700 django-kafka-streamer-1.1.0/.github/
+drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-05-29 13:57:53.217700 django-kafka-streamer-1.1.0/.github/workflows/
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1176 2023-01-13 17:59:53.000000 django-kafka-streamer-1.1.0/.github/workflows/tests.yml
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      212 2023-01-12 08:21:00.000000 django-kafka-streamer-1.1.0/.gitignore
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1348 2023-05-29 13:56:37.000000 django-kafka-streamer-1.1.0/LICENSE
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     2149 2023-05-29 13:57:53.233700 django-kafka-streamer-1.1.0/PKG-INFO
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1014 2023-05-29 13:56:37.000000 django-kafka-streamer-1.1.0/README.rst
+drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-05-29 13:57:53.225700 django-kafka-streamer-1.1.0/django_kafka_streamer.egg-info/
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     2149 2023-05-29 13:57:53.000000 django-kafka-streamer-1.1.0/django_kafka_streamer.egg-info/PKG-INFO
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1156 2023-05-29 13:57:53.000000 django-kafka-streamer-1.1.0/django_kafka_streamer.egg-info/SOURCES.txt
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)        1 2023-05-29 13:57:53.000000 django-kafka-streamer-1.1.0/django_kafka_streamer.egg-info/dependency_links.txt
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)       90 2023-05-29 13:57:53.000000 django-kafka-streamer-1.1.0/django_kafka_streamer.egg-info/requires.txt
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)       20 2023-05-29 13:57:53.000000 django-kafka-streamer-1.1.0/django_kafka_streamer.egg-info/top_level.txt
+drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-05-29 13:57:53.225700 django-kafka-streamer-1.1.0/kafkastreamer/
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      218 2023-05-29 13:56:41.000000 django-kafka-streamer-1.1.0/kafkastreamer/__init__.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      226 2023-01-12 15:04:45.000000 django-kafka-streamer-1.1.0/kafkastreamer/apps.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      337 2023-01-12 15:04:45.000000 django-kafka-streamer-1.1.0/kafkastreamer/constants.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     2076 2023-05-29 13:56:41.000000 django-kafka-streamer-1.1.0/kafkastreamer/context.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      864 2023-01-13 17:30:19.000000 django-kafka-streamer-1.1.0/kafkastreamer/decorators.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     3905 2023-05-29 13:56:41.000000 django-kafka-streamer-1.1.0/kafkastreamer/handlers.py
+drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-05-29 13:57:53.229700 django-kafka-streamer-1.1.0/kafkastreamer/management/
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)        0 2023-01-11 14:08:36.000000 django-kafka-streamer-1.1.0/kafkastreamer/management/__init__.py
+drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-05-29 13:57:53.229700 django-kafka-streamer-1.1.0/kafkastreamer/management/commands/
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)        0 2023-01-11 14:08:36.000000 django-kafka-streamer-1.1.0/kafkastreamer/management/commands/__init__.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1623 2023-01-12 15:06:59.000000 django-kafka-streamer-1.1.0/kafkastreamer/management/commands/kafkastreamer_refresh.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     4514 2023-05-29 13:56:41.000000 django-kafka-streamer-1.1.0/kafkastreamer/registry.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1042 2023-05-29 13:56:41.000000 django-kafka-streamer-1.1.0/kafkastreamer/serializers.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      673 2023-05-29 13:56:41.000000 django-kafka-streamer-1.1.0/kafkastreamer/settings.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)    21111 2023-05-29 13:56:41.000000 django-kafka-streamer-1.1.0/kafkastreamer/stream.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1130 2023-01-13 16:27:46.000000 django-kafka-streamer-1.1.0/kafkastreamer/tasks.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      110 2023-01-11 14:51:15.000000 django-kafka-streamer-1.1.0/pyproject.toml
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      102 2023-05-29 13:56:41.000000 django-kafka-streamer-1.1.0/pytest.ini
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1418 2023-05-29 13:57:53.233700 django-kafka-streamer-1.1.0/setup.cfg
+drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-05-29 13:57:53.229700 django-kafka-streamer-1.1.0/tests/
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)        0 2023-01-11 14:58:50.000000 django-kafka-streamer-1.1.0/tests/__init__.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      498 2023-05-29 13:56:41.000000 django-kafka-streamer-1.1.0/tests/conftest.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      753 2023-01-13 17:30:19.000000 django-kafka-streamer-1.1.0/tests/test_admin_site.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1321 2023-01-13 16:45:24.000000 django-kafka-streamer-1.1.0/tests/test_command_refresh.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     2146 2023-05-29 13:56:37.000000 django-kafka-streamer-1.1.0/tests/test_context.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1025 2023-05-29 13:56:37.000000 django-kafka-streamer-1.1.0/tests/test_real_kafka.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     2363 2023-01-13 16:46:56.000000 django-kafka-streamer-1.1.0/tests/test_registry.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1770 2023-05-29 13:56:37.000000 django-kafka-streamer-1.1.0/tests/test_serializers.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     3205 2023-05-29 13:56:37.000000 django-kafka-streamer-1.1.0/tests/test_stream_from_signals.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     3746 2023-05-29 13:56:37.000000 django-kafka-streamer-1.1.0/tests/test_stream_manual.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)    12612 2023-05-29 13:56:37.000000 django-kafka-streamer-1.1.0/tests/test_streamer.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1250 2023-01-13 16:47:57.000000 django-kafka-streamer-1.1.0/tests/test_tasks.py
+drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-05-29 13:57:53.229700 django-kafka-streamer-1.1.0/tests/testapp/
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)        0 2023-01-12 09:37:20.000000 django-kafka-streamer-1.1.0/tests/testapp/__init__.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      281 2023-01-13 16:59:01.000000 django-kafka-streamer-1.1.0/tests/testapp/admin.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      379 2023-01-12 15:50:11.000000 django-kafka-streamer-1.1.0/tests/testapp/models.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      592 2023-05-29 13:56:41.000000 django-kafka-streamer-1.1.0/tests/testapp/streamers.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      303 2023-01-12 15:07:04.000000 django-kafka-streamer-1.1.0/tests/utils.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      795 2023-05-29 13:56:41.000000 django-kafka-streamer-1.1.0/tox.ini
```

### Comparing `django-kafka-streamer-1.0.0/.github/workflows/tests.yml` & `django-kafka-streamer-1.1.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.0.0/LICENSE` & `django-kafka-streamer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.0.0/django_kafka_streamer.egg-info/SOURCES.txt` & `django-kafka-streamer-1.1.0/django_kafka_streamer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.0.0/kafkastreamer/context.py` & `django-kafka-streamer-1.1.0/kafkastreamer/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,15 @@
         _context.squash = {}
 
     try:
         yield
 
     finally:
         if is_top:
-
-            for (model, messages_d) in _context.squash.items():
+            for model, messages_d in _context.squash.items():
                 streamer = get_streamer(model)
                 messages = messages_d.values()
                 streamer.send_messages(messages)
 
             _context.squash = None
```

### Comparing `django-kafka-streamer-1.0.0/kafkastreamer/decorators.py` & `django-kafka-streamer-1.1.0/kafkastreamer/decorators.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.0.0/kafkastreamer/handlers.py` & `django-kafka-streamer-1.1.0/kafkastreamer/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from .constants import TYPE_CREATE, TYPE_DELETE, TYPE_UPDATE
 from .context import _add_to_squash, _context
 from .registry import get_streamer, get_streamer_for_related
 
 
 def handle_post_save(sender, instance=None, **kwargs):
-
     stop_handlers = getattr(_context, "stop_handlers", None)
     if stop_handlers is not None:
         if not stop_handlers or sender in stop_handlers:
             return
 
     squash = getattr(_context, "squash", None)
     created = kwargs.get("created", False)
@@ -28,15 +27,14 @@
         )
         if squash is not None:
             _add_to_squash(squash, sender, streamer, messages)
         else:
             streamer.send_messages(messages)
 
     for rel_name, streamer in get_streamer_for_related(sender):
-
         try:
             rel = getattr(instance, rel_name)
         except ObjectDoesNotExist:
             continue
 
         messages = None
         if isinstance(rel, models.Model):
@@ -112,10 +110,9 @@
             if squash is not None:
                 _add_to_squash(squash, model, streamer, messages)
             else:
                 streamer.send_messages(messages)
 
 
 def handle_m2m_changed(sender, instance=None, action=None, **kwargs):
-
     if action.startswith("post_"):
         handle_post_save(instance.__class__, instance=instance, **kwargs)
```

### Comparing `django-kafka-streamer-1.0.0/kafkastreamer/management/commands/kafkastreamer_refresh.py` & `django-kafka-streamer-1.1.0/kafkastreamer/management/commands/kafkastreamer_refresh.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.0.0/kafkastreamer/registry.py` & `django-kafka-streamer-1.1.0/kafkastreamer/registry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import collections
 from importlib import import_module
 
 from django.apps import apps
+from django.core.exceptions import ImproperlyConfigured
 from django.db import models
 from django.db.models.fields.related_descriptors import (
     ForwardManyToOneDescriptor,
     ForwardOneToOneDescriptor,
     ManyToManyDescriptor,
     ReverseManyToOneDescriptor,
     ReverseOneToOneDescriptor,
@@ -22,25 +23,34 @@
     return RegistryKey(
         model._meta.app_label,
         model._meta.object_name,
         rel_name,
     )
 
 
-def register(model, streamer_class, set_handlers=True, **kwargs):
+def register(model, streamer_class=None, set_handlers=True, **kwargs):
     """
-    Registers Django model using given streamer class
+    Registers Django model using given streamer class. May be used as plain
+    function call or as decorator on streamer class.
     """
     from .handlers import (
         handle_m2m_changed,
         handle_post_delete,
         handle_post_save,
         handle_pre_delete,
     )
 
+    def wrapper(cls):
+        register(model, cls)
+        return cls
+
+    if streamer_class is None:
+        # Called as class decorator
+        return wrapper
+
     streamer = streamer_class(**kwargs)
     _registry[_make_registry_key(model)] = streamer
 
     if set_handlers:
         post_save.connect(handle_post_save, sender=model)
         pre_delete.connect(handle_pre_delete, sender=model)
         post_delete.connect(handle_post_delete, sender=model)
@@ -74,14 +84,18 @@
         elif isinstance(rel_desc, ReverseOneToOneDescriptor):
             rel_model_and_attr.append(
                 (rel_desc.related.related_model, rel_desc.related.field.name, True)
             )
 
         for rel_model, rev_name, set_delete_handler in rel_model_and_attr:
             if rev_name:
+                if rev_name == "+":
+                    raise ImproperlyConfigured(
+                        f"No backward reference field from {rel_model} to {model}."
+                    )
                 _registry[_make_registry_key(rel_model, rev_name)] = streamer
 
                 if set_handlers:
                     post_save.connect(handle_post_save, sender=rel_model)
                     if set_delete_handler:
                         post_delete.connect(handle_post_delete, sender=rel_model)
             else:
```

### Comparing `django-kafka-streamer-1.0.0/kafkastreamer/serializers.py` & `django-kafka-streamer-1.1.0/kafkastreamer/serializers.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,14 +29,18 @@
         "_type": meta.msg_type,
         **context_fields,
         **msg.data,
     }
     if ensure_id and item.get("id") is None:
         item["id"] = msg.obj_id
 
-    return json.dumps(item, cls=DjangoJSONEncoder, ensure_ascii=ensure_ascii,).encode(
+    return json.dumps(
+        item,
+        cls=cls,
+        ensure_ascii=ensure_ascii,
+    ).encode(
         encoding,
     )
 
 
 def object_id_key_serializer(obj_id, encoding=DEFAULT_ENCODING):
     return bytes(str(obj_id or 0), encoding)
```

### Comparing `django-kafka-streamer-1.0.0/kafkastreamer/stream.py` & `django-kafka-streamer-1.1.0/kafkastreamer/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     TYPE_ENUMERATE,
     TYPE_EOS,
     TYPE_REFRESH,
     TYPE_UPDATE,
 )
 from .context import _add_to_squash, _context
 from .registry import get_registry, get_streamer
-from .serializers import flat_json_message_serializer, object_id_key_serializer
 from .settings import get_setting
 
 log = logging.getLogger(__name__)
 
 
 MessageContext = namedtuple(
     "MessageContext",
@@ -64,24 +63,22 @@
         queryset=None,
         manager=None,
         objects_ids=None,
         select_related=None,
         prefetch_related=None,
         **kwargs
     ):
-
         self.objects = objects
         self.queryset = queryset
         self.manager = manager
         self.objects_ids = objects_ids
         self.select_related = select_related
         self.prefetch_related = prefetch_related
 
     def get_objects(self):
-
         queryset = self.queryset
         if queryset is None and self.manager is not None:
             queryset = self.manager.all()
 
         if queryset is not None and self.objects_ids is not None:
             queryset = queryset.filter(pk__in=self.objects_ids).order_by()
             if self.select_related:
@@ -121,17 +118,21 @@
         for key, value in kwargs.items():
             if value is not None:
                 setattr(self, key, value)
         if not self.topic:
             raise ImproperlyConfigured("No streamer topic specified")
         self.batch_size = self.batch_size or get_setting("BATCH_SIZE")
         if self.message_serializer is None:
-            self.message_serializer = flat_json_message_serializer
+            self.message_serializer = get_setting(
+                "DEFAULT_MESSAGE_SERIALIZER", resolve=True
+            )
         if self.partition_key_serializer is None:
-            self.partition_key_serializer = object_id_key_serializer
+            self.partition_key_serializer = get_setting(
+                "DEFAULT_PARTITION_KEY_SERIALIZER", resolve=True
+            )
 
     def get_data_for_object(self, obj, batch):
         """
         Returns data fields for given object
         """
 
         def get_concrete_fields(obj, batch, related_name=None, exclude=None):
@@ -164,15 +165,14 @@
 
             return data
 
         data = get_concrete_fields(obj, batch, exclude=self.exclude)
 
         if self.include:
             for name in self.include:
-
                 method_name = "load_%s" % name
                 func = getattr(self, method_name, None)
                 try:
                     if func is not None:
                         value = func(obj, batch)
                     else:
                         value = getattr(obj, name)
@@ -426,15 +426,19 @@
             "value_serializer": self.message_serializer,
             "key_serializer": self.partition_key_serializer,
             "bootstrap_servers": get_setting("BOOTSTRAP_SERVERS"),
             **self.get_producer_options(),
             **kwargs,
         }
 
-        if not options.get("bootstrap_servers"):
+        if options.get("bootstrap_servers") is None:
+            raise ImproperlyConfigured(
+                "The `KAFKA_STREAMER['BOOTSTRAP_SERVERS']` is not configured."
+            )
+        if options["bootstrap_servers"] == []:
             return None
 
         try:
             producer = kafka.KafkaProducer(**options)
         except NoBrokersAvailable as e:
             log.error("Kafka connect error: %s", e)
             return None
@@ -646,15 +650,14 @@
 def full_refresh(model_or_manager=None, producer=None, flush=True):
     """
     Does full refresh for model or manager. Sends refresh message for each
     object, then sends enumerate message with objects IDs
     """
 
     def _refresh(streamer, manager, producer, flush, timestamp=None):
-
         if timestamp is None:
             timestamp = timezone.now()
 
         queryset = manager.all()
         objects_ids = list(queryset.order_by().values_list("pk", flat=True))
 
         count = streamer.send_objects(
```

### Comparing `django-kafka-streamer-1.0.0/kafkastreamer/tasks.py` & `django-kafka-streamer-1.1.0/kafkastreamer/tasks.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.0.0/setup.cfg` & `django-kafka-streamer-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.0.0/tests/test_admin_site.py` & `django-kafka-streamer-1.1.0/tests/test_admin_site.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.0.0/tests/test_command_refresh.py` & `django-kafka-streamer-1.1.0/tests/test_command_refresh.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.0.0/tests/test_context.py` & `django-kafka-streamer-1.1.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.0.0/tests/test_real_kafka.py` & `django-kafka-streamer-1.1.0/tests/test_real_kafka.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.0.0/tests/test_registry.py` & `django-kafka-streamer-1.1.0/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.0.0/tests/test_serializers.py` & `django-kafka-streamer-1.1.0/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.0.0/tests/test_stream_from_signals.py` & `django-kafka-streamer-1.1.0/tests/test_stream_from_signals.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.0.0/tests/test_stream_manual.py` & `django-kafka-streamer-1.1.0/tests/test_stream_manual.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.0.0/tests/test_streamer.py` & `django-kafka-streamer-1.1.0/tests/test_streamer.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.0.0/tests/test_tasks.py` & `django-kafka-streamer-1.1.0/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.0.0/tests/testapp/streamers.py` & `django-kafka-streamer-1.1.0/tests/testapp/streamers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 from kafkastreamer import Streamer, register
 from tests.testapp.models import ModelA, ModelB, ModelC
 
 
+@register(ModelA)
 class ModelAStreamer(Streamer):
     topic = "model-a"
 
 
-register(ModelA, ModelAStreamer)
-
-
+@register(ModelB)
 class ModelBStreamer(Streamer):
     topic = "model-b"
     include = ["z"]
 
     def load_z(self, obj, batch):
         return obj.x + obj.y
 
     def get_extra_data(self, obj, batch):
         return {"e": "extra"}
 
 
-register(ModelB, ModelBStreamer)
-
-
 class ModelCStreamer(Streamer):
     topic = "model-c"
     include = ["a", "b"]
     select_related = ["a", "b"]
 
 
+# use register as plain function call
 register(ModelC, ModelCStreamer)
```

