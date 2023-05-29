# Comparing `tmp/gopro-overlay-0.96.0.tar.gz` & `tmp/gopro-overlay-0.97.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gopro-overlay-0.96.0.tar", last modified: Fri May 26 15:11:51 2023, max compression
+gzip compressed data, was "gopro-overlay-0.97.0.tar", last modified: Mon May 29 08:59:07 2023, max compression
```

## Comparing `gopro-overlay-0.96.0.tar` & `gopro-overlay-0.97.0.tar`

### file list

```diff
@@ -1,145 +1,146 @@
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-26 15:11:51.954449 gopro-overlay-0.96.0/
--rw-rw-r--   0 richja    (1000) richja    (1000)    35691 2023-05-22 13:30:42.000000 gopro-overlay-0.96.0/LICENSE.md
--rw-rw-r--   0 richja    (1000) richja    (1000)       70 2022-02-02 12:18:46.000000 gopro-overlay-0.96.0/MANIFEST.in
--rw-rw-r--   0 richja    (1000) richja    (1000)    11681 2023-05-26 15:11:51.954449 gopro-overlay-0.96.0/PKG-INFO
--rw-rw-r--   0 richja    (1000) richja    (1000)    10888 2023-05-26 15:11:29.000000 gopro-overlay-0.96.0/README.md
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-26 15:11:51.942449 gopro-overlay-0.96.0/bin/
--rw-rw-r--   0 richja    (1000) richja    (1000)     3153 2022-05-23 15:18:05.000000 gopro-overlay-0.96.0/bin/gopro-contrib-data-extract.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1450 2022-02-03 15:47:43.000000 gopro-overlay-0.96.0/bin/gopro-cut.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    15036 2023-05-22 09:35:24.000000 gopro-overlay-0.96.0/bin/gopro-dashboard.py
--rwxrwxr-x   0 richja    (1000) richja    (1000)      770 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/bin/gopro-debug.py
--rwxrwxr-x   0 richja    (1000) richja    (1000)      596 2022-11-29 16:44:06.000000 gopro-overlay-0.96.0/bin/gopro-extract.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1035 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/bin/gopro-join.py
--rwxrwxr-x   0 richja    (1000) richja    (1000)     5527 2023-05-06 09:06:40.000000 gopro-overlay-0.96.0/bin/gopro-layout.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3702 2023-05-23 10:54:25.000000 gopro-overlay-0.96.0/bin/gopro-rename.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5783 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/bin/gopro-to-csv.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3412 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/bin/gopro-to-gpx.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-26 15:11:51.950449 gopro-overlay-0.96.0/gopro_overlay/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-02-02 11:42:38.000000 gopro-overlay-0.96.0/gopro_overlay/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      299 2023-05-26 15:09:52.000000 gopro-overlay-0.96.0/gopro_overlay/__version__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     7063 2023-05-22 08:55:54.000000 gopro-overlay-0.96.0/gopro_overlay/arguments.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5447 2023-05-08 10:30:40.000000 gopro-overlay-0.96.0/gopro_overlay/buffering.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      690 2022-11-29 17:00:53.000000 gopro-overlay-0.96.0/gopro_overlay/common.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      207 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/counter.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      483 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/date_overlap.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      531 2023-02-07 21:58:09.000000 gopro-overlay-0.96.0/gopro_overlay/dimensions.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1719 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/entry.py
--rw-rw-r--   0 richja    (1000) richja    (1000)       34 2022-11-23 14:47:58.000000 gopro-overlay-0.96.0/gopro_overlay/exceptions.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1345 2023-05-06 10:59:08.000000 gopro-overlay-0.96.0/gopro_overlay/execution.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/fake.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    10025 2023-05-22 09:32:45.000000 gopro-overlay-0.96.0/gopro_overlay/ffmpeg.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1285 2023-05-22 09:02:15.000000 gopro-overlay-0.96.0/gopro_overlay/ffmpeg_profile.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1958 2023-05-26 14:53:43.000000 gopro-overlay-0.96.0/gopro_overlay/filenaming.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2279 2023-05-01 11:53:38.000000 gopro-overlay-0.96.0/gopro_overlay/fit.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      122 2021-12-03 14:46:33.000000 gopro-overlay-0.96.0/gopro_overlay/font.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    10542 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/framemeta.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3000 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/framemeta_gpx.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      478 2022-05-27 13:38:56.000000 gopro-overlay-0.96.0/gopro_overlay/functional.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5703 2023-02-08 14:26:51.000000 gopro-overlay-0.96.0/gopro_overlay/geo.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2426 2023-02-09 10:45:34.000000 gopro-overlay-0.96.0/gopro_overlay/geo_render.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      525 2023-05-23 10:54:25.000000 gopro-overlay-0.96.0/gopro_overlay/geocode.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     8689 2023-03-15 08:32:52.000000 gopro-overlay-0.96.0/gopro_overlay/gpmd.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3275 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/gpmd_calculate.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3482 2022-11-23 14:02:47.000000 gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3420 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors_cori.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      525 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors_debug.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     8588 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors_gps.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2859 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors_grav.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4709 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors_xyz.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2963 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/gpx.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-26 15:11:51.950449 gopro-overlay-0.96.0/gopro_overlay/icons/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.96.0/gopro_overlay/icons/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    13448 2021-09-30 11:08:46.000000 gopro-overlay-0.96.0/gopro_overlay/icons/bicycle.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     8077 2021-09-30 11:08:22.000000 gopro-overlay-0.96.0/gopro_overlay/icons/car.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    22971 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/icons/faq.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    34059 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/icons/forbidden.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    19173 2021-09-20 15:22:09.000000 gopro-overlay-0.96.0/gopro_overlay/icons/gauge-1.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    15425 2021-09-20 15:24:33.000000 gopro-overlay-0.96.0/gopro_overlay/icons/gauge.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    12719 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/icons/gps_lock_2d.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     9239 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/icons/gps_lock_3d.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    32100 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/icons/gps_lock_none.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    28140 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/icons/gps_lock_unknown.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    13732 2021-09-21 11:34:05.000000 gopro-overlay-0.96.0/gopro_overlay/icons/heartbeat.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     5700 2021-09-30 11:09:17.000000 gopro-overlay-0.96.0/gopro_overlay/icons/ice-cream-van.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    20413 2021-09-20 15:26:49.000000 gopro-overlay-0.96.0/gopro_overlay/icons/mountain-range.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    13636 2021-09-20 15:27:04.000000 gopro-overlay-0.96.0/gopro_overlay/icons/mountain.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     8451 2022-11-06 20:16:59.000000 gopro-overlay-0.96.0/gopro_overlay/icons/power.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    14622 2021-09-20 15:58:10.000000 gopro-overlay-0.96.0/gopro_overlay/icons/ruler.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    15485 2021-09-20 15:27:45.000000 gopro-overlay-0.96.0/gopro_overlay/icons/slope-triangle.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    10147 2021-09-20 15:27:28.000000 gopro-overlay-0.96.0/gopro_overlay/icons/slope.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    15997 2021-09-20 15:22:31.000000 gopro-overlay-0.96.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     7655 2021-09-20 15:26:02.000000 gopro-overlay-0.96.0/gopro_overlay/icons/thermometer-1.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    10579 2021-09-20 15:25:42.000000 gopro-overlay-0.96.0/gopro_overlay/icons/thermometer.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    11096 2021-09-30 11:51:55.000000 gopro-overlay-0.96.0/gopro_overlay/icons/user.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     6958 2021-09-30 11:09:29.000000 gopro-overlay-0.96.0/gopro_overlay/icons/van-black-side-view.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     2074 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/journey.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3337 2023-05-06 09:06:40.000000 gopro-overlay-0.96.0/gopro_overlay/layout.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1025 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/layout_components.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    26241 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/layout_xml.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1067 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/layout_xml_attribute.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5498 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/layout_xml_cairo.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-26 15:11:51.954449 gopro-overlay-0.96.0/gopro_overlay/layouts/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.96.0/gopro_overlay/layouts/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3294 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/layouts/default-1920x1080.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     3515 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/layouts/default-2704x1520.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     3302 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/layouts/default-3840x2160.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     1510 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/layouts/example-2.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     8388 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/layouts/example.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     3802 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/layouts/power-1920x1080.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)      145 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/log.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      736 2021-09-30 11:21:57.000000 gopro-overlay-0.96.0/gopro_overlay/models.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      294 2022-02-09 11:24:51.000000 gopro-overlay-0.96.0/gopro_overlay/parsing.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     6672 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/point.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      575 2021-09-22 14:35:02.000000 gopro-overlay-0.96.0/gopro_overlay/privacy.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      329 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/process.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      891 2022-05-21 21:20:30.000000 gopro-overlay-0.96.0/gopro_overlay/progress_frames.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2297 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/rdp.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1224 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/smoothing.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2966 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/timeseries.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3005 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/timeseries_process.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1974 2022-09-24 19:15:22.000000 gopro-overlay-0.96.0/gopro_overlay/timeunits.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1287 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/timing.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      365 2022-11-29 15:04:43.000000 gopro-overlay-0.96.0/gopro_overlay/units.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-26 15:11:51.954449 gopro-overlay-0.96.0/gopro_overlay/widgets/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-11-02 15:56:34.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4453 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/asi.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2121 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/bar.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-26 15:11:51.954449 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2227 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/angle.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/annotation.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      643 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/background.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     6174 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/bordered.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      183 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/box.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3676 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/cairo.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1825 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/cap.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4190 2023-02-09 12:46:37.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/circuit.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1835 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/colour.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4777 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/ellipse.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      833 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/face.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5749 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/gauge_marker.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4184 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/gauge_round_254.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      424 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/line.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3619 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/needle.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      513 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/reading.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1923 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/scale.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      189 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/tick.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2412 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/chart.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3451 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/compass.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2226 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/compass_arrow.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      517 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/gps.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3687 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/gradient_bar.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2204 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/info.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    10811 2023-02-08 14:26:51.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/map.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      789 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/profile.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3107 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/text.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     8038 2023-05-06 09:06:40.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/widgets.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1509 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/widgets_experimental.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-26 15:11:51.950449 gopro-overlay-0.96.0/gopro_overlay.egg-info/
--rw-rw-r--   0 richja    (1000) richja    (1000)    11681 2023-05-26 15:11:51.000000 gopro-overlay-0.96.0/gopro_overlay.egg-info/PKG-INFO
--rw-rw-r--   0 richja    (1000) richja    (1000)     4192 2023-05-26 15:11:51.000000 gopro-overlay-0.96.0/gopro_overlay.egg-info/SOURCES.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)        1 2023-05-26 15:11:51.000000 gopro-overlay-0.96.0/gopro_overlay.egg-info/dependency_links.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)      132 2023-05-26 15:11:51.000000 gopro-overlay-0.96.0/gopro_overlay.egg-info/requires.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)       14 2023-05-26 15:11:51.000000 gopro-overlay-0.96.0/gopro_overlay.egg-info/top_level.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)       38 2023-05-26 15:11:51.954449 gopro-overlay-0.96.0/setup.cfg
--rw-rw-r--   0 richja    (1000) richja    (1000)     1933 2023-05-26 15:09:52.000000 gopro-overlay-0.96.0/setup.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 08:59:07.038049 gopro-overlay-0.97.0/
+-rw-rw-r--   0 richja    (1000) richja    (1000)    35691 2023-05-22 13:30:42.000000 gopro-overlay-0.97.0/LICENSE.md
+-rw-rw-r--   0 richja    (1000) richja    (1000)       70 2022-02-02 12:18:46.000000 gopro-overlay-0.97.0/MANIFEST.in
+-rw-rw-r--   0 richja    (1000) richja    (1000)    12013 2023-05-29 08:59:07.038049 gopro-overlay-0.97.0/PKG-INFO
+-rw-rw-r--   0 richja    (1000) richja    (1000)    11220 2023-05-29 08:57:30.000000 gopro-overlay-0.97.0/README.md
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 08:59:07.026049 gopro-overlay-0.97.0/bin/
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3153 2022-05-23 15:18:05.000000 gopro-overlay-0.97.0/bin/gopro-contrib-data-extract.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1450 2022-02-03 15:47:43.000000 gopro-overlay-0.97.0/bin/gopro-cut.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    15098 2023-05-29 08:34:54.000000 gopro-overlay-0.97.0/bin/gopro-dashboard.py
+-rwxrwxr-x   0 richja    (1000) richja    (1000)      770 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/bin/gopro-debug.py
+-rwxrwxr-x   0 richja    (1000) richja    (1000)      596 2022-11-29 16:44:06.000000 gopro-overlay-0.97.0/bin/gopro-extract.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1035 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/bin/gopro-join.py
+-rwxrwxr-x   0 richja    (1000) richja    (1000)     5603 2023-05-29 08:34:54.000000 gopro-overlay-0.97.0/bin/gopro-layout.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3702 2023-05-23 10:54:25.000000 gopro-overlay-0.97.0/bin/gopro-rename.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5783 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/bin/gopro-to-csv.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3412 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/bin/gopro-to-gpx.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 08:59:07.030049 gopro-overlay-0.97.0/gopro_overlay/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-02-02 11:42:38.000000 gopro-overlay-0.97.0/gopro_overlay/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      299 2023-05-29 08:55:36.000000 gopro-overlay-0.97.0/gopro_overlay/__version__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     7063 2023-05-22 08:55:54.000000 gopro-overlay-0.97.0/gopro_overlay/arguments.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5447 2023-05-08 10:30:40.000000 gopro-overlay-0.97.0/gopro_overlay/buffering.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      690 2022-11-29 17:00:53.000000 gopro-overlay-0.97.0/gopro_overlay/common.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      846 2023-05-27 14:18:06.000000 gopro-overlay-0.97.0/gopro_overlay/config.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      207 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/counter.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      483 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/date_overlap.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      531 2023-02-07 21:58:09.000000 gopro-overlay-0.97.0/gopro_overlay/dimensions.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1719 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/entry.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)       34 2022-11-23 14:47:58.000000 gopro-overlay-0.97.0/gopro_overlay/exceptions.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1345 2023-05-06 10:59:08.000000 gopro-overlay-0.97.0/gopro_overlay/execution.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/fake.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10025 2023-05-22 09:32:45.000000 gopro-overlay-0.97.0/gopro_overlay/ffmpeg.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1206 2023-05-27 14:12:20.000000 gopro-overlay-0.97.0/gopro_overlay/ffmpeg_profile.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1958 2023-05-26 14:53:43.000000 gopro-overlay-0.97.0/gopro_overlay/filenaming.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2279 2023-05-01 11:53:38.000000 gopro-overlay-0.97.0/gopro_overlay/fit.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      122 2021-12-03 14:46:33.000000 gopro-overlay-0.97.0/gopro_overlay/font.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10542 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/framemeta.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3000 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/framemeta_gpx.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      478 2022-05-27 13:38:56.000000 gopro-overlay-0.97.0/gopro_overlay/functional.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     6859 2023-05-29 08:34:54.000000 gopro-overlay-0.97.0/gopro_overlay/geo.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2426 2023-02-09 10:45:34.000000 gopro-overlay-0.97.0/gopro_overlay/geo_render.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      525 2023-05-23 10:54:25.000000 gopro-overlay-0.97.0/gopro_overlay/geocode.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8689 2023-03-15 08:32:52.000000 gopro-overlay-0.97.0/gopro_overlay/gpmd.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3275 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/gpmd_calculate.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3482 2022-11-23 14:02:47.000000 gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3420 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors_cori.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      525 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors_debug.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8588 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors_gps.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2859 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors_grav.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4709 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors_xyz.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2963 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/gpx.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 08:59:07.034049 gopro-overlay-0.97.0/gopro_overlay/icons/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.97.0/gopro_overlay/icons/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    13448 2021-09-30 11:08:46.000000 gopro-overlay-0.97.0/gopro_overlay/icons/bicycle.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8077 2021-09-30 11:08:22.000000 gopro-overlay-0.97.0/gopro_overlay/icons/car.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    22971 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/icons/faq.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    34059 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/icons/forbidden.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    19173 2021-09-20 15:22:09.000000 gopro-overlay-0.97.0/gopro_overlay/icons/gauge-1.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    15425 2021-09-20 15:24:33.000000 gopro-overlay-0.97.0/gopro_overlay/icons/gauge.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    12719 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/icons/gps_lock_2d.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     9239 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/icons/gps_lock_3d.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    32100 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/icons/gps_lock_none.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    28140 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/icons/gps_lock_unknown.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    13732 2021-09-21 11:34:05.000000 gopro-overlay-0.97.0/gopro_overlay/icons/heartbeat.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5700 2021-09-30 11:09:17.000000 gopro-overlay-0.97.0/gopro_overlay/icons/ice-cream-van.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    20413 2021-09-20 15:26:49.000000 gopro-overlay-0.97.0/gopro_overlay/icons/mountain-range.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    13636 2021-09-20 15:27:04.000000 gopro-overlay-0.97.0/gopro_overlay/icons/mountain.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8451 2022-11-06 20:16:59.000000 gopro-overlay-0.97.0/gopro_overlay/icons/power.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    14622 2021-09-20 15:58:10.000000 gopro-overlay-0.97.0/gopro_overlay/icons/ruler.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    15485 2021-09-20 15:27:45.000000 gopro-overlay-0.97.0/gopro_overlay/icons/slope-triangle.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10147 2021-09-20 15:27:28.000000 gopro-overlay-0.97.0/gopro_overlay/icons/slope.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    15997 2021-09-20 15:22:31.000000 gopro-overlay-0.97.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     7655 2021-09-20 15:26:02.000000 gopro-overlay-0.97.0/gopro_overlay/icons/thermometer-1.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10579 2021-09-20 15:25:42.000000 gopro-overlay-0.97.0/gopro_overlay/icons/thermometer.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    11096 2021-09-30 11:51:55.000000 gopro-overlay-0.97.0/gopro_overlay/icons/user.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     6958 2021-09-30 11:09:29.000000 gopro-overlay-0.97.0/gopro_overlay/icons/van-black-side-view.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2074 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/journey.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3337 2023-05-06 09:06:40.000000 gopro-overlay-0.97.0/gopro_overlay/layout.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1025 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/layout_components.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    26241 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/layout_xml.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1067 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/layout_xml_attribute.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5498 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/layout_xml_cairo.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 08:59:07.034049 gopro-overlay-0.97.0/gopro_overlay/layouts/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.97.0/gopro_overlay/layouts/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3294 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/layouts/default-1920x1080.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3515 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/layouts/default-2704x1520.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3302 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/layouts/default-3840x2160.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1510 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/layouts/example-2.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8388 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/layouts/example.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3802 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/layouts/power-1920x1080.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)      145 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/log.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      736 2021-09-30 11:21:57.000000 gopro-overlay-0.97.0/gopro_overlay/models.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      294 2022-02-09 11:24:51.000000 gopro-overlay-0.97.0/gopro_overlay/parsing.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     6672 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/point.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      575 2021-09-22 14:35:02.000000 gopro-overlay-0.97.0/gopro_overlay/privacy.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      329 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/process.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      891 2022-05-21 21:20:30.000000 gopro-overlay-0.97.0/gopro_overlay/progress_frames.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2297 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/rdp.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1224 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/smoothing.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2966 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/timeseries.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3005 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/timeseries_process.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1974 2022-09-24 19:15:22.000000 gopro-overlay-0.97.0/gopro_overlay/timeunits.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1287 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/timing.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      365 2022-11-29 15:04:43.000000 gopro-overlay-0.97.0/gopro_overlay/units.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 08:59:07.034049 gopro-overlay-0.97.0/gopro_overlay/widgets/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-11-02 15:56:34.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4453 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/asi.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2121 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/bar.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 08:59:07.038049 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2227 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/angle.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/annotation.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      643 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/background.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     6174 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/bordered.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      183 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/box.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3676 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/cairo.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1825 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/cap.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4190 2023-02-09 12:46:37.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/circuit.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1835 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/colour.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4777 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/ellipse.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      833 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/face.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5749 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/gauge_marker.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4184 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/gauge_round_254.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      424 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/line.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3619 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/needle.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      513 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/reading.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1923 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/scale.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      189 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/tick.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2412 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/chart.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3451 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/compass.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2226 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/compass_arrow.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      517 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/gps.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3687 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/gradient_bar.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2204 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/info.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10811 2023-02-08 14:26:51.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/map.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      789 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/profile.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3107 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/text.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8038 2023-05-06 09:06:40.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/widgets.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1509 2023-02-07 21:54:02.000000 gopro-overlay-0.97.0/gopro_overlay/widgets/widgets_experimental.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-29 08:59:07.030049 gopro-overlay-0.97.0/gopro_overlay.egg-info/
+-rw-rw-r--   0 richja    (1000) richja    (1000)    12013 2023-05-29 08:59:06.000000 gopro-overlay-0.97.0/gopro_overlay.egg-info/PKG-INFO
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4216 2023-05-29 08:59:07.000000 gopro-overlay-0.97.0/gopro_overlay.egg-info/SOURCES.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)        1 2023-05-29 08:59:06.000000 gopro-overlay-0.97.0/gopro_overlay.egg-info/dependency_links.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)      132 2023-05-29 08:59:06.000000 gopro-overlay-0.97.0/gopro_overlay.egg-info/requires.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)       14 2023-05-29 08:59:06.000000 gopro-overlay-0.97.0/gopro_overlay.egg-info/top_level.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)       38 2023-05-29 08:59:07.038049 gopro-overlay-0.97.0/setup.cfg
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1933 2023-05-29 08:55:36.000000 gopro-overlay-0.97.0/setup.py
```

### Comparing `gopro-overlay-0.96.0/LICENSE.md` & `gopro-overlay-0.97.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/PKG-INFO` & `gopro-overlay-0.97.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gopro-overlay
-Version: 0.96.0
+Version: 0.97.0
 Summary: Overlay graphics dashboards onto GoPro footage
 Home-page: https://github.com/time4tea/gopro-dashboard-overlay
 Author: James Richardson
 Author-email: james+gopro@time4tea.net
 License: MIT
 Project-URL: Source, https://github.com/time4tea/gopro-dashboard-overlay
 Classifier: Development Status :: 5 - Production/Stable
@@ -234,14 +234,16 @@
 https://github.com/progweb/gpx2video
 
 https://github.com/JuanIrache/gopro-telemetry
 
 ## Latest Changes
 
 If you find any issues with new releases, please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
+- 0.97.0 [Feature] Add new map style "local" - which will connect to a tileserver running locally on port 8000. This may be useful if you want to use a completely custom map - like a hand drawn one.
+  - For more details see: https://github.com/time4tea/gopro-dashboard-overlay/discussions/132 Thanks to @mattghub1 for the concept. 
 - 0.96.0 [Feature] Hopefully add support for older gopro files when joining. [#129](https://github.com/time4tea/gopro-dashboard-overlay/issues/129) Thanks [@FFMbyBicycle](https://github.com/FFMbyBicycle) for raising and some example code. 
 - 0.95.0 [Feature] Add api key support for geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-overlay/issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising.
 - 0.94.0 [Change] Update docker image to python3.11/ffmpeg 6.0 
 - 0.93.0 [Feature] Support for *fully gpu* decoding/overlay/encoding. Huge performance increase now possible. It takes a bit of work, but now can render at 12x realtime. See [docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md)
   - [Breaking] Remove support for `--output-size` as it didn't really work properly anyway. 
 - 0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially much faster rendering, but may not work on all architectures. Speed improvements highly dependent on `ffmpeg` performance. Likely much faster when using `--generate overlay`. Feedback welcomed.
 - 0.91.0 [Fix] Ignore FIT data items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for raising.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gopro-overlay Version: 0.96.0 Summary: Overlay
+Metadata-Version: 2.1 Name: gopro-overlay Version: 0.97.0 Summary: Overlay
 graphics dashboards onto GoPro footage Home-page: https://github.com/time4tea/
 gopro-dashboard-overlay Author: James Richardson Author-email:
 james+gopro@time4tea.net License: MIT Project-URL: Source, https://github.com/
 time4tea/gopro-dashboard-overlay Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.10
@@ -100,37 +100,41 @@
 Â© [Thunderforest](http://www.thunderforest.com/) ## References https://
 github.com/juanmcasillas/gopro2gpx https://github.com/JuanIrache/gopro-
 telemetry https://github.com/gopro/gpmf-parser https://coderunner.io/how-to-
 compress-gopro-movies-and-keep-metadata/ ## Other Related Software https://
 github.com/progweb/gpx2video https://github.com/JuanIrache/gopro-telemetry ##
 Latest Changes If you find any issues with new releases, please discuss in
 [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/
-discussions) - 0.96.0 [Feature] Hopefully add support for older gopro files
-when joining. [#129](https://github.com/time4tea/gopro-dashboard-overlay/
-issues/129) Thanks [@FFMbyBicycle](https://github.com/FFMbyBicycle) for raising
-and some example code. - 0.95.0 [Feature] Add api key support for geocode.xyz -
-[#117](https://github.com/time4tea/gopro-dashboard-overlay/issues/117) Thanks
-[@mishuha](https://github.com/mishuha) for raising. - 0.94.0 [Change] Update
-docker image to python3.11/ffmpeg 6.0 - 0.93.0 [Feature] Support for *fully
-gpu* decoding/overlay/encoding. Huge performance increase now possible. It
-takes a bit of work, but now can render at 12x realtime. See [docs/bin/
-PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md) - [Breaking] Remove
-support for `--output-size` as it didn't really work properly anyway. - 0.92.0
-[Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially much
-faster rendering, but may not work on all architectures. Speed improvements
-highly dependent on `ffmpeg` performance. Likely much faster when using `--
-generate overlay`. Feedback welcomed. - 0.91.0 [Fix] Ignore FIT data items that
-don't have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-
-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for
-raising. - 0.90.0 [Change] `cairo-circuit` now draws much more quickly. -
-[Change] Map rendering caches tile images more efficiently, so draws more
-quickly. - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` - A bit
-like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-round-
-annotated](docs/xml/examples/06-cairo-gauge-round-annotated) - 0.88.0 [Fix]
-Journey Map broke when no there were no locked GPS points in the movie. -
+discussions) - 0.97.0 [Feature] Add new map style "local" - which will connect
+to a tileserver running locally on port 8000. This may be useful if you want to
+use a completely custom map - like a hand drawn one. - For more details see:
+https://github.com/time4tea/gopro-dashboard-overlay/discussions/132 Thanks to
+@mattghub1 for the concept. - 0.96.0 [Feature] Hopefully add support for older
+gopro files when joining. [#129](https://github.com/time4tea/gopro-dashboard-
+overlay/issues/129) Thanks [@FFMbyBicycle](https://github.com/FFMbyBicycle) for
+raising and some example code. - 0.95.0 [Feature] Add api key support for
+geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-overlay/
+issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising. - 0.94.0
+[Change] Update docker image to python3.11/ffmpeg 6.0 - 0.93.0 [Feature]
+Support for *fully gpu* decoding/overlay/encoding. Huge performance increase
+now possible. It takes a bit of work, but now can render at 12x realtime. See
+[docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md) - [Breaking]
+Remove support for `--output-size` as it didn't really work properly anyway. -
+0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially
+much faster rendering, but may not work on all architectures. Speed
+improvements highly dependent on `ffmpeg` performance. Likely much faster when
+using `--generate overlay`. Feedback welcomed. - 0.91.0 [Fix] Ignore FIT data
+items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-
+dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/
+patkoscsaba) for raising. - 0.90.0 [Change] `cairo-circuit` now draws much more
+quickly. - [Change] Map rendering caches tile images more efficiently, so draws
+more quickly. - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` -
+A bit like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-
+round-annotated](docs/xml/examples/06-cairo-gauge-round-annotated) - 0.88.0
+[Fix] Journey Map broke when no there were no locked GPS points in the movie. -
 Thanks [@shahargli](https://github.com/shahargli) for reporting - 0.87.0 [Fix/
 Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`,
 instead use alpha of each colour. - 0.86.0 [Feature] New component `cairo-
 gauge-marker` - a nice clean gauge component, with a marker for the current
 value.. See docs [docs/xml/examples/06-cairo-gauge-marker](docs/xml/examples/
 06-cairo-gauge-marker) - 0.85.0 [Feature/Breaking Possibly] Add validation to
 attributes in layout files. This may cause some custom layouts to break! - But
```

### Comparing `gopro-overlay-0.96.0/README.md` & `gopro-overlay-0.97.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -213,14 +213,16 @@
 https://github.com/progweb/gpx2video
 
 https://github.com/JuanIrache/gopro-telemetry
 
 ## Latest Changes
 
 If you find any issues with new releases, please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
+- 0.97.0 [Feature] Add new map style "local" - which will connect to a tileserver running locally on port 8000. This may be useful if you want to use a completely custom map - like a hand drawn one.
+  - For more details see: https://github.com/time4tea/gopro-dashboard-overlay/discussions/132 Thanks to @mattghub1 for the concept. 
 - 0.96.0 [Feature] Hopefully add support for older gopro files when joining. [#129](https://github.com/time4tea/gopro-dashboard-overlay/issues/129) Thanks [@FFMbyBicycle](https://github.com/FFMbyBicycle) for raising and some example code. 
 - 0.95.0 [Feature] Add api key support for geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-overlay/issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising.
 - 0.94.0 [Change] Update docker image to python3.11/ffmpeg 6.0 
 - 0.93.0 [Feature] Support for *fully gpu* decoding/overlay/encoding. Huge performance increase now possible. It takes a bit of work, but now can render at 12x realtime. See [docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md)
   - [Breaking] Remove support for `--output-size` as it didn't really work properly anyway. 
 - 0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially much faster rendering, but may not work on all architectures. Speed improvements highly dependent on `ffmpeg` performance. Likely much faster when using `--generate overlay`. Feedback welcomed.
 - 0.91.0 [Fix] Ignore FIT data items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for raising.
```

#### html2text {}

```diff
@@ -89,41 +89,46 @@
 copyright) Some Maps Â© [Thunderforest](http://www.thunderforest.com/) ##
 References https://github.com/juanmcasillas/gopro2gpx https://github.com/
 JuanIrache/gopro-telemetry https://github.com/gopro/gpmf-parser https://
 coderunner.io/how-to-compress-gopro-movies-and-keep-metadata/ ## Other Related
 Software https://github.com/progweb/gpx2video https://github.com/JuanIrache/
 gopro-telemetry ## Latest Changes If you find any issues with new releases,
 please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-
-dashboard-overlay/discussions) - 0.96.0 [Feature] Hopefully add support for
-older gopro files when joining. [#129](https://github.com/time4tea/gopro-
-dashboard-overlay/issues/129) Thanks [@FFMbyBicycle](https://github.com/
-FFMbyBicycle) for raising and some example code. - 0.95.0 [Feature] Add api key
-support for geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-
-overlay/issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising.
-- 0.94.0 [Change] Update docker image to python3.11/ffmpeg 6.0 - 0.93.0
-[Feature] Support for *fully gpu* decoding/overlay/encoding. Huge performance
-increase now possible. It takes a bit of work, but now can render at 12x
-realtime. See [docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md) -
-[Breaking] Remove support for `--output-size` as it didn't really work properly
-anyway. - 0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering.
-Potentially much faster rendering, but may not work on all architectures. Speed
-improvements highly dependent on `ffmpeg` performance. Likely much faster when
-using `--generate overlay`. Feedback welcomed. - 0.91.0 [Fix] Ignore FIT data
-items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-
-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/
-patkoscsaba) for raising. - 0.90.0 [Change] `cairo-circuit` now draws much more
-quickly. - [Change] Map rendering caches tile images more efficiently, so draws
-more quickly. - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` -
-A bit like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-
-round-annotated](docs/xml/examples/06-cairo-gauge-round-annotated) - 0.88.0
-[Fix] Journey Map broke when no there were no locked GPS points in the movie. -
-Thanks [@shahargli](https://github.com/shahargli) for reporting - 0.87.0 [Fix/
-Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`,
-instead use alpha of each colour. - 0.86.0 [Feature] New component `cairo-
-gauge-marker` - a nice clean gauge component, with a marker for the current
-value.. See docs [docs/xml/examples/06-cairo-gauge-marker](docs/xml/examples/
-06-cairo-gauge-marker) - 0.85.0 [Feature/Breaking Possibly] Add validation to
-attributes in layout files. This may cause some custom layouts to break! - But
-they wouldn't have been working as intended. - [Change/Breaking] Change some
-`zone-bar` attribute names, aiming for standardisation - [Change/Breaking]
-Change some `cairo-circuit-map` attribute names, aiming for standardisation
-Older changes are in [CHANGELOG.md](CHANGELOG.md)
+dashboard-overlay/discussions) - 0.97.0 [Feature] Add new map style "local" -
+which will connect to a tileserver running locally on port 8000. This may be
+useful if you want to use a completely custom map - like a hand drawn one. -
+For more details see: https://github.com/time4tea/gopro-dashboard-overlay/
+discussions/132 Thanks to @mattghub1 for the concept. - 0.96.0 [Feature]
+Hopefully add support for older gopro files when joining. [#129](https://
+github.com/time4tea/gopro-dashboard-overlay/issues/129) Thanks [@FFMbyBicycle]
+(https://github.com/FFMbyBicycle) for raising and some example code. - 0.95.0
+[Feature] Add api key support for geocode.xyz - [#117](https://github.com/
+time4tea/gopro-dashboard-overlay/issues/117) Thanks [@mishuha](https://
+github.com/mishuha) for raising. - 0.94.0 [Change] Update docker image to
+python3.11/ffmpeg 6.0 - 0.93.0 [Feature] Support for *fully gpu* decoding/
+overlay/encoding. Huge performance increase now possible. It takes a bit of
+work, but now can render at 12x realtime. See [docs/bin/PERFORMANCE_GUIDE.md]
+(docs/bin/PERFORMANCE_GUIDE.md) - [Breaking] Remove support for `--output-size`
+as it didn't really work properly anyway. - 0.92.0 [Feature] `--double-buffer`
+- EXPERIMENTAL double-buffering. Potentially much faster rendering, but may not
+work on all architectures. Speed improvements highly dependent on `ffmpeg`
+performance. Likely much faster when using `--generate overlay`. Feedback
+welcomed. - 0.91.0 [Fix] Ignore FIT data items that don't have a GPS location.
+[#122](https://github.com/time4tea/gopro-dashboard-overlay/issues/122) Thanks
+[@patkoscsaba](https://github.com/patkoscsaba) for raising. - 0.90.0 [Change]
+`cairo-circuit` now draws much more quickly. - [Change] Map rendering caches
+tile images more efficiently, so draws more quickly. - 0.89.0 [Feature] New
+component `cairo-gauge-round-annotated` - A bit like a car speedometer - See
+docs [docs/xml/examples/06-cairo-gauge-round-annotated](docs/xml/examples/06-
+cairo-gauge-round-annotated) - 0.88.0 [Fix] Journey Map broke when no there
+were no locked GPS points in the movie. - Thanks [@shahargli](https://
+github.com/shahargli) for reporting - 0.87.0 [Fix/Breaking Possibly] `chart` -
+discovered a few bugs, now fixed. Removed `alpha`, instead use alpha of each
+colour. - 0.86.0 [Feature] New component `cairo-gauge-marker` - a nice clean
+gauge component, with a marker for the current value.. See docs [docs/xml/
+examples/06-cairo-gauge-marker](docs/xml/examples/06-cairo-gauge-marker) -
+0.85.0 [Feature/Breaking Possibly] Add validation to attributes in layout
+files. This may cause some custom layouts to break! - But they wouldn't have
+been working as intended. - [Change/Breaking] Change some `zone-bar` attribute
+names, aiming for standardisation - [Change/Breaking] Change some `cairo-
+circuit-map` attribute names, aiming for standardisation Older changes are in
+[CHANGELOG.md](CHANGELOG.md)
```

### Comparing `gopro-overlay-0.96.0/bin/gopro-contrib-data-extract.py` & `gopro-overlay-0.97.0/bin/gopro-contrib-data-extract.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/bin/gopro-cut.py` & `gopro-overlay-0.97.0/bin/gopro-cut.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/bin/gopro-dashboard.py` & `gopro-overlay-0.97.0/bin/gopro-dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 
 import progressbar
 
 from gopro_overlay import timeseries_process, progress_frames, gpx, fit
 from gopro_overlay.arguments import gopro_dashboard_arguments
 from gopro_overlay.buffering import SingleBuffer, DoubleBuffer
 from gopro_overlay.common import temp_file_name
+from gopro_overlay.config import Config
 from gopro_overlay.counter import ReasonCounter
 from gopro_overlay.date_overlap import DateRange
 from gopro_overlay.dimensions import dimension_from
 from gopro_overlay.execution import InProcessExecution
 from gopro_overlay.ffmpeg import FFMPEGOverlayVideo, FFMPEGOverlay, ffmpeg_is_installed, ffmpeg_libx264_is_installed, \
     find_streams, FFMPEGNull, ffmpeg_version
 from gopro_overlay.ffmpeg_profile import load_ffmpeg_profile
 from gopro_overlay.font import load_font
 from gopro_overlay.framemeta import framemeta_from
 from gopro_overlay.framemeta_gpx import merge_gpx_with_gopro, timeseries_to_framemeta
-from gopro_overlay.geo import CachingRenderer, api_key_finder
+from gopro_overlay.geo import MapRenderer, api_key_finder, MapStyler
 from gopro_overlay.gpmd import GPS_FIXED_VALUES, GPSFix
 from gopro_overlay.gpmd_visitors_gps import WorstOfGPSLockFilter, GPSLockTracker, GPSDOPFilter, GPSMaxSpeedFilter, GPSReportingFilter, GPSBBoxFilter, NullGPSLockFilter
 from gopro_overlay.layout import Overlay, speed_awareness_layout
 from gopro_overlay.layout_xml import layout_from_xml, load_xml_layout, Converters
 from gopro_overlay.log import log, fatal
 from gopro_overlay.point import Point
 from gopro_overlay.privacy import PrivacyZone, NoPrivacyZone
@@ -123,14 +124,16 @@
     # need in this scope for now
     inputpath: Optional[Path] = None
     generate = args.generate
 
     config_dir = args.config_dir
     config_dir.mkdir(exist_ok=True)
 
+    config_loader = Config(config_dir)
+
     cache_dir = args.cache_dir
     cache_dir.mkdir(exist_ok=True)
 
     with PoorTimer("program").timing():
 
         with PoorTimer("loading timeseries").timing():
 
@@ -254,28 +257,26 @@
             privacy_zone = PrivacyZone(
                 Point(float(lat), float(lon)),
                 units.Quantity(float(km), units.km)
             )
         else:
             privacy_zone = NoPrivacyZone()
 
-        key_finder = api_key_finder(args, args.config_dir)
-
-        with CachingRenderer(
+        with MapRenderer(
                 cache_dir=cache_dir,
-                style=args.map_style,
-                api_key_finder=key_finder).open() as renderer:
+                styler=MapStyler(api_key_finder=api_key_finder(config_loader, args))
+                ).open(args.map_style) as renderer:
 
             if args.profiler:
                 profiler = WidgetProfiler()
             else:
                 profiler = None
 
             if args.profile:
-                ffmpeg_options = load_ffmpeg_profile(config_dir, args.profile)
+                ffmpeg_options = load_ffmpeg_profile(config_loader, args.profile)
             else:
                 ffmpeg_options = None
 
             if args.show_ffmpeg:
                 redirect = None
             else:
                 redirect = temp_file_name()
```

### Comparing `gopro-overlay-0.96.0/bin/gopro-debug.py` & `gopro-overlay-0.97.0/bin/gopro-debug.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/bin/gopro-extract.py` & `gopro-overlay-0.97.0/bin/gopro-extract.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/bin/gopro-join.py` & `gopro-overlay-0.97.0/bin/gopro-join.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/bin/gopro-layout.py` & `gopro-overlay-0.97.0/bin/gopro-layout.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 from xml.etree import ElementTree
 
 from PIL import Image
 from pint import DimensionalityError
 
 from gopro_overlay import fake, geo, ffmpeg, timeseries_process
 from gopro_overlay.arguments import default_config_location
+from gopro_overlay.config import Config
 from gopro_overlay.dimensions import dimension_from, Dimension
 from gopro_overlay.ffmpeg import find_streams
 from gopro_overlay.font import load_font
 from gopro_overlay.framemeta import framemeta_from
-from gopro_overlay.geo import CachingRenderer, api_key_finder
+from gopro_overlay.geo import MapRenderer, api_key_finder, MapStyler
 from gopro_overlay.layout import Overlay
 from gopro_overlay.layout_xml import layout_from_xml, load_xml_layout
 from gopro_overlay.log import log
 from gopro_overlay.privacy import NoPrivacyZone
 from gopro_overlay.timeunits import timeunits
 from gopro_overlay.units import units
 from gopro_overlay.widgets.widgets import SimpleFrameSupplier
@@ -44,27 +45,28 @@
     parser.add_argument("--config-dir", help="Location of config files (api keys, profiles, ...)", type=pathlib.Path,
                         default=default_config_location)
     parser.add_argument("--cache-dir", help="Location of caches (map tiles, ...)", type=pathlib.Path,
                         default=default_config_location)
 
     parser.add_argument("--font", help="Selects a font", default="Roboto-Medium.ttf")
     parser.add_argument("--overlay-size", default="1920x1080", help="Size of frame, XxY, e.g. 1920x1080")
-    parser.add_argument("--gopro", type=pathlib.Path,  help="Use gopro video to supply a background image / journey")
+    parser.add_argument("--gopro", type=pathlib.Path, help="Use gopro video to supply a background image / journey")
 
     args = parser.parse_args()
 
     config_dir = args.config_dir
     config_dir.mkdir(exist_ok=True)
 
     cache_dir = args.cache_dir
     cache_dir.mkdir(exist_ok=True)
 
     font = load_font(args.font)
 
-    key_finder = api_key_finder(args, config_dir=config_dir)
+    config_loader = Config(config_dir)
+    key_finder = api_key_finder(config_loader, args)
 
     font = font.font_variant(size=16)
 
     layout_file: pathlib.Path = args.file
 
     rng = random.Random()
     rng.seed(12345)
@@ -94,18 +96,18 @@
             traceback.print_exc()
             log(f"{inputpath} appears to be located on a slow device. Please ensure both input and output files are on fast disks")
             exit(1)
 
     else:
         timeseries = fake.fake_framemeta(timedelta(minutes=5), step=timedelta(seconds=1), rng=rng, point_step=0.0001)
 
-    with CachingRenderer(
+    with MapRenderer(
             cache_dir=cache_dir,
-            style=args.map_style,
-            api_key_finder=key_finder).open() as renderer:
+            styler=MapStyler(api_key_finder=key_finder)
+    ).open(args.map_style) as renderer:
 
         last_updated = None
 
         while True:
             if not layout_file.exists():
                 log(f"Layout file not found: {layout_file}")
                 sleep(1)
```

### Comparing `gopro-overlay-0.96.0/bin/gopro-rename.py` & `gopro-overlay-0.97.0/bin/gopro-rename.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/bin/gopro-to-csv.py` & `gopro-overlay-0.97.0/bin/gopro-to-csv.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/bin/gopro-to-gpx.py` & `gopro-overlay-0.97.0/bin/gopro-to-gpx.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/arguments.py` & `gopro-overlay-0.97.0/gopro_overlay/arguments.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/buffering.py` & `gopro-overlay-0.97.0/gopro_overlay/buffering.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/common.py` & `gopro-overlay-0.97.0/gopro_overlay/common.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/dimensions.py` & `gopro-overlay-0.97.0/gopro_overlay/dimensions.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/entry.py` & `gopro-overlay-0.97.0/gopro_overlay/entry.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/execution.py` & `gopro-overlay-0.97.0/gopro_overlay/execution.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/fake.py` & `gopro-overlay-0.97.0/gopro_overlay/fake.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/ffmpeg.py` & `gopro-overlay-0.97.0/gopro_overlay/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/ffmpeg_profile.py` & `gopro-overlay-0.97.0/gopro_overlay/ffmpeg_profile.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 import json
 import pathlib
 
+from gopro_overlay.config import Config
 from gopro_overlay.ffmpeg import FFMPEGOptions
 
 
-def load_ffmpeg_profile(dir: pathlib.Path, profile: str):
-    profile_file = dir / "ffmpeg-profiles.json"
-    if not profile_file.exists():
-        raise ValueError(f"Expecting to find an FFMPEG Profile configuration at: {profile_file}")
-    with open(profile_file) as pf:
-        profile_json = json.load(pf)
+def load_ffmpeg_profile(config: Config, profile: str):
+    config_file = config.load("FFMPEG Profile", "ffmpeg-profiles.json")
+
+    profile_json = config_file.content
 
     if profile not in profile_json:
-        raise ValueError(f"Can't find key {profile} in {profile_file}")
+        raise ValueError(f"Can't find key {profile} in {config_file.location}")
 
     selected = profile_json[profile]
 
     if "input" in selected and type(selected["input"]) == list:
         input_options = selected["input"]
     else:
-        raise ValueError(f"Can't find input option list for key {profile} in {profile_file}")
+        raise ValueError(f"Can't find input option list for key {profile} in {config_file.location}")
 
     if "output" in selected and type(selected["output"]) == list:
         output_options = selected["output"]
     else:
-        raise ValueError(f"Can't find output option list for key {profile} in {profile_file}")
+        raise ValueError(f"Can't find output option list for key {profile} in {config_file.location}")
 
     filter_spec = None
 
     if "filter" in selected:
         if type(selected["filter"]) == str:
             filter_spec = selected["filter"]
         else:
```

### Comparing `gopro-overlay-0.96.0/gopro_overlay/filenaming.py` & `gopro-overlay-0.97.0/gopro_overlay/filenaming.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/fit.py` & `gopro-overlay-0.97.0/gopro_overlay/fit.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/framemeta.py` & `gopro-overlay-0.97.0/gopro_overlay/framemeta.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/framemeta_gpx.py` & `gopro-overlay-0.97.0/gopro_overlay/framemeta_gpx.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/geo.py` & `gopro-overlay-0.97.0/gopro_overlay/geo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import contextlib
 import dbm.ndbm
 import itertools
-import json
 import os
 import pathlib
 from functools import partial
+from typing import Optional, Tuple
 
 import geotiler
 from geotiler.cache import caching_downloader
 from geotiler.provider import MapProvider
 from geotiler.tile.io import fetch_tiles
 
+from gopro_overlay.config import Config
 from gopro_overlay.geo_render import my_render_map
 
 # most of the "stamen" maps in geotiler don't seem to work.
 map_styles = list(itertools.chain(
     ["osm"],
     [f"tf-{style}" for style in [
         "cycle", "transport", "landscape",
@@ -24,14 +25,15 @@
      ],
     [f"geo-{style}" for style in [
         "osm-carto", "osm-bright", "osm-bright-grey", "osm-bright-smooth",
         "klokantech-basic", "osm-liberty", "maptiler-3d", "toner", "toner-grey", "positron",
         "positron-blue", "positron-red", "dark-matter", "dark-matter-brown", "dark-matter-dark-grey",
         "dark-matter-dark-purple", "dark-matter-purple-roads", "dark-matter-yellow-roads"
     ]],
+    ["local"],
 ))
 
 
 def osm_attrs():
     return {
         "name": "OpenStreetMap",
         "attribution": "© OpenStreetMap contributors\nhttp://www.openstreetmap.org/copyright",
@@ -62,62 +64,88 @@
             "$MAPSTYLE$", style),
         "subdomains": ["a", "b", "c"],
         "api-key-ref": "thunderforest",
         "limit": 2,
     }
 
 
+def local_attrs(style):
+    return {
+        "name": "Local",
+        "url": "http://localhost:8000/{z}/{x}/{y}.{ext}",
+        "cache": False,
+        "limit": 2
+    }
+
+
 prefix_to_attrs = {
     "osm": osm_attrs,
     "tf": thunderforest_attrs,
-    "geo": geoapify_attrs
+    "geo": geoapify_attrs,
+    "local": local_attrs,
 }
 
 
+def configured_style(loader: Config, name: str) -> Optional[dict]:
+    config_file = loader.maybe("map-styles.json")
+    if config_file.exists():
+
+        if name in config_file.content:
+            attrs = config_file.content[name]
+
+            if not "url" in attrs:
+                raise ValueError(f"Required key 'url' not found for {name} in {config_file.location}")
+
+            return attrs
+    return None
+
+
 def attrs_for_style(name):
     if name == "osm":
         return osm_attrs()
 
-    prefix, style = name.split("-", 1)
+    if "-" in name:
+        prefix, style = name.split("-", 1)
+    else:
+        prefix = style = name
 
     if prefix in prefix_to_attrs:
         return prefix_to_attrs[prefix](style)
     else:
         raise KeyError(f"Unknown map provider: {name}")
 
 
-def provider_for_style(name, api_key_finder):
-    attrs = attrs_for_style(name)
-    if "api-key-ref" in attrs:
-        api_key = api_key_finder.find_api_key(attrs["api-key-ref"])
-    else:
-        api_key = None
-    return MapProvider(attrs, api_key)
-
-
 def dbm_downloader(dbm_file):
     def get_key(key):
         return dbm_file.get(key, None)
 
     def set_key(key, value):
         if value:
             dbm_file.setdefault(key, value)
 
     return partial(caching_downloader, get_key, set_key, fetch_tiles)
 
 
-def dbm_caching_renderer(provider, dbm_file):
+def dbm_caching_renderer(provider: MapProvider, dbm_file):
     def render(map, tiles=None, **kwargs):
         map.provider = provider
-        # return geotiler.render_map(map, tiles, downloader=dbm_downloader(dbm_file), **kwargs)
         return my_render_map(map, tiles, downloader=dbm_downloader(dbm_file), **kwargs)
 
     return render
 
 
+def no_caching_renderer(provider: MapProvider):
+    def render(map, tiles=None, **kwargs):
+        map.provider = provider
+
+        return geotiler.map.render_map(map, tiles, **kwargs)
+
+    return render
+
+
 class NullKeyFinder:
     def find_api_key(self, name):
         raise ValueError(f"I don't know any API keys. So can't give key for API '{name}'")
 
 
 class EnvKeyFinder:
     def find_api_key(self, name, env=os.environ):
@@ -136,26 +164,25 @@
         if key is not None:
             return key
 
         raise ValueError(f"No api key for {name}")
 
 
 class ConfigKeyFinder:
-    def __init__(self, config_dir: pathlib.Path):
-        self.config_dir = config_dir
+    def __init__(self, loader: Config):
+        self.loader = loader
 
     def find_api_key(self, name):
-        config_file = self.config_dir / "map-api-keys.json"
-        if config_file.exists():
-            config = json.loads(config_file.read_text())
+        config = self.loader.maybe("map-api-keys.json")
 
-            if name in config:
-                return config[name]
+        if config.exists():
+            if name in config.content:
+                return config.content[name]
 
-        raise ValueError(f"No api key for {name} in {config_file}")
+        raise ValueError(f"No api key for {name} in {config.location}")
 
 
 class CompositeKeyFinder:
     def __init__(self, *others):
         self.others = others
 
     def find_api_key(self, name):
@@ -171,28 +198,49 @@
     def __init__(self, key):
         self.key = key
 
     def find_api_key(self, name):
         return self.key
 
 
-def api_key_finder(args, config_dir: pathlib.Path):
+def api_key_finder(loader: Config, args):
     return CompositeKeyFinder(
         ArgsKeyFinder(args),
         EnvKeyFinder(),
-        ConfigKeyFinder(config_dir)
+        ConfigKeyFinder(loader)
     )
 
 
-class CachingRenderer:
+class MapStyler:
+    def __init__(self, api_key_finder=NullKeyFinder()):
+        self.api_key_finder = api_key_finder
 
-    def __init__(self, cache_dir: pathlib.Path, style="osm", api_key_finder=None):
-        if api_key_finder is None:
-            api_key_finder = NullKeyFinder()
+    def provide(self, style: str = "osm") -> Tuple[dict, str]:
+        return self.provider_for_style(style, self.api_key_finder)
 
+    def provider_for_style(self, name, api_key_finder) -> Tuple[dict, str]:
+        attrs = attrs_for_style(name)
+        if "api-key-ref" in attrs:
+            api_key = api_key_finder.find_api_key(attrs["api-key-ref"])
+        else:
+            api_key = None
+        return attrs, api_key
+
+
+class MapRenderer:
+
+    def __init__(self, cache_dir: pathlib.Path, styler: MapStyler):
         self.cache_dir = cache_dir
-        self.provider = provider_for_style(style, api_key_finder)
+        self.styler = styler
 
     @contextlib.contextmanager
-    def open(self):
-        with dbm.ndbm.open(str(self.cache_dir.joinpath("tilecache.ndbm")), "c") as db:
-            yield dbm_caching_renderer(self.provider, db)
+    def open(self, style: str = "osm"):
+
+        attrs, key = self.styler.provide(style)
+
+        map = MapProvider(attrs, key)
+
+        if attrs.get("cache", True):
+            with dbm.ndbm.open(str(self.cache_dir.joinpath("tilecache.ndbm")), "c") as db:
+                yield dbm_caching_renderer(map, db)
+        else:
+            yield no_caching_renderer(map)
```

### Comparing `gopro-overlay-0.96.0/gopro_overlay/geo_render.py` & `gopro-overlay-0.97.0/gopro_overlay/geo_render.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/geocode.py` & `gopro-overlay-0.97.0/gopro_overlay/geocode.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/gpmd.py` & `gopro-overlay-0.97.0/gopro_overlay/gpmd.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/gpmd_calculate.py` & `gopro-overlay-0.97.0/gopro_overlay/gpmd_calculate.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors.py` & `gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors_cori.py` & `gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors_cori.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors_debug.py` & `gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors_debug.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors_gps.py` & `gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors_gps.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors_grav.py` & `gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors_grav.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors_xyz.py` & `gopro-overlay-0.97.0/gopro_overlay/gpmd_visitors_xyz.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/gpx.py` & `gopro-overlay-0.97.0/gopro_overlay/gpx.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/bicycle.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/bicycle.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/car.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/car.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/faq.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/faq.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/forbidden.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/forbidden.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/gauge-1.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/gauge-1.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/gauge.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/gauge.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/gps_lock_2d.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/gps_lock_2d.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/gps_lock_3d.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/gps_lock_3d.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/gps_lock_none.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/gps_lock_none.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/gps_lock_unknown.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/gps_lock_unknown.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/heartbeat.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/heartbeat.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/ice-cream-van.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/ice-cream-van.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/mountain-range.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/mountain-range.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/mountain.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/mountain.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/power.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/power.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/ruler.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/ruler.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/slope-triangle.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/slope-triangle.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/slope.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/slope.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/thermometer-1.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/thermometer-1.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/thermometer.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/thermometer.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/user.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/user.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/icons/van-black-side-view.png` & `gopro-overlay-0.97.0/gopro_overlay/icons/van-black-side-view.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/journey.py` & `gopro-overlay-0.97.0/gopro_overlay/journey.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/layout.py` & `gopro-overlay-0.97.0/gopro_overlay/layout.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/layout_components.py` & `gopro-overlay-0.97.0/gopro_overlay/layout_components.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/layout_xml.py` & `gopro-overlay-0.97.0/gopro_overlay/layout_xml.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/layout_xml_attribute.py` & `gopro-overlay-0.97.0/gopro_overlay/layout_xml_attribute.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/layout_xml_cairo.py` & `gopro-overlay-0.97.0/gopro_overlay/layout_xml_cairo.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/layouts/default-1920x1080.xml` & `gopro-overlay-0.97.0/gopro_overlay/layouts/default-1920x1080.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/layouts/default-2704x1520.xml` & `gopro-overlay-0.97.0/gopro_overlay/layouts/default-2704x1520.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/layouts/default-3840x2160.xml` & `gopro-overlay-0.97.0/gopro_overlay/layouts/default-3840x2160.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/layouts/example-2.xml` & `gopro-overlay-0.97.0/gopro_overlay/layouts/example-2.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/layouts/example.xml` & `gopro-overlay-0.97.0/gopro_overlay/layouts/example.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/layouts/power-1920x1080.xml` & `gopro-overlay-0.97.0/gopro_overlay/layouts/power-1920x1080.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/models.py` & `gopro-overlay-0.97.0/gopro_overlay/models.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/point.py` & `gopro-overlay-0.97.0/gopro_overlay/point.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/privacy.py` & `gopro-overlay-0.97.0/gopro_overlay/privacy.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/progress_frames.py` & `gopro-overlay-0.97.0/gopro_overlay/progress_frames.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/rdp.py` & `gopro-overlay-0.97.0/gopro_overlay/rdp.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/smoothing.py` & `gopro-overlay-0.97.0/gopro_overlay/smoothing.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/timeseries.py` & `gopro-overlay-0.97.0/gopro_overlay/timeseries.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/timeseries_process.py` & `gopro-overlay-0.97.0/gopro_overlay/timeseries_process.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/timeunits.py` & `gopro-overlay-0.97.0/gopro_overlay/timeunits.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/timing.py` & `gopro-overlay-0.97.0/gopro_overlay/timing.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/asi.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/asi.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/bar.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/bar.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/angle.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/angle.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/annotation.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/annotation.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/background.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/background.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/bordered.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/bordered.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/cairo.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/cairo.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/cap.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/cap.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/circuit.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/circuit.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/colour.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/colour.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/ellipse.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/ellipse.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/face.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/face.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/gauge_marker.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/gauge_marker.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/gauge_round_254.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/gauge_round_254.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/needle.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/needle.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/reading.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/reading.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/scale.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/cairo/scale.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/chart.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/chart.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/compass.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/compass.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/compass_arrow.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/compass_arrow.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/gps.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/gps.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/gradient_bar.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/gradient_bar.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/info.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/info.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/map.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/map.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/profile.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/profile.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/text.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/text.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/widgets.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/widgets.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay/widgets/widgets_experimental.py` & `gopro-overlay-0.97.0/gopro_overlay/widgets/widgets_experimental.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.96.0/gopro_overlay.egg-info/PKG-INFO` & `gopro-overlay-0.97.0/gopro_overlay.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gopro-overlay
-Version: 0.96.0
+Version: 0.97.0
 Summary: Overlay graphics dashboards onto GoPro footage
 Home-page: https://github.com/time4tea/gopro-dashboard-overlay
 Author: James Richardson
 Author-email: james+gopro@time4tea.net
 License: MIT
 Project-URL: Source, https://github.com/time4tea/gopro-dashboard-overlay
 Classifier: Development Status :: 5 - Production/Stable
@@ -234,14 +234,16 @@
 https://github.com/progweb/gpx2video
 
 https://github.com/JuanIrache/gopro-telemetry
 
 ## Latest Changes
 
 If you find any issues with new releases, please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
+- 0.97.0 [Feature] Add new map style "local" - which will connect to a tileserver running locally on port 8000. This may be useful if you want to use a completely custom map - like a hand drawn one.
+  - For more details see: https://github.com/time4tea/gopro-dashboard-overlay/discussions/132 Thanks to @mattghub1 for the concept. 
 - 0.96.0 [Feature] Hopefully add support for older gopro files when joining. [#129](https://github.com/time4tea/gopro-dashboard-overlay/issues/129) Thanks [@FFMbyBicycle](https://github.com/FFMbyBicycle) for raising and some example code. 
 - 0.95.0 [Feature] Add api key support for geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-overlay/issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising.
 - 0.94.0 [Change] Update docker image to python3.11/ffmpeg 6.0 
 - 0.93.0 [Feature] Support for *fully gpu* decoding/overlay/encoding. Huge performance increase now possible. It takes a bit of work, but now can render at 12x realtime. See [docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md)
   - [Breaking] Remove support for `--output-size` as it didn't really work properly anyway. 
 - 0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially much faster rendering, but may not work on all architectures. Speed improvements highly dependent on `ffmpeg` performance. Likely much faster when using `--generate overlay`. Feedback welcomed.
 - 0.91.0 [Fix] Ignore FIT data items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for raising.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gopro-overlay Version: 0.96.0 Summary: Overlay
+Metadata-Version: 2.1 Name: gopro-overlay Version: 0.97.0 Summary: Overlay
 graphics dashboards onto GoPro footage Home-page: https://github.com/time4tea/
 gopro-dashboard-overlay Author: James Richardson Author-email:
 james+gopro@time4tea.net License: MIT Project-URL: Source, https://github.com/
 time4tea/gopro-dashboard-overlay Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.10
@@ -100,37 +100,41 @@
 Â© [Thunderforest](http://www.thunderforest.com/) ## References https://
 github.com/juanmcasillas/gopro2gpx https://github.com/JuanIrache/gopro-
 telemetry https://github.com/gopro/gpmf-parser https://coderunner.io/how-to-
 compress-gopro-movies-and-keep-metadata/ ## Other Related Software https://
 github.com/progweb/gpx2video https://github.com/JuanIrache/gopro-telemetry ##
 Latest Changes If you find any issues with new releases, please discuss in
 [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/
-discussions) - 0.96.0 [Feature] Hopefully add support for older gopro files
-when joining. [#129](https://github.com/time4tea/gopro-dashboard-overlay/
-issues/129) Thanks [@FFMbyBicycle](https://github.com/FFMbyBicycle) for raising
-and some example code. - 0.95.0 [Feature] Add api key support for geocode.xyz -
-[#117](https://github.com/time4tea/gopro-dashboard-overlay/issues/117) Thanks
-[@mishuha](https://github.com/mishuha) for raising. - 0.94.0 [Change] Update
-docker image to python3.11/ffmpeg 6.0 - 0.93.0 [Feature] Support for *fully
-gpu* decoding/overlay/encoding. Huge performance increase now possible. It
-takes a bit of work, but now can render at 12x realtime. See [docs/bin/
-PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md) - [Breaking] Remove
-support for `--output-size` as it didn't really work properly anyway. - 0.92.0
-[Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially much
-faster rendering, but may not work on all architectures. Speed improvements
-highly dependent on `ffmpeg` performance. Likely much faster when using `--
-generate overlay`. Feedback welcomed. - 0.91.0 [Fix] Ignore FIT data items that
-don't have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-
-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for
-raising. - 0.90.0 [Change] `cairo-circuit` now draws much more quickly. -
-[Change] Map rendering caches tile images more efficiently, so draws more
-quickly. - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` - A bit
-like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-round-
-annotated](docs/xml/examples/06-cairo-gauge-round-annotated) - 0.88.0 [Fix]
-Journey Map broke when no there were no locked GPS points in the movie. -
+discussions) - 0.97.0 [Feature] Add new map style "local" - which will connect
+to a tileserver running locally on port 8000. This may be useful if you want to
+use a completely custom map - like a hand drawn one. - For more details see:
+https://github.com/time4tea/gopro-dashboard-overlay/discussions/132 Thanks to
+@mattghub1 for the concept. - 0.96.0 [Feature] Hopefully add support for older
+gopro files when joining. [#129](https://github.com/time4tea/gopro-dashboard-
+overlay/issues/129) Thanks [@FFMbyBicycle](https://github.com/FFMbyBicycle) for
+raising and some example code. - 0.95.0 [Feature] Add api key support for
+geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-overlay/
+issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising. - 0.94.0
+[Change] Update docker image to python3.11/ffmpeg 6.0 - 0.93.0 [Feature]
+Support for *fully gpu* decoding/overlay/encoding. Huge performance increase
+now possible. It takes a bit of work, but now can render at 12x realtime. See
+[docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md) - [Breaking]
+Remove support for `--output-size` as it didn't really work properly anyway. -
+0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially
+much faster rendering, but may not work on all architectures. Speed
+improvements highly dependent on `ffmpeg` performance. Likely much faster when
+using `--generate overlay`. Feedback welcomed. - 0.91.0 [Fix] Ignore FIT data
+items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-
+dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/
+patkoscsaba) for raising. - 0.90.0 [Change] `cairo-circuit` now draws much more
+quickly. - [Change] Map rendering caches tile images more efficiently, so draws
+more quickly. - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` -
+A bit like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-
+round-annotated](docs/xml/examples/06-cairo-gauge-round-annotated) - 0.88.0
+[Fix] Journey Map broke when no there were no locked GPS points in the movie. -
 Thanks [@shahargli](https://github.com/shahargli) for reporting - 0.87.0 [Fix/
 Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`,
 instead use alpha of each colour. - 0.86.0 [Feature] New component `cairo-
 gauge-marker` - a nice clean gauge component, with a marker for the current
 value.. See docs [docs/xml/examples/06-cairo-gauge-marker](docs/xml/examples/
 06-cairo-gauge-marker) - 0.85.0 [Feature/Breaking Possibly] Add validation to
 attributes in layout files. This may cause some custom layouts to break! - But
```

### Comparing `gopro-overlay-0.96.0/gopro_overlay.egg-info/SOURCES.txt` & `gopro-overlay-0.97.0/gopro_overlay.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 bin/gopro-to-csv.py
 bin/gopro-to-gpx.py
 gopro_overlay/__init__.py
 gopro_overlay/__version__.py
 gopro_overlay/arguments.py
 gopro_overlay/buffering.py
 gopro_overlay/common.py
+gopro_overlay/config.py
 gopro_overlay/counter.py
 gopro_overlay/date_overlap.py
 gopro_overlay/dimensions.py
 gopro_overlay/entry.py
 gopro_overlay/exceptions.py
 gopro_overlay/execution.py
 gopro_overlay/fake.py
```

### Comparing `gopro-overlay-0.96.0/setup.py` & `gopro-overlay-0.97.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 test_requirements = [
     "pytest"
 ]
 
 setup(
     name="gopro-overlay",
-    version="0.96.0",
+    version="0.97.0",
     description="Overlay graphics dashboards onto GoPro footage",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/time4tea/gopro-dashboard-overlay",
     author="James Richardson",
     author_email="james+gopro@time4tea.net",
     license="MIT",
```

