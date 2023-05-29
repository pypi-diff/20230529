# Comparing `tmp/vot-toolkit-0.6.1.tar.gz` & `tmp/vot-toolkit-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vot-toolkit-0.6.1.tar", last modified: Fri May 12 15:14:46 2023, max compression
+gzip compressed data, was "vot-toolkit-0.6.2.tar", last modified: Tue May 16 14:36:57 2023, max compression
```

## Comparing `vot-toolkit-0.6.1.tar` & `vot-toolkit-0.6.2.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.168255 vot-toolkit-0.6.1/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      211 2022-03-25 11:28:05.000000 vot-toolkit-0.6.1/MANIFEST.in
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3646 2023-05-12 15:14:46.168255 vot-toolkit-0.6.1/PKG-INFO
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2716 2023-05-09 11:09:24.000000 vot-toolkit-0.6.1/README.md
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      295 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/requirements.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       38 2023-05-12 15:14:46.168255 vot-toolkit-0.6.1/setup.cfg
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1427 2023-05-09 11:09:24.000000 vot-toolkit-0.6.1/setup.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.140256 vot-toolkit-0.6.1/vot/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1889 2023-05-10 17:51:17.000000 vot-toolkit-0.6.1/vot/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      158 2021-04-20 09:19:05.000000 vot-toolkit-0.6.1/vot/__main__.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.144255 vot-toolkit-0.6.1/vot/analysis/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    15920 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/analysis/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    21427 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/analysis/_processor.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7608 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/analysis/accuracy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2517 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/analysis/failures.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16706 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/analysis/longterm.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12235 2023-04-18 14:33:10.000000 vot-toolkit-0.6.1/vot/analysis/multistart.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8824 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/analysis/supervised.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.148255 vot-toolkit-0.6.1/vot/dataset/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16723 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/dataset/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14672 2020-12-04 15:25:26.000000 vot-toolkit-0.6.1/vot/dataset/cow.png
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3079 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/dataset/dummy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5356 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/dataset/got10k.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    11511 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/dataset/otb.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4924 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/dataset/proxy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3753 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/dataset/trackingnet.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9239 2023-05-10 17:51:17.000000 vot-toolkit-0.6.1/vot/dataset/vot.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.152255 vot-toolkit-0.6.1/vot/document/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12362 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/document/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      465 2020-12-04 15:25:26.000000 vot-toolkit-0.6.1/vot/document/commands.tex
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5273 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/document/common.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5217 2021-04-15 12:10:29.000000 vot-toolkit-0.6.1/vot/document/html.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    89476 2020-12-04 15:25:26.000000 vot-toolkit-0.6.1/vot/document/jquery.js
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5748 2022-03-11 09:29:31.000000 vot-toolkit-0.6.1/vot/document/latex.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16184 2020-12-04 15:25:26.000000 vot-toolkit-0.6.1/vot/document/pure.css
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      647 2020-12-04 15:25:26.000000 vot-toolkit-0.6.1/vot/document/report.css
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1212 2020-12-04 15:25:26.000000 vot-toolkit-0.6.1/vot/document/report.js
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9933 2020-12-04 15:25:26.000000 vot-toolkit-0.6.1/vot/document/table.js
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        0 2022-03-23 08:48:42.000000 vot-toolkit-0.6.1/vot/document/tests.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.152255 vot-toolkit-0.6.1/vot/experiment/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7631 2023-05-12 15:11:47.000000 vot-toolkit-0.6.1/vot/experiment/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      798 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/experiment/helpers.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7180 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/experiment/multirun.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3044 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/experiment/multistart.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3214 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/experiment/transformer.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.152255 vot-toolkit-0.6.1/vot/region/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2373 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/region/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9258 2023-05-12 12:23:17.000000 vot-toolkit-0.6.1/vot/region/io.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9593 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/region/raster.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10172 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/region/shapes.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3238 2023-05-12 11:54:32.000000 vot-toolkit-0.6.1/vot/region/tests.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.156256 vot-toolkit-0.6.1/vot/stack/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3047 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      253 2022-03-25 11:28:05.000000 vot-toolkit-0.6.1/vot/stack/otb100.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      251 2022-03-25 11:28:05.000000 vot-toolkit-0.6.1/vot/stack/otb50.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.156256 vot-toolkit-0.6.1/vot/stack/tests/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      183 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/tests/basic.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      550 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/tests/multiobject.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      638 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/tests/segmentation.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      863 2022-03-25 11:28:05.000000 vot-toolkit-0.6.1/vot/stack/tests.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      351 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2013.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      374 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2014.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.156256 vot-toolkit-0.6.1/vot/stack/vot2015/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      405 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2015/rgb.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      322 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2015/tir.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.156256 vot-toolkit-0.6.1/vot/stack/vot2016/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      540 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2016/rgb.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      296 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2016/tir.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      856 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2017.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.156256 vot-toolkit-0.6.1/vot/stack/vot2018/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2018/longterm.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      791 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2018/shortterm.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.160256 vot-toolkit-0.6.1/vot/stack/vot2019/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2019/longterm.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2019/rgbd.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      396 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2019/rgbtir.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      789 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2019/shortterm.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.160256 vot-toolkit-0.6.1/vot/stack/vot2020/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2020/longterm.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2020/rgbd.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      396 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2020/rgbtir.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      867 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2020/shortterm.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.160256 vot-toolkit-0.6.1/vot/stack/vot2021/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2021/lt.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2021/rgbd.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      867 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2021/st.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.164255 vot-toolkit-0.6.1/vot/stack/vot2022/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      422 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/stack/vot2022/depth.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      482 2022-03-25 11:28:05.000000 vot-toolkit-0.6.1/vot/stack/vot2022/lt.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      424 2022-03-25 11:28:05.000000 vot-toolkit-0.6.1/vot/stack/vot2022/rgbd.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2022-03-25 11:28:05.000000 vot-toolkit-0.6.1/vot/stack/vot2022/stb.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2022-03-25 11:28:05.000000 vot-toolkit-0.6.1/vot/stack/vot2022/sts.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      193 2023-05-10 17:51:17.000000 vot-toolkit-0.6.1/vot/stack/vots2023.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.164255 vot-toolkit-0.6.1/vot/tracker/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    19774 2023-05-12 15:12:58.000000 vot-toolkit-0.6.1/vot/tracker/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      763 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/tracker/dummy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6642 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/tracker/results.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      476 2021-04-20 09:19:05.000000 vot-toolkit-0.6.1/vot/tracker/tests.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    19771 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/tracker/trax.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.168255 vot-toolkit-0.6.1/vot/utilities/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12508 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/utilities/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16476 2023-05-10 17:51:17.000000 vot-toolkit-0.6.1/vot/utilities/cli.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2635 2021-04-15 12:10:29.000000 vot-toolkit-0.6.1/vot/utilities/data.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8255 2021-04-15 12:10:29.000000 vot-toolkit-0.6.1/vot/utilities/draw.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3609 2020-12-04 15:25:26.000000 vot-toolkit-0.6.1/vot/utilities/migration.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3798 2021-04-20 09:19:05.000000 vot-toolkit-0.6.1/vot/utilities/net.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8133 2022-03-25 11:28:05.000000 vot-toolkit-0.6.1/vot/utilities/notebook.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       45 2023-05-09 11:09:24.000000 vot-toolkit-0.6.1/vot/version.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.168255 vot-toolkit-0.6.1/vot/workspace/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7013 2023-05-05 11:01:43.000000 vot-toolkit-0.6.1/vot/workspace/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10512 2023-05-12 11:16:07.000000 vot-toolkit-0.6.1/vot/workspace/storage.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1786 2023-05-12 10:35:28.000000 vot-toolkit-0.6.1/vot/workspace/tests.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-12 15:14:46.168255 vot-toolkit-0.6.1/vot_toolkit.egg-info/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3646 2023-05-12 15:14:45.000000 vot-toolkit-0.6.1/vot_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2409 2023-05-12 15:14:45.000000 vot-toolkit-0.6.1/vot_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        1 2023-05-12 15:14:45.000000 vot-toolkit-0.6.1/vot_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       48 2023-05-12 15:14:45.000000 vot-toolkit-0.6.1/vot_toolkit.egg-info/entry_points.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      296 2023-05-12 15:14:45.000000 vot-toolkit-0.6.1/vot_toolkit.egg-info/requires.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        4 2023-05-12 15:14:45.000000 vot-toolkit-0.6.1/vot_toolkit.egg-info/top_level.txt
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.862747 vot-toolkit-0.6.2/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      211 2022-03-25 11:28:05.000000 vot-toolkit-0.6.2/MANIFEST.in
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3646 2023-05-16 14:36:57.862747 vot-toolkit-0.6.2/PKG-INFO
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2716 2023-05-09 11:09:24.000000 vot-toolkit-0.6.2/README.md
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      295 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/requirements.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       38 2023-05-16 14:36:57.862747 vot-toolkit-0.6.2/setup.cfg
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1427 2023-05-09 11:09:24.000000 vot-toolkit-0.6.2/setup.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.834747 vot-toolkit-0.6.2/vot/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1889 2023-05-10 17:51:17.000000 vot-toolkit-0.6.2/vot/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      158 2021-04-20 09:19:05.000000 vot-toolkit-0.6.2/vot/__main__.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.834747 vot-toolkit-0.6.2/vot/analysis/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16084 2023-05-16 13:31:56.000000 vot-toolkit-0.6.2/vot/analysis/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    21427 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/analysis/_processor.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7601 2023-05-16 13:31:56.000000 vot-toolkit-0.6.2/vot/analysis/accuracy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2535 2023-05-16 13:31:56.000000 vot-toolkit-0.6.2/vot/analysis/failures.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16995 2023-05-16 13:31:56.000000 vot-toolkit-0.6.2/vot/analysis/longterm.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12289 2023-05-16 13:31:56.000000 vot-toolkit-0.6.2/vot/analysis/multistart.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8860 2023-05-16 13:31:56.000000 vot-toolkit-0.6.2/vot/analysis/supervised.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.838747 vot-toolkit-0.6.2/vot/dataset/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16723 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/dataset/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14672 2020-12-04 15:25:26.000000 vot-toolkit-0.6.2/vot/dataset/cow.png
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3079 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/dataset/dummy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5356 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/dataset/got10k.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    11511 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/dataset/otb.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4924 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/dataset/proxy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3753 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/dataset/trackingnet.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10365 2023-05-16 14:28:55.000000 vot-toolkit-0.6.2/vot/dataset/vot.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.842747 vot-toolkit-0.6.2/vot/document/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12362 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/document/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      465 2020-12-04 15:25:26.000000 vot-toolkit-0.6.2/vot/document/commands.tex
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5298 2023-05-16 13:31:56.000000 vot-toolkit-0.6.2/vot/document/common.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5217 2021-04-15 12:10:29.000000 vot-toolkit-0.6.2/vot/document/html.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    89476 2020-12-04 15:25:26.000000 vot-toolkit-0.6.2/vot/document/jquery.js
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5748 2022-03-11 09:29:31.000000 vot-toolkit-0.6.2/vot/document/latex.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16184 2020-12-04 15:25:26.000000 vot-toolkit-0.6.2/vot/document/pure.css
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      647 2020-12-04 15:25:26.000000 vot-toolkit-0.6.2/vot/document/report.css
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1212 2020-12-04 15:25:26.000000 vot-toolkit-0.6.2/vot/document/report.js
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9933 2020-12-04 15:25:26.000000 vot-toolkit-0.6.2/vot/document/table.js
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        0 2022-03-23 08:48:42.000000 vot-toolkit-0.6.2/vot/document/tests.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.842747 vot-toolkit-0.6.2/vot/experiment/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7631 2023-05-16 07:48:27.000000 vot-toolkit-0.6.2/vot/experiment/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      798 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/experiment/helpers.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7180 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/experiment/multirun.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3044 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/experiment/multistart.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3214 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/experiment/transformer.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.842747 vot-toolkit-0.6.2/vot/region/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2373 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/region/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9258 2023-05-16 07:48:27.000000 vot-toolkit-0.6.2/vot/region/io.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9593 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/region/raster.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10172 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/region/shapes.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3238 2023-05-16 07:48:27.000000 vot-toolkit-0.6.2/vot/region/tests.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.846747 vot-toolkit-0.6.2/vot/stack/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3047 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      253 2022-03-25 11:28:05.000000 vot-toolkit-0.6.2/vot/stack/otb100.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      251 2022-03-25 11:28:05.000000 vot-toolkit-0.6.2/vot/stack/otb50.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.846747 vot-toolkit-0.6.2/vot/stack/tests/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      183 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/tests/basic.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      541 2023-05-16 13:31:56.000000 vot-toolkit-0.6.2/vot/stack/tests/multiobject.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      638 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/tests/segmentation.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      863 2022-03-25 11:28:05.000000 vot-toolkit-0.6.2/vot/stack/tests.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      351 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2013.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      374 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2014.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.846747 vot-toolkit-0.6.2/vot/stack/vot2015/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      405 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2015/rgb.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      322 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2015/tir.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.846747 vot-toolkit-0.6.2/vot/stack/vot2016/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      540 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2016/rgb.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      296 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2016/tir.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      856 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2017.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.850747 vot-toolkit-0.6.2/vot/stack/vot2018/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2018/longterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      791 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2018/shortterm.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.850747 vot-toolkit-0.6.2/vot/stack/vot2019/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2019/longterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2019/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      396 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2019/rgbtir.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      789 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2019/shortterm.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.850747 vot-toolkit-0.6.2/vot/stack/vot2020/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2020/longterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2020/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      396 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2020/rgbtir.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      867 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2020/shortterm.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.854747 vot-toolkit-0.6.2/vot/stack/vot2021/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2021/lt.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2021/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      867 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2021/st.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.854747 vot-toolkit-0.6.2/vot/stack/vot2022/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      422 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2022/depth.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      482 2022-03-25 11:28:05.000000 vot-toolkit-0.6.2/vot/stack/vot2022/lt.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      424 2022-03-25 11:28:05.000000 vot-toolkit-0.6.2/vot/stack/vot2022/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2022-03-25 11:28:05.000000 vot-toolkit-0.6.2/vot/stack/vot2022/stb.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2022-03-25 11:28:05.000000 vot-toolkit-0.6.2/vot/stack/vot2022/sts.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      193 2023-05-10 17:51:17.000000 vot-toolkit-0.6.2/vot/stack/vots2023.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.858747 vot-toolkit-0.6.2/vot/tracker/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    19774 2023-05-16 07:48:27.000000 vot-toolkit-0.6.2/vot/tracker/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      763 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/tracker/dummy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6642 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/tracker/results.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      476 2021-04-20 09:19:05.000000 vot-toolkit-0.6.2/vot/tracker/tests.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    19771 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/tracker/trax.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.858747 vot-toolkit-0.6.2/vot/utilities/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12740 2023-05-16 14:21:10.000000 vot-toolkit-0.6.2/vot/utilities/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16476 2023-05-10 17:51:17.000000 vot-toolkit-0.6.2/vot/utilities/cli.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2635 2021-04-15 12:10:29.000000 vot-toolkit-0.6.2/vot/utilities/data.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8255 2021-04-15 12:10:29.000000 vot-toolkit-0.6.2/vot/utilities/draw.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3609 2020-12-04 15:25:26.000000 vot-toolkit-0.6.2/vot/utilities/migration.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5130 2023-05-16 14:33:12.000000 vot-toolkit-0.6.2/vot/utilities/net.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8133 2022-03-25 11:28:05.000000 vot-toolkit-0.6.2/vot/utilities/notebook.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       45 2023-05-16 13:31:56.000000 vot-toolkit-0.6.2/vot/version.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.858747 vot-toolkit-0.6.2/vot/workspace/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7013 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/workspace/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10512 2023-05-12 11:16:07.000000 vot-toolkit-0.6.2/vot/workspace/storage.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1786 2023-05-16 07:48:27.000000 vot-toolkit-0.6.2/vot/workspace/tests.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.862747 vot-toolkit-0.6.2/vot_toolkit.egg-info/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3646 2023-05-16 14:36:57.000000 vot-toolkit-0.6.2/vot_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2409 2023-05-16 14:36:57.000000 vot-toolkit-0.6.2/vot_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        1 2023-05-16 14:36:57.000000 vot-toolkit-0.6.2/vot_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       48 2023-05-16 14:36:57.000000 vot-toolkit-0.6.2/vot_toolkit.egg-info/entry_points.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      296 2023-05-16 14:36:57.000000 vot-toolkit-0.6.2/vot_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        4 2023-05-16 14:36:57.000000 vot-toolkit-0.6.2/vot_toolkit.egg-info/top_level.txt
```

### Comparing `vot-toolkit-0.6.1/PKG-INFO` & `vot-toolkit-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vot-toolkit
-Version: 0.6.1
+Version: 0.6.2
 Summary: Perform visual object tracking experiments and analyze results
 Home-page: https://github.com/votchallenge/toolkit
 Author: Luka Cehovin Zajc
 Author-email: luka.cehovin@gmail.com
 License: UNKNOWN
 Description: 
         The VOT evaluation toolkit
```

### Comparing `vot-toolkit-0.6.1/README.md` & `vot-toolkit-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/setup.py` & `vot-toolkit-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/__init__.py` & `vot-toolkit-0.6.2/vot/__init__.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/analysis/__init__.py` & `vot-toolkit-0.6.2/vot/analysis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,14 +194,21 @@
         self._identifier_cache = None
 
     def compatible(self, experiment: Experiment):
         raise NotImplementedError()
 
     @property
     def title(self) -> str:
+        if self.name is None:
+            return self._title_default
+        else:
+            return self.name
+
+    @property
+    def _title_default(self) -> str:
         raise NotImplementedError()
 
     def dependencies(self) -> List["Analysis"]:
         return []
 
     @property
     def identifier(self) -> str:
```

### Comparing `vot-toolkit-0.6.1/vot/analysis/_processor.py` & `vot-toolkit-0.6.2/vot/analysis/_processor.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/analysis/accuracy.py` & `vot-toolkit-0.6.2/vot/analysis/accuracy.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,19 +53,19 @@
     bounded = Boolean(default=True)
     threshold = Float(default=None, val_min=0, val_max=1)
 
     def compatible(self, experiment: Experiment):
         return isinstance(experiment, MultiRunExperiment)
 
     @property
-    def title(self):
+    def _title_default(self):
         return "Sequence accurarcy"
 
     def describe(self):
-        return Measure("Accuracy", "AUC", 0, 1, Sorting.DESCENDING),
+        return Measure(self.title, "", 0, 1, Sorting.DESCENDING),
 
     def subcompute(self, experiment: Experiment, tracker: Tracker, sequence: Sequence, dependencies: List[Grid]) -> Tuple[Any]:
 
         assert isinstance(experiment, MultiRunExperiment)
 
         objects = sequence.objects()
         objects_accuracy = 0
@@ -94,22 +94,22 @@
     analysis = Include(SequenceAccuracy)
     weighted = Boolean(default=True)
 
     def compatible(self, experiment: Experiment):
         return isinstance(experiment, MultiRunExperiment)
 
     @property
-    def title(self):
+    def _title_default(self):
         return "Accurarcy"
 
     def dependencies(self):
         return self.analysis,
 
     def describe(self):
-        return Measure("Accuracy", "AUC", 0, 1, Sorting.DESCENDING),
+        return Measure(self.title, "", 0, 1, Sorting.DESCENDING),
 
     def aggregate(self, _: Tracker, sequences: List[Sequence], results: Grid):
         accuracy = 0
         frames = 0
 
         for i, sequence in enumerate(sequences):
             if results[i, 0] is None:
@@ -134,19 +134,19 @@
     threshold = Float(default=None, val_min=0, val_max=1)
     resolution = Integer(default=100, val_min=2)
 
     def compatible(self, experiment: Experiment):
         return isinstance(experiment, MultiRunExperiment)
 
     @property
-    def title(self):
+    def _title_default(self):
         return "Sequence success plot"
 
     def describe(self):
-        return Curve("Success plot", 2, "Success", minimal=(0, 0), maximal=(1, 1), labels=("Threshold", "Success"), trait="success"),
+        return Curve("Plot", 2, "S", minimal=(0, 0), maximal=(1, 1), labels=("Threshold", "Success"), trait="success"),
 
     def subcompute(self, experiment: Experiment, tracker: Tracker, sequence: Sequence, dependencies: List[Grid]) -> Tuple[Any]:
 
         assert isinstance(experiment, MultiRunExperiment)
 
         objects = sequence.objects()
         bounds = (sequence.size) if self.bounded else None
@@ -187,19 +187,19 @@
     def dependencies(self):
         return self.analysis,
 
     def compatible(self, experiment: Experiment):
         return isinstance(experiment, MultiRunExperiment)
 
     @property
-    def title(self):
-        return "Sequence success plot"
+    def _title_default(self):
+        return "Success plot"
 
     def describe(self):
-        return Curve("Success plot", 2, "Success", minimal=(0, 0), maximal=(1, 1), labels=("Threshold", "Success"), trait="success"),
+        return Curve("Plot", 2, "S", minimal=(0, 0), maximal=(1, 1), labels=("Threshold", "Success"), trait="success"),
 
     def aggregate(self, _: Tracker, sequences: List[Sequence], results: Grid):
         axis_x = np.linspace(0, 1, self.resolution)
         axis_y = np.zeros_like(axis_x)
 
         for i, _ in enumerate(sequences):
             if results[i, 0] is None:
```

### Comparing `vot-toolkit-0.6.1/vot/analysis/failures.py` & `vot-toolkit-0.6.2/vot/analysis/failures.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 @analysis_registry.register("failures")
 class FailureCount(SeparableAnalysis):
 
     def compatible(self, experiment: Experiment):
         return isinstance(experiment, SupervisedExperiment)
 
     @property
-    def title(self):
+    def _title_default(self):
         return "Number of failures"
 
     def describe(self):
         return Measure("Failures", "F", 0, None, Sorting.ASCENDING),
 
     def subcompute(self, experiment: Experiment, tracker: Tracker, sequence: Sequence, dependencies: List[Grid]) -> Tuple[Any]:
 
@@ -61,15 +61,15 @@
     def compatible(self, experiment: Experiment):
         return isinstance(experiment, SupervisedExperiment)
 
     def dependencies(self):
         return self.analysis,
 
     @property
-    def title(self):
+    def _title_default(self):
         return "Number of failures"
 
     def describe(self):
         return Measure("Failures", "F", 0, None, Sorting.ASCENDING), 
 
     def aggregate(self, _: Tracker, sequences: List[Sequence], results: Grid):
         failures = 0
```

### Comparing `vot-toolkit-0.6.1/vot/analysis/longterm.py` & `vot-toolkit-0.6.2/vot/analysis/longterm.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             recall[i] = np.sum(overlaps[subset]) / n_visible
 
     return precision, recall
 
 class _ConfidenceScores(SeparableAnalysis):
 
     @property
-    def title(self):
+    def _title_default(self):
         return "Aggregate confidence scores"
 
     def describe(self):
         return None,
 
     def compatible(self, experiment: Experiment):
         return isinstance(experiment, UnsupervisedExperiment)
@@ -83,15 +83,15 @@
 
 
 class _Thresholds(SequenceAggregator):
 
     resolution = Integer(default=100)
 
     @property
-    def title(self):
+    def _title_default(self):
         return "Thresholds for tracking precision/recall"
 
     def describe(self):
         return None,
 
     def compatible(self, experiment: Experiment):
         return isinstance(experiment, UnsupervisedExperiment)
@@ -110,15 +110,15 @@
     """ Computes the precision/recall curves for a tracker for given sequences. """
 
     thresholds = Include(_Thresholds)
     ignore_unknown = Boolean(default=True)
     bounded = Boolean(default=True)
 
     @property
-    def title(self):
+    def _title_default(self):
         return "Tracking precision/recall"
 
     def describe(self):
         return Curve("Precision Recall curve", dimensions=2, abbreviation="PR", minimal=(0, 0), maximal=(1, 1), labels=("Recall", "Precision")), None
 
     def compatible(self, experiment: Experiment):
         return isinstance(experiment, UnsupervisedExperiment)
@@ -150,15 +150,15 @@
 @analysis_registry.register("pr_curve")
 class PrecisionRecallCurve(SequenceAggregator):
     """ Computes the average precision/recall curve for a tracker. """
 
     curves = Include(PrecisionRecallCurves)
 
     @property
-    def title(self):
+    def _title_default(self):
         return "Tracking precision/recall average curve"
 
     def describe(self):
         return self.curves.describe()
 
     def compatible(self, experiment: Experiment):
         return isinstance(experiment, UnsupervisedExperiment)
@@ -186,15 +186,15 @@
 @analysis_registry.register("f_curve")
 class FScoreCurve(Analysis):
 
     beta = Float(default=1)
     prcurve = Include(PrecisionRecallCurve)
 
     @property
-    def title(self):
+    def _title_default(self):
         return "Tracking precision/recall"
 
     def describe(self):
         return Plot("Tracking F-score curve", "F", wrt="normalized threshold", minimal=0, maximal=1), None
 
     def compatible(self, experiment: Experiment):
         return isinstance(experiment, UnsupervisedExperiment)
@@ -220,15 +220,15 @@
 @analysis_registry.register("average_tpr")
 class PrecisionRecall(Analysis):
 
     prcurve = Include(PrecisionRecallCurve)
     fcurve = Include(FScoreCurve)
 
     @property
-    def title(self):
+    def _title_default(self):
         return "Tracking precision/recall"
 
     def describe(self):
         return Measure("Precision", "Pr", minimal=0, maximal=1, direction=Sorting.DESCENDING), \
              Measure("Recall", "Re", minimal=0, maximal=1, direction=Sorting.DESCENDING), \
              Measure("F Score", "F", minimal=0, maximal=1, direction=Sorting.DESCENDING)
 
@@ -338,15 +338,15 @@
     bounded = Boolean(default=True)
     absence_threshold = Integer(default=10, val_min=0)
 
     def compatible(self, experiment: Experiment):
         return isinstance(experiment, MultiRunExperiment)
 
     @property
-    def title(self):
+    def _title_default(self):
         return "Quality Auxiliary"
 
     def describe(self):
         return Measure("Non-reported Error", "NRE", 0, 1, Sorting.DESCENDING), \
             Measure("Drift-rate Error", "DRE", 0, 1, Sorting.DESCENDING), \
             Measure("Absence-detection Quality", "ADQ", 0, 1, Sorting.DESCENDING),
 
@@ -386,24 +386,29 @@
             not_reported_error += CM / (CT + CF + CM)
             drift_rate_error += CF / (CT + CF + CM)
 
             if CN + CH > self.absence_threshold:
                 absence_detection += CN / (CN + CH)
                 absence_valid += 1
 
-        return not_reported_error / len(objects), drift_rate_error / len(objects), absence_detection / absence_valid,
+        if absence_valid > 0:
+            absence_detection /= absence_valid
+        else:
+            absence_detection = None
+
+        return not_reported_error / len(objects), drift_rate_error / len(objects), absence_detection,
 
 
 @analysis_registry.register("average_quality_auxiliary")
 class AverageQualityAuxiliary(SequenceAggregator):
 
     analysis = Include(QualityAuxiliary)
 
     @property
-    def title(self):
+    def _title_default(self):
         return "Quality Auxiliary"
 
     def dependencies(self):
         return self.analysis,
 
     def describe(self):
         return Measure("Non-reported Error", "NRE", 0, 1, Sorting.DESCENDING), \
@@ -413,21 +418,24 @@
     def compatible(self, experiment: Experiment):
         return isinstance(experiment, MultiRunExperiment)
 
     def aggregate(self, tracker: Tracker, sequences: List[Sequence], results: Grid):
         not_reported_error = 0
         drift_rate_error = 0
         absence_detection = 0
+        absence_count = 0
 
         for nre, dre, ad in results:
             not_reported_error += nre
             drift_rate_error += dre
-            absence_detection += ad
+            if ad is not None:
+                absence_count += 1
+                absence_detection += ad
 
-        return not_reported_error / len(sequences), drift_rate_error / len(sequences), absence_detection / len(sequences)
+        return not_reported_error / len(sequences), drift_rate_error / len(sequences), absence_detection / absence_count
 
 from vot.analysis import SequenceAggregator
 from vot.analysis.accuracy import SequenceAccuracy
 
 @analysis_registry.register("longterm_ar")
 class AccuracyRobustness(Analysis):
     """Longterm multi-object accuracy-robustness measure. """
@@ -439,15 +447,15 @@
     def dependencies(self) -> List[Analysis]:
         return self.counts, SequenceAccuracy(burnin=0, threshold=self.threshold, bounded=self.bounded, ignore_invisible=True, ignore_unknown=False)
     
     def compatible(self, experiment: Experiment):
         return isinstance(experiment, MultiRunExperiment)
 
     @property
-    def title(self):
+    def _title_default(self):
         return "Accuracy-robustness"
 
     def describe(self):
         return Measure("Accuracy", "A", minimal=0, maximal=1, direction=Sorting.DESCENDING), \
              Measure("Robustness", "R", minimal=0, direction=Sorting.DESCENDING), \
              Point("AR plot", dimensions=2, abbreviation="AR", minimal=(0, 0), \
                 maximal=(1, 1), labels=("Robustness", "Accuracy"), trait="ar")
```

### Comparing `vot-toolkit-0.6.1/vot/analysis/multistart.py` & `vot-toolkit-0.6.2/vot/analysis/multistart.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     burnin = Integer(default=10, val_min=0)
     grace = Integer(default=10, val_min=0)
     bounded = Boolean(default=True)
     threshold = Float(default=0.1, val_min=0, val_max=1)
 
     @property
-    def title(self):
+    def _title_default(self):
         return "AR Analysis"
 
     def describe(self):
         return Measure("Accuracy", "A", minimal=0, maximal=1, direction=Sorting.DESCENDING), \
              Measure("Robustness", "R", minimal=0, direction=Sorting.DESCENDING), \
              Point("AR plot", dimensions=2, abbreviation="AR",
                 minimal=(0, 0), maximal=(1, 1), labels=("Robustness", "Accuracy"), trait="ar"), \
@@ -107,15 +107,15 @@
 
 @analysis_registry.register("multistart_average_ar")
 class AverageAccuracyRobustness(SequenceAggregator):
 
     analysis = Include(AccuracyRobustness)
 
     @property
-    def title(self):
+    def _title_default(self):
         return "AR Analysis"
 
     def dependencies(self):
         return self.analysis, 
 
     def describe(self):
         return Measure("Accuracy", "A", minimal=0, maximal=1, direction=Sorting.DESCENDING), \
@@ -148,15 +148,15 @@
 
     burnin = Integer(default=10, val_min=0)
     grace = Integer(default=10, val_min=0)
     bounded = Boolean(default=True)
     threshold = Float(default=0.1, val_min=0, val_max=1)
 
     @property
-    def title(self):
+    def _title_default(self):
         return "Fragment Analysis"
 
     def describe(self):
         return Curve("Success", 2, "Sc", minimal=(0, 0), maximal=(1,1), trait="points"), Curve("Accuracy", 2, "Ac", minimal=(0, 0), maximal=(1,1), trait="points")
 
     def compatible(self, experiment: Experiment):
         return isinstance(experiment, MultiStartExperiment)
@@ -213,15 +213,15 @@
     grace = Integer(default=10, val_min=0)
     bounded = Boolean(default=True)
     threshold = Float(default=0.1, val_min=0, val_max=1)
 
     high = Integer()
 
     @property
-    def title(self):
+    def _title_default(self):
         return "EAO Curve"
 
     def describe(self):
         return Plot("Expected average overlap", "EAO", minimal=0, maximal=1, wrt="frames", trait="eao"),
 
     def compatible(self, experiment: Experiment):
         return isinstance(experiment, MultiStartExperiment)
@@ -279,15 +279,15 @@
 #TODO: remove high
 @analysis_registry.register("multistart_eao_curve")
 class EAOCurve(SequenceAggregator):
 
     curves = Include(EAOCurves)
     
     @property
-    def title(self):
+    def _title_default(self):
         return "EAO Curve"
 
     def describe(self):
         return Plot("Expected average overlap", "EAO", minimal=0, maximal=1, wrt="frames", trait="eao"),
 
     def compatible(self, experiment: Experiment):
         return isinstance(experiment, MultiStartExperiment)
@@ -311,15 +311,15 @@
 class EAOScore(Analysis):
 
     low = Integer()
     high = Integer()
     eaocurve = Include(EAOCurve)
 
     @property
-    def title(self):
+    def _title_default(self):
         return "EAO analysis"
 
     def describe(self):
         return Measure("Expected average overlap", "EAO", minimal=0, maximal=1, direction=Sorting.DESCENDING),
 
     def compatible(self, experiment: Experiment):
         return isinstance(experiment, MultiStartExperiment)
```

### Comparing `vot-toolkit-0.6.1/vot/analysis/supervised.py` & `vot-toolkit-0.6.2/vot/analysis/supervised.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
     sensitivity = Float(default=30, val_min=1)
     burnin = Integer(default=10, val_min=0)
     ignore_unknown = Boolean(default=True)
     bounded = Boolean(default=True)
 
     @property
-    def title(self):
+    def _title_default(self):
         return "AR analysis"
 
     def describe(self):
         return Measure("Accuracy", "A", minimal=0, maximal=1, direction=Sorting.DESCENDING), \
              Measure("Robustness", "R", minimal=0, direction=Sorting.ASCENDING), \
              Point("AR plot", dimensions=2, abbreviation="AR", minimal=(0, 0), \
                 maximal=(1, 1), labels=("Robustness", "Accuracy"), trait="ar"), \
@@ -110,15 +110,15 @@
 
 @analysis_registry.register("supervised_average_ar")
 class AverageAccuracyRobustness(SequenceAggregator):
 
     analysis = Include(AccuracyRobustness)
 
     @property
-    def title(self):
+    def _title_default(self):
         return "AR Analysis"
 
     def dependencies(self):
         return self.analysis,
 
     def describe(self):
         return Measure("Accuracy", "A", minimal=0, maximal=1, direction=Sorting.DESCENDING), \
@@ -147,15 +147,15 @@
 @analysis_registry.register("supervised_eao_curve")
 class EAOCurve(TrackerSeparableAnalysis):
 
     burnin = Integer(default=10, val_min=0)
     bounded = Boolean(default=True)
 
     @property
-    def title(self):
+    def _title_default(self):
         return "EAO Curve"
 
     def describe(self):
         return Plot("Expected Average Overlap", "EAO", minimal=0, maximal=1, trait="eao"),
 
     def compatible(self, experiment: Experiment):
         return isinstance(experiment, SupervisedExperiment)
@@ -203,15 +203,15 @@
 class EAOScore(Analysis):
 
     eaocurve = Include(EAOCurve)
     low = Integer()
     high = Integer()
 
     @property
-    def title(self):
+    def _title_default(self):
         return "EAO analysis"
 
     def describe(self):
         return Measure("Expected average overlap", "EAO", 0, 1, Sorting.DESCENDING),
 
     def compatible(self, experiment: Experiment):
         return isinstance(experiment, SupervisedExperiment)
```

### Comparing `vot-toolkit-0.6.1/vot/dataset/__init__.py` & `vot-toolkit-0.6.2/vot/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/dataset/cow.png` & `vot-toolkit-0.6.2/vot/dataset/cow.png`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/dataset/dummy.py` & `vot-toolkit-0.6.2/vot/dataset/dummy.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/dataset/got10k.py` & `vot-toolkit-0.6.2/vot/dataset/got10k.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/dataset/otb.py` & `vot-toolkit-0.6.2/vot/dataset/otb.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/dataset/proxy.py` & `vot-toolkit-0.6.2/vot/dataset/proxy.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/dataset/trackingnet.py` & `vot-toolkit-0.6.2/vot/dataset/trackingnet.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/dataset/vot.py` & `vot-toolkit-0.6.2/vot/dataset/vot.py`

 * *Files 10% similar despite different names*

```diff
@@ -161,62 +161,97 @@
         return self._sequences.values().__iter__()
 
     def list(self):
         return list(self._sequences.keys())
 
 def download_dataset_meta(url, path):
     from vot.utilities.net import download_uncompress, download_json, get_base_url, join_url, NetworkException
+    from vot.utilities import format_size
 
     meta = download_json(url)
 
-    logger.info('Downloading sequence dataset "%s" with %s sequences.', meta["name"], len(meta["sequences"]))
+    total_size = 0
+    for sequence in meta["sequences"]:
+        total_size += sequence["annotations"]["uncompressed"]
+        for channel in sequence["channels"].values():
+            total_size += channel["uncompressed"]
+
+    logger.info('Downloading sequence dataset "%s" with %s sequences (total %s).', meta["name"], len(meta["sequences"]), format_size(total_size))
 
     base_url = get_base_url(url) + "/"
 
+    failed = []
+
     with Progress("Downloading", len(meta["sequences"])) as progress:
         for sequence in meta["sequences"]:
             sequence_directory = os.path.join(path, sequence["name"])
             os.makedirs(sequence_directory, exist_ok=True)
 
+            if os.path.isfile(os.path.join(sequence_directory, "sequence")):
+                refdata = read_properties(os.path.join(sequence_directory, "sequence"))
+                if refdata["uid"] == sequence["annotations"]["uid"]:
+                    logger.info('Sequence "%s" already downloaded.', sequence["name"])
+                    progress.relative(1)
+                    continue
+
             data = {'name': sequence["name"], 'fps': sequence["fps"], 'format': 'default'}
 
             annotations_url = join_url(base_url, sequence["annotations"]["url"])
 
+            data["uid"] = sequence["annotations"]["uid"]
+
             try:
                 download_uncompress(annotations_url, sequence_directory)
             except NetworkException as e:
-                raise DatasetException("Unable do download annotations bundle")
+                logger.exception(e)
+                failed.append(sequence["name"])
+                continue
             except IOError as e:
-                raise DatasetException("Unable to extract annotations bundle, is the target directory writable and do you have enough space?")
+                logger.exception(e)
+                failed.append(sequence["name"])
+                continue
+
+            failure = False
 
             for cname, channel in sequence["channels"].items():
                 channel_directory = os.path.join(sequence_directory, cname)
                 os.makedirs(channel_directory, exist_ok=True)
 
                 channel_url = join_url(base_url, channel["url"])
 
                 try:
                     download_uncompress(channel_url, channel_directory)
                 except NetworkException as e:
-                    raise DatasetException("Unable do download channel bundle")
+                    logger.exception(e)
+                    failed.append(sequence["name"])
+                    failure = False
                 except IOError as e:
-                    raise DatasetException("Unable to extract channel bundle, is the target directory writable and do you have enough space?")
+                    logger.exception(e)
+                    failed.append(sequence["name"])
+                    failure = False
 
                 if "pattern" in channel:
                     data["channels." + cname] = cname + os.path.sep + channel["pattern"]
                 else:
                     data["channels." + cname] = cname + os.path.sep
 
-            write_properties(os.path.join(sequence_directory, 'sequence'), data)
+                if failure:
+                    continue
 
+            write_properties(os.path.join(sequence_directory, 'sequence'), data)
             progress.relative(1)
 
-    with open(os.path.join(path, "list.txt"), "w") as fp:
-        for sequence in meta["sequences"]:
-            fp.write('{}\n'.format(sequence["name"]))
+    if len(failed) > 0:
+        logger.error('Failed to download %d sequences.', len(failed))
+        logger.error('Failed sequences: %s', ', '.join(failed))
+    else:
+        logger.info('Successfully downloaded all sequences.')
+        with open(os.path.join(path, "list.txt"), "w") as fp:
+            for sequence in meta["sequences"]:
+                fp.write('{}\n'.format(sequence["name"]))
 
 def write_sequence(directory: str, sequence: Sequence):
 
     channels = sequence.channels()
 
     metadata = dict()
     metadata["channel.default"] = sequence.metadata("channel.default", "color")
```

### Comparing `vot-toolkit-0.6.1/vot/document/__init__.py` & `vot-toolkit-0.6.2/vot/document/__init__.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/document/common.py` & `vot-toolkit-0.6.2/vot/document/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
                 for t in order if order is not None else range(len(trackers)):
                     tracker = trackers[t]
                     values = aresults[t, 0]
                     data = values[i] if not values is None else None
                     plot(tracker, data)
 
-                experiment_plots.append((description.name, plot))
+                experiment_plots.append((analysis.title + " - " + description.name, plot))
 
         plots[experiment] = experiment_plots
 
     return plots
 
 def format_value(data):
     if data is None:
```

### Comparing `vot-toolkit-0.6.1/vot/document/html.py` & `vot-toolkit-0.6.2/vot/document/html.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/document/jquery.js` & `vot-toolkit-0.6.2/vot/document/jquery.js`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/document/latex.py` & `vot-toolkit-0.6.2/vot/document/latex.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/document/pure.css` & `vot-toolkit-0.6.2/vot/document/pure.css`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/document/report.css` & `vot-toolkit-0.6.2/vot/document/report.css`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/document/report.js` & `vot-toolkit-0.6.2/vot/document/report.js`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/document/table.js` & `vot-toolkit-0.6.2/vot/document/table.js`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/experiment/__init__.py` & `vot-toolkit-0.6.2/vot/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/experiment/helpers.py` & `vot-toolkit-0.6.2/vot/experiment/helpers.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/experiment/multirun.py` & `vot-toolkit-0.6.2/vot/experiment/multirun.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/experiment/multistart.py` & `vot-toolkit-0.6.2/vot/experiment/multistart.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/experiment/transformer.py` & `vot-toolkit-0.6.2/vot/experiment/transformer.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/region/__init__.py` & `vot-toolkit-0.6.2/vot/region/__init__.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/region/io.py` & `vot-toolkit-0.6.2/vot/region/io.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/region/raster.py` & `vot-toolkit-0.6.2/vot/region/raster.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/region/shapes.py` & `vot-toolkit-0.6.2/vot/region/shapes.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/region/tests.py` & `vot-toolkit-0.6.2/vot/region/tests.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/stack/__init__.py` & `vot-toolkit-0.6.2/vot/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/stack/tests/multiobject.yaml` & `vot-toolkit-0.6.2/vot/stack/tests/multiobject.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
       - type: average_success_plot
         name: Quality plot
         burnin: 0
         ignore_unknown: False
       - type: longterm_ar
         name: AR
       - type: average_quality_auxiliary
-        name: Auxiliary measures
+        name: Auxiliary
```

### Comparing `vot-toolkit-0.6.1/vot/stack/tests/segmentation.yaml` & `vot-toolkit-0.6.2/vot/stack/tests/segmentation.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/stack/tests.py` & `vot-toolkit-0.6.2/vot/stack/tests.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/stack/vot2016/rgb.yaml` & `vot-toolkit-0.6.2/vot/stack/vot2016/rgb.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/stack/vot2017.yaml` & `vot-toolkit-0.6.2/vot/stack/vot2017.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/stack/vot2018/shortterm.yaml` & `vot-toolkit-0.6.2/vot/stack/vot2018/shortterm.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/stack/vot2019/shortterm.yaml` & `vot-toolkit-0.6.2/vot/stack/vot2019/shortterm.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/stack/vot2020/shortterm.yaml` & `vot-toolkit-0.6.2/vot/stack/vot2020/shortterm.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/stack/vot2021/st.yaml` & `vot-toolkit-0.6.2/vot/stack/vot2021/st.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/stack/vot2022/stb.yaml` & `vot-toolkit-0.6.2/vot/stack/vot2022/stb.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/stack/vot2022/sts.yaml` & `vot-toolkit-0.6.2/vot/stack/vot2022/sts.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/tracker/__init__.py` & `vot-toolkit-0.6.2/vot/tracker/__init__.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/tracker/dummy.py` & `vot-toolkit-0.6.2/vot/tracker/dummy.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/tracker/results.py` & `vot-toolkit-0.6.2/vot/tracker/results.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/tracker/trax.py` & `vot-toolkit-0.6.2/vot/tracker/trax.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/utilities/__init__.py` & `vot-toolkit-0.6.2/vot/utilities/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -335,14 +335,21 @@
             return val.lower() in ['true', '1', 't', 'y', 'yes']
         else:
             return bool(val)
 
     except ValueError:
         raise RuntimeError("Logical value conversion error")
 
+def format_size(num, suffix="B"):
+    for unit in ["", "Ki", "Mi", "Gi", "Ti", "Pi", "Ei", "Zi"]:
+        if abs(num) < 1024.0:
+            return f"{num:3.1f}{unit}{suffix}"
+        num /= 1024.0
+    return f"{num:.1f}Yi{suffix}"
+
 def singleton(class_):
     instances = {}
     def getinstance(*args, **kwargs):
         if class_ not in instances:
             instances[class_] = class_(*args, **kwargs)
         return instances[class_]
     return getinstance
```

### Comparing `vot-toolkit-0.6.1/vot/utilities/cli.py` & `vot-toolkit-0.6.2/vot/utilities/cli.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/utilities/data.py` & `vot-toolkit-0.6.2/vot/utilities/data.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/utilities/draw.py` & `vot-toolkit-0.6.2/vot/utilities/draw.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/utilities/migration.py` & `vot-toolkit-0.6.2/vot/utilities/migration.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/utilities/net.py` & `vot-toolkit-0.6.2/vot/utilities/net.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 import shutil
 import tempfile
 from urllib.parse import urlparse, urljoin
 
 import requests
 
-from vot import ToolkitException
+from vot import ToolkitException, get_logger
 
 class NetworkException(ToolkitException):
     pass
 
 def get_base_url(url):
     return url.rsplit('/', 1)[0]
     
@@ -51,15 +51,17 @@
 def download_json(url):
     try:
         return requests.get(url).json()
     except requests.exceptions.RequestException as e:
         raise NetworkException("Unable to read JSON file {}".format(e))
 
 
-def download(url, output, callback=None, chunk_size=1024*32):
+def download(url, output, callback=None, chunk_size=1024*32, retry=10):
+    logger = get_logger()
+
     with requests.session() as sess:
 
         is_gdrive = is_google_drive_url(url)
         
         while True:
             res = sess.get(url, stream=True)
             
@@ -75,14 +77,15 @@
             # Need to redirect with confiramtion
             gurl = get_url_from_gdrive_confirmation(res.text)
 
             if gurl is None:
                 raise NetworkException("Permission denied for {}".format(gurl))
             url = gurl
 
+
         if output is None:
             if is_gdrive:
                 m = re.search('filename="(.*)"',
                             res.headers['Content-Disposition'])
                 output = m.groups()[0]
             else:
                 output = os.path.basename(url)
@@ -92,38 +95,67 @@
         if output_is_path:
             tmp_file = tempfile.mktemp()
             filehandle = open(tmp_file, 'wb')
         else:
             tmp_file = None
             filehandle = output
 
+        position = 0
+        progress = False
+
         try:
             total = res.headers.get('Content-Length')
-
             if total is not None:
                 total = int(total)
+            while True:
+                try:
+                    for chunk in res.iter_content(chunk_size=chunk_size):
+                        filehandle.write(chunk)
+                        position += len(chunk)
+                        progress = True
+                        if callback:
+                            callback(position, total)
+
+                    if position < total:
+                        raise requests.exceptions.RequestException("Connection closed")
+
+                    if tmp_file:
+                        filehandle.close()
+                        shutil.copy(tmp_file, output)
+                    break
+
+                except requests.exceptions.RequestException as e:
+                    if not progress:
+                        logger.warning("Error when downloading file, retrying")
+                        retry-=1
+                        if retry < 1:
+                            raise NetworkException("Unable to download file {}".format(e))
+                        res = sess.get(url, stream=True)
+                        filehandle.seek(0)
+                        position = 0
+                    else:
+                        logger.warning("Error when downloading file, trying to resume download")
+                        res = sess.get(url, stream=True, headers=({'Range': f'bytes={position}-'} if position > 0 else None))
+                    progress = False
+
+            if position < total:
+                raise NetworkException("Unable to download file")
 
-            for chunk in res.iter_content(chunk_size=chunk_size):
-                filehandle.write(chunk)
-                if callback:
-                    callback(len(chunk), total)
-            if tmp_file:
-                filehandle.close()
-                shutil.copy(tmp_file, output)
-        except IOError:
-            raise NetworkException("Error when downloading file")
+        except IOError as e:
+            raise NetworkException("Local I/O Error when downloading file: %s" % e)
         finally:
             try:
                 if tmp_file:
                     os.remove(tmp_file)
             except OSError:
                 pass
 
         return output
 
+
 def download_uncompress(url, path):
     from vot.utilities import extract_files
     _, ext = os.path.splitext(urlparse(url).path)
     tmp_file = tempfile.mktemp(suffix=ext)
     try:
         download(url, tmp_file)
         extract_files(tmp_file, path)
```

### Comparing `vot-toolkit-0.6.1/vot/utilities/notebook.py` & `vot-toolkit-0.6.2/vot/utilities/notebook.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/workspace/__init__.py` & `vot-toolkit-0.6.2/vot/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/workspace/storage.py` & `vot-toolkit-0.6.2/vot/workspace/storage.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot/workspace/tests.py` & `vot-toolkit-0.6.2/vot/workspace/tests.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.1/vot_toolkit.egg-info/PKG-INFO` & `vot-toolkit-0.6.2/vot_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vot-toolkit
-Version: 0.6.1
+Version: 0.6.2
 Summary: Perform visual object tracking experiments and analyze results
 Home-page: https://github.com/votchallenge/toolkit
 Author: Luka Cehovin Zajc
 Author-email: luka.cehovin@gmail.com
 License: UNKNOWN
 Description: 
         The VOT evaluation toolkit
```

### Comparing `vot-toolkit-0.6.1/vot_toolkit.egg-info/SOURCES.txt` & `vot-toolkit-0.6.2/vot_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

