# Comparing `tmp/csv_to_xls-0.0.2.tar.gz` & `tmp/csv_to_xls-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv_to_xls-0.0.2.tar", last modified: Mon May 29 19:23:53 2023, max compression
+gzip compressed data, was "csv_to_xls-0.0.4.tar", last modified: Mon May 29 19:29:40 2023, max compression
```

## Comparing `csv_to_xls-0.0.2.tar` & `csv_to_xls-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-05-29 19:23:53.952527 csv_to_xls-0.0.2/
--rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 csv_to_xls-0.0.2/LICENSE
--rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 csv_to_xls-0.0.2/MANIFEST.in
--rw-r--r--   0 hamel      (501) staff       (20)     3119 2023-05-29 19:23:53.952363 csv_to_xls-0.0.2/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)     2332 2023-05-29 19:23:37.000000 csv_to_xls-0.0.2/README.md
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-05-29 19:23:53.951202 csv_to_xls-0.0.2/csv_to_xls/
--rw-r--r--   0 hamel      (501) staff       (20)       22 2023-05-29 19:23:31.000000 csv_to_xls-0.0.2/csv_to_xls/__init__.py
--rw-r--r--   0 hamel      (501) staff       (20)      385 2023-05-29 19:23:31.000000 csv_to_xls-0.0.2/csv_to_xls/_modidx.py
--rw-r--r--   0 hamel      (501) staff       (20)     1666 2023-05-29 19:23:31.000000 csv_to_xls-0.0.2/csv_to_xls/core.py
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-05-29 19:23:53.952173 csv_to_xls-0.0.2/csv_to_xls.egg-info/
--rw-r--r--   0 hamel      (501) staff       (20)     3119 2023-05-29 19:23:53.000000 csv_to_xls-0.0.2/csv_to_xls.egg-info/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)      354 2023-05-29 19:23:53.000000 csv_to_xls-0.0.2/csv_to_xls.egg-info/SOURCES.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-05-29 19:23:53.000000 csv_to_xls-0.0.2/csv_to_xls.egg-info/dependency_links.txt
--rw-r--r--   0 hamel      (501) staff       (20)       95 2023-05-29 19:23:53.000000 csv_to_xls-0.0.2/csv_to_xls.egg-info/entry_points.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-05-29 19:14:53.000000 csv_to_xls-0.0.2/csv_to_xls.egg-info/not-zip-safe
--rw-r--r--   0 hamel      (501) staff       (20)       23 2023-05-29 19:23:53.000000 csv_to_xls-0.0.2/csv_to_xls.egg-info/requires.txt
--rw-r--r--   0 hamel      (501) staff       (20)       11 2023-05-29 19:23:53.000000 csv_to_xls-0.0.2/csv_to_xls.egg-info/top_level.txt
--rw-r--r--   0 hamel      (501) staff       (20)      976 2023-05-29 19:23:25.000000 csv_to_xls-0.0.2/settings.ini
--rw-r--r--   0 hamel      (501) staff       (20)       38 2023-05-29 19:23:53.952573 csv_to_xls-0.0.2/setup.cfg
--rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 csv_to_xls-0.0.2/setup.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-05-29 19:29:40.916682 csv_to_xls-0.0.4/
+-rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 csv_to_xls-0.0.4/LICENSE
+-rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 csv_to_xls-0.0.4/MANIFEST.in
+-rw-r--r--   0 hamel      (501) staff       (20)     3386 2023-05-29 19:29:40.916533 csv_to_xls-0.0.4/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)     2599 2023-05-29 19:28:09.000000 csv_to_xls-0.0.4/README.md
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-05-29 19:29:40.915196 csv_to_xls-0.0.4/csv_to_xls/
+-rw-r--r--   0 hamel      (501) staff       (20)       22 2023-05-29 19:29:27.000000 csv_to_xls-0.0.4/csv_to_xls/__init__.py
+-rw-r--r--   0 hamel      (501) staff       (20)      385 2023-05-29 19:29:27.000000 csv_to_xls-0.0.4/csv_to_xls/_modidx.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1666 2023-05-29 19:29:27.000000 csv_to_xls-0.0.4/csv_to_xls/core.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-05-29 19:29:40.916338 csv_to_xls-0.0.4/csv_to_xls.egg-info/
+-rw-r--r--   0 hamel      (501) staff       (20)     3386 2023-05-29 19:29:40.000000 csv_to_xls-0.0.4/csv_to_xls.egg-info/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)      354 2023-05-29 19:29:40.000000 csv_to_xls-0.0.4/csv_to_xls.egg-info/SOURCES.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-05-29 19:29:40.000000 csv_to_xls-0.0.4/csv_to_xls.egg-info/dependency_links.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       95 2023-05-29 19:29:40.000000 csv_to_xls-0.0.4/csv_to_xls.egg-info/entry_points.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-05-29 19:14:53.000000 csv_to_xls-0.0.4/csv_to_xls.egg-info/not-zip-safe
+-rw-r--r--   0 hamel      (501) staff       (20)       32 2023-05-29 19:29:40.000000 csv_to_xls-0.0.4/csv_to_xls.egg-info/requires.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       11 2023-05-29 19:29:40.000000 csv_to_xls-0.0.4/csv_to_xls.egg-info/top_level.txt
+-rw-r--r--   0 hamel      (501) staff       (20)      985 2023-05-29 19:29:14.000000 csv_to_xls-0.0.4/settings.ini
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2023-05-29 19:29:40.916731 csv_to_xls-0.0.4/setup.cfg
+-rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 csv_to_xls-0.0.4/setup.py
```

### Comparing `csv_to_xls-0.0.2/LICENSE` & `csv_to_xls-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `csv_to_xls-0.0.2/PKG-INFO` & `csv_to_xls-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv_to_xls
-Version: 0.0.2
+Version: 0.0.4
 Summary: convert csvs to excel
 Home-page: https://github.com/hamelsmu/csv_to_xls
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
@@ -36,15 +36,16 @@
 When you install `csv_to_xls` you will get a cli tool named `csv2xls`:
 
 ``` python
 !csv2xls --help
 ```
 
     usage: csv2xls [-h] [--file_glob FILE_GLOB] [--out_file OUT_FILE] [--recursive]
-                   [--symlinks] [--file_re FILE_RE] [--folder_re FOLDER_RE]
+                   [--delimiter DELIMITER] [--quotechar QUOTECHAR] [--symlinks]
+                   [--file_re FILE_RE] [--folder_re FOLDER_RE]
                    [--skip_file_glob SKIP_FILE_GLOB] [--skip_file_re SKIP_FILE_RE]
                    [--skip_folder_re SKIP_FOLDER_RE]
                    path
 
     Convert csv file(s) into an excel file, if multiple csvs put on tabs.
 
     positional arguments:
@@ -52,14 +53,17 @@
 
     optional arguments:
       -h, --help                       show this help message and exit
       --file_glob FILE_GLOB            Only include files matching glob (default:
                                        *.csv)
       --out_file OUT_FILE              output excel file (default: output.xlsx)
       --recursive                      search subfolders (default: False)
+      --delimiter DELIMITER            delimiter to use (default: ,)
+      --quotechar QUOTECHAR            quote character to escape the delimiter
+                                       (default: ")
       --symlinks                       follow symlinks? (default: False)
       --file_re FILE_RE                Only include files matching regex
       --folder_re FOLDER_RE            Only enter folders matching regex
       --skip_file_glob SKIP_FILE_GLOB  Skip files matching glob
       --skip_file_re SKIP_FILE_RE      Skip files matching regex
       --skip_folder_re SKIP_FOLDER_RE  Skip folders matching regex,
```

### Comparing `csv_to_xls-0.0.2/README.md` & `csv_to_xls-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 When you install `csv_to_xls` you will get a cli tool named `csv2xls`:
 
 ``` python
 !csv2xls --help
 ```
 
     usage: csv2xls [-h] [--file_glob FILE_GLOB] [--out_file OUT_FILE] [--recursive]
-                   [--symlinks] [--file_re FILE_RE] [--folder_re FOLDER_RE]
+                   [--delimiter DELIMITER] [--quotechar QUOTECHAR] [--symlinks]
+                   [--file_re FILE_RE] [--folder_re FOLDER_RE]
                    [--skip_file_glob SKIP_FILE_GLOB] [--skip_file_re SKIP_FILE_RE]
                    [--skip_folder_re SKIP_FOLDER_RE]
                    path
 
     Convert csv file(s) into an excel file, if multiple csvs put on tabs.
 
     positional arguments:
@@ -29,14 +30,17 @@
 
     optional arguments:
       -h, --help                       show this help message and exit
       --file_glob FILE_GLOB            Only include files matching glob (default:
                                        *.csv)
       --out_file OUT_FILE              output excel file (default: output.xlsx)
       --recursive                      search subfolders (default: False)
+      --delimiter DELIMITER            delimiter to use (default: ,)
+      --quotechar QUOTECHAR            quote character to escape the delimiter
+                                       (default: ")
       --symlinks                       follow symlinks? (default: False)
       --file_re FILE_RE                Only include files matching regex
       --folder_re FOLDER_RE            Only enter folders matching regex
       --skip_file_glob SKIP_FILE_GLOB  Skip files matching glob
       --skip_file_re SKIP_FILE_RE      Skip files matching regex
       --skip_folder_re SKIP_FOLDER_RE  Skip folders matching regex,
```

### Comparing `csv_to_xls-0.0.2/csv_to_xls/core.py` & `csv_to_xls-0.0.4/csv_to_xls/core.py`

 * *Files identical despite different names*

### Comparing `csv_to_xls-0.0.2/csv_to_xls.egg-info/PKG-INFO` & `csv_to_xls-0.0.4/csv_to_xls.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv-to-xls
-Version: 0.0.2
+Version: 0.0.4
 Summary: convert csvs to excel
 Home-page: https://github.com/hamelsmu/csv_to_xls
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
@@ -36,15 +36,16 @@
 When you install `csv_to_xls` you will get a cli tool named `csv2xls`:
 
 ``` python
 !csv2xls --help
 ```
 
     usage: csv2xls [-h] [--file_glob FILE_GLOB] [--out_file OUT_FILE] [--recursive]
-                   [--symlinks] [--file_re FILE_RE] [--folder_re FOLDER_RE]
+                   [--delimiter DELIMITER] [--quotechar QUOTECHAR] [--symlinks]
+                   [--file_re FILE_RE] [--folder_re FOLDER_RE]
                    [--skip_file_glob SKIP_FILE_GLOB] [--skip_file_re SKIP_FILE_RE]
                    [--skip_folder_re SKIP_FOLDER_RE]
                    path
 
     Convert csv file(s) into an excel file, if multiple csvs put on tabs.
 
     positional arguments:
@@ -52,14 +53,17 @@
 
     optional arguments:
       -h, --help                       show this help message and exit
       --file_glob FILE_GLOB            Only include files matching glob (default:
                                        *.csv)
       --out_file OUT_FILE              output excel file (default: output.xlsx)
       --recursive                      search subfolders (default: False)
+      --delimiter DELIMITER            delimiter to use (default: ,)
+      --quotechar QUOTECHAR            quote character to escape the delimiter
+                                       (default: ")
       --symlinks                       follow symlinks? (default: False)
       --file_re FILE_RE                Only include files matching regex
       --folder_re FOLDER_RE            Only enter folders matching regex
       --skip_file_glob SKIP_FILE_GLOB  Skip files matching glob
       --skip_file_re SKIP_FILE_RE      Skip files matching regex
       --skip_folder_re SKIP_FOLDER_RE  Skip folders matching regex,
```

### Comparing `csv_to_xls-0.0.2/settings.ini` & `csv_to_xls-0.0.4/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = csv_to_xls
 lib_name = %(repo)s
-version = 0.0.2
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = csv_to_xls
@@ -34,10 +34,10 @@
 description = convert csvs to excel
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = hamelsmu
 
 ### Optional ###
-requirements = fastcore pandas
+requirements = fastcore pandas openpyxl
 # dev_requirements = 
 console_scripts = csv2xls=csv_to_xls.core:convert
```

### Comparing `csv_to_xls-0.0.2/setup.py` & `csv_to_xls-0.0.4/setup.py`

 * *Files identical despite different names*

