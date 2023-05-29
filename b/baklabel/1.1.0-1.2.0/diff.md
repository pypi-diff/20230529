# Comparing `tmp/baklabel-1.1.0.tar.gz` & `tmp/baklabel-1.2.0.tar.gz`

## Comparing `baklabel-1.1.0.tar` & `baklabel-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 baklabel-1.1.0/doc/about.txt
--rw-r--r--   0        0        0    21203 2020-02-02 00:00:00.000000 baklabel-1.1.0/doc/backup_howto.txt
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 baklabel-1.1.0/doc/instructions.txt
--rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 baklabel-1.1.0/doc/release_note.txt
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 baklabel-1.1.0/doc/synopsis.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 baklabel-1.1.0/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 baklabel-1.1.0/src/baklabel/__init__.py
--rw-r--r--   0        0        0    22756 2020-02-02 00:00:00.000000 baklabel-1.1.0/src/baklabel/baklabel.py
--rw-r--r--   0        0        0    20348 2020-02-02 00:00:00.000000 baklabel-1.1.0/src/baklabel/test_baklabel.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 baklabel-1.1.0/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 baklabel-1.1.0/LICENSE
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 baklabel-1.1.0/README.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 baklabel-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 baklabel-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 baklabel-1.2.0/doc/about.txt
+-rw-r--r--   0        0        0    21203 2020-02-02 00:00:00.000000 baklabel-1.2.0/doc/backup_howto.txt
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 baklabel-1.2.0/doc/instructions.txt
+-rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 baklabel-1.2.0/doc/release_note.txt
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 baklabel-1.2.0/doc/synopsis.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 baklabel-1.2.0/src/baklabel/__init__.py
+-rw-r--r--   0        0        0    24128 2020-02-02 00:00:00.000000 baklabel-1.2.0/src/baklabel/baklabel.py
+-rw-r--r--   0        0        0    22619 2020-02-02 00:00:00.000000 baklabel-1.2.0/src/baklabel/test_baklabel.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 baklabel-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 baklabel-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 baklabel-1.2.0/README.md
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 baklabel-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 baklabel-1.2.0/PKG-INFO
```

### Comparing `baklabel-1.1.0/doc/backup_howto.txt` & `baklabel-1.2.0/doc/backup_howto.txt`

 * *Files identical despite different names*

### Comparing `baklabel-1.1.0/doc/instructions.txt` & `baklabel-1.2.0/doc/instructions.txt`

 * *Files identical despite different names*

### Comparing `baklabel-1.1.0/doc/release_note.txt` & `baklabel-1.2.0/doc/release_note.txt`

 * *Files identical despite different names*

### Comparing `baklabel-1.1.0/doc/synopsis.txt` & `baklabel-1.2.0/doc/synopsis.txt`

 * *Files identical despite different names*

### Comparing `baklabel-1.1.0/src/baklabel/baklabel.py` & `baklabel-1.2.0/src/baklabel/baklabel.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,41 +41,41 @@
 
 relnote = """baklabel - see Description below
 ========
 
 Version  Build Who  When/What
 ==============================
 
-ver 1.1.0 2729  md  23 May 2023 - Change from GPL3 to MIT license, change
-                    to pyproject.toml and clean up strings using f-strings
+ver 1.2.0   md  29 May 2023 - Improve guessdate() to resolve ambiguous dates
 
+ver 1.1.0   md  23 May 2023 - Change from GPL3 to MIT license, change to pyproject.toml
+                and clean up strings using f-strings
 
-ver 1.0.3 2729  md  24 Aug 2012 - Code review and tweaks to test importing
-                    to cater for in-house python path adjustments
 
-ver 1.0.2 2685  md  8 Mar 2011 - Refactored guessdate() out of __main__
-                    to permit string dates as a calling convenience
+ver 1.0.3   md  24 Aug 2012 - Code review and tweaks to test importing to cater for
+                in-house python path adjustments
 
-ver 1.0.1 2671  md  4 Nov 2010 - Minor refactoring and tidying comments
+ver 1.0.2   md  8 Mar 2011 - Refactored guessdate() out of __main__ to permit string
+                dates as a calling convenience
 
-ver 1.0.0 2670  md  3 Nov 2010 - New option to append current year to
-                    any month-end label, not just end-of-year.
+ver 1.0.1   md  4 Nov 2010 - Minor refactoring and tidying comments
 
-ver 0.2.0 2664  md  27 oct 2010 - Help now respects defaults which have
-                    been adjusted in the source code. A new default now
-                    permits adjustment of new_year_month which sets the
-                    end-of-year label to any desired month.
+ver 1.0.0   md  3 Nov 2010 - New option to append current year to any month-end label,
+                not just end-of-year.
 
-ver 0.1.0b 2646  md 8 oct 2010 - Added -d numeric option for setting
-                    the label to x days ago. Eg., -1 = yesterday. Also
-                    added a time trigger option in the -d switch such
-                    that, for example, -d 3am will produce yesterday's
-                    label if baklabel is called prior to 3am
+ver 0.2.0   md  27 oct 2010 - Help now respects defaults which have been adjusted in
+                the source code. A new default now permits adjustment of new_year_month
+                which sets the end-of-year label to any desired month.
 
-ver 0.0.0a 2640  md 1 jul 2010 - first written
+ver 0.1.0b   md 8 oct 2010 - Added -d numeric option for setting the label to x days
+                ago. Eg., -1 = yesterday. Also added a time trigger option in the -d
+                switch such that, for example, -d 3am will produce yesterday's label
+                if baklabel is called prior to 3am
+
+ver 0.0.0a   md 1 jul 2010 - first written
 
 
 Description
 ==========={0}
 
 Grandfathered Backups
 ====================={1}
@@ -198,34 +198,64 @@
 # avoid weekly backups (not recommended) with WEEKLY_DAY >= 7
 
 SMALLHOURS = 4
 # if the backup starts before SMALLHOURS am then use yesterday's label
 # otherwise use today's label
 
 
+def detect_system_date_format():
+    import locale
+    system_locale = locale.getlocale()
+    if system_locale[0]:
+        example_date = datetime(2023, 5, 29)  # Example date today will suffice
+        locale.setlocale(locale.LC_TIME, system_locale)  # Set the locale explicitly
+        formatted_date = example_date.strftime("%x")  # Get formatted date
+        system_date_format = formatted_date.replace(
+            "2023", "YYYY"
+        ).replace(
+            "05", "MM"
+        ).replace(
+            "29", "DD"
+        )
+        return system_date_format
+    else:
+        # Only if no locale is set - possibly needs "MM-DD-YY" but not tested
+        return "YYYY-MM-DD"  # Default date format if detection fails
+
 
-def guessdate(dstr):
-    # now conjure/guess a date from a string
+def guessdate(dstr, line=None):
+    # now conjure/guess a date from a ?-?-? or ?/?/? string
     bits = dstr.split('-')
     if len(bits) < 3:
         bits = dstr.split('/')
     if len(bits) == 3:
         if int(bits[0]) > 31: # must be ye, mo, da
             ye = int(bits[0])
             mo = int(bits[1])
             da = int(bits[2])
-        else:
-            if int(bits[1]) > 12: # must be mo, da, ye
+        else:  # bits[2] is the year
+            if int(bits[1]) > 12 and int(bits[2]) > 31: # must be mo, da, ye
                 mo = int(bits[0])
                 da = int(bits[1])
                 ye = int(bits[2])
-            else: # probably da, mo, ye - but maybe not
-                da = int(bits[0])
-                mo = int(bits[1])
-                ye = int(bits[2])
+            else: # ambiguous
+                system_date_format = detect_system_date_format()
+                if line:
+                    print(f"\n235 baklabel system_date_format = {system_date_format}")
+                now = datetime.now()
+                fmt = now.strftime('%x')
+                if line:
+                    print(f"\n238 baklabel fmt = {fmt}")
+                fbits = system_date_format.split("-")
+                if len(fbits) < 3:
+                    fbits = system_date_format.split('/')
+                if len(fbits) == 3:
+                    ye = int(bits[fbits.index("YYYY")])
+                    mo = int(bits[fbits.index("MM")])
+                    da = int(bits[fbits.index("DD")])
         return date(ye, mo, da)
     else:
         raise ValueError('Invalid date format')
 
 class Grandad:
 
     # See __doc__ = synopsis below
@@ -289,15 +319,15 @@
         append_eom_year=APPEND_YEAR_TO_EOM_LABEL,
         weekly_day=WEEKLY_DAY,
         smallhours=SMALLHOURS,
     ):
 
         # increment = -1 means yesterday so hard-code 0 to begin with
         self.increment = 0
-        # smallhours = 3 means use yesterday only until 3am
+        # smallhours = 3 means use yesterday only until 3am - don't care about DST
         self.smallhours = smallhours
         self.backupday = self._confirmday(backupday)
         self.tomorrow = date.fromordinal(self.backupday.toordinal() + 1)
         self.server_prefix = server_prefix
         self.new_year_month = new_year_month
         self.eoy_label = eoy_label
         self.append_eoy_year = append_eoy_year
```

### Comparing `baklabel-1.1.0/src/baklabel/test_baklabel.py` & `baklabel-1.2.0/src/baklabel/test_baklabel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,89 @@
 import unittest
 import os, sys
 from datetime import date
-from baklabel import Grandad
+from baklabel import Grandad, guessdate
 
 
-class test_baklabel(unittest.TestCase):
+class TestGuessdate(unittest.TestCase):
+
+    def test_usa_date_slash(self):
+        dlst = 12, 31, 2023
+        dstr = "/".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr)), '2023-12-31')
+
+
+    def test_eu_date_slash(self):
+        dlst = 2023, 12, 31
+        dstr = "/".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr)), '2023-12-31')
+
+
+    def test_au_date_slash(self):
+        dlst = 31, 12, 2023
+        dstr = "/".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr)), '2023-12-31')
+
+
+    def test_usa_date_ambig_slash(self):
+        dlst = 5, 6, 2023
+        dstr = "/".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr, line=None)), '2023-06-05')
+
+
+    def test_eu_date_ambig_slash(self):
+        dlst = 2023, 6, 5
+        dstr = "/".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr)), '2023-06-05')
+
+
+    def test_au_date_ambig_slash(self):
+        dlst = 5, 6, 2023
+        dstr = "/".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr)), '2023-06-05')
+
+
+    def test_usa_date_slash(self):
+        dlst = 12, 31, 2023
+        dstr = "-".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr)), '2023-12-31')
+
+
+    def test_eu_date(self):
+        dlst = 2023, 12, 31
+        dstr = "-".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr)), '2023-12-31')
+
+
+    def test_au_date(self):
+        dlst = 31, 12, 2023
+        dstr = "-".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr)), '2023-12-31')
+
+
+    def test_usa_date_ambig(self):
+        dlst = 5, 6, 2023
+        dstr = "-".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr, line=None)), '2023-06-05')
+
+
+    def test_eu_date_ambig(self):
+        dlst = 2023, 6, 5
+        dstr = "-".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr)), '2023-06-05')
+
+
+    def test_au_date_ambig(self):
+        dlst = 5, 6, 2023
+        dstr = "-".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr)), '2023-06-05')
+
+
+
+class TestBaklabel(unittest.TestCase):
     """
     def __init__(self,
         backupday=date.today(),
         server_prefix=SERVER_PREFIX,
         new_year_month=NEW_YEAR_MONTH,
         eoy_label=EOY_LABEL,
         append_eoy_year=APPEND_YEAR_TO_EOY_LABEL,
```

### Comparing `baklabel-1.1.0/LICENSE` & `baklabel-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `baklabel-1.1.0/README.md` & `baklabel-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `baklabel-1.1.0/pyproject.toml` & `baklabel-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "baklabel"
-version               = '1.1.0'
+version       = '1.2.0'
 authors = [
   { name="Mike Dewhirst", email="miked@dewhirst.com.au" },
 ]
 description = "Baklabel delivers a daily label fragment for grandfathered backups"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `baklabel-1.1.0/PKG-INFO` & `baklabel-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baklabel
-Version: 1.1.0
+Version: 1.2.0
 Summary: Baklabel delivers a daily label fragment for grandfathered backups
 Project-URL: Homepage, https://svn.climate.com.au/repos/pysrc/foss/baklabel
 Author-email: Mike Dewhirst <miked@dewhirst.com.au>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

