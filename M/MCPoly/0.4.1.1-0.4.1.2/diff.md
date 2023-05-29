# Comparing `tmp/MCPoly-0.4.1.1.tar.gz` & `tmp/MCPoly-0.4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MCPoly-0.4.1.1.tar", last modified: Mon May 29 09:29:55 2023, max compression
+gzip compressed data, was "MCPoly-0.4.1.2.tar", last modified: Mon May 29 11:10:54 2023, max compression
```

## Comparing `MCPoly-0.4.1.1.tar` & `MCPoly-0.4.1.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 09:29:55.543627 MCPoly-0.4.1.1/
--rw-r--r--   0 cxs454     (503) staff       (20)     1091 2023-05-03 15:22:57.000000 MCPoly-0.4.1.1/LICENSE
--rw-r--r--   0 cxs454     (503) staff       (20)       17 2023-05-04 08:23:11.000000 MCPoly-0.4.1.1/MANIFEST.in
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 09:29:55.533564 MCPoly-0.4.1.1/MCPoly/
--rw-r--r--   0 cxs454     (503) staff       (20)    14340 2023-05-29 09:29:27.000000 MCPoly-0.4.1.1/MCPoly/.DS_Store
--rw-r--r--   0 cxs454     (503) staff       (20)      178 2023-05-15 14:05:30.000000 MCPoly-0.4.1.1/MCPoly/__init__.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 09:29:55.534751 MCPoly-0.4.1.1/MCPoly/lmpset/
--rw-r--r--   0 cxs454     (503) staff       (20)       42 2023-05-29 08:31:35.000000 MCPoly-0.4.1.1/MCPoly/lmpset/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    16301 2023-05-29 06:37:57.000000 MCPoly-0.4.1.1/MCPoly/lmpset/chain.py
--rw-r--r--   0 cxs454     (503) staff       (20)    43926 2023-05-29 09:26:37.000000 MCPoly-0.4.1.1/MCPoly/lmpset/mould.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 09:29:55.536288 MCPoly-0.4.1.1/MCPoly/moldraw/
--rw-r--r--   0 cxs454     (503) staff       (20)     8966 2023-05-26 12:59:21.000000 MCPoly-0.4.1.1/MCPoly/moldraw/C_selection.py
--rw-r--r--   0 cxs454     (503) staff       (20)      128 2023-05-29 06:59:26.000000 MCPoly-0.4.1.1/MCPoly/moldraw/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    64145 2023-05-26 10:41:02.000000 MCPoly-0.4.1.1/MCPoly/moldraw/bind_selection.py
--rw-r--r--   0 cxs454     (503) staff       (20)    24385 2023-05-29 07:03:41.000000 MCPoly-0.4.1.1/MCPoly/moldraw/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)   181892 2023-05-26 12:59:34.000000 MCPoly-0.4.1.1/MCPoly/moldraw/molecule.py
--rw-r--r--   0 cxs454     (503) staff       (20)    98156 2023-05-26 10:40:13.000000 MCPoly-0.4.1.1/MCPoly/moldraw/sub_selection.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 09:29:55.538585 MCPoly-0.4.1.1/MCPoly/orcaset/
--rw-r--r--   0 cxs454     (503) staff       (20)     8635 2023-05-02 16:35:59.000000 MCPoly-0.4.1.1/MCPoly/orcaset/XYZtoINP.py
--rw-r--r--   0 cxs454     (503) staff       (20)      158 2023-05-11 15:49:25.000000 MCPoly-0.4.1.1/MCPoly/orcaset/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    16665 2023-05-15 14:09:24.000000 MCPoly-0.4.1.1/MCPoly/orcaset/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     7576 2023-05-15 14:09:22.000000 MCPoly-0.4.1.1/MCPoly/orcaset/mgui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     4842 2023-05-02 16:29:09.000000 MCPoly-0.4.1.1/MCPoly/orcaset/multiorca.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2072 2023-05-15 15:20:42.000000 MCPoly-0.4.1.1/MCPoly/orcaset/orca.py
--rw-r--r--   0 cxs454     (503) staff       (20)    18024 2023-05-16 09:54:57.000000 MCPoly-0.4.1.1/MCPoly/orcaset/ssgui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     8784 2023-05-11 15:46:31.000000 MCPoly-0.4.1.1/MCPoly/orcaset/ssorca.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2145 2023-05-09 08:28:02.000000 MCPoly-0.4.1.1/MCPoly/orcaset/view3dchoose.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 09:29:55.539506 MCPoly-0.4.1.1/MCPoly/sscurve/
--rw-r--r--   0 cxs454     (503) staff       (20)     1193 2023-05-02 16:03:26.000000 MCPoly-0.4.1.1/MCPoly/sscurve/YModulus.py
--rw-r--r--   0 cxs454     (503) staff       (20)       88 2023-05-09 08:48:45.000000 MCPoly-0.4.1.1/MCPoly/sscurve/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    12770 2023-05-17 15:37:43.000000 MCPoly-0.4.1.1/MCPoly/sscurve/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     5843 2023-05-19 09:04:58.000000 MCPoly-0.4.1.1/MCPoly/sscurve/multiple.py
--rw-r--r--   0 cxs454     (503) staff       (20)     6832 2023-05-19 08:52:37.000000 MCPoly-0.4.1.1/MCPoly/sscurve/single.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 09:29:55.540504 MCPoly-0.4.1.1/MCPoly/status/
--rw-r--r--   0 cxs454     (503) staff       (20)       62 2023-05-18 16:46:40.000000 MCPoly-0.4.1.1/MCPoly/status/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)     6202 2023-05-22 09:10:31.000000 MCPoly-0.4.1.1/MCPoly/status/echart.py
--rw-r--r--   0 cxs454     (503) staff       (20)    15750 2023-05-18 16:45:20.000000 MCPoly-0.4.1.1/MCPoly/status/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)    17836 2023-05-22 09:21:19.000000 MCPoly-0.4.1.1/MCPoly/status/status.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 09:29:55.541090 MCPoly-0.4.1.1/MCPoly/version/
--rw-r--r--   0 cxs454     (503) staff       (20)       23 2023-05-04 08:03:54.000000 MCPoly-0.4.1.1/MCPoly/version/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)       35 2023-05-29 09:29:16.000000 MCPoly-0.4.1.1/MCPoly/version/version.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 09:29:55.541453 MCPoly-0.4.1.1/MCPoly/view3d/
--rw-r--r--   0 cxs454     (503) staff       (20)       22 2023-04-30 18:16:37.000000 MCPoly-0.4.1.1/MCPoly/view3d/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)     1970 2023-05-09 13:30:17.000000 MCPoly-0.4.1.1/MCPoly/view3d/view3d.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 09:29:55.542009 MCPoly-0.4.1.1/MCPoly/vis/
--rw-r--r--   0 cxs454     (503) staff       (20)       18 2023-05-15 14:05:55.000000 MCPoly-0.4.1.1/MCPoly/vis/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2071 2023-05-29 07:04:54.000000 MCPoly-0.4.1.1/MCPoly/vis/vis.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 09:29:55.534325 MCPoly-0.4.1.1/MCPoly.egg-info/
--rw-r--r--   0 cxs454     (503) staff       (20)     3580 2023-05-29 09:29:55.000000 MCPoly-0.4.1.1/MCPoly.egg-info/PKG-INFO
--rw-r--r--   0 cxs454     (503) staff       (20)     1171 2023-05-29 09:29:55.000000 MCPoly-0.4.1.1/MCPoly.egg-info/SOURCES.txt
--rw-r--r--   0 cxs454     (503) staff       (20)        1 2023-05-29 09:29:55.000000 MCPoly-0.4.1.1/MCPoly.egg-info/dependency_links.txt
--rw-r--r--   0 cxs454     (503) staff       (20)      143 2023-05-29 09:29:55.000000 MCPoly-0.4.1.1/MCPoly.egg-info/requires.txt
--rw-r--r--   0 cxs454     (503) staff       (20)        7 2023-05-29 09:29:55.000000 MCPoly-0.4.1.1/MCPoly.egg-info/top_level.txt
--rw-r--r--   0 cxs454     (503) staff       (20)     3580 2023-05-29 09:29:55.543457 MCPoly-0.4.1.1/PKG-INFO
--rw-r--r--   0 cxs454     (503) staff       (20)     3216 2023-05-29 09:28:50.000000 MCPoly-0.4.1.1/README.md
--rw-r--r--   0 cxs454     (503) staff       (20)       38 2023-05-29 09:29:55.543674 MCPoly-0.4.1.1/setup.cfg
--rw-r--r--   0 cxs454     (503) staff       (20)     1033 2023-05-29 09:29:03.000000 MCPoly-0.4.1.1/setup.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 09:29:55.543007 MCPoly-0.4.1.1/tests/
--rw-r--r--   0 cxs454     (503) staff       (20)     4637 2023-05-02 12:31:39.000000 MCPoly-0.4.1.1/tests/test_lmpset.py
--rw-r--r--   0 cxs454     (503) staff       (20)      799 2023-05-03 10:12:20.000000 MCPoly-0.4.1.1/tests/test_moldraw.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2932 2023-05-02 17:01:47.000000 MCPoly-0.4.1.1/tests/test_orcaset.py
--rw-r--r--   0 cxs454     (503) staff       (20)     3535 2023-05-19 13:19:19.000000 MCPoly-0.4.1.1/tests/test_sscurve.py
--rw-r--r--   0 cxs454     (503) staff       (20)     5087 2023-05-22 09:21:41.000000 MCPoly-0.4.1.1/tests/test_status.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 11:10:54.813451 MCPoly-0.4.1.2/
+-rw-r--r--   0 cxs454     (503) staff       (20)     1091 2023-05-03 15:22:57.000000 MCPoly-0.4.1.2/LICENSE
+-rw-r--r--   0 cxs454     (503) staff       (20)       17 2023-05-04 08:23:11.000000 MCPoly-0.4.1.2/MANIFEST.in
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 11:10:54.806208 MCPoly-0.4.1.2/MCPoly/
+-rw-r--r--   0 cxs454     (503) staff       (20)    14340 2023-05-29 09:29:27.000000 MCPoly-0.4.1.2/MCPoly/.DS_Store
+-rw-r--r--   0 cxs454     (503) staff       (20)      178 2023-05-15 14:05:30.000000 MCPoly-0.4.1.2/MCPoly/__init__.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 11:10:54.807375 MCPoly-0.4.1.2/MCPoly/lmpset/
+-rw-r--r--   0 cxs454     (503) staff       (20)       42 2023-05-29 08:31:35.000000 MCPoly-0.4.1.2/MCPoly/lmpset/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    16301 2023-05-29 06:37:57.000000 MCPoly-0.4.1.2/MCPoly/lmpset/chain.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    45337 2023-05-29 11:10:08.000000 MCPoly-0.4.1.2/MCPoly/lmpset/mould.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 11:10:54.808741 MCPoly-0.4.1.2/MCPoly/moldraw/
+-rw-r--r--   0 cxs454     (503) staff       (20)     8966 2023-05-26 12:59:21.000000 MCPoly-0.4.1.2/MCPoly/moldraw/C_selection.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      128 2023-05-29 06:59:26.000000 MCPoly-0.4.1.2/MCPoly/moldraw/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    64145 2023-05-26 10:41:02.000000 MCPoly-0.4.1.2/MCPoly/moldraw/bind_selection.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    24385 2023-05-29 07:03:41.000000 MCPoly-0.4.1.2/MCPoly/moldraw/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)   181892 2023-05-26 12:59:34.000000 MCPoly-0.4.1.2/MCPoly/moldraw/molecule.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    98156 2023-05-26 10:40:13.000000 MCPoly-0.4.1.2/MCPoly/moldraw/sub_selection.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 11:10:54.810176 MCPoly-0.4.1.2/MCPoly/orcaset/
+-rw-r--r--   0 cxs454     (503) staff       (20)     8635 2023-05-02 16:35:59.000000 MCPoly-0.4.1.2/MCPoly/orcaset/XYZtoINP.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      158 2023-05-11 15:49:25.000000 MCPoly-0.4.1.2/MCPoly/orcaset/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    16665 2023-05-15 14:09:24.000000 MCPoly-0.4.1.2/MCPoly/orcaset/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     7576 2023-05-15 14:09:22.000000 MCPoly-0.4.1.2/MCPoly/orcaset/mgui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     4842 2023-05-02 16:29:09.000000 MCPoly-0.4.1.2/MCPoly/orcaset/multiorca.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     2072 2023-05-15 15:20:42.000000 MCPoly-0.4.1.2/MCPoly/orcaset/orca.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    18024 2023-05-16 09:54:57.000000 MCPoly-0.4.1.2/MCPoly/orcaset/ssgui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     8784 2023-05-11 15:46:31.000000 MCPoly-0.4.1.2/MCPoly/orcaset/ssorca.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     2145 2023-05-09 08:28:02.000000 MCPoly-0.4.1.2/MCPoly/orcaset/view3dchoose.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 11:10:54.810896 MCPoly-0.4.1.2/MCPoly/sscurve/
+-rw-r--r--   0 cxs454     (503) staff       (20)     1193 2023-05-02 16:03:26.000000 MCPoly-0.4.1.2/MCPoly/sscurve/YModulus.py
+-rw-r--r--   0 cxs454     (503) staff       (20)       88 2023-05-09 08:48:45.000000 MCPoly-0.4.1.2/MCPoly/sscurve/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    12770 2023-05-17 15:37:43.000000 MCPoly-0.4.1.2/MCPoly/sscurve/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     5843 2023-05-19 09:04:58.000000 MCPoly-0.4.1.2/MCPoly/sscurve/multiple.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     6832 2023-05-19 08:52:37.000000 MCPoly-0.4.1.2/MCPoly/sscurve/single.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 11:10:54.811480 MCPoly-0.4.1.2/MCPoly/status/
+-rw-r--r--   0 cxs454     (503) staff       (20)       62 2023-05-18 16:46:40.000000 MCPoly-0.4.1.2/MCPoly/status/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     6202 2023-05-22 09:10:31.000000 MCPoly-0.4.1.2/MCPoly/status/echart.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    15750 2023-05-18 16:45:20.000000 MCPoly-0.4.1.2/MCPoly/status/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    17836 2023-05-22 09:21:19.000000 MCPoly-0.4.1.2/MCPoly/status/status.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 11:10:54.811772 MCPoly-0.4.1.2/MCPoly/version/
+-rw-r--r--   0 cxs454     (503) staff       (20)       23 2023-05-04 08:03:54.000000 MCPoly-0.4.1.2/MCPoly/version/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)       35 2023-05-29 11:10:17.000000 MCPoly-0.4.1.2/MCPoly/version/version.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 11:10:54.812053 MCPoly-0.4.1.2/MCPoly/view3d/
+-rw-r--r--   0 cxs454     (503) staff       (20)       22 2023-04-30 18:16:37.000000 MCPoly-0.4.1.2/MCPoly/view3d/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     1970 2023-05-09 13:30:17.000000 MCPoly-0.4.1.2/MCPoly/view3d/view3d.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 11:10:54.812321 MCPoly-0.4.1.2/MCPoly/vis/
+-rw-r--r--   0 cxs454     (503) staff       (20)       18 2023-05-15 14:05:55.000000 MCPoly-0.4.1.2/MCPoly/vis/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     2071 2023-05-29 07:04:54.000000 MCPoly-0.4.1.2/MCPoly/vis/vis.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 11:10:54.806948 MCPoly-0.4.1.2/MCPoly.egg-info/
+-rw-r--r--   0 cxs454     (503) staff       (20)     3579 2023-05-29 11:10:54.000000 MCPoly-0.4.1.2/MCPoly.egg-info/PKG-INFO
+-rw-r--r--   0 cxs454     (503) staff       (20)     1171 2023-05-29 11:10:54.000000 MCPoly-0.4.1.2/MCPoly.egg-info/SOURCES.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)        1 2023-05-29 11:10:54.000000 MCPoly-0.4.1.2/MCPoly.egg-info/dependency_links.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)      143 2023-05-29 11:10:54.000000 MCPoly-0.4.1.2/MCPoly.egg-info/requires.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)        7 2023-05-29 11:10:54.000000 MCPoly-0.4.1.2/MCPoly.egg-info/top_level.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)     3579 2023-05-29 11:10:54.813272 MCPoly-0.4.1.2/PKG-INFO
+-rw-r--r--   0 cxs454     (503) staff       (20)     3215 2023-05-29 11:10:40.000000 MCPoly-0.4.1.2/README.md
+-rw-r--r--   0 cxs454     (503) staff       (20)       38 2023-05-29 11:10:54.813500 MCPoly-0.4.1.2/setup.cfg
+-rw-r--r--   0 cxs454     (503) staff       (20)     1033 2023-05-29 11:10:24.000000 MCPoly-0.4.1.2/setup.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-05-29 11:10:54.813071 MCPoly-0.4.1.2/tests/
+-rw-r--r--   0 cxs454     (503) staff       (20)     4637 2023-05-02 12:31:39.000000 MCPoly-0.4.1.2/tests/test_lmpset.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      799 2023-05-03 10:12:20.000000 MCPoly-0.4.1.2/tests/test_moldraw.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     2932 2023-05-02 17:01:47.000000 MCPoly-0.4.1.2/tests/test_orcaset.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     3535 2023-05-19 13:19:19.000000 MCPoly-0.4.1.2/tests/test_sscurve.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     5087 2023-05-22 09:21:41.000000 MCPoly-0.4.1.2/tests/test_status.py
```

### Comparing `MCPoly-0.4.1.1/LICENSE` & `MCPoly-0.4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/.DS_Store` & `MCPoly-0.4.1.2/MCPoly/.DS_Store`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/lmpset/chain.py` & `MCPoly-0.4.1.2/MCPoly/lmpset/chain.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/lmpset/mould.py` & `MCPoly-0.4.1.2/MCPoly/lmpset/mould.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import re
 import os
 import warnings
 import math as m
 from ase.io import read, write
 
-
 def replication(filename,x,xgap,y,ygap,z,zgap,absolute=False,startloc=[0,0,0],loc='./',chain=False):
     if absolute==True:
         warnings.warn('Make sure you avoid all the overlaps of molecules!')
     opath=os.getcwd()
     os.chdir(loc)
     xloc=startloc[0]
     yloc=startloc[1]
     zloc=startloc[2]
+    all_x=[]
     k=0
     w1=0
     w2=0
     w3=0
     w4=0
     w5=0
     l=[]
@@ -113,14 +113,16 @@
                     j=1
         elif w1==2:
             for i1 in range(x):
                 for i2 in range(y):
                     for i3 in range(z):
                         for i4 in range(len(l)):
                             f.write('{0} {1} {2} {3:.4f} {4:.5f} {5:.5f} {6:.5f}\n'.format(j,eval(l[i4][1]),eval(l[i4][2]),eval(l[i4][3]),eval(l[i4][-3])+(xd-real[0]+xgap)*i1-eval(x1[0]),eval(l[i4][-2])+(yd-real[1]+ygap)*i2-eval(y1[0]),eval(l[i4][-1])+(zd-real[2]+zgap)*i3-eval(z1[0])))
+                            if i1+i2+i3==0:
+                                all_x.append(eval(l[i4][-3]))
                             j=j+1
             l=[]
             j=1
             w1=0
             f.write('\n')
         elif w2==1:
             l1=re.findall(r'[0-9]+',line)
@@ -132,24 +134,36 @@
         elif w2==2:
             for i1 in range(x):
                 for i2 in range(y):
                     for i3 in range(z):
                         for i4 in range(len(l)):
                             if chain==True:
                                 if i4==len(l)-1:
-                                    if i1==0:
-                                        if eval(l[i4][2])>eval(l[i4][3])+eval(num)*k:
-                                            f.write('{0} {1} {2} {3}\n'.format(j,eval(l[i4][1]),eval(l[i4][2])+eval(num)*k+eval(num)*(x-1)*y*z),eval(l[i4][3])+eval(num)*k)
+                                    if all_x[eval(l[i4][2])-1]<=all_x[eval(l[i4][3])-1]:
+                                        if i1==0:
+                                            if eval(l[i4][2])>eval(l[i4][3])+eval(num)*k:
+                                                f.write('{0} {1} {2} {3}\n'.format(j,eval(l[i4][1]),eval(l[i4][2])+eval(num)*k+eval(num)*(x-1)*y*z),eval(l[i4][3])+eval(num)*k)
+                                            else:
+                                                f.write('{0} {1} {2} {3}\n'.format(j,eval(l[i4][1]),eval(l[i4][2])+eval(num)*k,eval(l[i4][3])+eval(num)*k+eval(num)*(x-1)*y*z))
                                         else:
-                                            f.write('{0} {1} {2} {3}\n'.format(j,eval(l[i4][1]),eval(l[i4][2])+eval(num)*k,eval(l[i4][3])+eval(num)*k+eval(num)*(x-1)*y*z))
-                                    else:
-                                        if eval(l[i4][2])>eval(l[i4][3])+eval(num)*k:
-                                            f.write('{0} {1} {2} {3}\n'.format(j,eval(l[i4][1]),eval(l[i4][2])+eval(num)*k-eval(num)*y*z,eval(l[i4][3])+eval(num)*k))
+                                            if eval(l[i4][2])>eval(l[i4][3])+eval(num)*k:
+                                                f.write('{0} {1} {2} {3}\n'.format(j,eval(l[i4][1]),eval(l[i4][2])+eval(num)*k-eval(num)*y*z,eval(l[i4][3])+eval(num)*k))
+                                            else:
+                                                f.write('{0} {1} {2} {3}\n'.format(j,eval(l[i4][1]),eval(l[i4][2])+eval(num)*k,eval(l[i4][3])+eval(num)*k-eval(num)*y*z))
+                                    elif all_x[eval(l[i4][2])-1]>all_x[eval(l[i4][3])-1]:
+                                        if i1==0:
+                                            if eval(l[i4][2])>eval(l[i4][3])+eval(num)*k:
+                                                f.write('{0} {1} {2} {3}\n'.format(j,eval(l[i4][1]),eval(l[i4][2])+eval(num)*k,eval(l[i4][3])+eval(num)*k+eval(num)*(x-1)*y*z))
+                                            else:
+                                                f.write('{0} {1} {2} {3}\n'.format(j,eval(l[i4][1]),eval(l[i4][2])+eval(num)*k+eval(num)*(x-1)*y*z,eval(l[i4][3])+eval(num)*k))
                                         else:
-                                            f.write('{0} {1} {2} {3}\n'.format(j,eval(l[i4][1]),eval(l[i4][2])+eval(num)*k,eval(l[i4][3])+eval(num)*k-eval(num)*y*z))
+                                            if eval(l[i4][2])>eval(l[i4][3])+eval(num)*k:
+                                                f.write('{0} {1} {2} {3}\n'.format(j,eval(l[i4][1]),eval(l[i4][2])+eval(num)*k,eval(l[i4][3])+eval(num)*k-eval(num)*y*z))
+                                            else:
+                                                f.write('{0} {1} {2} {3}\n'.format(j,eval(l[i4][1]),eval(l[i4][2])+eval(num)*k-eval(num)*y*z,eval(l[i4][3])+eval(num)*k))
                                 else:
                                     f.write('{0} {1} {2} {3}\n'.format(j,eval(l[i4][1]),eval(l[i4][2])+eval(num)*k,eval(l[i4][3])+eval(num)*k))
                             else:
                                 f.write('{0} {1} {2} {3}\n'.format(j,eval(l[i4][1]),eval(l[i4][2])+eval(num)*k,eval(l[i4][3])+eval(num)*k))
                             j=j+1
                         k=k+1
             l=[]
@@ -868,15 +882,15 @@
             3 1 2 0.0915 1.27330 2.34271 1.00000            3 1 2 0.0915 -8.01953 0.61332 -1.04153
             4 1 2 0.0915 2.72158 2.03208 1.98722            4 1 2 0.0915 -6.57166 0.30320 -0.05380
             5 1 3 -0.6883 1.56973 2.53667 4.33729           5 1 3 -0.6883 -7.72351 0.80779 2.29626
             6 1 2 0.0939 0.00000 2.94776 3.08107            6 1 2 0.0939 -9.29323 1.21888 1.04005
             
             ...                                             ...
         """
-        return replication(self.atoms,x,xgap,y,ygap,z,zgap,absolute,startloc,self.loc)
+        return replication(self.atoms,x,xgap,y,ygap,z,zgap,absolute,startloc,self.loc,chain)
     
     def brick(self,x,xgap,y,ygap,z,zgap,xpattern='0',ypattern='0',zpattern='0',shuffle=0,absolute=False,startloc=[0,0,0]):
         """
     The method to create a box with replicated molecular in brick settlement.
     * * * * *
      * * * *
     * * * * *
```

### Comparing `MCPoly-0.4.1.1/MCPoly/moldraw/C_selection.py` & `MCPoly-0.4.1.2/MCPoly/moldraw/C_selection.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/moldraw/bind_selection.py` & `MCPoly-0.4.1.2/MCPoly/moldraw/bind_selection.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/moldraw/gui.py` & `MCPoly-0.4.1.2/MCPoly/moldraw/gui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/moldraw/molecule.py` & `MCPoly-0.4.1.2/MCPoly/moldraw/molecule.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/moldraw/sub_selection.py` & `MCPoly-0.4.1.2/MCPoly/moldraw/sub_selection.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/orcaset/XYZtoINP.py` & `MCPoly-0.4.1.2/MCPoly/orcaset/XYZtoINP.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/orcaset/gui.py` & `MCPoly-0.4.1.2/MCPoly/orcaset/gui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/orcaset/mgui.py` & `MCPoly-0.4.1.2/MCPoly/orcaset/mgui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/orcaset/multiorca.py` & `MCPoly-0.4.1.2/MCPoly/orcaset/multiorca.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/orcaset/orca.py` & `MCPoly-0.4.1.2/MCPoly/orcaset/orca.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/orcaset/ssgui.py` & `MCPoly-0.4.1.2/MCPoly/orcaset/ssgui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/orcaset/ssorca.py` & `MCPoly-0.4.1.2/MCPoly/orcaset/ssorca.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/orcaset/view3dchoose.py` & `MCPoly-0.4.1.2/MCPoly/orcaset/view3dchoose.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/sscurve/YModulus.py` & `MCPoly-0.4.1.2/MCPoly/sscurve/YModulus.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/sscurve/gui.py` & `MCPoly-0.4.1.2/MCPoly/sscurve/gui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/sscurve/multiple.py` & `MCPoly-0.4.1.2/MCPoly/sscurve/multiple.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/sscurve/single.py` & `MCPoly-0.4.1.2/MCPoly/sscurve/single.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/status/echart.py` & `MCPoly-0.4.1.2/MCPoly/status/echart.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/status/gui.py` & `MCPoly-0.4.1.2/MCPoly/status/gui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/status/status.py` & `MCPoly-0.4.1.2/MCPoly/status/status.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/view3d/view3d.py` & `MCPoly-0.4.1.2/MCPoly/view3d/view3d.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly/vis/vis.py` & `MCPoly-0.4.1.2/MCPoly/vis/vis.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/MCPoly.egg-info/PKG-INFO` & `MCPoly-0.4.1.2/MCPoly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MCPoly
-Version: 0.4.1.1
+Version: 0.4.1.2
 Summary: Useful tools for Computational Chemistry for polymers
 Home-page: https://github.com/Omicron-Fluor/MCPoly/
 Author: Omicron Fluor
 Author-email: cxs454@student.bham.ac.uk
 License: MIT
 Keywords: ORCA,Mechanical Property,Computational Chemistry
 Description-Content-Type: text/markdown
@@ -13,15 +13,15 @@
 # MCPoly
 Some methods to deal with some manipulation of computational chemistry, mostly about mechanical properties of polymers.
 ![](./reference/function.png)
 
 ## Overview
 `MCPoly` is a Python library to make some steps of computational chemistry easier. It includes some functions of drawing molecule structures, creating proper .xyz , .inp , .mol and .data file, which specialised for using ORCA and LAMMPS, and some functions for researching the mechanical property of some polymers.
 
-## Updated in v0.4.1.1 (29.05.23)
+## Updated in v0.4.1.2(29.05.23)
 1. BIG UPDATE: Molecule Designer GUI is included in this package. You can now use it to draw molecule with 3D view at the same time.
 <img src="https://github.com/Omicron-Fluor/MCPoly/blob/main/reference/moldraw_gui.png">
 2. Add 'chain' in 'lmpset' package. You can now use it to convert periodic polymer structure input data now.
 
 ## Updated in v0.3.0 (19.05.23)
 1. BIG UPDATE: Now status package can be used to see energy and gibbs free energy by .energy and .gibbs.
 2. BIG UPDATE: The new Reaction Diagram GUI is included in this package. You can use it to merge some tables and sea the relevant reaction diagram as a reference.
```

### Comparing `MCPoly-0.4.1.1/MCPoly.egg-info/SOURCES.txt` & `MCPoly-0.4.1.2/MCPoly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/PKG-INFO` & `MCPoly-0.4.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MCPoly
-Version: 0.4.1.1
+Version: 0.4.1.2
 Summary: Useful tools for Computational Chemistry for polymers
 Home-page: https://github.com/Omicron-Fluor/MCPoly/
 Author: Omicron Fluor
 Author-email: cxs454@student.bham.ac.uk
 License: MIT
 Keywords: ORCA,Mechanical Property,Computational Chemistry
 Description-Content-Type: text/markdown
@@ -13,15 +13,15 @@
 # MCPoly
 Some methods to deal with some manipulation of computational chemistry, mostly about mechanical properties of polymers.
 ![](./reference/function.png)
 
 ## Overview
 `MCPoly` is a Python library to make some steps of computational chemistry easier. It includes some functions of drawing molecule structures, creating proper .xyz , .inp , .mol and .data file, which specialised for using ORCA and LAMMPS, and some functions for researching the mechanical property of some polymers.
 
-## Updated in v0.4.1.1 (29.05.23)
+## Updated in v0.4.1.2(29.05.23)
 1. BIG UPDATE: Molecule Designer GUI is included in this package. You can now use it to draw molecule with 3D view at the same time.
 <img src="https://github.com/Omicron-Fluor/MCPoly/blob/main/reference/moldraw_gui.png">
 2. Add 'chain' in 'lmpset' package. You can now use it to convert periodic polymer structure input data now.
 
 ## Updated in v0.3.0 (19.05.23)
 1. BIG UPDATE: Now status package can be used to see energy and gibbs free energy by .energy and .gibbs.
 2. BIG UPDATE: The new Reaction Diagram GUI is included in this package. You can use it to merge some tables and sea the relevant reaction diagram as a reference.
```

### Comparing `MCPoly-0.4.1.1/README.md` & `MCPoly-0.4.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # MCPoly
 Some methods to deal with some manipulation of computational chemistry, mostly about mechanical properties of polymers.
 ![](./reference/function.png)
 
 ## Overview
 `MCPoly` is a Python library to make some steps of computational chemistry easier. It includes some functions of drawing molecule structures, creating proper .xyz , .inp , .mol and .data file, which specialised for using ORCA and LAMMPS, and some functions for researching the mechanical property of some polymers.
 
-## Updated in v0.4.1.1 (29.05.23)
+## Updated in v0.4.1.2(29.05.23)
 1. BIG UPDATE: Molecule Designer GUI is included in this package. You can now use it to draw molecule with 3D view at the same time.
 <img src="https://github.com/Omicron-Fluor/MCPoly/blob/main/reference/moldraw_gui.png">
 2. Add 'chain' in 'lmpset' package. You can now use it to convert periodic polymer structure input data now.
 
 ## Updated in v0.3.0 (19.05.23)
 1. BIG UPDATE: Now status package can be used to see energy and gibbs free energy by .energy and .gibbs.
 2. BIG UPDATE: The new Reaction Diagram GUI is included in this package. You can use it to merge some tables and sea the relevant reaction diagram as a reference.
```

### Comparing `MCPoly-0.4.1.1/setup.py` & `MCPoly-0.4.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='MCPoly',
-    version='0.4.1.1',
+    version='0.4.1.2',
     description='Useful tools for Computational Chemistry for polymers',
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=['MCPoly','MCPoly.lmpset','MCPoly.moldraw','MCPoly.orcaset','MCPoly.sscurve','MCPoly.status','MCPoly.view3d','MCPoly.version','MCPoly.vis'],
     author='Omicron Fluor',
     author_email='cxs454@student.bham.ac.uk',
```

### Comparing `MCPoly-0.4.1.1/tests/test_lmpset.py` & `MCPoly-0.4.1.2/tests/test_lmpset.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/tests/test_moldraw.py` & `MCPoly-0.4.1.2/tests/test_moldraw.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/tests/test_orcaset.py` & `MCPoly-0.4.1.2/tests/test_orcaset.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/tests/test_sscurve.py` & `MCPoly-0.4.1.2/tests/test_sscurve.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.1.1/tests/test_status.py` & `MCPoly-0.4.1.2/tests/test_status.py`

 * *Files identical despite different names*

