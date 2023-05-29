# Comparing `tmp/pygubu-designer-0.35.tar.gz` & `tmp/pygubu-designer-0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygubu-designer-0.35.tar", last modified: Thu Mar  2 04:13:53 2023, max compression
+gzip compressed data, was "pygubu-designer-0.36.tar", last modified: Mon May 29 01:11:07 2023, max compression
```

## Comparing `pygubu-designer-0.35.tar` & `pygubu-designer-0.36.tar`

### file list

```diff
@@ -1,704 +1,704 @@
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:52.995342 pygubu-designer-0.35/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       67 2022-06-27 01:27:37.000000 pygubu-designer-0.35/AUTHORS
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5128 2022-09-21 21:46:21.000000 pygubu-designer-0.35/LEEME.md
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    35064 2022-08-14 23:01:15.000000 pygubu-designer-0.35/LICENSE.md
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6509 2022-08-14 23:01:15.000000 pygubu-designer-0.35/LISEZMOI.md
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      248 2022-08-13 03:36:27.000000 pygubu-designer-0.35/MANIFEST.in
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6500 2023-03-02 04:13:52.995342 pygubu-designer-0.35/PKG-INFO
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5007 2022-09-05 01:14:44.000000 pygubu-designer-0.35/README.md
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:48.927253 pygubu-designer-0.35/development/
--rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)     6434 2022-12-09 02:08:55.000000 pygubu-designer-0.35/development/create-imgs.py
--rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)     6876 2023-01-21 04:06:15.000000 pygubu-designer-0.35/development/dev-notes.txt
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2148 2022-11-30 02:55:30.000000 pygubu-designer-0.35/development/devtool.py
--rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)     3885 2022-09-01 03:11:29.000000 pygubu-designer-0.35/development/devtool.sh
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:48.967254 pygubu-designer-0.35/development/new-designer-icons/
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:48.971253 pygubu-designer-0.35/development/new-designer-icons/__pycache__/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2277 2023-01-16 18:51:44.000000 pygubu-designer-0.35/development/new-designer-icons/__pycache__/testnewiconsapp.cpython-311.pyc
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2780 2023-01-16 05:38:47.000000 pygubu-designer-0.35/development/new-designer-icons/main.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:49.663269 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2129 2023-01-17 03:53:17.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/button.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     7010 2023-01-17 03:53:17.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/button.svg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3744 2023-01-15 21:44:17.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/canvas.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4072 2023-01-15 21:44:22.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/canvas.svg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2101 2023-01-17 02:12:40.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/combobox.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     9271 2023-01-17 02:12:35.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/combobox.svg
--rw-------   0 ministerio  (1000) ministerio  (1000)     1252 2023-01-15 22:41:22.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/default.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4185 2023-01-15 22:13:29.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/default.svg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      665 2023-01-17 03:53:17.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/entry.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3834 2023-01-17 03:53:17.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/entry.svg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1552 2023-01-17 03:53:17.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/frame.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6047 2023-01-17 03:53:17.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/frame.svg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1142 2023-01-15 21:09:25.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/label.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5074 2023-01-15 21:10:01.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/label.svg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1666 2023-01-17 03:53:17.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/labelframe.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6735 2023-01-17 03:53:17.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/labelframe.svg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2133 2023-01-17 03:34:34.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/menubutton.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     8598 2023-01-17 03:34:30.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/menubutton.svg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      962 2023-01-16 19:11:46.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/notebook-tab.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3043 2023-01-16 19:12:17.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/notebook-tab.svg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1060 2023-01-16 20:29:13.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/notebook.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3693 2023-01-16 20:29:02.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/notebook.svg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      797 2023-01-17 01:34:55.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/pannedwindow-pane.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3257 2023-01-17 01:37:17.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/pannedwindow-pane.svg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      782 2023-01-17 01:33:01.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/pannedwindow.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3238 2023-01-17 01:33:20.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/pannedwindow.svg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1077 2023-01-15 21:28:54.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/progressbar.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5356 2023-01-15 21:29:31.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/progressbar.svg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      257 2023-01-15 23:05:13.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/rect848.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1786 2023-01-17 02:48:00.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/spinbutton.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     8481 2023-01-17 02:47:53.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/spinbutton.svg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1126 2023-01-17 03:00:24.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/textview.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6381 2023-01-17 03:00:15.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/textview.svg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      867 2023-01-15 21:34:06.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/toplevel.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3229 2023-01-15 21:40:40.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/toplevel.svg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1068 2023-01-15 22:23:58.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/treeview-col.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5481 2023-01-15 22:24:06.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/treeview-col.svg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      935 2023-01-15 22:22:00.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/treeview.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4893 2023-01-15 22:21:47.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/treeview.svg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2489 2023-01-15 22:38:13.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/viewport.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     7036 2023-01-15 22:38:17.000000 pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/viewport.svg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4315 2023-01-15 20:59:40.000000 pygubu-designer-0.35/development/new-designer-icons/template.svg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     7552 2023-01-15 05:57:56.000000 pygubu-designer-0.35/development/new-designer-icons/testnewicons.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      854 2023-01-16 05:38:47.000000 pygubu-designer-0.35/development/new-designer-icons/testnewiconsapp.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:49.787272 pygubu-designer-0.35/development/pygubuLogo/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5501 2022-08-13 03:36:28.000000 pygubu-designer-0.35/development/pygubuLogo/Python-logo-notext.svg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)   174121 2022-08-13 03:36:28.000000 pygubu-designer-0.35/development/pygubuLogo/logo_pygubu .ico
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)   101863 2022-08-13 03:36:28.000000 pygubu-designer-0.35/development/pygubuLogo/logo_pygubu.icns
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)   174121 2022-08-13 03:36:28.000000 pygubu-designer-0.35/development/pygubuLogo/logo_pygubu.ico
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)   175900 2022-08-13 03:36:28.000000 pygubu-designer-0.35/development/pygubuLogo/logo_pygubu.xcf
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)   124131 2022-08-13 03:36:28.000000 pygubu-designer-0.35/development/pygubuLogo/pyGubu_newLogo.svg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       92 2022-08-14 23:01:14.000000 pygubu-designer-0.35/development/pygubuLogo/rootOfSVGs.txt
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    10232 2022-08-13 03:36:28.000000 pygubu-designer-0.35/development/pygubuLogo/tcl-tk.svg
--rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)      627 2022-07-13 00:05:26.000000 pygubu-designer-0.35/development/pygubudesigner_.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       11 2022-08-15 00:47:17.000000 pygubu-designer-0.35/development/requirements.txt
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:49.927275 pygubu-designer-0.35/examples/
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:49.927275 pygubu-designer-0.35/examples/7guis/
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:49.959275 pygubu-designer-0.35/examples/7guis/01_counter/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1256 2022-07-06 23:05:06.000000 pygubu-designer-0.35/examples/7guis/01_counter/counter.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      798 2022-07-06 23:09:13.000000 pygubu-designer-0.35/examples/7guis/01_counter/counterapp.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:49.963275 pygubu-designer-0.35/examples/7guis/02_temperature_converter/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2687 2022-07-07 00:11:21.000000 pygubu-designer-0.35/examples/7guis/02_temperature_converter/tempconv.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1648 2022-07-13 00:05:26.000000 pygubu-designer-0.35/examples/7guis/02_temperature_converter/tempconvapp.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:49.967275 pygubu-designer-0.35/examples/7guis/03_flight_Booker/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2648 2022-07-11 00:53:14.000000 pygubu-designer-0.35/examples/7guis/03_flight_Booker/flight_booker.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3212 2022-08-15 00:05:30.000000 pygubu-designer-0.35/examples/7guis/03_flight_Booker/flightbookerapp.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:49.971276 pygubu-designer-0.35/examples/7guis/04_timer/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4089 2022-07-11 03:51:30.000000 pygubu-designer-0.35/examples/7guis/04_timer/timer.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1777 2022-07-13 00:05:26.000000 pygubu-designer-0.35/examples/7guis/04_timer/timerapp.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       81 2022-08-14 23:01:14.000000 pygubu-designer-0.35/examples/7guis/README.md
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      347 2022-07-06 22:57:52.000000 pygubu-designer-0.35/examples/README.md
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      546 2021-01-10 18:38:24.000000 pygubu-designer-0.35/examples/binding.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      960 2022-07-13 00:05:26.000000 pygubu-designer-0.35/examples/button_cb.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2053 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/button_cb.ui
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:48.691248 pygubu-designer-0.35/examples/canvas/
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.031277 pygubu-designer-0.35/examples/canvas/canvas-scrollregion/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      106 2022-08-14 23:01:14.000000 pygubu-designer-0.35/examples/canvas/canvas-scrollregion/README.md
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5196 2022-08-14 21:43:22.000000 pygubu-designer-0.35/examples/canvas/canvas-scrollregion/myapp.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5211 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/canvas/canvas-scrollregion/myapp.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      842 2021-01-10 18:38:24.000000 pygubu-designer-0.35/examples/canvas_example.ui
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.035277 pygubu-designer-0.35/examples/command_properties/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1221 2022-07-13 00:05:26.000000 pygubu-designer-0.35/examples/command_properties/command_properties.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2641 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/command_properties/command_properties.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1256 2022-08-14 21:43:21.000000 pygubu-designer-0.35/examples/command_properties/command_properties2.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3116 2022-08-14 21:43:22.000000 pygubu-designer-0.35/examples/commands.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    18575 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/commands.ui
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.039277 pygubu-designer-0.35/examples/control_variables/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      584 2022-07-13 00:05:26.000000 pygubu-designer-0.35/examples/control_variables/controlvariables.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3634 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/control_variables/controlvariables.ui
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.051277 pygubu-designer-0.35/examples/custom_widget/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      436 2022-08-14 23:01:15.000000 pygubu-designer-0.35/examples/custom_widget/README.md
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.179280 pygubu-designer-0.35/examples/custom_widget/__pycache__/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      547 2022-03-17 00:59:57.000000 pygubu-designer-0.35/examples/custom_widget/__pycache__/customappwidgets.cpython-38.pyc
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      591 2022-08-18 01:16:31.000000 pygubu-designer-0.35/examples/custom_widget/__pycache__/timerappwidgets.cpython-310.pyc
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      576 2022-04-15 19:20:34.000000 pygubu-designer-0.35/examples/custom_widget/__pycache__/timerappwidgets.cpython-38.pyc
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2301 2022-08-18 01:16:31.000000 pygubu-designer-0.35/examples/custom_widget/__pycache__/timewidget.cpython-310.pyc
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2286 2022-04-15 19:20:34.000000 pygubu-designer-0.35/examples/custom_widget/__pycache__/timewidget.cpython-38.pyc
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1311 2022-03-27 00:01:32.000000 pygubu-designer-0.35/examples/custom_widget/timer_main.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      515 2022-07-13 00:05:26.000000 pygubu-designer-0.35/examples/custom_widget/timerapp.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      287 2022-08-28 07:44:47.000000 pygubu-designer-0.35/examples/custom_widget/timerappwidgets.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2363 2022-07-13 00:05:26.000000 pygubu-designer-0.35/examples/custom_widget/timewidget.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.183280 pygubu-designer-0.35/examples/customtkinter/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      174 2023-03-02 02:10:26.000000 pygubu-designer-0.35/examples/customtkinter/README.md
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.183280 pygubu-designer-0.35/examples/customtkinter/complex/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    22578 2023-03-02 03:59:03.000000 pygubu-designer-0.35/examples/customtkinter/complex/complex_demo.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2365 2023-03-02 04:07:30.000000 pygubu-designer-0.35/examples/customtkinter/complex/complexdemoapp.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.187280 pygubu-designer-0.35/examples/customtkinter/simple/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6284 2023-03-02 03:09:01.000000 pygubu-designer-0.35/examples/customtkinter/simple/simple_demo.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1269 2023-03-02 04:07:30.000000 pygubu-designer-0.35/examples/customtkinter/simple/simpledemoapp.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.191280 pygubu-designer-0.35/examples/dialogs/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       51 2022-08-14 23:01:14.000000 pygubu-designer-0.35/examples/dialogs/README.md
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.251282 pygubu-designer-0.35/examples/dialogs/demo1/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       73 2022-08-14 23:01:14.000000 pygubu-designer-0.35/examples/dialogs/demo1/README.md
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1178 2022-07-13 00:05:26.000000 pygubu-designer-0.35/examples/dialogs/demo1/demo.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5699 2022-07-05 02:56:28.000000 pygubu-designer-0.35/examples/dialogs/demo1/demo.ui
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.271282 pygubu-designer-0.35/examples/dialogs/demo2/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       95 2022-08-14 23:01:14.000000 pygubu-designer-0.35/examples/dialogs/demo2/README.md
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1319 2022-08-14 21:43:21.000000 pygubu-designer-0.35/examples/dialogs/demo2/demo.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4523 2022-07-05 02:56:28.000000 pygubu-designer-0.35/examples/dialogs/demo2/demo.ui
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.275282 pygubu-designer-0.35/examples/dialogs/demo3/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       98 2022-08-14 23:01:14.000000 pygubu-designer-0.35/examples/dialogs/demo3/README.md
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4883 2022-08-14 21:43:22.000000 pygubu-designer-0.35/examples/dialogs/demo3/demo.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     9704 2022-07-05 02:56:28.000000 pygubu-designer-0.35/examples/dialogs/demo3/demo.ui
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.279282 pygubu-designer-0.35/examples/dialogs/demo4/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      314 2023-01-18 02:21:28.000000 pygubu-designer-0.35/examples/dialogs/demo4/README.md
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.279282 pygubu-designer-0.35/examples/dialogs/demo4/__pycache__/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1835 2023-01-18 00:24:03.000000 pygubu-designer-0.35/examples/dialogs/demo4/__pycache__/settingsdialog.cpython-310.pyc
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6987 2023-01-18 00:11:57.000000 pygubu-designer-0.35/examples/dialogs/demo4/settingsdemo.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1002 2023-01-18 02:21:28.000000 pygubu-designer-0.35/examples/dialogs/demo4/settingsdemoapp.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1319 2023-01-18 02:21:28.000000 pygubu-designer-0.35/examples/dialogs/demo4/settingsdialog.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.303283 pygubu-designer-0.35/examples/editable_treeview/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5044 2023-01-26 03:41:11.000000 pygubu-designer-0.35/examples/editable_treeview/demoapp.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     7875 2023-01-26 03:41:11.000000 pygubu-designer-0.35/examples/editable_treeview/demoapp.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1471 2021-01-10 18:38:24.000000 pygubu-designer-0.35/examples/example_grid_rc.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1631 2021-01-10 18:38:24.000000 pygubu-designer-0.35/examples/example_grid_rc_2.ui
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:48.699248 pygubu-designer-0.35/examples/forms/
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.303283 pygubu-designer-0.35/examples/forms/__pycache__/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1276 2023-02-19 20:59:37.000000 pygubu-designer-0.35/examples/forms/__pycache__/formsdemo1base.cpython-310.pyc
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      723 2021-01-10 18:38:24.000000 pygubu-designer-0.35/examples/framepad.ui
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.367284 pygubu-designer-0.35/examples/helloworld/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       82 2022-08-14 23:01:14.000000 pygubu-designer-0.35/examples/helloworld/README.md
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      740 2022-07-13 00:05:26.000000 pygubu-designer-0.35/examples/helloworld/helloworld.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1178 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/helloworld/helloworld.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      755 2022-07-13 00:05:26.000000 pygubu-designer-0.35/examples/helloworld/holamundo.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1176 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/helloworld/holamundo.ui
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.439286 pygubu-designer-0.35/examples/image_property/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4015 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/image_property/green.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      710 2022-07-13 00:05:26.000000 pygubu-designer-0.35/examples/image_property/image_property.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1682 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/image_property/image_property.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3270 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/image_property/red.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3572 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/image_property/yellow.gif
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.443286 pygubu-designer-0.35/examples/integration_with_cxFreeze/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      337 2022-08-14 23:01:14.000000 pygubu-designer-0.35/examples/integration_with_cxFreeze/README.md
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.511288 pygubu-designer-0.35/examples/integration_with_cxFreeze/imgs/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       72 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_cxFreeze/imgs/MenuIcon4.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       90 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_cxFreeze/imgs/ps_circle.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      104 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_cxFreeze/imgs/ps_cross.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       86 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_cxFreeze/imgs/ps_square.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      131 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_cxFreeze/imgs/ps_triangle.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6612 2022-08-16 20:22:58.000000 pygubu-designer-0.35/examples/integration_with_cxFreeze/myapp.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    12377 2022-04-15 23:45:30.000000 pygubu-designer-0.35/examples/integration_with_cxFreeze/myapp.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2529 2022-08-28 07:44:47.000000 pygubu-designer-0.35/examples/integration_with_cxFreeze/setup.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.583289 pygubu-designer-0.35/examples/integration_with_nuitka/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      366 2022-04-15 23:40:48.000000 pygubu-designer-0.35/examples/integration_with_nuitka/README.md
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.647290 pygubu-designer-0.35/examples/integration_with_nuitka/imgs/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       72 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_nuitka/imgs/MenuIcon4.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       90 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_nuitka/imgs/ps_circle.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      104 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_nuitka/imgs/ps_cross.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       86 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_nuitka/imgs/ps_square.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      131 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_nuitka/imgs/ps_triangle.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6510 2022-08-14 21:43:22.000000 pygubu-designer-0.35/examples/integration_with_nuitka/myapp.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    12377 2022-04-15 23:45:30.000000 pygubu-designer-0.35/examples/integration_with_nuitka/myapp.ui
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.731292 pygubu-designer-0.35/examples/integration_with_py2exe/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      258 2022-04-15 22:25:27.000000 pygubu-designer-0.35/examples/integration_with_py2exe/README.md
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.795294 pygubu-designer-0.35/examples/integration_with_py2exe/imgs/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       72 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_py2exe/imgs/MenuIcon4.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       90 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_py2exe/imgs/ps_circle.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      104 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_py2exe/imgs/ps_cross.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       86 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_py2exe/imgs/ps_square.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      131 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_py2exe/imgs/ps_triangle.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6602 2022-08-14 21:43:22.000000 pygubu-designer-0.35/examples/integration_with_py2exe/myapp.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    12377 2022-04-15 23:45:30.000000 pygubu-designer-0.35/examples/integration_with_py2exe/myapp.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2731 2022-08-28 07:44:47.000000 pygubu-designer-0.35/examples/integration_with_py2exe/setup.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.839295 pygubu-designer-0.35/examples/integration_with_pyinstaller/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      291 2022-04-15 22:36:07.000000 pygubu-designer-0.35/examples/integration_with_pyinstaller/README.md
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.871295 pygubu-designer-0.35/examples/integration_with_pyinstaller/imgs/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       72 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_pyinstaller/imgs/MenuIcon4.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       90 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_pyinstaller/imgs/ps_circle.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      104 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_pyinstaller/imgs/ps_cross.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       86 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_pyinstaller/imgs/ps_square.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      131 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_pyinstaller/imgs/ps_triangle.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6602 2022-08-14 21:43:22.000000 pygubu-designer-0.35/examples/integration_with_pyinstaller/myapp.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2513 2022-08-28 07:44:47.000000 pygubu-designer-0.35/examples/integration_with_pyinstaller/myapp.spec
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    12377 2022-04-15 23:45:30.000000 pygubu-designer-0.35/examples/integration_with_pyinstaller/myapp.ui
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.875295 pygubu-designer-0.35/examples/integration_with_tkcalendar/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      582 2022-08-14 23:01:15.000000 pygubu-designer-0.35/examples/integration_with_tkcalendar/README.md
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.903296 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp1/
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.907296 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp1/__pycache__/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      602 2022-04-15 19:22:18.000000 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp1/__pycache__/tkcalendarwidgets.cpython-38.pyc
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1141 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp1/main.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      526 2022-07-13 00:05:26.000000 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp1/myapp.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       34 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp1/requirements.txt
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      317 2022-08-28 07:44:47.000000 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp1/tkcalendarwidgets.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.919296 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp2/
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:50.971298 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp2/__pycache__/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      825 2022-08-18 01:20:29.000000 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp2/__pycache__/tkcalendarwidgets.cpython-310.pyc
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      810 2022-04-15 19:24:09.000000 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp2/__pycache__/tkcalendarwidgets.cpython-38.pyc
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1750 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp2/main.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      547 2022-07-13 00:05:26.000000 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp2/myapp.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       34 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp2/requirements.txt
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      644 2022-08-28 07:44:47.000000 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp2/tkcalendarwidgets.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.035299 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp3/
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.051299 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp3/__pycache__/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1607 2022-08-18 01:19:22.000000 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp3/__pycache__/tkcalendarwidgets.cpython-310.pyc
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1596 2022-07-31 21:44:20.000000 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp3/__pycache__/tkcalendarwidgets.cpython-38.pyc
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2190 2022-07-31 00:06:09.000000 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp3/main.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      755 2022-07-31 00:06:09.000000 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp3/myapp.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       34 2022-07-31 00:06:09.000000 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp3/requirements.txt
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1975 2022-08-28 07:44:47.000000 pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp3/tkcalendarwidgets.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.079300 pygubu-designer-0.35/examples/integration_with_zipapp/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      365 2022-09-19 01:07:31.000000 pygubu-designer-0.35/examples/integration_with_zipapp/README.md
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)   355908 2022-09-19 00:05:52.000000 pygubu-designer-0.35/examples/integration_with_zipapp/demoapp.pyz
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:48.711248 pygubu-designer-0.35/examples/integration_with_zipapp/src/
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.111301 pygubu-designer-0.35/examples/integration_with_zipapp/src/demoapp/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)        0 2022-09-11 23:06:21.000000 pygubu-designer-0.35/examples/integration_with_zipapp/src/demoapp/__init__.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.191302 pygubu-designer-0.35/examples/integration_with_zipapp/src/demoapp/data/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)        0 2022-09-12 02:32:35.000000 pygubu-designer-0.35/examples/integration_with_zipapp/src/demoapp/data/__init__.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3445 2022-09-19 00:02:37.000000 pygubu-designer-0.35/examples/integration_with_zipapp/src/demoapp/data/demoapp.ui
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.211303 pygubu-designer-0.35/examples/integration_with_zipapp/src/demoapp/data/extradata/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)        0 2022-09-18 01:57:22.000000 pygubu-designer-0.35/examples/integration_with_zipapp/src/demoapp/data/extradata/__init__.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      320 2022-09-19 00:20:17.000000 pygubu-designer-0.35/examples/integration_with_zipapp/src/demoapp/data/extradata/notes.txt
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4015 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_zipapp/src/demoapp/data/green.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      556 2022-09-11 22:28:25.000000 pygubu-designer-0.35/examples/integration_with_zipapp/src/demoapp/data/info.txt
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3270 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_zipapp/src/demoapp/data/red.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3572 2022-03-19 02:20:06.000000 pygubu-designer-0.35/examples/integration_with_zipapp/src/demoapp/data/yellow.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1013 2022-09-19 00:20:17.000000 pygubu-designer-0.35/examples/integration_with_zipapp/src/demoapp/main.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.235303 pygubu-designer-0.35/examples/jpg_image_on_canvas/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      825 2022-07-13 00:05:26.000000 pygubu-designer-0.35/examples/jpg_image_on_canvas/demoapp.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1244 2021-01-10 18:38:24.000000 pygubu-designer-0.35/examples/jpg_image_on_canvas/demoapp.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       14 2021-01-10 18:38:24.000000 pygubu-designer-0.35/examples/jpg_image_on_canvas/requirements.txt
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    38211 2021-01-10 18:38:24.000000 pygubu-designer-0.35/examples/jpg_image_on_canvas/seaside400.jpg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3187 2021-01-10 18:38:24.000000 pygubu-designer-0.35/examples/menubutton.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1347 2021-01-10 18:38:24.000000 pygubu-designer-0.35/examples/menuexample.ui
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.251304 pygubu-designer-0.35/examples/notebook/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5153 2022-12-10 21:50:50.000000 pygubu-designer-0.35/examples/notebook/demo1.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1379 2022-12-10 21:53:15.000000 pygubu-designer-0.35/examples/notebook/demo1app.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1835 2021-01-10 18:38:24.000000 pygubu-designer-0.35/examples/panedwindow.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3131 2021-01-10 18:38:24.000000 pygubu-designer-0.35/examples/panes_and_notebooks.ui
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.255304 pygubu-designer-0.35/examples/pathchooserdemo/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       32 2023-01-01 21:58:08.000000 pygubu-designer-0.35/examples/pathchooserdemo/README.md
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.275304 pygubu-designer-0.35/examples/pathchooserdemo/demo1/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1897 2023-01-01 21:36:25.000000 pygubu-designer-0.35/examples/pathchooserdemo/demo1/pathchooserdemo.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3220 2023-01-01 21:36:27.000000 pygubu-designer-0.35/examples/pathchooserdemo/demo1/pathchooserdemo.ui
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.279304 pygubu-designer-0.35/examples/pathchooserdemo/demo2/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2644 2023-01-01 22:13:59.000000 pygubu-designer-0.35/examples/pathchooserdemo/demo2/pathchooserdemo.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    10131 2023-01-17 17:00:07.000000 pygubu-designer-0.35/examples/pathchooserdemo/demo2/pathchooserdemo.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1840 2021-01-10 18:38:24.000000 pygubu-designer-0.35/examples/scrollbarhelper.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    10765 2021-10-11 04:39:54.000000 pygubu-designer-0.35/examples/scrolledframe-layouts.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     9388 2021-01-10 18:38:24.000000 pygubu-designer-0.35/examples/scrolledframe.ui
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.279304 pygubu-designer-0.35/examples/scrolledtext/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4030 2022-04-16 00:57:31.000000 pygubu-designer-0.35/examples/scrolledtext/scrolledtext_demo.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      977 2022-07-13 00:05:26.000000 pygubu-designer-0.35/examples/scrolledtext/scrolledtextdemoapp.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.331305 pygubu-designer-0.35/examples/static_image/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      539 2022-07-13 00:05:26.000000 pygubu-designer-0.35/examples/static_image/demoapp.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1676 2021-01-10 18:38:24.000000 pygubu-designer-0.35/examples/static_image/demoapp.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    23336 2021-01-10 18:38:24.000000 pygubu-designer-0.35/examples/static_image/logo_253.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       16 2021-01-10 18:38:24.000000 pygubu-designer-0.35/examples/static_image/requirements.txt
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:48.715248 pygubu-designer-0.35/examples/text/
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.339305 pygubu-designer-0.35/examples/text/logwindowdemo/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3075 2023-01-04 05:41:56.000000 pygubu-designer-0.35/examples/text/logwindowdemo/demo1.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1714 2023-01-04 05:47:58.000000 pygubu-designer-0.35/examples/text/logwindowdemo/demo1app.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.355306 pygubu-designer-0.35/examples/toplevel_centered/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      154 2022-08-14 23:01:14.000000 pygubu-designer-0.35/examples/toplevel_centered/README.md
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1216 2022-07-13 00:05:26.000000 pygubu-designer-0.35/examples/toplevel_centered/centered_demo1.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1216 2022-07-13 00:05:26.000000 pygubu-designer-0.35/examples/toplevel_centered/centered_demo2.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1016 2022-07-05 02:56:28.000000 pygubu-designer-0.35/examples/toplevel_centered/demo.ui
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.375306 pygubu-designer-0.35/examples/toplevel_menu/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       64 2022-08-14 23:01:14.000000 pygubu-designer-0.35/examples/toplevel_menu/README.md
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1291 2022-07-13 00:05:26.000000 pygubu-designer-0.35/examples/toplevel_menu/menu.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2470 2022-03-19 02:20:07.000000 pygubu-designer-0.35/examples/toplevel_menu/menu.ui
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.379306 pygubu-designer-0.35/examples/treeview/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       16 2022-12-06 19:21:35.000000 pygubu-designer-0.35/examples/treeview/README.md
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.435308 pygubu-designer-0.35/examples/treeview/demo1/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       43 2022-12-06 19:22:00.000000 pygubu-designer-0.35/examples/treeview/demo1/README.md
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1496 2022-07-13 00:05:26.000000 pygubu-designer-0.35/examples/treeview/demo1/treeview.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3473 2022-03-19 02:20:07.000000 pygubu-designer-0.35/examples/treeview/demo1/treeview.ui
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.447308 pygubu-designer-0.35/examples/treeview/demo2/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       64 2022-12-06 19:22:48.000000 pygubu-designer-0.35/examples/treeview/demo2/README.md
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    23736 2022-12-06 19:15:41.000000 pygubu-designer-0.35/examples/treeview/demo2/columns_stretching.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2712 2022-12-06 19:24:11.000000 pygubu-designer-0.35/examples/treeview/demo2/columnsstretchingdemo.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.471309 pygubu-designer-0.35/examples/user_input/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       89 2022-08-14 23:01:14.000000 pygubu-designer-0.35/examples/user_input/README.md
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       16 2021-01-10 18:38:24.000000 pygubu-designer-0.35/examples/user_input/requirements.txt
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    28967 2022-09-17 20:39:05.000000 pygubu-designer-0.35/examples/user_input/userinput.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3730 2022-09-17 21:03:37.000000 pygubu-designer-0.35/examples/user_input/userinputapp.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      883 2021-01-10 18:38:24.000000 pygubu-designer-0.35/examples/variables.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4346 2021-01-10 18:38:24.000000 pygubu-designer-0.35/examples/vscrolledframe.ui
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.487309 pygubu-designer-0.35/examples/windowdeleteevent/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      887 2022-07-13 00:05:26.000000 pygubu-designer-0.35/examples/windowdeleteevent/demo1.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1122 2022-03-19 02:20:07.000000 pygubu-designer-0.35/examples/windowdeleteevent/demo1.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      847 2022-07-31 01:37:40.000000 pygubu-designer-0.35/examples/windowdeleteevent/demo2.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1271 2022-07-31 01:37:40.000000 pygubu-designer-0.35/examples/windowdeleteevent/demo2.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)   104249 2022-04-16 04:21:16.000000 pygubu-designer-0.35/pygubu-designer.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2274 2023-03-02 04:08:24.000000 pygubu-designer-0.35/pyproject.toml
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       38 2023-03-02 04:13:52.995342 pygubu-designer-0.35/setup.cfg
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       61 2022-08-13 03:36:27.000000 pygubu-designer-0.35/setup.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:48.719248 pygubu-designer-0.35/src/
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.515309 pygubu-designer-0.35/src/pygubu_designer.egg-info/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6500 2023-03-02 04:13:48.000000 pygubu-designer-0.35/src/pygubu_designer.egg-info/PKG-INFO
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    35342 2023-03-02 04:13:48.000000 pygubu-designer-0.35/src/pygubu_designer.egg-info/SOURCES.txt
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)        1 2023-03-02 04:13:48.000000 pygubu-designer-0.35/src/pygubu_designer.egg-info/dependency_links.txt
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       65 2023-03-02 04:13:48.000000 pygubu-designer-0.35/src/pygubu_designer.egg-info/entry_points.txt
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      395 2023-03-02 04:13:48.000000 pygubu-designer-0.35/src/pygubu_designer.egg-info/requires.txt
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       15 2023-03-02 04:13:48.000000 pygubu-designer-0.35/src/pygubu_designer.egg-info/top_level.txt
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.575311 pygubu-designer-0.35/src/pygubudesigner/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      126 2023-03-02 04:08:24.000000 pygubu-designer-0.35/src/pygubudesigner/__init__.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      122 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/__main__.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1049 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/actions.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6314 2022-08-14 21:43:22.000000 pygubu-designer-0.35/src/pygubudesigner/bindingseditor.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.587311 pygubu-designer-0.35/src/pygubudesigner/codegen/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       76 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/codegen/__init__.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    18622 2022-12-18 03:36:24.000000 pygubu-designer-0.35/src/pygubudesigner/codegen/codebuilder.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    13356 2023-03-02 01:17:05.000000 pygubu-designer-0.35/src/pygubudesigner/codegen/scriptgenerator.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    11033 2022-08-15 00:04:47.000000 pygubu-designer-0.35/src/pygubudesigner/containerlayouteditor.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:48.735248 pygubu-designer-0.35/src/pygubudesigner/data/
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.639312 pygubu-designer-0.35/src/pygubudesigner/data/code_templates/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1404 2022-09-21 05:18:25.000000 pygubu-designer-0.35/src/pygubudesigner/data/code_templates/app.py.mako
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      370 2022-09-21 05:18:21.000000 pygubu-designer-0.35/src/pygubudesigner/data/code_templates/base.py.mako
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      818 2022-09-21 05:19:01.000000 pygubu-designer-0.35/src/pygubudesigner/data/code_templates/customstyles.py.mako
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      933 2022-09-01 03:11:46.000000 pygubu-designer-0.35/src/pygubudesigner/data/code_templates/script.py.mako
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      658 2022-09-21 05:19:25.000000 pygubu-designer-0.35/src/pygubudesigner/data/code_templates/widget.py.mako
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:48.727248 pygubu-designer-0.35/src/pygubudesigner/data/images/
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.695313 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       70 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/arrow-left2.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       71 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/arrow-right2.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       81 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/bin-16.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       85 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/cancel-circle-16.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       61 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/close.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       73 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/download3-16.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      121 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/download3-32.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      230 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/mglass.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      377 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/property_invalid.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      875 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/pygubu.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4897 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/pygubu200.gif
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:48.723248 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:51.991320 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      107 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.Labelwidget.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      352 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.calendarframe.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.dialog.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.editabletreeview.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      128 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.pathchooserinput.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrolledframe.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      224 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkinterscrolledtext.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      231 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.toplevelmenu.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Button.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Calendar.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Canvas.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Checkbutton.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Entry.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Frame.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Label.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      105 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.LabelFrame.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Listbox.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menu.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menubutton.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Checkbutton.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Command.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Radiobutton.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Separator.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Submenu.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       75 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Message.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      327 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.OptionMenu.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.Pane.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Radiobutton.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scale.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scrollbar.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Spinbox.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Text.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Toplevel.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.default.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Button.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Checkbutton.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1120 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Combobox.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Entry.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Frame.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Label.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.LabeledScale.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      126 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Labelframe.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Menubutton.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      100 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.Tab.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      327 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.OptionMenu.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.Pane.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Progressbar.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Radiobutton.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scale.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scrollbar.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Separator.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      105 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Sizegrip.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Spinbox.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      109 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.Column.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.gif
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:52.247326 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      132 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.Labelwidget.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      139 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.calendarframe.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      155 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.combobox.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      125 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.dialog.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      130 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.editabletreeview.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       96 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.pathchooserinput.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      153 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.scrollbarhelper.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      197 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.scrolledframe.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      127 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkinterscrolledtext.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      153 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkscrollbarhelper.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      197 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkscrolledframe.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      139 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.toplevelmenu.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      138 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Button.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      139 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Calendar.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      599 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Canvas.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      118 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Checkbutton.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       96 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Entry.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      124 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Frame.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      105 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Label.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      129 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.LabelFrame.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      130 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Listbox.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      139 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menu.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      140 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menubutton.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      156 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Checkbutton.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      108 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Command.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      195 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Radiobutton.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      108 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Separator.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      139 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Submenu.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       89 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Message.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      140 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.OptionMenu.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      108 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.PanedWindow.Pane.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      108 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.PanedWindow.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      124 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Radiobutton.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      111 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Scale.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      121 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Scrollbar.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      133 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Spinbox.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      114 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Text.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      125 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Toplevel.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       96 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.default.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      138 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Button.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      118 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Checkbutton.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      155 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Combobox.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       96 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Entry.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      124 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Frame.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      105 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Label.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      111 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.LabeledScale.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      129 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Labelframe.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      140 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Menubutton.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      142 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Notebook.Tab.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      131 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Notebook.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      140 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.OptionMenu.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      108 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Panedwindow.Pane.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      108 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Panedwindow.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      125 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Progressbar.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      124 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Radiobutton.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      111 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Scale.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      121 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Scrollbar.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       89 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Separator.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      153 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Sizegrip.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      133 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Spinbox.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      156 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Treeview.Column.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      130 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Treeview.gif
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:52.267326 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/fontentry/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      592 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-bold.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      567 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-italic.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      357 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-strikethrough.gif
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      572 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-underline.gif
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:52.311327 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/
--rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)      194 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/arrow-left2.png
--rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)      184 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/arrow-right2.png
--rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)      162 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/bin-16.png
--rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)      353 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/cancel-circle-16.png
--rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)      334 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/circle-left.png
--rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)      333 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/circle-right.png
--rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)      170 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/download3-16.png
--rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)      214 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/download3-32.png
--rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)      316 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/mglass.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      603 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/property_invalid.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4777 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/pygubu.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    15896 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/pygubu200.png
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:48.727248 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:52.555332 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      488 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.calendarframe.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      613 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.combobox.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      389 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.dialog.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      418 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.editabletreeview.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      379 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.pathchooserinput.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      480 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      509 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.scrolledframe.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      426 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkinterscrolledtext.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      480 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      509 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      518 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.toplevelmenu.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      638 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Button.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      488 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Calendar.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1088 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Canvas.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      524 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Checkbutton.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      379 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Entry.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      356 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Frame.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      706 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Label.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      418 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Listbox.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      518 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menu.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      440 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menubutton.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      527 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Checkbutton.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      334 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Command.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      433 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Radiobutton.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      325 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Separator.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      518 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Submenu.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      440 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.OptionMenu.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      349 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.PanedWindow.Pane.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      349 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.PanedWindow.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      508 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Radiobutton.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      429 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Scale.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      431 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Scrollbar.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      627 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Spinbox.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      426 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Text.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      389 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Toplevel.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      291 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.default.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      638 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Button.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      524 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Checkbutton.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      613 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Combobox.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      379 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Entry.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      356 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Frame.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      706 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Label.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      429 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.LabeledScale.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      440 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Menubutton.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      435 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Notebook.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      440 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.OptionMenu.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      349 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Panedwindow.Pane.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      349 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Panedwindow.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      545 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Progressbar.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      508 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Radiobutton.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      429 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Scale.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      431 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Scrollbar.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      293 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Separator.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      627 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Spinbox.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      418 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Treeview.png
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:52.739336 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      161 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.calendarframe.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      263 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.combobox.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      169 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.dialog.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      158 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.editabletreeview.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      125 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.pathchooserinput.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      186 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.scrollbarhelper.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      339 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.scrolledframe.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      148 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkinterscrolledtext.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      186 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkscrollbarhelper.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      339 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkscrolledframe.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      164 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.toplevelmenu.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      181 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Button.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      161 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Calendar.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      689 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Canvas.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      179 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Checkbutton.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      125 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Entry.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      143 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Frame.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      205 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Label.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      158 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Listbox.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      164 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menu.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      185 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menubutton.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      202 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Checkbutton.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      127 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Command.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      323 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Radiobutton.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      127 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Separator.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      164 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Submenu.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      185 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.OptionMenu.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      118 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.PanedWindow.Pane.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      118 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.PanedWindow.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      257 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Radiobutton.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      172 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Scale.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      155 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Scrollbar.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      206 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Spinbox.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      148 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Text.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      169 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Toplevel.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      116 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.default.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      181 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Button.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      179 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Checkbutton.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      263 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Combobox.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      125 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Entry.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      143 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Frame.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      205 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Label.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      172 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.LabeledScale.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      185 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Menubutton.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      175 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Notebook.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      185 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.OptionMenu.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      118 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Panedwindow.Pane.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      118 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Panedwindow.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      138 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Progressbar.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      257 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Radiobutton.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      172 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Scale.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      155 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Scrollbar.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      107 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Separator.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      206 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Spinbox.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      158 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Treeview.png
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:52.747336 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/fontentry/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      705 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-bold.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      619 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-italic.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      611 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-strikethrough.png
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      673 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-underline.png
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:52.819338 pygubu-designer-0.35/src/pygubudesigner/data/locale/
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:48.731248 pygubu-designer-0.35/src/pygubudesigner/data/locale/de/
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:52.831338 pygubu-designer-0.35/src/pygubudesigner/data/locale/de/LC_MESSAGES/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3438 2022-11-19 20:00:41.000000 pygubu-designer-0.35/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu-designer.mo
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      425 2022-11-19 19:57:36.000000 pygubu-designer-0.35/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu.mo
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:48.731248 pygubu-designer-0.35/src/pygubudesigner/data/locale/es/
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:52.843339 pygubu-designer-0.35/src/pygubudesigner/data/locale/es/LC_MESSAGES/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    11855 2022-11-19 20:00:41.000000 pygubu-designer-0.35/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu-designer.mo
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      789 2022-11-19 19:57:36.000000 pygubu-designer-0.35/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu.mo
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    56756 2022-11-19 19:56:03.000000 pygubu-designer-0.35/src/pygubudesigner/data/locale/pygubu-designer.pot
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    17181 2022-11-19 19:56:04.000000 pygubu-designer-0.35/src/pygubudesigner/data/locale/pygubu.pot
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:48.731248 pygubu-designer-0.35/src/pygubudesigner/data/locale/tr/
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:52.851339 pygubu-designer-0.35/src/pygubudesigner/data/locale/tr/LC_MESSAGES/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5317 2022-11-19 20:00:41.000000 pygubu-designer-0.35/src/pygubudesigner/data/locale/tr/LC_MESSAGES/pygubu-designer.mo
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      393 2022-11-19 19:57:36.000000 pygubu-designer-0.35/src/pygubudesigner/data/locale/tr/LC_MESSAGES/pygubu.mo
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:48.735248 pygubu-designer-0.35/src/pygubudesigner/data/locale/zh_CN/
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:52.863339 pygubu-designer-0.35/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    53467 2022-11-19 20:00:41.000000 pygubu-designer-0.35/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu-designer.mo
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    10457 2022-11-19 19:57:36.000000 pygubu-designer-0.35/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu.mo
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:48.735248 pygubu-designer-0.35/src/pygubudesigner/data/locale/zh_Hans/
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:52.879339 pygubu-designer-0.35/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    53109 2022-11-19 20:00:41.000000 pygubu-designer-0.35/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu-designer.mo
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      421 2022-11-19 19:57:37.000000 pygubu-designer-0.35/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu.mo
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:52.899340 pygubu-designer-0.35/src/pygubudesigner/data/ui/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    12950 2022-08-13 23:41:55.000000 pygubu-designer-0.35/src/pygubudesigner/data/ui/about_dialog.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6798 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/ui/ask_save_changes_dialog.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    10318 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/data/ui/container_layout_editor_base.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    30261 2023-03-01 06:05:51.000000 pygubu-designer-0.35/src/pygubudesigner/data/ui/preferences_dialog.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    82384 2023-03-02 01:17:05.000000 pygubu-designer-0.35/src/pygubudesigner/data/ui/pygubu-ui.ui
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2525 2022-08-13 05:04:19.000000 pygubu-designer-0.35/src/pygubudesigner/dialogs.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2122 2022-09-04 22:12:41.000000 pygubu-designer-0.35/src/pygubudesigner/i18n.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     8470 2022-08-14 21:43:22.000000 pygubu-designer-0.35/src/pygubudesigner/layouteditor.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2688 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/logpanel.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    32048 2023-03-02 01:17:05.000000 pygubu-designer-0.35/src/pygubudesigner/main.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    12042 2022-08-28 07:38:35.000000 pygubu-designer-0.35/src/pygubudesigner/preferences.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:52.923340 pygubu-designer-0.35/src/pygubudesigner/preview/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       63 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/preview/__init__.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2589 2023-01-12 04:06:54.000000 pygubu-designer-0.35/src/pygubudesigner/preview/builder.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    12465 2023-01-12 04:27:05.000000 pygubu-designer-0.35/src/pygubudesigner/preview/helper.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    16592 2023-01-22 03:21:37.000000 pygubu-designer-0.35/src/pygubudesigner/preview/preview.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:52.935341 pygubu-designer-0.35/src/pygubudesigner/properties/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      346 2022-11-04 03:45:23.000000 pygubu-designer-0.35/src/pygubudesigner/properties/__init__.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1866 2022-11-04 03:45:23.000000 pygubu-designer-0.35/src/pygubudesigner/properties/manager.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    50075 2022-12-12 02:37:14.000000 pygubu-designer-0.35/src/pygubudesigner/properties/predefined.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    31209 2022-12-10 03:26:32.000000 pygubu-designer-0.35/src/pygubudesigner/properties/propertieshelp.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5461 2022-11-04 03:45:24.000000 pygubu-designer-0.35/src/pygubudesigner/propertieseditor.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1915 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/rfilemanager.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5180 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/stylehandler.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    55165 2023-03-02 01:17:05.000000 pygubu-designer-0.35/src/pygubudesigner/uitreeeditor.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:52.947341 pygubu-designer-0.35/src/pygubudesigner/util/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5417 2023-03-02 01:17:18.000000 pygubu-designer-0.35/src/pygubudesigner/util/__init__.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4297 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/util/gridcalculator.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1964 2022-08-14 23:43:51.000000 pygubu-designer-0.35/src/pygubudesigner/util/keyboard.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1175 2022-08-31 01:01:59.000000 pygubu-designer-0.35/src/pygubudesigner/util/observable.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1160 2022-12-17 01:20:04.000000 pygubu-designer-0.35/src/pygubudesigner/util/screens.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2798 2022-08-14 23:34:19.000000 pygubu-designer-0.35/src/pygubudesigner/util/selecttool.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     7402 2022-11-04 03:45:24.000000 pygubu-designer-0.35/src/pygubudesigner/widgetdescr.py
-drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-03-02 04:13:52.991342 pygubu-designer-0.35/src/pygubudesigner/widgets/
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1048 2022-09-01 03:11:46.000000 pygubu-designer-0.35/src/pygubudesigner/widgets/__init__.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3055 2023-01-11 23:55:19.000000 pygubu-designer-0.35/src/pygubudesigner/widgets/bindingeditor.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3502 2022-08-15 00:27:55.000000 pygubu-designer-0.35/src/pygubudesigner/widgets/colorentry.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5327 2023-01-11 23:55:19.000000 pygubu-designer-0.35/src/pygubudesigner/widgets/commandentry.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3621 2022-12-06 23:53:57.000000 pygubu-designer-0.35/src/pygubudesigner/widgets/componentpalette.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5088 2022-08-15 00:07:57.000000 pygubu-designer-0.35/src/pygubudesigner/widgets/containerlayouteditorbase.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1640 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/widgets/cursorentry.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2681 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/widgets/dimensionentry.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2282 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/widgets/dynamicpropeditor.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5164 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/widgets/entryvalidatecommandeditor.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     8250 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/widgets/fontentry.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    10193 2023-01-18 04:05:01.000000 pygubu-designer-0.35/src/pygubudesigner/widgets/gridselector.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2491 2022-08-14 23:59:02.000000 pygubu-designer-0.35/src/pygubudesigner/widgets/imageentry.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3046 2023-01-11 23:55:19.000000 pygubu-designer-0.35/src/pygubudesigner/widgets/namedideditor.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2102 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/widgets/pixelcoordinateentry.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    11817 2023-01-11 23:55:19.000000 pygubu-designer-0.35/src/pygubudesigner/widgets/propertyeditor.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3059 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/widgets/relativeentry.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5174 2022-11-30 02:32:48.000000 pygubu-designer-0.35/src/pygubudesigner/widgets/stickyentry.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3255 2023-01-12 05:16:08.000000 pygubu-designer-0.35/src/pygubudesigner/widgets/tkvarentry.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5568 2022-08-14 21:43:23.000000 pygubu-designer-0.35/src/pygubudesigner/widgets/toolbarframe.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2488 2022-08-14 21:43:23.000000 pygubu-designer-0.35/src/pygubudesigner/widgets/ttkstyleentry.py
--rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2536 2022-08-13 03:36:28.000000 pygubu-designer-0.35/src/pygubudesigner/widgets/whentry.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.483322 pygubu-designer-0.36/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       67 2022-06-27 01:27:37.000000 pygubu-designer-0.36/AUTHORS
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5128 2022-09-21 21:46:21.000000 pygubu-designer-0.36/LEEME.md
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    35064 2022-08-14 23:01:15.000000 pygubu-designer-0.36/LICENSE.md
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6509 2022-08-14 23:01:15.000000 pygubu-designer-0.36/LISEZMOI.md
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      248 2022-08-13 03:36:27.000000 pygubu-designer-0.36/MANIFEST.in
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6500 2023-05-29 01:11:07.483322 pygubu-designer-0.36/PKG-INFO
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5007 2022-09-05 01:14:44.000000 pygubu-designer-0.36/README.md
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.019331 pygubu-designer-0.36/development/
+-rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)     6434 2022-12-09 02:08:55.000000 pygubu-designer-0.36/development/create-imgs.py
+-rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)     6876 2023-01-21 04:06:15.000000 pygubu-designer-0.36/development/dev-notes.txt
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2148 2022-11-30 02:55:30.000000 pygubu-designer-0.36/development/devtool.py
+-rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)     3885 2022-09-01 03:11:29.000000 pygubu-designer-0.36/development/devtool.sh
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.023331 pygubu-designer-0.36/development/new-designer-icons/
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.023331 pygubu-designer-0.36/development/new-designer-icons/__pycache__/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2277 2023-01-16 18:51:44.000000 pygubu-designer-0.36/development/new-designer-icons/__pycache__/testnewiconsapp.cpython-311.pyc
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2780 2023-01-16 05:38:47.000000 pygubu-designer-0.36/development/new-designer-icons/main.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.055331 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2129 2023-01-17 03:53:17.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/button.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     7010 2023-01-17 03:53:17.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/button.svg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3744 2023-01-15 21:44:17.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/canvas.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4072 2023-01-15 21:44:22.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/canvas.svg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2101 2023-01-17 02:12:40.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/combobox.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     9271 2023-01-17 02:12:35.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/combobox.svg
+-rw-------   0 ministerio  (1000) ministerio  (1000)     1252 2023-01-15 22:41:22.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/default.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4185 2023-01-15 22:13:29.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/default.svg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      665 2023-01-17 03:53:17.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/entry.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3834 2023-01-17 03:53:17.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/entry.svg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1552 2023-01-17 03:53:17.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/frame.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6047 2023-01-17 03:53:17.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/frame.svg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1142 2023-01-15 21:09:25.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/label.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5074 2023-01-15 21:10:01.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/label.svg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1666 2023-01-17 03:53:17.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/labelframe.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6735 2023-01-17 03:53:17.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/labelframe.svg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2133 2023-01-17 03:34:34.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/menubutton.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     8598 2023-01-17 03:34:30.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/menubutton.svg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      962 2023-01-16 19:11:46.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/notebook-tab.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3043 2023-01-16 19:12:17.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/notebook-tab.svg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1060 2023-01-16 20:29:13.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/notebook.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3693 2023-01-16 20:29:02.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/notebook.svg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      797 2023-01-17 01:34:55.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/pannedwindow-pane.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3257 2023-01-17 01:37:17.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/pannedwindow-pane.svg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      782 2023-01-17 01:33:01.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/pannedwindow.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3238 2023-01-17 01:33:20.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/pannedwindow.svg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1077 2023-01-15 21:28:54.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/progressbar.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5356 2023-01-15 21:29:31.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/progressbar.svg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      257 2023-01-15 23:05:13.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/rect848.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1786 2023-01-17 02:48:00.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/spinbutton.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     8481 2023-01-17 02:47:53.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/spinbutton.svg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1126 2023-01-17 03:00:24.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/textview.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6381 2023-01-17 03:00:15.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/textview.svg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      867 2023-01-15 21:34:06.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/toplevel.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3229 2023-01-15 21:40:40.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/toplevel.svg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1068 2023-01-15 22:23:58.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/treeview-col.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5481 2023-01-15 22:24:06.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/treeview-col.svg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      935 2023-01-15 22:22:00.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/treeview.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4893 2023-01-15 22:21:47.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/treeview.svg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2489 2023-01-15 22:38:13.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/viewport.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     7036 2023-01-15 22:38:17.000000 pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/viewport.svg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4315 2023-01-15 20:59:40.000000 pygubu-designer-0.36/development/new-designer-icons/template.svg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     7552 2023-01-15 05:57:56.000000 pygubu-designer-0.36/development/new-designer-icons/testnewicons.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      854 2023-01-16 05:38:47.000000 pygubu-designer-0.36/development/new-designer-icons/testnewiconsapp.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.071330 pygubu-designer-0.36/development/pygubuLogo/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5501 2022-08-13 03:36:28.000000 pygubu-designer-0.36/development/pygubuLogo/Python-logo-notext.svg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)   174121 2022-08-13 03:36:28.000000 pygubu-designer-0.36/development/pygubuLogo/logo_pygubu .ico
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)   101863 2022-08-13 03:36:28.000000 pygubu-designer-0.36/development/pygubuLogo/logo_pygubu.icns
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)   174121 2022-08-13 03:36:28.000000 pygubu-designer-0.36/development/pygubuLogo/logo_pygubu.ico
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)   175900 2022-08-13 03:36:28.000000 pygubu-designer-0.36/development/pygubuLogo/logo_pygubu.xcf
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)   124131 2022-08-13 03:36:28.000000 pygubu-designer-0.36/development/pygubuLogo/pyGubu_newLogo.svg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       92 2022-08-14 23:01:14.000000 pygubu-designer-0.36/development/pygubuLogo/rootOfSVGs.txt
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    10232 2022-08-13 03:36:28.000000 pygubu-designer-0.36/development/pygubuLogo/tcl-tk.svg
+-rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)      627 2022-07-13 00:05:26.000000 pygubu-designer-0.36/development/pygubudesigner_.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       11 2022-08-15 00:47:17.000000 pygubu-designer-0.36/development/requirements.txt
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.091330 pygubu-designer-0.36/examples/
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.095330 pygubu-designer-0.36/examples/7guis/
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.095330 pygubu-designer-0.36/examples/7guis/01_counter/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1256 2022-07-06 23:05:06.000000 pygubu-designer-0.36/examples/7guis/01_counter/counter.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      798 2022-07-06 23:09:13.000000 pygubu-designer-0.36/examples/7guis/01_counter/counterapp.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.099330 pygubu-designer-0.36/examples/7guis/02_temperature_converter/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2687 2022-07-07 00:11:21.000000 pygubu-designer-0.36/examples/7guis/02_temperature_converter/tempconv.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1648 2022-07-13 00:05:26.000000 pygubu-designer-0.36/examples/7guis/02_temperature_converter/tempconvapp.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.099330 pygubu-designer-0.36/examples/7guis/03_flight_Booker/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2648 2022-07-11 00:53:14.000000 pygubu-designer-0.36/examples/7guis/03_flight_Booker/flight_booker.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3212 2022-08-15 00:05:30.000000 pygubu-designer-0.36/examples/7guis/03_flight_Booker/flightbookerapp.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.103330 pygubu-designer-0.36/examples/7guis/04_timer/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4089 2022-07-11 03:51:30.000000 pygubu-designer-0.36/examples/7guis/04_timer/timer.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1777 2022-07-13 00:05:26.000000 pygubu-designer-0.36/examples/7guis/04_timer/timerapp.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       81 2022-08-14 23:01:14.000000 pygubu-designer-0.36/examples/7guis/README.md
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      347 2022-07-06 22:57:52.000000 pygubu-designer-0.36/examples/README.md
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      546 2021-01-10 18:38:24.000000 pygubu-designer-0.36/examples/binding.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      960 2022-07-13 00:05:26.000000 pygubu-designer-0.36/examples/button_cb.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2053 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/button_cb.ui
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:06.951333 pygubu-designer-0.36/examples/canvas/
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.103330 pygubu-designer-0.36/examples/canvas/canvas-scrollregion/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      106 2022-08-14 23:01:14.000000 pygubu-designer-0.36/examples/canvas/canvas-scrollregion/README.md
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5196 2022-08-14 21:43:22.000000 pygubu-designer-0.36/examples/canvas/canvas-scrollregion/myapp.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5211 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/canvas/canvas-scrollregion/myapp.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      842 2021-01-10 18:38:24.000000 pygubu-designer-0.36/examples/canvas_example.ui
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.107329 pygubu-designer-0.36/examples/command_properties/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1221 2022-07-13 00:05:26.000000 pygubu-designer-0.36/examples/command_properties/command_properties.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2641 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/command_properties/command_properties.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1256 2022-08-14 21:43:21.000000 pygubu-designer-0.36/examples/command_properties/command_properties2.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3116 2022-08-14 21:43:22.000000 pygubu-designer-0.36/examples/commands.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    18575 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/commands.ui
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.107329 pygubu-designer-0.36/examples/control_variables/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      584 2022-07-13 00:05:26.000000 pygubu-designer-0.36/examples/control_variables/controlvariables.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3634 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/control_variables/controlvariables.ui
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.111329 pygubu-designer-0.36/examples/custom_widget/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      436 2022-08-14 23:01:15.000000 pygubu-designer-0.36/examples/custom_widget/README.md
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.115329 pygubu-designer-0.36/examples/custom_widget/__pycache__/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      547 2022-03-17 00:59:57.000000 pygubu-designer-0.36/examples/custom_widget/__pycache__/customappwidgets.cpython-38.pyc
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      591 2022-08-18 01:16:31.000000 pygubu-designer-0.36/examples/custom_widget/__pycache__/timerappwidgets.cpython-310.pyc
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      576 2022-04-15 19:20:34.000000 pygubu-designer-0.36/examples/custom_widget/__pycache__/timerappwidgets.cpython-38.pyc
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2301 2022-08-18 01:16:31.000000 pygubu-designer-0.36/examples/custom_widget/__pycache__/timewidget.cpython-310.pyc
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2286 2022-04-15 19:20:34.000000 pygubu-designer-0.36/examples/custom_widget/__pycache__/timewidget.cpython-38.pyc
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1311 2022-03-27 00:01:32.000000 pygubu-designer-0.36/examples/custom_widget/timer_main.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      515 2022-07-13 00:05:26.000000 pygubu-designer-0.36/examples/custom_widget/timerapp.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      287 2022-08-28 07:44:47.000000 pygubu-designer-0.36/examples/custom_widget/timerappwidgets.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2363 2022-07-13 00:05:26.000000 pygubu-designer-0.36/examples/custom_widget/timewidget.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.115329 pygubu-designer-0.36/examples/customtkinter/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      174 2023-03-02 04:18:11.000000 pygubu-designer-0.36/examples/customtkinter/README.md
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.115329 pygubu-designer-0.36/examples/customtkinter/complex/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    22578 2023-03-02 04:18:11.000000 pygubu-designer-0.36/examples/customtkinter/complex/complex_demo.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2365 2023-03-02 04:18:11.000000 pygubu-designer-0.36/examples/customtkinter/complex/complexdemoapp.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.119329 pygubu-designer-0.36/examples/customtkinter/simple/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6284 2023-03-02 04:18:11.000000 pygubu-designer-0.36/examples/customtkinter/simple/simple_demo.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1269 2023-03-02 04:18:11.000000 pygubu-designer-0.36/examples/customtkinter/simple/simpledemoapp.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.119329 pygubu-designer-0.36/examples/dialogs/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       51 2022-08-14 23:01:14.000000 pygubu-designer-0.36/examples/dialogs/README.md
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.123329 pygubu-designer-0.36/examples/dialogs/demo1/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       73 2022-08-14 23:01:14.000000 pygubu-designer-0.36/examples/dialogs/demo1/README.md
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1178 2022-07-13 00:05:26.000000 pygubu-designer-0.36/examples/dialogs/demo1/demo.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5699 2022-07-05 02:56:28.000000 pygubu-designer-0.36/examples/dialogs/demo1/demo.ui
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.123329 pygubu-designer-0.36/examples/dialogs/demo2/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       95 2022-08-14 23:01:14.000000 pygubu-designer-0.36/examples/dialogs/demo2/README.md
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1319 2022-08-14 21:43:21.000000 pygubu-designer-0.36/examples/dialogs/demo2/demo.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4523 2022-07-05 02:56:28.000000 pygubu-designer-0.36/examples/dialogs/demo2/demo.ui
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.127329 pygubu-designer-0.36/examples/dialogs/demo3/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       98 2022-08-14 23:01:14.000000 pygubu-designer-0.36/examples/dialogs/demo3/README.md
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4883 2022-08-14 21:43:22.000000 pygubu-designer-0.36/examples/dialogs/demo3/demo.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     9704 2022-07-05 02:56:28.000000 pygubu-designer-0.36/examples/dialogs/demo3/demo.ui
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.131329 pygubu-designer-0.36/examples/dialogs/demo4/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      314 2023-01-18 02:21:28.000000 pygubu-designer-0.36/examples/dialogs/demo4/README.md
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.131329 pygubu-designer-0.36/examples/dialogs/demo4/__pycache__/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1835 2023-01-18 00:24:03.000000 pygubu-designer-0.36/examples/dialogs/demo4/__pycache__/settingsdialog.cpython-310.pyc
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6987 2023-01-18 00:11:57.000000 pygubu-designer-0.36/examples/dialogs/demo4/settingsdemo.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1002 2023-01-18 02:21:28.000000 pygubu-designer-0.36/examples/dialogs/demo4/settingsdemoapp.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1319 2023-01-18 02:21:28.000000 pygubu-designer-0.36/examples/dialogs/demo4/settingsdialog.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.131329 pygubu-designer-0.36/examples/editable_treeview/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5044 2023-01-26 03:41:11.000000 pygubu-designer-0.36/examples/editable_treeview/demoapp.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     7875 2023-01-26 03:41:11.000000 pygubu-designer-0.36/examples/editable_treeview/demoapp.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1471 2021-01-10 18:38:24.000000 pygubu-designer-0.36/examples/example_grid_rc.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1631 2021-01-10 18:38:24.000000 pygubu-designer-0.36/examples/example_grid_rc_2.ui
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:06.963333 pygubu-designer-0.36/examples/forms/
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.131329 pygubu-designer-0.36/examples/forms/__pycache__/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1276 2023-05-25 03:22:01.000000 pygubu-designer-0.36/examples/forms/__pycache__/formsdemo1base.cpython-310.pyc
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      723 2021-01-10 18:38:24.000000 pygubu-designer-0.36/examples/framepad.ui
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.135329 pygubu-designer-0.36/examples/helloworld/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       82 2022-08-14 23:01:14.000000 pygubu-designer-0.36/examples/helloworld/README.md
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      740 2022-07-13 00:05:26.000000 pygubu-designer-0.36/examples/helloworld/helloworld.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1178 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/helloworld/helloworld.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      755 2022-07-13 00:05:26.000000 pygubu-designer-0.36/examples/helloworld/holamundo.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1176 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/helloworld/holamundo.ui
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.139329 pygubu-designer-0.36/examples/image_property/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4015 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/image_property/green.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      710 2022-07-13 00:05:26.000000 pygubu-designer-0.36/examples/image_property/image_property.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1682 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/image_property/image_property.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3270 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/image_property/red.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3572 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/image_property/yellow.gif
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.143329 pygubu-designer-0.36/examples/integration_with_cxFreeze/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      337 2022-08-14 23:01:14.000000 pygubu-designer-0.36/examples/integration_with_cxFreeze/README.md
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.147329 pygubu-designer-0.36/examples/integration_with_cxFreeze/imgs/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       72 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_cxFreeze/imgs/MenuIcon4.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       90 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_cxFreeze/imgs/ps_circle.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      104 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_cxFreeze/imgs/ps_cross.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       86 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_cxFreeze/imgs/ps_square.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      131 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_cxFreeze/imgs/ps_triangle.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6612 2022-08-16 20:22:58.000000 pygubu-designer-0.36/examples/integration_with_cxFreeze/myapp.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    12377 2022-04-15 23:45:30.000000 pygubu-designer-0.36/examples/integration_with_cxFreeze/myapp.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2529 2022-08-28 07:44:47.000000 pygubu-designer-0.36/examples/integration_with_cxFreeze/setup.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.147329 pygubu-designer-0.36/examples/integration_with_nuitka/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      366 2022-04-15 23:40:48.000000 pygubu-designer-0.36/examples/integration_with_nuitka/README.md
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.151329 pygubu-designer-0.36/examples/integration_with_nuitka/imgs/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       72 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_nuitka/imgs/MenuIcon4.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       90 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_nuitka/imgs/ps_circle.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      104 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_nuitka/imgs/ps_cross.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       86 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_nuitka/imgs/ps_square.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      131 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_nuitka/imgs/ps_triangle.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6510 2022-08-14 21:43:22.000000 pygubu-designer-0.36/examples/integration_with_nuitka/myapp.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    12377 2022-04-15 23:45:30.000000 pygubu-designer-0.36/examples/integration_with_nuitka/myapp.ui
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.155328 pygubu-designer-0.36/examples/integration_with_py2exe/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      258 2022-04-15 22:25:27.000000 pygubu-designer-0.36/examples/integration_with_py2exe/README.md
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.159328 pygubu-designer-0.36/examples/integration_with_py2exe/imgs/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       72 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_py2exe/imgs/MenuIcon4.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       90 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_py2exe/imgs/ps_circle.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      104 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_py2exe/imgs/ps_cross.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       86 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_py2exe/imgs/ps_square.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      131 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_py2exe/imgs/ps_triangle.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6602 2022-08-14 21:43:22.000000 pygubu-designer-0.36/examples/integration_with_py2exe/myapp.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    12377 2022-04-15 23:45:30.000000 pygubu-designer-0.36/examples/integration_with_py2exe/myapp.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2731 2022-08-28 07:44:47.000000 pygubu-designer-0.36/examples/integration_with_py2exe/setup.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.163328 pygubu-designer-0.36/examples/integration_with_pyinstaller/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      291 2022-04-15 22:36:07.000000 pygubu-designer-0.36/examples/integration_with_pyinstaller/README.md
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.167328 pygubu-designer-0.36/examples/integration_with_pyinstaller/imgs/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       72 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_pyinstaller/imgs/MenuIcon4.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       90 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_pyinstaller/imgs/ps_circle.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      104 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_pyinstaller/imgs/ps_cross.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       86 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_pyinstaller/imgs/ps_square.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      131 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_pyinstaller/imgs/ps_triangle.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6602 2022-08-14 21:43:22.000000 pygubu-designer-0.36/examples/integration_with_pyinstaller/myapp.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2513 2022-08-28 07:44:47.000000 pygubu-designer-0.36/examples/integration_with_pyinstaller/myapp.spec
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    12377 2022-04-15 23:45:30.000000 pygubu-designer-0.36/examples/integration_with_pyinstaller/myapp.ui
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.167328 pygubu-designer-0.36/examples/integration_with_tkcalendar/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      582 2022-08-14 23:01:15.000000 pygubu-designer-0.36/examples/integration_with_tkcalendar/README.md
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.171328 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp1/
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.171328 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp1/__pycache__/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      602 2022-04-15 19:22:18.000000 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp1/__pycache__/tkcalendarwidgets.cpython-38.pyc
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1141 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp1/main.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      526 2022-07-13 00:05:26.000000 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp1/myapp.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       34 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp1/requirements.txt
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      317 2022-08-28 07:44:47.000000 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp1/tkcalendarwidgets.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.171328 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp2/
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.175328 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp2/__pycache__/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      825 2022-08-18 01:20:29.000000 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp2/__pycache__/tkcalendarwidgets.cpython-310.pyc
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      810 2022-04-15 19:24:09.000000 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp2/__pycache__/tkcalendarwidgets.cpython-38.pyc
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1750 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp2/main.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      547 2022-07-13 00:05:26.000000 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp2/myapp.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       34 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp2/requirements.txt
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      644 2022-08-28 07:44:47.000000 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp2/tkcalendarwidgets.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.179328 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp3/
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.179328 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp3/__pycache__/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1607 2022-08-18 01:19:22.000000 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp3/__pycache__/tkcalendarwidgets.cpython-310.pyc
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1596 2022-07-31 21:44:20.000000 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp3/__pycache__/tkcalendarwidgets.cpython-38.pyc
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2190 2022-07-31 00:06:09.000000 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp3/main.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      755 2022-07-31 00:06:09.000000 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp3/myapp.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       34 2022-07-31 00:06:09.000000 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp3/requirements.txt
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1975 2022-08-28 07:44:47.000000 pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp3/tkcalendarwidgets.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.179328 pygubu-designer-0.36/examples/integration_with_zipapp/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      365 2022-09-19 01:07:31.000000 pygubu-designer-0.36/examples/integration_with_zipapp/README.md
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)   355908 2022-09-19 00:05:52.000000 pygubu-designer-0.36/examples/integration_with_zipapp/demoapp.pyz
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:06.975332 pygubu-designer-0.36/examples/integration_with_zipapp/src/
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.187328 pygubu-designer-0.36/examples/integration_with_zipapp/src/demoapp/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)        0 2022-09-11 23:06:21.000000 pygubu-designer-0.36/examples/integration_with_zipapp/src/demoapp/__init__.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.191328 pygubu-designer-0.36/examples/integration_with_zipapp/src/demoapp/data/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)        0 2022-09-12 02:32:35.000000 pygubu-designer-0.36/examples/integration_with_zipapp/src/demoapp/data/__init__.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3445 2022-09-19 00:02:37.000000 pygubu-designer-0.36/examples/integration_with_zipapp/src/demoapp/data/demoapp.ui
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.191328 pygubu-designer-0.36/examples/integration_with_zipapp/src/demoapp/data/extradata/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)        0 2022-09-18 01:57:22.000000 pygubu-designer-0.36/examples/integration_with_zipapp/src/demoapp/data/extradata/__init__.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      320 2022-09-19 00:20:17.000000 pygubu-designer-0.36/examples/integration_with_zipapp/src/demoapp/data/extradata/notes.txt
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4015 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_zipapp/src/demoapp/data/green.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      556 2022-09-11 22:28:25.000000 pygubu-designer-0.36/examples/integration_with_zipapp/src/demoapp/data/info.txt
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3270 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_zipapp/src/demoapp/data/red.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3572 2022-03-19 02:20:06.000000 pygubu-designer-0.36/examples/integration_with_zipapp/src/demoapp/data/yellow.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1013 2022-09-19 00:20:17.000000 pygubu-designer-0.36/examples/integration_with_zipapp/src/demoapp/main.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.195328 pygubu-designer-0.36/examples/jpg_image_on_canvas/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      825 2022-07-13 00:05:26.000000 pygubu-designer-0.36/examples/jpg_image_on_canvas/demoapp.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1244 2021-01-10 18:38:24.000000 pygubu-designer-0.36/examples/jpg_image_on_canvas/demoapp.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       14 2021-01-10 18:38:24.000000 pygubu-designer-0.36/examples/jpg_image_on_canvas/requirements.txt
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    38211 2021-01-10 18:38:24.000000 pygubu-designer-0.36/examples/jpg_image_on_canvas/seaside400.jpg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3187 2021-01-10 18:38:24.000000 pygubu-designer-0.36/examples/menubutton.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1347 2021-01-10 18:38:24.000000 pygubu-designer-0.36/examples/menuexample.ui
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.195328 pygubu-designer-0.36/examples/notebook/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5153 2022-12-10 21:50:50.000000 pygubu-designer-0.36/examples/notebook/demo1.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1379 2022-12-10 21:53:15.000000 pygubu-designer-0.36/examples/notebook/demo1app.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1835 2021-01-10 18:38:24.000000 pygubu-designer-0.36/examples/panedwindow.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3131 2021-01-10 18:38:24.000000 pygubu-designer-0.36/examples/panes_and_notebooks.ui
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.199328 pygubu-designer-0.36/examples/pathchooserdemo/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       32 2023-01-01 21:58:08.000000 pygubu-designer-0.36/examples/pathchooserdemo/README.md
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.199328 pygubu-designer-0.36/examples/pathchooserdemo/demo1/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1897 2023-01-01 21:36:25.000000 pygubu-designer-0.36/examples/pathchooserdemo/demo1/pathchooserdemo.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3220 2023-01-01 21:36:27.000000 pygubu-designer-0.36/examples/pathchooserdemo/demo1/pathchooserdemo.ui
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.199328 pygubu-designer-0.36/examples/pathchooserdemo/demo2/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2644 2023-01-01 22:13:59.000000 pygubu-designer-0.36/examples/pathchooserdemo/demo2/pathchooserdemo.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    10131 2023-01-17 17:00:07.000000 pygubu-designer-0.36/examples/pathchooserdemo/demo2/pathchooserdemo.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1840 2021-01-10 18:38:24.000000 pygubu-designer-0.36/examples/scrollbarhelper.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    10765 2021-10-11 04:39:54.000000 pygubu-designer-0.36/examples/scrolledframe-layouts.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     9388 2021-01-10 18:38:24.000000 pygubu-designer-0.36/examples/scrolledframe.ui
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.203328 pygubu-designer-0.36/examples/scrolledtext/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4030 2022-04-16 00:57:31.000000 pygubu-designer-0.36/examples/scrolledtext/scrolledtext_demo.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      977 2022-07-13 00:05:26.000000 pygubu-designer-0.36/examples/scrolledtext/scrolledtextdemoapp.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.203328 pygubu-designer-0.36/examples/static_image/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      539 2022-07-13 00:05:26.000000 pygubu-designer-0.36/examples/static_image/demoapp.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1676 2021-01-10 18:38:24.000000 pygubu-designer-0.36/examples/static_image/demoapp.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    23336 2021-01-10 18:38:24.000000 pygubu-designer-0.36/examples/static_image/logo_253.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       16 2021-01-10 18:38:24.000000 pygubu-designer-0.36/examples/static_image/requirements.txt
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:06.979332 pygubu-designer-0.36/examples/text/
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.207327 pygubu-designer-0.36/examples/text/logwindowdemo/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3075 2023-01-04 05:41:56.000000 pygubu-designer-0.36/examples/text/logwindowdemo/demo1.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1714 2023-01-04 05:47:58.000000 pygubu-designer-0.36/examples/text/logwindowdemo/demo1app.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.207327 pygubu-designer-0.36/examples/toplevel_centered/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      154 2022-08-14 23:01:14.000000 pygubu-designer-0.36/examples/toplevel_centered/README.md
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1216 2022-07-13 00:05:26.000000 pygubu-designer-0.36/examples/toplevel_centered/centered_demo1.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1216 2022-07-13 00:05:26.000000 pygubu-designer-0.36/examples/toplevel_centered/centered_demo2.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1016 2022-07-05 02:56:28.000000 pygubu-designer-0.36/examples/toplevel_centered/demo.ui
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.211327 pygubu-designer-0.36/examples/toplevel_menu/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       64 2022-08-14 23:01:14.000000 pygubu-designer-0.36/examples/toplevel_menu/README.md
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1291 2022-07-13 00:05:26.000000 pygubu-designer-0.36/examples/toplevel_menu/menu.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2470 2022-03-19 02:20:07.000000 pygubu-designer-0.36/examples/toplevel_menu/menu.ui
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.211327 pygubu-designer-0.36/examples/treeview/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       16 2022-12-06 19:21:35.000000 pygubu-designer-0.36/examples/treeview/README.md
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.215327 pygubu-designer-0.36/examples/treeview/demo1/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       43 2022-12-06 19:22:00.000000 pygubu-designer-0.36/examples/treeview/demo1/README.md
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1496 2022-07-13 00:05:26.000000 pygubu-designer-0.36/examples/treeview/demo1/treeview.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3473 2022-03-19 02:20:07.000000 pygubu-designer-0.36/examples/treeview/demo1/treeview.ui
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.219327 pygubu-designer-0.36/examples/treeview/demo2/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       64 2022-12-06 19:22:48.000000 pygubu-designer-0.36/examples/treeview/demo2/README.md
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    23736 2022-12-06 19:15:41.000000 pygubu-designer-0.36/examples/treeview/demo2/columns_stretching.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2712 2022-12-06 19:24:11.000000 pygubu-designer-0.36/examples/treeview/demo2/columnsstretchingdemo.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.223327 pygubu-designer-0.36/examples/user_input/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       89 2022-08-14 23:01:14.000000 pygubu-designer-0.36/examples/user_input/README.md
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       16 2021-01-10 18:38:24.000000 pygubu-designer-0.36/examples/user_input/requirements.txt
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    28967 2022-09-17 20:39:05.000000 pygubu-designer-0.36/examples/user_input/userinput.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3730 2022-09-17 21:03:37.000000 pygubu-designer-0.36/examples/user_input/userinputapp.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      883 2021-01-10 18:38:24.000000 pygubu-designer-0.36/examples/variables.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4346 2021-01-10 18:38:24.000000 pygubu-designer-0.36/examples/vscrolledframe.ui
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.227327 pygubu-designer-0.36/examples/windowdeleteevent/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      887 2022-07-13 00:05:26.000000 pygubu-designer-0.36/examples/windowdeleteevent/demo1.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1122 2022-03-19 02:20:07.000000 pygubu-designer-0.36/examples/windowdeleteevent/demo1.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      847 2022-07-31 01:37:40.000000 pygubu-designer-0.36/examples/windowdeleteevent/demo2.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1271 2022-07-31 01:37:40.000000 pygubu-designer-0.36/examples/windowdeleteevent/demo2.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)   104249 2022-04-16 04:21:16.000000 pygubu-designer-0.36/pygubu-designer.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2274 2023-05-29 01:07:41.000000 pygubu-designer-0.36/pyproject.toml
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       38 2023-05-29 01:11:07.483322 pygubu-designer-0.36/setup.cfg
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       61 2022-08-13 03:36:27.000000 pygubu-designer-0.36/setup.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:06.987332 pygubu-designer-0.36/src/
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.231327 pygubu-designer-0.36/src/pygubu_designer.egg-info/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6500 2023-05-29 01:11:06.000000 pygubu-designer-0.36/src/pygubu_designer.egg-info/PKG-INFO
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    35342 2023-05-29 01:11:06.000000 pygubu-designer-0.36/src/pygubu_designer.egg-info/SOURCES.txt
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)        1 2023-05-29 01:11:06.000000 pygubu-designer-0.36/src/pygubu_designer.egg-info/dependency_links.txt
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       65 2023-05-29 01:11:06.000000 pygubu-designer-0.36/src/pygubu_designer.egg-info/entry_points.txt
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      395 2023-05-29 01:11:06.000000 pygubu-designer-0.36/src/pygubu_designer.egg-info/requires.txt
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       15 2023-05-29 01:11:06.000000 pygubu-designer-0.36/src/pygubu_designer.egg-info/top_level.txt
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.239327 pygubu-designer-0.36/src/pygubudesigner/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      126 2023-05-29 01:07:25.000000 pygubu-designer-0.36/src/pygubudesigner/__init__.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      122 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/__main__.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1049 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/actions.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6314 2022-08-14 21:43:22.000000 pygubu-designer-0.36/src/pygubudesigner/bindingseditor.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.243327 pygubu-designer-0.36/src/pygubudesigner/codegen/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       76 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/codegen/__init__.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    19334 2023-03-23 00:35:13.000000 pygubu-designer-0.36/src/pygubudesigner/codegen/codebuilder.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    13625 2023-05-29 00:09:09.000000 pygubu-designer-0.36/src/pygubudesigner/codegen/scriptgenerator.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    11033 2022-08-15 00:04:47.000000 pygubu-designer-0.36/src/pygubudesigner/containerlayouteditor.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.003332 pygubu-designer-0.36/src/pygubudesigner/data/
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.247326 pygubu-designer-0.36/src/pygubudesigner/data/code_templates/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1732 2023-03-23 00:35:13.000000 pygubu-designer-0.36/src/pygubudesigner/data/code_templates/app.py.mako
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      370 2022-09-21 05:18:21.000000 pygubu-designer-0.36/src/pygubudesigner/data/code_templates/base.py.mako
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      818 2022-09-21 05:19:01.000000 pygubu-designer-0.36/src/pygubudesigner/data/code_templates/customstyles.py.mako
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      870 2023-03-23 00:35:13.000000 pygubu-designer-0.36/src/pygubudesigner/data/code_templates/script.py.mako
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      658 2022-09-21 05:19:25.000000 pygubu-designer-0.36/src/pygubudesigner/data/code_templates/widget.py.mako
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:06.991332 pygubu-designer-0.36/src/pygubudesigner/data/images/
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.255326 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       70 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/arrow-left2.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       71 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/arrow-right2.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       81 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/bin-16.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       85 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/cancel-circle-16.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       61 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/close.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       73 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/download3-16.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      121 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/download3-32.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      230 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/mglass.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      377 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/property_invalid.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      875 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/pygubu.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4897 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/pygubu200.gif
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:06.991332 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.295326 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      107 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.Labelwidget.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      352 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.calendarframe.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.dialog.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.editabletreeview.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      128 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.pathchooserinput.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrolledframe.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      224 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkinterscrolledtext.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      231 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.toplevelmenu.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Button.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Calendar.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Canvas.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Checkbutton.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Entry.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Frame.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Label.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      105 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.LabelFrame.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Listbox.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menu.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menubutton.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Checkbutton.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Command.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Radiobutton.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Separator.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Submenu.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       75 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Message.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      327 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.OptionMenu.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.Pane.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Radiobutton.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scale.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scrollbar.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Spinbox.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Text.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Toplevel.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.default.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Button.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Checkbutton.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1120 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Combobox.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Entry.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Frame.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Label.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.LabeledScale.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      126 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Labelframe.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Menubutton.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      100 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.Tab.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      327 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.OptionMenu.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.Pane.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Progressbar.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Radiobutton.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scale.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scrollbar.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Separator.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      105 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Sizegrip.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Spinbox.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      109 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.Column.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1095 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.gif
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.339325 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      132 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.Labelwidget.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      139 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.calendarframe.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      155 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.combobox.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      125 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.dialog.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      130 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.editabletreeview.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       96 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.pathchooserinput.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      153 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.scrollbarhelper.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      197 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.scrolledframe.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      127 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkinterscrolledtext.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      153 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkscrollbarhelper.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      197 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkscrolledframe.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      139 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.toplevelmenu.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      138 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Button.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      139 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Calendar.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      599 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Canvas.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      118 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Checkbutton.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       96 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Entry.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      124 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Frame.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      105 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Label.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      129 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.LabelFrame.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      130 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Listbox.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      139 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menu.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      140 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menubutton.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      156 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Checkbutton.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      108 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Command.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      195 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Radiobutton.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      108 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Separator.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      139 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Submenu.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       89 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Message.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      140 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.OptionMenu.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      108 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.PanedWindow.Pane.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      108 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.PanedWindow.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      124 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Radiobutton.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      111 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Scale.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      121 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Scrollbar.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      133 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Spinbox.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      114 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Text.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      125 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Toplevel.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       96 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.default.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      138 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Button.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      118 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Checkbutton.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      155 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Combobox.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       96 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Entry.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      124 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Frame.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      105 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Label.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      111 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.LabeledScale.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      129 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Labelframe.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      140 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Menubutton.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      142 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Notebook.Tab.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      131 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Notebook.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      140 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.OptionMenu.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      108 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Panedwindow.Pane.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      108 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Panedwindow.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      125 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Progressbar.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      124 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Radiobutton.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      111 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Scale.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      121 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Scrollbar.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       89 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Separator.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      153 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Sizegrip.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      133 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Spinbox.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      156 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Treeview.Column.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      130 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Treeview.gif
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.343325 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/fontentry/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      592 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-bold.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      567 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-italic.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      357 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-strikethrough.gif
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      572 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-underline.gif
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.351324 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/
+-rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)      194 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/arrow-left2.png
+-rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)      184 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/arrow-right2.png
+-rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)      162 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/bin-16.png
+-rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)      353 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/cancel-circle-16.png
+-rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)      334 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/circle-left.png
+-rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)      333 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/circle-right.png
+-rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)      170 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/download3-16.png
+-rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)      214 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/download3-32.png
+-rwxrwxr-x   0 ministerio  (1000) ministerio  (1000)      316 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/mglass.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      603 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/property_invalid.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4777 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/pygubu.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    15896 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/pygubu200.png
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:06.995332 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.391324 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      488 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.calendarframe.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      613 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.combobox.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      389 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.dialog.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      418 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.editabletreeview.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      379 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.pathchooserinput.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      480 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      509 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.scrolledframe.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      426 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkinterscrolledtext.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      480 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      509 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      518 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.toplevelmenu.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      638 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Button.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      488 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Calendar.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1088 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Canvas.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      524 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Checkbutton.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      379 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Entry.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      356 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Frame.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      706 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Label.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      418 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Listbox.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      518 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menu.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      440 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menubutton.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      527 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Checkbutton.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      334 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Command.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      433 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Radiobutton.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      325 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Separator.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      518 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Submenu.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      440 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.OptionMenu.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      349 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.PanedWindow.Pane.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      349 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.PanedWindow.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      508 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Radiobutton.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      429 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Scale.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      431 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Scrollbar.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      627 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Spinbox.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      426 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Text.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      389 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Toplevel.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      291 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.default.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      638 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Button.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      524 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Checkbutton.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      613 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Combobox.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      379 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Entry.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      356 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Frame.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      706 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Label.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      429 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.LabeledScale.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      440 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Menubutton.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      435 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Notebook.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      440 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.OptionMenu.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      349 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Panedwindow.Pane.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      349 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Panedwindow.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      545 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Progressbar.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      508 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Radiobutton.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      429 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Scale.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      431 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Scrollbar.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      293 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Separator.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      627 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Spinbox.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      418 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Treeview.png
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.431323 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      161 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.calendarframe.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      263 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.combobox.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      169 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.dialog.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      158 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.editabletreeview.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      125 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.pathchooserinput.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      186 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.scrollbarhelper.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      339 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.scrolledframe.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      148 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkinterscrolledtext.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      186 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkscrollbarhelper.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      339 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkscrolledframe.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      164 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.toplevelmenu.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      181 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Button.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      161 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Calendar.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      689 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Canvas.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      179 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Checkbutton.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      125 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Entry.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      143 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Frame.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      205 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Label.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      158 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Listbox.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      164 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menu.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      185 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menubutton.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      202 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Checkbutton.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      127 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Command.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      323 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Radiobutton.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      127 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Separator.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      164 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Submenu.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      185 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.OptionMenu.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      118 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.PanedWindow.Pane.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      118 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.PanedWindow.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      257 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Radiobutton.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      172 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Scale.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      155 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Scrollbar.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      206 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Spinbox.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      148 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Text.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      169 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Toplevel.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      116 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.default.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      181 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Button.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      179 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Checkbutton.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      263 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Combobox.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      125 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Entry.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      143 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Frame.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      205 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Label.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      172 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.LabeledScale.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      185 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Menubutton.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      175 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Notebook.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      185 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.OptionMenu.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      118 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Panedwindow.Pane.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      118 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Panedwindow.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      138 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Progressbar.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      257 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Radiobutton.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      172 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Scale.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      155 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Scrollbar.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      107 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Separator.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      206 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Spinbox.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      158 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Treeview.png
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.435323 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/fontentry/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      705 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-bold.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      619 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-italic.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      611 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-strikethrough.png
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      673 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-underline.png
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.435323 pygubu-designer-0.36/src/pygubudesigner/data/locale/
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:06.995332 pygubu-designer-0.36/src/pygubudesigner/data/locale/de/
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.439323 pygubu-designer-0.36/src/pygubudesigner/data/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3438 2022-11-19 20:00:41.000000 pygubu-designer-0.36/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu-designer.mo
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      425 2022-11-19 19:57:36.000000 pygubu-designer-0.36/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu.mo
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:06.995332 pygubu-designer-0.36/src/pygubudesigner/data/locale/es/
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.443323 pygubu-designer-0.36/src/pygubudesigner/data/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    11855 2022-11-19 20:00:41.000000 pygubu-designer-0.36/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu-designer.mo
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      789 2022-11-19 19:57:36.000000 pygubu-designer-0.36/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu.mo
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    56756 2022-11-19 19:56:03.000000 pygubu-designer-0.36/src/pygubudesigner/data/locale/pygubu-designer.pot
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    17181 2022-11-19 19:56:04.000000 pygubu-designer-0.36/src/pygubudesigner/data/locale/pygubu.pot
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:06.999332 pygubu-designer-0.36/src/pygubudesigner/data/locale/tr/
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.443323 pygubu-designer-0.36/src/pygubudesigner/data/locale/tr/LC_MESSAGES/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5317 2022-11-19 20:00:41.000000 pygubu-designer-0.36/src/pygubudesigner/data/locale/tr/LC_MESSAGES/pygubu-designer.mo
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      393 2022-11-19 19:57:36.000000 pygubu-designer-0.36/src/pygubudesigner/data/locale/tr/LC_MESSAGES/pygubu.mo
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:06.999332 pygubu-designer-0.36/src/pygubudesigner/data/locale/zh_CN/
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.447322 pygubu-designer-0.36/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    53467 2022-11-19 20:00:41.000000 pygubu-designer-0.36/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu-designer.mo
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    10457 2022-11-19 19:57:36.000000 pygubu-designer-0.36/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu.mo
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:06.999332 pygubu-designer-0.36/src/pygubudesigner/data/locale/zh_Hans/
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.451322 pygubu-designer-0.36/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    53109 2022-11-19 20:00:41.000000 pygubu-designer-0.36/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu-designer.mo
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      421 2022-11-19 19:57:37.000000 pygubu-designer-0.36/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu.mo
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.455322 pygubu-designer-0.36/src/pygubudesigner/data/ui/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    12950 2022-08-13 23:41:55.000000 pygubu-designer-0.36/src/pygubudesigner/data/ui/about_dialog.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     6798 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/ui/ask_save_changes_dialog.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    10318 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/data/ui/container_layout_editor_base.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    31137 2023-05-29 00:25:02.000000 pygubu-designer-0.36/src/pygubudesigner/data/ui/preferences_dialog.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    82384 2023-05-29 00:09:09.000000 pygubu-designer-0.36/src/pygubudesigner/data/ui/pygubu-ui.ui
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2525 2022-08-13 05:04:19.000000 pygubu-designer-0.36/src/pygubudesigner/dialogs.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2122 2022-09-04 22:12:41.000000 pygubu-designer-0.36/src/pygubudesigner/i18n.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     8470 2022-08-14 21:43:22.000000 pygubu-designer-0.36/src/pygubudesigner/layouteditor.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2688 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/logpanel.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    32262 2023-05-29 00:26:37.000000 pygubu-designer-0.36/src/pygubudesigner/main.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    12137 2023-05-29 00:27:35.000000 pygubu-designer-0.36/src/pygubudesigner/preferences.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.455322 pygubu-designer-0.36/src/pygubudesigner/preview/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)       63 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/preview/__init__.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2589 2023-05-29 00:09:09.000000 pygubu-designer-0.36/src/pygubudesigner/preview/builder.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    12465 2023-01-12 04:27:05.000000 pygubu-designer-0.36/src/pygubudesigner/preview/helper.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    16592 2023-01-22 03:21:37.000000 pygubu-designer-0.36/src/pygubudesigner/preview/preview.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.459322 pygubu-designer-0.36/src/pygubudesigner/properties/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)      346 2023-05-29 00:09:09.000000 pygubu-designer-0.36/src/pygubudesigner/properties/__init__.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1866 2022-11-04 03:45:23.000000 pygubu-designer-0.36/src/pygubudesigner/properties/manager.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    50075 2023-05-29 00:09:10.000000 pygubu-designer-0.36/src/pygubudesigner/properties/predefined.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    31209 2022-12-10 03:26:32.000000 pygubu-designer-0.36/src/pygubudesigner/properties/propertieshelp.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5461 2023-05-29 00:09:10.000000 pygubu-designer-0.36/src/pygubudesigner/propertieseditor.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1915 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/rfilemanager.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5180 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/stylehandler.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    55165 2023-05-29 00:09:10.000000 pygubu-designer-0.36/src/pygubudesigner/uitreeeditor.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.467322 pygubu-designer-0.36/src/pygubudesigner/util/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5417 2023-03-02 04:18:11.000000 pygubu-designer-0.36/src/pygubudesigner/util/__init__.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     4297 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/util/gridcalculator.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1964 2022-08-14 23:43:51.000000 pygubu-designer-0.36/src/pygubudesigner/util/keyboard.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1175 2022-08-31 01:01:59.000000 pygubu-designer-0.36/src/pygubudesigner/util/observable.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1160 2022-12-17 01:20:04.000000 pygubu-designer-0.36/src/pygubudesigner/util/screens.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2798 2022-08-14 23:34:19.000000 pygubu-designer-0.36/src/pygubudesigner/util/selecttool.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     7402 2022-11-04 03:45:24.000000 pygubu-designer-0.36/src/pygubudesigner/widgetdescr.py
+drwxrwxr-x   0 ministerio  (1000) ministerio  (1000)        0 2023-05-29 01:11:07.483322 pygubu-designer-0.36/src/pygubudesigner/widgets/
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1048 2022-09-01 03:11:46.000000 pygubu-designer-0.36/src/pygubudesigner/widgets/__init__.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3063 2023-03-18 00:51:28.000000 pygubu-designer-0.36/src/pygubudesigner/widgets/bindingeditor.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3502 2022-08-15 00:27:55.000000 pygubu-designer-0.36/src/pygubudesigner/widgets/colorentry.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5327 2023-01-11 23:55:19.000000 pygubu-designer-0.36/src/pygubudesigner/widgets/commandentry.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3621 2022-12-06 23:53:57.000000 pygubu-designer-0.36/src/pygubudesigner/widgets/componentpalette.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5088 2022-08-15 00:07:57.000000 pygubu-designer-0.36/src/pygubudesigner/widgets/containerlayouteditorbase.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     1640 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/widgets/cursorentry.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2681 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/widgets/dimensionentry.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2282 2023-04-23 01:58:21.000000 pygubu-designer-0.36/src/pygubudesigner/widgets/dynamicpropeditor.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5164 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/widgets/entryvalidatecommandeditor.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     8250 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/widgets/fontentry.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    10193 2023-01-18 04:05:01.000000 pygubu-designer-0.36/src/pygubudesigner/widgets/gridselector.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2491 2022-08-14 23:59:02.000000 pygubu-designer-0.36/src/pygubudesigner/widgets/imageentry.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3046 2023-01-11 23:55:19.000000 pygubu-designer-0.36/src/pygubudesigner/widgets/namedideditor.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2102 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/widgets/pixelcoordinateentry.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)    11817 2023-05-29 00:09:10.000000 pygubu-designer-0.36/src/pygubudesigner/widgets/propertyeditor.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3059 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/widgets/relativeentry.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5174 2022-11-30 02:32:48.000000 pygubu-designer-0.36/src/pygubudesigner/widgets/stickyentry.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     3255 2023-01-12 05:16:08.000000 pygubu-designer-0.36/src/pygubudesigner/widgets/tkvarentry.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     5568 2022-08-14 21:43:23.000000 pygubu-designer-0.36/src/pygubudesigner/widgets/toolbarframe.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2488 2022-08-14 21:43:23.000000 pygubu-designer-0.36/src/pygubudesigner/widgets/ttkstyleentry.py
+-rw-rw-r--   0 ministerio  (1000) ministerio  (1000)     2536 2022-08-13 03:36:28.000000 pygubu-designer-0.36/src/pygubudesigner/widgets/whentry.py
```

### Comparing `pygubu-designer-0.35/LEEME.md` & `pygubu-designer-0.36/LEEME.md`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/LICENSE.md` & `pygubu-designer-0.36/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/LISEZMOI.md` & `pygubu-designer-0.36/LISEZMOI.md`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/PKG-INFO` & `pygubu-designer-0.36/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygubu-designer
-Version: 0.35
+Version: 0.36
 Summary: A simple GUI designer for the python tkinter module
 Author-email: Alejandro Autalan <alejandroautalan@gmail.com>
 License: GPL-3
 Project-URL: Documentation, https://github.com/alejandroautalan/pygubu-designer#readme
 Project-URL: Issues, https://github.com/alejandroautalan/pygubu-designer/issues
 Project-URL: Source, https://github.com/alejandroautalan/pygubu-designer
 Keywords: gui,tkinter,designer
```

### Comparing `pygubu-designer-0.35/README.md` & `pygubu-designer-0.36/README.md`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/create-imgs.py` & `pygubu-designer-0.36/development/create-imgs.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/dev-notes.txt` & `pygubu-designer-0.36/development/dev-notes.txt`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/devtool.py` & `pygubu-designer-0.36/development/devtool.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/devtool.sh` & `pygubu-designer-0.36/development/devtool.sh`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/__pycache__/testnewiconsapp.cpython-311.pyc` & `pygubu-designer-0.36/development/new-designer-icons/__pycache__/testnewiconsapp.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/main.py` & `pygubu-designer-0.36/development/new-designer-icons/main.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/button.png` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/button.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/button.svg` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/button.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/canvas.png` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/canvas.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/canvas.svg` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/canvas.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/combobox.png` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/combobox.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/combobox.svg` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/combobox.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/default.png` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/default.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/default.svg` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/default.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/entry.png` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/entry.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/entry.svg` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/entry.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/frame.png` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/frame.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/frame.svg` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/frame.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/label.png` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/label.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/label.svg` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/label.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/labelframe.png` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/labelframe.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/labelframe.svg` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/labelframe.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/menubutton.png` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/menubutton.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/menubutton.svg` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/menubutton.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/notebook-tab.png` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/notebook-tab.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/notebook-tab.svg` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/notebook-tab.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/notebook.png` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/notebook.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/notebook.svg` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/notebook.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/pannedwindow-pane.png` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/pannedwindow-pane.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/pannedwindow-pane.svg` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/pannedwindow-pane.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/pannedwindow.png` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/pannedwindow.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/pannedwindow.svg` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/pannedwindow.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/progressbar.png` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/progressbar.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/progressbar.svg` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/progressbar.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/spinbutton.png` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/spinbutton.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/spinbutton.svg` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/spinbutton.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/textview.png` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/textview.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/textview.svg` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/textview.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/toplevel.png` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/toplevel.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/toplevel.svg` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/toplevel.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/treeview-col.png` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/treeview-col.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/treeview-col.svg` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/treeview-col.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/treeview.png` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/treeview.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/treeview.svg` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/treeview.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/viewport.png` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/viewport.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/pygubu-icons/viewport.svg` & `pygubu-designer-0.36/development/new-designer-icons/pygubu-icons/viewport.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/template.svg` & `pygubu-designer-0.36/development/new-designer-icons/template.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/testnewicons.ui` & `pygubu-designer-0.36/development/new-designer-icons/testnewicons.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/new-designer-icons/testnewiconsapp.py` & `pygubu-designer-0.36/development/new-designer-icons/testnewiconsapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/pygubuLogo/Python-logo-notext.svg` & `pygubu-designer-0.36/development/pygubuLogo/Python-logo-notext.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/pygubuLogo/logo_pygubu .ico` & `pygubu-designer-0.36/development/pygubuLogo/logo_pygubu .ico`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/pygubuLogo/logo_pygubu.icns` & `pygubu-designer-0.36/development/pygubuLogo/logo_pygubu.icns`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/pygubuLogo/logo_pygubu.ico` & `pygubu-designer-0.36/development/pygubuLogo/logo_pygubu.ico`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/pygubuLogo/logo_pygubu.xcf` & `pygubu-designer-0.36/development/pygubuLogo/logo_pygubu.xcf`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/pygubuLogo/pyGubu_newLogo.svg` & `pygubu-designer-0.36/development/pygubuLogo/pyGubu_newLogo.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/pygubuLogo/tcl-tk.svg` & `pygubu-designer-0.36/development/pygubuLogo/tcl-tk.svg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/development/pygubudesigner_.py` & `pygubu-designer-0.36/development/pygubudesigner_.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/7guis/01_counter/counter.ui` & `pygubu-designer-0.36/examples/7guis/01_counter/counter.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/7guis/01_counter/counterapp.py` & `pygubu-designer-0.36/examples/7guis/01_counter/counterapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/7guis/02_temperature_converter/tempconv.ui` & `pygubu-designer-0.36/examples/7guis/02_temperature_converter/tempconv.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/7guis/02_temperature_converter/tempconvapp.py` & `pygubu-designer-0.36/examples/7guis/02_temperature_converter/tempconvapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/7guis/03_flight_Booker/flight_booker.ui` & `pygubu-designer-0.36/examples/7guis/03_flight_Booker/flight_booker.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/7guis/03_flight_Booker/flightbookerapp.py` & `pygubu-designer-0.36/examples/7guis/03_flight_Booker/flightbookerapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/7guis/04_timer/timer.ui` & `pygubu-designer-0.36/examples/7guis/04_timer/timer.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/7guis/04_timer/timerapp.py` & `pygubu-designer-0.36/examples/7guis/04_timer/timerapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/binding.ui` & `pygubu-designer-0.36/examples/binding.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/button_cb.py` & `pygubu-designer-0.36/examples/button_cb.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/button_cb.ui` & `pygubu-designer-0.36/examples/button_cb.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/canvas/canvas-scrollregion/myapp.py` & `pygubu-designer-0.36/examples/canvas/canvas-scrollregion/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/canvas/canvas-scrollregion/myapp.ui` & `pygubu-designer-0.36/examples/canvas/canvas-scrollregion/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/canvas_example.ui` & `pygubu-designer-0.36/examples/canvas_example.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/command_properties/command_properties.py` & `pygubu-designer-0.36/examples/command_properties/command_properties.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/command_properties/command_properties.ui` & `pygubu-designer-0.36/examples/command_properties/command_properties.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/command_properties/command_properties2.py` & `pygubu-designer-0.36/examples/command_properties/command_properties2.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/commands.py` & `pygubu-designer-0.36/examples/commands.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/commands.ui` & `pygubu-designer-0.36/examples/commands.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/control_variables/controlvariables.py` & `pygubu-designer-0.36/examples/control_variables/controlvariables.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/control_variables/controlvariables.ui` & `pygubu-designer-0.36/examples/control_variables/controlvariables.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/custom_widget/__pycache__/customappwidgets.cpython-38.pyc` & `pygubu-designer-0.36/examples/custom_widget/__pycache__/customappwidgets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/custom_widget/__pycache__/timerappwidgets.cpython-310.pyc` & `pygubu-designer-0.36/examples/custom_widget/__pycache__/timerappwidgets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/custom_widget/__pycache__/timerappwidgets.cpython-38.pyc` & `pygubu-designer-0.36/examples/custom_widget/__pycache__/timerappwidgets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/custom_widget/__pycache__/timewidget.cpython-310.pyc` & `pygubu-designer-0.36/examples/custom_widget/__pycache__/timewidget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/custom_widget/__pycache__/timewidget.cpython-38.pyc` & `pygubu-designer-0.36/examples/custom_widget/__pycache__/timewidget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/custom_widget/timer_main.ui` & `pygubu-designer-0.36/examples/custom_widget/timer_main.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/custom_widget/timerapp.py` & `pygubu-designer-0.36/examples/custom_widget/timerapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/custom_widget/timewidget.py` & `pygubu-designer-0.36/examples/custom_widget/timewidget.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/customtkinter/complex/complex_demo.ui` & `pygubu-designer-0.36/examples/customtkinter/complex/complex_demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/customtkinter/complex/complexdemoapp.py` & `pygubu-designer-0.36/examples/customtkinter/complex/complexdemoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/customtkinter/simple/simple_demo.ui` & `pygubu-designer-0.36/examples/customtkinter/simple/simple_demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/customtkinter/simple/simpledemoapp.py` & `pygubu-designer-0.36/examples/customtkinter/simple/simpledemoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/dialogs/demo1/demo.py` & `pygubu-designer-0.36/examples/dialogs/demo1/demo.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/dialogs/demo1/demo.ui` & `pygubu-designer-0.36/examples/dialogs/demo1/demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/dialogs/demo2/demo.py` & `pygubu-designer-0.36/examples/dialogs/demo2/demo.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/dialogs/demo2/demo.ui` & `pygubu-designer-0.36/examples/dialogs/demo2/demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/dialogs/demo3/demo.py` & `pygubu-designer-0.36/examples/dialogs/demo3/demo.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/dialogs/demo3/demo.ui` & `pygubu-designer-0.36/examples/dialogs/demo3/demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/dialogs/demo4/__pycache__/settingsdialog.cpython-310.pyc` & `pygubu-designer-0.36/examples/dialogs/demo4/__pycache__/settingsdialog.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/dialogs/demo4/settingsdemo.ui` & `pygubu-designer-0.36/examples/dialogs/demo4/settingsdemo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/dialogs/demo4/settingsdemoapp.py` & `pygubu-designer-0.36/examples/dialogs/demo4/settingsdemoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/dialogs/demo4/settingsdialog.py` & `pygubu-designer-0.36/examples/dialogs/demo4/settingsdialog.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/editable_treeview/demoapp.py` & `pygubu-designer-0.36/examples/editable_treeview/demoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/editable_treeview/demoapp.ui` & `pygubu-designer-0.36/examples/editable_treeview/demoapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/example_grid_rc.ui` & `pygubu-designer-0.36/examples/example_grid_rc.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/example_grid_rc_2.ui` & `pygubu-designer-0.36/examples/example_grid_rc_2.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/forms/__pycache__/formsdemo1base.cpython-310.pyc` & `pygubu-designer-0.36/examples/forms/__pycache__/formsdemo1base.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Feb 19 20:48:00 2023 UTC, .py size: 679 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 008b f263 a702 0000  o..........c....
+00000000: 6f0d 0d0a 0000 0000 a1b5 6a64 a802 0000  o.........jd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6500  d.l.Z.d.d.l.Z.e.
 00000040: a002 6503 a101 6a04 5a05 6505 6402 1b00  ..e...j.Z.e.d...
 00000050: 5a06 4700 6403 6404 8400 6404 8302 5a07  Z.G.d.d...d...Z.
 00000060: 6508 6405 6b02 7226 6507 8300 5a09 6509  e.d.k.r&e...Z.e.
 00000070: a00a a100 0100 6401 5300 6401 5300 2906  ......d.S.d.S.).
@@ -32,49 +32,49 @@
 000001f0: 00a9 0072 1000 0000 fa61 2f68 6f6d 652f  ...r.....a/home/
 00000200: 6d69 6e69 7374 6572 696f 2f50 7269 7661  ministerio/Priva
 00000210: 646f 2f70 726f 6a65 6374 732f 7079 6775  do/projects/pygu
 00000220: 6275 2d70 726f 6a65 6374 2f70 7967 7562  bu-project/pygub
 00000230: 752d 6465 7369 676e 6572 2f65 7861 6d70  u-designer/examp
 00000240: 6c65 732f 666f 726d 732f 666f 726d 7364  les/forms/formsd
 00000250: 656d 6f31 6261 7365 2e70 79da 085f 5f69  emo1base.py..__i
-00000260: 6e69 745f 5f09 0000 0073 0a00 0000 0e01  nit__....s......
+00000260: 6e69 745f 5f0a 0000 0073 0a00 0000 0e01  nit__....s......
 00000270: 0a01 0a01 0e02 0e01 7a17 466f 726d 7344  ........z.FormsD
 00000280: 656d 6f31 4261 7365 2e5f 5f69 6e69 745f  emo1Base.__init_
 00000290: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
 000002a0: 0000 0200 0000 4300 0000 730e 0000 007c  ......C...s....|
 000002b0: 006a 00a0 01a1 0001 0064 0053 00a9 014e  .j.......d.S...N
 000002c0: 2902 720c 0000 00da 086d 6169 6e6c 6f6f  ).r......mainloo
 000002d0: 70a9 0172 0e00 0000 7210 0000 0072 1000  p..r....r....r..
-000002e0: 0000 7211 0000 00da 0372 756e 1100 0000  ..r......run....
+000002e0: 0000 7211 0000 00da 0372 756e 1200 0000  ..r......run....
 000002f0: 7302 0000 000e 017a 1246 6f72 6d73 4465  s......z.FormsDe
 00000300: 6d6f 3142 6173 652e 7275 6e63 0100 0000  mo1Base.runc....
 00000310: 0000 0000 0000 0000 0100 0000 0100 0000  ................
 00000320: 4300 0000 f304 0000 0064 0053 0072 1300  C........d.S.r..
 00000330: 0000 7210 0000 0072 1500 0000 7210 0000  ..r....r....r...
 00000340: 0072 1000 0000 7211 0000 00da 106f 6e5f  .r....r......on_
-00000350: 6368 6563 6b5f 6368 616e 6765 6414 0000  check_changed...
+00000350: 6368 6563 6b5f 6368 616e 6765 6415 0000  check_changed...
 00000360: 00f3 0200 0000 0401 7a1f 466f 726d 7344  ........z.FormsD
 00000370: 656d 6f31 4261 7365 2e6f 6e5f 6368 6563  emo1Base.on_chec
 00000380: 6b5f 6368 616e 6765 6463 0100 0000 0000  k_changedc......
 00000390: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
 000003a0: 0000 7217 0000 0072 1300 0000 7210 0000  ..r....r....r...
 000003b0: 0072 1500 0000 7210 0000 0072 1000 0000  .r....r....r....
 000003c0: 7211 0000 00da 116f 6e5f 7375 626d 6974  r......on_submit
-000003d0: 5f63 6c69 636b 6564 1700 0000 7219 0000  _clicked....r...
+000003d0: 5f63 6c69 636b 6564 1800 0000 7219 0000  _clicked....r...
 000003e0: 007a 2046 6f72 6d73 4465 6d6f 3142 6173  .z FormsDemo1Bas
 000003f0: 652e 6f6e 5f73 7562 6d69 745f 636c 6963  e.on_submit_clic
 00000400: 6b65 6472 1300 0000 2907 da08 5f5f 6e61  kedr....)...__na
 00000410: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
 00000420: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7212  ..__qualname__r.
 00000430: 0000 0072 1600 0000 7218 0000 0072 1a00  ...r....r....r..
 00000440: 0000 7210 0000 0072 1000 0000 7210 0000  ..r....r....r...
-00000450: 0072 1100 0000 7202 0000 0008 0000 0073  .r....r........s
+00000450: 0072 1100 0000 7202 0000 0009 0000 0073  .r....r........s
 00000460: 0a00 0000 0800 0a01 0808 0803 0c03 7202  ..............r.
 00000470: 0000 00da 085f 5f6d 6169 6e5f 5f29 0bda  .....__main__)..
 00000480: 0770 6174 686c 6962 7204 0000 00da 0450  .pathlibr......P
 00000490: 6174 68da 085f 5f66 696c 655f 5fda 0670  ath..__file__..p
 000004a0: 6172 656e 7472 0800 0000 720a 0000 0072  arentr....r....r
 000004b0: 0200 0000 721b 0000 00da 0361 7070 7216  ....r......appr.
 000004c0: 0000 0072 1000 0000 7210 0000 0072 1000  ...r....r....r..
 000004d0: 0000 7211 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000004e0: 3e01 0000 0073 1200 0000 0801 0801 0c01  >....s..........
+000004e0: 3e01 0000 0073 1200 0000 0801 0801 0c02  >....s..........
 000004f0: 0801 0e03 0813 0601 0c01 04fe            ............
```

### Comparing `pygubu-designer-0.35/examples/framepad.ui` & `pygubu-designer-0.36/examples/framepad.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/helloworld/helloworld.py` & `pygubu-designer-0.36/examples/helloworld/helloworld.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/helloworld/helloworld.ui` & `pygubu-designer-0.36/examples/helloworld/helloworld.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/helloworld/holamundo.py` & `pygubu-designer-0.36/examples/helloworld/holamundo.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/helloworld/holamundo.ui` & `pygubu-designer-0.36/examples/helloworld/holamundo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/image_property/green.gif` & `pygubu-designer-0.36/examples/image_property/green.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/image_property/image_property.py` & `pygubu-designer-0.36/examples/image_property/image_property.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/image_property/image_property.ui` & `pygubu-designer-0.36/examples/image_property/image_property.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/image_property/red.gif` & `pygubu-designer-0.36/examples/image_property/red.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/image_property/yellow.gif` & `pygubu-designer-0.36/examples/image_property/yellow.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_cxFreeze/myapp.py` & `pygubu-designer-0.36/examples/integration_with_cxFreeze/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_cxFreeze/myapp.ui` & `pygubu-designer-0.36/examples/integration_with_cxFreeze/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_cxFreeze/setup.py` & `pygubu-designer-0.36/examples/integration_with_cxFreeze/setup.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_nuitka/myapp.py` & `pygubu-designer-0.36/examples/integration_with_nuitka/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_nuitka/myapp.ui` & `pygubu-designer-0.36/examples/integration_with_nuitka/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_py2exe/myapp.py` & `pygubu-designer-0.36/examples/integration_with_py2exe/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_py2exe/myapp.ui` & `pygubu-designer-0.36/examples/integration_with_py2exe/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_py2exe/setup.py` & `pygubu-designer-0.36/examples/integration_with_py2exe/setup.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_pyinstaller/myapp.py` & `pygubu-designer-0.36/examples/integration_with_pyinstaller/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_pyinstaller/myapp.spec` & `pygubu-designer-0.36/examples/integration_with_pyinstaller/myapp.spec`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_pyinstaller/myapp.ui` & `pygubu-designer-0.36/examples/integration_with_pyinstaller/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_tkcalendar/README.md` & `pygubu-designer-0.36/examples/integration_with_tkcalendar/README.md`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp1/__pycache__/tkcalendarwidgets.cpython-38.pyc` & `pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp1/__pycache__/tkcalendarwidgets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp1/main.ui` & `pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp1/main.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp1/myapp.py` & `pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp1/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp2/__pycache__/tkcalendarwidgets.cpython-310.pyc` & `pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp2/__pycache__/tkcalendarwidgets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp2/__pycache__/tkcalendarwidgets.cpython-38.pyc` & `pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp2/__pycache__/tkcalendarwidgets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp2/main.ui` & `pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp2/main.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp2/myapp.py` & `pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp2/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp2/tkcalendarwidgets.py` & `pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp2/tkcalendarwidgets.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp3/__pycache__/tkcalendarwidgets.cpython-310.pyc` & `pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp3/__pycache__/tkcalendarwidgets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp3/__pycache__/tkcalendarwidgets.cpython-38.pyc` & `pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp3/__pycache__/tkcalendarwidgets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp3/main.ui` & `pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp3/main.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp3/myapp.py` & `pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp3/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_tkcalendar/myapp3/tkcalendarwidgets.py` & `pygubu-designer-0.36/examples/integration_with_tkcalendar/myapp3/tkcalendarwidgets.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_zipapp/demoapp.pyz` & `pygubu-designer-0.36/examples/integration_with_zipapp/demoapp.pyz`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_zipapp/src/demoapp/data/demoapp.ui` & `pygubu-designer-0.36/examples/integration_with_zipapp/src/demoapp/data/demoapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_zipapp/src/demoapp/data/green.gif` & `pygubu-designer-0.36/examples/integration_with_zipapp/src/demoapp/data/green.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_zipapp/src/demoapp/data/info.txt` & `pygubu-designer-0.36/examples/integration_with_zipapp/src/demoapp/data/info.txt`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_zipapp/src/demoapp/data/red.gif` & `pygubu-designer-0.36/examples/integration_with_zipapp/src/demoapp/data/red.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_zipapp/src/demoapp/data/yellow.gif` & `pygubu-designer-0.36/examples/integration_with_zipapp/src/demoapp/data/yellow.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/integration_with_zipapp/src/demoapp/main.py` & `pygubu-designer-0.36/examples/integration_with_zipapp/src/demoapp/main.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/jpg_image_on_canvas/demoapp.py` & `pygubu-designer-0.36/examples/jpg_image_on_canvas/demoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/jpg_image_on_canvas/demoapp.ui` & `pygubu-designer-0.36/examples/jpg_image_on_canvas/demoapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/jpg_image_on_canvas/seaside400.jpg` & `pygubu-designer-0.36/examples/jpg_image_on_canvas/seaside400.jpg`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/menubutton.ui` & `pygubu-designer-0.36/examples/menubutton.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/menuexample.ui` & `pygubu-designer-0.36/examples/menuexample.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/notebook/demo1.ui` & `pygubu-designer-0.36/examples/notebook/demo1.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/notebook/demo1app.py` & `pygubu-designer-0.36/examples/notebook/demo1app.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/panedwindow.ui` & `pygubu-designer-0.36/examples/panedwindow.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/panes_and_notebooks.ui` & `pygubu-designer-0.36/examples/panes_and_notebooks.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/pathchooserdemo/demo1/pathchooserdemo.py` & `pygubu-designer-0.36/examples/pathchooserdemo/demo1/pathchooserdemo.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/pathchooserdemo/demo1/pathchooserdemo.ui` & `pygubu-designer-0.36/examples/pathchooserdemo/demo1/pathchooserdemo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/pathchooserdemo/demo2/pathchooserdemo.py` & `pygubu-designer-0.36/examples/pathchooserdemo/demo2/pathchooserdemo.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/pathchooserdemo/demo2/pathchooserdemo.ui` & `pygubu-designer-0.36/examples/pathchooserdemo/demo2/pathchooserdemo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/scrollbarhelper.ui` & `pygubu-designer-0.36/examples/scrollbarhelper.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/scrolledframe-layouts.ui` & `pygubu-designer-0.36/examples/scrolledframe-layouts.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/scrolledframe.ui` & `pygubu-designer-0.36/examples/scrolledframe.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/scrolledtext/scrolledtext_demo.ui` & `pygubu-designer-0.36/examples/scrolledtext/scrolledtext_demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/scrolledtext/scrolledtextdemoapp.py` & `pygubu-designer-0.36/examples/scrolledtext/scrolledtextdemoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/static_image/demoapp.py` & `pygubu-designer-0.36/examples/static_image/demoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/static_image/demoapp.ui` & `pygubu-designer-0.36/examples/static_image/demoapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/static_image/logo_253.png` & `pygubu-designer-0.36/examples/static_image/logo_253.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/text/logwindowdemo/demo1.ui` & `pygubu-designer-0.36/examples/text/logwindowdemo/demo1.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/text/logwindowdemo/demo1app.py` & `pygubu-designer-0.36/examples/text/logwindowdemo/demo1app.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/toplevel_centered/centered_demo1.py` & `pygubu-designer-0.36/examples/toplevel_centered/centered_demo1.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/toplevel_centered/centered_demo2.py` & `pygubu-designer-0.36/examples/toplevel_centered/centered_demo2.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/toplevel_centered/demo.ui` & `pygubu-designer-0.36/examples/toplevel_centered/demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/toplevel_menu/menu.py` & `pygubu-designer-0.36/examples/toplevel_menu/menu.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/toplevel_menu/menu.ui` & `pygubu-designer-0.36/examples/toplevel_menu/menu.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/treeview/demo1/treeview.py` & `pygubu-designer-0.36/examples/treeview/demo1/treeview.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/treeview/demo1/treeview.ui` & `pygubu-designer-0.36/examples/treeview/demo1/treeview.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/treeview/demo2/columns_stretching.ui` & `pygubu-designer-0.36/examples/treeview/demo2/columns_stretching.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/treeview/demo2/columnsstretchingdemo.py` & `pygubu-designer-0.36/examples/treeview/demo2/columnsstretchingdemo.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/user_input/userinput.ui` & `pygubu-designer-0.36/examples/user_input/userinput.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/user_input/userinputapp.py` & `pygubu-designer-0.36/examples/user_input/userinputapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/variables.ui` & `pygubu-designer-0.36/examples/variables.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/vscrolledframe.ui` & `pygubu-designer-0.36/examples/vscrolledframe.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/windowdeleteevent/demo1.py` & `pygubu-designer-0.36/examples/windowdeleteevent/demo1.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/windowdeleteevent/demo1.ui` & `pygubu-designer-0.36/examples/windowdeleteevent/demo1.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/windowdeleteevent/demo2.py` & `pygubu-designer-0.36/examples/windowdeleteevent/demo2.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/examples/windowdeleteevent/demo2.ui` & `pygubu-designer-0.36/examples/windowdeleteevent/demo2.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/pygubu-designer.png` & `pygubu-designer-0.36/pygubu-designer.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/pyproject.toml` & `pygubu-designer-0.36/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
   "Topic :: Software Development :: User Interfaces",
 ]
 dependencies = [
     "appdirs >=1.4.3",
     "Mako >=1.1.4",
     "screeninfo >=0.8",
     "autopep8 >=1.7",
-    "pygubu >=0.30"
+    "pygubu >=0.31"
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/alejandroautalan/pygubu-designer#readme"
 Issues = "https://github.com/alejandroautalan/pygubu-designer/issues"
 Source = "https://github.com/alejandroautalan/pygubu-designer"
```

### Comparing `pygubu-designer-0.35/src/pygubu_designer.egg-info/PKG-INFO` & `pygubu-designer-0.36/src/pygubu_designer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygubu-designer
-Version: 0.35
+Version: 0.36
 Summary: A simple GUI designer for the python tkinter module
 Author-email: Alejandro Autalan <alejandroautalan@gmail.com>
 License: GPL-3
 Project-URL: Documentation, https://github.com/alejandroautalan/pygubu-designer#readme
 Project-URL: Issues, https://github.com/alejandroautalan/pygubu-designer/issues
 Project-URL: Source, https://github.com/alejandroautalan/pygubu-designer
 Keywords: gui,tkinter,designer
```

### Comparing `pygubu-designer-0.35/src/pygubu_designer.egg-info/SOURCES.txt` & `pygubu-designer-0.36/src/pygubu_designer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/actions.py` & `pygubu-designer-0.36/src/pygubudesigner/actions.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/bindingseditor.py` & `pygubu-designer-0.36/src/pygubudesigner/bindingseditor.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/codegen/codebuilder.py` & `pygubu-designer-0.36/src/pygubudesigner/codegen/codebuilder.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,30 +94,33 @@
         self._methods = OrderedDict()
         self._methods_target_code_ids = {}
         self._realize_mode = RealizeMode.APP
         self._current_method = None
         self._current_target = None
         self._generated_target_id = None
         self.all_ids_as_attributes = False
+        self._first_object_created = False
 
     def add_import_line(self, module_name, as_name=None, priority=0):
         if module_name not in self._extra_imports:
             self._extra_imports[module_name] = (as_name, priority)
 
     def _process_options(self, kw):
         kwdef = {
             "as_class": True,
             "tabspaces": 8,
             "script_type": ScriptType.APP_WITH_UI,
+            "on_first_object_cb": None,
         }
         kwdef.update(kw)
         self._options = kwdef
         self.as_class = self._options["as_class"]
         self.tabspaces = self._options["tabspaces"]
         self._script_type = self._options["script_type"]
+        self._on_first_object_cb = self._options["on_first_object_cb"]
 
     def _process_results(self, target):
         code = []
         for line in self._code:
             line = "{}{}\n".format(" " * self.tabspaces, line)
             code.append(line)
         code = "".join(code)
@@ -167,21 +170,28 @@
             target,
             as_class=False,
             tabspaces=8,
             script_type=ScriptType.APP_WITH_UI,
         )
         return self._process_results(target)
 
-    def generate_app_code(self, uidef, target, methods_for: list = None):
+    def generate_app_code(
+        self,
+        uidef,
+        target,
+        methods_for: list = None,
+        on_first_object_cb: str = None,
+    ):
         self.generate(
             uidef,
             target,
             as_class=True,
             tabspaces=8,
             script_type=ScriptType.APP_CODE,
+            on_first_object_cb=on_first_object_cb,
         )
         if methods_for is not None:
             self._realize_mode = RealizeMode.METHOD
             for target_id in methods_for:
                 self._current_method = target_id
                 self._methods[target_id] = []
                 self._methods_target_code_ids = {}
@@ -387,14 +397,27 @@
             create = builder.code_realize(bmaster, uniqueid)
             self._add_new_code(create)
 
             # configuration
             configure = builder.code_configure()
             self._add_new_code(configure)
 
+            # <<
+            if (
+                self._first_object_created is False
+                and self._on_first_object_cb is not None
+            ):
+                lines = [
+                    "# First object created",
+                    f"{self._on_first_object_cb}({uniqueid})",
+                    "",
+                ]
+                self._add_new_code(lines)
+                self._first_object_created = True
+
             # Children
             for childmeta in self.uidefinition.widget_children(originalid):
                 childid = self._code_realize(builder, childmeta)
                 code = builder.code_child_add(childid)
                 self._add_new_code(code)
 
             # Configuration after adding all children
```

### Comparing `pygubu-designer-0.35/src/pygubudesigner/codegen/scriptgenerator.py` & `pygubu-designer-0.36/src/pygubudesigner/codegen/scriptgenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,20 +184,27 @@
                 self.set_code(final_code)
             elif template == "codescript":
                 if not main_widget_is_toplevel:
                     generator.add_import_line("tkinter", "tk")
                 if self.use_ttkdefs_file_var.get():
                     generator.add_import_line("tkinter.ttk", "ttk", priority=1)
 
+                first_object_callback = None
+                if self.use_ttkdefs_file_var.get():
+                    first_object_callback = "self.setup_ttk_styles"
+
                 methods = []
                 if set_main_menu:
                     methods.append(main_menu_id)
                 # Generate code
                 code = generator.generate_app_code(
-                    uidef, target, methods_for=methods
+                    uidef,
+                    target,
+                    methods_for=methods,
+                    on_first_object_cb=first_object_callback,
                 )
 
                 # Prepare template context
                 context["widget_code"] = code[target]
                 context["import_lines"] = code["imports"]
                 context["callbacks"] = code["callbacks"]
                 context["methods"] = code["methods"]
```

### Comparing `pygubu-designer-0.35/src/pygubudesigner/containerlayouteditor.py` & `pygubu-designer-0.36/src/pygubudesigner/containerlayouteditor.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/code_templates/app.py.mako` & `pygubu-designer-0.36/src/pygubudesigner/data/code_templates/app.py.mako`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,26 @@
 <%block name="project_paths" filter="trim">
 PROJECT_PATH = pathlib.Path(__file__).parent
 PROJECT_UI = PROJECT_PATH / "${project_name}"
 </%block>
 
 <%block name="class_definition" filter="trim">
 class ${class_name}:
-%if with_i18n_support:
+%if with_i18n_support and has_ttk_styles:
+    def __init__(self, master=None, translator=None):
+        self.builder = builder = pygubu.Builder(
+            translator=translator,
+            on_first_object=self.setup_ttk_styles)
+%elif with_i18n_support:
     def __init__(self, master=None, translator=None):
         self.builder = builder = pygubu.Builder(translator)
+%elif has_ttk_styles:
+    def __init__(self, master=None):
+        self.builder = builder = pygubu.Builder(
+            on_first_object=self.setup_ttk_styles)
 %else:
     def __init__(self, master=None):
         self.builder = builder = pygubu.Builder()
 %endif
         builder.add_resource_path(PROJECT_PATH)
         builder.add_from_file(PROJECT_UI)
         # Main widget
@@ -26,26 +35,21 @@
 
           %for var in tkvariables:
         self.${var} = None
           %endfor
         builder.import_variables(self, ${tkvariables})
 
         %endif
-        %if has_ttk_styles:
-
-        self.setup_ttk_styles()
-
-        %endif
         builder.connect_callbacks(self)
 
     def run(self):
         self.mainwindow.mainloop()
     %if has_ttk_styles:
 
-    def setup_ttk_styles(self):
+    def setup_ttk_styles(self, widget=None):
         # ttk styles configuration
         self.style = style = ttk.Style()
         optiondb = style.master
 ${ttk_styles}
     %endif
 
 ${callbacks}\
```

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/code_templates/customstyles.py.mako` & `pygubu-designer-0.36/src/pygubudesigner/data/code_templates/customstyles.py.mako`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/code_templates/script.py.mako` & `pygubu-designer-0.36/src/pygubudesigner/data/code_templates/script.py.mako`

 * *Files 13% similar despite different names*

```diff
@@ -15,24 +15,20 @@
         # Main widget
         self.mainwindow = ${target_code_id}
 %if set_main_menu:
         # Main menu
         _main_menu = self.create_${main_menu_id}(self.mainwindow)
         self.mainwindow.configure(menu=_main_menu)
 %endif
-        %if has_ttk_styles:
-
-        self.setup_ttk_styles()
-        %endif
 
     def run(self):
         self.mainwindow.mainloop()
     %if has_ttk_styles:
 
-    def setup_ttk_styles(self):
+    def setup_ttk_styles(self, widget=None):
         # ttk styles configuration
         self.style = style = ttk.Style()
         optiondb = style.master
 ${ttk_styles}
     %endif
 
 ${methods}\
```

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/code_templates/widget.py.mako` & `pygubu-designer-0.36/src/pygubudesigner/data/code_templates/widget.py.mako`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/pygubu.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/pygubu.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/pygubu200.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/pygubu200.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.dialog.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.dialog.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.editabletreeview.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.editabletreeview.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrolledframe.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrolledframe.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Button.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Button.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Calendar.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Calendar.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Canvas.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Canvas.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Checkbutton.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Checkbutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Entry.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Entry.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Frame.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Frame.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Label.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Label.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Listbox.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Listbox.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menu.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menu.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menubutton.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menubutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Checkbutton.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Checkbutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Command.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Command.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Radiobutton.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Radiobutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Separator.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Separator.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Submenu.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Submenu.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.Pane.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.Pane.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Radiobutton.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Radiobutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scale.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scale.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scrollbar.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scrollbar.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Spinbox.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Spinbox.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Text.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Text.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Toplevel.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Toplevel.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.default.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.default.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Button.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Button.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Checkbutton.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Checkbutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Combobox.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Combobox.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Entry.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Entry.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Frame.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Frame.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Label.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Label.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.LabeledScale.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.LabeledScale.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Menubutton.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Menubutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.Pane.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.Pane.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Progressbar.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Progressbar.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Radiobutton.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Radiobutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scale.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scale.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scrollbar.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scrollbar.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Separator.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Separator.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Spinbox.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Spinbox.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Canvas.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Canvas.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-bold.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-bold.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-italic.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-italic.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-underline.gif` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-underline.gif`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/property_invalid.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/property_invalid.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/pygubu.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/pygubu.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/pygubu200.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/pygubu200.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.combobox.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.combobox.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.toplevelmenu.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.toplevelmenu.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Button.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Button.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Canvas.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Canvas.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Checkbutton.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Checkbutton.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Label.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Label.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menu.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menu.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Checkbutton.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Checkbutton.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Submenu.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Submenu.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Spinbox.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Spinbox.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Button.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Button.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Checkbutton.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Checkbutton.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Combobox.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Combobox.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Label.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Label.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Progressbar.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Progressbar.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Spinbox.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Spinbox.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Canvas.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Canvas.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-bold.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-bold.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-italic.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-italic.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-strikethrough.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-strikethrough.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-underline.png` & `pygubu-designer-0.36/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-underline.png`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu-designer.mo` & `pygubu-designer-0.36/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu-designer.mo`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu-designer.mo` & `pygubu-designer-0.36/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu-designer.mo`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu.mo` & `pygubu-designer-0.36/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu.mo`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/locale/pygubu-designer.pot` & `pygubu-designer-0.36/src/pygubudesigner/data/locale/pygubu-designer.pot`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/locale/pygubu.pot` & `pygubu-designer-0.36/src/pygubudesigner/data/locale/pygubu.pot`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/locale/tr/LC_MESSAGES/pygubu-designer.mo` & `pygubu-designer-0.36/src/pygubudesigner/data/locale/tr/LC_MESSAGES/pygubu-designer.mo`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu-designer.mo` & `pygubu-designer-0.36/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu-designer.mo`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu.mo` & `pygubu-designer-0.36/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu.mo`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu-designer.mo` & `pygubu-designer-0.36/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu-designer.mo`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/ui/about_dialog.ui` & `pygubu-designer-0.36/src/pygubudesigner/data/ui/about_dialog.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/ui/ask_save_changes_dialog.ui` & `pygubu-designer-0.36/src/pygubudesigner/data/ui/ask_save_changes_dialog.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/ui/container_layout_editor_base.ui` & `pygubu-designer-0.36/src/pygubudesigner/data/ui/container_layout_editor_base.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/ui/preferences_dialog.ui` & `pygubu-designer-0.36/src/pygubudesigner/data/ui/preferences_dialog.ui`

 * *Files 1% similar despite different names*

#### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/ui/preferences_dialog.ui` & `pygubu-designer-0.36/src/pygubudesigner/data/ui/preferences_dialog.ui`

```diff
@@ -132,14 +132,28 @@
                               <property name="column">0</property>
                               <property name="pady">4</property>
                               <property name="row">3</property>
                               <property name="sticky">w</property>
                             </layout>
                           </object>
                         </child>
+                        <child>
+                          <object class="ttk.Checkbutton" id="chk_auto_generate_code">
+                            <property name="offvalue">no</property>
+                            <property name="onvalue">yes</property>
+                            <property name="text" translatable="yes">Automatically generate code</property>
+                            <property name="variable">string:auto_generate_code</property>
+                            <layout manager="grid">
+                              <property name="column">0</property>
+                              <property name="pady">4</property>
+                              <property name="row">4</property>
+                              <property name="sticky">w</property>
+                            </layout>
+                          </object>
+                        </child>
                       </object>
                     </child>
                     <child>
                       <object class="ttk.Labelframe" id="labelframe_1">
                         <property name="height">200</property>
                         <property name="padding">10 0 10 5</property>
                         <property name="text" translatable="yes">Widget naming</property>
```

### Comparing `pygubu-designer-0.35/src/pygubudesigner/data/ui/pygubu-ui.ui` & `pygubu-designer-0.36/src/pygubudesigner/data/ui/pygubu-ui.ui`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/dialogs.py` & `pygubu-designer-0.36/src/pygubudesigner/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/i18n.py` & `pygubu-designer-0.36/src/pygubudesigner/i18n.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/layouteditor.py` & `pygubu-designer-0.36/src/pygubudesigner/layouteditor.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/logpanel.py` & `pygubu-designer-0.36/src/pygubudesigner/logpanel.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/main.py` & `pygubu-designer-0.36/src/pygubudesigner/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -872,24 +872,28 @@
         else:
             name = Path(self.currentfile).name
         return name
 
     def nbmain_tab_changed(self, event):
         if event.widget.index("current") == 1:  # Index 1 is the code-tab
             self.script_generator.configure()
+            if pref.get_option("auto_generate_code") == "yes":
+                self.on_code_generate_clicked()
 
     # Tab code management
     def on_code_generate_clicked(self):
         self.script_generator.on_code_generate_clicked()
 
     def on_code_copy_clicked(self):
         self.script_generator.on_code_copy_clicked()
 
     def on_code_template_changed(self):
         self.script_generator.on_code_template_changed()
+        if pref.get_option("auto_generate_code") == "yes":
+            self.on_code_generate_clicked()
 
     def on_code_save_clicked(self):
         self.script_generator.on_code_save_clicked()
 
     def setup_bottom_panel(self):
         self.log_panel = LogPanelManager(self)
         self.setup_logger_handler()
```

### Comparing `pygubu-designer-0.35/src/pygubudesigner/preferences.py` & `pygubu-designer-0.36/src/pygubudesigner/preferences.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,18 @@
         "values": '["pack", "grid", "place"]',
         "default": "pack",
     },
     "center_preview": {
         "values": '["yes", "no"]',
         "default": "no",
     },
+    "auto_generate_code": {
+        "values": '["yes", "no"]',
+        "default": "no",
+    },
     "geometry": {
         "default": "640x480",
     },
     "widget_naming_separator": {
         "values": '["NONE", "UNDERSCORE"]',
         "default": "NONE",
     },
```

### Comparing `pygubu-designer-0.35/src/pygubudesigner/preview/builder.py` & `pygubu-designer-0.36/src/pygubudesigner/preview/builder.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/preview/helper.py` & `pygubu-designer-0.36/src/pygubudesigner/preview/helper.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/preview/preview.py` & `pygubu-designer-0.36/src/pygubudesigner/preview/preview.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/properties/manager.py` & `pygubu-designer-0.36/src/pygubudesigner/properties/manager.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/properties/predefined.py` & `pygubu-designer-0.36/src/pygubudesigner/properties/predefined.py`

 * *Files 0% similar despite different names*

```diff
@@ -1579,15 +1579,15 @@
         "params": {"mode": "whentry"},
         "help": help_for("maxsize-toplevel"),
     },
     "overrideredirect": {
         "editor": "dynamic",
         "params": {
             "mode": "choice",
-            "values": ("", "True", "False"),
+            "values": ("", "true", "false"),
             "state": "readonly",
         },
         "help": help_for("overrideredirect-custom"),
     },
     "resizable": {
         "editor": "dynamic",
         "params": {
@@ -1650,16 +1650,16 @@
     # pack/grid/place common properties
     "padx": {"editor": "twodimensionentry", "help": help_for("padx-layout")},
     "pady": {"editor": "twodimensionentry", "help": help_for("pady-layout")},
     "ipadx": {"editor": "dimensionentry", "help": help_for("ipadx-layout")},
     "ipady": {"editor": "dimensionentry", "help": help_for("ipady-layout")},
     "propagate": {
         "editor": "choice",
-        "params": {"values": ("True", "False"), "state": "readonly"},
-        "default": "True",
+        "params": {"values": ("true", "false"), "state": "readonly"},
+        "default": "true",
         "help": help_for("propagate-layout"),
     },
     "anchor": {
         "editor": "choice",
         "params": {
             "values": (
                 "",
```

### Comparing `pygubu-designer-0.35/src/pygubudesigner/properties/propertieshelp.py` & `pygubu-designer-0.36/src/pygubudesigner/properties/propertieshelp.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/propertieseditor.py` & `pygubu-designer-0.36/src/pygubudesigner/propertieseditor.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/rfilemanager.py` & `pygubu-designer-0.36/src/pygubudesigner/rfilemanager.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/stylehandler.py` & `pygubu-designer-0.36/src/pygubudesigner/stylehandler.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/uitreeeditor.py` & `pygubu-designer-0.36/src/pygubudesigner/uitreeeditor.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/util/__init__.py` & `pygubu-designer-0.36/src/pygubudesigner/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/util/gridcalculator.py` & `pygubu-designer-0.36/src/pygubudesigner/util/gridcalculator.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/util/keyboard.py` & `pygubu-designer-0.36/src/pygubudesigner/util/keyboard.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/util/observable.py` & `pygubu-designer-0.36/src/pygubudesigner/util/observable.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/util/screens.py` & `pygubu-designer-0.36/src/pygubudesigner/util/screens.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/util/selecttool.py` & `pygubu-designer-0.36/src/pygubudesigner/util/selecttool.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgetdescr.py` & `pygubu-designer-0.36/src/pygubudesigner/widgetdescr.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgets/__init__.py` & `pygubu-designer-0.36/src/pygubudesigner/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgets/bindingeditor.py` & `pygubu-designer-0.36/src/pygubudesigner/widgets/bindingeditor.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,16 @@
     "ButtonPress",
     "Button",
     "ButtonRelease",
     "Configure",
     "Deactivate",
     "Destroy",
     "Enter",
-    "ExposeFocusIn",
+    "Expose",
+    "FocusIn",
     "FocusOut",
     "KeyPress",
     "Key",
     "KeyRelease",
     "Leave",
     "Map",
     "Motion",
```

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgets/colorentry.py` & `pygubu-designer-0.36/src/pygubudesigner/widgets/colorentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgets/commandentry.py` & `pygubu-designer-0.36/src/pygubudesigner/widgets/commandentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgets/componentpalette.py` & `pygubu-designer-0.36/src/pygubudesigner/widgets/componentpalette.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgets/containerlayouteditorbase.py` & `pygubu-designer-0.36/src/pygubudesigner/widgets/containerlayouteditorbase.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgets/cursorentry.py` & `pygubu-designer-0.36/src/pygubudesigner/widgets/cursorentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgets/dimensionentry.py` & `pygubu-designer-0.36/src/pygubudesigner/widgets/dimensionentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgets/dynamicpropeditor.py` & `pygubu-designer-0.36/src/pygubudesigner/widgets/dynamicpropeditor.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgets/entryvalidatecommandeditor.py` & `pygubu-designer-0.36/src/pygubudesigner/widgets/entryvalidatecommandeditor.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgets/fontentry.py` & `pygubu-designer-0.36/src/pygubudesigner/widgets/fontentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgets/gridselector.py` & `pygubu-designer-0.36/src/pygubudesigner/widgets/gridselector.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgets/imageentry.py` & `pygubu-designer-0.36/src/pygubudesigner/widgets/imageentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgets/namedideditor.py` & `pygubu-designer-0.36/src/pygubudesigner/widgets/namedideditor.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgets/pixelcoordinateentry.py` & `pygubu-designer-0.36/src/pygubudesigner/widgets/pixelcoordinateentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgets/propertyeditor.py` & `pygubu-designer-0.36/src/pygubudesigner/widgets/propertyeditor.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgets/relativeentry.py` & `pygubu-designer-0.36/src/pygubudesigner/widgets/relativeentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgets/stickyentry.py` & `pygubu-designer-0.36/src/pygubudesigner/widgets/stickyentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgets/tkvarentry.py` & `pygubu-designer-0.36/src/pygubudesigner/widgets/tkvarentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgets/toolbarframe.py` & `pygubu-designer-0.36/src/pygubudesigner/widgets/toolbarframe.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgets/ttkstyleentry.py` & `pygubu-designer-0.36/src/pygubudesigner/widgets/ttkstyleentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-designer-0.35/src/pygubudesigner/widgets/whentry.py` & `pygubu-designer-0.36/src/pygubudesigner/widgets/whentry.py`

 * *Files identical despite different names*

