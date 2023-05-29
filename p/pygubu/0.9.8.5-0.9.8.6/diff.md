# Comparing `tmp/pygubu-0.9.8.5.tar.gz` & `tmp/pygubu-0.9.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pygubu-0.9.8.5.tar", last modified: Fri Mar 13 23:52:49 2020, max compression
+gzip compressed data, was "dist/pygubu-0.9.8.6.tar", last modified: Mon Mar 23 21:43:53 2020, max compression
```

## Comparing `pygubu-0.9.8.5.tar` & `pygubu-0.9.8.6.tar`

### file list

```diff
@@ -1,299 +1,299 @@
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:49.000000 pygubu-0.9.8.5/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    35068 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/COPYING
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/examples/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2860 2018-07-08 00:30:31.000000 pygubu-0.9.8.5/examples/commands.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      842 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/canvas_example.ui
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      546 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/binding.ui
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1012 2018-07-08 00:30:31.000000 pygubu-0.9.8.5/examples/button_cb.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3131 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/panes_and_notebooks.ui
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/examples/cx_freeze/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    13917 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/cx_freeze/myapp.ui
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1123 2018-07-08 00:30:31.000000 pygubu-0.9.8.5/examples/cx_freeze/setup.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     6306 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/cx_freeze/myapp.py
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/examples/cx_freeze/imgs/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      131 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/cx_freeze/imgs/ps_triangle.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       90 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/cx_freeze/imgs/ps_circle.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       86 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/cx_freeze/imgs/ps_square.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       72 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/cx_freeze/imgs/MenuIcon4.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      104 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/cx_freeze/imgs/ps_cross.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1631 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/example_grid_rc_2.ui
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4346 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/vscrolledframe.ui
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1840 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/scrollbarhelper.ui
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2458 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/menu.ui
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      883 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/variables.ui
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1628 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/button_cb.ui
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/examples/py2exe/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    13917 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/py2exe/myapp.ui
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1064 2018-07-08 00:30:31.000000 pygubu-0.9.8.5/examples/py2exe/setup.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     6296 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/py2exe/myapp.py
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/examples/py2exe/imgs/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      131 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/py2exe/imgs/ps_triangle.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       90 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/py2exe/imgs/ps_circle.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       86 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/py2exe/imgs/ps_square.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       72 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/py2exe/imgs/MenuIcon4.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      104 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/py2exe/imgs/ps_cross.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     9388 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/scrolledframe.ui
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1835 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/panedwindow.ui
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    13778 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/commands.ui
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1207 2018-07-08 00:30:31.000000 pygubu-0.9.8.5/examples/menu.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      723 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/framepad.ui
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/examples/nuitka/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    13917 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/nuitka/myapp.ui
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      140 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/nuitka/compile.bat
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     6152 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/nuitka/myapp.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       73 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/nuitka/copydatafiles.bat
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/examples/nuitka/imgs/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      131 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/nuitka/imgs/ps_triangle.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       90 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/nuitka/imgs/ps_circle.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       86 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/nuitka/imgs/ps_square.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       72 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/nuitka/imgs/MenuIcon4.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      104 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/nuitka/imgs/ps_cross.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      457 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/nuitka/nuitkahelper.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1471 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/example_grid_rc.ui
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1347 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/menuexample.ui
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2383 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/treeview.ui
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/examples/helloworld/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1608 2020-03-01 21:50:40.000000 pygubu-0.9.8.5/examples/helloworld/helloworld.ui
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      483 2020-03-01 21:50:40.000000 pygubu-0.9.8.5/examples/helloworld/helloworld.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1606 2020-03-01 21:50:40.000000 pygubu-0.9.8.5/examples/helloworld/holamundo.ui
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      482 2020-03-01 21:50:40.000000 pygubu-0.9.8.5/examples/helloworld/holamundo.py
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/examples/pyinstaller/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    13917 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/pyinstaller/myapp.ui
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1358 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/pyinstaller/myapp.spec
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     6296 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/pyinstaller/myapp.py
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/examples/pyinstaller/imgs/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      131 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/pyinstaller/imgs/ps_triangle.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       90 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/pyinstaller/imgs/ps_circle.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       86 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/pyinstaller/imgs/ps_square.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       72 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/pyinstaller/imgs/MenuIcon4.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      104 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/pyinstaller/imgs/ps_cross.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3187 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/examples/menubutton.ui
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      763 2018-07-08 00:30:31.000000 pygubu-0.9.8.5/examples/treeview.py
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/po/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     7100 2018-07-08 00:30:31.000000 pygubu-0.9.8.5/po/pygubu.pot
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      375 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/po/pygubu.mo
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4112 2020-03-01 21:50:40.000000 pygubu-0.9.8.5/setup.py
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/pygubu.egg-info/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       22 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/pygubu.egg-info/top_level.txt
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    11445 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/pygubu.egg-info/SOURCES.txt
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        1 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/pygubu.egg-info/dependency_links.txt
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2748 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/pygubu.egg-info/PKG-INFO
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       13 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/pygubu.egg-info/requires.txt
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       66 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/pygubu.egg-info/entry_points.txt
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/pygubu/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1962 2020-03-13 23:46:26.000000 pygubu-0.9.8.5/pygubu/__init__.py
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/pygubu/widgets/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        0 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubu/widgets/__init__.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1019 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubu/widgets/scrollbarhelper.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4454 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubu/widgets/dialog.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4643 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubu/widgets/accordionframe.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1026 2018-07-08 00:30:32.000000 pygubu-0.9.8.5/pygubu/widgets/ttkspinbox.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     6009 2019-10-02 02:35:20.000000 pygubu-0.9.8.5/pygubu/widgets/tkscrollbarhelper.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    18429 2019-07-24 02:26:35.000000 pygubu-0.9.8.5/pygubu/widgets/calendarframe.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2989 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubu/widgets/autoarrangeframe.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    12401 2020-03-13 23:42:39.000000 pygubu-0.9.8.5/pygubu/widgets/tkscrolledframe.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1010 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubu/widgets/scrolledframe.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     7336 2019-07-24 02:26:35.000000 pygubu-0.9.8.5/pygubu/widgets/combobox.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3787 2019-07-24 02:26:35.000000 pygubu-0.9.8.5/pygubu/widgets/pathchooserinput.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1781 2019-07-24 02:26:35.000000 pygubu-0.9.8.5/pygubu/widgets/simpletooltip.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    10709 2019-10-02 02:35:20.000000 pygubu-0.9.8.5/pygubu/widgets/editabletreeview.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3394 2018-05-13 16:19:39.000000 pygubu-0.9.8.5/pygubu/binding.py
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/pygubu/builder/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    14127 2020-03-04 00:48:46.000000 pygubu-0.9.8.5/pygubu/builder/__init__.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    24059 2020-03-04 03:43:13.000000 pygubu-0.9.8.5/pygubu/builder/tkstdwidgets.py
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/pygubu/builder/widgets/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        0 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubu/builder/widgets/__init__.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      968 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubu/builder/widgets/scrollbarhelper.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1288 2018-07-08 00:30:32.000000 pygubu-0.9.8.5/pygubu/builder/widgets/dialog.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1144 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubu/builder/widgets/tkscrollbarhelper.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2075 2019-07-24 02:26:35.000000 pygubu-0.9.8.5/pygubu/builder/widgets/calendarframe.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1543 2018-07-08 00:30:32.000000 pygubu-0.9.8.5/pygubu/builder/widgets/tkscrolledframe.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1389 2018-07-08 00:30:32.000000 pygubu-0.9.8.5/pygubu/builder/widgets/scrolledframe.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1049 2019-07-24 02:26:35.000000 pygubu-0.9.8.5/pygubu/builder/widgets/combobox.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1159 2019-07-24 02:26:35.000000 pygubu-0.9.8.5/pygubu/builder/widgets/pathchooserinput.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      859 2018-07-08 00:30:32.000000 pygubu-0.9.8.5/pygubu/builder/widgets/editabletreeview.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    14564 2019-07-23 05:40:39.000000 pygubu-0.9.8.5/pygubu/builder/ttkstdwidgets.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     9967 2020-03-04 00:48:46.000000 pygubu-0.9.8.5/pygubu/builder/builderobject.py
--rwxrwxr-x   0 alejandro  (1000) alejandro  (1000)     4560 2018-07-08 00:30:32.000000 pygubu-0.9.8.5/pygubu/ui2code.py
--rwxrwxr-x   0 alejandro  (1000) alejandro  (1000)     2722 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubu/testui.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     6624 2019-11-03 04:12:09.000000 pygubu-0.9.8.5/pygubu/stockimage.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     5993 2020-03-01 21:50:40.000000 pygubu-0.9.8.5/README.md
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      146 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/MANIFEST.in
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       38 2020-03-13 23:52:49.000000 pygubu-0.9.8.5/setup.cfg
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/pygubudesigner/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1450 2018-07-08 00:30:32.000000 pygubu-0.9.8.5/pygubudesigner/__init__.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     9000 2020-03-04 00:48:46.000000 pygubu-0.9.8.5/pygubudesigner/layouteditor.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3905 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/widgetdescr.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    21327 2020-03-04 03:00:30.000000 pygubu-0.9.8.5/pygubudesigner/previewer.py
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:49.000000 pygubu-0.9.8.5/pygubudesigner/widgets/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      575 2018-07-08 00:30:32.000000 pygubu-0.9.8.5/pygubudesigner/widgets/__init__.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2310 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/widgets/tkvarentry.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4590 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/widgets/sizeentry.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2312 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/widgets/dimensionentry.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     8296 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/widgets/fontentry.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2617 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/widgets/whentry.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     5387 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/widgets/stickyentry.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     8799 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/widgets/propertyeditor.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2738 2019-11-03 04:12:09.000000 pygubu-0.9.8.5/pygubudesigner/widgets/imageentry.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4631 2020-03-04 02:25:51.000000 pygubu-0.9.8.5/pygubudesigner/widgets/toplevelframe.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2278 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/widgets/dynamicpropeditor.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3411 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/widgets/colorentry.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    22792 2020-03-04 03:30:20.000000 pygubu-0.9.8.5/pygubudesigner/main.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    27488 2020-03-04 03:36:26.000000 pygubu-0.9.8.5/pygubudesigner/uitreeeditor.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3816 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/bindingseditor.py
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:49.000000 pygubu-0.9.8.5/pygubudesigner/ui/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    40338 2019-07-24 02:26:35.000000 pygubu-0.9.8.5/pygubudesigner/ui/pygubu-ui.ui
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    14277 2018-07-08 00:30:32.000000 pygubu-0.9.8.5/pygubudesigner/ui/preferences_dialog.ui
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4414 2018-07-08 00:26:59.000000 pygubu-0.9.8.5/pygubudesigner/ui/about_dialog.ui
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1646 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/widgeteditor.py
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:49.000000 pygubu-0.9.8.5/pygubudesigner/util/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3471 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/util/__init__.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1270 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/util/observable.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3033 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/util/selecttool.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1574 2018-07-08 00:30:32.000000 pygubu-0.9.8.5/pygubudesigner/i18n.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     5794 2019-07-23 04:22:51.000000 pygubu-0.9.8.5/pygubudesigner/propertieseditor.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      122 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/__main__.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    27083 2019-07-23 02:46:24.000000 pygubu-0.9.8.5/pygubudesigner/properties.py
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/pygubudesigner/locale/
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/pygubudesigner/locale/de/
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:49.000000 pygubu-0.9.8.5/pygubudesigner/locale/de/LC_MESSAGES/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     8797 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/locale/de/LC_MESSAGES/pygubu.po
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     5210 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/locale/de/LC_MESSAGES/pygubu.mo
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/pygubudesigner/locale/es/
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:49.000000 pygubu-0.9.8.5/pygubudesigner/locale/es/LC_MESSAGES/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     8669 2018-07-08 00:30:32.000000 pygubu-0.9.8.5/pygubudesigner/locale/es/LC_MESSAGES/pygubu.po
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     5001 2018-07-08 00:30:32.000000 pygubu-0.9.8.5/pygubudesigner/locale/es/LC_MESSAGES/pygubu.mo
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:49.000000 pygubu-0.9.8.5/pygubudesigner/images/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       70 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/indicator_ne.gif
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:48.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:49.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      111 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Scale.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      124 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/ttk.Radiobutton.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      124 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Radiobutton.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      124 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/ttk.Frame.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      599 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Canvas.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      108 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.PanedWindow.Pane.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       96 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/ttk.Entry.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      130 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Listbox.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      139 2018-07-08 00:30:32.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/pygubu.builder.widgets.calendarframe.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      118 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/ttk.Checkbutton.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      197 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/pygubu.builder.widgets.scrolledframe.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      108 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/ttk.Panedwindow.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      125 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Toplevel.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      108 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Menuitem.Command.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      121 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Scrollbar.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      155 2018-07-08 00:30:32.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/pygubu.builder.widgets.combobox.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      111 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/ttk.Scale.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      114 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Text.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      140 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Menubutton.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      130 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/ttk.Treeview.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      125 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/pygubu.builder.widgets.dialog.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      156 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Menuitem.Checkbutton.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      139 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Calendar.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      156 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/ttk.Treeview.Column.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      140 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/ttk.Menubutton.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      108 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Menuitem.Separator.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      197 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/pygubu.builder.widgets.tkscrolledframe.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       89 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Message.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       89 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/ttk.Separator.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      124 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Frame.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      195 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Menuitem.Radiobutton.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      108 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/ttk.Panedwindow.Pane.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      105 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/ttk.Label.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      138 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Button.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      153 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/pygubu.builder.widgets.tkscrollbarhelper.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      139 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Menu.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      155 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/ttk.Combobox.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       96 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.default.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      129 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/ttk.Labelframe.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      108 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.PanedWindow.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      131 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/ttk.Notebook.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      133 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/ttk.Spinbox.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      121 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/ttk.Scrollbar.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       96 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Entry.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      153 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/pygubu.builder.widgets.scrollbarhelper.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      118 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Checkbutton.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       96 2018-07-08 00:30:32.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/pygubu.builder.widgets.pathchooserinput.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      132 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/pygubu.builder.widgets.Labelwidget.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      138 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/ttk.Button.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      125 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/ttk.Progressbar.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      129 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.LabelFrame.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      153 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/ttk.Sizegrip.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      133 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Spinbox.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      139 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Menuitem.Submenu.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      142 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/ttk.Notebook.Tab.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      130 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/pygubu.builder.widgets.editabletreeview.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      105 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Label.gif
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:49.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/fontentry/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      567 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/fontentry/format-text-italic.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      357 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/fontentry/format-text-strikethrough.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      592 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/fontentry/format-text-bold.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      572 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/fontentry/format-text-underline.gif
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:49.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/propertyeditor/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      377 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/propertyeditor/property_invalid.gif
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-13 23:52:49.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Scale.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Radiobutton.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Radiobutton.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Frame.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Canvas.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.PanedWindow.Pane.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Entry.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Listbox.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      352 2018-07-08 00:30:32.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.calendarframe.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Checkbutton.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.scrolledframe.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Panedwindow.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Toplevel.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Menuitem.Command.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Scrollbar.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Scale.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Text.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Menubutton.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Treeview.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.dialog.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Menuitem.Checkbutton.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Calendar.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      109 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Treeview.Column.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Menubutton.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Menuitem.Separator.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       75 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Message.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Separator.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Frame.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Menuitem.Radiobutton.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Panedwindow.Pane.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Label.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Button.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Menu.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1120 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Combobox.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.default.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      126 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Labelframe.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.PanedWindow.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Notebook.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Spinbox.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Scrollbar.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Entry.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Checkbutton.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      128 2018-07-08 00:30:32.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.pathchooserinput.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      107 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.Labelwidget.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Button.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Progressbar.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      105 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.LabelFrame.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      105 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Sizegrip.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Spinbox.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Menuitem.Submenu.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      100 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Notebook.Tab.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.editabletreeview.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Label.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       74 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/mglass.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      875 2018-07-08 00:26:59.000000 pygubu-0.9.8.5/pygubudesigner/images/pygubu.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       61 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/close.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       69 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/indicator_nw.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4897 2018-07-08 00:26:59.000000 pygubu-0.9.8.5/pygubudesigner/images/pygubu200.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       70 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/indicator_sw.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       69 2018-01-17 20:34:39.000000 pygubu-0.9.8.5/pygubudesigner/images/indicator_se.gif
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4722 2019-07-24 02:26:35.000000 pygubu-0.9.8.5/pygubudesigner/preferences.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2748 2020-03-13 23:52:49.000000 pygubu-0.9.8.5/PKG-INFO
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    35068 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/COPYING
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/examples/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2860 2018-07-08 00:30:31.000000 pygubu-0.9.8.6/examples/commands.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      842 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/canvas_example.ui
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      546 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/binding.ui
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1012 2018-07-08 00:30:31.000000 pygubu-0.9.8.6/examples/button_cb.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3131 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/panes_and_notebooks.ui
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/examples/cx_freeze/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    13917 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/cx_freeze/myapp.ui
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1123 2018-07-08 00:30:31.000000 pygubu-0.9.8.6/examples/cx_freeze/setup.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     6306 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/cx_freeze/myapp.py
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/examples/cx_freeze/imgs/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      131 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/cx_freeze/imgs/ps_triangle.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       90 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/cx_freeze/imgs/ps_circle.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       86 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/cx_freeze/imgs/ps_square.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       72 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/cx_freeze/imgs/MenuIcon4.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      104 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/cx_freeze/imgs/ps_cross.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1631 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/example_grid_rc_2.ui
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4346 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/vscrolledframe.ui
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1840 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/scrollbarhelper.ui
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2458 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/menu.ui
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      883 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/variables.ui
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1628 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/button_cb.ui
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/examples/py2exe/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    13917 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/py2exe/myapp.ui
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1064 2018-07-08 00:30:31.000000 pygubu-0.9.8.6/examples/py2exe/setup.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     6296 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/py2exe/myapp.py
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/examples/py2exe/imgs/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      131 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/py2exe/imgs/ps_triangle.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       90 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/py2exe/imgs/ps_circle.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       86 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/py2exe/imgs/ps_square.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       72 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/py2exe/imgs/MenuIcon4.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      104 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/py2exe/imgs/ps_cross.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     9388 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/scrolledframe.ui
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1835 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/panedwindow.ui
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    13778 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/commands.ui
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1207 2018-07-08 00:30:31.000000 pygubu-0.9.8.6/examples/menu.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      723 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/framepad.ui
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/examples/nuitka/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    13917 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/nuitka/myapp.ui
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      140 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/nuitka/compile.bat
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     6152 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/nuitka/myapp.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       73 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/nuitka/copydatafiles.bat
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/examples/nuitka/imgs/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      131 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/nuitka/imgs/ps_triangle.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       90 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/nuitka/imgs/ps_circle.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       86 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/nuitka/imgs/ps_square.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       72 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/nuitka/imgs/MenuIcon4.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      104 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/nuitka/imgs/ps_cross.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      457 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/nuitka/nuitkahelper.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1471 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/example_grid_rc.ui
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1347 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/menuexample.ui
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2383 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/treeview.ui
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/examples/helloworld/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1608 2020-03-01 21:50:40.000000 pygubu-0.9.8.6/examples/helloworld/helloworld.ui
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      483 2020-03-01 21:50:40.000000 pygubu-0.9.8.6/examples/helloworld/helloworld.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1606 2020-03-01 21:50:40.000000 pygubu-0.9.8.6/examples/helloworld/holamundo.ui
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      482 2020-03-01 21:50:40.000000 pygubu-0.9.8.6/examples/helloworld/holamundo.py
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/examples/pyinstaller/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    13917 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/pyinstaller/myapp.ui
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1358 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/pyinstaller/myapp.spec
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     6296 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/pyinstaller/myapp.py
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/examples/pyinstaller/imgs/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      131 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/pyinstaller/imgs/ps_triangle.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       90 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/pyinstaller/imgs/ps_circle.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       86 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/pyinstaller/imgs/ps_square.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       72 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/pyinstaller/imgs/MenuIcon4.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      104 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/pyinstaller/imgs/ps_cross.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3187 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/examples/menubutton.ui
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      763 2018-07-08 00:30:31.000000 pygubu-0.9.8.6/examples/treeview.py
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/po/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     7100 2018-07-08 00:30:31.000000 pygubu-0.9.8.6/po/pygubu.pot
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      375 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/po/pygubu.mo
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4112 2020-03-01 21:50:40.000000 pygubu-0.9.8.6/setup.py
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/pygubu.egg-info/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       22 2020-03-23 21:43:52.000000 pygubu-0.9.8.6/pygubu.egg-info/top_level.txt
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    11445 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/pygubu.egg-info/SOURCES.txt
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        1 2020-03-23 21:43:52.000000 pygubu-0.9.8.6/pygubu.egg-info/dependency_links.txt
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2748 2020-03-23 21:43:52.000000 pygubu-0.9.8.6/pygubu.egg-info/PKG-INFO
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       13 2020-03-23 21:43:52.000000 pygubu-0.9.8.6/pygubu.egg-info/requires.txt
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       66 2020-03-23 21:43:52.000000 pygubu-0.9.8.6/pygubu.egg-info/entry_points.txt
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/pygubu/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1962 2020-03-23 21:41:57.000000 pygubu-0.9.8.6/pygubu/__init__.py
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/pygubu/widgets/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        0 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubu/widgets/__init__.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1019 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubu/widgets/scrollbarhelper.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4454 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubu/widgets/dialog.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4643 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubu/widgets/accordionframe.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1026 2018-07-08 00:30:32.000000 pygubu-0.9.8.6/pygubu/widgets/ttkspinbox.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     6009 2019-10-02 02:35:20.000000 pygubu-0.9.8.6/pygubu/widgets/tkscrollbarhelper.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    18429 2019-07-24 02:26:35.000000 pygubu-0.9.8.6/pygubu/widgets/calendarframe.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2989 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubu/widgets/autoarrangeframe.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    12401 2020-03-13 23:42:39.000000 pygubu-0.9.8.6/pygubu/widgets/tkscrolledframe.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1010 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubu/widgets/scrolledframe.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     7336 2019-07-24 02:26:35.000000 pygubu-0.9.8.6/pygubu/widgets/combobox.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3787 2019-07-24 02:26:35.000000 pygubu-0.9.8.6/pygubu/widgets/pathchooserinput.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1781 2019-07-24 02:26:35.000000 pygubu-0.9.8.6/pygubu/widgets/simpletooltip.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    10709 2019-10-02 02:35:20.000000 pygubu-0.9.8.6/pygubu/widgets/editabletreeview.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3394 2018-05-13 16:19:39.000000 pygubu-0.9.8.6/pygubu/binding.py
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/pygubu/builder/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    14127 2020-03-04 00:48:46.000000 pygubu-0.9.8.6/pygubu/builder/__init__.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    24059 2020-03-04 03:43:13.000000 pygubu-0.9.8.6/pygubu/builder/tkstdwidgets.py
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/pygubu/builder/widgets/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        0 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubu/builder/widgets/__init__.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      968 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubu/builder/widgets/scrollbarhelper.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1391 2020-03-23 01:17:38.000000 pygubu-0.9.8.6/pygubu/builder/widgets/dialog.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1144 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubu/builder/widgets/tkscrollbarhelper.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2075 2019-07-24 02:26:35.000000 pygubu-0.9.8.6/pygubu/builder/widgets/calendarframe.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1543 2018-07-08 00:30:32.000000 pygubu-0.9.8.6/pygubu/builder/widgets/tkscrolledframe.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1389 2018-07-08 00:30:32.000000 pygubu-0.9.8.6/pygubu/builder/widgets/scrolledframe.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1049 2019-07-24 02:26:35.000000 pygubu-0.9.8.6/pygubu/builder/widgets/combobox.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1159 2019-07-24 02:26:35.000000 pygubu-0.9.8.6/pygubu/builder/widgets/pathchooserinput.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      859 2018-07-08 00:30:32.000000 pygubu-0.9.8.6/pygubu/builder/widgets/editabletreeview.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    14564 2019-07-23 05:40:39.000000 pygubu-0.9.8.6/pygubu/builder/ttkstdwidgets.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     9967 2020-03-04 00:48:46.000000 pygubu-0.9.8.6/pygubu/builder/builderobject.py
+-rwxrwxr-x   0 alejandro  (1000) alejandro  (1000)     4560 2018-07-08 00:30:32.000000 pygubu-0.9.8.6/pygubu/ui2code.py
+-rwxrwxr-x   0 alejandro  (1000) alejandro  (1000)     2722 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubu/testui.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     6624 2019-11-03 04:12:09.000000 pygubu-0.9.8.6/pygubu/stockimage.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     5993 2020-03-01 21:50:40.000000 pygubu-0.9.8.6/README.md
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      146 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/MANIFEST.in
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       38 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/setup.cfg
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/pygubudesigner/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1450 2018-07-08 00:30:32.000000 pygubu-0.9.8.6/pygubudesigner/__init__.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     9000 2020-03-04 00:48:46.000000 pygubu-0.9.8.6/pygubudesigner/layouteditor.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3905 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/widgetdescr.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    21327 2020-03-04 03:00:30.000000 pygubu-0.9.8.6/pygubudesigner/previewer.py
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/pygubudesigner/widgets/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      575 2018-07-08 00:30:32.000000 pygubu-0.9.8.6/pygubudesigner/widgets/__init__.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2310 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/widgets/tkvarentry.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4590 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/widgets/sizeentry.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2312 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/widgets/dimensionentry.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     8296 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/widgets/fontentry.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2617 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/widgets/whentry.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     5387 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/widgets/stickyentry.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     8799 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/widgets/propertyeditor.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2738 2019-11-03 04:12:09.000000 pygubu-0.9.8.6/pygubudesigner/widgets/imageentry.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4631 2020-03-04 02:25:51.000000 pygubu-0.9.8.6/pygubudesigner/widgets/toplevelframe.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2278 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/widgets/dynamicpropeditor.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3411 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/widgets/colorentry.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    22792 2020-03-04 03:30:20.000000 pygubu-0.9.8.6/pygubudesigner/main.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    27488 2020-03-04 03:36:26.000000 pygubu-0.9.8.6/pygubudesigner/uitreeeditor.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3816 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/bindingseditor.py
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/pygubudesigner/ui/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    40338 2019-07-24 02:26:35.000000 pygubu-0.9.8.6/pygubudesigner/ui/pygubu-ui.ui
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    14277 2018-07-08 00:30:32.000000 pygubu-0.9.8.6/pygubudesigner/ui/preferences_dialog.ui
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4414 2018-07-08 00:26:59.000000 pygubu-0.9.8.6/pygubudesigner/ui/about_dialog.ui
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1646 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/widgeteditor.py
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/pygubudesigner/util/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3471 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/util/__init__.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1270 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/util/observable.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3033 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/util/selecttool.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1574 2018-07-08 00:30:32.000000 pygubu-0.9.8.6/pygubudesigner/i18n.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     5794 2019-07-23 04:22:51.000000 pygubu-0.9.8.6/pygubudesigner/propertieseditor.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      122 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/__main__.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)    27083 2019-07-23 02:46:24.000000 pygubu-0.9.8.6/pygubudesigner/properties.py
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/pygubudesigner/locale/
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/pygubudesigner/locale/de/
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/pygubudesigner/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     8797 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/locale/de/LC_MESSAGES/pygubu.po
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     5210 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/locale/de/LC_MESSAGES/pygubu.mo
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/pygubudesigner/locale/es/
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/pygubudesigner/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     8669 2018-07-08 00:30:32.000000 pygubu-0.9.8.6/pygubudesigner/locale/es/LC_MESSAGES/pygubu.po
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     5001 2018-07-08 00:30:32.000000 pygubu-0.9.8.6/pygubudesigner/locale/es/LC_MESSAGES/pygubu.mo
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/pygubudesigner/images/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       70 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/indicator_ne.gif
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      111 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Scale.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      124 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/ttk.Radiobutton.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      124 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Radiobutton.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      124 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/ttk.Frame.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      599 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Canvas.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      108 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.PanedWindow.Pane.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       96 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/ttk.Entry.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      130 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Listbox.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      139 2018-07-08 00:30:32.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/pygubu.builder.widgets.calendarframe.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      118 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/ttk.Checkbutton.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      197 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/pygubu.builder.widgets.scrolledframe.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      108 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/ttk.Panedwindow.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      125 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Toplevel.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      108 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Menuitem.Command.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      121 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Scrollbar.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      155 2018-07-08 00:30:32.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/pygubu.builder.widgets.combobox.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      111 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/ttk.Scale.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      114 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Text.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      140 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Menubutton.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      130 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/ttk.Treeview.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      125 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/pygubu.builder.widgets.dialog.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      156 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Menuitem.Checkbutton.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      139 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Calendar.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      156 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/ttk.Treeview.Column.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      140 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/ttk.Menubutton.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      108 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Menuitem.Separator.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      197 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/pygubu.builder.widgets.tkscrolledframe.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       89 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Message.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       89 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/ttk.Separator.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      124 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Frame.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      195 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Menuitem.Radiobutton.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      108 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/ttk.Panedwindow.Pane.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      105 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/ttk.Label.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      138 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Button.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      153 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/pygubu.builder.widgets.tkscrollbarhelper.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      139 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Menu.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      155 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/ttk.Combobox.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       96 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.default.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      129 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/ttk.Labelframe.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      108 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.PanedWindow.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      131 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/ttk.Notebook.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      133 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/ttk.Spinbox.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      121 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/ttk.Scrollbar.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       96 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Entry.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      153 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/pygubu.builder.widgets.scrollbarhelper.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      118 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Checkbutton.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       96 2018-07-08 00:30:32.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/pygubu.builder.widgets.pathchooserinput.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      132 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/pygubu.builder.widgets.Labelwidget.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      138 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/ttk.Button.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      125 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/ttk.Progressbar.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      129 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.LabelFrame.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      153 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/ttk.Sizegrip.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      133 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Spinbox.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      139 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Menuitem.Submenu.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      142 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/ttk.Notebook.Tab.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      130 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/pygubu.builder.widgets.editabletreeview.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      105 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Label.gif
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/fontentry/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      567 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/fontentry/format-text-italic.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      357 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/fontentry/format-text-strikethrough.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      592 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/fontentry/format-text-bold.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      572 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/fontentry/format-text-underline.gif
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/propertyeditor/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      377 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/propertyeditor/property_invalid.gif
+drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Scale.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Radiobutton.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Radiobutton.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Frame.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Canvas.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.PanedWindow.Pane.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Entry.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Listbox.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      352 2018-07-08 00:30:32.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.calendarframe.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Checkbutton.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.scrolledframe.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Panedwindow.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Toplevel.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Menuitem.Command.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Scrollbar.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Scale.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Text.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Menubutton.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Treeview.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.dialog.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Menuitem.Checkbutton.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Calendar.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      109 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Treeview.Column.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Menubutton.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Menuitem.Separator.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       75 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Message.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Separator.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Frame.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Menuitem.Radiobutton.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Panedwindow.Pane.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Label.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Button.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Menu.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1120 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Combobox.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.default.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      126 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Labelframe.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.PanedWindow.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Notebook.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Spinbox.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Scrollbar.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Entry.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Checkbutton.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      128 2018-07-08 00:30:32.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.pathchooserinput.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      107 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.Labelwidget.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Button.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Progressbar.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      105 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.LabelFrame.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      105 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Sizegrip.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Spinbox.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Menuitem.Submenu.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      100 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Notebook.Tab.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.editabletreeview.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1095 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Label.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       74 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/mglass.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      875 2018-07-08 00:26:59.000000 pygubu-0.9.8.6/pygubudesigner/images/pygubu.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       61 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/close.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       69 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/indicator_nw.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4897 2018-07-08 00:26:59.000000 pygubu-0.9.8.6/pygubudesigner/images/pygubu200.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       70 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/indicator_sw.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       69 2018-01-17 20:34:39.000000 pygubu-0.9.8.6/pygubudesigner/images/indicator_se.gif
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4722 2019-07-24 02:26:35.000000 pygubu-0.9.8.6/pygubudesigner/preferences.py
+-rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2748 2020-03-23 21:43:53.000000 pygubu-0.9.8.6/PKG-INFO
```

### Comparing `pygubu-0.9.8.5/COPYING` & `pygubu-0.9.8.6/COPYING`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/commands.py` & `pygubu-0.9.8.6/examples/commands.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/canvas_example.ui` & `pygubu-0.9.8.6/examples/canvas_example.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/binding.ui` & `pygubu-0.9.8.6/examples/binding.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/button_cb.py` & `pygubu-0.9.8.6/examples/button_cb.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/panes_and_notebooks.ui` & `pygubu-0.9.8.6/examples/panes_and_notebooks.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/cx_freeze/myapp.ui` & `pygubu-0.9.8.6/examples/cx_freeze/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/cx_freeze/setup.py` & `pygubu-0.9.8.6/examples/cx_freeze/setup.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/cx_freeze/myapp.py` & `pygubu-0.9.8.6/examples/cx_freeze/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/example_grid_rc_2.ui` & `pygubu-0.9.8.6/examples/example_grid_rc_2.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/vscrolledframe.ui` & `pygubu-0.9.8.6/examples/vscrolledframe.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/scrollbarhelper.ui` & `pygubu-0.9.8.6/examples/scrollbarhelper.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/menu.ui` & `pygubu-0.9.8.6/examples/menu.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/variables.ui` & `pygubu-0.9.8.6/examples/variables.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/button_cb.ui` & `pygubu-0.9.8.6/examples/button_cb.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/py2exe/myapp.ui` & `pygubu-0.9.8.6/examples/py2exe/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/py2exe/setup.py` & `pygubu-0.9.8.6/examples/py2exe/setup.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/py2exe/myapp.py` & `pygubu-0.9.8.6/examples/py2exe/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/scrolledframe.ui` & `pygubu-0.9.8.6/examples/scrolledframe.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/panedwindow.ui` & `pygubu-0.9.8.6/examples/panedwindow.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/commands.ui` & `pygubu-0.9.8.6/examples/commands.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/menu.py` & `pygubu-0.9.8.6/examples/menu.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/framepad.ui` & `pygubu-0.9.8.6/examples/framepad.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/nuitka/myapp.ui` & `pygubu-0.9.8.6/examples/nuitka/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/nuitka/myapp.py` & `pygubu-0.9.8.6/examples/nuitka/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/example_grid_rc.ui` & `pygubu-0.9.8.6/examples/example_grid_rc.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/menuexample.ui` & `pygubu-0.9.8.6/examples/menuexample.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/treeview.ui` & `pygubu-0.9.8.6/examples/treeview.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/helloworld/helloworld.ui` & `pygubu-0.9.8.6/examples/helloworld/helloworld.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/helloworld/holamundo.ui` & `pygubu-0.9.8.6/examples/helloworld/holamundo.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/pyinstaller/myapp.ui` & `pygubu-0.9.8.6/examples/pyinstaller/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/pyinstaller/myapp.spec` & `pygubu-0.9.8.6/examples/pyinstaller/myapp.spec`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/pyinstaller/myapp.py` & `pygubu-0.9.8.6/examples/pyinstaller/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/menubutton.ui` & `pygubu-0.9.8.6/examples/menubutton.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/examples/treeview.py` & `pygubu-0.9.8.6/examples/treeview.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/po/pygubu.pot` & `pygubu-0.9.8.6/po/pygubu.pot`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/setup.py` & `pygubu-0.9.8.6/setup.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu.egg-info/SOURCES.txt` & `pygubu-0.9.8.6/pygubu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu.egg-info/PKG-INFO` & `pygubu-0.9.8.6/pygubu.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pygubu
-Version: 0.9.8.5
+Version: 0.9.8.6
 Summary: A tkinter GUI builder.
 Home-page: https://github.com/alejandroautalan/pygubu
 Author: Alejandro Autalán
 Author-email: alejandroautalan@gmail.com
 License: GPL-3
 Description: 
         Welcome to pygubu a GUI designer for tkinter
```

### Comparing `pygubu-0.9.8.5/pygubu/__init__.py` & `pygubu-0.9.8.6/pygubu/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import pygubu.builder.builderobject
 from pygubu.builder import Builder
 from pygubu.builder.builderobject import BuilderObject, register_widget
 from pygubu.binding import remove_binding, ApplicationLevelBindManager
 
 
-__version__ = '0.9.8.5'
+__version__ = '0.9.8.6'
 
 
 def register_property(name, description):
     return pygubu.builder.builderobject.register_property(name, description)
```

### Comparing `pygubu-0.9.8.5/pygubu/widgets/scrollbarhelper.py` & `pygubu-0.9.8.6/pygubu/widgets/scrollbarhelper.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/widgets/dialog.py` & `pygubu-0.9.8.6/pygubu/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/widgets/accordionframe.py` & `pygubu-0.9.8.6/pygubu/widgets/accordionframe.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/widgets/ttkspinbox.py` & `pygubu-0.9.8.6/pygubu/widgets/ttkspinbox.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/widgets/tkscrollbarhelper.py` & `pygubu-0.9.8.6/pygubu/widgets/tkscrollbarhelper.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/widgets/calendarframe.py` & `pygubu-0.9.8.6/pygubu/widgets/calendarframe.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/widgets/autoarrangeframe.py` & `pygubu-0.9.8.6/pygubu/widgets/autoarrangeframe.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/widgets/tkscrolledframe.py` & `pygubu-0.9.8.6/pygubu/widgets/tkscrolledframe.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/widgets/scrolledframe.py` & `pygubu-0.9.8.6/pygubu/widgets/scrolledframe.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/widgets/combobox.py` & `pygubu-0.9.8.6/pygubu/widgets/combobox.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/widgets/pathchooserinput.py` & `pygubu-0.9.8.6/pygubu/widgets/pathchooserinput.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/widgets/simpletooltip.py` & `pygubu-0.9.8.6/pygubu/widgets/simpletooltip.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/widgets/editabletreeview.py` & `pygubu-0.9.8.6/pygubu/widgets/editabletreeview.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/binding.py` & `pygubu-0.9.8.6/pygubu/binding.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/builder/__init__.py` & `pygubu-0.9.8.6/pygubu/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/builder/tkstdwidgets.py` & `pygubu-0.9.8.6/pygubu/builder/tkstdwidgets.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/builder/widgets/scrollbarhelper.py` & `pygubu-0.9.8.6/pygubu/builder/widgets/scrollbarhelper.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/builder/widgets/dialog.py` & `pygubu-0.9.8.6/pygubu/builder/widgets/dialog.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,18 @@
     OPTIONS_STANDARD = TKToplevel.OPTIONS_STANDARD
     OPTIONS_SPECIFIC = TKToplevel.OPTIONS_SPECIFIC
     OPTIONS_CUSTOM = \
         TKToplevel.OPTIONS_CUSTOM + ('modal',)
     properties = OPTIONS_STANDARD + OPTIONS_SPECIFIC + OPTIONS_CUSTOM
 
     def realize(self, parent):
-        BuilderObject.realize(self, parent)
+        super(TKToplevel, self).realize(parent)
+    
+    def layout(self, target=None):
+        super(DialogBO, self).layout(self.widget.toplevel)
 
     def _set_property(self, target_widget, pname, value):
         if pname == 'modal':
             modal = False
             value = value.lower()
             if value == 'true':
                 modal = True
```

### Comparing `pygubu-0.9.8.5/pygubu/builder/widgets/tkscrollbarhelper.py` & `pygubu-0.9.8.6/pygubu/builder/widgets/tkscrollbarhelper.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/builder/widgets/calendarframe.py` & `pygubu-0.9.8.6/pygubu/builder/widgets/calendarframe.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/builder/widgets/tkscrolledframe.py` & `pygubu-0.9.8.6/pygubu/builder/widgets/tkscrolledframe.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/builder/widgets/scrolledframe.py` & `pygubu-0.9.8.6/pygubu/builder/widgets/scrolledframe.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/builder/widgets/combobox.py` & `pygubu-0.9.8.6/pygubu/builder/widgets/combobox.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/builder/widgets/pathchooserinput.py` & `pygubu-0.9.8.6/pygubu/builder/widgets/pathchooserinput.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/builder/widgets/editabletreeview.py` & `pygubu-0.9.8.6/pygubu/builder/widgets/editabletreeview.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/builder/ttkstdwidgets.py` & `pygubu-0.9.8.6/pygubu/builder/ttkstdwidgets.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/builder/builderobject.py` & `pygubu-0.9.8.6/pygubu/builder/builderobject.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/ui2code.py` & `pygubu-0.9.8.6/pygubu/ui2code.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/testui.py` & `pygubu-0.9.8.6/pygubu/testui.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubu/stockimage.py` & `pygubu-0.9.8.6/pygubu/stockimage.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/README.md` & `pygubu-0.9.8.6/README.md`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/__init__.py` & `pygubu-0.9.8.6/pygubudesigner/__init__.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/layouteditor.py` & `pygubu-0.9.8.6/pygubudesigner/layouteditor.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/widgetdescr.py` & `pygubu-0.9.8.6/pygubudesigner/widgetdescr.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/previewer.py` & `pygubu-0.9.8.6/pygubudesigner/previewer.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/widgets/__init__.py` & `pygubu-0.9.8.6/pygubudesigner/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/widgets/tkvarentry.py` & `pygubu-0.9.8.6/pygubudesigner/widgets/tkvarentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/widgets/sizeentry.py` & `pygubu-0.9.8.6/pygubudesigner/widgets/sizeentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/widgets/dimensionentry.py` & `pygubu-0.9.8.6/pygubudesigner/widgets/dimensionentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/widgets/fontentry.py` & `pygubu-0.9.8.6/pygubudesigner/widgets/fontentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/widgets/whentry.py` & `pygubu-0.9.8.6/pygubudesigner/widgets/whentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/widgets/stickyentry.py` & `pygubu-0.9.8.6/pygubudesigner/widgets/stickyentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/widgets/propertyeditor.py` & `pygubu-0.9.8.6/pygubudesigner/widgets/propertyeditor.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/widgets/imageentry.py` & `pygubu-0.9.8.6/pygubudesigner/widgets/imageentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/widgets/toplevelframe.py` & `pygubu-0.9.8.6/pygubudesigner/widgets/toplevelframe.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/widgets/dynamicpropeditor.py` & `pygubu-0.9.8.6/pygubudesigner/widgets/dynamicpropeditor.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/widgets/colorentry.py` & `pygubu-0.9.8.6/pygubudesigner/widgets/colorentry.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/main.py` & `pygubu-0.9.8.6/pygubudesigner/main.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/uitreeeditor.py` & `pygubu-0.9.8.6/pygubudesigner/uitreeeditor.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/bindingseditor.py` & `pygubu-0.9.8.6/pygubudesigner/bindingseditor.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/ui/pygubu-ui.ui` & `pygubu-0.9.8.6/pygubudesigner/ui/pygubu-ui.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/ui/preferences_dialog.ui` & `pygubu-0.9.8.6/pygubudesigner/ui/preferences_dialog.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/ui/about_dialog.ui` & `pygubu-0.9.8.6/pygubudesigner/ui/about_dialog.ui`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/widgeteditor.py` & `pygubu-0.9.8.6/pygubudesigner/widgeteditor.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/util/__init__.py` & `pygubu-0.9.8.6/pygubudesigner/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/util/observable.py` & `pygubu-0.9.8.6/pygubudesigner/util/observable.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/util/selecttool.py` & `pygubu-0.9.8.6/pygubudesigner/util/selecttool.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/i18n.py` & `pygubu-0.9.8.6/pygubudesigner/i18n.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/propertieseditor.py` & `pygubu-0.9.8.6/pygubudesigner/propertieseditor.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/properties.py` & `pygubu-0.9.8.6/pygubudesigner/properties.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/locale/de/LC_MESSAGES/pygubu.po` & `pygubu-0.9.8.6/pygubudesigner/locale/de/LC_MESSAGES/pygubu.po`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/locale/de/LC_MESSAGES/pygubu.mo` & `pygubu-0.9.8.6/pygubudesigner/locale/de/LC_MESSAGES/pygubu.mo`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/locale/es/LC_MESSAGES/pygubu.po` & `pygubu-0.9.8.6/pygubudesigner/locale/es/LC_MESSAGES/pygubu.po`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/locale/es/LC_MESSAGES/pygubu.mo` & `pygubu-0.9.8.6/pygubudesigner/locale/es/LC_MESSAGES/pygubu.mo`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/22x22/tk.Canvas.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/22x22/tk.Canvas.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/fontentry/format-text-italic.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/fontentry/format-text-italic.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/fontentry/format-text-bold.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/fontentry/format-text-bold.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/fontentry/format-text-underline.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/fontentry/format-text-underline.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Scale.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Scale.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Radiobutton.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Radiobutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Radiobutton.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Radiobutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Frame.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Frame.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Canvas.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Canvas.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.PanedWindow.Pane.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.PanedWindow.Pane.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Entry.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Entry.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Listbox.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Listbox.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Checkbutton.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Checkbutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.scrolledframe.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.scrolledframe.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Panedwindow.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Panedwindow.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Toplevel.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Toplevel.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Menuitem.Command.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Menuitem.Command.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Scrollbar.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Scrollbar.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Scale.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Scale.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Text.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Text.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Menubutton.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Menubutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Treeview.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Treeview.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.dialog.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.dialog.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Menuitem.Checkbutton.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Menuitem.Checkbutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Calendar.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Calendar.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Menubutton.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Menubutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Menuitem.Separator.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Menuitem.Separator.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Separator.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Separator.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Frame.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Frame.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Menuitem.Radiobutton.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Menuitem.Radiobutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Panedwindow.Pane.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Panedwindow.Pane.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Label.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Label.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Button.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Button.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Menu.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Menu.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Combobox.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Combobox.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.default.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.default.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.PanedWindow.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.PanedWindow.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Notebook.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Notebook.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Spinbox.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Spinbox.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Scrollbar.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Scrollbar.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Entry.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Entry.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Checkbutton.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Checkbutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Button.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Button.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/ttk.Progressbar.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/ttk.Progressbar.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Spinbox.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Spinbox.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Menuitem.Submenu.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Menuitem.Submenu.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.editabletreeview.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/pygubu.builder.widgets.editabletreeview.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/widgets/16x16/tk.Label.gif` & `pygubu-0.9.8.6/pygubudesigner/images/widgets/16x16/tk.Label.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/pygubu.gif` & `pygubu-0.9.8.6/pygubudesigner/images/pygubu.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/images/pygubu200.gif` & `pygubu-0.9.8.6/pygubudesigner/images/pygubu200.gif`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/pygubudesigner/preferences.py` & `pygubu-0.9.8.6/pygubudesigner/preferences.py`

 * *Files identical despite different names*

### Comparing `pygubu-0.9.8.5/PKG-INFO` & `pygubu-0.9.8.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pygubu
-Version: 0.9.8.5
+Version: 0.9.8.6
 Summary: A tkinter GUI builder.
 Home-page: https://github.com/alejandroautalan/pygubu
 Author: Alejandro Autalán
 Author-email: alejandroautalan@gmail.com
 License: GPL-3
 Description: 
         Welcome to pygubu a GUI designer for tkinter
```

