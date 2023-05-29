# Comparing `tmp/dfbrowse-0.1.0.tar.gz` & `tmp/dfbrowse-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfbrowse-0.1.0.tar", max compression
+gzip compressed data, was "dfbrowse-0.1.1.tar", max compression
```

## Comparing `dfbrowse-0.1.0.tar` & `dfbrowse-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11347 2023-05-28 01:46:02.033611 dfbrowse-0.1.0/LICENSE
--rw-r--r--   0        0        0     2161 2023-05-28 21:00:08.337966 dfbrowse-0.1.0/README.md
--rw-r--r--   0        0        0       96 2023-05-28 21:00:08.338178 dfbrowse-0.1.0/dfbrowse/__init__.py
--rwxr-xr-x   0        0        0      805 2023-05-28 21:00:08.338275 dfbrowse-0.1.0/dfbrowse/browse_dataframe_csvs.py
--rw-r--r--   0        0        0      699 2023-05-28 21:00:08.338332 dfbrowse-0.1.0/dfbrowse/browser_utils.py
--rw-r--r--   0        0        0     2505 2023-05-28 21:00:08.338394 dfbrowse-0.1.0/dfbrowse/chunk_search_utils.py
--rw-r--r--   0        0        0    27702 2023-05-28 21:00:08.338576 dfbrowse-0.1.0/dfbrowse/dataframe_browser.py
--rw-r--r--   0        0        0     1806 2023-05-28 21:00:08.338695 dfbrowse-0.1.0/dfbrowse/dataframe_browser_functions.py
--rw-r--r--   0        0        0     2364 2023-05-28 21:00:08.338847 dfbrowse-0.1.0/dfbrowse/dataframe_utils.py
--rw-r--r--   0        0        0      879 2023-05-28 21:00:08.338930 dfbrowse-0.1.0/dfbrowse/func_core.py
--rw-r--r--   0        0        0     1062 2023-05-28 21:00:08.339011 dfbrowse-0.1.0/dfbrowse/gui_debug.py
--rw-r--r--   0        0        0     1794 2023-05-28 21:00:08.339115 dfbrowse-0.1.0/dfbrowse/ipython_cli.py
--rw-r--r--   0        0        0       73 2023-05-28 21:00:08.339207 dfbrowse-0.1.0/dfbrowse/ipython_main.py
--rw-r--r--   0        0        0     1316 2023-05-28 21:00:08.339301 dfbrowse-0.1.0/dfbrowse/ipython_utils.py
--rw-r--r--   0        0        0     3249 2023-05-28 21:00:08.339415 dfbrowse-0.1.0/dfbrowse/keybindings.py
--rw-r--r--   0        0        0     1071 2023-05-28 21:00:08.339474 dfbrowse-0.1.0/dfbrowse/list_utils.py
--rwxr-xr-x   0        0        0      143 2023-05-28 21:00:08.339545 dfbrowse-0.1.0/dfbrowse/main.sh
--rw-r--r--   0        0        0    24480 2023-05-28 21:00:08.339723 dfbrowse-0.1.0/dfbrowse/urwid_table_browser.py
--rw-r--r--   0        0        0     5471 2023-05-28 21:00:08.339848 dfbrowse-0.1.0/dfbrowse/urwid_utils.py
--rw-r--r--   0        0        0      504 2023-05-28 21:00:08.339985 dfbrowse-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2692 1970-01-01 00:00:00.000000 dfbrowse-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11347 2023-05-28 01:46:02.033611 dfbrowse-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2210 2023-05-29 03:29:38.630678 dfbrowse-0.1.1/README.md
+-rw-r--r--   0        0        0       96 2023-05-28 21:00:08.338178 dfbrowse-0.1.1/dfbrowse/__init__.py
+-rwxr-xr-x   0        0        0      805 2023-05-28 21:00:08.338275 dfbrowse-0.1.1/dfbrowse/browse_dataframe_csvs.py
+-rw-r--r--   0        0        0      699 2023-05-28 21:00:08.338332 dfbrowse-0.1.1/dfbrowse/browser_utils.py
+-rw-r--r--   0        0        0     2481 2023-05-29 03:25:37.203584 dfbrowse-0.1.1/dfbrowse/chunk_search_utils.py
+-rw-r--r--   0        0        0    27702 2023-05-28 21:00:08.338576 dfbrowse-0.1.1/dfbrowse/dataframe_browser.py
+-rw-r--r--   0        0        0     1806 2023-05-28 21:00:08.338695 dfbrowse-0.1.1/dfbrowse/dataframe_browser_functions.py
+-rw-r--r--   0        0        0     2364 2023-05-28 21:00:08.338847 dfbrowse-0.1.1/dfbrowse/dataframe_utils.py
+-rw-r--r--   0        0        0      879 2023-05-28 21:00:08.338930 dfbrowse-0.1.1/dfbrowse/func_core.py
+-rw-r--r--   0        0        0     1062 2023-05-28 21:00:08.339011 dfbrowse-0.1.1/dfbrowse/gui_debug.py
+-rw-r--r--   0        0        0     1794 2023-05-28 21:00:08.339115 dfbrowse-0.1.1/dfbrowse/ipython_cli.py
+-rw-r--r--   0        0        0       73 2023-05-28 21:00:08.339207 dfbrowse-0.1.1/dfbrowse/ipython_main.py
+-rw-r--r--   0        0        0     1316 2023-05-28 21:00:08.339301 dfbrowse-0.1.1/dfbrowse/ipython_utils.py
+-rw-r--r--   0        0        0     3271 2023-05-29 03:27:38.255742 dfbrowse-0.1.1/dfbrowse/keybindings.py
+-rw-r--r--   0        0        0     1071 2023-05-28 21:00:08.339474 dfbrowse-0.1.1/dfbrowse/list_utils.py
+-rwxr-xr-x   0        0        0      143 2023-05-28 21:00:08.339545 dfbrowse-0.1.1/dfbrowse/main.sh
+-rw-r--r--   0        0        0    24493 2023-05-29 03:28:15.468882 dfbrowse-0.1.1/dfbrowse/urwid_table_browser.py
+-rw-r--r--   0        0        0     5471 2023-05-28 21:00:08.339848 dfbrowse-0.1.1/dfbrowse/urwid_utils.py
+-rw-r--r--   0        0        0      504 2023-05-29 03:30:19.374850 dfbrowse-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2741 1970-01-01 00:00:00.000000 dfbrowse-0.1.1/PKG-INFO
```

### Comparing `dfbrowse-0.1.0/LICENSE` & `dfbrowse-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dfbrowse-0.1.0/README.md` & `dfbrowse-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 # dfbrowse
 
 Python library that provides spreadsheet-style browsing of a Pandas
 dataframe within a terminal/curses environment.
 
-It was borne out of my love for curses-style/modal interfaces, and a frustration with how
-difficult it is to really navigate/browse/inspect a large dataframe
-while you're operating on it within IPython.
+It was borne out of my love for curses-style/modal interfaces, and a
+frustration with how difficult it is to really navigate/browse/inspect
+a large dataframe while you're operating on it within IPython.
 
-![alt text](./.images/see-it.png)
+![Image visible on GitHub](./.images/see-it.png)
 
 ## Installation
 
-Right now, there's not a great way to install this except as a
-standalone environment using `poetry`.
-
-It may also be possible to install into an existing environment using
-a from-source `pip install`.
+`pip install dfbrowse`
 
 ## Getting started
 
 dfbrowse is generally intended to be used _inside_ IPython. Start by
 launching IPython, then import the IPython magics:
 
 ```
@@ -42,15 +38,17 @@
 %show emp
 ```
 
 ### Inside the browser
 
 Once inside the browser, you can navigate with arrow keys and the mouse.
 
-Press `?` to find out about some basic navigation commands.
+Press `?` to find out about some basic browsing commands. You can
+resize columns, hide them, reorder them, and even search the row
+contents, with a few keystrokes.
 
 There are many other commands that you can discover in `keybindings.py`.
 
 There are even more commands that can be discovered by typing `/` and
 then pressing TAB. These are pre-registered functions, such as
 `str_match` and `query`, that perform some operation on a
 dataframe. The returned dataframe will be rendered in the browser.
@@ -64,7 +62,12 @@
 
 ### quitting and reentering
 
 You can use `q` on your keyboard to go back to the shell/ipython session.
 
 Re-enter the browser via `%show <df_name>`, or `%fg` to foreground the
 most recent dataframe.
+
+## bugs
+
+There are lots. I even know about some of them. Please feel free to
+report any you find on GitHub.
```

### Comparing `dfbrowse-0.1.0/dfbrowse/browse_dataframe_csvs.py` & `dfbrowse-0.1.1/dfbrowse/browse_dataframe_csvs.py`

 * *Files identical despite different names*

### Comparing `dfbrowse-0.1.0/dfbrowse/browser_utils.py` & `dfbrowse-0.1.1/dfbrowse/browser_utils.py`

 * *Files identical despite different names*

### Comparing `dfbrowse-0.1.0/dfbrowse/chunk_search_utils.py` & `dfbrowse-0.1.1/dfbrowse/chunk_search_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 
 def search_chunk_yielder(sliceable, start_location, down=True, chunk_size=100):
     start_of_next_chunk = start_location
     while not_at_end(sliceable, start_of_next_chunk, down):
         yield get_next_chunk(sliceable, start_of_next_chunk, chunk_size, down)
         start_of_next_chunk = start_of_next_chunk + chunk_size if down else start_of_next_chunk - chunk_size
-    raise StopIteration
 
 
 def search_list_for_str(lst, search_string, starting_item, down, case_insensitive):
     """returns index into list representing string found, or None if not found"""
     search_string = search_string.lower() if case_insensitive else search_string
     search_slice_end = len(lst) if down else 0
     search_list = lst[starting_item:] if down else reversed(lst[:starting_item+1])
```

### Comparing `dfbrowse-0.1.0/dfbrowse/dataframe_browser.py` & `dfbrowse-0.1.1/dfbrowse/dataframe_browser.py`

 * *Files identical despite different names*

### Comparing `dfbrowse-0.1.0/dfbrowse/dataframe_browser_functions.py` & `dfbrowse-0.1.1/dfbrowse/dataframe_browser_functions.py`

 * *Files identical despite different names*

### Comparing `dfbrowse-0.1.0/dfbrowse/dataframe_utils.py` & `dfbrowse-0.1.1/dfbrowse/dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `dfbrowse-0.1.0/dfbrowse/func_core.py` & `dfbrowse-0.1.1/dfbrowse/func_core.py`

 * *Files identical despite different names*

### Comparing `dfbrowse-0.1.0/dfbrowse/gui_debug.py` & `dfbrowse-0.1.1/dfbrowse/gui_debug.py`

 * *Files identical despite different names*

### Comparing `dfbrowse-0.1.0/dfbrowse/ipython_cli.py` & `dfbrowse-0.1.1/dfbrowse/ipython_cli.py`

 * *Files identical despite different names*

### Comparing `dfbrowse-0.1.0/dfbrowse/ipython_utils.py` & `dfbrowse-0.1.1/dfbrowse/ipython_utils.py`

 * *Files identical despite different names*

### Comparing `dfbrowse-0.1.0/dfbrowse/keybindings.py` & `dfbrowse-0.1.1/dfbrowse/keybindings.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,19 @@
     def keybindings(self):
         return self.keybindings
     def format_error(self, e, cmd_str, **kwargs):
         return error_fmt_str.format(cmd_str)
 
 # supports multiple keybindings per command
 _commands = { # these commands are specifically for use in the browser
+    'cancel': ['esc', 'ctrl g'],
     'insert-column': ['i'],
     'hide-column': ['H'],
-    'search': ['ctrl s'],  # not working for... some reason? I think ipython might be stealing it.
-    'search-backward': ['ctrl r'],
+    'search': ['ctrl s', 'meta s'],  # ctrl s not working for... some reason?
+    'search-backward': ['ctrl r', 'meta r'],
     'sort-ascending': ['s'],
     'sort-descending': ['S'],
     'browse-right': ['right', 'l'],
     'browse-left': ['left', 'h'],
     'browse-up': ['up', 'k'],
     'browse-down': ['down', 'j'],
     'undo': ['u', 'ctrl /'],
```

### Comparing `dfbrowse-0.1.0/dfbrowse/list_utils.py` & `dfbrowse-0.1.1/dfbrowse/list_utils.py`

 * *Files identical despite different names*

### Comparing `dfbrowse-0.1.0/dfbrowse/urwid_table_browser.py` & `dfbrowse-0.1.1/dfbrowse/urwid_table_browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             name=name, cols=cols, rows=rows, current_col=current_col,
             current_row=current_row, row_percent=int(100*current_row/rows),
             current_cell=current_cell))
     def show_basic_commands(self):
         # help text
         self.set_text(
             '(hjkl) browse; (H)ide col; (+-) colwidth; (,.) move col; (u)ndo; '
-            '(ctrl-s)ea(r)ch col; (s)ort; / to see other cmds; (q)uit'
+            '(alt-s)ea(r)ch col; (s)ort; / to see other cmds; (q)uit'
         )
     def show_command_options(self):
         self.set_text('type column name to add, then press enter. Press Esc to return to browsing.')
 
 
 class Minibuffer(urwid.WidgetWrap):
     # TODO modify the minibuffer so it knows very little about the
@@ -191,22 +191,22 @@
                 print('cmd str is', cmd_str)
                 self._submit_command(cmd_str)
                 self.edit_text.set_edit_text('')
             except Exception as e:
                 print('error trying to submit command: ', self.active_command, cmd_str)
                 print(e)
                 self.browser_frame.hint(cmd_hint(self.active_command).format(cmd_str))
-        elif key == 'esc' or key == 'ctrl g':
+        elif key in keybs('cancel'):
             self.give_away_focus()
         elif key == 'ctrl c':
             # raise urwid.ExitMainLoop()
             self.give_away_focus()
-        elif key == 'ctrl s':
+        elif key in keybs('search'):
             self._search(self.edit_text.get_edit_text(), True, True)
-        elif key == 'ctrl r':
+        elif key in keybs('search-backward'):
             self._search(self.edit_text.get_edit_text(), False, True)
         else: # active search - TODO maybe replace with 'active results' being fed directly to the command callback
             self.edit_text.keypress(size, key)
             if key != 'backspace':
                 if self.active_command == 'search':
                     print('asking for forward search')
                     self._search(self.edit_text.get_edit_text(), True, False)
```

### Comparing `dfbrowse-0.1.0/dfbrowse/urwid_utils.py` & `dfbrowse-0.1.1/dfbrowse/urwid_utils.py`

 * *Files identical despite different names*

### Comparing `dfbrowse-0.1.0/PKG-INFO` & `dfbrowse-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfbrowse
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Peter Gaultney
 Author-email: petergaultney@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -16,27 +16,23 @@
 Description-Content-Type: text/markdown
 
 # dfbrowse
 
 Python library that provides spreadsheet-style browsing of a Pandas
 dataframe within a terminal/curses environment.
 
-It was borne out of my love for curses-style/modal interfaces, and a frustration with how
-difficult it is to really navigate/browse/inspect a large dataframe
-while you're operating on it within IPython.
+It was borne out of my love for curses-style/modal interfaces, and a
+frustration with how difficult it is to really navigate/browse/inspect
+a large dataframe while you're operating on it within IPython.
 
-![alt text](./.images/see-it.png)
+![Image visible on GitHub](./.images/see-it.png)
 
 ## Installation
 
-Right now, there's not a great way to install this except as a
-standalone environment using `poetry`.
-
-It may also be possible to install into an existing environment using
-a from-source `pip install`.
+`pip install dfbrowse`
 
 ## Getting started
 
 dfbrowse is generally intended to be used _inside_ IPython. Start by
 launching IPython, then import the IPython magics:
 
 ```
@@ -59,15 +55,17 @@
 %show emp
 ```
 
 ### Inside the browser
 
 Once inside the browser, you can navigate with arrow keys and the mouse.
 
-Press `?` to find out about some basic navigation commands.
+Press `?` to find out about some basic browsing commands. You can
+resize columns, hide them, reorder them, and even search the row
+contents, with a few keystrokes.
 
 There are many other commands that you can discover in `keybindings.py`.
 
 There are even more commands that can be discovered by typing `/` and
 then pressing TAB. These are pre-registered functions, such as
 `str_match` and `query`, that perform some operation on a
 dataframe. The returned dataframe will be rendered in the browser.
@@ -82,7 +80,12 @@
 ### quitting and reentering
 
 You can use `q` on your keyboard to go back to the shell/ipython session.
 
 Re-enter the browser via `%show <df_name>`, or `%fg` to foreground the
 most recent dataframe.
 
+## bugs
+
+There are lots. I even know about some of them. Please feel free to
+report any you find on GitHub.
+
```

