# Comparing `tmp/django_dynamic_storage-0.1.3.tar.gz` & `tmp/django_dynamic_storage-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_dynamic_storage-0.1.3.tar", max compression
+gzip compressed data, was "django_dynamic_storage-0.1.4.tar", max compression
```

## Comparing `django_dynamic_storage-0.1.3.tar` & `django_dynamic_storage-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      717 2023-05-28 14:44:04.879858 django_dynamic_storage-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-05-28 14:44:04.879858 django_dynamic_storage-0.1.3/dynamic_storage/__init__.py
--rw-r--r--   0        0        0     5418 2023-05-28 14:44:04.883859 django_dynamic_storage-0.1.3/dynamic_storage/models.py
--rw-r--r--   0        0        0      120 2023-05-28 14:44:04.883859 django_dynamic_storage-0.1.3/dynamic_storage/signals.py
--rw-r--r--   0        0        0     1410 2023-05-28 14:44:04.883859 django_dynamic_storage-0.1.3/dynamic_storage/storage.py
--rw-r--r--   0        0        0     1064 2023-05-28 14:44:04.883859 django_dynamic_storage-0.1.3/dynamic_storage/test/storage.py
--rw-r--r--   0        0        0      745 2023-05-28 14:44:04.883859 django_dynamic_storage-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 django_dynamic_storage-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3241 2023-05-29 06:09:43.310598 django_dynamic_storage-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 06:09:43.310598 django_dynamic_storage-0.1.4/dynamic_storage/__init__.py
+-rw-r--r--   0        0        0     5418 2023-05-29 06:09:43.310598 django_dynamic_storage-0.1.4/dynamic_storage/models.py
+-rw-r--r--   0        0        0      120 2023-05-29 06:09:43.310598 django_dynamic_storage-0.1.4/dynamic_storage/signals.py
+-rw-r--r--   0        0        0     1492 2023-05-29 06:09:43.310598 django_dynamic_storage-0.1.4/dynamic_storage/storage.py
+-rw-r--r--   0        0        0     1064 2023-05-29 06:09:43.310598 django_dynamic_storage-0.1.4/dynamic_storage/test/storage.py
+-rw-r--r--   0        0        0     1188 2023-05-29 06:09:43.310598 django_dynamic_storage-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4409 1970-01-01 00:00:00.000000 django_dynamic_storage-0.1.4/PKG-INFO
```

### Comparing `django_dynamic_storage-0.1.3/dynamic_storage/models.py` & `django_dynamic_storage-0.1.4/dynamic_storage/models.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_storage-0.1.3/dynamic_storage/storage.py` & `django_dynamic_storage-0.1.4/dynamic_storage/storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,18 @@
 
     def __eq__(self, other) -> bool:
         """
         how to differentiate two instances of the same storage class
         Override this for your use case,
         for example add the comparison based on bucket names
         """
-        return self.__class__ == other.__class__
+        return (
+            self.__class__ == other.__class__
+            and self.init_params() == other.init_params()
+        )
 
     def uninit(self) -> prob:
         """get the required properties for future initialization"""
         return {
             "import_path": f"{self.__class__.__module__}.{self.__class__.__qualname__}",
             "constructor": self.init_params(),
         }
```

### Comparing `django_dynamic_storage-0.1.3/dynamic_storage/test/storage.py` & `django_dynamic_storage-0.1.4/dynamic_storage/test/storage.py`

 * *Files identical despite different names*

