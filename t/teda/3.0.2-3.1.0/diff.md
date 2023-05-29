# Comparing `tmp/teda-3.0.2.tar.gz` & `tmp/teda-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teda-3.0.2.tar", max compression
+gzip compressed data, was "teda-3.1.0.tar", max compression
```

## Comparing `teda-3.0.2.tar` & `teda-3.1.0.tar`

### file list

```diff
@@ -1,74 +1,130 @@
--rw-r--r--   0        0        0     1066 2020-06-04 16:42:55.000000 teda-3.0.2/LICENSE
--rw-r--r--   0        0        0     4719 2020-12-02 21:00:51.000070 teda-3.0.2/README.md
--rw-r--r--   0        0        0      454 2023-04-28 05:38:12.203689 teda-3.0.2/pyproject.toml
--rw-r--r--   0        0        0       32 2020-06-04 16:24:35.000000 teda-3.0.2/teda/__init__.py
--rw-r--r--   0        0        0     2117 2023-04-28 02:39:09.920354 teda-3.0.2/teda/command_line.py
--rw-r--r--   0        0        0     1958 2020-07-01 12:39:55.000000 teda-3.0.2/teda/console.py
--rw-r--r--   0        0        0     1531 2020-12-03 12:27:12.916427 teda-3.0.2/teda/draggingComponent.py
--rw-r--r--   0        0        0     2105 2020-04-22 14:55:56.000000 teda-3.0.2/teda/fitsopen.py
--rw-r--r--   0        0        0     2043 2020-05-20 13:57:09.000000 teda-3.0.2/teda/fitting.py
--rw-r--r--   0        0        0     2716 2020-07-01 13:22:36.000000 teda-3.0.2/teda/icons/1-2-24px.svg
--rw-r--r--   0        0        0     2238 2020-07-01 13:22:36.000000 teda-3.0.2/teda/icons/1-4-24px.svg
--rw-r--r--   0        0        0      298 2020-06-10 13:51:52.000000 teda-3.0.2/teda/icons/add_circle_outline-24px.svg
--rw-r--r--   0        0        0      380 2020-07-01 13:22:36.000000 teda-3.0.2/teda/icons/autopause-24px.svg
--rw-r--r--   0        0        0      222 2020-07-01 13:22:36.000000 teda-3.0.2/teda/icons/autopause_disabled-24px.svg
--rw-r--r--   0        0        0      262 2020-06-10 13:51:52.000000 teda-3.0.2/teda/icons/circle-24px.svg
--rw-r--r--   0        0        0      249 2020-07-01 13:22:36.000000 teda-3.0.2/teda/icons/count1-24px.svg
--rw-r--r--   0        0        0      315 2020-07-01 13:22:36.000000 teda-3.0.2/teda/icons/count2-24px.svg
--rw-r--r--   0        0        0      343 2020-07-01 13:22:36.000000 teda-3.0.2/teda/icons/count3-24px.svg
--rw-r--r--   0        0        0      270 2020-07-01 13:22:36.000000 teda-3.0.2/teda/icons/count4-24px.svg
--rw-r--r--   0        0        0      296 2020-07-01 13:22:36.000000 teda-3.0.2/teda/icons/count5-24px.svg
--rw-r--r--   0        0        0      349 2020-06-10 13:51:52.000000 teda-3.0.2/teda/icons/delete_forever-24px.svg
--rw-r--r--   0        0        0      518 2020-05-14 14:33:36.000000 teda-3.0.2/teda/icons/file-earmark-plus.svg
--rw-r--r--   0        0        0      402 2020-07-01 12:47:01.000000 teda-3.0.2/teda/icons/filter_alt-24px.svg
--rw-r--r--   0        0        0      257 2020-07-01 12:47:01.000000 teda-3.0.2/teda/icons/folder-24px.svg
--rw-r--r--   0        0        0      217 2020-06-08 17:33:08.000000 teda-3.0.2/teda/icons/home-24px.svg
--rw-r--r--   0        0        0      343 2020-06-08 17:32:29.000000 teda-3.0.2/teda/icons/house-24px.svg
--rw-r--r--   0        0        0      196 2020-06-08 17:30:35.000000 teda-3.0.2/teda/icons/keyboard_arrow_left-24px.svg
--rw-r--r--   0        0        0      194 2020-06-08 17:30:21.000000 teda-3.0.2/teda/icons/keyboard_arrow_right-24px.svg
--rw-r--r--   0        0        0      977 2020-06-05 15:03:11.000000 teda-3.0.2/teda/icons/new.png
--rw-r--r--   0        0        0      367 2020-06-10 13:51:52.000000 teda-3.0.2/teda/icons/not_started-24px.svg
--rw-r--r--   0        0        0      261 2020-06-08 17:13:41.000000 teda-3.0.2/teda/icons/note_add-24px.svg
--rw-r--r--   0        0        0      245 2020-07-01 13:22:36.000000 teda-3.0.2/teda/icons/panning-24px.svg
--rw-r--r--   0        0        0      292 2020-06-08 17:34:43.000000 teda-3.0.2/teda/icons/pause_circle_outline-24px.svg
--rw-r--r--   0        0        0      344 2020-07-01 12:47:01.000000 teda-3.0.2/teda/icons/photo_filter-24px.svg
--rw-r--r--   0        0        0      285 2020-06-08 17:34:37.000000 teda-3.0.2/teda/icons/play_circle_outline-24px.svg
--rw-r--r--   0        0        0      379 2020-07-01 12:39:55.000000 teda-3.0.2/teda/icons/push_pin-24px.svg
--rw-r--r--   0        0        0      304 2020-07-01 13:22:36.000000 teda-3.0.2/teda/icons/save-24px.svg
--rw-r--r--   0        0        0      203 2020-06-08 17:29:29.000000 teda-3.0.2/teda/icons/skip_next-24px.svg
--rw-r--r--   0        0        0      206 2020-06-08 17:29:33.000000 teda-3.0.2/teda/icons/skip_previous-24px.svg
--rw-r--r--   0        0        0     1245 2020-12-03 12:27:12.917053 teda-3.0.2/teda/icons/slider-24px.svg
--rw-r--r--   0        0        0      385 2020-06-08 17:34:40.000000 teda-3.0.2/teda/icons/stop_circle-24px.svg
--rw-r--r--   0        0        0     2638 2020-07-01 13:22:36.000000 teda-3.0.2/teda/icons/x2-24px.svg
--rw-r--r--   0        0        0     2159 2020-07-01 13:22:36.000000 teda-3.0.2/teda/icons/x4-24px.svg
--rw-r--r--   0        0        0      571 2023-04-28 02:39:09.916622 teda-3.0.2/teda/icons.py
--rw-r--r--   0        0        0        0 2020-06-04 14:08:12.000000 teda-3.0.2/teda/models/__init__.py
--rw-r--r--   0        0        0     1014 2020-06-04 10:29:56.000000 teda-3.0.2/teda/models/cmaps.py
--rw-r--r--   0        0        0     3002 2023-04-28 04:32:12.682801 teda-3.0.2/teda/models/coordinates.py
--rw-r--r--   0        0        0     5435 2020-12-02 21:00:51.002196 teda-3.0.2/teda/models/scalesModel.py
--rw-r--r--   0        0        0    16439 2023-04-28 03:24:57.907274 teda-3.0.2/teda/painterComponent.py
--rw-r--r--   0        0        0     2967 2023-04-28 02:39:09.864767 teda-3.0.2/teda/painterShapes/CircleCenterShape.py
--rw-r--r--   0        0        0        0 2020-06-04 11:27:56.000000 teda-3.0.2/teda/painterShapes/__init__.py
--rw-r--r--   0        0        0     1885 2023-04-28 02:39:09.885266 teda-3.0.2/teda/painterShapes/circleShape.py
--rw-r--r--   0        0        0     2227 2023-04-28 02:39:09.889630 teda-3.0.2/teda/painterShapes/rectangleMinatureShape.py
--rwxr-xr-x   0        0        0     1410 2023-04-28 02:57:03.732713 teda-3.0.2/teda/teda_fits.py
--rw-r--r--   0        0        0      123 2023-04-28 05:38:21.533025 teda-3.0.2/teda/version.py
--rw-r--r--   0        0        0    34219 2023-04-28 02:50:04.151992 teda-3.0.2/teda/viewer_mainwindow.py
--rw-r--r--   0        0        0        0 2020-06-04 14:07:28.000000 teda-3.0.2/teda/views/__init__.py
--rw-r--r--   0        0        0    17605 2023-04-28 03:13:13.702006 teda-3.0.2/teda/views/fitsplot.py
--rw-r--r--   0        0        0     2602 2020-12-03 12:21:15.958669 teda-3.0.2/teda/views/fitsplot_fitsfile.py
--rw-r--r--   0        0        0     2498 2020-12-02 21:00:51.007550 teda-3.0.2/teda/views/fitsplotcontrolled.py
--rw-r--r--   0        0        0     1143 2020-06-04 11:45:26.000000 teda-3.0.2/teda/views/fitsplotzoomed.py
--rw-r--r--   0        0        0        0 2020-06-04 14:10:29.000000 teda-3.0.2/teda/widgets/__init__.py
--rw-r--r--   0        0        0     6566 2023-04-28 05:36:33.166255 teda-3.0.2/teda/widgets/fileSystemWidget.py
--rw-r--r--   0        0        0     2976 2023-04-28 02:39:09.907291 teda-3.0.2/teda/widgets/fullViewWidget.py
--rw-r--r--   0        0        0     3270 2023-04-28 02:39:09.874014 teda-3.0.2/teda/widgets/headerTableWidget.py
--rw-r--r--   0        0        0     2295 2023-04-28 02:39:09.924105 teda-3.0.2/teda/widgets/info.py
--rw-r--r--   0        0        0     3293 2023-04-28 02:39:09.869422 teda-3.0.2/teda/widgets/radialprofile.py
--rw-r--r--   0        0        0     5299 2023-04-28 02:39:09.899380 teda-3.0.2/teda/widgets/radialprofileIRAF.py
--rw-r--r--   0        0        0    24353 2023-04-28 04:12:12.833462 teda-3.0.2/teda/widgets/scaleWidget.py
--rw-r--r--   0        0        0    12534 2023-04-28 02:48:42.836537 teda-3.0.2/teda/widgets/scanToolbar.py
--rw-r--r--   0        0        0     6207 2023-04-28 02:39:09.903950 teda-3.0.2/teda/widgets/slider.py
--rw-r--r--   0        0        0     1357 2023-04-28 02:39:09.895011 teda-3.0.2/teda/widgets/zoomViewWidget.py
--rw-r--r--   0        0        0    49708 1970-01-01 00:00:00.000000 teda-3.0.2/setup.py
--rw-r--r--   0        0        0     5439 1970-01-01 00:00:00.000000 teda-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2020-06-04 16:42:55.000000 teda-3.1.0/LICENSE
+-rw-r--r--   0        0        0     4719 2020-12-02 21:00:51.000070 teda-3.1.0/README.md
+-rw-r--r--   0        0        0      478 2023-05-29 11:14:23.668158 teda-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8196 2020-09-07 16:29:27.113605 teda-3.1.0/teda/.DS_Store
+-rw-r--r--   0        0        0       32 2020-06-04 16:24:35.000000 teda-3.1.0/teda/__init__.py
+-rw-r--r--   0        0        0     2116 2023-05-28 13:57:12.142317 teda-3.1.0/teda/command_line.py
+-rw-r--r--   0        0        0     1958 2020-07-01 12:39:55.000000 teda-3.1.0/teda/console.py
+-rw-r--r--   0        0        0     1531 2020-12-03 12:27:12.916427 teda-3.1.0/teda/draggingComponent.py
+-rw-r--r--   0        0        0     2105 2020-04-22 14:55:56.000000 teda-3.1.0/teda/fitsopen.py
+-rw-r--r--   0        0        0     2042 2023-05-29 09:48:43.095118 teda-3.1.0/teda/fitting.py
+-rw-r--r--   0        0        0     6148 2020-06-16 15:09:14.000000 teda-3.1.0/teda/icons/.DS_Store
+-rw-r--r--   0        0        0     2716 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/1-2-24px.svg
+-rw-r--r--   0        0        0     2238 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/1-4-24px.svg
+-rw-r--r--   0        0        0      298 2020-06-10 13:51:52.000000 teda-3.1.0/teda/icons/add_circle_outline-24px.svg
+-rw-r--r--   0        0        0      380 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/autopause-24px.svg
+-rw-r--r--   0        0        0      222 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/autopause_disabled-24px.svg
+-rw-r--r--   0        0        0      262 2020-06-10 13:51:52.000000 teda-3.1.0/teda/icons/circle-24px.svg
+-rw-r--r--   0        0        0      249 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/count1-24px.svg
+-rw-r--r--   0        0        0      315 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/count2-24px.svg
+-rw-r--r--   0        0        0      343 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/count3-24px.svg
+-rw-r--r--   0        0        0      270 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/count4-24px.svg
+-rw-r--r--   0        0        0      296 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/count5-24px.svg
+-rw-r--r--   0        0        0      349 2020-06-10 13:51:52.000000 teda-3.1.0/teda/icons/delete_forever-24px.svg
+-rw-r--r--   0        0        0      518 2020-05-14 14:33:36.000000 teda-3.1.0/teda/icons/file-earmark-plus.svg
+-rw-r--r--   0        0        0      402 2020-07-01 12:47:01.000000 teda-3.1.0/teda/icons/filter_alt-24px.svg
+-rw-r--r--   0        0        0      257 2020-07-01 12:47:01.000000 teda-3.1.0/teda/icons/folder-24px.svg
+-rw-r--r--   0        0        0      217 2020-06-08 17:33:08.000000 teda-3.1.0/teda/icons/home-24px.svg
+-rw-r--r--   0        0        0      343 2020-06-08 17:32:29.000000 teda-3.1.0/teda/icons/house-24px.svg
+-rw-r--r--   0        0        0      196 2020-06-08 17:30:35.000000 teda-3.1.0/teda/icons/keyboard_arrow_left-24px.svg
+-rw-r--r--   0        0        0      194 2020-06-08 17:30:21.000000 teda-3.1.0/teda/icons/keyboard_arrow_right-24px.svg
+-rw-r--r--   0        0        0      977 2020-06-05 15:03:11.000000 teda-3.1.0/teda/icons/new.png
+-rw-r--r--   0        0        0      367 2020-06-10 13:51:52.000000 teda-3.1.0/teda/icons/not_started-24px.svg
+-rw-r--r--   0        0        0      261 2020-06-08 17:13:41.000000 teda-3.1.0/teda/icons/note_add-24px.svg
+-rw-r--r--   0        0        0      245 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/panning-24px.svg
+-rw-r--r--   0        0        0      292 2020-06-08 17:34:43.000000 teda-3.1.0/teda/icons/pause_circle_outline-24px.svg
+-rw-r--r--   0        0        0      344 2020-07-01 12:47:01.000000 teda-3.1.0/teda/icons/photo_filter-24px.svg
+-rw-r--r--   0        0        0      285 2020-06-08 17:34:37.000000 teda-3.1.0/teda/icons/play_circle_outline-24px.svg
+-rw-r--r--   0        0        0      379 2020-07-01 12:39:55.000000 teda-3.1.0/teda/icons/push_pin-24px.svg
+-rw-r--r--   0        0        0      333 2023-05-28 16:06:33.651338 teda-3.1.0/teda/icons/refresh-24px.svg
+-rw-r--r--   0        0        0      304 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/save-24px.svg
+-rw-r--r--   0        0        0      203 2020-06-08 17:29:29.000000 teda-3.1.0/teda/icons/skip_next-24px.svg
+-rw-r--r--   0        0        0      206 2020-06-08 17:29:33.000000 teda-3.1.0/teda/icons/skip_previous-24px.svg
+-rw-r--r--   0        0        0     1245 2020-12-03 12:27:12.917053 teda-3.1.0/teda/icons/slider-24px.svg
+-rw-r--r--   0        0        0      295 2023-05-29 09:17:04.891965 teda-3.1.0/teda/icons/sort-24px.svg
+-rw-r--r--   0        0        0      385 2020-06-08 17:34:40.000000 teda-3.1.0/teda/icons/stop_circle-24px.svg
+-rw-r--r--   0        0        0     2638 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/x2-24px.svg
+-rw-r--r--   0        0        0     2159 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/x4-24px.svg
+-rw-r--r--   0        0        0      571 2023-04-28 02:39:09.916622 teda-3.1.0/teda/icons.py
+-rw-r--r--   0        0        0        0 2020-06-04 14:08:12.000000 teda-3.1.0/teda/models/__init__.py
+-rw-r--r--   0        0        0      163 2023-04-27 22:41:43.996886 teda-3.1.0/teda/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      141 2020-06-04 14:13:27.000000 teda-3.1.0/teda/models/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     2415 2023-04-27 22:42:14.936963 teda-3.1.0/teda/models/__pycache__/cmaps.cpython-311.pyc
+-rw-r--r--   0        0        0     1444 2020-06-04 14:13:27.000000 teda-3.1.0/teda/models/__pycache__/cmaps.cpython-37.pyc
+-rw-r--r--   0        0        0     5832 2023-04-28 04:32:52.894102 teda-3.1.0/teda/models/__pycache__/coordinates.cpython-311.pyc
+-rw-r--r--   0        0        0     3346 2020-12-03 12:42:28.079005 teda-3.1.0/teda/models/__pycache__/coordinates.cpython-37.pyc
+-rw-r--r--   0        0        0     5448 2023-04-27 22:41:43.998909 teda-3.1.0/teda/models/__pycache__/scalesModel.cpython-311.pyc
+-rw-r--r--   0        0        0     3219 2020-12-02 23:53:51.561303 teda-3.1.0/teda/models/__pycache__/scalesModel.cpython-37.pyc
+-rw-r--r--   0        0        0     3792 2020-12-03 12:42:28.214696 teda-3.1.0/teda/models/__pycache__/shapes_group.cpython-37.pyc
+-rw-r--r--   0        0        0        0 2023-05-28 16:18:53.841906 teda-3.1.0/teda/models/aaa.tmp
+-rw-r--r--   0        0        0     1014 2020-06-04 10:29:56.000000 teda-3.1.0/teda/models/cmaps.py
+-rw-r--r--   0        0        0     3002 2023-04-28 04:32:12.682801 teda-3.1.0/teda/models/coordinates.py
+-rw-r--r--   0        0        0     5435 2020-12-02 21:00:51.002196 teda-3.1.0/teda/models/scalesModel.py
+-rw-r--r--   0        0        0        0 2023-05-28 16:19:13.093531 teda-3.1.0/teda/models/zzz.tmp
+-rw-r--r--   0        0        0    16439 2023-04-28 03:24:57.907274 teda-3.1.0/teda/painterComponent.py
+-rw-r--r--   0        0        0     2967 2023-04-28 02:39:09.864767 teda-3.1.0/teda/painterShapes/CircleCenterShape.py
+-rw-r--r--   0        0        0        0 2020-06-04 11:27:56.000000 teda-3.1.0/teda/painterShapes/__init__.py
+-rw-r--r--   0        0        0     6220 2023-04-28 02:47:29.368730 teda-3.1.0/teda/painterShapes/__pycache__/CircleCenterShape.cpython-311.pyc
+-rw-r--r--   0        0        0     3410 2020-06-04 11:53:07.000000 teda-3.1.0/teda/painterShapes/__pycache__/CircleCenterShape.cpython-37.pyc
+-rw-r--r--   0        0        0      170 2023-04-27 22:41:44.734595 teda-3.1.0/teda/painterShapes/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      148 2020-06-04 11:53:07.000000 teda-3.1.0/teda/painterShapes/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     4007 2023-04-28 02:47:29.366538 teda-3.1.0/teda/painterShapes/__pycache__/circleShape.cpython-311.pyc
+-rw-r--r--   0        0        0     2626 2020-12-03 13:28:14.814864 teda-3.1.0/teda/painterShapes/__pycache__/circleShape.cpython-37.pyc
+-rw-r--r--   0        0        0     4369 2023-04-28 02:47:29.370222 teda-3.1.0/teda/painterShapes/__pycache__/rectangleMinatureShape.cpython-311.pyc
+-rw-r--r--   0        0        0     2977 2020-06-04 11:53:07.000000 teda-3.1.0/teda/painterShapes/__pycache__/rectangleMinatureShape.cpython-37.pyc
+-rw-r--r--   0        0        0     1885 2023-04-28 02:39:09.885266 teda-3.1.0/teda/painterShapes/circleShape.py
+-rw-r--r--   0        0        0     2227 2023-04-28 02:39:09.889630 teda-3.1.0/teda/painterShapes/rectangleMinatureShape.py
+-rwxr-xr-x   0        0        0     1410 2023-04-28 02:57:03.732713 teda-3.1.0/teda/teda_fits.py
+-rw-r--r--   0        0        0      123 2023-05-29 11:13:55.600540 teda-3.1.0/teda/version.py
+-rw-r--r--   0        0        0    34360 2023-05-29 09:52:50.872380 teda-3.1.0/teda/viewer_mainwindow.py
+-rw-r--r--   0        0        0        0 2020-06-04 14:07:28.000000 teda-3.1.0/teda/views/__init__.py
+-rw-r--r--   0        0        0      162 2023-04-27 22:41:33.450750 teda-3.1.0/teda/views/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      140 2020-06-04 14:13:26.000000 teda-3.1.0/teda/views/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0    27001 2023-04-28 03:13:18.985069 teda-3.1.0/teda/views/__pycache__/fitsplot.cpython-311.pyc
+-rw-r--r--   0        0        0    13679 2020-12-02 23:53:51.217493 teda-3.1.0/teda/views/__pycache__/fitsplot.cpython-37.pyc
+-rw-r--r--   0        0        0     5676 2023-05-29 09:30:58.321016 teda-3.1.0/teda/views/__pycache__/fitsplot_fitsfile.cpython-311.pyc
+-rw-r--r--   0        0        0     2895 2020-12-03 12:42:28.076708 teda-3.1.0/teda/views/__pycache__/fitsplot_fitsfile.cpython-37.pyc
+-rw-r--r--   0        0        0     4376 2023-04-27 22:41:44.002790 teda-3.1.0/teda/views/__pycache__/fitsplotcontrolled.cpython-311.pyc
+-rw-r--r--   0        0        0     2621 2020-12-02 23:53:51.563344 teda-3.1.0/teda/views/__pycache__/fitsplotcontrolled.cpython-37.pyc
+-rw-r--r--   0        0        0     2325 2023-04-27 22:42:14.915899 teda-3.1.0/teda/views/__pycache__/fitsplotzoomed.cpython-311.pyc
+-rw-r--r--   0        0        0     1419 2020-06-04 14:13:27.000000 teda-3.1.0/teda/views/__pycache__/fitsplotzoomed.cpython-37.pyc
+-rw-r--r--   0        0        0    17605 2023-04-28 03:13:13.702006 teda-3.1.0/teda/views/fitsplot.py
+-rw-r--r--   0        0        0     2856 2023-05-29 09:27:03.636226 teda-3.1.0/teda/views/fitsplot_fitsfile.py
+-rw-r--r--   0        0        0     2498 2020-12-02 21:00:51.007550 teda-3.1.0/teda/views/fitsplotcontrolled.py
+-rw-r--r--   0        0        0     1143 2020-06-04 11:45:26.000000 teda-3.1.0/teda/views/fitsplotzoomed.py
+-rw-r--r--   0        0        0        0 2020-06-04 14:10:29.000000 teda-3.1.0/teda/widgets/__init__.py
+-rw-r--r--   0        0        0      164 2023-04-27 22:42:14.909974 teda-3.1.0/teda/widgets/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      142 2020-06-04 14:13:27.000000 teda-3.1.0/teda/widgets/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0    16801 2023-05-29 11:27:40.997985 teda-3.1.0/teda/widgets/__pycache__/fileSystemWidget.cpython-311.pyc
+-rw-r--r--   0        0        0     5546 2020-12-03 13:28:14.901959 teda-3.1.0/teda/widgets/__pycache__/fileSystemWidget.cpython-37.pyc
+-rw-r--r--   0        0        0     4931 2023-04-28 02:47:51.449604 teda-3.1.0/teda/widgets/__pycache__/fullViewWidget.cpython-311.pyc
+-rw-r--r--   0        0        0     2462 2020-06-04 14:13:27.000000 teda-3.1.0/teda/widgets/__pycache__/fullViewWidget.cpython-37.pyc
+-rw-r--r--   0        0        0     7076 2023-04-28 02:47:51.457738 teda-3.1.0/teda/widgets/__pycache__/headerTableWidget.cpython-311.pyc
+-rw-r--r--   0        0        0     3338 2020-07-01 12:05:10.000000 teda-3.1.0/teda/widgets/__pycache__/headerTableWidget.cpython-37.pyc
+-rw-r--r--   0        0        0     5518 2023-04-28 02:48:50.345439 teda-3.1.0/teda/widgets/__pycache__/info.cpython-311.pyc
+-rw-r--r--   0        0        0     2716 2020-12-03 13:28:14.900070 teda-3.1.0/teda/widgets/__pycache__/info.cpython-37.pyc
+-rw-r--r--   0        0        0     6042 2023-04-28 02:47:51.447525 teda-3.1.0/teda/widgets/__pycache__/radialprofile.cpython-311.pyc
+-rw-r--r--   0        0        0     3310 2020-06-06 15:32:49.000000 teda-3.1.0/teda/widgets/__pycache__/radialprofile.cpython-37.pyc
+-rw-r--r--   0        0        0     8717 2023-05-29 10:59:20.013231 teda-3.1.0/teda/widgets/__pycache__/radialprofileIRAF.cpython-311.pyc
+-rw-r--r--   0        0        0     4754 2020-06-16 14:25:09.000000 teda-3.1.0/teda/widgets/__pycache__/radialprofileIRAF.cpython-37.pyc
+-rw-r--r--   0        0        0     5923 2020-12-03 12:42:28.423269 teda-3.1.0/teda/widgets/__pycache__/regionsWidget.cpython-37.pyc
+-rw-r--r--   0        0        0    41551 2023-04-28 04:13:26.808651 teda-3.1.0/teda/widgets/__pycache__/scaleWidget.cpython-311.pyc
+-rw-r--r--   0        0        0    17990 2020-12-03 13:28:14.896657 teda-3.1.0/teda/widgets/__pycache__/scaleWidget.cpython-37.pyc
+-rw-r--r--   0        0        0    20348 2023-04-28 02:48:50.342163 teda-3.1.0/teda/widgets/__pycache__/scanToolbar.cpython-311.pyc
+-rw-r--r--   0        0        0     9700 2020-07-01 13:54:40.000000 teda-3.1.0/teda/widgets/__pycache__/scanToolbar.cpython-37.pyc
+-rw-r--r--   0        0        0    12512 2023-04-28 02:47:51.468296 teda-3.1.0/teda/widgets/__pycache__/slider.cpython-311.pyc
+-rw-r--r--   0        0        0     6731 2020-12-02 23:53:51.755329 teda-3.1.0/teda/widgets/__pycache__/slider.cpython-37.pyc
+-rw-r--r--   0        0        0     2853 2023-04-28 02:47:51.451127 teda-3.1.0/teda/widgets/__pycache__/zoomViewWidget.cpython-311.pyc
+-rw-r--r--   0        0        0     1605 2020-06-04 14:13:27.000000 teda-3.1.0/teda/widgets/__pycache__/zoomViewWidget.cpython-37.pyc
+-rw-r--r--   0        0        0     8342 2023-05-29 11:27:30.901972 teda-3.1.0/teda/widgets/fileSystemWidget.py
+-rw-r--r--   0        0        0     2976 2023-04-28 02:39:09.907291 teda-3.1.0/teda/widgets/fullViewWidget.py
+-rw-r--r--   0        0        0     3270 2023-04-28 02:39:09.874014 teda-3.1.0/teda/widgets/headerTableWidget.py
+-rw-r--r--   0        0        0     2295 2023-04-28 02:39:09.924105 teda-3.1.0/teda/widgets/info.py
+-rw-r--r--   0        0        0     3293 2023-04-28 02:39:09.869422 teda-3.1.0/teda/widgets/radialprofile.py
+-rw-r--r--   0        0        0     5546 2023-05-29 10:58:34.283016 teda-3.1.0/teda/widgets/radialprofileIRAF.py
+-rw-r--r--   0        0        0    24353 2023-04-28 04:12:12.833462 teda-3.1.0/teda/widgets/scaleWidget.py
+-rw-r--r--   0        0        0    12534 2023-04-28 02:48:42.836537 teda-3.1.0/teda/widgets/scanToolbar.py
+-rw-r--r--   0        0        0     6207 2023-04-28 02:39:09.903950 teda-3.1.0/teda/widgets/slider.py
+-rw-r--r--   0        0        0     1357 2023-04-28 02:39:09.895011 teda-3.1.0/teda/widgets/zoomViewWidget.py
+-rw-r--r--   0        0        0     5758 1970-01-01 00:00:00.000000 teda-3.1.0/setup.py
+-rw-r--r--   0        0        0     5381 1970-01-01 00:00:00.000000 teda-3.1.0/PKG-INFO
```

### Comparing `teda-3.0.2/LICENSE` & `teda-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/README.md` & `teda-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/command_line.py` & `teda-3.1.0/teda/command_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     def parseCommandLine(self, parser):    # QCommandLineParser
 
         parser.setApplicationDescription(QApplication.applicationName())
         parser.setSingleDashWordOptionMode(QCommandLineParser.ParseAsLongOptions)
 
         model = QStringListModel(["i", "ignore-settings"])
-        ignoreSettingsOption = QCommandLineOption (model.stringList(), "Ingnore settings file")
+        ignoreSettingsOption = QCommandLineOption (model.stringList(), "Ignore settings file")
         parser.addOption(ignoreSettingsOption)
 
         model = QStringListModel(["f", "file"])
         openFileOption = QCommandLineOption(model.stringList(), "Open file", "file")
         parser.addOption(openFileOption)
 
         helpOption = parser.addHelpOption()
```

### Comparing `teda-3.0.2/teda/console.py` & `teda-3.1.0/teda/console.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/draggingComponent.py` & `teda-3.1.0/teda/draggingComponent.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/fitsopen.py` & `teda-3.1.0/teda/fitsopen.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/fitting.py` & `teda-3.1.0/teda/fitting.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,16 +49,16 @@
     # gauss = lambda xy, a, c, mu_x, mu_y, sig2: c + a * np.exp(-((mu_x - xy[0])** 2 + (mu_y - xy[1])** 2) / (2 * sig2))
 
     minimal = np.nanmin(values)
     maximal = np.nanmax(values)
     opt, cov = optimize.curve_fit(gauss, xy, values,
                                   p0=[maximal - minimal, minimal, initial_mu[0], initial_mu[1], 1.0],
                                   bounds=(
-                                      [0.0, -np.inf, initial_mu[0]-mu_radius[0], initial_mu[1]-mu_radius[1], -np.inf],
-                                      [ np.inf,  np.inf, initial_mu[0]+mu_radius[0], initial_mu[1]+mu_radius[1],  np.inf])
+                                      [0.0,     -2.0**18, initial_mu[0]-mu_radius[0], initial_mu[1]-mu_radius[1], 0.0],
+                                      [2.0**19,  2.0**18, initial_mu[0]+mu_radius[0], initial_mu[1]+mu_radius[1], 1e10])
                                   )
     res = (gauss(xy, *opt) - values)
     rmse = math.sqrt((res * res).sum() / len(values)),
     try:
         sig = math.sqrt(opt[4])
     except ValueError:
         sig = 0
```

### Comparing `teda-3.0.2/teda/icons/1-2-24px.svg` & `teda-3.1.0/teda/icons/1-2-24px.svg`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/icons/1-4-24px.svg` & `teda-3.1.0/teda/icons/1-4-24px.svg`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/icons/file-earmark-plus.svg` & `teda-3.1.0/teda/icons/file-earmark-plus.svg`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/icons/new.png` & `teda-3.1.0/teda/icons/new.png`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/icons/slider-24px.svg` & `teda-3.1.0/teda/icons/slider-24px.svg`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/icons/x2-24px.svg` & `teda-3.1.0/teda/icons/x2-24px.svg`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/icons/x4-24px.svg` & `teda-3.1.0/teda/icons/x4-24px.svg`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/icons.py` & `teda-3.1.0/teda/icons.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/models/cmaps.py` & `teda-3.1.0/teda/models/cmaps.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/models/coordinates.py` & `teda-3.1.0/teda/models/coordinates.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/models/scalesModel.py` & `teda-3.1.0/teda/models/scalesModel.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/painterComponent.py` & `teda-3.1.0/teda/painterComponent.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/painterShapes/CircleCenterShape.py` & `teda-3.1.0/teda/painterShapes/CircleCenterShape.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/painterShapes/circleShape.py` & `teda-3.1.0/teda/painterShapes/circleShape.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/painterShapes/rectangleMinatureShape.py` & `teda-3.1.0/teda/painterShapes/rectangleMinatureShape.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/teda_fits.py` & `teda-3.1.0/teda/teda_fits.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/viewer_mainwindow.py` & `teda-3.1.0/teda/viewer_mainwindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,18 @@
             settings = QSettings()
             settings.beginGroup("Files")
             filename = settings.value("lastFile")
             settings.endGroup()
         else:
             filename = self.tedaCommandLine.openFile
         if filename:
-            self.open_fits(filename)
+            try:
+                self.open_fits(filename)
+            except (FileNotFoundError, OSError) as e:
+                print(f'Error opening last file {filename}: {e}')
 
     def readAppState(self):
         if self.tedaCommandLine.ignoreSettings:
             return
         settings = QSettings()
         settings.beginGroup("WCS")
         self.wcsSexAct.setChecked(bool(settings.value("sexagesimal", True)))
```

### Comparing `teda-3.0.2/teda/views/fitsplot.py` & `teda-3.1.0/teda/views/fitsplot.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/views/fitsplot_fitsfile.py` & `teda-3.1.0/teda/views/fitsplot_fitsfile.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import logging
 from astropy.io import fits
 from astropy.io.fits.hdu import(PrimaryHDU, ImageHDU)
 import traitlets as tr
 
 from .fitsplotcontrolled import FitsPlotterControlled
 
+logger = logging.getLogger(__name__.rsplit('.')[-1])
+
 
 class FitsPlotterFitsFile(FitsPlotterControlled):
 
     fitsfile = tr.Unicode(allow_none=True)
 
     def __init__(self, fitsfile=None, hdu=0, figure=None, ax=None, interval=None, intervalkwargs=None, stretch=None,
                  stretchkwargs=None, cmap_model=None, scale_model=None):
@@ -30,16 +33,19 @@
     def open(self):
         if self._huds is None and self.fitsfile:
             self._huds = fits.open(self.fitsfile, lazy_load_hdus=False)
             self._huds.info()
 
     def set_file(self, filename):
         if filename is not None:
-            self._huds = fits.open(filename, lazy_load_hdus=False)
-            self._huds.info()
+            try:
+                self._huds = fits.open(filename, lazy_load_hdus=False)
+                self._huds.info()
+            except (FileNotFoundError, OSError) as e:
+                logger.error(f'Can not open file {filename}: {e}')
         else:
             self._huds = None
         self.fitsfile = filename
 
     @data.setter
     def data(self, d):
         raise TypeError('Can not set data directly in FitsPlotterFitsFile. Set fits file instead')
@@ -72,18 +78,18 @@
         except AttributeError: # ax is None or not WCSAxies
             pass
 
     def isFitsFile(self,filename,showinfo = True):
         try:
             fits.open(filename)
             return True
-        except FileNotFoundError:
+        except FileNotFoundError as e:
             if showinfo:
-                print('Błąd w odczycie pliku')
+                logger.error(f'Can not find file {filename}: {e}')
             return False
-        except OSError:
+        except OSError as e:
             if showinfo:
-                print('Pusty lub błedny format pliku')
+                logger.error(f'Can not open file {filename}: {e}')
             return False
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `teda-3.0.2/teda/views/fitsplotcontrolled.py` & `teda-3.1.0/teda/views/fitsplotcontrolled.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/views/fitsplotzoomed.py` & `teda-3.1.0/teda/views/fitsplotzoomed.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/widgets/fileSystemWidget.py` & `teda-3.1.0/teda/widgets/fileSystemWidget.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,55 @@
 from PySide6.QtCore import QDir
 from PySide6.QtGui import Qt, QAction
 from PySide6.QtWidgets import QWidget, QHBoxLayout, QFileSystemModel, QTreeView, QListView, QVBoxLayout, \
-    QPushButton, QToolButton, QFileDialog, QSplitter
+    QPushButton, QToolButton, QFileDialog, QSplitter, QApplication
 
 from teda.icons import IconFactory
 
 
 class FileSystemWidget(QWidget):
 
     def __init__(self, parent, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.currentRootPath = '/'
         self.currentPath = QDir.currentPath()
 
-        self.mainWindow = parent;
+        self.mainWindow = parent
 
         self.chooseDirAction = QAction(IconFactory.getIcon('folder'), 'Root directory', self, statusTip="Change root directory", triggered=self.chooseRootDir)
+
         self.showOFAction = QAction(IconFactory.getIcon('filter_alt'), 'Show only FITS files', self, statusTip="Show only FITS/all files", triggered=self.showOFFiles)
         self.showOFAction.setCheckable(True)
-        self.showOFAction.toggled.connect(self.showOFFiles)
+        # self.showOFAction.toggled.connect(self.showOFFiles)
+
+        self.refreshFilesAction = QAction(IconFactory.getIcon('refresh'), 'Auto-refresh files', self, statusTip="Auto-refresh on new files", triggered=self.refreshFiles)
+        self.refreshFilesAction.setCheckable(True)
+
+        self.sortFilesAction = QAction(IconFactory.getIcon('sort'), 'Reverse file sort', self, statusTip="Ascending/Descending sort of files (by name)", triggered=self.sortFiles)
+        self.sortFilesAction.setCheckable(True)
 
         self.chooseDirBtn = QToolButton()
         self.chooseDirBtn.setDefaultAction(self.chooseDirAction)
 
         self.showOFBtn = QToolButton()
         self.showOFBtn.setDefaultAction(self.showOFAction)
 
+        self.refreshFilesBtn = QToolButton()
+        self.refreshFilesBtn.setDefaultAction(self.refreshFilesAction)
+
+        self.sortFilesBtn = QToolButton()
+        self.sortFilesBtn.setDefaultAction(self.sortFilesAction)
 
         iconlayout = QHBoxLayout()
         iconlayout.setAlignment(Qt.AlignLeft)
         iconlayout.addWidget(self.chooseDirBtn)
         iconlayout.addWidget(self.showOFBtn)
+        iconlayout.addWidget(self.refreshFilesBtn)
+        iconlayout.addWidget(self.sortFilesBtn)
 
         self.viewsSplitter = QSplitter(Qt.Horizontal)
         self.viewsSplitter.splitterMoved.connect(self.splitterMoved)
 
         self.dirsModel = QFileSystemModel(self)
         self.dirsModel.setOption(QFileSystemModel.DontWatchForChanges, True)
         self.dirsModel.setFilter(QDir.NoDotAndDotDot | QDir.AllDirs)
@@ -47,14 +61,15 @@
 
         self.dirs.clicked.connect(self.onDirsClick)
         self.dirs.doubleClicked.connect(self.onDirsDoubleClick)
 
         self.filesModel = QFileSystemModel(self)
         self.filesModel.setOption(QFileSystemModel.DontWatchForChanges, True)
         self.filesModel.setFilter(QDir.NoDotAndDotDot | QDir.Files)
+        self.filesModel.sort(0, Qt.AscendingOrder)
         self.filesModel.setNameFilterDisables(False)
 
         self.files = QListView()
         self.files.setModel(self.filesModel)
         self.files.doubleClicked.connect(self.onFilesDoubleClick)
 
         self.viewsSplitter.addWidget(self.dirs)
@@ -140,33 +155,55 @@
         if self.showOFAction.isChecked():
             self.dirsModel.setNameFilters(["*.FITS", "*.fits"])
             self.filesModel.setNameFilters(["*.FITS", "*.fits"])
         else:
             self.dirsModel.setNameFilters(["*"])
             self.filesModel.setNameFilters(["*"])
 
+    def refreshFiles(self):
+        if self.refreshFilesAction.isChecked():
+            self.filesModel.setOption(QFileSystemModel.DontWatchForChanges, False)
+        else:
+            self.filesModel.setOption(QFileSystemModel.DontWatchForChanges, True)
+
+    def sortFiles(self):
+        if self.sortFilesAction.isChecked():
+            self.filesModel.sort(0, Qt.DescendingOrder)
+        else:
+            self.filesModel.sort(0, Qt.AscendingOrder)
+
     def writeSettings(self, settings):
         settings.beginGroup("fileWidget")
         settings.setValue('splitterGeometry',self.viewsSplitter.saveGeometry())
         settings.setValue('splitterState',self.viewsSplitter.saveState())
         settings.setValue('rootPath',self.currentRootPath)
         settings.setValue('path',self.currentPath)
+        settings.setValue('showOF',self.showOFAction.isChecked())
+        settings.setValue('refresh',self.refreshFilesAction.isChecked())
+        settings.setValue('sort',self.sortFilesAction.isChecked())
         settings.endGroup()
 
     def readSettings(self, settings):
         settings.beginGroup("fileWidget")
         self.viewsSplitter.restoreGeometry(settings.value("splitterGeometry"))
         self.viewsSplitter.restoreState(settings.value("splitterState"))
         rootPath = settings.value("rootPath")
         path = settings.value("path")
+        self.showOFAction.setChecked(settings.value("showOF"))
+        self.refreshFilesAction.setChecked(settings.value("refresh"))
+        self.sortFilesAction.setChecked(settings.value("sort"))
         settings.endGroup()
 
         if rootPath is None:
             rootPath = '/'
         self.setRootPath(rootPath)
 
         if path is None:
             path = QDir.currentPath()
         self.setPath(path)
 
         self.splitterMoved(self.viewsSplitter.handle(1).pos().x(), 0)
 
+        self.showOFFiles()
+        self.refreshFiles()
+        self.sortFiles()
+
```

### Comparing `teda-3.0.2/teda/widgets/fullViewWidget.py` & `teda-3.1.0/teda/widgets/fullViewWidget.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/widgets/headerTableWidget.py` & `teda-3.1.0/teda/widgets/headerTableWidget.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/widgets/info.py` & `teda-3.1.0/teda/widgets/info.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/widgets/radialprofile.py` & `teda-3.1.0/teda/widgets/radialprofile.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/widgets/radialprofileIRAF.py` & `teda-3.1.0/teda/widgets/radialprofileIRAF.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,19 @@
         -------
         x_linespace, y_fit, rmse, fwhm, sky
         """
         # mu=0 gaussian + constant
         x, y = np.asarray(x), np.asarray(y)
         gauss0 = lambda x, a, c, sig2: c + a * np.exp(-x**2/(2*sig2))
 
-        opt, cov = optimize.curve_fit(gauss0, x, y, p0=[1.0, 0.0, 1.0])
+        opt, cov = optimize.curve_fit(gauss0, x, y, p0=[1.0, 0.0, 1.0],
+                                      bounds=([-2.0**19, -2.0**16, 0.0],
+                                              [2.0**19,   2.0**16, 70]  # max fwhm=20
+                                              )
+                                      )
         res = gauss0(x, *opt) - y
         rmse = math.sqrt((res*res).sum()/len(res))
         try:
             fwhm = 2.355 * math.sqrt(opt[2])
         except ValueError:
             fwhm = 0
         sky = opt[1]
```

### Comparing `teda-3.0.2/teda/widgets/scaleWidget.py` & `teda-3.1.0/teda/widgets/scaleWidget.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/widgets/scanToolbar.py` & `teda-3.1.0/teda/widgets/scanToolbar.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/widgets/slider.py` & `teda-3.1.0/teda/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/teda/widgets/zoomViewWidget.py` & `teda-3.1.0/teda/widgets/zoomViewWidget.py`

 * *Files identical despite different names*

### Comparing `teda-3.0.2/PKG-INFO` & `teda-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: teda
-Version: 3.0.2
+Version: 3.1.0
 Summary: Yet Another FITS Viewer
 License: MIT
 Author: majkelx
 Author-email: mkalusz@camk.edu.pl
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: astropy (>=5.2.2,<6.0.0)
+Requires-Dist: astropy (>5.2.2)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: pyside6 (>=6.5.0,<7.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: traitlets (>=5.9.0,<6.0.0)
 Description-Content-Type: text/markdown
 
 # TeDa FITS Viewer
```

