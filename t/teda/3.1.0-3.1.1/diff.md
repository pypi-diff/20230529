# Comparing `tmp/teda-3.1.0.tar.gz` & `tmp/teda-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teda-3.1.0.tar", max compression
+gzip compressed data, was "teda-3.1.1.tar", max compression
```

## Comparing `teda-3.1.0.tar` & `teda-3.1.1.tar`

### file list

```diff
@@ -1,130 +1,130 @@
--rw-r--r--   0        0        0     1066 2020-06-04 16:42:55.000000 teda-3.1.0/LICENSE
--rw-r--r--   0        0        0     4719 2020-12-02 21:00:51.000070 teda-3.1.0/README.md
--rw-r--r--   0        0        0      478 2023-05-29 11:14:23.668158 teda-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     8196 2020-09-07 16:29:27.113605 teda-3.1.0/teda/.DS_Store
--rw-r--r--   0        0        0       32 2020-06-04 16:24:35.000000 teda-3.1.0/teda/__init__.py
--rw-r--r--   0        0        0     2116 2023-05-28 13:57:12.142317 teda-3.1.0/teda/command_line.py
--rw-r--r--   0        0        0     1958 2020-07-01 12:39:55.000000 teda-3.1.0/teda/console.py
--rw-r--r--   0        0        0     1531 2020-12-03 12:27:12.916427 teda-3.1.0/teda/draggingComponent.py
--rw-r--r--   0        0        0     2105 2020-04-22 14:55:56.000000 teda-3.1.0/teda/fitsopen.py
--rw-r--r--   0        0        0     2042 2023-05-29 09:48:43.095118 teda-3.1.0/teda/fitting.py
--rw-r--r--   0        0        0     6148 2020-06-16 15:09:14.000000 teda-3.1.0/teda/icons/.DS_Store
--rw-r--r--   0        0        0     2716 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/1-2-24px.svg
--rw-r--r--   0        0        0     2238 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/1-4-24px.svg
--rw-r--r--   0        0        0      298 2020-06-10 13:51:52.000000 teda-3.1.0/teda/icons/add_circle_outline-24px.svg
--rw-r--r--   0        0        0      380 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/autopause-24px.svg
--rw-r--r--   0        0        0      222 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/autopause_disabled-24px.svg
--rw-r--r--   0        0        0      262 2020-06-10 13:51:52.000000 teda-3.1.0/teda/icons/circle-24px.svg
--rw-r--r--   0        0        0      249 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/count1-24px.svg
--rw-r--r--   0        0        0      315 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/count2-24px.svg
--rw-r--r--   0        0        0      343 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/count3-24px.svg
--rw-r--r--   0        0        0      270 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/count4-24px.svg
--rw-r--r--   0        0        0      296 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/count5-24px.svg
--rw-r--r--   0        0        0      349 2020-06-10 13:51:52.000000 teda-3.1.0/teda/icons/delete_forever-24px.svg
--rw-r--r--   0        0        0      518 2020-05-14 14:33:36.000000 teda-3.1.0/teda/icons/file-earmark-plus.svg
--rw-r--r--   0        0        0      402 2020-07-01 12:47:01.000000 teda-3.1.0/teda/icons/filter_alt-24px.svg
--rw-r--r--   0        0        0      257 2020-07-01 12:47:01.000000 teda-3.1.0/teda/icons/folder-24px.svg
--rw-r--r--   0        0        0      217 2020-06-08 17:33:08.000000 teda-3.1.0/teda/icons/home-24px.svg
--rw-r--r--   0        0        0      343 2020-06-08 17:32:29.000000 teda-3.1.0/teda/icons/house-24px.svg
--rw-r--r--   0        0        0      196 2020-06-08 17:30:35.000000 teda-3.1.0/teda/icons/keyboard_arrow_left-24px.svg
--rw-r--r--   0        0        0      194 2020-06-08 17:30:21.000000 teda-3.1.0/teda/icons/keyboard_arrow_right-24px.svg
--rw-r--r--   0        0        0      977 2020-06-05 15:03:11.000000 teda-3.1.0/teda/icons/new.png
--rw-r--r--   0        0        0      367 2020-06-10 13:51:52.000000 teda-3.1.0/teda/icons/not_started-24px.svg
--rw-r--r--   0        0        0      261 2020-06-08 17:13:41.000000 teda-3.1.0/teda/icons/note_add-24px.svg
--rw-r--r--   0        0        0      245 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/panning-24px.svg
--rw-r--r--   0        0        0      292 2020-06-08 17:34:43.000000 teda-3.1.0/teda/icons/pause_circle_outline-24px.svg
--rw-r--r--   0        0        0      344 2020-07-01 12:47:01.000000 teda-3.1.0/teda/icons/photo_filter-24px.svg
--rw-r--r--   0        0        0      285 2020-06-08 17:34:37.000000 teda-3.1.0/teda/icons/play_circle_outline-24px.svg
--rw-r--r--   0        0        0      379 2020-07-01 12:39:55.000000 teda-3.1.0/teda/icons/push_pin-24px.svg
--rw-r--r--   0        0        0      333 2023-05-28 16:06:33.651338 teda-3.1.0/teda/icons/refresh-24px.svg
--rw-r--r--   0        0        0      304 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/save-24px.svg
--rw-r--r--   0        0        0      203 2020-06-08 17:29:29.000000 teda-3.1.0/teda/icons/skip_next-24px.svg
--rw-r--r--   0        0        0      206 2020-06-08 17:29:33.000000 teda-3.1.0/teda/icons/skip_previous-24px.svg
--rw-r--r--   0        0        0     1245 2020-12-03 12:27:12.917053 teda-3.1.0/teda/icons/slider-24px.svg
--rw-r--r--   0        0        0      295 2023-05-29 09:17:04.891965 teda-3.1.0/teda/icons/sort-24px.svg
--rw-r--r--   0        0        0      385 2020-06-08 17:34:40.000000 teda-3.1.0/teda/icons/stop_circle-24px.svg
--rw-r--r--   0        0        0     2638 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/x2-24px.svg
--rw-r--r--   0        0        0     2159 2020-07-01 13:22:36.000000 teda-3.1.0/teda/icons/x4-24px.svg
--rw-r--r--   0        0        0      571 2023-04-28 02:39:09.916622 teda-3.1.0/teda/icons.py
--rw-r--r--   0        0        0        0 2020-06-04 14:08:12.000000 teda-3.1.0/teda/models/__init__.py
--rw-r--r--   0        0        0      163 2023-04-27 22:41:43.996886 teda-3.1.0/teda/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      141 2020-06-04 14:13:27.000000 teda-3.1.0/teda/models/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     2415 2023-04-27 22:42:14.936963 teda-3.1.0/teda/models/__pycache__/cmaps.cpython-311.pyc
--rw-r--r--   0        0        0     1444 2020-06-04 14:13:27.000000 teda-3.1.0/teda/models/__pycache__/cmaps.cpython-37.pyc
--rw-r--r--   0        0        0     5832 2023-04-28 04:32:52.894102 teda-3.1.0/teda/models/__pycache__/coordinates.cpython-311.pyc
--rw-r--r--   0        0        0     3346 2020-12-03 12:42:28.079005 teda-3.1.0/teda/models/__pycache__/coordinates.cpython-37.pyc
--rw-r--r--   0        0        0     5448 2023-04-27 22:41:43.998909 teda-3.1.0/teda/models/__pycache__/scalesModel.cpython-311.pyc
--rw-r--r--   0        0        0     3219 2020-12-02 23:53:51.561303 teda-3.1.0/teda/models/__pycache__/scalesModel.cpython-37.pyc
--rw-r--r--   0        0        0     3792 2020-12-03 12:42:28.214696 teda-3.1.0/teda/models/__pycache__/shapes_group.cpython-37.pyc
--rw-r--r--   0        0        0        0 2023-05-28 16:18:53.841906 teda-3.1.0/teda/models/aaa.tmp
--rw-r--r--   0        0        0     1014 2020-06-04 10:29:56.000000 teda-3.1.0/teda/models/cmaps.py
--rw-r--r--   0        0        0     3002 2023-04-28 04:32:12.682801 teda-3.1.0/teda/models/coordinates.py
--rw-r--r--   0        0        0     5435 2020-12-02 21:00:51.002196 teda-3.1.0/teda/models/scalesModel.py
--rw-r--r--   0        0        0        0 2023-05-28 16:19:13.093531 teda-3.1.0/teda/models/zzz.tmp
--rw-r--r--   0        0        0    16439 2023-04-28 03:24:57.907274 teda-3.1.0/teda/painterComponent.py
--rw-r--r--   0        0        0     2967 2023-04-28 02:39:09.864767 teda-3.1.0/teda/painterShapes/CircleCenterShape.py
--rw-r--r--   0        0        0        0 2020-06-04 11:27:56.000000 teda-3.1.0/teda/painterShapes/__init__.py
--rw-r--r--   0        0        0     6220 2023-04-28 02:47:29.368730 teda-3.1.0/teda/painterShapes/__pycache__/CircleCenterShape.cpython-311.pyc
--rw-r--r--   0        0        0     3410 2020-06-04 11:53:07.000000 teda-3.1.0/teda/painterShapes/__pycache__/CircleCenterShape.cpython-37.pyc
--rw-r--r--   0        0        0      170 2023-04-27 22:41:44.734595 teda-3.1.0/teda/painterShapes/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      148 2020-06-04 11:53:07.000000 teda-3.1.0/teda/painterShapes/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     4007 2023-04-28 02:47:29.366538 teda-3.1.0/teda/painterShapes/__pycache__/circleShape.cpython-311.pyc
--rw-r--r--   0        0        0     2626 2020-12-03 13:28:14.814864 teda-3.1.0/teda/painterShapes/__pycache__/circleShape.cpython-37.pyc
--rw-r--r--   0        0        0     4369 2023-04-28 02:47:29.370222 teda-3.1.0/teda/painterShapes/__pycache__/rectangleMinatureShape.cpython-311.pyc
--rw-r--r--   0        0        0     2977 2020-06-04 11:53:07.000000 teda-3.1.0/teda/painterShapes/__pycache__/rectangleMinatureShape.cpython-37.pyc
--rw-r--r--   0        0        0     1885 2023-04-28 02:39:09.885266 teda-3.1.0/teda/painterShapes/circleShape.py
--rw-r--r--   0        0        0     2227 2023-04-28 02:39:09.889630 teda-3.1.0/teda/painterShapes/rectangleMinatureShape.py
--rwxr-xr-x   0        0        0     1410 2023-04-28 02:57:03.732713 teda-3.1.0/teda/teda_fits.py
--rw-r--r--   0        0        0      123 2023-05-29 11:13:55.600540 teda-3.1.0/teda/version.py
--rw-r--r--   0        0        0    34360 2023-05-29 09:52:50.872380 teda-3.1.0/teda/viewer_mainwindow.py
--rw-r--r--   0        0        0        0 2020-06-04 14:07:28.000000 teda-3.1.0/teda/views/__init__.py
--rw-r--r--   0        0        0      162 2023-04-27 22:41:33.450750 teda-3.1.0/teda/views/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      140 2020-06-04 14:13:26.000000 teda-3.1.0/teda/views/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0    27001 2023-04-28 03:13:18.985069 teda-3.1.0/teda/views/__pycache__/fitsplot.cpython-311.pyc
--rw-r--r--   0        0        0    13679 2020-12-02 23:53:51.217493 teda-3.1.0/teda/views/__pycache__/fitsplot.cpython-37.pyc
--rw-r--r--   0        0        0     5676 2023-05-29 09:30:58.321016 teda-3.1.0/teda/views/__pycache__/fitsplot_fitsfile.cpython-311.pyc
--rw-r--r--   0        0        0     2895 2020-12-03 12:42:28.076708 teda-3.1.0/teda/views/__pycache__/fitsplot_fitsfile.cpython-37.pyc
--rw-r--r--   0        0        0     4376 2023-04-27 22:41:44.002790 teda-3.1.0/teda/views/__pycache__/fitsplotcontrolled.cpython-311.pyc
--rw-r--r--   0        0        0     2621 2020-12-02 23:53:51.563344 teda-3.1.0/teda/views/__pycache__/fitsplotcontrolled.cpython-37.pyc
--rw-r--r--   0        0        0     2325 2023-04-27 22:42:14.915899 teda-3.1.0/teda/views/__pycache__/fitsplotzoomed.cpython-311.pyc
--rw-r--r--   0        0        0     1419 2020-06-04 14:13:27.000000 teda-3.1.0/teda/views/__pycache__/fitsplotzoomed.cpython-37.pyc
--rw-r--r--   0        0        0    17605 2023-04-28 03:13:13.702006 teda-3.1.0/teda/views/fitsplot.py
--rw-r--r--   0        0        0     2856 2023-05-29 09:27:03.636226 teda-3.1.0/teda/views/fitsplot_fitsfile.py
--rw-r--r--   0        0        0     2498 2020-12-02 21:00:51.007550 teda-3.1.0/teda/views/fitsplotcontrolled.py
--rw-r--r--   0        0        0     1143 2020-06-04 11:45:26.000000 teda-3.1.0/teda/views/fitsplotzoomed.py
--rw-r--r--   0        0        0        0 2020-06-04 14:10:29.000000 teda-3.1.0/teda/widgets/__init__.py
--rw-r--r--   0        0        0      164 2023-04-27 22:42:14.909974 teda-3.1.0/teda/widgets/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      142 2020-06-04 14:13:27.000000 teda-3.1.0/teda/widgets/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0    16801 2023-05-29 11:27:40.997985 teda-3.1.0/teda/widgets/__pycache__/fileSystemWidget.cpython-311.pyc
--rw-r--r--   0        0        0     5546 2020-12-03 13:28:14.901959 teda-3.1.0/teda/widgets/__pycache__/fileSystemWidget.cpython-37.pyc
--rw-r--r--   0        0        0     4931 2023-04-28 02:47:51.449604 teda-3.1.0/teda/widgets/__pycache__/fullViewWidget.cpython-311.pyc
--rw-r--r--   0        0        0     2462 2020-06-04 14:13:27.000000 teda-3.1.0/teda/widgets/__pycache__/fullViewWidget.cpython-37.pyc
--rw-r--r--   0        0        0     7076 2023-04-28 02:47:51.457738 teda-3.1.0/teda/widgets/__pycache__/headerTableWidget.cpython-311.pyc
--rw-r--r--   0        0        0     3338 2020-07-01 12:05:10.000000 teda-3.1.0/teda/widgets/__pycache__/headerTableWidget.cpython-37.pyc
--rw-r--r--   0        0        0     5518 2023-04-28 02:48:50.345439 teda-3.1.0/teda/widgets/__pycache__/info.cpython-311.pyc
--rw-r--r--   0        0        0     2716 2020-12-03 13:28:14.900070 teda-3.1.0/teda/widgets/__pycache__/info.cpython-37.pyc
--rw-r--r--   0        0        0     6042 2023-04-28 02:47:51.447525 teda-3.1.0/teda/widgets/__pycache__/radialprofile.cpython-311.pyc
--rw-r--r--   0        0        0     3310 2020-06-06 15:32:49.000000 teda-3.1.0/teda/widgets/__pycache__/radialprofile.cpython-37.pyc
--rw-r--r--   0        0        0     8717 2023-05-29 10:59:20.013231 teda-3.1.0/teda/widgets/__pycache__/radialprofileIRAF.cpython-311.pyc
--rw-r--r--   0        0        0     4754 2020-06-16 14:25:09.000000 teda-3.1.0/teda/widgets/__pycache__/radialprofileIRAF.cpython-37.pyc
--rw-r--r--   0        0        0     5923 2020-12-03 12:42:28.423269 teda-3.1.0/teda/widgets/__pycache__/regionsWidget.cpython-37.pyc
--rw-r--r--   0        0        0    41551 2023-04-28 04:13:26.808651 teda-3.1.0/teda/widgets/__pycache__/scaleWidget.cpython-311.pyc
--rw-r--r--   0        0        0    17990 2020-12-03 13:28:14.896657 teda-3.1.0/teda/widgets/__pycache__/scaleWidget.cpython-37.pyc
--rw-r--r--   0        0        0    20348 2023-04-28 02:48:50.342163 teda-3.1.0/teda/widgets/__pycache__/scanToolbar.cpython-311.pyc
--rw-r--r--   0        0        0     9700 2020-07-01 13:54:40.000000 teda-3.1.0/teda/widgets/__pycache__/scanToolbar.cpython-37.pyc
--rw-r--r--   0        0        0    12512 2023-04-28 02:47:51.468296 teda-3.1.0/teda/widgets/__pycache__/slider.cpython-311.pyc
--rw-r--r--   0        0        0     6731 2020-12-02 23:53:51.755329 teda-3.1.0/teda/widgets/__pycache__/slider.cpython-37.pyc
--rw-r--r--   0        0        0     2853 2023-04-28 02:47:51.451127 teda-3.1.0/teda/widgets/__pycache__/zoomViewWidget.cpython-311.pyc
--rw-r--r--   0        0        0     1605 2020-06-04 14:13:27.000000 teda-3.1.0/teda/widgets/__pycache__/zoomViewWidget.cpython-37.pyc
--rw-r--r--   0        0        0     8342 2023-05-29 11:27:30.901972 teda-3.1.0/teda/widgets/fileSystemWidget.py
--rw-r--r--   0        0        0     2976 2023-04-28 02:39:09.907291 teda-3.1.0/teda/widgets/fullViewWidget.py
--rw-r--r--   0        0        0     3270 2023-04-28 02:39:09.874014 teda-3.1.0/teda/widgets/headerTableWidget.py
--rw-r--r--   0        0        0     2295 2023-04-28 02:39:09.924105 teda-3.1.0/teda/widgets/info.py
--rw-r--r--   0        0        0     3293 2023-04-28 02:39:09.869422 teda-3.1.0/teda/widgets/radialprofile.py
--rw-r--r--   0        0        0     5546 2023-05-29 10:58:34.283016 teda-3.1.0/teda/widgets/radialprofileIRAF.py
--rw-r--r--   0        0        0    24353 2023-04-28 04:12:12.833462 teda-3.1.0/teda/widgets/scaleWidget.py
--rw-r--r--   0        0        0    12534 2023-04-28 02:48:42.836537 teda-3.1.0/teda/widgets/scanToolbar.py
--rw-r--r--   0        0        0     6207 2023-04-28 02:39:09.903950 teda-3.1.0/teda/widgets/slider.py
--rw-r--r--   0        0        0     1357 2023-04-28 02:39:09.895011 teda-3.1.0/teda/widgets/zoomViewWidget.py
--rw-r--r--   0        0        0     5758 1970-01-01 00:00:00.000000 teda-3.1.0/setup.py
--rw-r--r--   0        0        0     5381 1970-01-01 00:00:00.000000 teda-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2020-06-04 16:42:55.000000 teda-3.1.1/LICENSE
+-rw-r--r--   0        0        0     4719 2020-12-02 21:00:51.000070 teda-3.1.1/README.md
+-rw-r--r--   0        0        0      478 2023-05-29 11:54:26.314503 teda-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8196 2020-09-07 16:29:27.113605 teda-3.1.1/teda/.DS_Store
+-rw-r--r--   0        0        0       32 2020-06-04 16:24:35.000000 teda-3.1.1/teda/__init__.py
+-rw-r--r--   0        0        0     2116 2023-05-28 13:57:12.142317 teda-3.1.1/teda/command_line.py
+-rw-r--r--   0        0        0     1958 2020-07-01 12:39:55.000000 teda-3.1.1/teda/console.py
+-rw-r--r--   0        0        0     1531 2020-12-03 12:27:12.916427 teda-3.1.1/teda/draggingComponent.py
+-rw-r--r--   0        0        0     2105 2020-04-22 14:55:56.000000 teda-3.1.1/teda/fitsopen.py
+-rw-r--r--   0        0        0     2042 2023-05-29 09:48:43.095118 teda-3.1.1/teda/fitting.py
+-rw-r--r--   0        0        0     6148 2020-06-16 15:09:14.000000 teda-3.1.1/teda/icons/.DS_Store
+-rw-r--r--   0        0        0     2716 2020-07-01 13:22:36.000000 teda-3.1.1/teda/icons/1-2-24px.svg
+-rw-r--r--   0        0        0     2238 2020-07-01 13:22:36.000000 teda-3.1.1/teda/icons/1-4-24px.svg
+-rw-r--r--   0        0        0      298 2020-06-10 13:51:52.000000 teda-3.1.1/teda/icons/add_circle_outline-24px.svg
+-rw-r--r--   0        0        0      380 2020-07-01 13:22:36.000000 teda-3.1.1/teda/icons/autopause-24px.svg
+-rw-r--r--   0        0        0      222 2020-07-01 13:22:36.000000 teda-3.1.1/teda/icons/autopause_disabled-24px.svg
+-rw-r--r--   0        0        0      262 2020-06-10 13:51:52.000000 teda-3.1.1/teda/icons/circle-24px.svg
+-rw-r--r--   0        0        0      249 2020-07-01 13:22:36.000000 teda-3.1.1/teda/icons/count1-24px.svg
+-rw-r--r--   0        0        0      315 2020-07-01 13:22:36.000000 teda-3.1.1/teda/icons/count2-24px.svg
+-rw-r--r--   0        0        0      343 2020-07-01 13:22:36.000000 teda-3.1.1/teda/icons/count3-24px.svg
+-rw-r--r--   0        0        0      270 2020-07-01 13:22:36.000000 teda-3.1.1/teda/icons/count4-24px.svg
+-rw-r--r--   0        0        0      296 2020-07-01 13:22:36.000000 teda-3.1.1/teda/icons/count5-24px.svg
+-rw-r--r--   0        0        0      349 2020-06-10 13:51:52.000000 teda-3.1.1/teda/icons/delete_forever-24px.svg
+-rw-r--r--   0        0        0      518 2020-05-14 14:33:36.000000 teda-3.1.1/teda/icons/file-earmark-plus.svg
+-rw-r--r--   0        0        0      402 2020-07-01 12:47:01.000000 teda-3.1.1/teda/icons/filter_alt-24px.svg
+-rw-r--r--   0        0        0      257 2020-07-01 12:47:01.000000 teda-3.1.1/teda/icons/folder-24px.svg
+-rw-r--r--   0        0        0      217 2020-06-08 17:33:08.000000 teda-3.1.1/teda/icons/home-24px.svg
+-rw-r--r--   0        0        0      343 2020-06-08 17:32:29.000000 teda-3.1.1/teda/icons/house-24px.svg
+-rw-r--r--   0        0        0      196 2020-06-08 17:30:35.000000 teda-3.1.1/teda/icons/keyboard_arrow_left-24px.svg
+-rw-r--r--   0        0        0      194 2020-06-08 17:30:21.000000 teda-3.1.1/teda/icons/keyboard_arrow_right-24px.svg
+-rw-r--r--   0        0        0      977 2020-06-05 15:03:11.000000 teda-3.1.1/teda/icons/new.png
+-rw-r--r--   0        0        0      367 2020-06-10 13:51:52.000000 teda-3.1.1/teda/icons/not_started-24px.svg
+-rw-r--r--   0        0        0      261 2020-06-08 17:13:41.000000 teda-3.1.1/teda/icons/note_add-24px.svg
+-rw-r--r--   0        0        0      245 2020-07-01 13:22:36.000000 teda-3.1.1/teda/icons/panning-24px.svg
+-rw-r--r--   0        0        0      292 2020-06-08 17:34:43.000000 teda-3.1.1/teda/icons/pause_circle_outline-24px.svg
+-rw-r--r--   0        0        0      344 2020-07-01 12:47:01.000000 teda-3.1.1/teda/icons/photo_filter-24px.svg
+-rw-r--r--   0        0        0      285 2020-06-08 17:34:37.000000 teda-3.1.1/teda/icons/play_circle_outline-24px.svg
+-rw-r--r--   0        0        0      379 2020-07-01 12:39:55.000000 teda-3.1.1/teda/icons/push_pin-24px.svg
+-rw-r--r--   0        0        0      333 2023-05-28 16:06:33.651338 teda-3.1.1/teda/icons/refresh-24px.svg
+-rw-r--r--   0        0        0      304 2020-07-01 13:22:36.000000 teda-3.1.1/teda/icons/save-24px.svg
+-rw-r--r--   0        0        0      203 2020-06-08 17:29:29.000000 teda-3.1.1/teda/icons/skip_next-24px.svg
+-rw-r--r--   0        0        0      206 2020-06-08 17:29:33.000000 teda-3.1.1/teda/icons/skip_previous-24px.svg
+-rw-r--r--   0        0        0     1245 2020-12-03 12:27:12.917053 teda-3.1.1/teda/icons/slider-24px.svg
+-rw-r--r--   0        0        0      295 2023-05-29 09:17:04.891965 teda-3.1.1/teda/icons/sort-24px.svg
+-rw-r--r--   0        0        0      385 2020-06-08 17:34:40.000000 teda-3.1.1/teda/icons/stop_circle-24px.svg
+-rw-r--r--   0        0        0     2638 2020-07-01 13:22:36.000000 teda-3.1.1/teda/icons/x2-24px.svg
+-rw-r--r--   0        0        0     2159 2020-07-01 13:22:36.000000 teda-3.1.1/teda/icons/x4-24px.svg
+-rw-r--r--   0        0        0      571 2023-04-28 02:39:09.916622 teda-3.1.1/teda/icons.py
+-rw-r--r--   0        0        0        0 2020-06-04 14:08:12.000000 teda-3.1.1/teda/models/__init__.py
+-rw-r--r--   0        0        0      163 2023-04-27 22:41:43.996886 teda-3.1.1/teda/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      141 2020-06-04 14:13:27.000000 teda-3.1.1/teda/models/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     2415 2023-04-27 22:42:14.936963 teda-3.1.1/teda/models/__pycache__/cmaps.cpython-311.pyc
+-rw-r--r--   0        0        0     1444 2020-06-04 14:13:27.000000 teda-3.1.1/teda/models/__pycache__/cmaps.cpython-37.pyc
+-rw-r--r--   0        0        0     5832 2023-04-28 04:32:52.894102 teda-3.1.1/teda/models/__pycache__/coordinates.cpython-311.pyc
+-rw-r--r--   0        0        0     3346 2020-12-03 12:42:28.079005 teda-3.1.1/teda/models/__pycache__/coordinates.cpython-37.pyc
+-rw-r--r--   0        0        0     5448 2023-04-27 22:41:43.998909 teda-3.1.1/teda/models/__pycache__/scalesModel.cpython-311.pyc
+-rw-r--r--   0        0        0     3219 2020-12-02 23:53:51.561303 teda-3.1.1/teda/models/__pycache__/scalesModel.cpython-37.pyc
+-rw-r--r--   0        0        0     3792 2020-12-03 12:42:28.214696 teda-3.1.1/teda/models/__pycache__/shapes_group.cpython-37.pyc
+-rw-r--r--   0        0        0        0 2023-05-28 16:18:53.841906 teda-3.1.1/teda/models/aaa.tmp
+-rw-r--r--   0        0        0     1014 2020-06-04 10:29:56.000000 teda-3.1.1/teda/models/cmaps.py
+-rw-r--r--   0        0        0     3002 2023-04-28 04:32:12.682801 teda-3.1.1/teda/models/coordinates.py
+-rw-r--r--   0        0        0     5435 2020-12-02 21:00:51.002196 teda-3.1.1/teda/models/scalesModel.py
+-rw-r--r--   0        0        0        0 2023-05-28 16:19:13.093531 teda-3.1.1/teda/models/zzz.tmp
+-rw-r--r--   0        0        0    16439 2023-04-28 03:24:57.907274 teda-3.1.1/teda/painterComponent.py
+-rw-r--r--   0        0        0     2967 2023-04-28 02:39:09.864767 teda-3.1.1/teda/painterShapes/CircleCenterShape.py
+-rw-r--r--   0        0        0        0 2020-06-04 11:27:56.000000 teda-3.1.1/teda/painterShapes/__init__.py
+-rw-r--r--   0        0        0     6220 2023-04-28 02:47:29.368730 teda-3.1.1/teda/painterShapes/__pycache__/CircleCenterShape.cpython-311.pyc
+-rw-r--r--   0        0        0     3410 2020-06-04 11:53:07.000000 teda-3.1.1/teda/painterShapes/__pycache__/CircleCenterShape.cpython-37.pyc
+-rw-r--r--   0        0        0      170 2023-04-27 22:41:44.734595 teda-3.1.1/teda/painterShapes/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      148 2020-06-04 11:53:07.000000 teda-3.1.1/teda/painterShapes/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     4007 2023-04-28 02:47:29.366538 teda-3.1.1/teda/painterShapes/__pycache__/circleShape.cpython-311.pyc
+-rw-r--r--   0        0        0     2626 2020-12-03 13:28:14.814864 teda-3.1.1/teda/painterShapes/__pycache__/circleShape.cpython-37.pyc
+-rw-r--r--   0        0        0     4369 2023-04-28 02:47:29.370222 teda-3.1.1/teda/painterShapes/__pycache__/rectangleMinatureShape.cpython-311.pyc
+-rw-r--r--   0        0        0     2977 2020-06-04 11:53:07.000000 teda-3.1.1/teda/painterShapes/__pycache__/rectangleMinatureShape.cpython-37.pyc
+-rw-r--r--   0        0        0     1885 2023-04-28 02:39:09.885266 teda-3.1.1/teda/painterShapes/circleShape.py
+-rw-r--r--   0        0        0     2227 2023-04-28 02:39:09.889630 teda-3.1.1/teda/painterShapes/rectangleMinatureShape.py
+-rwxr-xr-x   0        0        0     1410 2023-04-28 02:57:03.732713 teda-3.1.1/teda/teda_fits.py
+-rw-r--r--   0        0        0      123 2023-05-29 11:54:38.327543 teda-3.1.1/teda/version.py
+-rw-r--r--   0        0        0    34360 2023-05-29 09:52:50.872380 teda-3.1.1/teda/viewer_mainwindow.py
+-rw-r--r--   0        0        0        0 2020-06-04 14:07:28.000000 teda-3.1.1/teda/views/__init__.py
+-rw-r--r--   0        0        0      162 2023-04-27 22:41:33.450750 teda-3.1.1/teda/views/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      140 2020-06-04 14:13:26.000000 teda-3.1.1/teda/views/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0    27001 2023-04-28 03:13:18.985069 teda-3.1.1/teda/views/__pycache__/fitsplot.cpython-311.pyc
+-rw-r--r--   0        0        0    13679 2020-12-02 23:53:51.217493 teda-3.1.1/teda/views/__pycache__/fitsplot.cpython-37.pyc
+-rw-r--r--   0        0        0     5676 2023-05-29 09:30:58.321016 teda-3.1.1/teda/views/__pycache__/fitsplot_fitsfile.cpython-311.pyc
+-rw-r--r--   0        0        0     2895 2020-12-03 12:42:28.076708 teda-3.1.1/teda/views/__pycache__/fitsplot_fitsfile.cpython-37.pyc
+-rw-r--r--   0        0        0     4376 2023-04-27 22:41:44.002790 teda-3.1.1/teda/views/__pycache__/fitsplotcontrolled.cpython-311.pyc
+-rw-r--r--   0        0        0     2621 2020-12-02 23:53:51.563344 teda-3.1.1/teda/views/__pycache__/fitsplotcontrolled.cpython-37.pyc
+-rw-r--r--   0        0        0     2325 2023-04-27 22:42:14.915899 teda-3.1.1/teda/views/__pycache__/fitsplotzoomed.cpython-311.pyc
+-rw-r--r--   0        0        0     1419 2020-06-04 14:13:27.000000 teda-3.1.1/teda/views/__pycache__/fitsplotzoomed.cpython-37.pyc
+-rw-r--r--   0        0        0    17605 2023-04-28 03:13:13.702006 teda-3.1.1/teda/views/fitsplot.py
+-rw-r--r--   0        0        0     2856 2023-05-29 09:27:03.636226 teda-3.1.1/teda/views/fitsplot_fitsfile.py
+-rw-r--r--   0        0        0     2498 2020-12-02 21:00:51.007550 teda-3.1.1/teda/views/fitsplotcontrolled.py
+-rw-r--r--   0        0        0     1143 2020-06-04 11:45:26.000000 teda-3.1.1/teda/views/fitsplotzoomed.py
+-rw-r--r--   0        0        0        0 2020-06-04 14:10:29.000000 teda-3.1.1/teda/widgets/__init__.py
+-rw-r--r--   0        0        0      164 2023-04-27 22:42:14.909974 teda-3.1.1/teda/widgets/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      142 2020-06-04 14:13:27.000000 teda-3.1.1/teda/widgets/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0    16801 2023-05-29 11:27:40.997985 teda-3.1.1/teda/widgets/__pycache__/fileSystemWidget.cpython-311.pyc
+-rw-r--r--   0        0        0     5546 2020-12-03 13:28:14.901959 teda-3.1.1/teda/widgets/__pycache__/fileSystemWidget.cpython-37.pyc
+-rw-r--r--   0        0        0     4931 2023-04-28 02:47:51.449604 teda-3.1.1/teda/widgets/__pycache__/fullViewWidget.cpython-311.pyc
+-rw-r--r--   0        0        0     2462 2020-06-04 14:13:27.000000 teda-3.1.1/teda/widgets/__pycache__/fullViewWidget.cpython-37.pyc
+-rw-r--r--   0        0        0     7076 2023-04-28 02:47:51.457738 teda-3.1.1/teda/widgets/__pycache__/headerTableWidget.cpython-311.pyc
+-rw-r--r--   0        0        0     3338 2020-07-01 12:05:10.000000 teda-3.1.1/teda/widgets/__pycache__/headerTableWidget.cpython-37.pyc
+-rw-r--r--   0        0        0     5518 2023-04-28 02:48:50.345439 teda-3.1.1/teda/widgets/__pycache__/info.cpython-311.pyc
+-rw-r--r--   0        0        0     2716 2020-12-03 13:28:14.900070 teda-3.1.1/teda/widgets/__pycache__/info.cpython-37.pyc
+-rw-r--r--   0        0        0     6042 2023-04-28 02:47:51.447525 teda-3.1.1/teda/widgets/__pycache__/radialprofile.cpython-311.pyc
+-rw-r--r--   0        0        0     3310 2020-06-06 15:32:49.000000 teda-3.1.1/teda/widgets/__pycache__/radialprofile.cpython-37.pyc
+-rw-r--r--   0        0        0     8717 2023-05-29 10:59:20.013231 teda-3.1.1/teda/widgets/__pycache__/radialprofileIRAF.cpython-311.pyc
+-rw-r--r--   0        0        0     4754 2020-06-16 14:25:09.000000 teda-3.1.1/teda/widgets/__pycache__/radialprofileIRAF.cpython-37.pyc
+-rw-r--r--   0        0        0     5923 2020-12-03 12:42:28.423269 teda-3.1.1/teda/widgets/__pycache__/regionsWidget.cpython-37.pyc
+-rw-r--r--   0        0        0    41551 2023-04-28 04:13:26.808651 teda-3.1.1/teda/widgets/__pycache__/scaleWidget.cpython-311.pyc
+-rw-r--r--   0        0        0    17990 2020-12-03 13:28:14.896657 teda-3.1.1/teda/widgets/__pycache__/scaleWidget.cpython-37.pyc
+-rw-r--r--   0        0        0    20348 2023-04-28 02:48:50.342163 teda-3.1.1/teda/widgets/__pycache__/scanToolbar.cpython-311.pyc
+-rw-r--r--   0        0        0     9700 2020-07-01 13:54:40.000000 teda-3.1.1/teda/widgets/__pycache__/scanToolbar.cpython-37.pyc
+-rw-r--r--   0        0        0    12512 2023-04-28 02:47:51.468296 teda-3.1.1/teda/widgets/__pycache__/slider.cpython-311.pyc
+-rw-r--r--   0        0        0     6731 2020-12-02 23:53:51.755329 teda-3.1.1/teda/widgets/__pycache__/slider.cpython-37.pyc
+-rw-r--r--   0        0        0     2853 2023-04-28 02:47:51.451127 teda-3.1.1/teda/widgets/__pycache__/zoomViewWidget.cpython-311.pyc
+-rw-r--r--   0        0        0     1605 2020-06-04 14:13:27.000000 teda-3.1.1/teda/widgets/__pycache__/zoomViewWidget.cpython-37.pyc
+-rw-r--r--   0        0        0     8366 2023-05-29 11:53:54.656613 teda-3.1.1/teda/widgets/fileSystemWidget.py
+-rw-r--r--   0        0        0     2976 2023-04-28 02:39:09.907291 teda-3.1.1/teda/widgets/fullViewWidget.py
+-rw-r--r--   0        0        0     3270 2023-04-28 02:39:09.874014 teda-3.1.1/teda/widgets/headerTableWidget.py
+-rw-r--r--   0        0        0     2295 2023-04-28 02:39:09.924105 teda-3.1.1/teda/widgets/info.py
+-rw-r--r--   0        0        0     3293 2023-04-28 02:39:09.869422 teda-3.1.1/teda/widgets/radialprofile.py
+-rw-r--r--   0        0        0     5546 2023-05-29 10:58:34.283016 teda-3.1.1/teda/widgets/radialprofileIRAF.py
+-rw-r--r--   0        0        0    24353 2023-04-28 04:12:12.833462 teda-3.1.1/teda/widgets/scaleWidget.py
+-rw-r--r--   0        0        0    12534 2023-04-28 02:48:42.836537 teda-3.1.1/teda/widgets/scanToolbar.py
+-rw-r--r--   0        0        0     6207 2023-04-28 02:39:09.903950 teda-3.1.1/teda/widgets/slider.py
+-rw-r--r--   0        0        0     1357 2023-04-28 02:39:09.895011 teda-3.1.1/teda/widgets/zoomViewWidget.py
+-rw-r--r--   0        0        0     5758 1970-01-01 00:00:00.000000 teda-3.1.1/setup.py
+-rw-r--r--   0        0        0     5381 1970-01-01 00:00:00.000000 teda-3.1.1/PKG-INFO
```

### Comparing `teda-3.1.0/LICENSE` & `teda-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/README.md` & `teda-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/.DS_Store` & `teda-3.1.1/teda/.DS_Store`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/command_line.py` & `teda-3.1.1/teda/command_line.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/console.py` & `teda-3.1.1/teda/console.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/draggingComponent.py` & `teda-3.1.1/teda/draggingComponent.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/fitsopen.py` & `teda-3.1.1/teda/fitsopen.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/fitting.py` & `teda-3.1.1/teda/fitting.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/icons/.DS_Store` & `teda-3.1.1/teda/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/icons/1-2-24px.svg` & `teda-3.1.1/teda/icons/1-2-24px.svg`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/icons/1-4-24px.svg` & `teda-3.1.1/teda/icons/1-4-24px.svg`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/icons/file-earmark-plus.svg` & `teda-3.1.1/teda/icons/file-earmark-plus.svg`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/icons/new.png` & `teda-3.1.1/teda/icons/new.png`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/icons/slider-24px.svg` & `teda-3.1.1/teda/icons/slider-24px.svg`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/icons/x2-24px.svg` & `teda-3.1.1/teda/icons/x2-24px.svg`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/icons/x4-24px.svg` & `teda-3.1.1/teda/icons/x4-24px.svg`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/icons.py` & `teda-3.1.1/teda/icons.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/models/__pycache__/cmaps.cpython-311.pyc` & `teda-3.1.1/teda/models/__pycache__/cmaps.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/models/__pycache__/cmaps.cpython-37.pyc` & `teda-3.1.1/teda/models/__pycache__/cmaps.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/models/__pycache__/coordinates.cpython-311.pyc` & `teda-3.1.1/teda/models/__pycache__/coordinates.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/models/__pycache__/coordinates.cpython-37.pyc` & `teda-3.1.1/teda/models/__pycache__/coordinates.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/models/__pycache__/scalesModel.cpython-311.pyc` & `teda-3.1.1/teda/models/__pycache__/scalesModel.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/models/__pycache__/scalesModel.cpython-37.pyc` & `teda-3.1.1/teda/models/__pycache__/scalesModel.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/models/__pycache__/shapes_group.cpython-37.pyc` & `teda-3.1.1/teda/models/__pycache__/shapes_group.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/models/cmaps.py` & `teda-3.1.1/teda/models/cmaps.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/models/coordinates.py` & `teda-3.1.1/teda/models/coordinates.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/models/scalesModel.py` & `teda-3.1.1/teda/models/scalesModel.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/painterComponent.py` & `teda-3.1.1/teda/painterComponent.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/painterShapes/CircleCenterShape.py` & `teda-3.1.1/teda/painterShapes/CircleCenterShape.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/painterShapes/__pycache__/CircleCenterShape.cpython-311.pyc` & `teda-3.1.1/teda/painterShapes/__pycache__/CircleCenterShape.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/painterShapes/__pycache__/CircleCenterShape.cpython-37.pyc` & `teda-3.1.1/teda/painterShapes/__pycache__/CircleCenterShape.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/painterShapes/__pycache__/circleShape.cpython-311.pyc` & `teda-3.1.1/teda/painterShapes/__pycache__/circleShape.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/painterShapes/__pycache__/circleShape.cpython-37.pyc` & `teda-3.1.1/teda/painterShapes/__pycache__/circleShape.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/painterShapes/__pycache__/rectangleMinatureShape.cpython-311.pyc` & `teda-3.1.1/teda/painterShapes/__pycache__/rectangleMinatureShape.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/painterShapes/__pycache__/rectangleMinatureShape.cpython-37.pyc` & `teda-3.1.1/teda/painterShapes/__pycache__/rectangleMinatureShape.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/painterShapes/circleShape.py` & `teda-3.1.1/teda/painterShapes/circleShape.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/painterShapes/rectangleMinatureShape.py` & `teda-3.1.1/teda/painterShapes/rectangleMinatureShape.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/teda_fits.py` & `teda-3.1.1/teda/teda_fits.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/viewer_mainwindow.py` & `teda-3.1.1/teda/viewer_mainwindow.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/views/__pycache__/fitsplot.cpython-311.pyc` & `teda-3.1.1/teda/views/__pycache__/fitsplot.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/views/__pycache__/fitsplot.cpython-37.pyc` & `teda-3.1.1/teda/views/__pycache__/fitsplot.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/views/__pycache__/fitsplot_fitsfile.cpython-311.pyc` & `teda-3.1.1/teda/views/__pycache__/fitsplot_fitsfile.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/views/__pycache__/fitsplot_fitsfile.cpython-37.pyc` & `teda-3.1.1/teda/views/__pycache__/fitsplot_fitsfile.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/views/__pycache__/fitsplotcontrolled.cpython-311.pyc` & `teda-3.1.1/teda/views/__pycache__/fitsplotcontrolled.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/views/__pycache__/fitsplotcontrolled.cpython-37.pyc` & `teda-3.1.1/teda/views/__pycache__/fitsplotcontrolled.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/views/__pycache__/fitsplotzoomed.cpython-311.pyc` & `teda-3.1.1/teda/views/__pycache__/fitsplotzoomed.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/views/__pycache__/fitsplotzoomed.cpython-37.pyc` & `teda-3.1.1/teda/views/__pycache__/fitsplotzoomed.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/views/fitsplot.py` & `teda-3.1.1/teda/views/fitsplot.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/views/fitsplot_fitsfile.py` & `teda-3.1.1/teda/views/fitsplot_fitsfile.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/views/fitsplotcontrolled.py` & `teda-3.1.1/teda/views/fitsplotcontrolled.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/views/fitsplotzoomed.py` & `teda-3.1.1/teda/views/fitsplotzoomed.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/__pycache__/fileSystemWidget.cpython-311.pyc` & `teda-3.1.1/teda/widgets/__pycache__/fileSystemWidget.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/__pycache__/fileSystemWidget.cpython-37.pyc` & `teda-3.1.1/teda/widgets/__pycache__/fileSystemWidget.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/__pycache__/fullViewWidget.cpython-311.pyc` & `teda-3.1.1/teda/widgets/__pycache__/fullViewWidget.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/__pycache__/fullViewWidget.cpython-37.pyc` & `teda-3.1.1/teda/widgets/__pycache__/fullViewWidget.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/__pycache__/headerTableWidget.cpython-311.pyc` & `teda-3.1.1/teda/widgets/__pycache__/headerTableWidget.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/__pycache__/headerTableWidget.cpython-37.pyc` & `teda-3.1.1/teda/widgets/__pycache__/headerTableWidget.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/__pycache__/info.cpython-311.pyc` & `teda-3.1.1/teda/widgets/__pycache__/info.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/__pycache__/info.cpython-37.pyc` & `teda-3.1.1/teda/widgets/__pycache__/info.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/__pycache__/radialprofile.cpython-311.pyc` & `teda-3.1.1/teda/widgets/__pycache__/radialprofile.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/__pycache__/radialprofile.cpython-37.pyc` & `teda-3.1.1/teda/widgets/__pycache__/radialprofile.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/__pycache__/radialprofileIRAF.cpython-311.pyc` & `teda-3.1.1/teda/widgets/__pycache__/radialprofileIRAF.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/__pycache__/radialprofileIRAF.cpython-37.pyc` & `teda-3.1.1/teda/widgets/__pycache__/radialprofileIRAF.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/__pycache__/regionsWidget.cpython-37.pyc` & `teda-3.1.1/teda/widgets/__pycache__/regionsWidget.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/__pycache__/scaleWidget.cpython-311.pyc` & `teda-3.1.1/teda/widgets/__pycache__/scaleWidget.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/__pycache__/scaleWidget.cpython-37.pyc` & `teda-3.1.1/teda/widgets/__pycache__/scaleWidget.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/__pycache__/scanToolbar.cpython-311.pyc` & `teda-3.1.1/teda/widgets/__pycache__/scanToolbar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/__pycache__/scanToolbar.cpython-37.pyc` & `teda-3.1.1/teda/widgets/__pycache__/scanToolbar.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/__pycache__/slider.cpython-311.pyc` & `teda-3.1.1/teda/widgets/__pycache__/slider.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/__pycache__/slider.cpython-37.pyc` & `teda-3.1.1/teda/widgets/__pycache__/slider.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/__pycache__/zoomViewWidget.cpython-311.pyc` & `teda-3.1.1/teda/widgets/__pycache__/zoomViewWidget.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/__pycache__/zoomViewWidget.cpython-37.pyc` & `teda-3.1.1/teda/widgets/__pycache__/zoomViewWidget.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/fileSystemWidget.py` & `teda-3.1.1/teda/widgets/fileSystemWidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,17 +184,17 @@
 
     def readSettings(self, settings):
         settings.beginGroup("fileWidget")
         self.viewsSplitter.restoreGeometry(settings.value("splitterGeometry"))
         self.viewsSplitter.restoreState(settings.value("splitterState"))
         rootPath = settings.value("rootPath")
         path = settings.value("path")
-        self.showOFAction.setChecked(settings.value("showOF"))
-        self.refreshFilesAction.setChecked(settings.value("refresh"))
-        self.sortFilesAction.setChecked(settings.value("sort"))
+        self.showOFAction.setChecked(settings.value("showOF") == True)
+        self.refreshFilesAction.setChecked(settings.value("refresh") == True)
+        self.sortFilesAction.setChecked(settings.value("sort") == True)
         settings.endGroup()
 
         if rootPath is None:
             rootPath = '/'
         self.setRootPath(rootPath)
 
         if path is None:
```

### Comparing `teda-3.1.0/teda/widgets/fullViewWidget.py` & `teda-3.1.1/teda/widgets/fullViewWidget.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/headerTableWidget.py` & `teda-3.1.1/teda/widgets/headerTableWidget.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/info.py` & `teda-3.1.1/teda/widgets/info.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/radialprofile.py` & `teda-3.1.1/teda/widgets/radialprofile.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/radialprofileIRAF.py` & `teda-3.1.1/teda/widgets/radialprofileIRAF.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/scaleWidget.py` & `teda-3.1.1/teda/widgets/scaleWidget.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/scanToolbar.py` & `teda-3.1.1/teda/widgets/scanToolbar.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/slider.py` & `teda-3.1.1/teda/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/teda/widgets/zoomViewWidget.py` & `teda-3.1.1/teda/widgets/zoomViewWidget.py`

 * *Files identical despite different names*

### Comparing `teda-3.1.0/setup.py` & `teda-3.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'traitlets>=5.9.0,<6.0.0']
 
 entry_points = \
 {'console_scripts': ['teda = teda.teda_fits:main']}
 
 setup_kwargs = {
     'name': 'teda',
-    'version': '3.1.0',
+    'version': '3.1.1',
     'description': 'Yet Another FITS Viewer',
     'long_description': '# TeDa FITS Viewer\n\nObservatory optimized FITS Images viewer\n\n![](img/teda.png)\n\n## Key Features\n* Flexible windows and widgets layout\n* WCS support\n* Radial Profile with gaussoide fit (try `r`-key)\n* Scan mode: observes directory for changes and automatically opens new FITS\n* Integrated ipython console with direct access to data and application\n\n## Installation\n``` bash\n   pip install teda\n   teda_viewer \n``` \n### Optional dependencies\nTo use ipython console the `qtconsole` package is needed, additionally:\n``` bash\n    pip install qtconsole\n``` \nFor directory scanning functionality, the `watchdog` package should be installed, e.g. \n``` bash\n    pip install watchdog\n``` \n\n## Run\nThe installation scripts should install the command:\n```\n    teda_viewer\n```\nTry \n```\n    teda_viewer --help\n```\nfor list of command line parameters.\n\n## Dynamic Scale and Color\nThe dynamic scale of the image, and color mapping can be adjusted form \nthe **Dynamic Scale** panel. From menu: **View/Dynamic Scale**\n\n## Fits Header Cards Pinning\nOn the FITS Header panel, selected keys can be *pinned* to appear\non the top ot the list. This can be done via context (right-click) menu.\n\nThe set of pinned keys is saved and preserved between sessions.  \n\n## Radial Profile\nThe **Radial Profile** button turns on the mode of selecting targets for \nthe radial profile analysis. Make sure the radial profile panel is visible \n(View/Radial Profile). The shortcut for displaying radial profile of the star \nunder cursor is the **R**-key.\n\nThe centroid of the star is corrected within small (be precise!) radius\nusing the bivariate gaussoide fit.\n\nTogether with the pixels values, the radial profile presents 1D fit of\n"gaussian(r) + sky". This fit provides information of presented fwhm and sky level.\n   \n\n## Integrated Python Console\nIn order to use integrated python console the `qtconsole` module, and it\'s\ndependencies (jupyter related) have to be installed. This is not done by\ndefault `pip` installation to keep number of dependencies reasonably small.\nInstall `qtconsole` by:\n``` bash\n    pip install qtconsole\n``` \n\nThe console is available form menu **View/Python Console**\n### Predefined variables\nThe console has a number of predefined variables set:\n* `ax: WCSAxesSubplot` main plotting axes.\n* `window: MainWindow` main window\n* `data: numpy.ndarray` current HDU data\n* `header: astropy.fits.Header` current HDU header\n* `wcs: astropy.wcs.WCS` the WCS transformer\n\n### Plotting\nTo plot directly on the console, run the following magic command `%matplotlib inline`.\n\nWhen plotting on the main canvas, the result will appear after redrawing\nmain figure by `ax.figure.canvas.draw()`.\n\nThe example below, draws linear profile on the console and corresponding\nline on the main FITS display:    \n  \n``` python\n%matplotlib inline\nimport matplotlib.pyplot as plt\nax.plot([10,30], [10,10])\nax.figure.canvas.draw()\nplt.plot(data[10,10:30])\n```\n\n## Directory Scan\nThe **Scan Toolbar** (hidden by default) provides controls for the \ndirectory scanning mode.\n\nThis mode is intended to observe newly created FITS files in observatory.\n\nAfter pressing **Scan** button, and choosing directory, TeDa Fits Viewer will\nload most recent FITS file from that directory, and keep watching the directory \nfor changes. When new FITS file is added to directory, it will be loaded \nautomatically.\n\nUser can pause scanning using **Pause** button. There is also **auto pause** feature,\nwhen active, any mouse movement in the main area pauses scanning for 5 seconds,\navoiding FITS reload when working.\n\nAfter un-pausing (manually or after idle 5 seconds when auto-pause) the newest\nFITS will be loaded if any new files appeared during the pause.\n\nDirectory scanning needs the [`watchdog`](https://pypi.org/project/watchdog/) component to be \ninstalled manually (optional dependence).\n\n## Directory Panel\nThe Directory Panel can be shown using menu command **View-Directory view**.\n\nThe Directory Panel is convenient files navigator. The panel has two views:\n* Directory Tree\n* Files List\n\nUser can collapse any of them using divider handle and use only remaining one.\nIf the tree view is the only visible, it shows directories and files as well.      \n\n## Development version install\n``` bash\n\n    git clone https://github.com/majkelx/teda.git\n    cd teda\n    python -m venv venv\n    source ./venv/bin/activate\n    pip install -r requirements.txt\n    pip install -e .\n```\n\n## Bugs, remarks, greetings and contribution \nPlease use [GitHub issues tracker](https://github.com/majkelx/teda/issues) \nand [pull requests](https://github.com/majkelx/teda/pulls).\n\n\n@2020  [AkondLab](http://www.akond.com) for the [Araucaria Project](https://araucaria.camk.edu.pl).\n',
     'author': 'majkelx',
     'author_email': 'mkalusz@camk.edu.pl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `teda-3.1.0/PKG-INFO` & `teda-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teda
-Version: 3.1.0
+Version: 3.1.1
 Summary: Yet Another FITS Viewer
 License: MIT
 Author: majkelx
 Author-email: mkalusz@camk.edu.pl
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

