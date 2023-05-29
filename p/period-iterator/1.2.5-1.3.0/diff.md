# Comparing `tmp/period-iterator-1.2.5.tar.gz` & `tmp/period-iterator-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/period-iterator-1.2.5.tar", last modified: Wed Jun 10 06:20:56 2020, max compression
+gzip compressed data, was "period-iterator-1.3.0.tar", last modified: Mon May 29 05:24:05 2023, max compression
```

## Comparing `period-iterator-1.2.5.tar` & `period-iterator-1.3.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-10 06:20:56.927456 period-iterator-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (116)     1549 2020-06-10 06:20:56.927456 period-iterator-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      660 2020-06-10 06:20:42.000000 period-iterator-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-10 06:20:56.923456 period-iterator-1.2.5/period_iterator/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-10 06:20:42.000000 period-iterator-1.2.5/period_iterator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1586 2020-06-10 06:20:42.000000 period-iterator-1.2.5/period_iterator/period_cursor.py
--rw-r--r--   0 runner    (1001) docker     (116)     4571 2020-06-10 06:20:42.000000 period-iterator-1.2.5/period_iterator/period_iterator.py
--rw-r--r--   0 runner    (1001) docker     (116)      153 2020-06-10 06:20:42.000000 period-iterator-1.2.5/period_iterator/period_timezone.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-10 06:20:56.927456 period-iterator-1.2.5/period_iterator/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-10 06:20:42.000000 period-iterator-1.2.5/period_iterator/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1087 2020-06-10 06:20:42.000000 period-iterator-1.2.5/period_iterator/tests/test_period_cursor.py
--rw-r--r--   0 runner    (1001) docker     (116)     3583 2020-06-10 06:20:42.000000 period-iterator-1.2.5/period_iterator/tests/test_period_iterator.py
--rw-r--r--   0 runner    (1001) docker     (116)      495 2020-06-10 06:20:42.000000 period-iterator-1.2.5/period_iterator/tests/test_period_timezone.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-10 06:20:56.927456 period-iterator-1.2.5/period_iterator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1549 2020-06-10 06:20:56.000000 period-iterator-1.2.5/period_iterator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      513 2020-06-10 06:20:56.000000 period-iterator-1.2.5/period_iterator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-06-10 06:20:56.000000 period-iterator-1.2.5/period_iterator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       21 2020-06-10 06:20:56.000000 period-iterator-1.2.5/period_iterator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2020-06-10 06:20:56.000000 period-iterator-1.2.5/period_iterator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-06-10 06:20:56.927456 period-iterator-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     3530 2020-06-10 06:20:42.000000 period-iterator-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 05:24:05.926372 period-iterator-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-29 05:23:45.000000 period-iterator-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-29 05:24:05.926372 period-iterator-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-29 05:23:45.000000 period-iterator-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 05:24:05.922372 period-iterator-1.3.0/period_iterator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 05:23:45.000000 period-iterator-1.3.0/period_iterator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-29 05:23:45.000000 period-iterator-1.3.0/period_iterator/period_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-29 05:23:45.000000 period-iterator-1.3.0/period_iterator/period_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-29 05:23:45.000000 period-iterator-1.3.0/period_iterator/period_timezone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 05:24:05.926372 period-iterator-1.3.0/period_iterator/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 05:23:45.000000 period-iterator-1.3.0/period_iterator/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-29 05:23:45.000000 period-iterator-1.3.0/period_iterator/tests/test_period_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-29 05:23:45.000000 period-iterator-1.3.0/period_iterator/tests/test_period_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-29 05:23:45.000000 period-iterator-1.3.0/period_iterator/tests/test_period_timezone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 05:24:05.926372 period-iterator-1.3.0/period_iterator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-29 05:24:05.000000 period-iterator-1.3.0/period_iterator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-29 05:24:05.000000 period-iterator-1.3.0/period_iterator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 05:24:05.000000 period-iterator-1.3.0/period_iterator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-29 05:24:05.000000 period-iterator-1.3.0/period_iterator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 05:24:05.000000 period-iterator-1.3.0/period_iterator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 05:24:05.926372 period-iterator-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-29 05:23:45.000000 period-iterator-1.3.0/setup.py
```

### Comparing `period-iterator-1.2.5/PKG-INFO` & `period-iterator-1.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 Metadata-Version: 2.1
 Name: period-iterator
-Version: 1.2.5
+Version: 1.3.0
 Summary: Period Iterator
 Home-page: https://github.com/chonla/period-iterator
 Author: Chonlasith Jucksriporn
 Author-email: chonlasith@gmail.com
 License: MIT
-Description: # Period Iterator
-        
-        Period Iterator is a library easing you to iterate through given period.
-        
-        ## Usage
-        
-        ```python
-        from period_iterator.period_iterator import period_iterator
-        
-        period = period_iterator('2020-02-01,2020-02-03', 'Asia/Bangkok')
-        
-        while True:
-            print(period.cursor.begin()) # Begin of day
-            print(period.cursor.end()) # End of day
-            if not period.next():
-                break
-        
-        # Expected Output
-        #
-        # 2020-02-01T00:00:00+07:00
-        # 2020-02-01T23:59:59+07:00
-        # 2020-02-02T00:00:00+07:00
-        # 2020-02-02T23:59:59+07:00
-        # 2020-02-03T00:00:00+07:00
-        # 2020-02-03T23:59:59+07:00
-        ```
-        
-        ## License
-        
-        [MIT](https://github.com/chonla/period-iterator/blob/master/LICENSE)
-        
 Keywords: period,iterator
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Period Iterator
+
+Period Iterator is a library easing you to iterate through given period.
+
+## Usage
+
+```python
+from period_iterator.period_iterator import period_iterator
+
+period = period_iterator('2020-02-01,2020-02-03', 'Asia/Bangkok')
+
+while True:
+    print(period.cursor.begin()) # Begin of day
+    print(period.cursor.end()) # End of day
+    print(period.cursor.date()) # Date
+    if not period.next():
+        break
+
+# Expected Output
+#
+# 2020-02-01T00:00:00+07:00
+# 2020-02-01T23:59:59+07:00
+# 2020-02-01
+# 2020-02-02T00:00:00+07:00
+# 2020-02-02T23:59:59+07:00
+# 2020-02-02
+# 2020-02-03T00:00:00+07:00
+# 2020-02-03T23:59:59+07:00
+# 2020-02-03
+```
+
+## License
+
+[MIT](https://github.com/chonla/period-iterator/blob/master/LICENSE)
```

### Comparing `period-iterator-1.2.5/README.md` & `period-iterator-1.3.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -8,23 +8,27 @@
 from period_iterator.period_iterator import period_iterator
 
 period = period_iterator('2020-02-01,2020-02-03', 'Asia/Bangkok')
 
 while True:
     print(period.cursor.begin()) # Begin of day
     print(period.cursor.end()) # End of day
+    print(period.cursor.date()) # Date
     if not period.next():
         break
 
 # Expected Output
 #
 # 2020-02-01T00:00:00+07:00
 # 2020-02-01T23:59:59+07:00
+# 2020-02-01
 # 2020-02-02T00:00:00+07:00
 # 2020-02-02T23:59:59+07:00
+# 2020-02-02
 # 2020-02-03T00:00:00+07:00
 # 2020-02-03T23:59:59+07:00
+# 2020-02-03
 ```
 
 ## License
 
 [MIT](https://github.com/chonla/period-iterator/blob/master/LICENSE)
```

### Comparing `period-iterator-1.2.5/period_iterator/period_cursor.py` & `period-iterator-1.3.0/period_iterator/period_cursor.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,30 +8,33 @@
         self.timezone_name = timezone_name
         self.timezone = timezone(timezone_name)
         self.now = datetime.now(self.timezone)
         tzfmt = period_timezone()
         self.timezone_offset = tzfmt.format(self.now.strftime('%Z'))
 
         self.cursor = datetime.fromisoformat(timestamp)
-        self.comparableCursor = self.cursor.strftime('%Y-%m-%d')
+        self.comparable_cursor = self.cursor.strftime('%Y-%m-%d')
 
     def __ge__(self, other):
-        return self.comparableCursor >= other.comparableCursor
+        return self.comparable_cursor >= other.comparable_cursor
 
     def __eq__(self, other):
-        return self.comparableCursor == other.comparableCursor
+        return self.comparable_cursor == other.comparable_cursor
 
     def __repr__(self):
-        return self.comparableCursor
+        return self.comparable_cursor
 
     def tomorrow(self):
         return period_cursor((self.cursor + relativedelta.relativedelta(days=1)).strftime('%Y-%m-%dT%H:%M:%S{}'.format(self.timezone_offset)), self.timezone_name)
 
     def begin(self, format='default'):
         if format=='default':
             return self.cursor.strftime('%Y-%m-%dT00:00:00{}'.format(self.timezone_offset))
         return datetime.fromisoformat(self.cursor.strftime('%Y-%m-%dT00:00:00{}'.format(self.timezone_offset))).strftime(format)
 
     def end(self, format='default'):
         if format=='default':
             return self.cursor.strftime('%Y-%m-%dT23:59:59{}'.format(self.timezone_offset))
-        return datetime.fromisoformat(self.cursor.strftime('%Y-%m-%dT23:59:59{}'.format(self.timezone_offset))).strftime(format)
+        return datetime.fromisoformat(self.cursor.strftime('%Y-%m-%dT23:59:59{}'.format(self.timezone_offset))).strftime(format)
+
+    def date(self):
+        return self.cursor.strftime('%Y-%m-%d')
```

### Comparing `period-iterator-1.2.5/period_iterator/period_iterator.py` & `period-iterator-1.3.0/period_iterator/period_iterator.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 import re
 from .period_timezone import period_timezone
 
 class period_iterator:
     def __init__(self, period, timezone_name):
         self.timezone_name = timezone_name
         self.timezone = timezone(timezone_name)
-        self.now = datetime.now(self.timezone)
+
+        self.now = datetime.now()
         tzfmt = period_timezone()
-        self.timezone_offset = tzfmt.format(self.now.strftime('%Z'))
+        self.timezone_offset = tzfmt.format(datetime.now(self.timezone).strftime('%Z'))
 
         if period == 'lastonequarterhour':
             offset_from_15 = self.now.minute % 15
             baseline = self.now - \
                 relativedelta.relativedelta(minutes=-offset_from_15)
             start = baseline + relativedelta.relativedelta(minutes=-15)
             end = baseline + relativedelta.relativedelta(minutes=-1)
```

### Comparing `period-iterator-1.2.5/period_iterator/tests/test_period_cursor.py` & `period-iterator-1.3.0/period_iterator/tests/test_period_cursor.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,8 +16,20 @@
         cursor2 = period_cursor('2020-03-05T13:34:56+07:00', 'Asia/Bangkok')
         assert cursor2 >= cursor1
         assert not (cursor1 >= cursor2)
 
     def test_tomorrow(self):
         cursor = period_cursor('2020-03-04T12:34:56+07:00', 'Asia/Bangkok')
         tomorrow_cursor = period_cursor('2020-03-05T12:34:56+07:00', 'Asia/Bangkok')
-        assert cursor.tomorrow() == tomorrow_cursor
+        assert cursor.tomorrow() == tomorrow_cursor
+
+    def test_date(self):
+        cursor = period_cursor('2020-03-04T12:34:56+07:00', 'Asia/Bangkok')
+        assert cursor.date() == '2020-03-04'
+
+    def test_tomorrow_date(self):
+        cursor = period_cursor('2020-03-04T12:34:56+07:00', 'Asia/Bangkok')
+        assert cursor.tomorrow().date() == '2020-03-05'
+
+    def test_day_after_tomorrow_date(self):
+        cursor = period_cursor('2020-03-30T12:34:56+07:00', 'Asia/Bangkok')
+        assert cursor.tomorrow().tomorrow().date() == '2020-04-01'
```

### Comparing `period-iterator-1.2.5/period_iterator/tests/test_period_iterator.py` & `period-iterator-1.3.0/period_iterator/tests/test_period_iterator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from ..period_iterator import period_iterator
 from ..period_cursor import period_cursor
-from libfaketime import fake_time
-from datetime import datetime
+from freezegun import freeze_time
 import pytest
 
 @pytest.fixture()
 def timezone_name():
     yield 'Asia/Bangkok'
 
-@fake_time('2019-12-31 17:00:00', tz_offset=7) # It is 2020-01-01T00:00:00+0700
+@freeze_time('2019-12-31 17:00:00', tz_offset=7) # It is 2020-01-01T00:00:00+0700
 class test_period_iterator():
     def test_period_with_start_end(self, timezone_name):
         period = period_iterator('lastmonth,thismonth', timezone_name)
         assert period.start == '2019-12-01T00:00:00+07:00'
         assert period.stop == '2020-01-31T23:59:59+07:00'
     
     def test_period_with_single_timestamp(self, timezone_name):
```

### Comparing `period-iterator-1.2.5/period_iterator.egg-info/PKG-INFO` & `period-iterator-1.3.0/period_iterator.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 Metadata-Version: 2.1
 Name: period-iterator
-Version: 1.2.5
+Version: 1.3.0
 Summary: Period Iterator
 Home-page: https://github.com/chonla/period-iterator
 Author: Chonlasith Jucksriporn
 Author-email: chonlasith@gmail.com
 License: MIT
-Description: # Period Iterator
-        
-        Period Iterator is a library easing you to iterate through given period.
-        
-        ## Usage
-        
-        ```python
-        from period_iterator.period_iterator import period_iterator
-        
-        period = period_iterator('2020-02-01,2020-02-03', 'Asia/Bangkok')
-        
-        while True:
-            print(period.cursor.begin()) # Begin of day
-            print(period.cursor.end()) # End of day
-            if not period.next():
-                break
-        
-        # Expected Output
-        #
-        # 2020-02-01T00:00:00+07:00
-        # 2020-02-01T23:59:59+07:00
-        # 2020-02-02T00:00:00+07:00
-        # 2020-02-02T23:59:59+07:00
-        # 2020-02-03T00:00:00+07:00
-        # 2020-02-03T23:59:59+07:00
-        ```
-        
-        ## License
-        
-        [MIT](https://github.com/chonla/period-iterator/blob/master/LICENSE)
-        
 Keywords: period,iterator
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Period Iterator
+
+Period Iterator is a library easing you to iterate through given period.
+
+## Usage
+
+```python
+from period_iterator.period_iterator import period_iterator
+
+period = period_iterator('2020-02-01,2020-02-03', 'Asia/Bangkok')
+
+while True:
+    print(period.cursor.begin()) # Begin of day
+    print(period.cursor.end()) # End of day
+    print(period.cursor.date()) # Date
+    if not period.next():
+        break
+
+# Expected Output
+#
+# 2020-02-01T00:00:00+07:00
+# 2020-02-01T23:59:59+07:00
+# 2020-02-01
+# 2020-02-02T00:00:00+07:00
+# 2020-02-02T23:59:59+07:00
+# 2020-02-02
+# 2020-02-03T00:00:00+07:00
+# 2020-02-03T23:59:59+07:00
+# 2020-02-03
+```
+
+## License
+
+[MIT](https://github.com/chonla/period-iterator/blob/master/LICENSE)
```

### Comparing `period-iterator-1.2.5/period_iterator.egg-info/SOURCES.txt` & `period-iterator-1.3.0/period_iterator.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 period_iterator/__init__.py
 period_iterator/period_cursor.py
 period_iterator/period_iterator.py
 period_iterator/period_timezone.py
 period_iterator.egg-info/PKG-INFO
```

### Comparing `period-iterator-1.2.5/setup.py` & `period-iterator-1.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 setup(
     name='period-iterator',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.2.5',
+    version='1.3.0',
 
     description='Period Iterator',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://github.com/chonla/period-iterator',
@@ -48,14 +48,17 @@
         # Pick your license as you wish (should match "license" above)
         'License :: OSI Approved :: MIT License',
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 
     # What does your project relate to?
     keywords='period, iterator',
 
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
```

