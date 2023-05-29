# Comparing `tmp/tksheet-6.1.9.tar.gz` & `tmp/tksheet-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-6.1.9.tar", last modified: Wed May 24 13:05:23 2023, max compression
+gzip compressed data, was "tksheet-6.2.0.tar", last modified: Mon May 29 11:30:32 2023, max compression
```

## Comparing `tksheet-6.1.9.tar` & `tksheet-6.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 13:05:23.351043 tksheet-6.1.9/
--rw-rw-rw-   0        0        0     1101 2023-05-23 07:18:56.000000 tksheet-6.1.9/LICENSE.txt
--rw-rw-rw-   0        0        0     3657 2023-05-24 13:05:23.351043 tksheet-6.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     3007 2023-05-23 07:18:56.000000 tksheet-6.1.9/README.md
--rw-rw-rw-   0        0        0       86 2023-05-24 13:05:23.351043 tksheet-6.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1010 2023-05-24 11:43:22.000000 tksheet-6.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 13:05:23.351043 tksheet-6.1.9/tksheet/
--rw-rw-rw-   0        0        0     1901 2023-05-23 07:18:56.000000 tksheet-6.1.9/tksheet/__init__.py
--rw-rw-rw-   0        0        0   164362 2023-05-23 15:59:10.000000 tksheet-6.1.9/tksheet/_tksheet.py
--rw-rw-rw-   0        0        0   111722 2023-05-23 16:04:58.000000 tksheet-6.1.9/tksheet/_tksheet_column_headers.py
--rw-rw-rw-   0        0        0     8846 2023-05-23 07:18:56.000000 tksheet-6.1.9/tksheet/_tksheet_formatters.py
--rw-rw-rw-   0        0        0   333268 2023-05-24 13:01:11.000000 tksheet-6.1.9/tksheet/_tksheet_main_table.py
--rw-rw-rw-   0        0        0    12695 2023-05-23 07:18:57.000000 tksheet-6.1.9/tksheet/_tksheet_other_classes.py
--rw-rw-rw-   0        0        0   108646 2023-05-23 16:03:40.000000 tksheet-6.1.9/tksheet/_tksheet_row_index.py
--rw-rw-rw-   0        0        0     5746 2023-05-23 07:18:57.000000 tksheet-6.1.9/tksheet/_tksheet_top_left_rectangle.py
--rw-rw-rw-   0        0        0    59987 2023-05-23 07:18:57.000000 tksheet-6.1.9/tksheet/_tksheet_vars.py
-drwxrwxrwx   0        0        0        0 2023-05-24 13:05:23.351043 tksheet-6.1.9/tksheet.egg-info/
--rw-rw-rw-   0        0        0     3657 2023-05-24 13:05:23.000000 tksheet-6.1.9/tksheet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-05-24 13:05:23.000000 tksheet-6.1.9/tksheet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 13:05:23.000000 tksheet-6.1.9/tksheet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-24 13:05:23.000000 tksheet-6.1.9/tksheet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 11:30:32.240130 tksheet-6.2.0/
+-rw-rw-rw-   0        0        0     1101 2023-05-28 17:19:38.000000 tksheet-6.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     3657 2023-05-29 11:30:32.240130 tksheet-6.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3007 2023-05-28 17:19:38.000000 tksheet-6.2.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-29 11:30:32.240130 tksheet-6.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1010 2023-05-28 17:20:16.000000 tksheet-6.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 11:30:32.240130 tksheet-6.2.0/tksheet/
+-rw-rw-rw-   0        0        0     1901 2023-05-28 17:19:38.000000 tksheet-6.2.0/tksheet/__init__.py
+-rw-rw-rw-   0        0        0   164380 2023-05-29 09:52:00.000000 tksheet-6.2.0/tksheet/_tksheet.py
+-rw-rw-rw-   0        0        0   111722 2023-05-28 17:19:38.000000 tksheet-6.2.0/tksheet/_tksheet_column_headers.py
+-rw-rw-rw-   0        0        0     8844 2023-05-29 11:00:01.000000 tksheet-6.2.0/tksheet/_tksheet_formatters.py
+-rw-rw-rw-   0        0        0   333219 2023-05-29 09:49:54.000000 tksheet-6.2.0/tksheet/_tksheet_main_table.py
+-rw-rw-rw-   0        0        0    12695 2023-05-28 17:19:39.000000 tksheet-6.2.0/tksheet/_tksheet_other_classes.py
+-rw-rw-rw-   0        0        0   108646 2023-05-28 17:19:39.000000 tksheet-6.2.0/tksheet/_tksheet_row_index.py
+-rw-rw-rw-   0        0        0     5746 2023-05-28 17:19:39.000000 tksheet-6.2.0/tksheet/_tksheet_top_left_rectangle.py
+-rw-rw-rw-   0        0        0    59987 2023-05-28 17:19:39.000000 tksheet-6.2.0/tksheet/_tksheet_vars.py
+drwxrwxrwx   0        0        0        0 2023-05-29 11:30:32.240130 tksheet-6.2.0/tksheet.egg-info/
+-rw-rw-rw-   0        0        0     3657 2023-05-29 11:30:32.000000 tksheet-6.2.0/tksheet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-05-29 11:30:32.000000 tksheet-6.2.0/tksheet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 11:30:32.000000 tksheet-6.2.0/tksheet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-29 11:30:32.000000 tksheet-6.2.0/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-6.1.9/LICENSE.txt` & `tksheet-6.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.9/PKG-INFO` & `tksheet-6.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.1.9
+Version: 6.2.0
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.1.9.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.2.0.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `tksheet-6.1.9/README.md` & `tksheet-6.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.9/setup.py` & `tksheet-6.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding = 'utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'tksheet',
   packages = ['tksheet'],
-  version = '6.1.9',
+  version = '6.2.0',
   python_requires = '>=3.6',
   license = 'MIT',
   description = 'Tkinter table / sheet widget',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'ragardner',
   author_email = 'github@ragardner.simplelogin.com',
   url = 'https://github.com/ragardner/tksheet',
-  download_url = 'https://github.com/ragardner/tksheet/archive/6.1.9.tar.gz',
+  download_url = 'https://github.com/ragardner/tksheet/archive/6.2.0.tar.gz',
   keywords = ['tkinter', 'table', 'widget', 'sheet', 'grid', 'tk'],
   install_requires = [],
   classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License'
```

### Comparing `tksheet-6.1.9/tksheet/__init__.py` & `tksheet-6.2.0/tksheet/__init__.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.9/tksheet/_tksheet.py` & `tksheet-6.2.0/tksheet/_tksheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import tkinter as tk
 from collections import deque
 from itertools import accumulate, chain, islice
 from tkinter import ttk
 import bisect
-from typing import Union, Callable
+from typing import Union, Callable, List, Set, Tuple
 
 from ._tksheet_column_headers import ColumnHeaders
 from ._tksheet_main_table import MainTable
 from ._tksheet_other_classes import (
     GeneratedMouseEvent,
     SelectCellEvent,
     dropdown_search_function,
@@ -40,16 +40,16 @@
         show_top_left: bool = True,
         show_row_index: bool = True,
         show_header: bool = True,
         show_x_scrollbar: bool = True,
         show_y_scrollbar: bool = True,
         width: int = None,
         height: int = None,
-        headers: list = None,
-        header: list = None,
+        headers: List = None,
+        header: List = None,
         default_header: str = "letters",  # letters, numbers or both
         default_row_index: str = "numbers",  # letters, numbers or both
         to_clipboard_delimiter="\t",
         to_clipboard_quotechar='"',
         to_clipboard_lineterminator="\n",
         from_clipboard_delimiters=["\t"],
         show_default_header_for_empty: bool = True,
@@ -58,52 +58,52 @@
         expand_sheet_if_paste_too_big: bool = False,
         paste_insert_column_limit: int = None,
         paste_insert_row_limit: int = None,
         show_dropdown_borders: bool = False,
         arrow_key_down_right_scroll_page: bool = False,
         enable_edit_cell_auto_resize: bool = True,
         edit_cell_validation: bool = True,
-        data_reference: list = None,
-        data: list = None,
+        data_reference: List = None,
+        data: List = None,
         # either (start row, end row, "rows"),
         #     or (start column, end column, "columns")
         # or (cells start row,
         #     cells start column,
         #     cells end row,
         #     cells end column,
         #     "cells")
-        startup_select: tuple = None,
+        startup_select: Tuple = None,
         startup_focus: bool = True,
         total_columns: int = None,
         total_rows: int = None,
         column_width: int = 120,
         header_height: str = "1",  # str or int
         max_column_width: str = "inf",  # str or int
         max_row_height: str = "inf",  # str or int
         max_header_height: str = "inf",  # str or int
         max_index_width: str = "inf",  # str or int
-        row_index: list = None,
-        index: list = None,
+        row_index: List = None,
+        index: List = None,
         after_redraw_time_ms: int = 20,
         row_index_width: int = None,
         auto_resize_default_row_index: bool = True,
         auto_resize_columns: Union[int, None] = None,
         auto_resize_rows: Union[int, None] = None,
         set_all_heights_and_widths: bool = False,
         row_height: str = "1",  # str or int
-        font: tuple = get_font(),
-        header_font: tuple = get_heading_font(),
-        index_font: tuple = get_index_font(),  # currently has no effect
-        popup_menu_font: tuple = get_font(),
+        font: Tuple = get_font(),
+        header_font: Tuple = get_heading_font(),
+        index_font: Tuple = get_index_font(),  # currently has no effect
+        popup_menu_font: Tuple = get_font(),
         align: str = "w",
         header_align: str = "center",
         row_index_align: str = "center",
-        displayed_columns: list = [],
+        displayed_columns: List = [],
         all_columns_displayed: bool = True,
-        displayed_rows: list = [],
+        displayed_rows: List = [],
         all_rows_displayed: bool = True,
         max_undos: int = 30,
         outline_thickness: int = 0,
         outline_color: str = theme_light_blue["outline_color"],
         column_drag_and_drop_perform: bool = True,
         row_drag_and_drop_perform: bool = True,
         empty_horizontal: int = 150,
@@ -831,15 +831,15 @@
 
     def emit_event(self, event, data={}):
         self.event_generate(event, data=data)
 
     def bind_event(self, sequence: str, func: Callable, add: Union[str, None] = None) -> None:
         widget = self
 
-        def _substitute(*args) -> tuple[None]:
+        def _substitute(*args) -> Tuple[None]:
             def e() -> None:
                 return None
 
             e.data = args[0]
             e.widget = widget
             return (e,)
 
@@ -1131,15 +1131,15 @@
                 if verify:
                     self.MT.row_positions = [
                         qmin if z < qmin or not isinstance(z, int) or isinstance(z, bool) else z for z in row_heights
                     ]
                 else:
                     self.MT.row_positions = list(accumulate(chain([0], (height for height in row_heights))))
 
-    def verify_row_heights(self, row_heights: list, canvas_positions=False):
+    def verify_row_heights(self, row_heights: List, canvas_positions=False):
         if row_heights[0] != 0 or isinstance(row_heights[0], bool):
             return False
         if not isinstance(row_heights, list):
             return False
         if canvas_positions:
             if any(
                 x - z < self.MT.min_row_height or not isinstance(x, int) or isinstance(x, bool)
@@ -1147,15 +1147,15 @@
             ):
                 return False
         elif not canvas_positions:
             if any(z < self.MT.min_row_height or not isinstance(z, int) or isinstance(z, bool) for z in row_heights):
                 return False
         return True
 
-    def verify_column_widths(self, column_widths: list, canvas_positions=False):
+    def verify_column_widths(self, column_widths: List, canvas_positions=False):
         if column_widths[0] != 0 or isinstance(column_widths[0], bool):
             return False
         if not isinstance(column_widths, list):
             return False
         if canvas_positions:
             if any(
                 x - z < self.MT.min_column_width or not isinstance(x, int) or isinstance(x, bool)
@@ -1213,15 +1213,15 @@
     def delete_row_position(self, idx: int, deselect_all=False):
         self.MT.del_row_position(idx=idx, deselect_all=deselect_all)
 
     def delete_row(self, idx=0, deselect_all=False, redraw=True):
         self.delete_rows(rows={idx}, deselect_all=deselect_all, redraw=False)
         self.set_refresh_timer(redraw)
 
-    def delete_rows(self, rows: set = set(), deselect_all=False, redraw=True):
+    def delete_rows(self, rows: Set = set(), deselect_all=False, redraw=True):
         if deselect_all:
             self.deselect("all", redraw=False)
         if isinstance(rows, set):
             to_del = rows
         else:
             to_del = set(rows)
         if not to_del:
@@ -1346,15 +1346,15 @@
     def delete_column_position(self, idx: int, deselect_all=False):
         self.MT.del_col_position(idx, deselect_all=deselect_all)
 
     def delete_column(self, idx=0, deselect_all=False, redraw=True):
         self.delete_columns(columns={idx}, deselect_all=deselect_all, redraw=False)
         self.set_refresh_timer(redraw)
 
-    def delete_columns(self, columns: set = set(), deselect_all=False, redraw=True):
+    def delete_columns(self, columns: Set = set(), deselect_all=False, redraw=True):
         if deselect_all:
             self.deselect("all", redraw=False)
         if isinstance(columns, set):
             to_del = columns
         else:
             to_del = set(columns)
         if not to_del:
@@ -2693,15 +2693,15 @@
                 if c >= len(self.MT.data[rn]):
                     self.MT.fix_row_len(rn, c)
                 self.set_cell_data(r=rn, c=c, value=v, redraw=False, keep_formatting=keep_formatting)
         self.set_refresh_timer(redraw)
 
     def insert_column(
         self,
-        values: Union[list, tuple, int, None] = None,
+        values: Union[List, Tuple, int, None] = None,
         idx: Union[str, int] = "end",
         width=None,
         deselect_all=False,
         add_rows=True,
         equalize_data_row_lengths=True,
         mod_column_positions=True,
         redraw=True,
@@ -2715,15 +2715,15 @@
             equalize_data_row_lengths,
             mod_column_positions,
             redraw,
         )
 
     def insert_columns(
         self,
-        columns: Union[list, tuple, int, None] = 1,
+        columns: Union[List, Tuple, int, None] = 1,
         idx: Union[str, int] = "end",
         widths=None,
         deselect_all=False,
         add_rows=True,
         equalize_data_row_lengths=True,
         mod_column_positions=True,
         redraw=True,
@@ -2804,15 +2804,15 @@
             }
             self.MT.col_options = {cn if cn < idx else cn + num_add: t for cn, t in self.MT.col_options.items()}
             self.CH.cell_options = {cn if cn < idx else cn + num_add: t for cn, t in self.CH.cell_options.items()}
         self.set_refresh_timer(redraw)
 
     def insert_row(
         self,
-        values: Union[list, None] = None,
+        values: Union[List, None] = None,
         idx: Union[str, int] = "end",
         height=None,
         deselect_all=False,
         add_columns=False,
         mod_row_positions=True,
         redraw=True,
     ):
@@ -2824,15 +2824,15 @@
             add_columns=add_columns,
             mod_row_positions=mod_row_positions,
             redraw=redraw,
         )
 
     def insert_rows(
         self,
-        rows: Union[list, int] = 1,
+        rows: Union[List, int] = 1,
         idx: Union[str, int] = "end",
         heights=None,
         deselect_all=False,
         add_columns=True,
         mod_row_positions=True,
         redraw=True,
     ):
```

### Comparing `tksheet-6.1.9/tksheet/_tksheet_column_headers.py` & `tksheet-6.2.0/tksheet/_tksheet_column_headers.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.9/tksheet/_tksheet_formatters.py` & `tksheet-6.2.0/tksheet/_tksheet_formatters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Union
+from typing import Any, Union, Dict
 
 from ._tksheet_vars import (
     falsy,
     nonelike,
     truthy,
 )
 
@@ -60,67 +60,67 @@
     try:
         to_bool(v)
         return True
     except Exception:
         return False
 
 
-def to_str(v: Any, **kwargs: dict) -> str:
+def to_str(v: Any, **kwargs: Dict) -> str:
     return f"{v}"
 
 
-def float_to_str(v: Union[int, float], **kwargs: dict) -> str:
+def float_to_str(v: Union[int, float], **kwargs: Dict) -> str:
     if isinstance(v, float):
         if v.is_integer():
             return f"{int(v)}"
         if "decimals" in kwargs and isinstance(kwargs["decimals"], int):
             if kwargs["decimals"]:
                 return f"{round(v, kwargs['decimals'])}"
             return f"{int(round(v, kwargs['decimals']))}"
     return f"{v}"
 
 
-def percentage_to_str(v: Union[int, float], **kwargs: dict) -> str:
+def percentage_to_str(v: Union[int, float], **kwargs: Dict) -> str:
     if isinstance(v, (int, float)):
         x = v * 100
         if isinstance(x, float):
             if x.is_integer():
                 return f"{int(x)}%"
             if "decimals" in kwargs and isinstance(kwargs["decimals"], int):
                 if kwargs["decimals"]:
                     return f"{round(x, kwargs['decimals'])}%"
                 return f"{int(round(x, kwargs['decimals']))}%"
     return f"{x}%"
 
 
-def bool_to_str(v: Any, **kwargs: dict) -> str:
+def bool_to_str(v: Any, **kwargs: Dict) -> str:
     return f"{v}"
 
 
 def int_formatter(
     datatypes=int,
     format_function=to_int,
     to_str_function=to_str,
     **kwargs,
-) -> dict:
+) -> Dict:
     return formatter(
         datatypes=datatypes,
         format_function=format_function,
         to_str_function=to_str_function,
         **kwargs,
     )
 
 
 def float_formatter(
     datatypes=float,
     format_function=to_float,
     to_str_function=float_to_str,
     decimals=2,
     **kwargs,
-) -> dict:
+) -> Dict:
     return formatter(
         datatypes=datatypes,
         format_function=format_function,
         to_str_function=to_str_function,
         decimals=decimals,
         **kwargs,
     )
@@ -128,15 +128,15 @@
 
 def percentage_formatter(
     datatypes=float,
     format_function=to_float,
     to_str_function=percentage_to_str,
     decimals=2,
     **kwargs,
-) -> dict:
+) -> Dict:
     return formatter(
         datatypes=datatypes,
         format_function=format_function,
         to_str_function=to_str_function,
         decimals=decimals,
         **kwargs,
     )
@@ -146,15 +146,15 @@
     datatypes=bool,
     format_function=to_bool,
     to_str_function=bool_to_str,
     invalid_value="NA",
     truthy_values=truthy,
     falsy_values=falsy,
     **kwargs,
-) -> dict:
+) -> Dict:
     return formatter(
         datatypes=datatypes,
         format_function=format_function,
         to_str_function=to_str_function,
         invalid_value=invalid_value,
         truthy_values=truthy_values,
         falsy_values=falsy_values,
@@ -168,15 +168,15 @@
     to_str_function=to_str,
     invalid_value="NaN",
     nullable=True,
     pre_format_function=None,
     post_format_function=None,
     clipboard_function=None,
     **kwargs,
-) -> dict:
+) -> Dict:
     return {
         **dict(
             datatypes=datatypes,
             format_function=format_function,
             to_str_function=to_str_function,
             invalid_value=invalid_value,
             nullable=nullable,
@@ -307,15 +307,15 @@
     def get_clipboard_data(self):
         if self.clipboard_function is not None:
             return self.clipboard_function(self.value, **self.kwargs)
         if isinstance(self.value, (int, float, bool)):
             return self.value
         return self.__str__()
 
-    def __eq__(self, __value: object) -> bool:
+    def __eq__(self, __value) -> bool:
         # in case of custom formatter class
         # compare the values
         try:
             if hasattr(__value, "value"):
                 return self.value == __value.value
         except Exception:
             pass
```

### Comparing `tksheet-6.1.9/tksheet/_tksheet_main_table.py` & `tksheet-6.2.0/tksheet/_tksheet_main_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import tkinter as tk
 import zlib
 from collections import defaultdict, deque
 from itertools import accumulate, chain, cycle, islice, product, repeat
 from math import ceil, floor
 from tkinter import TclError
 from typing import Any, Union
-
 from ._tksheet_formatters import (
     data_to_str,
     format_data,
     get_clipboard_data,
     get_data_with_valid_check,
     is_bool_like,
     try_to_bool,
@@ -332,18 +331,18 @@
         self.popup_menu_highlight_bg = kwargs["popup_menu_highlight_bg"]
         self.popup_menu_highlight_fg = kwargs["popup_menu_highlight_fg"]
         self.rc_popup_menu = None
         self.empty_rc_popup_menu = None
         self.basic_bindings()
         self.create_rc_menus()
 
-    def refresh(self, event=None) -> None:
+    def refresh(self, event=None):
         self.main_table_redraw_grid_and_text(True, True)
 
-    def window_configured(self, event) -> None:
+    def window_configured(self, event):
         w = self.parentframe.winfo_width()
         if w != self.parentframe_width:
             self.parentframe_width = w
             self.allow_auto_resize_columns = True
         h = self.parentframe.winfo_height()
         if h != self.parentframe_height:
             self.parentframe_height = h
@@ -3502,15 +3501,15 @@
                 self.get_lines_cell_height(int(self.default_header_height[0]), font=self.header_font)
                 if self.default_header_height[0] != "pixels"
                 else self.default_header_height[1],
             )
         self.set_min_column_width()
         self.CH.set_height(self.default_header_height[1], set_TL=True)
 
-    def set_index_font(self, newfont: Union[tuple, None] = None) -> tuple:
+    def set_index_font(self, newfont=None):
         if newfont:
             if not isinstance(newfont, tuple):
                 raise ValueError("Argument must be tuple e.g. ('Carlito', 12, 'normal')")
             if len(newfont) != 3:
                 raise ValueError("Argument must be three-tuple")
             if not isinstance(newfont[0], str) or not isinstance(newfont[1], int) or not isinstance(newfont[2], str):
                 raise ValueError(
```

### Comparing `tksheet-6.1.9/tksheet/_tksheet_other_classes.py` & `tksheet-6.2.0/tksheet/_tksheet_other_classes.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.9/tksheet/_tksheet_row_index.py` & `tksheet-6.2.0/tksheet/_tksheet_row_index.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.9/tksheet/_tksheet_top_left_rectangle.py` & `tksheet-6.2.0/tksheet/_tksheet_top_left_rectangle.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.9/tksheet/_tksheet_vars.py` & `tksheet-6.2.0/tksheet/_tksheet_vars.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.9/tksheet.egg-info/PKG-INFO` & `tksheet-6.2.0/tksheet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.1.9
+Version: 6.2.0
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.1.9.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.2.0.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

