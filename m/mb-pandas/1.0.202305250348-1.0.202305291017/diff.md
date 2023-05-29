# Comparing `tmp/mb_pandas-1.0.202305250348-py3-none-any.whl.zip` & `tmp/mb_pandas-1.0.202305291017-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 9349 bytes, number of entries: 13
+Zip file size: 9363 bytes, number of entries: 13
 -rw-rw-r--  2.0 unx      162 b- defN 23-May-25 03:48 mb_pandas/src/__init__.py
 -rw-rw-r--  2.0 unx     1612 b- defN 23-May-25 03:36 mb_pandas/src/aio.py
 -rw-rw-r--  2.0 unx      482 b- defN 23-May-25 03:36 mb_pandas/src/convert_data.py
--rw-rw-r--  2.0 unx     3451 b- defN 23-May-25 03:36 mb_pandas/src/dfload.py
+-rw-rw-r--  2.0 unx     3516 b- defN 23-May-29 10:17 mb_pandas/src/dfload.py
 -rw-rw-r--  2.0 unx     2418 b- defN 23-May-25 03:36 mb_pandas/src/profiler.py
 -rw-rw-r--  2.0 unx     6091 b- defN 23-Apr-04 14:19 mb_pandas/src/transform.py
--rw-rw-r--  2.0 unx      396 b- defN 23-May-25 03:48 mb_pandas/src/version.py
--rwxrwxr-x  2.0 unx     1671 b- defN 23-May-25 03:48 mb_pandas-1.0.202305250348.data/scripts/df_profile
--rwxrwxr-x  2.0 unx     3683 b- defN 23-May-25 03:48 mb_pandas-1.0.202305250348.data/scripts/df_view
--rw-rw-r--  2.0 unx      224 b- defN 23-May-25 03:48 mb_pandas-1.0.202305250348.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-25 03:48 mb_pandas-1.0.202305250348.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-May-25 03:48 mb_pandas-1.0.202305250348.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1128 b- defN 23-May-25 03:48 mb_pandas-1.0.202305250348.dist-info/RECORD
-13 files, 21420 bytes uncompressed, 7441 bytes compressed:  65.3%
+-rw-rw-r--  2.0 unx      396 b- defN 23-May-29 10:17 mb_pandas/src/version.py
+-rwxrwxr-x  2.0 unx     1671 b- defN 23-May-29 10:17 mb_pandas-1.0.202305291017.data/scripts/df_profile
+-rwxrwxr-x  2.0 unx     3683 b- defN 23-May-29 10:17 mb_pandas-1.0.202305291017.data/scripts/df_view
+-rw-rw-r--  2.0 unx      224 b- defN 23-May-29 10:17 mb_pandas-1.0.202305291017.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-29 10:17 mb_pandas-1.0.202305291017.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-May-29 10:17 mb_pandas-1.0.202305291017.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1128 b- defN 23-May-29 10:17 mb_pandas-1.0.202305291017.dist-info/RECORD
+13 files, 21485 bytes uncompressed, 7455 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: mb_pandas/src/transform.py
 Comment: 
 
 Filename: mb_pandas/src/version.py
 Comment: 
 
-Filename: mb_pandas-1.0.202305250348.data/scripts/df_profile
+Filename: mb_pandas-1.0.202305291017.data/scripts/df_profile
 Comment: 
 
-Filename: mb_pandas-1.0.202305250348.data/scripts/df_view
+Filename: mb_pandas-1.0.202305291017.data/scripts/df_view
 Comment: 
 
-Filename: mb_pandas-1.0.202305250348.dist-info/METADATA
+Filename: mb_pandas-1.0.202305291017.dist-info/METADATA
 Comment: 
 
-Filename: mb_pandas-1.0.202305250348.dist-info/WHEEL
+Filename: mb_pandas-1.0.202305291017.dist-info/WHEEL
 Comment: 
 
-Filename: mb_pandas-1.0.202305250348.dist-info/top_level.txt
+Filename: mb_pandas-1.0.202305291017.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_pandas-1.0.202305250348.dist-info/RECORD
+Filename: mb_pandas-1.0.202305291017.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb_pandas/src/dfload.py

```diff
@@ -77,14 +77,16 @@
         file_path (csv): path to csv file/parquet file
         show_progress (bool): show progress bar
         literal_ast_columns (list): columns to be converted to literal ast
         logger (logger): logger object
     Output:
         df (pd.DataFrame): pandas dataframe
     """
+    if type(file_path) == pd.DataFrame:
+        return file_path
     try:
         if file_path.endswith('.csv'):
             df = asyncio.run(load_df_new(file_path,show_progress=show_progress))
         elif file_path.endswith('.parquet'):
             df = asyncio.run(load_df_new_parquet(file_path,show_progress=show_progress))
         if logger:
             logger.info("Loaded dataframe from {} using asyncio".format(file_path))
```

## mb_pandas/src/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('05')
-VERSION_DAY = int('25')
-VERSION_HOUR = int('03')
-VERSION_MINUTE = int('48')
+VERSION_DAY = int('29')
+VERSION_HOUR = int('10')
+VERSION_MINUTE = int('17')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202305250348
-version_date = '2023/05/25 03:48'
+PATCH_VERSION = 202305291017
+version_date = '2023/05/29 10:17'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mb_pandas-1.0.202305250348.data/scripts/df_profile` & `mb_pandas-1.0.202305291017.data/scripts/df_profile`

 * *Files identical despite different names*

## Comparing `mb_pandas-1.0.202305250348.data/scripts/df_view` & `mb_pandas-1.0.202305291017.data/scripts/df_view`

 * *Files identical despite different names*

## Comparing `mb_pandas-1.0.202305250348.dist-info/RECORD` & `mb_pandas-1.0.202305291017.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 mb_pandas/src/__init__.py,sha256=WU80RSEXwgPXneLCZV_JyaMkKzAGEvYo9Icq0QzfBJE,162
 mb_pandas/src/aio.py,sha256=UK3o2TMFDeNQvhiFAulAyd1fKJPjrShEbK-Y-85tlsM,1612
 mb_pandas/src/convert_data.py,sha256=Wp1yDT9Ie-lBZGE7WmsMXB7nN3mv0MwbiloInr1aoc0,482
-mb_pandas/src/dfload.py,sha256=35lcohyvdhIx_a17FxHlCQ5gmSkyGczTG9mqzLFjFzw,3451
+mb_pandas/src/dfload.py,sha256=Yet5dq8R0NDi69UXiUAfQMwbWqhLRGjXqhUvJI5pBSw,3516
 mb_pandas/src/profiler.py,sha256=iX_nAksh-HzjyhQLnbutvEtNVGfVwja2CsQ1zaYZbeA,2418
 mb_pandas/src/transform.py,sha256=Pq-xTzpfktzAlpu4dg42Kd6uoSI5mcq8vHhetFhgDUM,6091
-mb_pandas/src/version.py,sha256=zQ8q7stBym_4gRszoV4UHNEDiwunTug1cWw98ocDYJU,396
-mb_pandas-1.0.202305250348.data/scripts/df_profile,sha256=zi4GRNQ6P5_JEB_0wMYB1KzLRG59eHXxRZG_I84lTYQ,1671
-mb_pandas-1.0.202305250348.data/scripts/df_view,sha256=BbS_rNgrPl7Raz_zVmTBqw_dvyAhc3-KqS4W2LV0_yo,3683
-mb_pandas-1.0.202305250348.dist-info/METADATA,sha256=l7OehfclCftbTEuzFP8xJuWE2kZLbThVSuCYP3_iFXU,224
-mb_pandas-1.0.202305250348.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mb_pandas-1.0.202305250348.dist-info/top_level.txt,sha256=5JkDz2-6yNAp6GiwpeR4FpxqXVysaksS5MD1iAvfMgo,10
-mb_pandas-1.0.202305250348.dist-info/RECORD,,
+mb_pandas/src/version.py,sha256=r9EY8Si-2jT7bo407jqyZmS5iTZeshf1SxOT4X365d4,396
+mb_pandas-1.0.202305291017.data/scripts/df_profile,sha256=zi4GRNQ6P5_JEB_0wMYB1KzLRG59eHXxRZG_I84lTYQ,1671
+mb_pandas-1.0.202305291017.data/scripts/df_view,sha256=BbS_rNgrPl7Raz_zVmTBqw_dvyAhc3-KqS4W2LV0_yo,3683
+mb_pandas-1.0.202305291017.dist-info/METADATA,sha256=B7nAjdhT6Ui67ENDTE5aDn7Aso-gU6B5GlC1iEkG95Q,224
+mb_pandas-1.0.202305291017.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+mb_pandas-1.0.202305291017.dist-info/top_level.txt,sha256=5JkDz2-6yNAp6GiwpeR4FpxqXVysaksS5MD1iAvfMgo,10
+mb_pandas-1.0.202305291017.dist-info/RECORD,,
```

