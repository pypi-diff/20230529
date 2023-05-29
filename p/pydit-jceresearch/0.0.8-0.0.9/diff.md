# Comparing `tmp/pydit-jceresearch-0.0.8.tar.gz` & `tmp/pydit-jceresearch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydit-jceresearch-0.0.8.tar", max compression
+gzip compressed data, was "pydit-jceresearch-0.0.9.tar", max compression
```

## Comparing `pydit-jceresearch-0.0.8.tar` & `pydit-jceresearch-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0     1069 2022-05-02 20:49:00.676018 pydit-jceresearch-0.0.8/LICENSE
--rw-r--r--   0        0        0      330 2022-07-03 06:34:33.925858 pydit-jceresearch-0.0.8/pydit/__init__.py
--rw-r--r--   0        0        0    14076 2022-07-13 20:12:18.435178 pydit-jceresearch-0.0.8/pydit/filemanager.py
--rw-r--r--   0        0        0     1637 2022-07-03 05:58:28.788651 pydit-jceresearch-0.0.8/pydit/functions/__init__.py
--rw-r--r--   0        0        0     5389 2022-06-05 11:30:21.104652 pydit-jceresearch-0.0.8/pydit/functions/anonymise.py
--rw-r--r--   0        0        0     8838 2022-07-09 20:22:24.464033 pydit-jceresearch-0.0.8/pydit/functions/benford.py
--rw-r--r--   0        0        0     3763 2022-06-19 14:26:39.547105 pydit-jceresearch-0.0.8/pydit/functions/blanks.py
--rw-r--r--   0        0        0     2541 2022-07-09 19:02:06.754596 pydit-jceresearch-0.0.8/pydit/functions/calendar.py
--rw-r--r--   0        0        0     4465 2022-06-07 07:08:57.271637 pydit-jceresearch-0.0.8/pydit/functions/cleanup_dataframe_columns_names.py
--rw-r--r--   0        0        0     3472 2022-07-13 20:12:18.428691 pydit-jceresearch-0.0.8/pydit/functions/coalesce_dataframe_columns.py
--rw-r--r--   0        0        0     3696 2022-06-20 20:59:59.202509 pydit-jceresearch-0.0.8/pydit/functions/coalesce_dataframe_values.py
--rw-r--r--   0        0        0     1775 2022-06-04 20:58:00.602842 pydit-jceresearch-0.0.8/pydit/functions/collapse_dataframe_levels.py
--rw-r--r--   0        0        0     8880 2022-07-03 05:47:05.701180 pydit-jceresearch-0.0.8/pydit/functions/counts.py
--rw-r--r--   0        0        0     6073 2022-07-11 07:34:55.965982 pydit-jceresearch-0.0.8/pydit/functions/duplicates.py
--rw-r--r--   0        0        0     4749 2022-07-03 05:47:05.701533 pydit-jceresearch-0.0.8/pydit/functions/fillna.py
--rw-r--r--   0        0        0     3550 2022-07-16 20:37:30.450360 pydit-jceresearch-0.0.8/pydit/functions/groupby_text_concatenate.py
--rw-r--r--   0        0        0    10200 2022-07-09 16:39:40.083694 pydit-jceresearch-0.0.8/pydit/functions/keyword_search_batch.py
--rw-r--r--   0        0        0     2109 2022-07-03 05:47:05.701774 pydit-jceresearch-0.0.8/pydit/functions/merge.py
--rw-r--r--   0        0        0     3226 2022-06-07 07:29:34.574311 pydit-jceresearch-0.0.8/pydit/functions/percentile.py
--rw-r--r--   0        0        0     3212 2022-07-03 05:47:05.702131 pydit-jceresearch-0.0.8/pydit/functions/profile_dataframe_statistics.py
--rw-r--r--   0        0        0     9016 2022-06-04 20:50:39.796910 pydit-jceresearch-0.0.8/pydit/functions/referential_integrity_check.py
--rw-r--r--   0        0        0     3555 2022-06-04 20:44:01.604426 pydit-jceresearch-0.0.8/pydit/functions/sequence.py
--rw-r--r--   0        0        0     2611 2022-06-19 14:48:26.368420 pydit-jceresearch-0.0.8/pydit/functions/truncate_datetime.py
--rw-r--r--   0        0        0     2260 2022-07-03 05:47:05.702686 pydit-jceresearch-0.0.8/pydit/logger.py
--rw-r--r--   0        0        0     6695 2022-06-09 05:09:49.973753 pydit-jceresearch-0.0.8/pydit/utils.py
--rw-r--r--   0        0        0      746 2022-07-16 20:42:57.515318 pydit-jceresearch-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      747 2022-07-16 21:06:44.040609 pydit-jceresearch-0.0.8/setup.py
--rw-r--r--   0        0        0      860 2022-07-16 21:06:44.040991 pydit-jceresearch-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-05-02 20:49:00.676018 pydit-jceresearch-0.0.9/LICENSE
+-rw-r--r--   0        0        0      448 2022-08-07 19:25:06.120393 pydit-jceresearch-0.0.9/pydit/__init__.py
+-rw-r--r--   0        0        0    15220 2022-08-20 07:56:58.878136 pydit-jceresearch-0.0.9/pydit/filemanager.py
+-rw-r--r--   0        0        0     1557 2022-08-20 07:58:18.211694 pydit-jceresearch-0.0.9/pydit/functions/__init__.py
+-rw-r--r--   0        0        0     5389 2022-06-05 11:30:21.104652 pydit-jceresearch-0.0.9/pydit/functions/anonymise.py
+-rw-r--r--   0        0        0     8838 2022-07-09 20:22:24.464033 pydit-jceresearch-0.0.9/pydit/functions/benford.py
+-rw-r--r--   0        0        0     3763 2022-06-19 14:26:39.547105 pydit-jceresearch-0.0.9/pydit/functions/blanks.py
+-rw-r--r--   0        0        0     2556 2022-08-11 19:22:53.687135 pydit-jceresearch-0.0.9/pydit/functions/calendar_table.py
+-rw-r--r--   0        0        0     1110 2022-07-30 20:06:52.731433 pydit-jceresearch-0.0.9/pydit/functions/charts.py
+-rw-r--r--   0        0        0     5213 2022-08-20 09:08:24.094330 pydit-jceresearch-0.0.9/pydit/functions/cleanup_dataframe_columns_names.py
+-rw-r--r--   0        0        0     3472 2022-07-13 20:12:18.428691 pydit-jceresearch-0.0.9/pydit/functions/coalesce_dataframe_columns.py
+-rw-r--r--   0        0        0     3668 2022-08-01 16:43:32.593256 pydit-jceresearch-0.0.9/pydit/functions/coalesce_dataframe_values.py
+-rw-r--r--   0        0        0     1775 2022-06-04 20:58:00.602842 pydit-jceresearch-0.0.9/pydit/functions/collapse_dataframe_levels.py
+-rw-r--r--   0        0        0     9268 2022-07-30 20:06:52.732497 pydit-jceresearch-0.0.9/pydit/functions/counts.py
+-rw-r--r--   0        0        0     6073 2022-07-11 07:34:55.965982 pydit-jceresearch-0.0.9/pydit/functions/duplicates.py
+-rw-r--r--   0        0        0     4749 2022-07-03 05:47:05.701533 pydit-jceresearch-0.0.9/pydit/functions/fillna.py
+-rw-r--r--   0        0        0     3550 2022-07-16 20:37:30.450360 pydit-jceresearch-0.0.9/pydit/functions/groupby_text_concatenate.py
+-rw-r--r--   0        0        0    10417 2022-08-19 08:29:42.778626 pydit-jceresearch-0.0.9/pydit/functions/keyword_search_batch.py
+-rw-r--r--   0        0        0     2109 2022-07-03 05:47:05.701774 pydit-jceresearch-0.0.9/pydit/functions/merge.py
+-rw-r--r--   0        0        0     3015 2022-08-20 07:56:50.719381 pydit-jceresearch-0.0.9/pydit/functions/percentile.py
+-rw-r--r--   0        0        0     3212 2022-07-03 05:47:05.702131 pydit-jceresearch-0.0.9/pydit/functions/profile_dataframe_statistics.py
+-rw-r--r--   0        0        0     9015 2022-07-30 20:06:52.733261 pydit-jceresearch-0.0.9/pydit/functions/referential_integrity_check.py
+-rw-r--r--   0        0        0     3555 2022-06-04 20:44:01.604426 pydit-jceresearch-0.0.9/pydit/functions/sequence.py
+-rw-r--r--   0        0        0     4240 2022-07-30 20:06:52.733573 pydit-jceresearch-0.0.9/pydit/functions/test.png
+-rw-r--r--   0        0        0     2611 2022-06-19 14:48:26.368420 pydit-jceresearch-0.0.9/pydit/functions/truncate_datetime.py
+-rw-r--r--   0        0        0     5422 2022-07-23 09:07:40.458604 pydit-jceresearch-0.0.9/pydit/logger.py
+-rw-r--r--   0        0        0     6699 2022-08-20 08:00:04.826240 pydit-jceresearch-0.0.9/pydit/utils.py
+-rw-r--r--   0        0        0      759 2022-08-20 11:56:31.249205 pydit-jceresearch-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      747 2022-08-20 11:56:38.169271 pydit-jceresearch-0.0.9/setup.py
+-rw-r--r--   0        0        0      860 2022-08-20 11:56:38.169614 pydit-jceresearch-0.0.9/PKG-INFO
```

### Comparing `pydit-jceresearch-0.0.8/LICENSE` & `pydit-jceresearch-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pydit-jceresearch-0.0.8/pydit/functions/__init__.py` & `pydit-jceresearch-0.0.9/pydit/functions/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """ 
-Sub-package (./functions) containing the core functionality of pydit.
-
-Functions are imported individually so they can be used from pydit directly:
-e.g. pydit.create_calendar()
+Sub-package (./functions) containing the core functionality.
 
 The modules are also self standing, you should be able to copy any .py file
 and import it in your script to use it with no dependencies on other modules.
 
 There are currently no exceptions to this design principle.
 
 """
 
-from .calendar import create_calendar
+from .calendar_table import create_calendar
 from .percentile import add_percentile
 from .profile_dataframe_statistics import profile_dataframe
 from .duplicates import check_duplicates
 from .sequence import check_sequence
 from .referential_integrity_check import check_referential_integrity
 from .fillna import fillna_smart
 from .blanks import check_blanks
@@ -30,12 +27,13 @@
 from .collapse_dataframe_levels import collapse_levels
 from .groupby_text_concatenate import groupby_text
 from .keyword_search_batch import keyword_search
 from .truncate_datetime import truncate_datetime_dataframe
 from .merge import merge_force_suffix
 from .counts import count_related_key
 from .counts import count_values_in_col
+from .charts import chart_bar
 
 
 # Here we import each of the functions in the functions/ directory to have them
 # available in the functions namespace.
 # In turn functions gets imported with * at root
```

### Comparing `pydit-jceresearch-0.0.8/pydit/functions/anonymise.py` & `pydit-jceresearch-0.0.9/pydit/functions/anonymise.py`

 * *Files identical despite different names*

### Comparing `pydit-jceresearch-0.0.8/pydit/functions/benford.py` & `pydit-jceresearch-0.0.9/pydit/functions/benford.py`

 * *Files identical despite different names*

### Comparing `pydit-jceresearch-0.0.8/pydit/functions/blanks.py` & `pydit-jceresearch-0.0.9/pydit/functions/blanks.py`

 * *Files identical despite different names*

### Comparing `pydit-jceresearch-0.0.8/pydit/functions/calendar.py` & `pydit-jceresearch-0.0.9/pydit/functions/calendar_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,16 @@
             - yyyyww (week number), int
             - yyyyq (quarter), int
 
     """
     df = pd.DataFrame({"date": pd.date_range(start, end)})
     df["day"] = df.date.dt.day
     df["month"] = df["date"].dt.month
-    df["week"] = df["date"].dt.week
+    df["week"] = df["date"].dt.isocalendar().week
+
     df["quarter"] = df.date.dt.quarter
     df["year"] = df.date.dt.year
     df["weekend"] = df.date.dt.weekday >= 5
     df["weekday"] = df.date.dt.weekday
 
     df["weekday_name"] = df.date.dt.day_name()
     df["weekday_name_short"] = df.date.dt.day_name().str[0:3]
@@ -73,12 +74,12 @@
     df.insert(3, "yyyyq", (df.year.astype(str) + df.quarter.astype(str)).astype(int))
 
     def _calculate_week_number(d):
         """Calculate the week number for a given date"""
         if d.week == 52 and d.dayofyear < 8:
             return (d.year - 1) * 100 + d.week
         else:
-            return (d.year * 100 )+ d.week
+            return (d.year * 100) + d.week
 
     df["yyyyww"] = df.apply(lambda r: _calculate_week_number(r["date"]), axis=1)
 
     return df
```

### Comparing `pydit-jceresearch-0.0.8/pydit/functions/cleanup_dataframe_columns_names.py` & `pydit-jceresearch-0.0.9/pydit/functions/cleanup_dataframe_columns_names.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,42 @@
 """ Module for cleaning up column names """
 
 import logging
 import string
 import re
 import random
+import unicodedata
+
+import pandas as pd
+
 
 logger = logging.getLogger(__name__)
 
 
+def _strip_accents(text: str) -> str:
+    """Remove accents from an unicode text.
+    Inspired from [StackOverflow][so].
+    [so]: https://stackoverflow.com/questions/517923/what-is-the-best-way-to-remove-accents-in-a-python-unicode-strin
+    """  # noqa: E501
+
+    return "".join(
+        letter
+        for letter in unicodedata.normalize("NFD", text)
+        if not unicodedata.combining(letter)
+    )
+
+
 def _deduplicate_list(
     list_to_deduplicate, default_field_name="column", force_lower_case=True
 ):
     """Internal function for deduplicating a list.
 
     Uses enumerate and a loop, so it is not good for very long lists.
     This function is meant to be used for header/field names, where performance
-    is not a concern given the size of the list being on the 10s.
+    is not a concern given the size of the list to deduplicate.
 
     This is a copy of the corresponding function in the utility module
     V0.1 - 14 May 2022
 
     Parameters
     -----------
 
@@ -83,59 +100,70 @@
                     new_value = el + "_" + _get_random_string(8)
                     if new_value in new_list:
                         return False
         new_list.append(new_value)
     return new_list
 
 
-def cleanup_column_names(df, max_field_name_len=40, inplace=False):
+def cleanup_column_names(obj, max_field_name_len=40, inplace=False):
     """Cleanup the column names of a Pandas dataframe.
 
     e.g. removes non alphanumeric chars, _ instead of space, perc instead
     of %, strips trailing spaces, converts to lowercase.
 
     Parameters
     ----------
-    df : pandas.DataFrame
-        The dataframe to clean up
+    obj : pandas.DataFrame or list of strings
+        The dataframe or a list of strings to clean up.
     max_field_name_len : int, optional, default 40
         The maximum length of the field name
     inplace : bool, optional, default False
         If True, will modify the dataframe inplace
 
     Returns
     -------
     pandas.DataFrame
         Pandas DataFrame with cleaned column names
 
     """
-    prev_cols = list(df.columns)
+    if isinstance(obj, list):
+        prev_cols = obj
+    elif isinstance(obj, pd.DataFrame):
+        prev_cols = list(obj.columns)
+
     new_cols = []
     for e in prev_cols:
         try:
             new = str(e)
         except Exception as e:
             logger.exception(e)
-            new = ""
+            new = "unnamed"
+            continue
+        new = _strip_accents(new)
         new = re.sub("%", "pc", new)
         new = re.sub(r"[^a-zA-Z0-9£$€]", " ", new)
         new = re.sub(" +", " ", new)
         new = new[0:max_field_name_len]
         new = str.lower(new.strip())
         new = re.sub(" +", "_", new)
 
         new_cols.append(new)
     # We apply arbitrary limit of field names to avoid some random issues with importing in
     # other systems, for example PowerBI has a limit of 80 charts for importing column
     # names, just in case keeping this quite low, feel free to increase or remove
     new_cols = _deduplicate_list(new_cols)
+
     if not inplace:
-        df = df.copy()
-    df.columns = new_cols
-    logger.debug("Previous column names:%s", prev_cols)
-    logger.info("New columns names:%s", list(df.columns))
-    if len(df.columns) != len(set(df.columns)):
+        obj = obj.copy()
+    if isinstance(obj, list):
+        for i, v in enumerate(obj):
+            obj[i] = new_cols[i]
+    else:
+        obj.columns = new_cols
+    logger.debug("Previous names:%s", prev_cols)
+    logger.info("New names:%s", list(new_cols))
+    if len(new_cols) != len(set(new_cols)):
         raise ValueError("Duplicated column names remain!!! check what happened")
     if inplace:
         return True
     else:
-        return df
+        return obj
```

### Comparing `pydit-jceresearch-0.0.8/pydit/functions/coalesce_dataframe_columns.py` & `pydit-jceresearch-0.0.9/pydit/functions/coalesce_dataframe_columns.py`

 * *Files identical despite different names*

### Comparing `pydit-jceresearch-0.0.8/pydit/functions/coalesce_dataframe_values.py` & `pydit-jceresearch-0.0.9/pydit/functions/coalesce_dataframe_values.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Parameters
     ----------
     df_in : pandas.DataFrame
         The dataframe to clean up
     cols : list
         The column names to coalesce
     top_n_values_to_keep : int, optional, default 10
-        The number of top values to keep. 
+        The number of top values to keep.
     translation_dict : dict, optional, default None
         A dictionary to use for manual translation/coalescing.
     other_label : str or int, optional, default "OTHER"
         The label to use for the other values.
 
     Returns
     -------
@@ -56,33 +56,31 @@
         if len(cols) == 1:
             col = cols[0]
         elif len(cols) > 1:
 
             def concat_categories(r, cols):
                 try:
                     v = "_".join([str(v) for v in r[cols].values])
-                except Exception as e:
+                except Exception:
                     v = np.NAN
                 return v
 
             col = "_".join(cols)
             df[col] = df.apply(lambda r: concat_categories(r, cols), axis=1)
 
         else:
             return "empty list"
 
     if isinstance(other_label, str):
-        flag_str_label=True
+        flag_str_label = True
     elif isinstance(other_label, int):
-        flag_str_label=False
+        flag_str_label = False
     else:
         raise TypeError("other_label must be a string or an integer")
 
-
-
     if top_n_values_to_keep <= 0:
         raise ValueError("top_n_values_to_keep must be greater than 0")
 
     if translation_dict:
         df[col + "_translate"] = df.apply(
             lambda r: translation_dict[r[col]]
             if r[col] in translation_dict
@@ -105,15 +103,13 @@
             lambda r: str.strip(str.upper(str(r[col])))
             if r[col] in value_counts_topN
             else other_label,
             axis=1,
         )
     else:
         df[col + "_collapsed"] = df.apply(
-            lambda r: r[col]
-            if r[col] in value_counts_topN
-            else other_label,
+            lambda r: r[col] if r[col] in value_counts_topN else other_label,
             axis=1,
         )
     logger.info("Unique values after: %s", len(df[col + "_collapsed"].unique()))
     logger.info("Value counts:\n%s", df[col + "_collapsed"].value_counts())
     return df
```

### Comparing `pydit-jceresearch-0.0.8/pydit/functions/collapse_dataframe_levels.py` & `pydit-jceresearch-0.0.9/pydit/functions/collapse_dataframe_levels.py`

 * *Files identical despite different names*

### Comparing `pydit-jceresearch-0.0.8/pydit/functions/counts.py` & `pydit-jceresearch-0.0.9/pydit/functions/counts.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 import logging
 
 import pandas as pd
 
 logger = logging.getLogger(__name__)
 
 
-def count_values_in_col(df, col, column_name=None, combined=False, inplace=False):
+def count_values_in_col(
+    df, col, column_name=None, combined=False, percentage=False, inplace=False
+):
     """Generates a column counting occurrence of values in a given column.
 
     If several columns provided, it will generate a column for each of them, but
     if combined is True, it will generate a column counting unique
     combinations of values in the columns.
 
 
@@ -24,18 +26,21 @@
         col : str or list of str
             Name of the column containing values to tally
         column_name : str or list of str, optional, default None
             Name of the columns to be created containing the count of values
             If None, the column name will be "count_[col]".
         combined : bool, optional, default False
             Whether or not compute the counts combining all the columns provided
+        percentage: bool, optional, default False
+            Whether to return percentage over total count
         inplace : bool, optional, default False
             Whether or not to mutate the original DataFrame
 
 
+
         Returns
         -------
         pd.DataFrame
             New dataframe with a new column containing the count of values
             If inplace is True, the original DataFrame is modified.
 
     """
@@ -56,15 +61,17 @@
             raise TypeError("column_name must be a string or list of strings")
         else:
             flag_auto_name = True  # we ignore the column_name
     elif isinstance(col, list):
         cols_list = col
         if isinstance(column_name, list):
             if len(column_name) != len(cols_list):
-                raise ValueError("column_name must be the same length as col")
+                raise ValueError(
+                    "column_name, if a list must be the same length as the col list"
+                )
         else:
             flag_auto_name = True  # ignore whatever we put there
     else:
         raise TypeError("Expecting a string or list of strings")
     for c in cols_list:
         if c not in df.columns:
             raise ValueError("Column not found in dataframe")
@@ -79,21 +86,25 @@
         if flag_auto_name:
             cn = "count_combined"
         else:
             cn = column_name[0]
         df[cn] = count_list
     else:
         for i, c in enumerate(cols_list):
-            count_summary = df[c].value_counts(dropna=False)
-            count_list = [count_summary[val] for index, val in enumerate(df[c])]
+            # count_summary = df[c].value_counts(dropna=False)
+            # count_list = [count_summary[val] for index, val in enumerate(df[c])]
             if flag_auto_name:
                 cn = "count_" + c
             else:
                 cn = column_name[i]
-            df[cn] = count_list
+            # df[cn] = count_list
+            df[cn] = df[c].map(df[c].value_counts(dropna=False))
+            if percentage:
+                count_records = float(df.shape[0])
+                df[cn] = df[cn] / count_records
 
     if inplace:
         return True
     return df
 
 
 def count_related_key(df1, df2, left_on="", right_on="", on="", inplace=False):
```

### Comparing `pydit-jceresearch-0.0.8/pydit/functions/duplicates.py` & `pydit-jceresearch-0.0.9/pydit/functions/duplicates.py`

 * *Files identical despite different names*

### Comparing `pydit-jceresearch-0.0.8/pydit/functions/fillna.py` & `pydit-jceresearch-0.0.9/pydit/functions/fillna.py`

 * *Files identical despite different names*

### Comparing `pydit-jceresearch-0.0.8/pydit/functions/groupby_text_concatenate.py` & `pydit-jceresearch-0.0.9/pydit/functions/groupby_text_concatenate.py`

 * *Files identical despite different names*

### Comparing `pydit-jceresearch-0.0.8/pydit/functions/keyword_search_batch.py` & `pydit-jceresearch-0.0.9/pydit/functions/keyword_search_batch.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,30 +108,33 @@
     key_column=None,
 ):
     """
     Searches the keywords in a dataframe or series and returns a matrix of matches
 
     Creates a boolean column in the dataframe, one per keyword
     and a combined column that is True if any of the other columns is True.
-    For simplicity we name columns sequentially as pushing keywords straight
-    as columns may yield error with special characters or duplicated/banned names
+    For simplicity by default we name columns sequentially, pushing keywords
+    straight away as columns may yield error with special characters or
+    duplicated/banned names.
+    If you need labels there is an option to provide them.
 
     Parameters
     ----------
     obj : pandas.DataFrame or pandas.Series
         The dataframe or series to search
     keywords : list
         The list of regular expressions or string keywords to search for.
     columns : list
         The list of columns to search in, if None then all columns are searched
     return_data : str, optional default="full"
-        If "full" then the dataframe is returned,
+        If "full" then the full dataframe is returned, plus hit columns
         If "target" then the target columns and hits are returned,
-        If "hits" then only the boolean columns will be returned
-        if "details" then a dataframe with a hit per row is returned
+        If "result" then only the boolean result columns will be returned,
+        If "detail" then a dataframe with a hit per row is returned
+        If you use "full_hits", "target_hits" or "result_hits" then only hit rows are returned
     regexp : bool, default True
         If True then the keywords are treated as regular expressions, otherwise
         a simpler string search is performed.
     case_sensitive : bool, default False
         If True then the keywords are case sensitive. The most typical
         case is that we do NOT care about case sensitivity.
         Note: use case_sensitive=True and include special prefix (?i) in the
@@ -146,15 +149,15 @@
         the returned dataframe
 
     Returns
     -------
     DataFrame
         A copy of the dataframe with the new hit columns added or just
         the boolean columns for each keyword (depending on return_hit_columns_only)
-        Plus a combined column that is true if any of the other columns is true.
+        Plus a column kw_match_all that is True if any of the other columns is True.
 
     """
 
     # Various input validation
     if not isinstance(keywords, (list, str)):
         raise ValueError("keywords must be a list of strings or a string")
     if isinstance(keywords, str):
@@ -195,27 +198,37 @@
         logger.info("Applying simple keyword search instead of regexp")
     if labels:
         if len(set(labels)) < len(keywords):
             logger.info(
                 "Labels provided are repeated, so they will be rolled up using OR logical operator"
             )
     return_data = return_data.lower()
-    if return_data not in ["full", "target", "hits", "details"]:
-        raise ValueError("return_data must be one of full, target, hits or details")
+    if return_data not in [
+        "full",
+        "target",
+        "result",
+        "detail",
+        "full_hits",
+        "target_hits",
+        "result_hits",
+    ]:
+        raise ValueError(
+            "return_data must be one of full, target, result or detail or ending with _hits"
+        )
 
     if return_data == "full":
         logger.info("Returning full dataframe")
-    if return_data == "hits":
-        logger.info("Returning hits only")
-    if return_data == "details":
+    if return_data == "result":
+        logger.info("Returning results (boolean) columns only")
+    if return_data == "detail":
         logger.info("Returning details")
-    if return_data == "targets":
-        logger.info("Returning targets columns and hits")
+    if return_data == "target":
+        logger.info("Returning target and boolean columns")
 
-    if return_data == "details":
+    if return_data == "detail":
         if key_column is None:
             raise ValueError("Must provide a key column if return_details is True")
         if key_column not in dffull.columns:
             raise ValueError("Key column %s not found in dataframe" % key_column)
 
     # Here the main part of the function starts
     df.fillna("", inplace=True)
@@ -225,37 +238,15 @@
         df["dummy_keyword_search"] = df[columns].astype(str)
 
     if regexp:
         dfres = _keyword_search_re(keywords, df, case_sensitive)
     else:
         dfres = _keyword_search_str(keywords, df, case_sensitive)
 
-    if labels:
-        dfres_labelled = dfres.copy()
-        if len(set(labels)) == len(dfres_labelled.columns):
-            dfres_labelled.columns = labels
-        else:
-            # we are dealing with multiple labels to group
-            dfresg = pd.DataFrame()
-            for l in set(labels):
-                cols = []
-                for i, c in enumerate(dfres_labelled.columns):
-                    if l == labels[i]:
-                        cols.append(c)
-                dfresg[l] = np.logical_or.reduce(dfres_labelled[cols], axis=1)
-            dfres_labelled = dfresg.copy()
-        dfres_labelled["kw_match_all"] = dfres.apply(any, axis=1)
-        # we are using the original dfres here on purpose, the test suite needs
-        # to test that they match against the grouped columns
-
-    # we add the combined any() (ie. or) column to dfres after we processed the
-    # labels because otherwise the list of labels and hits wouldnt match
-    dfres["kw_match_all"] = dfres.apply(any, axis=1)
-
-    if return_data == "details":
+    if "detail" in return_data:
         df = dffull.join(dfres)
         zeroes = max(math.ceil(math.log10(len(keywords))), 2)
         list_hits = []
         for i, kw in enumerate(keywords):
             hit_field = "kw_match" + str.zfill(str(i + 1), zeroes)
             if labels:
                 label = labels[i]
@@ -266,23 +257,41 @@
             dftemp["keyword"] = kw
             list_hits.append(dftemp)
         dfd = pd.concat(list_hits)
         logger.info("Returning search hits details in %s rows", dfd.shape[0])
         return dfd
 
     if labels:
-        df_hits = dfres_labelled
-    else:
-        df_hits = dfres
+        if len(set(labels)) == len(dfres.columns):
+            dfres.columns = labels
+        else:
+            # we are dealing with multiple labels to group
+            dfresg = pd.DataFrame()
+            for l in set(labels):
+                cols = []
+                for i, c in enumerate(dfres.columns):
+                    if l == labels[i]:
+                        cols.append(c)
+                dfresg[l] = np.logical_or.reduce(dfres[cols], axis=1)
+            dfres = dfresg.copy()
+
+    # we add the combined any() (ie. or) column to dfres after we processed the
+    # labels because otherwise the list of labels and hits wouldnt match
+    dfres["kw_match_all"] = dfres.apply(any, axis=1)
+    # we add a hit count column for convenience
+    dfres["kw_match_count"] = dfres.apply(sum, axis=1)
+
+    if "_hits" in return_data:
+        dfres = dfres[dfres["kw_match_all"] == True].copy()
 
-    if return_data == "hits":
-        logger.info("Returning hit columns %s", df_hits.columns)
-        return df_hits
+    if "result" in return_data:
+        logger.info("Returning hit columns %s", dfres.columns)
+        return dfres
 
-    if return_data == "targets":
-        df = df.join(df_hits)
+    if "target" in return_data:
+        df = df[columns].join(dfres).copy()
         logger.info("Returning target columns: %s", df.columns)
         return df
 
-    dffull = dffull.join(df_hits)
+    dffull = dffull.join(dfres).copy()
     logger.info("Returning all columns: %s", dffull.columns)
     return dffull
```

### Comparing `pydit-jceresearch-0.0.8/pydit/functions/merge.py` & `pydit-jceresearch-0.0.9/pydit/functions/merge.py`

 * *Files identical despite different names*

### Comparing `pydit-jceresearch-0.0.8/pydit/functions/percentile.py` & `pydit-jceresearch-0.0.9/pydit/functions/percentile.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,22 +44,14 @@
 
     Returns
     -------
     pandas.DataFrame
         If inplace=False, returns a copy of the dataframe with the new columns added.
         If inplace=True, it will return True, and mutate the original dataframes.
 
-    Examples
-    --------
-    >>> import pydit
-    >>> pydit.start_logging_info()
-    >>> df = pydit.create_test_df()
-    >>> df = pydit.add_percentile(df, "col1")
-    >>> print(list(df("percentile_in_col1")))
-
     """
 
     if not isinstance(df, pd.DataFrame):
         raise TypeError("df must be a pandas DataFrame")
     if not isinstance(col, (str, list)):
         raise TypeError("col must be a string or, at a stretch, a list of one element")
     if isinstance(col, list):
```

### Comparing `pydit-jceresearch-0.0.8/pydit/functions/profile_dataframe_statistics.py` & `pydit-jceresearch-0.0.9/pydit/functions/profile_dataframe_statistics.py`

 * *Files identical despite different names*

### Comparing `pydit-jceresearch-0.0.8/pydit/functions/referential_integrity_check.py` & `pydit-jceresearch-0.0.9/pydit/functions/referential_integrity_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,8 +216,7 @@
                 else:
                     explain(
                         expl,
                         "Both have duplicates and values non shared with each other",
                     )
 
                     return "partial overlap and both have duplicates"
-
```

### Comparing `pydit-jceresearch-0.0.8/pydit/functions/sequence.py` & `pydit-jceresearch-0.0.9/pydit/functions/sequence.py`

 * *Files identical despite different names*

### Comparing `pydit-jceresearch-0.0.8/pydit/functions/truncate_datetime.py` & `pydit-jceresearch-0.0.9/pydit/functions/truncate_datetime.py`

 * *Files identical despite different names*

### Comparing `pydit-jceresearch-0.0.8/pydit/utils.py` & `pydit-jceresearch-0.0.9/pydit/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Utility functions, they are not used directly in the core functions.
 
 The functions below can be used directly.
 However, when needed for a specific core function, instead of importing them, 
 we would create a copy of the function and rename it with an _ prefix.
 This is to ensure that a core function's module is self-standing, ie can be
-used/imported independently of pydit.
+used/imported with no other dependencies.
 
 """
 import random
 import string
 import logging
 import re
 from datetime import datetime
```

### Comparing `pydit-jceresearch-0.0.8/pyproject.toml` & `pydit-jceresearch-0.0.9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "pydit-jceresearch"
 packages = [
 	{ include = "pydit" }
 ]
-version = "0.0.8"
+version = "0.0.9"
 description = "Data cleansing tools for Internal Auditors"
 authors = ["jceresearch <jceresearch@users.noreply.github.com>"]
 keywords=["internal audit", "munging", "cleansing", "audit"]
 classifiers=[
 "Development Status :: 3 - Alpha",
 "Programming Language :: Python :: 3 :: Only",
 "License :: OSI Approved :: MIT License"
@@ -23,9 +23,9 @@
 matplotlib="*"
 myst-parser ="*"
 
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.0.0","setuptools"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pydit-jceresearch-0.0.8/setup.py` & `pydit-jceresearch-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'myst-parser',
  'numpy>=1.22,<2.0',
  'openpyxl>=3.0.0,<4.0.0',
  'pandas>=1.2.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'pydit-jceresearch',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Data cleansing tools for Internal Auditors',
     'long_description': None,
     'author': 'jceresearch',
     'author_email': 'jceresearch@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `pydit-jceresearch-0.0.8/PKG-INFO` & `pydit-jceresearch-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydit-jceresearch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Data cleansing tools for Internal Auditors
 License: MIT
 Keywords: internal audit,munging,cleansing,audit
 Author: jceresearch
 Author-email: jceresearch@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

