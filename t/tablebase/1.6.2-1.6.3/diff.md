# Comparing `tmp/tablebase-1.6.2.tar.gz` & `tmp/tablebase-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\AllFiles\PythonLibs\tablebase\dist\.tmp-wl7xyb_b\tablebase-1.6.2.tar", last modified: Sun May 28 00:59:45 2023, max compression
+gzip compressed data, was "C:\AllFiles\PythonLibs\tablebase\dist\.tmp-xk2ow7pa\tablebase-1.6.3.tar", last modified: Mon May 29 20:18:26 2023, max compression
```

## Comparing `tablebase-1.6.2.tar` & `tablebase-1.6.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 00:59:45.701393 tablebase-1.6.2/
--rw-rw-rw-   0        0        0     1086 2022-07-18 21:48:23.000000 tablebase-1.6.2/LICENSE
--rw-rw-rw-   0        0        0     1084 2021-04-03 19:09:23.000000 tablebase-1.6.2/LICENSE.txt
--rw-rw-rw-   0        0        0      399 2023-05-28 00:59:45.701393 tablebase-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0      721 2022-07-20 22:00:14.000000 tablebase-1.6.2/README.md
--rw-rw-rw-   0        0        0       86 2022-11-01 20:19:29.000000 tablebase-1.6.2/pyproject.toml
--rw-rw-rw-   0        0        0      494 2023-05-28 00:59:45.704300 tablebase-1.6.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 00:59:45.654534 tablebase-1.6.2/tablebase/
--rw-rw-rw-   0        0        0       40 2022-05-08 21:07:22.000000 tablebase-1.6.2/tablebase/__init__.py
--rw-rw-rw-   0        0        0    10790 2023-05-28 00:54:54.000000 tablebase-1.6.2/tablebase/tablebase.py
-drwxrwxrwx   0        0        0        0 2023-05-28 00:59:45.698375 tablebase-1.6.2/tablebase.egg-info/
--rw-rw-rw-   0        0        0      399 2023-05-28 00:59:45.000000 tablebase-1.6.2/tablebase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-05-28 00:59:45.000000 tablebase-1.6.2/tablebase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 00:59:45.000000 tablebase-1.6.2/tablebase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-28 00:59:45.000000 tablebase-1.6.2/tablebase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 20:18:26.404408 tablebase-1.6.3/
+-rw-rw-rw-   0        0        0     1086 2022-07-18 21:48:23.000000 tablebase-1.6.3/LICENSE
+-rw-rw-rw-   0        0        0     1084 2021-04-03 19:09:23.000000 tablebase-1.6.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1102 2023-05-29 20:18:26.404408 tablebase-1.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0      770 2023-05-29 20:11:43.000000 tablebase-1.6.3/README.md
+-rw-rw-rw-   0        0        0       86 2022-11-01 20:19:29.000000 tablebase-1.6.3/pyproject.toml
+-rw-rw-rw-   0        0        0      443 2023-05-29 20:18:26.464976 tablebase-1.6.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 20:18:26.356405 tablebase-1.6.3/tablebase/
+-rw-rw-rw-   0        0        0       40 2022-05-08 21:07:22.000000 tablebase-1.6.3/tablebase/__init__.py
+-rw-rw-rw-   0        0        0    10725 2023-05-29 19:49:23.000000 tablebase-1.6.3/tablebase/tablebase.py
+drwxrwxrwx   0        0        0        0 2023-05-29 20:18:26.397400 tablebase-1.6.3/tablebase.egg-info/
+-rw-rw-rw-   0        0        0     1102 2023-05-29 20:18:26.000000 tablebase-1.6.3/tablebase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-05-29 20:18:26.000000 tablebase-1.6.3/tablebase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 20:18:26.000000 tablebase-1.6.3/tablebase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-29 20:18:26.000000 tablebase-1.6.3/tablebase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 20:18:26.400401 tablebase-1.6.3/tests/
+-rw-rw-rw-   0        0        0     5368 2023-05-29 19:46:38.000000 tablebase-1.6.3/tests/test.py
```

### Comparing `tablebase-1.6.2/LICENSE` & `tablebase-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tablebase-1.6.2/LICENSE.txt` & `tablebase-1.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tablebase-1.6.2/README.md` & `tablebase-1.6.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Tablebase
 =============
 
-Note: If you found a bug please open an issue. If not create a discussion.
+If you found a bug, need a feature, or have question please open an [issue](https://github.com/sasmlange/tablebase/issues).
 
 All relesses starting at 1.4.2 can be found [here](https://github.com/sasmlange/tablebase/releases)
 
 What is Tablebase?
 ------------------------
 
 Tablebase is a python package to make coding with tables
```

### Comparing `tablebase-1.6.2/tablebase/tablebase.py` & `tablebase-1.6.3/tablebase/tablebase.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,19 +142,18 @@
         :param col_name: The name of your new column.
         :param default_value: The default value for new records in that column or a list of specific values for this column.
         :return:
         """
         self.table_content[0].append(col_name)
 
         for i in range(int(len(self.table_content)) - 1):
-            if type(default_value) is str:
-                self.table_content[i + 1].append(default_value)
-            elif type(default_value) is list:
-
+            if type(default_value) is list:
                 self.table_content[i + 1].append(default_value[i])
+            else:
+                self.table_content[i + 1].append(default_value)
 
     def edit_row(self, row_num, new_value):
         """
         Used to edit a row.
 
         :param row_num: The row number to edit.
         :param new_value: Use a list override a row. If you use a dictionary, the key will be the column name.
@@ -274,13 +273,11 @@
     """
     Used to import a CSV file.
 
     :param csv_path: The path to your CSV
     :param divider: The divider between columns.
     """
     def __init__(self, csv_path, divider=","):
-        self.csv_path = csv_path
-
         with open(csv_path) as csv_file:
             csv_content_list = list(csv.reader(csv_file, delimiter=divider))
 
         self.table_content = csv_content_list
```

