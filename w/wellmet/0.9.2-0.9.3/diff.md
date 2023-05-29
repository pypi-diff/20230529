# Comparing `tmp/wellmet-0.9.2.tar.gz` & `tmp/wellmet-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wellmet-0.9.2.tar", last modified: Sun May 28 15:35:38 2023, max compression
+gzip compressed data, was "wellmet-0.9.3.tar", last modified: Mon May 29 17:30:15 2023, max compression
```

## Comparing `wellmet-0.9.2.tar` & `wellmet-0.9.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-28 15:35:38.465829 wellmet-0.9.2/
--rw-r--r--   0 user         (0) root         (0)     1093 2022-04-30 17:02:31.028049 wellmet-0.9.2/LICENSE
--rw-r--r--   0 user         (0) root         (0)      753 2023-05-28 15:35:38.460324 wellmet-0.9.2/PKG-INFO
--rw-r--r--   0 user         (0) root         (0)     2355 2023-05-28 15:29:58.028049 wellmet-0.9.2/README.md
--rw-r--r--   0 user         (0) root         (0)      892 2023-05-28 15:35:13.028311 wellmet-0.9.2/pyproject.toml
--rw-r--r--   0 user         (0) root         (0)       38 2023-05-28 15:35:38.466092 wellmet-0.9.2/setup.cfg
--rw-r--r--   0 user         (0) root         (0)     1208 2023-05-28 15:35:07.028311 wellmet-0.9.2/setup.py
-drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-28 15:35:38.228327 wellmet-0.9.2/wellmet/
--rw-r--r--   0 user         (0) root         (0)    30048 2023-05-28 14:15:30.028311 wellmet-0.9.2/wellmet/IS_stat.py
--rw-r--r--   0 user         (0) root         (0)       86 2023-05-28 15:34:51.028573 wellmet-0.9.2/wellmet/__init__.py
--rw-r--r--   0 user         (0) root         (0)       72 2022-04-30 16:53:41.028573 wellmet-0.9.2/wellmet/__main__.py
--rw-r--r--   0 user         (0) root         (0)    11243 2023-05-28 14:15:30.028573 wellmet-0.9.2/wellmet/candybox.py
--rw-r--r--   0 user         (0) root         (0)     6756 2023-05-28 14:15:30.028835 wellmet-0.9.2/wellmet/candynodes.py
--rw-r--r--   0 user         (0) root         (0)    50875 2023-02-09 22:14:32.028835 wellmet-0.9.2/wellmet/convex_hull.py
-drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-28 15:35:38.299106 wellmet-0.9.2/wellmet/dicebox/
--rw-r--r--   0 user         (0) root         (0)    14745 2023-01-15 11:46:20.030671 wellmet-0.9.2/wellmet/dicebox/__circumtri.py
--rw-r--r--   0 user         (0) root         (0)        6 2022-04-30 16:53:41.030933 wellmet-0.9.2/wellmet/dicebox/__init__.py
--rw-r--r--   0 user         (0) root         (0)    17010 2023-01-15 11:46:40.030933 wellmet-0.9.2/wellmet/dicebox/_circumtri.py
--rw-r--r--   0 user         (0) root         (0)     7865 2023-02-01 00:06:26.030933 wellmet-0.9.2/wellmet/dicebox/_exploration.py
--rw-r--r--   0 user         (0) root         (0)    73380 2023-01-15 11:48:48.031195 wellmet-0.9.2/wellmet/dicebox/censoring.py
--rw-r--r--   0 user         (0) root         (0)    33598 2023-02-11 03:48:27.031195 wellmet-0.9.2/wellmet/dicebox/circumtri.py
--rw-r--r--   0 user         (0) root         (0)   100174 2023-01-15 11:50:00.031195 wellmet-0.9.2/wellmet/dicebox/goal.py
--rw-r--r--   0 user         (0) root         (0)    36893 2023-01-15 11:50:38.028835 wellmet-0.9.2/wellmet/estimation.py
--rw-r--r--   0 user         (0) root         (0)    52580 2023-01-15 11:51:29.029098 wellmet-0.9.2/wellmet/f_models.py
--rw-r--r--   0 user         (0) root         (0)    42237 2023-03-12 14:45:57.029098 wellmet-0.9.2/wellmet/g_models.py
--rw-r--r--   0 user         (0) root         (0)    21042 2023-05-28 14:15:30.029098 wellmet-0.9.2/wellmet/ghull.py
--rw-r--r--   0 user         (0) root         (0)     3234 2022-05-13 19:15:46.029098 wellmet-0.9.2/wellmet/misc.py
-drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-28 15:35:38.358088 wellmet-0.9.2/wellmet/mplot/
--rw-r--r--   0 user         (0) root         (0)     1407 2022-04-30 16:53:41.031457 wellmet-0.9.2/wellmet/mplot/__init__.py
--rw-r--r--   0 user         (0) root         (0)     9741 2022-04-30 16:53:41.031457 wellmet-0.9.2/wellmet/mplot/_axes3d.py
--rw-r--r--   0 user         (0) root         (0)      714 2022-04-30 16:53:41.031457 wellmet-0.9.2/wellmet/mplot/_axis3d_margins_patch.py
--rw-r--r--   0 user         (0) root         (0)    23492 2023-03-30 13:18:09.031457 wellmet-0.9.2/wellmet/mplot/mart.py
--rw-r--r--   0 user         (0) root         (0)    13647 2023-01-15 11:54:22.031719 wellmet-0.9.2/wellmet/mplot/mart3d.py
--rw-r--r--   0 user         (0) root         (0)    26324 2023-03-15 21:00:41.031719 wellmet-0.9.2/wellmet/mplot/maxes.py
--rw-r--r--   0 user         (0) root         (0)     5577 2022-04-30 16:53:41.031719 wellmet-0.9.2/wellmet/mplot/maxes3d.py
--rw-r--r--   0 user         (0) root         (0)    17778 2023-03-16 03:04:56.031981 wellmet-0.9.2/wellmet/mplot/mfigs.py
--rw-r--r--   0 user         (0) root         (0)    10463 2023-02-02 13:58:18.031981 wellmet-0.9.2/wellmet/mplot/mgraph.py
--rw-r--r--   0 user         (0) root         (0)     1132 2022-04-30 16:53:41.031981 wellmet-0.9.2/wellmet/mplot/misc.py
-drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-28 15:35:38.423362 wellmet-0.9.2/wellmet/qt_gui/
--rw-r--r--   0 user         (0) root         (0)        6 2022-04-30 16:53:41.032243 wellmet-0.9.2/wellmet/qt_gui/__init__.py
--rw-r--r--   0 user         (0) root         (0)    44438 2023-01-15 11:54:47.032243 wellmet-0.9.2/wellmet/qt_gui/gl_plot.py
--rw-r--r--   0 user         (0) root         (0)      348 2022-10-16 03:13:28.032243 wellmet-0.9.2/wellmet/qt_gui/gui_startup.py
--rw-r--r--   0 user         (0) root         (0)     1970 2022-10-07 12:30:43.032505 wellmet-0.9.2/wellmet/qt_gui/qt_box_functions.py
--rw-r--r--   0 user         (0) root         (0)    26239 2023-05-28 15:18:02.032505 wellmet-0.9.2/wellmet/qt_gui/qt_dicebox.py
--rw-r--r--   0 user         (0) root         (0)    35342 2023-01-17 14:19:12.032505 wellmet-0.9.2/wellmet/qt_gui/qt_graph_widgets.py
--rw-r--r--   0 user         (0) root         (0)    24326 2023-05-28 14:20:54.032768 wellmet-0.9.2/wellmet/qt_gui/qt_gui.py
--rw-r--r--   0 user         (0) root         (0)    38391 2022-12-21 15:13:48.032768 wellmet-0.9.2/wellmet/qt_gui/qt_pairwise.py
--rw-r--r--   0 user         (0) root         (0)    99810 2023-05-28 14:19:00.032768 wellmet-0.9.2/wellmet/qt_gui/qt_plot.py
--rw-r--r--   0 user         (0) root         (0)     3244 2023-01-10 05:21:15.033030 wellmet-0.9.2/wellmet/qt_gui/qt_testcases.py
--rw-r--r--   0 user         (0) root         (0)    56858 2022-11-29 15:50:00.033030 wellmet-0.9.2/wellmet/qt_gui/qt_voronoi.py
--rw-r--r--   0 user         (0) root         (0)    10956 2023-01-15 11:55:28.029360 wellmet-0.9.2/wellmet/reader.py
--rw-r--r--   0 user         (0) root         (0)     4416 2023-01-15 11:56:01.029360 wellmet-0.9.2/wellmet/samplebox.py
--rw-r--r--   0 user         (0) root         (0)     6558 2022-04-30 16:53:42.029360 wellmet-0.9.2/wellmet/sball.py
--rw-r--r--   0 user         (0) root         (0)     6739 2022-04-30 16:53:42.029622 wellmet-0.9.2/wellmet/schemes.py
--rw-r--r--   0 user         (0) root         (0)     8309 2023-05-28 14:15:30.029622 wellmet-0.9.2/wellmet/shell.py
--rw-r--r--   0 user         (0) root         (0)   134283 2023-03-16 18:30:34.029622 wellmet-0.9.2/wellmet/simplex.py
--rw-r--r--   0 user         (0) root         (0)    13090 2023-05-28 14:15:30.029884 wellmet-0.9.2/wellmet/spring.py
--rw-r--r--   0 user         (0) root         (0)    10953 2022-04-30 16:53:42.029884 wellmet-0.9.2/wellmet/stm_df.py
-drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-28 15:35:38.454033 wellmet-0.9.2/wellmet/testcases/
--rw-r--r--   0 user         (0) root         (0)        0 2023-05-28 13:48:40.033030 wellmet-0.9.2/wellmet/testcases/__init__.py
--rw-r--r--   0 user         (0) root         (0)     8987 2023-03-12 15:00:08.033030 wellmet-0.9.2/wellmet/testcases/gaussian_2D.py
--rw-r--r--   0 user         (0) root         (0)     8183 2023-05-28 14:14:11.033292 wellmet-0.9.2/wellmet/testcases/testcases_2D.py
--rw-r--r--   0 user         (0) root         (0)     3741 2023-02-24 08:01:44.033292 wellmet-0.9.2/wellmet/testcases/testcases_2D_papers.py
--rw-r--r--   0 user         (0) root         (0)     2572 2023-01-14 08:20:10.033292 wellmet-0.9.2/wellmet/testcases/testcases_nD.py
--rw-r--r--   0 user         (0) root         (0)    11998 2023-01-30 12:29:31.033554 wellmet-0.9.2/wellmet/testcases/testcases_nD_papers.py
--rw-r--r--   0 user         (0) root         (0)    47956 2023-01-15 11:58:08.029884 wellmet-0.9.2/wellmet/voronoi.py
--rw-r--r--   0 user         (0) root         (0)     2465 2023-05-28 14:15:30.030146 wellmet-0.9.2/wellmet/welford.py
--rw-r--r--   0 user         (0) root         (0)    32101 2023-03-15 04:11:34.030146 wellmet-0.9.2/wellmet/whitebox.py
--rw-r--r--   0 user         (0) root         (0)    26468 2023-05-28 14:15:30.030146 wellmet-0.9.2/wellmet/wireframe.py
-drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-28 15:35:38.257687 wellmet-0.9.2/wellmet.egg-info/
--rw-r--r--   0 user         (0) root         (0)      753 2023-05-28 15:35:37.030408 wellmet-0.9.2/wellmet.egg-info/PKG-INFO
--rw-r--r--   0 user         (0) root         (0)     1632 2023-05-28 15:35:38.030408 wellmet-0.9.2/wellmet.egg-info/SOURCES.txt
--rw-r--r--   0 user         (0) root         (0)        1 2023-05-28 15:35:37.030408 wellmet-0.9.2/wellmet.egg-info/dependency_links.txt
--rw-r--r--   0 user         (0) root         (0)       57 2023-05-28 15:35:37.030671 wellmet-0.9.2/wellmet.egg-info/requires.txt
--rw-r--r--   0 user         (0) root         (0)        8 2023-05-28 15:35:37.030671 wellmet-0.9.2/wellmet.egg-info/top_level.txt
+drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-29 17:30:15.209977 wellmet-0.9.3/
+-rw-r--r--   0 user         (0) root         (0)     1093 2022-04-30 17:02:31.029360 wellmet-0.9.3/LICENSE
+-rw-r--r--   0 user         (0) root         (0)     5050 2023-05-29 17:30:15.210501 wellmet-0.9.3/PKG-INFO
+-rw-r--r--   0 user         (0) root         (0)     4380 2023-05-29 17:30:06.029622 wellmet-0.9.3/README.md
+-rw-r--r--   0 user         (0) root         (0)      899 2023-05-29 13:26:34.029622 wellmet-0.9.3/pyproject.toml
+-rw-r--r--   0 user         (0) root         (0)      794 2023-05-29 17:30:15.219152 wellmet-0.9.3/setup.cfg
+-rw-r--r--   0 user         (0) root         (0)       54 2023-05-29 15:46:17.029622 wellmet-0.9.3/setup.py
+drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-29 17:30:14.932184 wellmet-0.9.3/wellmet/
+-rw-r--r--   0 user         (0) root         (0)    30048 2023-05-28 14:15:30.029884 wellmet-0.9.3/wellmet/IS_stat.py
+-rw-r--r--   0 user         (0) root         (0)       86 2023-05-28 15:34:51.029884 wellmet-0.9.3/wellmet/__init__.py
+-rw-r--r--   0 user         (0) root         (0)       72 2022-04-30 16:53:41.029884 wellmet-0.9.3/wellmet/__main__.py
+-rw-r--r--   0 user         (0) root         (0)    11243 2023-05-28 14:15:30.030146 wellmet-0.9.3/wellmet/candybox.py
+-rw-r--r--   0 user         (0) root         (0)     6756 2023-05-28 14:15:30.030146 wellmet-0.9.3/wellmet/candynodes.py
+-rw-r--r--   0 user         (0) root         (0)    50875 2023-05-29 17:12:11.030146 wellmet-0.9.3/wellmet/convex_hull.py
+drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-29 17:30:15.015728 wellmet-0.9.3/wellmet/dicebox/
+-rw-r--r--   0 user         (0) root         (0)    14745 2023-05-29 17:12:04.032243 wellmet-0.9.3/wellmet/dicebox/__circumtri.py
+-rw-r--r--   0 user         (0) root         (0)        6 2022-04-30 16:53:41.032243 wellmet-0.9.3/wellmet/dicebox/__init__.py
+-rw-r--r--   0 user         (0) root         (0)    17010 2023-05-29 17:12:04.032243 wellmet-0.9.3/wellmet/dicebox/_circumtri.py
+-rw-r--r--   0 user         (0) root         (0)     7865 2023-05-29 17:12:04.032505 wellmet-0.9.3/wellmet/dicebox/_exploration.py
+-rw-r--r--   0 user         (0) root         (0)    73380 2023-01-15 11:48:48.032505 wellmet-0.9.3/wellmet/dicebox/censoring.py
+-rw-r--r--   0 user         (0) root         (0)    33598 2023-05-29 17:12:04.032505 wellmet-0.9.3/wellmet/dicebox/circumtri.py
+-rw-r--r--   0 user         (0) root         (0)   100174 2023-01-15 11:50:00.032768 wellmet-0.9.3/wellmet/dicebox/goal.py
+-rw-r--r--   0 user         (0) root         (0)    36893 2023-01-15 11:50:38.030408 wellmet-0.9.3/wellmet/estimation.py
+-rw-r--r--   0 user         (0) root         (0)    52580 2023-01-15 11:51:29.030408 wellmet-0.9.3/wellmet/f_models.py
+-rw-r--r--   0 user         (0) root         (0)    42237 2023-03-12 14:45:57.030408 wellmet-0.9.3/wellmet/g_models.py
+-rw-r--r--   0 user         (0) root         (0)    21042 2023-05-28 14:15:30.030671 wellmet-0.9.3/wellmet/ghull.py
+-rw-r--r--   0 user         (0) root         (0)     3234 2022-05-13 19:15:46.030671 wellmet-0.9.3/wellmet/misc.py
+drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-29 17:30:15.085459 wellmet-0.9.3/wellmet/mplot/
+-rw-r--r--   0 user         (0) root         (0)     1407 2022-04-30 16:53:41.032768 wellmet-0.9.3/wellmet/mplot/__init__.py
+-rw-r--r--   0 user         (0) root         (0)     9741 2022-04-30 16:53:41.032768 wellmet-0.9.3/wellmet/mplot/_axes3d.py
+-rw-r--r--   0 user         (0) root         (0)      714 2022-04-30 16:53:41.033030 wellmet-0.9.3/wellmet/mplot/_axis3d_margins_patch.py
+-rw-r--r--   0 user         (0) root         (0)    23492 2023-03-30 13:18:09.033030 wellmet-0.9.3/wellmet/mplot/mart.py
+-rw-r--r--   0 user         (0) root         (0)    13647 2023-01-15 11:54:22.033030 wellmet-0.9.3/wellmet/mplot/mart3d.py
+-rw-r--r--   0 user         (0) root         (0)    26324 2023-05-29 17:11:54.033292 wellmet-0.9.3/wellmet/mplot/maxes.py
+-rw-r--r--   0 user         (0) root         (0)     5577 2022-04-30 16:53:41.033292 wellmet-0.9.3/wellmet/mplot/maxes3d.py
+-rw-r--r--   0 user         (0) root         (0)    17778 2023-05-29 17:11:54.033292 wellmet-0.9.3/wellmet/mplot/mfigs.py
+-rw-r--r--   0 user         (0) root         (0)    10463 2023-02-02 13:58:18.033292 wellmet-0.9.3/wellmet/mplot/mgraph.py
+-rw-r--r--   0 user         (0) root         (0)     1132 2022-04-30 16:53:41.033554 wellmet-0.9.3/wellmet/mplot/misc.py
+drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-29 17:30:15.162529 wellmet-0.9.3/wellmet/qt_gui/
+-rw-r--r--   0 user         (0) root         (0)        6 2022-04-30 16:53:41.033554 wellmet-0.9.3/wellmet/qt_gui/__init__.py
+-rw-r--r--   0 user         (0) root         (0)    44438 2023-01-15 11:54:47.033554 wellmet-0.9.3/wellmet/qt_gui/gl_plot.py
+-rw-r--r--   0 user         (0) root         (0)      348 2022-10-16 03:13:28.033816 wellmet-0.9.3/wellmet/qt_gui/gui_startup.py
+-rw-r--r--   0 user         (0) root         (0)     1970 2022-10-07 12:30:43.033816 wellmet-0.9.3/wellmet/qt_gui/qt_box_functions.py
+-rw-r--r--   0 user         (0) root         (0)    26239 2023-05-28 15:18:02.033816 wellmet-0.9.3/wellmet/qt_gui/qt_dicebox.py
+-rw-r--r--   0 user         (0) root         (0)    35342 2023-01-17 14:19:12.034078 wellmet-0.9.3/wellmet/qt_gui/qt_graph_widgets.py
+-rw-r--r--   0 user         (0) root         (0)    24326 2023-05-28 14:20:54.034078 wellmet-0.9.3/wellmet/qt_gui/qt_gui.py
+-rw-r--r--   0 user         (0) root         (0)    38391 2022-12-21 15:13:48.034078 wellmet-0.9.3/wellmet/qt_gui/qt_pairwise.py
+-rw-r--r--   0 user         (0) root         (0)    99810 2023-05-29 17:13:09.034340 wellmet-0.9.3/wellmet/qt_gui/qt_plot.py
+-rw-r--r--   0 user         (0) root         (0)     3244 2023-01-10 05:21:15.034340 wellmet-0.9.3/wellmet/qt_gui/qt_testcases.py
+-rw-r--r--   0 user         (0) root         (0)    56858 2022-11-29 15:50:00.034340 wellmet-0.9.3/wellmet/qt_gui/qt_voronoi.py
+-rw-r--r--   0 user         (0) root         (0)    10956 2023-01-15 11:55:28.030671 wellmet-0.9.3/wellmet/reader.py
+-rw-r--r--   0 user         (0) root         (0)     4416 2023-01-15 11:56:01.030933 wellmet-0.9.3/wellmet/samplebox.py
+-rw-r--r--   0 user         (0) root         (0)     6558 2022-04-30 16:53:42.030933 wellmet-0.9.3/wellmet/sball.py
+-rw-r--r--   0 user         (0) root         (0)     6739 2023-05-29 17:11:42.030933 wellmet-0.9.3/wellmet/schemes.py
+-rw-r--r--   0 user         (0) root         (0)     8309 2023-05-28 14:15:30.030933 wellmet-0.9.3/wellmet/shell.py
+-rw-r--r--   0 user         (0) root         (0)   134283 2023-05-29 17:11:31.031195 wellmet-0.9.3/wellmet/simplex.py
+-rw-r--r--   0 user         (0) root         (0)    13090 2023-05-28 14:15:30.031195 wellmet-0.9.3/wellmet/spring.py
+-rw-r--r--   0 user         (0) root         (0)    10953 2022-04-30 16:53:42.031457 wellmet-0.9.3/wellmet/stm_df.py
+drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-29 17:30:15.202375 wellmet-0.9.3/wellmet/testcases/
+-rw-r--r--   0 user         (0) root         (0)        0 2023-05-28 13:48:40.034603 wellmet-0.9.3/wellmet/testcases/__init__.py
+-rw-r--r--   0 user         (0) root         (0)     8987 2023-03-12 15:00:08.034603 wellmet-0.9.3/wellmet/testcases/gaussian_2D.py
+-rw-r--r--   0 user         (0) root         (0)     8183 2023-05-28 14:14:11.034603 wellmet-0.9.3/wellmet/testcases/testcases_2D.py
+-rw-r--r--   0 user         (0) root         (0)     3741 2023-02-24 08:01:44.034603 wellmet-0.9.3/wellmet/testcases/testcases_2D_papers.py
+-rw-r--r--   0 user         (0) root         (0)     2572 2023-01-14 08:20:10.034865 wellmet-0.9.3/wellmet/testcases/testcases_nD.py
+-rw-r--r--   0 user         (0) root         (0)    11998 2023-01-30 12:29:31.034865 wellmet-0.9.3/wellmet/testcases/testcases_nD_papers.py
+-rw-r--r--   0 user         (0) root         (0)    47956 2023-01-15 11:58:08.031457 wellmet-0.9.3/wellmet/voronoi.py
+-rw-r--r--   0 user         (0) root         (0)     2465 2023-05-28 14:15:30.031457 wellmet-0.9.3/wellmet/welford.py
+-rw-r--r--   0 user         (0) root         (0)    32101 2023-03-15 04:11:34.031457 wellmet-0.9.3/wellmet/whitebox.py
+-rw-r--r--   0 user         (0) root         (0)    26468 2023-05-28 14:15:30.031719 wellmet-0.9.3/wellmet/wireframe.py
+drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-29 17:30:14.967049 wellmet-0.9.3/wellmet.egg-info/
+-rw-r--r--   0 user         (0) root         (0)     5050 2023-05-29 17:30:14.031719 wellmet-0.9.3/wellmet.egg-info/PKG-INFO
+-rw-r--r--   0 user         (0) root         (0)     1642 2023-05-29 17:30:14.031719 wellmet-0.9.3/wellmet.egg-info/SOURCES.txt
+-rw-r--r--   0 user         (0) root         (0)        1 2023-05-29 17:30:14.031981 wellmet-0.9.3/wellmet.egg-info/dependency_links.txt
+-rw-r--r--   0 user         (0) root         (0)       70 2023-05-29 17:30:14.031981 wellmet-0.9.3/wellmet.egg-info/requires.txt
+-rw-r--r--   0 user         (0) root         (0)        8 2023-05-29 17:30:14.031981 wellmet-0.9.3/wellmet.egg-info/top_level.txt
```

### Comparing `wellmet-0.9.2/LICENSE` & `wellmet-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/pyproject.toml` & `wellmet-0.9.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "wellmet"
 version = "0.9.2"
 authors = [
   { name="Gerasimov Aleksei", email="ger-alex@seznam.cz" },
 ]
```

### Comparing `wellmet-0.9.2/wellmet/IS_stat.py` & `wellmet-0.9.3/wellmet/IS_stat.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/candybox.py` & `wellmet-0.9.3/wellmet/candybox.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/candynodes.py` & `wellmet-0.9.3/wellmet/candynodes.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/convex_hull.py` & `wellmet-0.9.3/wellmet/convex_hull.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/dicebox/__circumtri.py` & `wellmet-0.9.3/wellmet/dicebox/__circumtri.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/dicebox/_circumtri.py` & `wellmet-0.9.3/wellmet/dicebox/_circumtri.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/dicebox/_exploration.py` & `wellmet-0.9.3/wellmet/dicebox/_exploration.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/dicebox/censoring.py` & `wellmet-0.9.3/wellmet/dicebox/censoring.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/dicebox/circumtri.py` & `wellmet-0.9.3/wellmet/dicebox/circumtri.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/dicebox/goal.py` & `wellmet-0.9.3/wellmet/dicebox/goal.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/estimation.py` & `wellmet-0.9.3/wellmet/estimation.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/f_models.py` & `wellmet-0.9.3/wellmet/f_models.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/g_models.py` & `wellmet-0.9.3/wellmet/g_models.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/ghull.py` & `wellmet-0.9.3/wellmet/ghull.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/misc.py` & `wellmet-0.9.3/wellmet/misc.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/mplot/__init__.py` & `wellmet-0.9.3/wellmet/mplot/__init__.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/mplot/_axes3d.py` & `wellmet-0.9.3/wellmet/mplot/_axes3d.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/mplot/_axis3d_margins_patch.py` & `wellmet-0.9.3/wellmet/mplot/_axis3d_margins_patch.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/mplot/mart.py` & `wellmet-0.9.3/wellmet/mplot/mart.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/mplot/mart3d.py` & `wellmet-0.9.3/wellmet/mplot/mart3d.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/mplot/maxes.py` & `wellmet-0.9.3/wellmet/mplot/maxes.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/mplot/maxes3d.py` & `wellmet-0.9.3/wellmet/mplot/maxes3d.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/mplot/mfigs.py` & `wellmet-0.9.3/wellmet/mplot/mfigs.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/mplot/mgraph.py` & `wellmet-0.9.3/wellmet/mplot/mgraph.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/mplot/misc.py` & `wellmet-0.9.3/wellmet/mplot/misc.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/qt_gui/gl_plot.py` & `wellmet-0.9.3/wellmet/qt_gui/gl_plot.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/qt_gui/qt_box_functions.py` & `wellmet-0.9.3/wellmet/qt_gui/qt_box_functions.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/qt_gui/qt_dicebox.py` & `wellmet-0.9.3/wellmet/qt_gui/qt_dicebox.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/qt_gui/qt_graph_widgets.py` & `wellmet-0.9.3/wellmet/qt_gui/qt_graph_widgets.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/qt_gui/qt_gui.py` & `wellmet-0.9.3/wellmet/qt_gui/qt_gui.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/qt_gui/qt_pairwise.py` & `wellmet-0.9.3/wellmet/qt_gui/qt_pairwise.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/qt_gui/qt_plot.py` & `wellmet-0.9.3/wellmet/qt_gui/qt_plot.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/qt_gui/qt_testcases.py` & `wellmet-0.9.3/wellmet/qt_gui/qt_testcases.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/qt_gui/qt_voronoi.py` & `wellmet-0.9.3/wellmet/qt_gui/qt_voronoi.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/reader.py` & `wellmet-0.9.3/wellmet/reader.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/samplebox.py` & `wellmet-0.9.3/wellmet/samplebox.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/sball.py` & `wellmet-0.9.3/wellmet/sball.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/schemes.py` & `wellmet-0.9.3/wellmet/schemes.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/shell.py` & `wellmet-0.9.3/wellmet/shell.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/simplex.py` & `wellmet-0.9.3/wellmet/simplex.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/spring.py` & `wellmet-0.9.3/wellmet/spring.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/stm_df.py` & `wellmet-0.9.3/wellmet/stm_df.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/testcases/gaussian_2D.py` & `wellmet-0.9.3/wellmet/testcases/gaussian_2D.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/testcases/testcases_2D.py` & `wellmet-0.9.3/wellmet/testcases/testcases_2D.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/testcases/testcases_2D_papers.py` & `wellmet-0.9.3/wellmet/testcases/testcases_2D_papers.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/testcases/testcases_nD.py` & `wellmet-0.9.3/wellmet/testcases/testcases_nD.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/testcases/testcases_nD_papers.py` & `wellmet-0.9.3/wellmet/testcases/testcases_nD_papers.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/voronoi.py` & `wellmet-0.9.3/wellmet/voronoi.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/welford.py` & `wellmet-0.9.3/wellmet/welford.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/whitebox.py` & `wellmet-0.9.3/wellmet/whitebox.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet/wireframe.py` & `wellmet-0.9.3/wellmet/wireframe.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.2/wellmet.egg-info/SOURCES.txt` & `wellmet-0.9.3/wellmet.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
+setup.cfg
 setup.py
 wellmet/IS_stat.py
 wellmet/__init__.py
 wellmet/__main__.py
 wellmet/candybox.py
 wellmet/candynodes.py
 wellmet/convex_hull.py
```

