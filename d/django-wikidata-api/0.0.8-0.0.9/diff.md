# Comparing `tmp/django-wikidata-api-0.0.8.tar.gz` & `tmp/django-wikidata-api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-wikidata-api-0.0.8.tar", last modified: Wed Feb 19 03:46:46 2020, max compression
+gzip compressed data, was "dist/django-wikidata-api-0.0.9.tar", last modified: Thu Feb 20 00:52:07 2020, max compression
```

## Comparing `django-wikidata-api-0.0.8.tar` & `django-wikidata-api-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 ksealsnutt   (501) staff       (20)        0 2020-02-19 03:46:46.000000 django-wikidata-api-0.0.8/
--rw-r--r--   0 ksealsnutt   (501) staff       (20)     4530 2020-01-27 15:43:17.000000 django-wikidata-api-0.0.8/CONTRIBUTING.md
--rw-r--r--   0 ksealsnutt   (501) staff       (20)    34523 2019-10-21 17:50:40.000000 django-wikidata-api-0.0.8/LICENSE
--rw-r--r--   0 ksealsnutt   (501) staff       (20)      158 2019-10-21 19:13:50.000000 django-wikidata-api-0.0.8/MANIFEST.in
--rw-r--r--   0 ksealsnutt   (501) staff       (20)     2076 2020-02-19 03:46:46.000000 django-wikidata-api-0.0.8/PKG-INFO
--rw-r--r--   0 ksealsnutt   (501) staff       (20)     1109 2019-10-22 02:53:41.000000 django-wikidata-api-0.0.8/README.md
-drwxr-xr-x   0 ksealsnutt   (501) staff       (20)        0 2020-02-19 03:46:46.000000 django-wikidata-api-0.0.8/django_wikidata_api/
--rw-r--r--   0 ksealsnutt   (501) staff       (20)       51 2020-01-27 15:43:17.000000 django-wikidata-api-0.0.8/django_wikidata_api/__init__.py
--rw-r--r--   0 ksealsnutt   (501) staff       (20)      123 2020-01-27 15:43:17.000000 django-wikidata-api-0.0.8/django_wikidata_api/admin.py
--rw-r--r--   0 ksealsnutt   (501) staff       (20)      217 2020-01-27 15:43:17.000000 django-wikidata-api-0.0.8/django_wikidata_api/apps.py
--rw-r--r--   0 ksealsnutt   (501) staff       (20)      145 2020-02-19 03:43:56.000000 django-wikidata-api-0.0.8/django_wikidata_api/exceptions.py
--rw-r--r--   0 ksealsnutt   (501) staff       (20)    13211 2020-01-27 15:43:20.000000 django-wikidata-api-0.0.8/django_wikidata_api/fields.py
--rw-r--r--   0 ksealsnutt   (501) staff       (20)    16538 2020-02-19 03:43:56.000000 django-wikidata-api-0.0.8/django_wikidata_api/models.py
--rw-r--r--   0 ksealsnutt   (501) staff       (20)     2098 2020-01-27 22:51:37.000000 django-wikidata-api-0.0.8/django_wikidata_api/serializers.py
--rw-r--r--   0 ksealsnutt   (501) staff       (20)      514 2020-01-27 15:43:17.000000 django-wikidata-api-0.0.8/django_wikidata_api/urls.py
--rw-r--r--   0 ksealsnutt   (501) staff       (20)     1275 2020-01-27 15:43:17.000000 django-wikidata-api-0.0.8/django_wikidata_api/utils.py
--rw-r--r--   0 ksealsnutt   (501) staff       (20)      956 2020-01-27 15:43:17.000000 django-wikidata-api-0.0.8/django_wikidata_api/views.py
--rw-r--r--   0 ksealsnutt   (501) staff       (20)     5851 2020-01-27 22:51:37.000000 django-wikidata-api-0.0.8/django_wikidata_api/viewsets.py
-drwxr-xr-x   0 ksealsnutt   (501) staff       (20)        0 2020-02-19 03:46:46.000000 django-wikidata-api-0.0.8/django_wikidata_api.egg-info/
--rw-r--r--   0 ksealsnutt   (501) staff       (20)     2076 2020-02-19 03:46:46.000000 django-wikidata-api-0.0.8/django_wikidata_api.egg-info/PKG-INFO
--rw-r--r--   0 ksealsnutt   (501) staff       (20)      612 2020-02-19 03:46:46.000000 django-wikidata-api-0.0.8/django_wikidata_api.egg-info/SOURCES.txt
--rw-r--r--   0 ksealsnutt   (501) staff       (20)        1 2020-02-19 03:46:46.000000 django-wikidata-api-0.0.8/django_wikidata_api.egg-info/dependency_links.txt
--rw-r--r--   0 ksealsnutt   (501) staff       (20)      129 2020-02-19 03:46:46.000000 django-wikidata-api-0.0.8/django_wikidata_api.egg-info/requires.txt
--rw-r--r--   0 ksealsnutt   (501) staff       (20)       20 2020-02-19 03:46:46.000000 django-wikidata-api-0.0.8/django_wikidata_api.egg-info/top_level.txt
--rw-r--r--   0 ksealsnutt   (501) staff       (20)       38 2020-02-19 03:46:46.000000 django-wikidata-api-0.0.8/setup.cfg
--rw-r--r--   0 ksealsnutt   (501) staff       (20)     1447 2020-02-19 03:46:02.000000 django-wikidata-api-0.0.8/setup.py
--rw-r--r--   0 ksealsnutt   (501) staff       (20)      513 2019-10-28 15:35:13.000000 django-wikidata-api-0.0.8/tox.ini
+drwxr-xr-x   0 ksealsnutt   (501) staff       (20)        0 2020-02-20 00:52:07.000000 django-wikidata-api-0.0.9/
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)     4530 2020-02-19 20:00:27.000000 django-wikidata-api-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)    34523 2019-10-21 17:50:40.000000 django-wikidata-api-0.0.9/LICENSE
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)      158 2019-10-21 19:13:50.000000 django-wikidata-api-0.0.9/MANIFEST.in
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)     2076 2020-02-20 00:52:07.000000 django-wikidata-api-0.0.9/PKG-INFO
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)     1109 2019-10-22 02:53:41.000000 django-wikidata-api-0.0.9/README.md
+drwxr-xr-x   0 ksealsnutt   (501) staff       (20)        0 2020-02-20 00:52:07.000000 django-wikidata-api-0.0.9/django_wikidata_api/
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)       51 2020-02-19 20:00:27.000000 django-wikidata-api-0.0.9/django_wikidata_api/__init__.py
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)      123 2020-02-19 20:00:27.000000 django-wikidata-api-0.0.9/django_wikidata_api/admin.py
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)      217 2020-02-19 20:00:27.000000 django-wikidata-api-0.0.9/django_wikidata_api/apps.py
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)      145 2020-02-19 20:00:27.000000 django-wikidata-api-0.0.9/django_wikidata_api/exceptions.py
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)    13784 2020-02-19 21:25:03.000000 django-wikidata-api-0.0.9/django_wikidata_api/fields.py
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)    16765 2020-02-19 21:25:03.000000 django-wikidata-api-0.0.9/django_wikidata_api/models.py
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)     2098 2020-02-19 20:00:27.000000 django-wikidata-api-0.0.9/django_wikidata_api/serializers.py
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)      514 2020-02-19 20:00:27.000000 django-wikidata-api-0.0.9/django_wikidata_api/urls.py
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)     1275 2020-02-19 20:00:27.000000 django-wikidata-api-0.0.9/django_wikidata_api/utils.py
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)      956 2020-02-19 20:00:27.000000 django-wikidata-api-0.0.9/django_wikidata_api/views.py
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)     5851 2020-02-19 20:00:27.000000 django-wikidata-api-0.0.9/django_wikidata_api/viewsets.py
+drwxr-xr-x   0 ksealsnutt   (501) staff       (20)        0 2020-02-20 00:52:07.000000 django-wikidata-api-0.0.9/django_wikidata_api.egg-info/
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)     2076 2020-02-20 00:52:07.000000 django-wikidata-api-0.0.9/django_wikidata_api.egg-info/PKG-INFO
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)      612 2020-02-20 00:52:07.000000 django-wikidata-api-0.0.9/django_wikidata_api.egg-info/SOURCES.txt
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)        1 2020-02-20 00:52:07.000000 django-wikidata-api-0.0.9/django_wikidata_api.egg-info/dependency_links.txt
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)      129 2020-02-20 00:52:07.000000 django-wikidata-api-0.0.9/django_wikidata_api.egg-info/requires.txt
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)       20 2020-02-20 00:52:07.000000 django-wikidata-api-0.0.9/django_wikidata_api.egg-info/top_level.txt
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)       38 2020-02-20 00:52:07.000000 django-wikidata-api-0.0.9/setup.cfg
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)     1447 2020-02-20 00:51:51.000000 django-wikidata-api-0.0.9/setup.py
+-rw-r--r--   0 ksealsnutt   (501) staff       (20)      513 2019-10-28 15:35:13.000000 django-wikidata-api-0.0.9/tox.ini
```

### Comparing `django-wikidata-api-0.0.8/CONTRIBUTING.md` & `django-wikidata-api-0.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-wikidata-api-0.0.8/LICENSE` & `django-wikidata-api-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-wikidata-api-0.0.8/PKG-INFO` & `django-wikidata-api-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-wikidata-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Package for interfacing with Wikidata within a Django App
 Home-page: https://github.com/kennethsn/django-wikidata-api
 Author: Kenneth Seals-Nutt
 Author-email: kenneth@seals-nutt.com
 License: AGPL-3.0
 Description: # django-wikidata-api
         [![PyPI](https://img.shields.io/pypi/v/django-wikidata-api?style=flat-square)](https://pypi.org/project/django-wikidata-api/)
```

### Comparing `django-wikidata-api-0.0.8/README.md` & `django-wikidata-api-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `django-wikidata-api-0.0.8/django_wikidata_api/fields.py` & `django-wikidata-api-0.0.9/django_wikidata_api/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,21 +18,22 @@
     name = None
     serializer_field_class = serializers.Field
     default_serializer_settings = {}
     serializer = None
     sparql_field_suffix = ""
 
     def __init__(self, properties=None, values=None, default=None, required=False, entity_name='main',
-                 serializer_settings=None, public=None, **kwargs):
+                 serializer_settings=None, public=None, show_in_minimal=False, **kwargs):
         self.entity_name = entity_name
         self.properties = properties
         self.values = values
         self.default = default
         self.required = required
         self.public = public  # used to override private _attrs
+        self.show_in_minimal = show_in_minimal  # used to determine if a field should show up in the list view
         self.from_name = "?{}{}".format(self.entity_name, self.sparql_field_suffix)
         set_kwargs(self, kwargs)
         self.set_serializer(serializer_settings or {})
 
     def __repr__(self):
         return "<{}: {}>".format(self.__class__.__name__, self.name)
 
@@ -74,15 +75,15 @@
 
         Args:
             minimal (Optional[Bool]): True if only need ID, label and description, False otherwise
 
         Returns (str):
 
         """
-        return "" if minimal else f"?{self.name}"
+        return "" if self.use_minimal(minimal) else f"?{self.name}"
 
     def to_wikidata_filter(self):
         """
         Get the portion of a SPARQL query that specifies the filtering in the WHERE clause.
         Returns (str):
 
         Raises (AssertionError): If there are no self.properties defined
@@ -117,14 +118,26 @@
             wikidata_response (Dict[str, Dict[str, str]]):
 
         Returns (str):
 
         """
         return get_wikidata_field(wikidata_response, self.name, self.default)
 
+    def use_minimal(self, minimal):
+        """
+        Check if this field should return a minimal version or full version for query building.
+
+        Args:
+            minimal (Bool):
+
+        Returns (Bool):
+
+        """
+        return minimal and not self.show_in_minimal
+
 
 class WikidataListResponseMixin(object):
     separator = '|'
     name = None
     default = None
     serializer_field_class = serializers.ListField
     default_serializer_settings = {'allow_null': True, 'allow_empty': True}
@@ -214,19 +227,20 @@
     service_property = "schema:description"
     sparql_field_suffix = 'Description'
 
 
 class WikidataEntityField(WikidataField):
     # TODO: Add Item and Property SubClasses
     serializer_field_class = serializers.RegexField
-    default_serializer_settings = {'allow_blank': False, 'regex': "(Q|q)\d+", 'min_length': 2, 'max_length': 20,
+    default_serializer_settings = {'allow_blank': False, 'regex': r"(Q|q)\d+", 'min_length': 2, 'max_length': 20,
                                    'help_text': "Wikidata Item Identifier (ex. Q59961716)"}
     wikidata_filter = None
 
     def __init__(self, triples, **kwargs):
+        self.triples = triples
         super(WikidataEntityField, self).__init__(**kwargs)
         self.wikidata_filter = " ".join(triple.format(self.entity_name) for triple in triples)
 
     def to_wikidata_filter(self):
         return self.wikidata_filter if self.required else "OPTIONAL {{ {} }}".format(self.wikidata_filter)
 
     def to_wikidata_group(self):
@@ -283,16 +297,16 @@
 
         Args:
             minimal (Optional[Bool]): True if only need ID, label and description, False otherwise
 
         Returns (str):
 
         """
-        return "" if minimal else f"(GROUP_CONCAT(DISTINCT ?{self.name}_item; SEPARATOR='{self.separator}') " \
-                                  f"AS ?{self.name})"
+        return "" if self.use_minimal(minimal) else f"(GROUP_CONCAT(DISTINCT ?{self.name}_item; " \
+                                                     f"SEPARATOR='{self.separator}') AS ?{self.name})"
 
     def to_wikidata_filter(self):
         prop_string = self._prop_sparql_string()
         wd_filter = "?{self.entity_name} {props} ?{self.name}_item .".format(self=self, props=prop_string)
         return wd_filter if self.required else "OPTIONAL {{ {} }}".format(wd_filter)
 
     def to_wikidata_group(self):
@@ -314,16 +328,16 @@
 
         Args:
             minimal (Optional[Bool]): True if only need ID, label and description, False otherwise
 
         Returns (str):
 
         """
-        return "" if minimal else f"(GROUP_CONCAT(DISTINCT ?{self.entity_name}_alt_label; " \
-                                  f"SEPARATOR='{self.separator}') AS ?{self.name})"
+        return "" if self.use_minimal(minimal) else f"(GROUP_CONCAT(DISTINCT ?{self.entity_name}_alt_label; " \
+                                                     f"SEPARATOR='{self.separator}') AS ?{self.name})"
 
     def to_wikidata_filter(self):
         # TODO: add language support in here
         wd_filter = "?{self.entity_name} skos:altLabel ?{self.entity_name}_alt_label ." \
                "FILTER (lang(?{self.entity_name}_alt_label)='en')".format(self=self)
         return wd_filter if self.required else "OPTIONAL {{ {} }}".format(wd_filter)
 
@@ -341,16 +355,16 @@
 
         Args:
             minimal (Optional[Bool]): True if only need ID, label and description, False otherwise
 
         Returns (str):
 
         """
-        return "" if minimal else f"(GROUP_CONCAT(DISTINCT ?{self.name}_itemLabel; " \
-                                  f"SEPARATOR='{self.separator}') AS ?{self.name})"
+        return "" if self.use_minimal(minimal) else f"(GROUP_CONCAT(DISTINCT ?{self.name}_itemLabel; " \
+                                                     f"SEPARATOR='{self.separator}') AS ?{self.name})"
 
     def to_wikidata_service(self):
         return "?{self.name}_item rdfs:label ?{self.name}_itemLabel . ".format(self=self)
 
 
 class SchemaAboutField(WikidataField):
     """ Field used to connect SPARQL to another external resource. """
```

### Comparing `django-wikidata-api-0.0.8/django_wikidata_api/models.py` & `django-wikidata-api-0.0.9/django_wikidata_api/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     """ Base Wikidata Item Model """
     class Meta(object):
         """ Meta options for this model. """
         verbose_name = 'Wikidata Item'
         verbose_name_plural = None
         property_fields = None  # TODO: Make a property_field decorator
 
-    main = WikidataMainEntityField(triples=[], required=True)
-    label = WikidataLabelField(required=True)
-    description = WikidataDescriptionField()
+    main = WikidataMainEntityField(triples=[], required=True, show_in_minimal=True)
+    label = WikidataLabelField(required=True, show_in_minimal=True)
+    description = WikidataDescriptionField(show_in_minimal=True)
     alt_labels = WikidataAltLabelField()
     schema = None
     # Instance Attributes set dynamically:
     id = None
     conformance = WikidataConformanceField()
 
     # dynamically set class attributes:
@@ -250,16 +250,17 @@
 
         """
         if count:
             minimal = True
         fields = cls().get_wikidata_fields()
         to_fields = ' '.join(f.to_wikidata_field(minimal) for f in fields)
         to_filters = ' '.join(f.to_wikidata_filter() for f in fields if f.required or not minimal)
-        to_services = "" if minimal else ' '.join(f.to_wikidata_service() for f in fields)
-        to_group = "" if minimal else f"GROUP BY {' '.join(f.to_wikidata_group() for f in fields)}"
+        to_services = ' '.join(f.to_wikidata_service() for f in fields if not f.use_minimal(minimal)).strip()
+        _to_group_text = ' '.join(f.to_wikidata_group() for f in fields).strip()
+        to_group = f"GROUP BY {_to_group_text}" if _to_group_text else ""
         if values:
             _values = values[offset or 0:]
             if limit:
                 _values = _values[:limit]
             value_filter = "VALUES (?main) {{ (wd:{vals}) }}".format(vals=") (wd:".join(val for val in _values))
             limit_by = ""
             offset_by = ""
@@ -423,14 +424,18 @@
     def __str__(self):
         return "{} ({})".format(self.label, self.main)
 
 
 class WDTriple(object):
     def __init__(self, prop, values, subclass=False, minus=False):
         assert not (len(values) > 1 and minus), "Union and Minus should not be used in the same clause"
+        self.prop_id = prop
         self.prop = "{}/wdt:P279*".format(prop) if subclass else prop
         self.values = values
+        self.subclass = subclass
+        self.minus = minus
+
         query = " UNION ".join(f"{{{{ ?{{name}} wdt:{self.prop} wd:{val}.}}}}" for val in self.values)
         self._query = f"MINUS {query}" if minus else query
 
     def format(self, field_name):
         return self._query.format(name=field_name)
```

### Comparing `django-wikidata-api-0.0.8/django_wikidata_api/serializers.py` & `django-wikidata-api-0.0.9/django_wikidata_api/serializers.py`

 * *Files identical despite different names*

### Comparing `django-wikidata-api-0.0.8/django_wikidata_api/urls.py` & `django-wikidata-api-0.0.9/django_wikidata_api/urls.py`

 * *Files identical despite different names*

### Comparing `django-wikidata-api-0.0.8/django_wikidata_api/utils.py` & `django-wikidata-api-0.0.9/django_wikidata_api/utils.py`

 * *Files identical despite different names*

### Comparing `django-wikidata-api-0.0.8/django_wikidata_api/views.py` & `django-wikidata-api-0.0.9/django_wikidata_api/views.py`

 * *Files identical despite different names*

### Comparing `django-wikidata-api-0.0.8/django_wikidata_api/viewsets.py` & `django-wikidata-api-0.0.9/django_wikidata_api/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-wikidata-api-0.0.8/django_wikidata_api.egg-info/PKG-INFO` & `django-wikidata-api-0.0.9/django_wikidata_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-wikidata-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Package for interfacing with Wikidata within a Django App
 Home-page: https://github.com/kennethsn/django-wikidata-api
 Author: Kenneth Seals-Nutt
 Author-email: kenneth@seals-nutt.com
 License: AGPL-3.0
 Description: # django-wikidata-api
         [![PyPI](https://img.shields.io/pypi/v/django-wikidata-api?style=flat-square)](https://pypi.org/project/django-wikidata-api/)
```

### Comparing `django-wikidata-api-0.0.8/django_wikidata_api.egg-info/SOURCES.txt` & `django-wikidata-api-0.0.9/django_wikidata_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-wikidata-api-0.0.8/setup.py` & `django-wikidata-api-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 README = open(os.path.join(here, 'README.md')).read()
 
 setup(
     name='django-wikidata-api',
-    version='0.0.8',
+    version='0.0.9',
     packages=['django_wikidata_api'],
     description='Python Package for interfacing with Wikidata within a Django App',
     long_description=README,
     long_description_content_type="text/markdown",
     author='Kenneth Seals-Nutt',
     author_email='kenneth@seals-nutt.com',
     url='https://github.com/kennethsn/django-wikidata-api',
```

### Comparing `django-wikidata-api-0.0.8/tox.ini` & `django-wikidata-api-0.0.9/tox.ini`

 * *Files identical despite different names*

