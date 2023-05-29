# Comparing `tmp/th2_common_utils-2.0.0.dev4574477823.tar.gz` & `tmp/th2_common_utils-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "th2_common_utils-2.0.0.dev4574477823.tar", max compression
+gzip compressed data, was "th2_common_utils-2.0.1.tar", max compression
```

## Comparing `th2_common_utils-2.0.0.dev4574477823.tar` & `th2_common_utils-2.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-03-31 11:17:47.646234 th2_common_utils-2.0.0.dev4574477823/LICENSE
--rw-r--r--   0        0        0      255 2023-03-31 11:17:47.646234 th2_common_utils-2.0.0.dev4574477823/README.md
--rw-r--r--   0        0        0      711 2023-03-31 11:18:03.674849 th2_common_utils-2.0.0.dev4574477823/pyproject.toml
--rw-r--r--   0        0        0     1060 2023-03-31 11:17:47.646234 th2_common_utils-2.0.0.dev4574477823/th2_common_utils/__init__.py
--rw-r--r--   0        0        0     6584 2023-03-31 11:17:47.646234 th2_common_utils-2.0.0.dev4574477823/th2_common_utils/converters/filter_converters.py
--rw-r--r--   0        0        0    10267 2023-03-31 11:17:47.646234 th2_common_utils-2.0.0.dev4574477823/th2_common_utils/converters/message_converters.py
--rw-r--r--   0        0        0     2966 2023-03-31 11:17:47.646234 th2_common_utils-2.0.0.dev4574477823/th2_common_utils/event_components.py
--rw-r--r--   0        0        0     3405 2023-03-31 11:17:47.646234 th2_common_utils-2.0.0.dev4574477823/th2_common_utils/event_utils.py
--rw-r--r--   0        0        0     2924 2023-03-31 11:17:47.646234 th2_common_utils-2.0.0.dev4574477823/th2_common_utils/message_fields_access.py
--rw-r--r--   0        0        0     1179 1970-01-01 00:00:00.000000 th2_common_utils-2.0.0.dev4574477823/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-31 18:21:14.912795 th2_common_utils-2.0.1/LICENSE
+-rw-r--r--   0        0        0      255 2023-03-31 18:21:14.912795 th2_common_utils-2.0.1/README.md
+-rw-r--r--   0        0        0      697 2023-03-31 18:21:14.912795 th2_common_utils-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1060 2023-03-31 18:21:14.912795 th2_common_utils-2.0.1/th2_common_utils/__init__.py
+-rw-r--r--   0        0        0     6584 2023-03-31 18:21:14.912795 th2_common_utils-2.0.1/th2_common_utils/converters/filter_converters.py
+-rw-r--r--   0        0        0    10267 2023-03-31 18:21:14.912795 th2_common_utils-2.0.1/th2_common_utils/converters/message_converters.py
+-rw-r--r--   0        0        0     2966 2023-03-31 18:21:14.912795 th2_common_utils-2.0.1/th2_common_utils/event_components.py
+-rw-r--r--   0        0        0     3412 2023-03-31 18:21:14.912795 th2_common_utils-2.0.1/th2_common_utils/event_utils.py
+-rw-r--r--   0        0        0     2924 2023-03-31 18:21:14.912795 th2_common_utils-2.0.1/th2_common_utils/message_fields_access.py
+-rw-r--r--   0        0        0     1165 1970-01-01 00:00:00.000000 th2_common_utils-2.0.1/PKG-INFO
```

### Comparing `th2_common_utils-2.0.0.dev4574477823/LICENSE` & `th2_common_utils-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `th2_common_utils-2.0.0.dev4574477823/pyproject.toml` & `th2_common_utils-2.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "th2-common-utils"
-version = "2.0.0.dev4574477823"
+version = "2.0.1"
 description = "Python library with useful functions for developers and QA needs"
 authors = ["TH2-devs <th2-devs@exactprosystems.com>"]
 readme = "README.md"
 license = "Apache License 2.0"
 homepage = "https://github.com/th2-net/th2-common-utils-py"
 repository = "https://github.com/th2-net/th2-common-utils-py"
 include = [
```

### Comparing `th2_common_utils-2.0.0.dev4574477823/th2_common_utils/__init__.py` & `th2_common_utils-2.0.1/th2_common_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_common_utils-2.0.0.dev4574477823/th2_common_utils/converters/filter_converters.py` & `th2_common_utils-2.0.1/th2_common_utils/converters/filter_converters.py`

 * *Files identical despite different names*

### Comparing `th2_common_utils-2.0.0.dev4574477823/th2_common_utils/converters/message_converters.py` & `th2_common_utils-2.0.1/th2_common_utils/converters/message_converters.py`

 * *Files identical despite different names*

### Comparing `th2_common_utils-2.0.0.dev4574477823/th2_common_utils/event_components.py` & `th2_common_utils-2.0.1/th2_common_utils/event_components.py`

 * *Files identical despite different names*

### Comparing `th2_common_utils-2.0.0.dev4574477823/th2_common_utils/event_utils.py` & `th2_common_utils-2.0.1/th2_common_utils/event_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,10 +88,10 @@
         id=event_id or create_event_id(book_name, scope, start_timestamp),
         parent_id=parent_id,
         end_timestamp=end_timestamp or create_timestamp(),
         status=status,  # type: ignore
         name=name,
         type=event_type,
         body=bytes(body
-                   if isinstance(body, (MessageComponent, TreeTableComponent))
+                   if isinstance(body, (MessageComponent, TreeTableComponent, bytes))
                    else MessageComponent(body)) if body is not None else b'',
         attached_message_ids=attached_message_ids)
```

### Comparing `th2_common_utils-2.0.0.dev4574477823/th2_common_utils/message_fields_access.py` & `th2_common_utils-2.0.1/th2_common_utils/message_fields_access.py`

 * *Files identical despite different names*

### Comparing `th2_common_utils-2.0.0.dev4574477823/PKG-INFO` & `th2_common_utils-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-common-utils
-Version: 2.0.0.dev4574477823
+Version: 2.0.1
 Summary: Python library with useful functions for developers and QA needs
 Home-page: https://github.com/th2-net/th2-common-utils-py
 License: Apache-2.0
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

