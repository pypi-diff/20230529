# Comparing `tmp/clevertable-2.6.0.tar.gz` & `tmp/clevertable-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clevertable-2.6.0.tar", last modified: Thu May 25 10:08:34 2023, max compression
+gzip compressed data, was "clevertable-3.0.0.tar", last modified: Mon May 29 18:30:31 2023, max compression
```

## Comparing `clevertable-2.6.0.tar` & `clevertable-3.0.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 10:08:34.406273 clevertable-2.6.0/
--rw-rw-rw-   0        0        0     1086 2023-04-21 11:55:46.000000 clevertable-2.6.0/LICENSE
--rw-rw-rw-   0        0        0    34992 2023-05-25 10:08:34.406273 clevertable-2.6.0/PKG-INFO
--rw-rw-rw-   0        0        0    33222 2023-05-24 08:31:40.000000 clevertable-2.6.0/README.md
--rw-rw-rw-   0        0        0     1306 2023-05-25 10:07:33.000000 clevertable-2.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 10:08:34.406273 clevertable-2.6.0/setup.cfg
--rw-rw-rw-   0        0        0      230 2023-04-21 12:00:42.000000 clevertable-2.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:08:34.327043 clevertable-2.6.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 10:08:34.390064 clevertable-2.6.0/src/clevertable/
--rw-rw-rw-   0        0        0     3512 2023-05-24 08:33:41.000000 clevertable-2.6.0/src/clevertable/Binary.py
--rw-rw-rw-   0        0        0      268 2023-05-17 09:40:22.000000 clevertable-2.6.0/src/clevertable/Const.py
--rw-rw-rw-   0        0        0     3016 2023-05-24 04:34:02.000000 clevertable-2.6.0/src/clevertable/ConversionProfile.py
--rw-rw-rw-   0        0        0     3803 2023-05-09 06:20:57.000000 clevertable-2.6.0/src/clevertable/Converter.py
--rw-rw-rw-   0        0        0     4273 2023-05-25 10:05:38.000000 clevertable-2.6.0/src/clevertable/DataFrameProfile.py
--rw-rw-rw-   0        0        0      924 2023-05-03 13:32:15.000000 clevertable-2.6.0/src/clevertable/Enumerate.py
--rw-rw-rw-   0        0        0      258 2023-05-01 13:13:02.000000 clevertable-2.6.0/src/clevertable/Flatten.py
--rw-rw-rw-   0        0        0     3857 2023-05-04 10:30:56.000000 clevertable-2.6.0/src/clevertable/Float.py
--rw-rw-rw-   0        0        0      877 2023-05-01 13:05:29.000000 clevertable-2.6.0/src/clevertable/ForEach.py
--rw-rw-rw-   0        0        0     4948 2023-05-17 10:26:00.000000 clevertable-2.6.0/src/clevertable/Function.py
--rw-rw-rw-   0        0        0      211 2023-05-01 14:33:13.000000 clevertable-2.6.0/src/clevertable/Id.py
--rw-rw-rw-   0        0        0      366 2023-05-01 17:38:30.000000 clevertable-2.6.0/src/clevertable/Ignore.py
--rw-rw-rw-   0        0        0     3018 2023-05-04 06:01:53.000000 clevertable-2.6.0/src/clevertable/Infer.py
--rw-rw-rw-   0        0        0      402 2023-05-24 08:56:57.000000 clevertable-2.6.0/src/clevertable/Label.py
--rw-rw-rw-   0        0        0     3302 2023-05-04 18:08:01.000000 clevertable-2.6.0/src/clevertable/List.py
--rw-rw-rw-   0        0        0     1343 2023-05-03 09:48:28.000000 clevertable-2.6.0/src/clevertable/Map.py
--rw-rw-rw-   0        0        0     1446 2023-05-04 18:08:46.000000 clevertable-2.6.0/src/clevertable/OneHot.py
--rw-rw-rw-   0        0        0     1663 2023-05-24 09:36:41.000000 clevertable-2.6.0/src/clevertable/Parallel.py
--rw-rw-rw-   0        0        0     2872 2023-05-04 05:25:50.000000 clevertable-2.6.0/src/clevertable/Pipeline.py
--rw-rw-rw-   0        0        0     7230 2023-05-24 11:10:15.000000 clevertable-2.6.0/src/clevertable/RecordProfile.py
--rw-rw-rw-   0        0        0      835 2023-05-04 12:11:29.000000 clevertable-2.6.0/src/clevertable/Split.py
--rw-rw-rw-   0        0        0     3370 2023-05-17 10:34:53.000000 clevertable-2.6.0/src/clevertable/StrictFunction.py
--rw-rw-rw-   0        0        0      989 2023-05-04 12:12:21.000000 clevertable-2.6.0/src/clevertable/Strip.py
--rw-rw-rw-   0        0        0     1159 2023-05-17 09:23:55.000000 clevertable-2.6.0/src/clevertable/Transpose.py
--rw-rw-rw-   0        0        0     2751 2023-05-10 15:17:59.000000 clevertable-2.6.0/src/clevertable/Try.py
--rw-rw-rw-   0        0        0      716 2023-05-25 10:07:33.000000 clevertable-2.6.0/src/clevertable/__init__.py
--rw-rw-rw-   0        0        0     1271 2023-05-04 11:54:43.000000 clevertable-2.6.0/src/clevertable/__main__.py
--rw-rw-rw-   0        0        0     2664 2023-05-17 09:41:23.000000 clevertable-2.6.0/src/clevertable/_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:08:34.406273 clevertable-2.6.0/src/clevertable.egg-info/
--rw-rw-rw-   0        0        0    34992 2023-05-25 10:08:34.000000 clevertable-2.6.0/src/clevertable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1044 2023-05-25 10:08:34.000000 clevertable-2.6.0/src/clevertable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 10:08:34.000000 clevertable-2.6.0/src/clevertable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-25 10:08:34.000000 clevertable-2.6.0/src/clevertable.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-05-25 10:08:34.000000 clevertable-2.6.0/src/clevertable.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-25 10:08:34.000000 clevertable-2.6.0/src/clevertable.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 18:30:31.661082 clevertable-3.0.0/
+-rw-rw-rw-   0        0        0     1086 2023-04-21 11:55:46.000000 clevertable-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0    35991 2023-05-29 18:30:31.661082 clevertable-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    34221 2023-05-29 18:29:05.000000 clevertable-3.0.0/README.md
+-rw-rw-rw-   0        0        0     1306 2023-05-29 18:29:58.000000 clevertable-3.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 18:30:31.661082 clevertable-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      230 2023-04-21 12:00:42.000000 clevertable-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 18:30:31.617707 clevertable-3.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 18:30:31.661082 clevertable-3.0.0/src/clevertable/
+-rw-rw-rw-   0        0        0     3518 2023-05-29 17:24:28.000000 clevertable-3.0.0/src/clevertable/Binary.py
+-rw-rw-rw-   0        0        0      268 2023-05-29 17:07:53.000000 clevertable-3.0.0/src/clevertable/Const.py
+-rw-rw-rw-   0        0        0     3016 2023-05-29 17:07:53.000000 clevertable-3.0.0/src/clevertable/ConversionProfile.py
+-rw-rw-rw-   0        0        0     3765 2023-05-29 17:37:25.000000 clevertable-3.0.0/src/clevertable/Converter.py
+-rw-rw-rw-   0        0        0     4367 2023-05-29 17:37:25.000000 clevertable-3.0.0/src/clevertable/DataFrameProfile.py
+-rw-rw-rw-   0        0        0     1018 2023-05-29 18:08:53.000000 clevertable-3.0.0/src/clevertable/Enumerate.py
+-rw-rw-rw-   0        0        0      291 2023-05-29 17:07:53.000000 clevertable-3.0.0/src/clevertable/Flatten.py
+-rw-rw-rw-   0        0        0     3854 2023-05-29 17:24:28.000000 clevertable-3.0.0/src/clevertable/Float.py
+-rw-rw-rw-   0        0        0      896 2023-05-29 17:37:25.000000 clevertable-3.0.0/src/clevertable/ForEach.py
+-rw-rw-rw-   0        0        0     4976 2023-05-29 17:37:25.000000 clevertable-3.0.0/src/clevertable/Function.py
+-rw-rw-rw-   0        0        0      213 2023-05-29 17:07:53.000000 clevertable-3.0.0/src/clevertable/Id.py
+-rw-rw-rw-   0        0        0      369 2023-05-29 17:43:58.000000 clevertable-3.0.0/src/clevertable/Ignore.py
+-rw-rw-rw-   0        0        0     3021 2023-05-29 17:55:13.000000 clevertable-3.0.0/src/clevertable/Infer.py
+-rw-rw-rw-   0        0        0      398 2023-05-29 17:11:23.000000 clevertable-3.0.0/src/clevertable/Label.py
+-rw-rw-rw-   0        0        0     3302 2023-05-29 17:07:53.000000 clevertable-3.0.0/src/clevertable/List.py
+-rw-rw-rw-   0        0        0     1566 2023-05-29 18:13:39.000000 clevertable-3.0.0/src/clevertable/Map.py
+-rw-rw-rw-   0        0        0     1558 2023-05-29 17:59:47.000000 clevertable-3.0.0/src/clevertable/OneHot.py
+-rw-rw-rw-   0        0        0     1830 2023-05-29 17:43:58.000000 clevertable-3.0.0/src/clevertable/Parallel.py
+-rw-rw-rw-   0        0        0     2877 2023-05-29 17:07:53.000000 clevertable-3.0.0/src/clevertable/Pipeline.py
+-rw-rw-rw-   0        0        0     9269 2023-05-29 17:50:54.000000 clevertable-3.0.0/src/clevertable/RecordProfile.py
+-rw-rw-rw-   0        0        0      843 2023-05-29 17:51:55.000000 clevertable-3.0.0/src/clevertable/Split.py
+-rw-rw-rw-   0        0        0     3576 2023-05-29 17:18:36.000000 clevertable-3.0.0/src/clevertable/StrictFunction.py
+-rw-rw-rw-   0        0        0      991 2023-05-29 17:52:36.000000 clevertable-3.0.0/src/clevertable/Strip.py
+-rw-rw-rw-   0        0        0     1194 2023-05-29 17:18:36.000000 clevertable-3.0.0/src/clevertable/Transpose.py
+-rw-rw-rw-   0        0        0     2769 2023-05-29 17:07:53.000000 clevertable-3.0.0/src/clevertable/Try.py
+-rw-rw-rw-   0        0        0      716 2023-05-29 18:29:58.000000 clevertable-3.0.0/src/clevertable/__init__.py
+-rw-rw-rw-   0        0        0     1271 2023-05-29 17:07:53.000000 clevertable-3.0.0/src/clevertable/__main__.py
+-rw-rw-rw-   0        0        0     2501 2023-05-29 17:43:58.000000 clevertable-3.0.0/src/clevertable/_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-29 18:30:31.661082 clevertable-3.0.0/src/clevertable.egg-info/
+-rw-rw-rw-   0        0        0    35991 2023-05-29 18:30:31.000000 clevertable-3.0.0/src/clevertable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1044 2023-05-29 18:30:31.000000 clevertable-3.0.0/src/clevertable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 18:30:31.000000 clevertable-3.0.0/src/clevertable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-29 18:30:31.000000 clevertable-3.0.0/src/clevertable.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2023-05-29 18:30:31.000000 clevertable-3.0.0/src/clevertable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-29 18:30:31.000000 clevertable-3.0.0/src/clevertable.egg-info/top_level.txt
```

### Comparing `clevertable-2.6.0/LICENSE` & `clevertable-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clevertable-2.6.0/PKG-INFO` & `clevertable-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevertable
-Version: 2.6.0
+Version: 3.0.0
 Summary: Low effort conversion of tabular data into numerical values.
 Author: Tom Mohr
 License: MIT License
         
         Copyright (c) 2023 Tom Mohr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -108,14 +108,22 @@
   profile["Column 5"] += OneHot()
   ```
 - After `fit()`, you can access the inferred state of the converters.
   ```python
   my_weather_conv = profile["Weather"]            # e.g. OneHot()
   my_weather_categories = my_weather_conv.values  # e.g. ["sunny", "cloudy", "rainy"]
   ```
+- Send multiple columns into one converter:
+  ```python
+  profile["Column 1", "Column 2"] = max
+  ```
+- Send nested columns into one converter:
+  ```python
+  profile[("Column 1", "Column 2"), "Column 3"] = Parallel(max, min)
+  ```
 
 # Tutorial
 
 Suppose you want to convert the following table of survey results in a 2D numpy array of numbers:
 
 | Country | Age | Diagnosis | Hospitalized | Education level | Symptoms        |
 |---------|-----|-----------|--------------|-----------------|-----------------|
@@ -173,15 +181,15 @@
 
 We can access the individual converters and their properties by indexing the profile with the column name:
 
 ```python
 country_converter = profile["Country"]  # Enumerate('china', 'france', 'germany', ...)
 
 # see which integer corresponds to which country:
-countries_list = country_converter.values  # ['china', 'france', 'germany', ...]
+countries_list = country_converter.values  # ('china', 'france', 'germany', ...)
 ```
 
 You can now use this profile to convert data:
 
 ```python
 # transform the whole table:
 df = profile.transform(table)  # pandas.DataFrame
@@ -420,15 +428,15 @@
 
 | Country | ⇒ | Country |
 |---------|---|---------|
 | france  |   | 0       |
 | italy   |   | 2       |
 | germany |   | 1       |
 
-Their index in the list is used as the numerical value.
+Their index in the argument list is used as the numerical value.
 If no values are specified, the values found in the provided
 data are sorted in lexically ascending order.
 
 ---
 
 ### OneHot
 
@@ -556,29 +564,36 @@
 ```
 
 | Symptoms               | ⇒ | Symptoms=cough | Symptoms=fever | Symptoms=headache |
 |------------------------|---|----------------|----------------|-------------------|
 | fever, cough, headache |   | 1              | 1              | 1                 |
 | headache, cough        |   | 1              | 0              | 1                 |
 
-The default separator for `list` is a comma.<br>
+The default delimiter is a comma.<br>
+You can specify a custom delimiter via the `delimiter` argument:
+
+```python
+"Symptoms": List(delimiter=";")
+"Symptoms": List(delimiter=[",", ";"])  # also accepts lists
+```
+
 The passed strings are interpreted as regular expressions.
 
 ### ListAndOr
 
 ```python
 "Symptoms": ListAndOr()
 ```
 
 | Symptoms                  | ⇒ | Symptoms=cough | Symptoms=fever | Symptoms=headache |
 |---------------------------|---|----------------|----------------|-------------------|
 | fever, cough and headache |   | 1              | 1              | 1                 |
 | headache or cough         |   | 1              | 0              | 1                 |
 
-The default separators for `list_and_or` are comma, "and" and "or".<br>
+The default delimiters are comma, "and" and "or".<br>
 The passed strings are interpreted as regular expressions.
 
 ### Map
 
 ### Strip
 
 ### Split
@@ -623,15 +638,15 @@
 
 ```python
 Parallel(converter1, converter2, ...)
 ```
 
 Apply different converters to the respective items.
 Usually used in a Pipeline after other converters that create outputs with multiple items (e.g. `Split()`).
-Also, you usually want to use `Flatten()` after this, as each individual converter will return a list of items,
+Also, you usually want to use `Flatten()` after this, as each individual converter will return a tuple of items,
 even if it only contains one item.
 Example:
 
 ```python
 "Latitude;Longitude": [
     Split(";"),  # must always result in two items, because Parallel() has 2 converters
     Parallel(Ignore(), Float()),  # ignore latitude, convert longitude to float -> [[], [longitude]]
@@ -680,77 +695,86 @@
 
 ### Label
 
 ### Flatten
 
 ### Transpose
 
-Can transpose nested lists, given that the nested lists are of equal length.
+Can transpose nested tuples, given that the nested tuples are of equal length.
 
 For example, look at this elegant implementation of the [`List()`](#list) converter:
 
 ```python
 "Symptoms": [
     Split(r"\s*,\s*"),  # split at comma
     ForEach(OneHot()),
     Transpose(),
     ForEach(max),
     Flatten()
 ]
 ```
 
 `Transpose()` allows us to apply `max` to each column of the one-hot encodings
-across all list elements.
+across all tuple elements.
 
 ### Function
 
 ```python
 Function(transform, labels=None)
 ```
 
 Shorthand: Instead of `Function(transform, None)`, just write `transform`, where `transform` is some callable.
 
 Creates a custom converter from a custom ``transform()`` function
 (and optionally, a custom ``labels()`` function).
 This is a handy way to create a converter that doesn't need ``fit()``.
 
-Unlike ``StrictFunction()``, this class can handle functions that don't accept or return lists,
+Unlike ``StrictFunction()``, this class can handle functions that don't accept or return tuples,
 which often allows for more concise code.
 
 This is achieved during ``fit()`` as follows:
 
-1. If all incoming items are 1-element lists, it sets a flag ``UNPACK_OUTPUT`` to always
+1. If all incoming items are 1-element tuples, it sets a flag ``UNPACK_OUTPUT`` to always
    unpack the element before passing them to the wrapped function during ``transform()``.
-2. If during ``fit()`` the wrapped function doesn't return lists,
-   it tries to turn that output into a list:
+2. If during ``fit()`` the wrapped function doesn't return tuples,
+   it tries to turn that output into a tuple:
     - If the output is always a non-string iterable, it will simply set a
-      flag ``CONVERT_ITERABLE`` to always convert the iterable output into a list during ``transform()``.
+      flag ``CONVERT_ITERABLE`` to always convert the iterable output into a tuple during ``transform()``.
     - Otherwise, it sets a flag ``WRAP_OUTPUT`` to always wrap the output in a
-      1-element list during ``transform()``.
+      1-element tuple during ``transform()``.
 
 A similar logic is applied to the labels.
 If a custom labels function is given, the following procedure is followed during ``labels()``:
 
-1. If the incoming labels are a 1-element list, the single label is unpacked before
+1. If the incoming labels are a 1-element tuples, the single label is unpacked before
    it is passed to the custom labels function.
-2. If the custom labels function returns something other than a list,
-   this class tries to convert it into a list:
-    - If the output is a non-string iterable, it is converted into a list.
-    - Otherwise, the output is wrapped in a 1-element list.
+2. If the custom labels function returns something other than a tuple,
+   this class tries to convert it into a tuple:
+    - If the output is a non-string iterable, it is converted into a tuple.
+    - Otherwise, the output is wrapped in a 1-element tuple.
 
 If no custom labels function is given, the output labels are generated based on the
 output cardinality inferred during ``fit()`` and according to the following logic:
 
 - If the number of incoming labels is identical to the output cardinality,
   the labels will be returned unchanged.
-- Otherwise, the number of incoming labels must be 1 and the output labels are generated by adding suffixes
-  ``_0``, ``_1``, etc. to the single input label.
+- If there are multiple incoming labels but a single output label,
+  the output label is formed by joining the incoming labels with ``, ``.
+- If there is a single incoming label but multiple output labels,
+  the output labels are formed by adding suffixes ``_0``, ``_1``, etc.
+  to the single input label.
+
+|                    | **1 Output Label** | **M Output Labels**          |
+|--------------------|--------------------|------------------------------|
+| **1 Input Label**  | identical          | suffixes ``_0``, ``_1``, ... |
+| **N Input Labels** | join with ``, ``   | identical if M=N, else ERROR |
 
 A special case are functions returning output of varying cardinality during ``fit()``.
-In this case, a single input label is returned.
+In this case, a single label is returned.
+If only one input label is given, that single label is returned.
 If multiple input labels are given, they are joined with ``_``.
 
 The following example turns a text column into two columns containing the ascii code of the first and last letter.
 
 ```python
 "Name": lambda x: (ord(x[0]), ord(x[-1]))
 ```
@@ -760,80 +784,80 @@
 | Alice |   | 97     | 101    |
 | Bob   |   | 98     | 98     |
 
 (Remember that by default, all text entries are converted to
 lowercase before further processing.)
 
 As you can see, the number of columns is inferred directly from the return value of the conversion function.
-If the function returns a list, the resulting column names are indexed.
+If the function returns a tuple, the resulting column names are indexed.
 
 You can also set the labels explicitly with a lambda function
 that takes the input column name as an argument and returns output column names:
 
 ```python
-"Name": Function(lambda x: [ord(x[0]), ord(x[-1])],
-                 labels=lambda s: [f"ord(first letter of {s})", f"ord(last letter of {s})"]),
+"Name": Function(lambda x: (ord(x[0]), ord(x[-1])),
+                 labels=lambda s: (f"ord(first letter of {s})", f"ord(last letter of {s})")),
 ```
 
 | Name  | ⇒ | ord(first letter of Name) | ord(last letter of Name) |
 |-------|---|---------------------------|--------------------------|
 | Alice |   | 97                        | 101                      |
 | Bob   |   | 98                        | 98                       |
 
 However, remember that you can always simply use [`Label()`](#label) to rename the columns after the conversion,
 if you don't need the output column names to depend on the input column names.
 
 ```python
-"Name": [lambda x: [ord(x[0]), ord(x[-1])],
+"Name": [lambda x: (ord(x[0]), ord(x[-1])),
          Labels("ord(first letter)", "ord(last letter)")],
 ```
 
 ### StrictFunction
 
 ```python
 StrictFunction(transform, labels=None)
 ```
 
 Works mostly like [`Function()`](#function), but simpler:
-``transform`` and ``labels`` must both accept and return lists.
+``transform`` and ``labels`` must both accept and return tuples.
 Instead of something like this:
 
 ```python
 "Name": str.lower,
 ```
 
 you have to write this:
 
 ```python
-"Name": StrictFunction(lambda x: [str.lower(x[0])])
+"Name": StrictFunction(lambda x: (str.lower(x[0]),))  # notice the comma, which makes it a 1-element tuple
 ```
 
-That is, you will still receive 1-element lists as lists to the function,
-even if all input elements during `fit()` are 1-element lists.
-Also, you must now explicitly return a list,
-even if it is just a 1-element list, as otherwise an error will be raised.
+That is, you will still receive 1-element tuples as tuples to the function,
+even if all input elements during `fit()` are 1-element tuples.
+Also, you must now explicitly return a tuple,
+even if it is just a 1-element tuple, as otherwise an error will be raised.
 
 See [`Function()`](#function) for a convenient extension of this converter.
 
 ---
 
 ## Understanding Multi-Column Converters
 
 A converter returns two things:
 
 - `transform()`: the items of the transformed data
 - `labels()`: a label for each item
 
-Both return values are lists.
+Both return values are tuples.
 
 For top-level converters, this then creates the corresponding amount of columns.
 This includes the case of
 
-- a 1-element list `[item]`, which is the case for most converters.
-- an empty list `[]`, in which the result is ignored.
+- a 1-element tuple `(item,)`, which is the case for most converters.
+- an empty tuple `()`, in which the result is ignored.
   (In fact, this is exactly how `Ignore()` is implemented.)
 
 This means, however, that for top-level converters, `labels()` and `transform()`
 must return the same number of items.
 That is because `labels()` is used to create the output column names.
 If `transform()` returns a different number of items, that will raise an error for top-level converters.
```

### Comparing `clevertable-2.6.0/README.md` & `clevertable-3.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,22 @@
   profile["Column 5"] += OneHot()
   ```
 - After `fit()`, you can access the inferred state of the converters.
   ```python
   my_weather_conv = profile["Weather"]            # e.g. OneHot()
   my_weather_categories = my_weather_conv.values  # e.g. ["sunny", "cloudy", "rainy"]
   ```
+- Send multiple columns into one converter:
+  ```python
+  profile["Column 1", "Column 2"] = max
+  ```
+- Send nested columns into one converter:
+  ```python
+  profile[("Column 1", "Column 2"), "Column 3"] = Parallel(max, min)
+  ```
 
 # Tutorial
 
 Suppose you want to convert the following table of survey results in a 2D numpy array of numbers:
 
 | Country | Age | Diagnosis | Hospitalized | Education level | Symptoms        |
 |---------|-----|-----------|--------------|-----------------|-----------------|
@@ -136,15 +144,15 @@
 
 We can access the individual converters and their properties by indexing the profile with the column name:
 
 ```python
 country_converter = profile["Country"]  # Enumerate('china', 'france', 'germany', ...)
 
 # see which integer corresponds to which country:
-countries_list = country_converter.values  # ['china', 'france', 'germany', ...]
+countries_list = country_converter.values  # ('china', 'france', 'germany', ...)
 ```
 
 You can now use this profile to convert data:
 
 ```python
 # transform the whole table:
 df = profile.transform(table)  # pandas.DataFrame
@@ -383,15 +391,15 @@
 
 | Country | ⇒ | Country |
 |---------|---|---------|
 | france  |   | 0       |
 | italy   |   | 2       |
 | germany |   | 1       |
 
-Their index in the list is used as the numerical value.
+Their index in the argument list is used as the numerical value.
 If no values are specified, the values found in the provided
 data are sorted in lexically ascending order.
 
 ---
 
 ### OneHot
 
@@ -519,29 +527,36 @@
 ```
 
 | Symptoms               | ⇒ | Symptoms=cough | Symptoms=fever | Symptoms=headache |
 |------------------------|---|----------------|----------------|-------------------|
 | fever, cough, headache |   | 1              | 1              | 1                 |
 | headache, cough        |   | 1              | 0              | 1                 |
 
-The default separator for `list` is a comma.<br>
+The default delimiter is a comma.<br>
+You can specify a custom delimiter via the `delimiter` argument:
+
+```python
+"Symptoms": List(delimiter=";")
+"Symptoms": List(delimiter=[",", ";"])  # also accepts lists
+```
+
 The passed strings are interpreted as regular expressions.
 
 ### ListAndOr
 
 ```python
 "Symptoms": ListAndOr()
 ```
 
 | Symptoms                  | ⇒ | Symptoms=cough | Symptoms=fever | Symptoms=headache |
 |---------------------------|---|----------------|----------------|-------------------|
 | fever, cough and headache |   | 1              | 1              | 1                 |
 | headache or cough         |   | 1              | 0              | 1                 |
 
-The default separators for `list_and_or` are comma, "and" and "or".<br>
+The default delimiters are comma, "and" and "or".<br>
 The passed strings are interpreted as regular expressions.
 
 ### Map
 
 ### Strip
 
 ### Split
@@ -586,15 +601,15 @@
 
 ```python
 Parallel(converter1, converter2, ...)
 ```
 
 Apply different converters to the respective items.
 Usually used in a Pipeline after other converters that create outputs with multiple items (e.g. `Split()`).
-Also, you usually want to use `Flatten()` after this, as each individual converter will return a list of items,
+Also, you usually want to use `Flatten()` after this, as each individual converter will return a tuple of items,
 even if it only contains one item.
 Example:
 
 ```python
 "Latitude;Longitude": [
     Split(";"),  # must always result in two items, because Parallel() has 2 converters
     Parallel(Ignore(), Float()),  # ignore latitude, convert longitude to float -> [[], [longitude]]
@@ -643,77 +658,86 @@
 
 ### Label
 
 ### Flatten
 
 ### Transpose
 
-Can transpose nested lists, given that the nested lists are of equal length.
+Can transpose nested tuples, given that the nested tuples are of equal length.
 
 For example, look at this elegant implementation of the [`List()`](#list) converter:
 
 ```python
 "Symptoms": [
     Split(r"\s*,\s*"),  # split at comma
     ForEach(OneHot()),
     Transpose(),
     ForEach(max),
     Flatten()
 ]
 ```
 
 `Transpose()` allows us to apply `max` to each column of the one-hot encodings
-across all list elements.
+across all tuple elements.
 
 ### Function
 
 ```python
 Function(transform, labels=None)
 ```
 
 Shorthand: Instead of `Function(transform, None)`, just write `transform`, where `transform` is some callable.
 
 Creates a custom converter from a custom ``transform()`` function
 (and optionally, a custom ``labels()`` function).
 This is a handy way to create a converter that doesn't need ``fit()``.
 
-Unlike ``StrictFunction()``, this class can handle functions that don't accept or return lists,
+Unlike ``StrictFunction()``, this class can handle functions that don't accept or return tuples,
 which often allows for more concise code.
 
 This is achieved during ``fit()`` as follows:
 
-1. If all incoming items are 1-element lists, it sets a flag ``UNPACK_OUTPUT`` to always
+1. If all incoming items are 1-element tuples, it sets a flag ``UNPACK_OUTPUT`` to always
    unpack the element before passing them to the wrapped function during ``transform()``.
-2. If during ``fit()`` the wrapped function doesn't return lists,
-   it tries to turn that output into a list:
+2. If during ``fit()`` the wrapped function doesn't return tuples,
+   it tries to turn that output into a tuple:
     - If the output is always a non-string iterable, it will simply set a
-      flag ``CONVERT_ITERABLE`` to always convert the iterable output into a list during ``transform()``.
+      flag ``CONVERT_ITERABLE`` to always convert the iterable output into a tuple during ``transform()``.
     - Otherwise, it sets a flag ``WRAP_OUTPUT`` to always wrap the output in a
-      1-element list during ``transform()``.
+      1-element tuple during ``transform()``.
 
 A similar logic is applied to the labels.
 If a custom labels function is given, the following procedure is followed during ``labels()``:
 
-1. If the incoming labels are a 1-element list, the single label is unpacked before
+1. If the incoming labels are a 1-element tuples, the single label is unpacked before
    it is passed to the custom labels function.
-2. If the custom labels function returns something other than a list,
-   this class tries to convert it into a list:
-    - If the output is a non-string iterable, it is converted into a list.
-    - Otherwise, the output is wrapped in a 1-element list.
+2. If the custom labels function returns something other than a tuple,
+   this class tries to convert it into a tuple:
+    - If the output is a non-string iterable, it is converted into a tuple.
+    - Otherwise, the output is wrapped in a 1-element tuple.
 
 If no custom labels function is given, the output labels are generated based on the
 output cardinality inferred during ``fit()`` and according to the following logic:
 
 - If the number of incoming labels is identical to the output cardinality,
   the labels will be returned unchanged.
-- Otherwise, the number of incoming labels must be 1 and the output labels are generated by adding suffixes
-  ``_0``, ``_1``, etc. to the single input label.
+- If there are multiple incoming labels but a single output label,
+  the output label is formed by joining the incoming labels with ``, ``.
+- If there is a single incoming label but multiple output labels,
+  the output labels are formed by adding suffixes ``_0``, ``_1``, etc.
+  to the single input label.
+
+|                    | **1 Output Label** | **M Output Labels**          |
+|--------------------|--------------------|------------------------------|
+| **1 Input Label**  | identical          | suffixes ``_0``, ``_1``, ... |
+| **N Input Labels** | join with ``, ``   | identical if M=N, else ERROR |
 
 A special case are functions returning output of varying cardinality during ``fit()``.
-In this case, a single input label is returned.
+In this case, a single label is returned.
+If only one input label is given, that single label is returned.
 If multiple input labels are given, they are joined with ``_``.
 
 The following example turns a text column into two columns containing the ascii code of the first and last letter.
 
 ```python
 "Name": lambda x: (ord(x[0]), ord(x[-1]))
 ```
@@ -723,80 +747,80 @@
 | Alice |   | 97     | 101    |
 | Bob   |   | 98     | 98     |
 
 (Remember that by default, all text entries are converted to
 lowercase before further processing.)
 
 As you can see, the number of columns is inferred directly from the return value of the conversion function.
-If the function returns a list, the resulting column names are indexed.
+If the function returns a tuple, the resulting column names are indexed.
 
 You can also set the labels explicitly with a lambda function
 that takes the input column name as an argument and returns output column names:
 
 ```python
-"Name": Function(lambda x: [ord(x[0]), ord(x[-1])],
-                 labels=lambda s: [f"ord(first letter of {s})", f"ord(last letter of {s})"]),
+"Name": Function(lambda x: (ord(x[0]), ord(x[-1])),
+                 labels=lambda s: (f"ord(first letter of {s})", f"ord(last letter of {s})")),
 ```
 
 | Name  | ⇒ | ord(first letter of Name) | ord(last letter of Name) |
 |-------|---|---------------------------|--------------------------|
 | Alice |   | 97                        | 101                      |
 | Bob   |   | 98                        | 98                       |
 
 However, remember that you can always simply use [`Label()`](#label) to rename the columns after the conversion,
 if you don't need the output column names to depend on the input column names.
 
 ```python
-"Name": [lambda x: [ord(x[0]), ord(x[-1])],
+"Name": [lambda x: (ord(x[0]), ord(x[-1])),
          Labels("ord(first letter)", "ord(last letter)")],
 ```
 
 ### StrictFunction
 
 ```python
 StrictFunction(transform, labels=None)
 ```
 
 Works mostly like [`Function()`](#function), but simpler:
-``transform`` and ``labels`` must both accept and return lists.
+``transform`` and ``labels`` must both accept and return tuples.
 Instead of something like this:
 
 ```python
 "Name": str.lower,
 ```
 
 you have to write this:
 
 ```python
-"Name": StrictFunction(lambda x: [str.lower(x[0])])
+"Name": StrictFunction(lambda x: (str.lower(x[0]),))  # notice the comma, which makes it a 1-element tuple
 ```
 
-That is, you will still receive 1-element lists as lists to the function,
-even if all input elements during `fit()` are 1-element lists.
-Also, you must now explicitly return a list,
-even if it is just a 1-element list, as otherwise an error will be raised.
+That is, you will still receive 1-element tuples as tuples to the function,
+even if all input elements during `fit()` are 1-element tuples.
+Also, you must now explicitly return a tuple,
+even if it is just a 1-element tuple, as otherwise an error will be raised.
 
 See [`Function()`](#function) for a convenient extension of this converter.
 
 ---
 
 ## Understanding Multi-Column Converters
 
 A converter returns two things:
 
 - `transform()`: the items of the transformed data
 - `labels()`: a label for each item
 
-Both return values are lists.
+Both return values are tuples.
 
 For top-level converters, this then creates the corresponding amount of columns.
 This includes the case of
 
-- a 1-element list `[item]`, which is the case for most converters.
-- an empty list `[]`, in which the result is ignored.
+- a 1-element tuple `(item,)`, which is the case for most converters.
+- an empty tuple `()`, in which the result is ignored.
   (In fact, this is exactly how `Ignore()` is implemented.)
 
 This means, however, that for top-level converters, `labels()` and `transform()`
 must return the same number of items.
 That is because `labels()` is used to create the output column names.
 If `transform()` returns a different number of items, that will raise an error for top-level converters.
```

### Comparing `clevertable-2.6.0/pyproject.toml` & `clevertable-3.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clevertable"
-version = "2.6.0"
+version = "3.0.0"
 description = "Low effort conversion of tabular data into numerical values."
 readme = "README.md"
 authors = [{ name = "Tom Mohr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -29,15 +29,15 @@
 [project.urls]
 Homepage = "https://github.com/tom-mohr/clevertable"
 
 [project.scripts]
 clevertable = "clevertable.__main__:main"
 
 [tool.bumpver]
-current_version = "2.6.0"
+current_version = "3.0.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `clevertable-2.6.0/src/clevertable/Binary.py` & `clevertable-3.0.0/src/clevertable/Binary.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             negative = set(negative)  # ensure set
         else:
             negative = {negative}  # wrap single value in set
 
         self.positive: set = positive
         self.negative: set = negative
 
-    def fit(self, rows: list[list]):
+    def fit(self, rows: list[tuple]):
         if self.positive or self.negative:
             # at least either one positive or negative value was passed to the constructor,
             # -> no need to infer them from the data
             return
 
         values = [row[0] for row in rows]  # unpack 1-element rows
 
@@ -62,25 +62,25 @@
             self.negative = common_negative
             return
 
         # at this point, there are some values that we don't know whether they are positive or negative
         # -> simply pick the lexically smallest value as negative
         self.negative = {sorted(values)[0]}
 
-    def transform(self, row: list) -> list:
-        val = row[0]  # unpack 1-element list
+    def transform(self, row: tuple) -> tuple:
+        val = row[0]  # unpack 1-element tuple
 
         if self.positive and self.negative:
             # ensure the value is either in positive or in negative
             if val not in self.positive and val not in self.negative:
                 raise ValueError(f"Value '{val}' is neither in the positive nor in the negative values.")
         if self.positive:
-            return [int(val in self.positive)]
+            return (int(val in self.positive),)
         else:
-            return [1 - int(val in self.negative)]
+            return (1 - int(val in self.negative),)
 
     def __repr__(self):
         args = []
         if self.__args_positive is not None:
             args.append(f"positive={repr(self.__args_positive)}")
         if self.__args_negative is not None:
             args.append(f"negative={repr(self.__args_negative)}")
```

### Comparing `clevertable-2.6.0/src/clevertable/ConversionProfile.py` & `clevertable-3.0.0/src/clevertable/ConversionProfile.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.6.0/src/clevertable/Converter.py` & `clevertable-3.0.0/src/clevertable/Converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,63 +4,62 @@
 
 
 class Converter(ABC):
     """
     Base class for all converters.
     A converter is used to convert a single column of data into one or multiple columns of data."""
 
-    def fit(self, rows: list[list]):
+    def fit(self, rows: list[tuple]):
         """The converter is presented representative sample data.
         In this method, the converter should adapt its internal state so that there will
         be no errors when transform() is called with the same data.
         Implementations of this method can make the following assumptions:
 
         - The given list of values contains at least one element.
         - This method will only be called once per instance.
         """
         pass
 
-    def labels(self, labels: list) -> list:
+    def labels(self, labels: tuple) -> tuple:
         """Returns the labels that should be associated with the output data of this converter.
         For top-level converters, this will result in the names of the output columns.
         If the converter only results in one output column, this method should still return the
-        name of the output column as a 1-element list.
+        name of the output column as a 1-element tuple.
 
         This method can be called as soon this converter's fit() method has been called.
 
         For converters for which the values returned by transform() vary in size even after fit() was called,
-        this method can simply return a list of labels whose length matches the length of one possible output.
-        This could for example simply be a one-element list.
+        this method can simply return a tuple of labels whose length matches the length of one possible output.
+        This could for example simply be a one-element tuple.
         If these converters are not used as top-level converters, this is not a problem if other converters
         handle this output further and ensure a constant output size.
 
         If top-level converters return labels with identical names,
         the duplicated names will be made unique, e.g. by appending an index number.
 
         By default, this method simply returns the given labels unchanged.
 
         :param labels: The labels of the input data.
-                       For top-level converters, this is a 1-element list containing the name of the
+                       For top-level converters, this is a 1-element tuple containing the name of the
                        original column that will be converted.
         """
         return labels
 
     @abstractmethod
-    def transform(self, row: list) -> list:
+    def transform(self, row: tuple) -> tuple:
         """
-        Transforms a list of input values into a list of output values.
-        Input and output may be of different size, but they must be lists.
-        I.e. if the input is a single value, it will still be passed to this method as a 1-element list.
-        If the output is a single value, it must still be returned as a 1-element list.
+        Transforms a tuple of input values into a tuple of output values.
+        Input and output may be of different size, but they must be tuples.
+        I.e. if the input is a single value, it will still be passed to this method as a 1-element tuple.
+        If the output is a single value, it must still be returned as a 1-element tuple.
 
-        For top-level converters, the input will always be a 1-element list,
-        and the size of the output will determine the number of columns in the converted table
+        For top-level converters, the length of the output will determine the number of columns in the converted table
         resulting from this converter.
 
-        :param row: List of values to be converted. Single values will be passed as 1-element lists.
+        :param row: Tuple of values to be converted. Single values will be passed as 1-element tuples.
         """
         raise NotImplementedError()
 
     def __repr__(self):
         """
         Returns a string representation of this converter.
         If possible, this should be a string that can be used to create a new instance.
```

### Comparing `clevertable-2.6.0/src/clevertable/DataFrameProfile.py` & `clevertable-3.0.0/src/clevertable/DataFrameProfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from textwrap import indent
 from typing import Callable, Optional
 
 import pandas as pd
 
 from .RecordProfile import RecordProfile
 
 
@@ -35,35 +36,36 @@
         """
         Fit the profile to the given DataFrame.
         :param df: The DataFrame to fit to.
         :return: self
         """
         dicts = df.to_dict(orient="records")
         dicts = [self.__pre_process_dict(d) for d in dicts]  # pre-process each dict
-        rows = [[d] for d in dicts]  # wrap each dict in a 1-element list
+        rows = [(d,) for d in dicts]  # wrap each dict in a 1-element tuple
 
         self._record_profile.fit(rows)
 
         return self
 
     def transform(self, df: pd.DataFrame) -> pd.DataFrame:
         dicts = df.to_dict(orient="records")
         transformed_dicts = []
         for i, d in enumerate(dicts):
             try:
                 d = self.transform_single(d)
             except Exception as e:
                 # add helpful context to error message
-                raise Exception(f"Error during transform() of row {i}: {e}") from e
+                raise Exception(f"Error during transform() of row {i}:\n"
+                                f"{indent(str(e), ' ' * 4)}") from e
             transformed_dicts.append(d)
         return pd.DataFrame.from_records(transformed_dicts)
 
     def transform_single(self, row: dict[str, any]) -> dict[str, any]:
         row = self.__pre_process_dict(row)
-        return self._record_profile.transform([row])[0]  # wrap, transform, and unpack again
+        return self._record_profile.transform((row,))[0]  # wrap, transform, and unpack again
 
     def fit_transform(self, df: pd.DataFrame) -> pd.DataFrame:
         self.fit(df)
         return self.transform(df)
 
     def update(self, profile: dict[str, any]) -> 'DataFrameProfile':
         """
@@ -71,18 +73,18 @@
         :param profile: A dictionary that maps column names to converters.
         :return: self
         """
         self._record_profile.update(profile)
         return self
 
     @property
-    def column_names(self) -> dict[str, list]:
+    def column_names(self) -> dict[any, tuple]:
         """
         A dictionary that maps input column names to output column names.
-        Note that the output column names are lists, even if there is only a single
+        Note that the output column names are tuples, even if there is only a single
         output column for the respective input column.
         """
         return self._record_profile.keys
 
     def __pre_process_dict(self, d: dict[str, any]) -> dict[str, any]:
         return {k: self.__pre_process(v) for k, v in d.items()}
```

### Comparing `clevertable-2.6.0/src/clevertable/Float.py` & `clevertable-3.0.0/src/clevertable/Float.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
         self.__default_value = default
 
     @property
     def default(self):
         return self.__default_value
 
-    def fit(self, rows: list[list]):
+    def fit(self, rows: list[tuple]):
 
         values = [row[0] for row in rows]  # unpack 1-element rows
 
         if self.__default_value in ("mean", "median", "mode"):
             # replace default value with the corresponding number
 
             # collect all numbers that can be parsed
@@ -87,27 +87,27 @@
                 self.__default_value = float(mean(parsed_values))
             elif self.__default_value == "median":
                 self.__default_value = float(median(parsed_values))
             elif self.__default_value == "mode":
                 mode_, count = mode(parsed_values, keepdims=False)
                 self.__default_value = float(mode_)
 
-    def transform(self, row: list) -> list:
-        val = row[0]  # unpack 1-element list
-        number = _try_float(val)
-        if number is not None:
-            return [number]
+    def transform(self, row: tuple) -> tuple:
+        val = row[0]  # unpack 1-element tuple
+        num = _try_float(val)
+        if num is not None:
+            return (num,)
 
         # conversion / parsing failed.
         # ensure that a usable default value exists
         if self.__default_value is None:
             raise ValueError(f"Cannot transform value '{val}' to float,"
                              f" because parsing failed and no default value was specified.")
         if self.__default_value in ("mean", "median", "mode"):
             raise ValueError(f"You must call fit() before transform().")
 
-        return [self.__default_value]
+        return (self.__default_value,)
 
     def __repr__(self):
         if self.__default_value is None:
             return "Float()"
         return f"Float(default={repr(self.__default_value)})"
```

### Comparing `clevertable-2.6.0/src/clevertable/Function.py` & `clevertable-3.0.0/src/clevertable/Function.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 
     def __init__(self, transform: callable, labels: Callable[[any], any] = None):
         """
         Creates a custom converter from a custom ``transform()`` function
         (and optionally, a custom ``labels()`` function).
         This is a handy way to create a converter that doesn't implement ``fit()`` (i.e. doesn't have a state).
 
-        Unlike ``StrictFunction``, this class can handle functions that don't accept or return lists,
+        Unlike ``StrictFunction``, this class can handle functions that don't accept or return tuples,
         which often allows for more concise code.
 
         This is achieved during ``fit()`` as follows:
 
-        1. If all incoming items are 1-element lists, it sets a flag ``UNPACK_OUTPUT`` to always
+        1. If all incoming items are 1-element tuples, it sets a flag ``UNPACK_OUTPUT`` to always
            unpack the element before passing them to the wrapped function during ``transform()``.
-        2. If during ``fit()`` the wrapped function doesn't return lists,
-           it tries to turn that output into a list:
+        2. If during ``fit()`` the wrapped function doesn't return tuples,
+           it tries to turn that output into a tuple:
             - If the output is always a non-string iterable, it will simply set a
-              flag ``CONVERT_ITERABLE`` to always convert the iterable output into a list during ``transform()``.
+              flag ``CONVERT_ITERABLE`` to always convert the iterable output into a tuple during ``transform()``.
             - Otherwise, it sets a flag ``WRAP_OUTPUT`` to always wrap the output in a
-              1-element list during ``transform()``.
+              1-element tuple during ``transform()``.
 
         A similar logic is applied to the labels.
         See :class:`StrictFunction` for details.
 
         :param transform: The function to wrap. Turns input into output.
         :param labels: Turns incoming labels into output labels.
         """
@@ -39,80 +39,80 @@
         self.__transform = transform
         self.__labels = labels
 
         self._unpack_single_input: bool = None
         self._convert_iterable_output: bool = None
         self._wrap_output: bool = None
 
-    def __fixed_transform(self, row: list) -> list:
+    def __fixed_transform(self, row: tuple) -> tuple:
         row = self.__input_processing(row)
         row = self.__transform(row)
         row = self.__output_processing(row)
         return row
 
-    def __fixed_labels(self, labels: list) -> list:
+    def __fixed_labels(self, labels: tuple) -> tuple:
         # should only be called if given labels func is not None
 
         if len(labels) == 1:
-            labels = labels[0]  # unpack 1-element list
+            labels = labels[0]  # unpack 1-element tuples
 
         labels = self.__labels(labels)
 
-        if isinstance(labels, list):
+        if isinstance(labels, tuple):
             return labels
-        # turn the output into a list:
+        # turn the output into a tuple:
         if isinstance(labels, Iterable) and not isinstance(labels, str):  # non-string iterable
-            return list(labels)
-        return [labels]  # wrap single values
+            return tuple(labels)
+        return (labels,)  # wrap single values
 
-    def fit(self, rows: list[list]):
+    def fit(self, rows: list[tuple]):
         self.__set_flags(rows)
         super().fit(rows)
 
-    def __set_flags(self, rows: list[list]):
+    def __set_flags(self, rows: list[tuple]):
         """
         This method looks at the fit data and determines how the input and output must be processed
         during ``transform()`` in order to make the wrapped function work.
         """
-        # infer from data: unpack if the input is always a 1-element list
-        self._unpack_single_input = all(isinstance(row, list) and len(row) == 1 for row in rows)
+        # infer from data: unpack if the input is always a 1-element tuple
+        self._unpack_single_input = all(isinstance(row, tuple) and len(row) == 1 for row in rows)
 
         # apply input processing accordingly
         rows = [self.__input_processing(row)
                 for row in rows]
 
         # transform data with func
         rows = [self.__transform(row) for row in rows]
 
         self._convert_iterable_output = False
         self._wrap_output = False
-        if not all(isinstance(o, list) for o in rows):
-            # turn the output into a list:
+        if not all(isinstance(o, tuple) for o in rows):
+            # turn the output into a tuple:
             if all(isinstance(o, Iterable) and not isinstance(o, str) for o in rows):  # non-string iterables
                 self._convert_iterable_output = True
             else:
                 self._wrap_output = True
 
-    def __input_processing(self, row: list) -> any:
+    def __input_processing(self, row: tuple) -> any:
         if self._unpack_single_input:
             assert len(row) == 1, \
                 f"Function {self.__transform.__name__} expects a single value, but got {len(row)}!"
             return row[0]
         return row
 
-    def __output_processing(self, output: any) -> list:
+    def __output_processing(self, output: any) -> tuple:
         if self._wrap_output:
-            return [output]
+            return (output,)
         if self._convert_iterable_output:
             assert isinstance(output, Iterable) and not isinstance(output, str), \
                 f"Function {self.__transform.__name__} did not return" \
                 f" a non-string iterable: {repr(output)}"
-            return list(output)
-        assert isinstance(output, list), \
-            f"Function {self.__transform.__name__} did not return a list: {repr(output)}"
+            return tuple(output)
+        assert isinstance(output, tuple), \
+            f"Function {self.__transform.__name__} did not return a tuple: {repr(output)}"
         return output
 
     def __repr__(self):
         if self.__labels is None:
             # callables are parsed to Function()
             return self.__transform.__name__
         return f"Function({self.__transform.__name__}, {self.__labels.__name__})"
```

### Comparing `clevertable-2.6.0/src/clevertable/Infer.py` & `clevertable-3.0.0/src/clevertable/Infer.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,54 +15,54 @@
 
     def __repr__(self):
         return repr(self.inferred)
 
     def __getitem__(self, item):
         return self.inferred[item]
 
-    def fit(self, rows: list[list]):
+    def fit(self, rows: list[tuple]):
         """
         Tries to infer this converter from the given data.
         If a converter could be inferred, it is fitted with the data and stored in self.inferred.
         :raises ValueError: if no converter can be inferred and ignore_uninferrable is False
         """
         try:
             self.inferred = _infer_converter_from_data(rows)
         except ValueError as e:
             if self.ignore_uninferrable:
                 self.inferred = Ignore()
             raise e
         self.inferred.fit(rows)
 
-    def labels(self, labels: list) -> list:
+    def labels(self, labels: tuple) -> tuple:
         return self.inferred.labels(labels)
 
-    def transform(self, row: list) -> list:
+    def transform(self, row: tuple) -> tuple:
         return self.inferred.transform(row)
 
 
-def _infer_converter_from_data(rows: list[list]) -> Converter:
+def _infer_converter_from_data(rows: list[tuple]) -> Converter:
     """Tries to infer the best converter from the given data.
     If no converter can be inferred, a ValueError is raised."""
     # dynamic imports in order to break circular dependency
     from .Binary import Binary
     from .Enumerate import Enumerate
     from .Float import Float
     from .Float import _try_float
     from .List import List, ListAndOr
     from .OneHot import OneHot
 
-    # if only contains 1-element lists
+    # if only contains 1-element rows:
     if all(len(row) == 1 for row in rows):
 
         values = [row[0] for row in rows]  # unpack 1-element rows
 
         # if only contains numbers:
-        if all([isinstance(val, numbers.Number) or val in (None, "") or _try_float(val) is not None
-                for val in values]):
+        if all(isinstance(val, numbers.Number) or val in (None, "") or _try_float(val) is not None
+               for val in values):
             return Float()
 
         # since numerical approach failed,
         # we now try categorical approaches
         string_values = [val for val in values if isinstance(val, str)]
 
         # check if it can be split according to List()
```

### Comparing `clevertable-2.6.0/src/clevertable/List.py` & `clevertable-3.0.0/src/clevertable/List.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.6.0/src/clevertable/Map.py` & `clevertable-3.0.0/src/clevertable/Map.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,30 +5,34 @@
 
 class Map(Converter):
 
     def __init__(self, lookup_table: dict, default=None):
         """
         Converts values according to a lookup table.
         If the value is not found in the lookup table, the default value is returned.
-        Values may be single values or lists of values.
+        Values may be single values or tuples of values.
         """
         if len(lookup_table) == 0:
             raise ValueError("Empty lookup table is not allowed.")
-        # if any value is not a list, convert all values to a list
-        if any(not isinstance(val, list) for val in lookup_table.values()):
-            lookup_table = {key: [val] for key, val in lookup_table.items()}
-        self.lookup_table = lookup_table
-        self.default_value = default
+        # if any value is not a tuple, convert all values to a 1-element tuple
+        if any(not isinstance(val, tuple) for val in lookup_table.values()):
+            lookup_table = {key: (val,) for key, val in lookup_table.items()}
+        self.lookup_table: dict[any, tuple] = lookup_table
 
-    def transform(self, row: list) -> list:
+        self.__default_arg = default  # save original arg for repr()
+        if default is not None and not isinstance(default, tuple):
+            default = (default,)
+        self.default_value: tuple | None = default
+
+    def transform(self, row: tuple) -> tuple:
         val = row[0]
         if val in self.lookup_table:
             return self.lookup_table[val]
         if self.default_value is not None:
             return self.default_value
         raise KeyError(f"Value '{val}' not found in lookup table and no default value is specified.")
 
     def __repr__(self):
-        if self.default_value is None:
+        if self.__default_arg is None:
             return repr(self.lookup_table)
         else:
-            return f"Map({repr(self.lookup_table)}, default={repr(self.default_value)})"
+            return f"Map({repr(self.lookup_table)}, default={repr(self.__default_arg)})"
```

### Comparing `clevertable-2.6.0/src/clevertable/Parallel.py` & `clevertable-3.0.0/src/clevertable/Parallel.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,33 +9,35 @@
         """
         Apply multiple converters to the respective elements of the input.
         During fit(), top-level Infer() converters are replaced with the inferred converter.
         :param converters: The converters in the same order as the input elements which they should be applied to.
         """
         self.converters = [_parse_converter(conv) for conv in converters]
 
-    def fit(self, rows: list[list]):
+    def fit(self, rows: list[tuple]):
 
         # transpose rows
         cols = list(zip(*rows))
 
         for conv, col in zip(self.converters, cols):
-            values = [[val] for val in col]  # each row must be a list
+            values = [(val,) for val in col]  # each row must be a tuple
             conv.fit(values)
 
         # replace all Infer converters with the nested inferred converter
         for i, conv in enumerate(self.converters):
             if isinstance(conv, Infer):
                 assert conv.inferred is not None, \
                     f"Infer() converter at index {i} did not infer a converter during fit()"
                 self.converters[i] = conv.inferred
 
-    def labels(self, labels: list) -> list:
+    def labels(self, labels: tuple) -> tuple:
+        assert isinstance(labels, tuple)
         assert len(labels) == len(self.converters)
-        return [conv.labels([label]) for label, conv in zip(labels, self.converters)]
+        return tuple(conv.labels((label,)) for label, conv in zip(labels, self.converters))
 
-    def transform(self, row: list) -> list:
-        assert len(row) == len(self.converters)
-        return [conv.transform([val]) for val, conv in zip(row, self.converters)]
+    def transform(self, row: tuple) -> tuple:
+        assert len(row) == len(self.converters), \
+            f"Parallel converter expected {len(self.converters)} elements, but got {len(row)}: {row}"
+        return tuple(conv.transform((val,)) for val, conv in zip(row, self.converters))
 
     def __repr__(self):
         return f"Parallel({', '.join(repr(conv) for conv in self.converters)})"
```

### Comparing `clevertable-2.6.0/src/clevertable/Pipeline.py` & `clevertable-3.0.0/src/clevertable/Pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 
 class _Pipeline(Converter):
 
     def __init__(self, first: any, second: any):
         self.first = _parse_converter(first)
         self.second = _parse_converter(second)
 
-    def fit(self, rows: list[list]):
+    def fit(self, rows: list[tuple]):
         self.first.fit(rows)
         self.second.fit([self.first.transform(row) for row in rows])
 
         # replace Infer() converters with the nested inferred converter
         if isinstance(self.first, Infer):
             assert self.first.inferred is not None, \
                 f"Infer() converter for did not infer a converter during fit()"
             self.first = self.first.inferred
         if isinstance(self.second, Infer):
             assert self.second.inferred is not None, \
                 f"Infer() converter for did not infer a converter during fit()"
             self.second = self.second.inferred
 
-    def labels(self, labels: list) -> list:
+    def labels(self, labels: tuple) -> tuple:
         return self.second.labels(self.first.labels(labels))
 
-    def transform(self, row: list) -> list:
+    def transform(self, row: tuple) -> tuple:
         return self.second.transform(self.first.transform(row))
 
     def __repr__(self):
         return f"{self.__class__.__name__}({repr(self.first)}, {repr(self.second)})"
 
 
 class Pipeline(_Pipeline):
```

### Comparing `clevertable-2.6.0/src/clevertable/Split.py` & `clevertable-3.0.0/src/clevertable/Split.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,17 +15,17 @@
         if not delimiters:
             delimiters = _DEFAULT_SPLITS
             self.__default_args = True
         else:
             self.__default_args = False
         self.regex = "|".join(delimiters)
 
-    def transform(self, row: list) -> list[str]:
-        val = row[0]  # unpack 1-element list
+    def transform(self, row: tuple) -> tuple[str]:
+        val = row[0]  # unpack 1-element row
         if not isinstance(val, str):
             raise ValueError(f"Split() can only be applied to strings, not to value of type {type(val)}: {val}")
-        return re.split(self.regex, val)
+        return tuple(re.split(self.regex, val))
 
     def __repr__(self):
         if self.__default_args:
             return "Split()"
         return f"Split({repr(self.regex)})"
```

### Comparing `clevertable-2.6.0/src/clevertable/StrictFunction.py` & `clevertable-3.0.0/src/clevertable/StrictFunction.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,65 +14,70 @@
         For a converter that accepts more general functions, see ``Function``.
 
         If no custom labels function is given, the output labels are generated based on the
         output cardinality inferred during ``fit()`` and according to the following logic:
 
         - If the number of incoming labels is identical to the output cardinality,
           the labels will be returned unchanged.
-        - Otherwise, the number of incoming labels must be 1 and the output labels are generated by adding suffixes
-          ``_0``, ``_1``, etc. to the single input label.
+        - If there are multiple incoming labels but a single output label,
+          the output label is formed by joining the incoming labels with ``, ``.
+        - If there is a single incoming label but multiple output labels,
+          the output labels are formed by adding suffixes ``_0``, ``_1``, etc.
+          to the single input label.
 
         A special case are functions returning output of varying cardinality during ``fit()``.
-        In this case, a single input label is returned.
+        In this case, a single label is returned.
+        If only one input label is given, that single label is returned.
         If multiple input labels are given, they are joined with ``_``.
 
         :param transform: The function to wrap. Turns input into output.
         :param labels: Turns incoming labels into output labels.
         """
         self._transform = transform
         self._labels = labels
 
         self._output_cardinality: int = None
 
-    def fit(self, rows: list[list]):
+    def fit(self, rows: list[tuple]):
         # infer output cardinality (only needed if no labels function is given)
         if self._labels is None:
             rows = [self._transform(row) for row in rows]
             self._output_cardinality = len(rows[0])
 
             # check if output cardinality varies:
             if not all(len(row) == self._output_cardinality for row in rows):
                 self._output_cardinality = -1  # a value of -1 represents varying output cardinality
                 return
 
-    def transform(self, row: list) -> list:
+    def transform(self, row: tuple) -> tuple:
         return self._transform(row)
 
-    def labels(self, labels: list) -> list:
-        if self._labels is None:
+    def labels(self, labels: tuple) -> tuple:
+        if self._labels is not None:
+            return self._labels(labels)  # use custom labels function
+
+        if self._output_cardinality == -1:  # -1 represents varying output cardinality
+            s = ", ".join(str(x) for x in labels)
+            return (s,)
+
+        if len(labels) == self._output_cardinality:
+            return labels
 
-            if self._output_cardinality == -1:
-                # -1 represents varying output cardinality
-                return ["_".join(labels)]
-
-            if len(labels) == self._output_cardinality:
-                return labels
-
-            # generate label names:
-
-            if self._output_cardinality == 0:
-                # can do this even for len(labels) != 1
-                return []
-            assert len(labels) == 1, \
-                f"The needed {self._output_cardinality} labels for function {self._transform.__name__}" \
-                f"can only be generated from a single input label, but received {repr(labels)}."
+        if self._output_cardinality == 0:
+            return ()
+
+        if self._output_cardinality == 1:
+            s = ", ".join(str(x) for x in labels)
+            return (s,)
+
+        if len(labels) == 1:
             label = labels[0]
-            return [f"{label}_{i}" for i in range(self._output_cardinality)]
-        else:
-            # use custom labels function
-            return self._labels(labels)
+            return tuple(f"{label}_{i}" for i in range(self._output_cardinality))
+
+        raise ValueError(f"Cannot generate {self._output_cardinality} output labels"
+                         f" from {len(labels)} input labels: {repr(labels)}")
 
     def __repr__(self):
         args = [self._transform.__name__]
         if self._labels is not None:
             args.append(self._labels.__name__)
         return f"StrictFunction({', '.join(args)})"
```

### Comparing `clevertable-2.6.0/src/clevertable/Strip.py` & `clevertable-3.0.0/src/clevertable/Strip.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
         # remove whole substring either at the end or beginning
         prefixes = map(lambda s: f'^{s}', strip)
         suffixes = map(lambda s: f'{s}$', strip)
         fixes = list(prefixes) + list(suffixes)
         self.regex = "|".join(fixes)
 
-    def transform(self, row: list) -> list:
-        val = row[0]  # unpack 1-element list
+    def transform(self, row: tuple) -> tuple:
+        val = row[0]  # unpack 1-element row
         if not isinstance(val, str):
             raise ValueError(f"Strip() can only be applied to strings, not to value of type {type(val)}: {val}")
-        return [re.sub(self.regex, "", val)]
+        return (re.sub(self.regex, "", val),)
 
     def __repr__(self):
         if self.__default_args:
             return "Strip()"
         return f"Strip({repr(self.regex)})"
```

### Comparing `clevertable-2.6.0/src/clevertable/Try.py` & `clevertable-3.0.0/src/clevertable/Try.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,24 +17,24 @@
         """
         if exceptions is None:
             self.exceptions = (Exception,)
         else:
             self.exceptions = tuple(exceptions)
         self.converters = [_parse_converter(conv) for conv in converters]
 
-    def fit(self, rows: list[list]):
+    def fit(self, rows: list[tuple]):
         convs = list(self.converters)
         while convs:
             conv = convs.pop(0)
             conv.fit(rows)
 
             if not convs:
                 return  # no need to transform with last converter
 
-            next_rows = []  # values that raise an exception
+            next_rows: list[tuple] = []  # values that raise an exception
             for row in rows:
                 try:
                     conv.transform(row)
                 except Exception as e:
                     if not isinstance(e, self.exceptions):
                         raise e
                     next_rows.append(row)
@@ -47,20 +47,20 @@
         # replace Infer() converters with the nested inferred converter
         for i, conv in enumerate(self.converters):
             if isinstance(conv, Infer):
                 assert conv.inferred is not None, \
                     f"Infer() converter for did not infer a converter during fit()"
                 self.converters[i] = conv.inferred
 
-    def labels(self, labels: list) -> list:
+    def labels(self, labels: tuple) -> tuple:
         if self.converters:
             return self.converters[0].labels(labels)
         return labels
 
-    def transform(self, row: list) -> list:
+    def transform(self, row: tuple) -> tuple:
         for conv in self.converters:
             try:
                 return conv.transform(row)
             except Exception as e:
                 if not isinstance(e, self.exceptions):
                     raise e
         return row
```

### Comparing `clevertable-2.6.0/src/clevertable/__init__.py` & `clevertable-3.0.0/src/clevertable/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.6.0"
+__version__ = "3.0.0"
 
 from .Binary import Binary
 from .Const import Const
 from .ConversionProfile import ConversionProfile
 from .Converter import Converter
 from .Enumerate import Enumerate
 from .Flatten import Flatten
```

### Comparing `clevertable-2.6.0/src/clevertable/__main__.py` & `clevertable-3.0.0/src/clevertable/__main__.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.6.0/src/clevertable/_utils.py` & `clevertable-3.0.0/src/clevertable/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,43 +37,36 @@
     if type(obj) is str:  # strings are iterable, but we don't want to split them into characters
         return [obj]
     if isinstance(obj, Iterable):
         return list(obj)
     return [obj]
 
 
-def _replace_none_recursively(obj: any, replacement: any) -> any:
-    # only works for lists!
-    if obj is None:
-        return replacement
-    if isinstance(obj, list):
-        return [_replace_none_recursively(o, replacement) for o in obj]
-    return obj
-
-
-def _index_duplicates(labels: list[str], index_func: Callable[[str, int], str]) -> list[str]:
+def _index_duplicates(labels: tuple[str], index_func: Callable[[str, int], str]) -> tuple[str]:
     """
     Add index suffix to all duplicate strings.
     This is done repeatedly until no duplicates are left,
     i.e. the returned list is guaranteed to have no duplicates.
-    :param labels: List of strings, may contain duplicates.
+    :param labels: Tuple of strings, may contain duplicates.
     :param index_func: (label, occurrence_count) -> new_label
     :return:
     """
     if len(labels) == 1:
         return labels
     # add index suffix to all duplicate strings
     # e.g. ["apple", "banana", "apple"] -> ["apple_1", "banana", "apple_2"]
     # for complete safety, repeat this until no duplicates are left
     while len(set(labels)) != len(labels):  # while duplicates are present
         counts = {label: labels.count(label) for label in set(labels)}
         occurrence_count = {label: 0 for label in set(labels)}
+        labels = list(labels)  # need write access
         for i, label in enumerate(labels):
             count = counts[label]
             occurrence_count[label] += 1
             if count > 1:
                 labels[i] = index_func(label, occurrence_count[label])
+        labels = tuple(labels)
     return labels
 
 
-def _flatten(list_of_lists: list[list]) -> list:
-    return [e for inner_list in list_of_lists for e in inner_list]
+def _flatten_tuples(tuple_of_tuples: tuple[tuple]) -> tuple:
+    return tuple(e for inner_list in tuple_of_tuples for e in inner_list)
```

### Comparing `clevertable-2.6.0/src/clevertable.egg-info/PKG-INFO` & `clevertable-3.0.0/src/clevertable.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevertable
-Version: 2.6.0
+Version: 3.0.0
 Summary: Low effort conversion of tabular data into numerical values.
 Author: Tom Mohr
 License: MIT License
         
         Copyright (c) 2023 Tom Mohr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -108,14 +108,22 @@
   profile["Column 5"] += OneHot()
   ```
 - After `fit()`, you can access the inferred state of the converters.
   ```python
   my_weather_conv = profile["Weather"]            # e.g. OneHot()
   my_weather_categories = my_weather_conv.values  # e.g. ["sunny", "cloudy", "rainy"]
   ```
+- Send multiple columns into one converter:
+  ```python
+  profile["Column 1", "Column 2"] = max
+  ```
+- Send nested columns into one converter:
+  ```python
+  profile[("Column 1", "Column 2"), "Column 3"] = Parallel(max, min)
+  ```
 
 # Tutorial
 
 Suppose you want to convert the following table of survey results in a 2D numpy array of numbers:
 
 | Country | Age | Diagnosis | Hospitalized | Education level | Symptoms        |
 |---------|-----|-----------|--------------|-----------------|-----------------|
@@ -173,15 +181,15 @@
 
 We can access the individual converters and their properties by indexing the profile with the column name:
 
 ```python
 country_converter = profile["Country"]  # Enumerate('china', 'france', 'germany', ...)
 
 # see which integer corresponds to which country:
-countries_list = country_converter.values  # ['china', 'france', 'germany', ...]
+countries_list = country_converter.values  # ('china', 'france', 'germany', ...)
 ```
 
 You can now use this profile to convert data:
 
 ```python
 # transform the whole table:
 df = profile.transform(table)  # pandas.DataFrame
@@ -420,15 +428,15 @@
 
 | Country | ⇒ | Country |
 |---------|---|---------|
 | france  |   | 0       |
 | italy   |   | 2       |
 | germany |   | 1       |
 
-Their index in the list is used as the numerical value.
+Their index in the argument list is used as the numerical value.
 If no values are specified, the values found in the provided
 data are sorted in lexically ascending order.
 
 ---
 
 ### OneHot
 
@@ -556,29 +564,36 @@
 ```
 
 | Symptoms               | ⇒ | Symptoms=cough | Symptoms=fever | Symptoms=headache |
 |------------------------|---|----------------|----------------|-------------------|
 | fever, cough, headache |   | 1              | 1              | 1                 |
 | headache, cough        |   | 1              | 0              | 1                 |
 
-The default separator for `list` is a comma.<br>
+The default delimiter is a comma.<br>
+You can specify a custom delimiter via the `delimiter` argument:
+
+```python
+"Symptoms": List(delimiter=";")
+"Symptoms": List(delimiter=[",", ";"])  # also accepts lists
+```
+
 The passed strings are interpreted as regular expressions.
 
 ### ListAndOr
 
 ```python
 "Symptoms": ListAndOr()
 ```
 
 | Symptoms                  | ⇒ | Symptoms=cough | Symptoms=fever | Symptoms=headache |
 |---------------------------|---|----------------|----------------|-------------------|
 | fever, cough and headache |   | 1              | 1              | 1                 |
 | headache or cough         |   | 1              | 0              | 1                 |
 
-The default separators for `list_and_or` are comma, "and" and "or".<br>
+The default delimiters are comma, "and" and "or".<br>
 The passed strings are interpreted as regular expressions.
 
 ### Map
 
 ### Strip
 
 ### Split
@@ -623,15 +638,15 @@
 
 ```python
 Parallel(converter1, converter2, ...)
 ```
 
 Apply different converters to the respective items.
 Usually used in a Pipeline after other converters that create outputs with multiple items (e.g. `Split()`).
-Also, you usually want to use `Flatten()` after this, as each individual converter will return a list of items,
+Also, you usually want to use `Flatten()` after this, as each individual converter will return a tuple of items,
 even if it only contains one item.
 Example:
 
 ```python
 "Latitude;Longitude": [
     Split(";"),  # must always result in two items, because Parallel() has 2 converters
     Parallel(Ignore(), Float()),  # ignore latitude, convert longitude to float -> [[], [longitude]]
@@ -680,77 +695,86 @@
 
 ### Label
 
 ### Flatten
 
 ### Transpose
 
-Can transpose nested lists, given that the nested lists are of equal length.
+Can transpose nested tuples, given that the nested tuples are of equal length.
 
 For example, look at this elegant implementation of the [`List()`](#list) converter:
 
 ```python
 "Symptoms": [
     Split(r"\s*,\s*"),  # split at comma
     ForEach(OneHot()),
     Transpose(),
     ForEach(max),
     Flatten()
 ]
 ```
 
 `Transpose()` allows us to apply `max` to each column of the one-hot encodings
-across all list elements.
+across all tuple elements.
 
 ### Function
 
 ```python
 Function(transform, labels=None)
 ```
 
 Shorthand: Instead of `Function(transform, None)`, just write `transform`, where `transform` is some callable.
 
 Creates a custom converter from a custom ``transform()`` function
 (and optionally, a custom ``labels()`` function).
 This is a handy way to create a converter that doesn't need ``fit()``.
 
-Unlike ``StrictFunction()``, this class can handle functions that don't accept or return lists,
+Unlike ``StrictFunction()``, this class can handle functions that don't accept or return tuples,
 which often allows for more concise code.
 
 This is achieved during ``fit()`` as follows:
 
-1. If all incoming items are 1-element lists, it sets a flag ``UNPACK_OUTPUT`` to always
+1. If all incoming items are 1-element tuples, it sets a flag ``UNPACK_OUTPUT`` to always
    unpack the element before passing them to the wrapped function during ``transform()``.
-2. If during ``fit()`` the wrapped function doesn't return lists,
-   it tries to turn that output into a list:
+2. If during ``fit()`` the wrapped function doesn't return tuples,
+   it tries to turn that output into a tuple:
     - If the output is always a non-string iterable, it will simply set a
-      flag ``CONVERT_ITERABLE`` to always convert the iterable output into a list during ``transform()``.
+      flag ``CONVERT_ITERABLE`` to always convert the iterable output into a tuple during ``transform()``.
     - Otherwise, it sets a flag ``WRAP_OUTPUT`` to always wrap the output in a
-      1-element list during ``transform()``.
+      1-element tuple during ``transform()``.
 
 A similar logic is applied to the labels.
 If a custom labels function is given, the following procedure is followed during ``labels()``:
 
-1. If the incoming labels are a 1-element list, the single label is unpacked before
+1. If the incoming labels are a 1-element tuples, the single label is unpacked before
    it is passed to the custom labels function.
-2. If the custom labels function returns something other than a list,
-   this class tries to convert it into a list:
-    - If the output is a non-string iterable, it is converted into a list.
-    - Otherwise, the output is wrapped in a 1-element list.
+2. If the custom labels function returns something other than a tuple,
+   this class tries to convert it into a tuple:
+    - If the output is a non-string iterable, it is converted into a tuple.
+    - Otherwise, the output is wrapped in a 1-element tuple.
 
 If no custom labels function is given, the output labels are generated based on the
 output cardinality inferred during ``fit()`` and according to the following logic:
 
 - If the number of incoming labels is identical to the output cardinality,
   the labels will be returned unchanged.
-- Otherwise, the number of incoming labels must be 1 and the output labels are generated by adding suffixes
-  ``_0``, ``_1``, etc. to the single input label.
+- If there are multiple incoming labels but a single output label,
+  the output label is formed by joining the incoming labels with ``, ``.
+- If there is a single incoming label but multiple output labels,
+  the output labels are formed by adding suffixes ``_0``, ``_1``, etc.
+  to the single input label.
+
+|                    | **1 Output Label** | **M Output Labels**          |
+|--------------------|--------------------|------------------------------|
+| **1 Input Label**  | identical          | suffixes ``_0``, ``_1``, ... |
+| **N Input Labels** | join with ``, ``   | identical if M=N, else ERROR |
 
 A special case are functions returning output of varying cardinality during ``fit()``.
-In this case, a single input label is returned.
+In this case, a single label is returned.
+If only one input label is given, that single label is returned.
 If multiple input labels are given, they are joined with ``_``.
 
 The following example turns a text column into two columns containing the ascii code of the first and last letter.
 
 ```python
 "Name": lambda x: (ord(x[0]), ord(x[-1]))
 ```
@@ -760,80 +784,80 @@
 | Alice |   | 97     | 101    |
 | Bob   |   | 98     | 98     |
 
 (Remember that by default, all text entries are converted to
 lowercase before further processing.)
 
 As you can see, the number of columns is inferred directly from the return value of the conversion function.
-If the function returns a list, the resulting column names are indexed.
+If the function returns a tuple, the resulting column names are indexed.
 
 You can also set the labels explicitly with a lambda function
 that takes the input column name as an argument and returns output column names:
 
 ```python
-"Name": Function(lambda x: [ord(x[0]), ord(x[-1])],
-                 labels=lambda s: [f"ord(first letter of {s})", f"ord(last letter of {s})"]),
+"Name": Function(lambda x: (ord(x[0]), ord(x[-1])),
+                 labels=lambda s: (f"ord(first letter of {s})", f"ord(last letter of {s})")),
 ```
 
 | Name  | ⇒ | ord(first letter of Name) | ord(last letter of Name) |
 |-------|---|---------------------------|--------------------------|
 | Alice |   | 97                        | 101                      |
 | Bob   |   | 98                        | 98                       |
 
 However, remember that you can always simply use [`Label()`](#label) to rename the columns after the conversion,
 if you don't need the output column names to depend on the input column names.
 
 ```python
-"Name": [lambda x: [ord(x[0]), ord(x[-1])],
+"Name": [lambda x: (ord(x[0]), ord(x[-1])),
          Labels("ord(first letter)", "ord(last letter)")],
 ```
 
 ### StrictFunction
 
 ```python
 StrictFunction(transform, labels=None)
 ```
 
 Works mostly like [`Function()`](#function), but simpler:
-``transform`` and ``labels`` must both accept and return lists.
+``transform`` and ``labels`` must both accept and return tuples.
 Instead of something like this:
 
 ```python
 "Name": str.lower,
 ```
 
 you have to write this:
 
 ```python
-"Name": StrictFunction(lambda x: [str.lower(x[0])])
+"Name": StrictFunction(lambda x: (str.lower(x[0]),))  # notice the comma, which makes it a 1-element tuple
 ```
 
-That is, you will still receive 1-element lists as lists to the function,
-even if all input elements during `fit()` are 1-element lists.
-Also, you must now explicitly return a list,
-even if it is just a 1-element list, as otherwise an error will be raised.
+That is, you will still receive 1-element tuples as tuples to the function,
+even if all input elements during `fit()` are 1-element tuples.
+Also, you must now explicitly return a tuple,
+even if it is just a 1-element tuple, as otherwise an error will be raised.
 
 See [`Function()`](#function) for a convenient extension of this converter.
 
 ---
 
 ## Understanding Multi-Column Converters
 
 A converter returns two things:
 
 - `transform()`: the items of the transformed data
 - `labels()`: a label for each item
 
-Both return values are lists.
+Both return values are tuples.
 
 For top-level converters, this then creates the corresponding amount of columns.
 This includes the case of
 
-- a 1-element list `[item]`, which is the case for most converters.
-- an empty list `[]`, in which the result is ignored.
+- a 1-element tuple `(item,)`, which is the case for most converters.
+- an empty tuple `()`, in which the result is ignored.
   (In fact, this is exactly how `Ignore()` is implemented.)
 
 This means, however, that for top-level converters, `labels()` and `transform()`
 must return the same number of items.
 That is because `labels()` is used to create the output column names.
 If `transform()` returns a different number of items, that will raise an error for top-level converters.
```

### Comparing `clevertable-2.6.0/src/clevertable.egg-info/SOURCES.txt` & `clevertable-3.0.0/src/clevertable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

