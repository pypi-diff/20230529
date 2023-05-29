# Comparing `tmp/django-treenode-0.8.1.tar.gz` & `tmp/django-treenode-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-treenode-0.8.1.tar", last modified: Thu May 17 21:25:38 2018, max compression
+gzip compressed data, was "dist/django-treenode-0.9.0.tar", last modified: Mon Jun 11 14:04:10 2018, max compression
```

## Comparing `django-treenode-0.8.1.tar` & `django-treenode-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2018-05-17 21:25:38.000000 django-treenode-0.8.1/
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2018-05-17 21:25:38.000000 django-treenode-0.8.1/django_treenode.egg-info/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)        1 2018-05-17 21:25:38.000000 django-treenode-0.8.1/django_treenode.egg-info/dependency_links.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    14544 2018-05-17 21:25:38.000000 django-treenode-0.8.1/django_treenode.egg-info/PKG-INFO
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      472 2018-05-17 21:25:38.000000 django-treenode-0.8.1/django_treenode.egg-info/SOURCES.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)        9 2018-05-17 21:25:38.000000 django-treenode-0.8.1/django_treenode.egg-info/top_level.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1070 2018-04-03 19:32:25.000000 django-treenode-0.8.1/LICENSE.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      114 2018-04-10 12:54:10.000000 django-treenode-0.8.1/MANIFEST.in
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    14544 2018-05-17 21:25:38.000000 django-treenode-0.8.1/PKG-INFO
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     8513 2018-05-17 20:27:45.000000 django-treenode-0.8.1/README.md
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     9710 2018-05-17 20:28:46.000000 django-treenode-0.8.1/README.rst
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)       79 2018-05-17 21:25:38.000000 django-treenode-0.8.1/setup.cfg
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2132 2018-05-09 08:42:11.000000 django-treenode-0.8.1/setup.py
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2018-05-17 21:25:38.000000 django-treenode-0.8.1/treenode/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      190 2018-05-17 20:31:37.000000 django-treenode-0.8.1/treenode/__init__.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2762 2018-05-09 08:35:21.000000 django-treenode-0.8.1/treenode/admin.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1038 2018-05-11 14:07:57.000000 django-treenode-0.8.1/treenode/debug.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      572 2018-05-09 09:50:23.000000 django-treenode-0.8.1/treenode/forms.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      285 2018-05-17 13:54:51.000000 django-treenode-0.8.1/treenode/memory.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    21843 2018-05-17 21:23:03.000000 django-treenode-0.8.1/treenode/models.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2000 2018-05-17 13:46:30.000000 django-treenode-0.8.1/treenode/signals.py
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2018-05-17 21:25:38.000000 django-treenode-0.8.1/treenode/static/
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2018-05-17 21:25:38.000000 django-treenode-0.8.1/treenode/static/treenode/
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2018-05-17 21:25:38.000000 django-treenode-0.8.1/treenode/static/treenode/css/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1392 2018-04-18 08:14:14.000000 django-treenode-0.8.1/treenode/static/treenode/css/treenode.css
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2018-05-17 21:25:38.000000 django-treenode-0.8.1/treenode/static/treenode/js/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     7727 2018-04-24 10:31:39.000000 django-treenode-0.8.1/treenode/static/treenode/js/treenode.js
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      274 2018-04-26 15:33:17.000000 django-treenode-0.8.1/treenode/utils.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)       47 2018-05-17 21:23:08.000000 django-treenode-0.8.1/treenode/version.py
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2018-06-11 14:04:10.000000 django-treenode-0.9.0/
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2018-06-11 14:04:10.000000 django-treenode-0.9.0/django_treenode.egg-info/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)        1 2018-06-11 14:04:10.000000 django-treenode-0.9.0/django_treenode.egg-info/dependency_links.txt
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    14534 2018-06-11 14:04:10.000000 django-treenode-0.9.0/django_treenode.egg-info/PKG-INFO
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      490 2018-06-11 14:04:10.000000 django-treenode-0.9.0/django_treenode.egg-info/SOURCES.txt
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)        9 2018-06-11 14:04:10.000000 django-treenode-0.9.0/django_treenode.egg-info/top_level.txt
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1070 2018-04-03 19:32:25.000000 django-treenode-0.9.0/LICENSE.txt
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      114 2018-04-10 12:54:10.000000 django-treenode-0.9.0/MANIFEST.in
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    14534 2018-06-11 14:04:10.000000 django-treenode-0.9.0/PKG-INFO
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     8503 2018-06-11 13:48:34.000000 django-treenode-0.9.0/README.md
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     9700 2018-06-11 13:48:34.000000 django-treenode-0.9.0/README.rst
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)       79 2018-06-11 14:04:10.000000 django-treenode-0.9.0/setup.cfg
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2132 2018-05-09 08:42:11.000000 django-treenode-0.9.0/setup.py
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2018-06-11 14:04:10.000000 django-treenode-0.9.0/treenode/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      190 2018-05-17 20:31:51.000000 django-treenode-0.9.0/treenode/__init__.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2762 2018-05-09 08:35:21.000000 django-treenode-0.9.0/treenode/admin.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      671 2018-06-11 13:43:10.000000 django-treenode-0.9.0/treenode/cache.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1038 2018-05-11 14:07:57.000000 django-treenode-0.9.0/treenode/debug.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      572 2018-05-09 09:50:23.000000 django-treenode-0.9.0/treenode/forms.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      522 2018-06-11 10:57:13.000000 django-treenode-0.9.0/treenode/memory.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    22984 2018-06-11 13:49:54.000000 django-treenode-0.9.0/treenode/models.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2000 2018-05-17 13:46:30.000000 django-treenode-0.9.0/treenode/signals.py
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2018-06-11 14:04:10.000000 django-treenode-0.9.0/treenode/static/
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2018-06-11 14:04:10.000000 django-treenode-0.9.0/treenode/static/treenode/
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2018-06-11 14:04:10.000000 django-treenode-0.9.0/treenode/static/treenode/css/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1392 2018-04-18 08:14:14.000000 django-treenode-0.9.0/treenode/static/treenode/css/treenode.css
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2018-06-11 14:04:10.000000 django-treenode-0.9.0/treenode/static/treenode/js/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     7727 2018-04-24 10:31:39.000000 django-treenode-0.9.0/treenode/static/treenode/js/treenode.js
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      274 2018-06-11 10:37:24.000000 django-treenode-0.9.0/treenode/utils.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)       47 2018-06-11 13:07:54.000000 django-treenode-0.9.0/treenode/version.py
```

### Comparing `django-treenode-0.8.1/django_treenode.egg-info/PKG-INFO` & `django-treenode-0.9.0/django_treenode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 1.1
 Name: django-treenode
-Version: 0.8.1
+Version: 0.9.0
 Summary: django-treenode is probably the best abstract model / admin for your tree based stuff.
 Home-page: https://github.com/fabiocaccamo/django-treenode
 Author: Fabio Caccamo
 Author-email: fabio.caccamo@gmail.com
 License: MIT
-Download-URL: https://github.com/fabiocaccamo/django-treenode/archive/0.8.1.tar.gz
+Download-URL: https://github.com/fabiocaccamo/django-treenode/archive/0.9.0.tar.gz
 Description: |Build Status| |coverage| |Code Health| |Requirements Status| |PyPI version| |Py versions| |License|
         
         django-treenode
         ===============
         
         Probably the best abstract model / admin for your **tree** based stuff.
         
         Features
         --------
         
-        -  **Fast** - get ``ancestors``, ``children``, ``descendants``, ``parent``, ``root``, ``siblings``, ``tree``, ... *(1 query)*
-        -  **Synced** - in-memory model instances are automatically updated *(0 queries)*
+        -  **Fast** - get ``ancestors``, ``children``, ``descendants``, ``parent``, ``root``, ``siblings``, ``tree`` with **no queries**
+        -  **Synced** - in-memory model instances are automatically updated
         -  **Compatibility** - you can easily add treenode to existing projects
         -  **No dependencies**
         -  **Easy configuration** - just extend the abstract model / model-admin
         -  **Admin integration** - great tree visualization with optional accordion
         
         +------------------+---------------------+
         | Simple admin     | Accordion admin     |
@@ -155,15 +155,15 @@
         
         Get the **ancestors queryset** *(0 queries)*:
         
         .. code:: python
         
             obj.get_ancestors_queryset()
         
-        Get the **breadcrumbs** to current node (included) *(1 query)*
+        Get the **breadcrumbs** to current node (included) *(1 query)*:
         
         .. code:: python
         
             obj.get_breadcrumbs(attr=None)
             # or
             obj.breadcrumbs
```

### Comparing `django-treenode-0.8.1/LICENSE.txt` & `django-treenode-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-treenode-0.8.1/PKG-INFO` & `django-treenode-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 1.1
 Name: django-treenode
-Version: 0.8.1
+Version: 0.9.0
 Summary: django-treenode is probably the best abstract model / admin for your tree based stuff.
 Home-page: https://github.com/fabiocaccamo/django-treenode
 Author: Fabio Caccamo
 Author-email: fabio.caccamo@gmail.com
 License: MIT
-Download-URL: https://github.com/fabiocaccamo/django-treenode/archive/0.8.1.tar.gz
+Download-URL: https://github.com/fabiocaccamo/django-treenode/archive/0.9.0.tar.gz
 Description: |Build Status| |coverage| |Code Health| |Requirements Status| |PyPI version| |Py versions| |License|
         
         django-treenode
         ===============
         
         Probably the best abstract model / admin for your **tree** based stuff.
         
         Features
         --------
         
-        -  **Fast** - get ``ancestors``, ``children``, ``descendants``, ``parent``, ``root``, ``siblings``, ``tree``, ... *(1 query)*
-        -  **Synced** - in-memory model instances are automatically updated *(0 queries)*
+        -  **Fast** - get ``ancestors``, ``children``, ``descendants``, ``parent``, ``root``, ``siblings``, ``tree`` with **no queries**
+        -  **Synced** - in-memory model instances are automatically updated
         -  **Compatibility** - you can easily add treenode to existing projects
         -  **No dependencies**
         -  **Easy configuration** - just extend the abstract model / model-admin
         -  **Admin integration** - great tree visualization with optional accordion
         
         +------------------+---------------------+
         | Simple admin     | Accordion admin     |
@@ -155,15 +155,15 @@
         
         Get the **ancestors queryset** *(0 queries)*:
         
         .. code:: python
         
             obj.get_ancestors_queryset()
         
-        Get the **breadcrumbs** to current node (included) *(1 query)*
+        Get the **breadcrumbs** to current node (included) *(1 query)*:
         
         .. code:: python
         
             obj.get_breadcrumbs(attr=None)
             # or
             obj.breadcrumbs
```

### Comparing `django-treenode-0.8.1/README.md` & `django-treenode-0.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 [simple-admin]: https://user-images.githubusercontent.com/1035294/39823224-dff5944c-53ac-11e8-9d7f-60f1a31b2730.png
 [accordion-admin]: https://user-images.githubusercontent.com/1035294/39823232-e3a5d99e-53ac-11e8-98ad-edd6b77c44a4.png
 
 # django-treenode
 Probably the best abstract model / admin for your **tree** based stuff.
 
 ## Features
-- **Fast** - get `ancestors`, `children`, `descendants`, `parent`, `root`, `siblings`, `tree`, ... *(1 query)*
-- **Synced** - in-memory model instances are automatically updated *(0 queries)*
+- **Fast** - get `ancestors`, `children`, `descendants`, `parent`, `root`, `siblings`, `tree` with **no queries**
+- **Synced** - in-memory model instances are automatically updated
 - **Compatibility** - you can easily add treenode to existing projects
 - **No dependencies**
 - **Easy configuration** - just extend the abstract model / model-admin
 - **Admin integration** - great tree visualization with optional accordion
 
 | Simple admin | Accordion admin |
 | --- | --- |
@@ -131,15 +131,15 @@
 ```
 
 Get the **ancestors queryset** *(0 queries)*:
 ```python
 obj.get_ancestors_queryset()
 ```
 
-Get the **breadcrumbs** to current node (included) *(1 query)*
+Get the **breadcrumbs** to current node (included) *(1 query)*:
 ```python
 obj.get_breadcrumbs(attr=None)
 # or
 obj.breadcrumbs
 ```
 
 Get a **list containing all children** *(1 query)*:
```

### Comparing `django-treenode-0.8.1/README.rst` & `django-treenode-0.9.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 ===============
 
 Probably the best abstract model / admin for your **tree** based stuff.
 
 Features
 --------
 
--  **Fast** - get ``ancestors``, ``children``, ``descendants``, ``parent``, ``root``, ``siblings``, ``tree``, ... *(1 query)*
--  **Synced** - in-memory model instances are automatically updated *(0 queries)*
+-  **Fast** - get ``ancestors``, ``children``, ``descendants``, ``parent``, ``root``, ``siblings``, ``tree`` with **no queries**
+-  **Synced** - in-memory model instances are automatically updated
 -  **Compatibility** - you can easily add treenode to existing projects
 -  **No dependencies**
 -  **Easy configuration** - just extend the abstract model / model-admin
 -  **Admin integration** - great tree visualization with optional accordion
 
 +------------------+---------------------+
 | Simple admin     | Accordion admin     |
@@ -146,15 +146,15 @@
 
 Get the **ancestors queryset** *(0 queries)*:
 
 .. code:: python
 
     obj.get_ancestors_queryset()
 
-Get the **breadcrumbs** to current node (included) *(1 query)*
+Get the **breadcrumbs** to current node (included) *(1 query)*:
 
 .. code:: python
 
     obj.get_breadcrumbs(attr=None)
     # or
     obj.breadcrumbs
```

### Comparing `django-treenode-0.8.1/setup.py` & `django-treenode-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-treenode-0.8.1/treenode/admin.py` & `django-treenode-0.9.0/treenode/admin.py`

 * *Files identical despite different names*

### Comparing `django-treenode-0.8.1/treenode/debug.py` & `django-treenode-0.9.0/treenode/debug.py`

 * *Files identical despite different names*

### Comparing `django-treenode-0.8.1/treenode/forms.py` & `django-treenode-0.9.0/treenode/forms.py`

 * *Files identical despite different names*

### Comparing `django-treenode-0.8.1/treenode/models.py` & `django-treenode-0.9.0/treenode/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 from django.db import models, transaction
 from django.utils.encoding import force_text, python_2_unicode_compatible
 from django.utils.safestring import mark_safe
 from django.utils.text import slugify
 from django.utils.translation import gettext_lazy as _
 
 from . import classproperty
+from .cache import clear_cache, query_cache, update_cache
 from .debug import debug_performance
-from .memory import clear_refs, get_refs
+from .memory import clear_refs, update_refs
 from .signals import connect_signals, no_signals
 from .utils import join_pks, split_pks
 
 
 @python_2_unicode_compatible
 class TreeNodeModel(models.Model):
 
@@ -77,16 +78,16 @@
         verbose_name=_('Descendants count'), )
 
     tn_index = models.PositiveSmallIntegerField(
         default=0, editable=False,
         verbose_name=_('Index'), )
 
     tn_level = models.PositiveSmallIntegerField(
-        default=0, editable=False,
-        validators=[MinValueValidator(0), MaxValueValidator(10)],
+        default=1, editable=False,
+        validators=[MinValueValidator(1), MaxValueValidator(10)],
         verbose_name=_('Level'), )
 
     tn_parent = models.ForeignKey('self',
         related_name='tn_children',
         on_delete=models.CASCADE,
         blank=True, null=True,
         verbose_name=_('Parent'), )
@@ -118,57 +119,67 @@
 
     @classmethod
     def delete_tree(cls):
         with no_signals():
             with transaction.atomic():
                 cls.objects.all().delete()
             clear_refs(cls)
+            clear_cache(cls)
 
-    def get_ancestors(self):
-        return list(self.get_ancestors_queryset())
+    def get_ancestors(self, cache=True):
+        if cache:
+            return query_cache(self.__class__, pks=self.tn_ancestors_pks)
+        else:
+            return list(self.get_ancestors_queryset())
 
     def get_ancestors_count(self):
         return self.tn_ancestors_count
 
     def get_ancestors_queryset(self):
         return self.__class__.objects.filter(
             pk__in=split_pks(self.tn_ancestors_pks))
 
-    def get_breadcrumbs(self, attr=None):
-        objs = self.get_ancestors() + [self]
+    def get_breadcrumbs(self, attr=None, cache=True):
+        objs = self.get_ancestors(cache=cache) + [self]
         return [getattr(obj, attr) for obj in objs] if attr else objs
 
-    def get_children(self):
-        return list(self.get_children_queryset())
+    def get_children(self, cache=True):
+        if cache:
+            return query_cache(self.__class__, pks=self.tn_children_pks)
+        else:
+            return list(self.get_children_queryset())
 
     def get_children_count(self):
         return self.tn_children_count
 
     def get_children_queryset(self):
         return self.__class__.objects.filter(
             pk__in=split_pks(self.tn_children_pks))
 
     def get_depth(self):
         return self.tn_depth
 
-    def get_descendants(self):
-        return list(self.get_descendants_queryset())
+    def get_descendants(self, cache=True):
+        if cache:
+            return query_cache(self.__class__, pks=self.tn_descendants_pks)
+        else:
+            return list(self.get_descendants_queryset())
 
     def get_descendants_count(self):
         return self.tn_descendants_count
 
     def get_descendants_queryset(self):
         return self.__class__.objects.filter(
             pk__in=split_pks(self.tn_descendants_pks))
 
-    def get_descendants_tree(self):
-        return self.__get_nodes_tree(self)
+    def get_descendants_tree(self, cache=True):
+        return self.__get_nodes_tree(instance=self, cache=cache)
 
-    def get_descendants_tree_display(self):
-        objs = list(self.get_descendants_queryset())
+    def get_descendants_tree_display(self, cache=True):
+        objs = self.get_descendants(cache=cache)
         strs = ['%s' % (obj, ) for obj in objs]
         d = '\n'.join(strs)
         return d
 
     # def get_descendants_tree_dump(self, indent=2, default=None):
     #     data = self.get_descendants_tree()
     #     func = lambda obj:str(obj.pk)
@@ -223,51 +234,64 @@
     def get_priority(self):
         return self.tn_priority
 
     def set_priority(self, val):
         self.tn_priority = val
         self.save()
 
-    def get_root(self):
+    def get_root(self, cache=True):
         root_pk = (split_pks(self.tn_ancestors_pks) + [self.pk])[0]
-        root_obj = self.__class__.objects.get(pk=root_pk)
+        if cache:
+            root_obj = query_cache(self.__class__, pk=root_pk)
+        else:
+            root_obj = self.__class__.objects.get(pk=root_pk)
         return root_obj
 
     @classmethod
-    def get_roots(cls):
-        return list(cls.get_roots_queryset())
+    def get_roots(cls, cache=True):
+        if cache:
+            return [obj for obj in query_cache(cls) if obj.tn_ancestors_count == 0]
+        else:
+            return list(cls.get_roots_queryset())
 
     @classmethod
     def get_roots_queryset(cls):
-        return cls.objects.filter(tn_parent=None)
+        # return cls.objects.filter(tn_parent=None)
+        return cls.objects.filter(tn_ancestors_count=0)
 
-    def get_siblings(self):
-        return list(self.get_siblings_queryset())
+    def get_siblings(self, cache=True):
+        if cache:
+            return query_cache(self.__class__, pks=self.tn_siblings_pks)
+        else:
+            return list(self.get_siblings_queryset())
 
     def get_siblings_count(self):
         return self.tn_siblings_count
 
     def get_siblings_queryset(self):
         return self.__class__.objects.filter(
             pk__in=split_pks(self.tn_siblings_pks))
 
     @classmethod
-    def get_tree(cls):
-        return cls.__get_nodes_tree()
+    def get_tree(cls, cache=True):
+        return cls.__get_nodes_tree(instance=None, cache=cache)
 
     @classmethod
-    def get_tree_display(cls):
-        objs = list(cls.objects.all())
+    def get_tree_display(cls, cache=True):
+        if cache:
+            objs = query_cache(cls)
+        else:
+            objs = list(cls.objects.all())
         strs = ['%s' % (obj, ) for obj in objs]
         d = '\n'.join(strs)
         return d
 
     # @classmethod
-    # def get_tree_dump(cls, indent=2, default=None):
-    #     data = cls.get_tree()
+    # def get_tree_dump(cls, cache=True, indent=2, default=None):
+    #     data = cls.get_tree(cache=cache)
     #     func = lambda obj:str(obj.pk)
     #     dump = json.dumps(data,
     #         sort_keys=True,
     #         indent=indent,
     #         default=func if not default else default)
     #     return dump
 
@@ -334,20 +358,18 @@
 
             with transaction.atomic():
                 for obj_key, obj_data in objs_data.items():
                     obj_pk = int(obj_key)
                     cls.objects.filter(pk=obj_pk).update(**obj_data)
 
             # update in-memory instances
-            for obj in get_refs(cls):
-                obj_key = str(obj.pk)
-                obj_data = objs_data.get(obj_key)
-                if obj_data:
-                    for key, value in obj_data.items():
-                        setattr(obj, key, value)
+            update_refs(cls, objs_data)
+
+            # update cache instances
+            update_cache(cls)
 
     # Private methods
 
     def __get_node_order_str(self):
         priority_max = 99999
         priority_len = len(str(priority_max))
         priority_val = priority_max - min(self.tn_priority, priority_max)
@@ -551,35 +573,41 @@
 
         # clean list data
         objs_list = [obj for obj in objs_list if str(obj.pk) in objs_data]
 
         return (objs_qs, objs_list, objs_dict, objs_data, )
 
     @classmethod
-    def __get_nodes_tree(cls, instance=None):
+    def __get_nodes_tree(cls, instance=None, cache=True):
 
         def __get_node_tree(obj):
             child_tree = { 'node':obj, 'tree':[] }
             if obj.tn_children_pks:
                 children_pks = split_pks(obj.tn_children_pks)
                 for child_pk in children_pks:
                     child_key = str(child_pk)
                     child_obj = objs_dict.get(child_key)
                     if child_obj:
                         child_tree['tree'].append(
                             __get_node_tree(child_obj))
             return child_tree
 
         if instance:
-            objs_pks = split_pks(instance.tn_descendants_pks)
-            objs_list = list(cls.objects.filter(pk__in=objs_pks))
+            objs_pks = instance.tn_descendants_pks
+            if cache:
+                objs_list = query_cache(cls, pks=objs_pks)
+            else:
+                objs_list = list(cls.objects.filter(pk__in=split_pks(objs_pks)))
             objs_dict = { str(obj.pk):obj for obj in objs_list }
             objs_tree = __get_node_tree(instance)['tree']
         else:
-            objs_list = list(cls.objects.all())
+            if cache:
+                objs_list = query_cache(cls)
+            else:
+                objs_list = list(cls.objects.all())
             objs_dict = { str(obj.pk):obj for obj in objs_list }
             objs_tree = [__get_node_tree(obj) for obj in objs_list if obj.tn_level == 1]
 
         return objs_tree
 
     class Meta:
         abstract = True
```

### Comparing `django-treenode-0.8.1/treenode/signals.py` & `django-treenode-0.9.0/treenode/signals.py`

 * *Files identical despite different names*

### Comparing `django-treenode-0.8.1/treenode/static/treenode/css/treenode.css` & `django-treenode-0.9.0/treenode/static/treenode/css/treenode.css`

 * *Files identical despite different names*

### Comparing `django-treenode-0.8.1/treenode/static/treenode/js/treenode.js` & `django-treenode-0.9.0/treenode/static/treenode/js/treenode.js`

 * *Files identical despite different names*

