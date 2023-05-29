# Comparing `tmp/django_toolshed-0.5.8.tar.gz` & `tmp/django_toolshed-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_toolshed-0.5.8.tar", max compression
+gzip compressed data, was "django_toolshed-0.5.9.tar", max compression
```

## Comparing `django_toolshed-0.5.8.tar` & `django_toolshed-0.5.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-05-26 16:33:22.599223 django_toolshed-0.5.8/LICENSE
--rw-r--r--   0        0        0       22 2023-05-26 16:33:22.599223 django_toolshed-0.5.8/django_toolshed/__init__.py
--rw-r--r--   0        0        0      292 2023-05-26 16:33:22.599223 django_toolshed-0.5.8/django_toolshed/apps.py
--rwxr-xr-x   0        0        0     1381 2023-05-26 16:33:22.599223 django_toolshed-0.5.8/django_toolshed/celery_auto_app.py
--rw-r--r--   0        0        0      254 2023-05-26 16:33:22.599223 django_toolshed-0.5.8/django_toolshed/celery_urls.py
--rw-r--r--   0        0        0     3260 2023-05-28 13:32:11.311872 django_toolshed-0.5.8/django_toolshed/celery_views.py
--rw-r--r--   0        0        0      969 2023-05-26 16:33:22.599223 django_toolshed-0.5.8/django_toolshed/management/commands/create_management_command.py
--rw-r--r--   0        0        0      264 2023-05-26 16:33:22.599223 django_toolshed-0.5.8/django_toolshed/management/commands/list_apps.py
--rw-r--r--   0        0        0      637 2023-05-26 16:33:22.599223 django_toolshed-0.5.8/django_toolshed/management/commands/list_commands.py
--rw-r--r--   0        0        0      321 2023-05-26 16:33:22.599223 django_toolshed-0.5.8/django_toolshed/management/commands/list_users.py
--rw-r--r--   0        0        0     1797 2023-05-28 11:56:50.471025 django_toolshed-0.5.8/django_toolshed/mixins.py
--rw-r--r--   0        0        0       37 2023-05-26 16:33:22.599223 django_toolshed-0.5.8/django_toolshed/signals.py
--rw-r--r--   0        0        0        0 2023-05-26 16:33:22.599223 django_toolshed-0.5.8/django_toolshed/static/django_toolshed/css/.gitkeep
--rw-r--r--   0        0        0        0 2023-05-26 16:33:22.599223 django_toolshed-0.5.8/django_toolshed/static/django_toolshed/images/.gitkeep
--rw-r--r--   0        0        0        0 2023-05-26 16:33:22.599223 django_toolshed-0.5.8/django_toolshed/static/django_toolshed/js/.gitkeep
--rw-r--r--   0        0        0        0 2023-05-26 16:33:22.599223 django_toolshed-0.5.8/django_toolshed/templates/django_toolshed/.gitkeep
--rw-r--r--   0        0        0       47 2023-05-26 16:33:22.599223 django_toolshed-0.5.8/django_toolshed/urls.py
--rw-r--r--   0        0        0     1106 2023-05-28 13:32:19.240005 django_toolshed-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 django_toolshed-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-26 16:33:22.599223 django_toolshed-0.5.9/LICENSE
+-rw-r--r--   0        0        0       22 2023-05-26 16:33:22.599223 django_toolshed-0.5.9/django_toolshed/__init__.py
+-rw-r--r--   0        0        0      292 2023-05-26 16:33:22.599223 django_toolshed-0.5.9/django_toolshed/apps.py
+-rwxr-xr-x   0        0        0     1381 2023-05-26 16:33:22.599223 django_toolshed-0.5.9/django_toolshed/celery_auto_app.py
+-rw-r--r--   0        0        0      254 2023-05-26 16:33:22.599223 django_toolshed-0.5.9/django_toolshed/celery_urls.py
+-rw-r--r--   0        0        0     3233 2023-05-29 10:42:50.924435 django_toolshed-0.5.9/django_toolshed/celery_views.py
+-rw-r--r--   0        0        0      969 2023-05-26 16:33:22.599223 django_toolshed-0.5.9/django_toolshed/management/commands/create_management_command.py
+-rw-r--r--   0        0        0      264 2023-05-26 16:33:22.599223 django_toolshed-0.5.9/django_toolshed/management/commands/list_apps.py
+-rw-r--r--   0        0        0      637 2023-05-26 16:33:22.599223 django_toolshed-0.5.9/django_toolshed/management/commands/list_commands.py
+-rw-r--r--   0        0        0      321 2023-05-26 16:33:22.599223 django_toolshed-0.5.9/django_toolshed/management/commands/list_users.py
+-rw-r--r--   0        0        0     1797 2023-05-28 11:56:50.471025 django_toolshed-0.5.9/django_toolshed/mixins.py
+-rw-r--r--   0        0        0       37 2023-05-26 16:33:22.599223 django_toolshed-0.5.9/django_toolshed/signals.py
+-rw-r--r--   0        0        0        0 2023-05-26 16:33:22.599223 django_toolshed-0.5.9/django_toolshed/static/django_toolshed/css/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-26 16:33:22.599223 django_toolshed-0.5.9/django_toolshed/static/django_toolshed/images/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-26 16:33:22.599223 django_toolshed-0.5.9/django_toolshed/static/django_toolshed/js/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-26 16:33:22.599223 django_toolshed-0.5.9/django_toolshed/templates/django_toolshed/.gitkeep
+-rw-r--r--   0        0        0       47 2023-05-26 16:33:22.599223 django_toolshed-0.5.9/django_toolshed/urls.py
+-rw-r--r--   0        0        0     1106 2023-05-29 10:43:09.095715 django_toolshed-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 django_toolshed-0.5.9/PKG-INFO
```

### Comparing `django_toolshed-0.5.8/LICENSE` & `django_toolshed-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django_toolshed-0.5.8/django_toolshed/celery_auto_app.py` & `django_toolshed-0.5.9/django_toolshed/celery_auto_app.py`

 * *Files identical despite different names*

### Comparing `django_toolshed-0.5.8/django_toolshed/celery_views.py` & `django_toolshed-0.5.9/django_toolshed/celery_views.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,27 +8,26 @@
 from drf_spectacular.utils import OpenApiParameter, extend_schema
 from rest_framework import serializers
 from rest_framework.decorators import action
 from rest_framework.exceptions import NotFound, ParseError
 from rest_framework.response import Response
 from rest_framework.viewsets import ViewSet
 
-# Avoid re-generating API docs and API clients
-celery_states = [(v, v) for v in sorted(ALL_STATES)]
-
 
 class CreateTaskSerializer(serializers.Serializer):
     task_name = serializers.CharField()
     args = serializers.ListField(required=False)
     kwargs = serializers.DictField(required=False)
 
 
 class ReadTaskSerializer(serializers.Serializer):
     task_id = serializers.CharField()
-    status = serializers.ChoiceField(choices=celery_states)
+    status = serializers.ChoiceField(
+        choices=[(v.lower(), v.capitalize()) for v in sorted(ALL_STATES)]
+    )
 
 
 class CeleryTaskViewSet(ViewSet):
     serializer_class = None
 
     @extend_schema(
         operation_id="read_task_status",
@@ -40,15 +39,15 @@
         responses={200: ReadTaskSerializer},
     )
     def retrieve(self, request, pk=None, **kwargs):
         async_result = AsyncResult(pk)
         serializer = ReadTaskSerializer(
             data=dict(
                 task_id=async_result.task_id,
-                status=async_result.status,
+                status=async_result.status.lower(),
             )
         )
         serializer.is_valid(raise_exception=True)
         return Response(serializer.data)
 
     @extend_schema(
         operation_id="create_task",
@@ -69,15 +68,15 @@
             args=serializer.data.get("args"),
             kwargs=serializer.data.get("kwargs"),
         )
         logging.info(f"Triggered celery {task_name=} via HTTP request")
         serializer = ReadTaskSerializer(
             data=dict(
                 task_id=async_result.task_id,
-                status=async_result.status,
+                status=async_result.status.lower(),
             )
         )
         serializer.is_valid(raise_exception=True)
         return Response(serializer.data, status=201)
 
     @action(detail=False, methods=["GET"])
     def types(self, request):
```

### Comparing `django_toolshed-0.5.8/django_toolshed/management/commands/create_management_command.py` & `django_toolshed-0.5.9/django_toolshed/management/commands/create_management_command.py`

 * *Files identical despite different names*

### Comparing `django_toolshed-0.5.8/django_toolshed/management/commands/list_commands.py` & `django_toolshed-0.5.9/django_toolshed/management/commands/list_commands.py`

 * *Files identical despite different names*

### Comparing `django_toolshed-0.5.8/django_toolshed/mixins.py` & `django_toolshed-0.5.9/django_toolshed/mixins.py`

 * *Files identical despite different names*

### Comparing `django_toolshed-0.5.8/pyproject.toml` & `django_toolshed-0.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-toolshed"
-version = "0.5.8"
+version = "0.5.9"
 description = ""
 authors = ["Dani Hodovic <you@example.com>"]
 license = "MIT"
 
 [tool.poetry.scripts]
 celery-auto-app = "django_toolshed.celery_auto_app:command"
```

### Comparing `django_toolshed-0.5.8/PKG-INFO` & `django_toolshed-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-toolshed
-Version: 0.5.8
+Version: 0.5.9
 Summary: 
 License: MIT
 Author: Dani Hodovic
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

