# Comparing `tmp/solox-2.6.3.tar.gz` & `tmp/solox-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/SoloX/SoloX/dist/.tmp-rb7jp8we/solox-2.6.3.tar", last modified: Wed May 17 01:23:16 2023, max compression
+gzip compressed data, was "/home/runner/work/SoloX/SoloX/dist/.tmp-mq4e96qp/solox-2.6.4.tar", last modified: Mon May 29 08:34:00 2023, max compression
```

## Comparing `solox-2.6.3.tar` & `solox-2.6.4.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-17 01:23:07.000000 solox-2.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-17 01:23:07.000000 solox-2.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-17 01:23:16.000000 solox-2.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-17 01:23:07.000000 solox-2.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-17 01:23:16.000000 solox-2.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-17 01:23:07.000000 solox-2.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-17 01:23:07.000000 solox-2.6.3/solox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-17 01:23:07.000000 solox-2.6.3/solox/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-17 01:23:07.000000 solox-2.6.3/solox/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/public/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12374 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/_iosPerf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/public/adb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/public/adb/linux/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/adb/linux/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/public/adb/linux_arm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/adb/linux_arm/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/public/adb/mac/
--rwxr-xr-x   0 runner    (1001) docker     (123)  7328624 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/adb/mac/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/public/adb/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/adb/windows/AdbWinApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/adb/windows/AdbWinUsbApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/adb/windows/adb.exe
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)    22010 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/apm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/apm_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)    31724 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    20468 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/fps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/public/iosperf/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30884 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_crash.py
--rw-r--r--   0 runner    (1001) docker     (123)    41300 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_hexdump.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_imagemounter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_installation.py
--rw-r--r--   0 runner    (1001) docker     (123)    39237 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_ipautil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_perf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_safe_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_wdaproxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/bplist.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/plistlib2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/requests_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/struct2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/public/report_template/
--rw-r--r--   0 runner    (1001) docker     (123)    29240 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/report_template/android.html
--rw-r--r--   0 runner    (1001) docker     (123)    29276 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/report_template/ios.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/css/highlight.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/css/select2-bootstrap-5-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/css/select2-bootstrap-5-theme.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/css/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/css/sweetalert2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/css/tabler.demo.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/css/tabler.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/static/image/
--rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/image/404.png
--rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/image/500.png
--rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/image/avatar.png
--rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/image/coffee.png
--rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/image/empty.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/static/image/readme/
--rw-r--r--   0 runner    (1001) docker     (123)   796212 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/image/readme/home.png
--rw-r--r--   0 runner    (1001) docker     (123)   699302 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/image/readme/pk.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/js/apexcharts.js
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/js/gray.js
--rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/js/highstock.js
--rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/js/html2canvas.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/js/select2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/js/socket.io.js
--rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/js/sweetalert2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/js/tabler.demo.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/js/tabler.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/static/logo/
--rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/logo/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-05-17 01:23:07.000000 solox-2.6.3/solox/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-05-17 01:23:07.000000 solox-2.6.3/solox/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)    65740 2023-05-17 01:23:07.000000 solox-2.6.3/solox/templates/analysis.html
--rw-r--r--   0 runner    (1001) docker     (123)    43308 2023-05-17 01:23:07.000000 solox-2.6.3/solox/templates/analysis_compare.html
--rw-r--r--   0 runner    (1001) docker     (123)    38287 2023-05-17 01:23:07.000000 solox-2.6.3/solox/templates/analysis_pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    33714 2023-05-17 01:23:07.000000 solox-2.6.3/solox/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)   101070 2023-05-17 01:23:07.000000 solox-2.6.3/solox/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    55676 2023-05-17 01:23:07.000000 solox-2.6.3/solox/templates/pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    34893 2023-05-17 01:23:07.000000 solox-2.6.3/solox/templates/report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/view/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-17 01:23:07.000000 solox-2.6.3/solox/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-05-17 01:23:07.000000 solox-2.6.3/solox/view/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-05-17 01:23:07.000000 solox-2.6.3/solox/view/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-17 01:23:07.000000 solox-2.6.3/solox/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-17 01:23:16.000000 solox-2.6.3/solox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-17 01:23:16.000000 solox-2.6.3/solox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 01:23:16.000000 solox-2.6.3/solox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 01:23:16.000000 solox-2.6.3/solox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-17 01:23:16.000000 solox-2.6.3/solox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-29 08:33:51.000000 solox-2.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-29 08:33:51.000000 solox-2.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-05-29 08:34:00.000000 solox-2.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-29 08:33:51.000000 solox-2.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-29 08:34:00.000000 solox-2.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-29 08:33:51.000000 solox-2.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-29 08:33:51.000000 solox-2.6.4/solox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-29 08:33:51.000000 solox-2.6.4/solox/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-29 08:33:51.000000 solox-2.6.4/solox/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/public/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12374 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/_iosPerf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/public/adb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/public/adb/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/adb/linux/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/public/adb/linux_arm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/adb/linux_arm/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/public/adb/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)  7328624 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/adb/mac/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/public/adb/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/adb/windows/AdbWinApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/adb/windows/AdbWinUsbApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/adb/windows/adb.exe
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22010 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/apm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/apm_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31724 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20468 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/fps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/public/iosperf/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30884 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_crash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41300 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_hexdump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_imagemounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39237 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_ipautil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_safe_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_wdaproxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/bplist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/plistlib2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/requests_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/struct2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/public/report_template/
+-rw-r--r--   0 runner    (1001) docker     (123)    29240 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/report_template/android.html
+-rw-r--r--   0 runner    (1001) docker     (123)    29276 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/report_template/ios.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/css/highlight.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/css/select2-bootstrap-5-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/css/select2-bootstrap-5-theme.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/css/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/css/sweetalert2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/css/tabler.demo.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/css/tabler.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/static/image/
+-rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/image/404.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/image/500.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/image/avatar.png
+-rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/image/coffee.png
+-rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/image/empty.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/static/image/readme/
+-rw-r--r--   0 runner    (1001) docker     (123)   796212 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/image/readme/home.png
+-rw-r--r--   0 runner    (1001) docker     (123)   699302 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/image/readme/pk.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/js/apexcharts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/js/gray.js
+-rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/js/highstock.js
+-rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/js/html2canvas.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/js/select2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/js/socket.io.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/js/sweetalert2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/js/tabler.demo.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/js/tabler.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/static/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/logo/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-05-29 08:33:51.000000 solox-2.6.4/solox/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-05-29 08:33:51.000000 solox-2.6.4/solox/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)    65740 2023-05-29 08:33:51.000000 solox-2.6.4/solox/templates/analysis.html
+-rw-r--r--   0 runner    (1001) docker     (123)    43308 2023-05-29 08:33:51.000000 solox-2.6.4/solox/templates/analysis_compare.html
+-rw-r--r--   0 runner    (1001) docker     (123)    38287 2023-05-29 08:33:51.000000 solox-2.6.4/solox/templates/analysis_pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    33714 2023-05-29 08:33:51.000000 solox-2.6.4/solox/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)   101171 2023-05-29 08:33:51.000000 solox-2.6.4/solox/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    55676 2023-05-29 08:33:51.000000 solox-2.6.4/solox/templates/pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    34893 2023-05-29 08:33:51.000000 solox-2.6.4/solox/templates/report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/view/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-29 08:33:51.000000 solox-2.6.4/solox/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-05-29 08:33:51.000000 solox-2.6.4/solox/view/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-05-29 08:33:51.000000 solox-2.6.4/solox/view/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-29 08:33:51.000000 solox-2.6.4/solox/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-05-29 08:34:00.000000 solox-2.6.4/solox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-29 08:34:00.000000 solox-2.6.4/solox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 08:34:00.000000 solox-2.6.4/solox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-29 08:34:00.000000 solox-2.6.4/solox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 08:34:00.000000 solox-2.6.4/solox.egg-info/top_level.txt
```

### Comparing `solox-2.6.3/LICENSE` & `solox-2.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/PKG-INFO` & `solox-2.6.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solox
-Version: 2.6.3
+Version: 2.6.4
 Summary: SoloX - Real-time collection tool for Android/iOS performance data.
 Home-page: https://github.com/smart-test-ti/SoloX
 Author: Rafa Chen
 Author-email: rafacheninc@gamil.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -33,15 +33,15 @@
 
 ## 🔎Preview
 
 SoloX - Real-time collection tool for Android/iOS performance data.
 
 We are committed to solving inefficient, cumbersome test execution, and our goal is Simple Test In SoloX!
 
-<img src="https://cdn.nlark.com/yuque/0/2022/png/153412/1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0"  width="100%" >
+![preview](https://github.com/smart-test-ti/SoloX/assets/24454096/6941452f-6410-4730-a532-0d69d0f7fdb8)
 
 ## 📦Requirements
 
 - Install Python 3.10 + [**Download**](https://www.python.org/downloads/)
 - Install adb and configure environment variables (SoloX's  adb may not necessarily fit your computer) [**Download**](https://developer.android.com/studio/releases/platform-tools)
 
 💡 Python 3.6 ~ 3.9 , please download a version of solox lower than 2.5.4. 
@@ -138,15 +138,15 @@
 * **Data Integrality:** We provide the data about CPU, GPU, Memory, Battery, Network,FPS, Jank, etc., which you may easy to get.
 * **Beautiful Report:** A beautiful and detailed report analysis, where to store, visualize, edit, manage, and download all the test cases collected with SoloX no matter where you are or when is it.
 * **Useful Monitoring Settings:** Support setting alarm values, collecting duration, and accessing mobile devices on other PC machines during the monitoring process.
 * **PK Model:** Supports simultaneous comparative testing of two mobile devices.
   - 🌱2-devices: test the same app on two different phones.
   - 🌱2-apps: test two different apps on two phones with the same configuration.
 
-* **Collect in python/API:** Support Python and API to collect performance data, helping users easily integrate into automated testing processes.
+* **Collect In Python/API:** Support Python and API to collect performance data, helping users easily integrate into automated testing processes.
 
 ## Browser
 
 <img src="https://cdn.nlark.com/yuque/0/2023/png/153412/1677553244198-96ce5709-f33f-4038-888f-f330d1f74450.png" alt="Chrome" width="50px" height="50px" />
 
 ## Terminal
```

### Comparing `solox-2.6.3/README.md` & `solox-2.6.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 ## 🔎Preview
 
 SoloX - Real-time collection tool for Android/iOS performance data.
 
 We are committed to solving inefficient, cumbersome test execution, and our goal is Simple Test In SoloX!
 
-<img src="https://cdn.nlark.com/yuque/0/2022/png/153412/1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0"  width="100%" >
+![preview](https://github.com/smart-test-ti/SoloX/assets/24454096/6941452f-6410-4730-a532-0d69d0f7fdb8)
 
 ## 📦Requirements
 
 - Install Python 3.10 + [**Download**](https://www.python.org/downloads/)
 - Install adb and configure environment variables (SoloX's  adb may not necessarily fit your computer) [**Download**](https://developer.android.com/studio/releases/platform-tools)
 
 💡 Python 3.6 ~ 3.9 , please download a version of solox lower than 2.5.4. 
@@ -123,15 +123,15 @@
 * **Data Integrality:** We provide the data about CPU, GPU, Memory, Battery, Network,FPS, Jank, etc., which you may easy to get.
 * **Beautiful Report:** A beautiful and detailed report analysis, where to store, visualize, edit, manage, and download all the test cases collected with SoloX no matter where you are or when is it.
 * **Useful Monitoring Settings:** Support setting alarm values, collecting duration, and accessing mobile devices on other PC machines during the monitoring process.
 * **PK Model:** Supports simultaneous comparative testing of two mobile devices.
   - 🌱2-devices: test the same app on two different phones.
   - 🌱2-apps: test two different apps on two phones with the same configuration.
 
-* **Collect in python/API:** Support Python and API to collect performance data, helping users easily integrate into automated testing processes.
+* **Collect In Python/API:** Support Python and API to collect performance data, helping users easily integrate into automated testing processes.
 
 ## Browser
 
 <img src="https://cdn.nlark.com/yuque/0/2023/png/153412/1677553244198-96ce5709-f33f-4038-888f-f330d1f74450.png" alt="Chrome" width="50px" height="50px" />
 
 ## Terminal
```

### Comparing `solox-2.6.3/setup.py` & `solox-2.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/__main__.py` & `solox-2.6.4/solox/__main__.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/debug.py` & `solox-2.6.4/solox/debug.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/_iosPerf.py` & `solox-2.6.4/solox/public/_iosPerf.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/adb/mac/adb` & `solox-2.6.4/solox/public/adb/mac/adb`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/adb.py` & `solox-2.6.4/solox/public/adb.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/apm.py` & `solox-2.6.4/solox/public/apm.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/apm_pk.py` & `solox-2.6.4/solox/public/apm_pk.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/common.py` & `solox-2.6.4/solox/public/common.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/fps.py` & `solox-2.6.4/solox/public/fps.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/__main__.py` & `solox-2.6.4/solox/public/iosperf/__main__.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/_crash.py` & `solox-2.6.4/solox/public/iosperf/_crash.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/_device.py` & `solox-2.6.4/solox/public/iosperf/_device.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/_hexdump.py` & `solox-2.6.4/solox/public/iosperf/_hexdump.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/_imagemounter.py` & `solox-2.6.4/solox/public/iosperf/_imagemounter.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/_installation.py` & `solox-2.6.4/solox/public/iosperf/_installation.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/_instruments.py` & `solox-2.6.4/solox/public/iosperf/_instruments.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/_ipautil.py` & `solox-2.6.4/solox/public/iosperf/_ipautil.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/_perf.py` & `solox-2.6.4/solox/public/iosperf/_perf.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/_proto.py` & `solox-2.6.4/solox/public/iosperf/_proto.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/_relay.py` & `solox-2.6.4/solox/public/iosperf/_relay.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/_safe_socket.py` & `solox-2.6.4/solox/public/iosperf/_safe_socket.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/_ssl.py` & `solox-2.6.4/solox/public/iosperf/_ssl.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/_sync.py` & `solox-2.6.4/solox/public/iosperf/_sync.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/_types.py` & `solox-2.6.4/solox/public/iosperf/_types.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/_usbmux.py` & `solox-2.6.4/solox/public/iosperf/_usbmux.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/_utils.py` & `solox-2.6.4/solox/public/iosperf/_utils.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/_wdaproxy.py` & `solox-2.6.4/solox/public/iosperf/_wdaproxy.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/bplist.py` & `solox-2.6.4/solox/public/iosperf/bplist.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/exceptions.py` & `solox-2.6.4/solox/public/iosperf/exceptions.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/plistlib2.py` & `solox-2.6.4/solox/public/iosperf/plistlib2.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/requests_usbmux.py` & `solox-2.6.4/solox/public/iosperf/requests_usbmux.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/iosperf/struct2.py` & `solox-2.6.4/solox/public/iosperf/struct2.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/report_template/android.html` & `solox-2.6.4/solox/public/report_template/android.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/public/report_template/ios.html` & `solox-2.6.4/solox/public/report_template/ios.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/css/highlight.min.css` & `solox-2.6.4/solox/static/css/highlight.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/css/select2-bootstrap-5-theme.min.css` & `solox-2.6.4/solox/static/css/select2-bootstrap-5-theme.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/css/select2-bootstrap-5-theme.rtl.min.css` & `solox-2.6.4/solox/static/css/select2-bootstrap-5-theme.rtl.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/css/select2.min.css` & `solox-2.6.4/solox/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/css/sweetalert2.min.css` & `solox-2.6.4/solox/static/css/sweetalert2.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/css/tabler.demo.min.css` & `solox-2.6.4/solox/static/css/tabler.demo.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/css/tabler.min.css` & `solox-2.6.4/solox/static/css/tabler.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/image/404.png` & `solox-2.6.4/solox/static/image/404.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/image/500.png` & `solox-2.6.4/solox/static/image/500.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/image/avatar.png` & `solox-2.6.4/solox/static/image/avatar.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/image/coffee.png` & `solox-2.6.4/solox/static/image/coffee.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/image/empty.png` & `solox-2.6.4/solox/static/image/empty.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/image/readme/home.png` & `solox-2.6.4/solox/static/image/readme/home.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/image/readme/pk.png` & `solox-2.6.4/solox/static/image/readme/pk.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/js/apexcharts.js` & `solox-2.6.4/solox/static/js/apexcharts.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/js/gray.js` & `solox-2.6.4/solox/static/js/gray.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/js/highlight.min.js` & `solox-2.6.4/solox/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/js/highstock.js` & `solox-2.6.4/solox/static/js/highstock.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/js/html2canvas.min.js` & `solox-2.6.4/solox/static/js/html2canvas.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/js/jquery.min.js` & `solox-2.6.4/solox/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/js/select2.min.js` & `solox-2.6.4/solox/static/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/js/socket.io.js` & `solox-2.6.4/solox/static/js/socket.io.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/js/sweetalert2.min.js` & `solox-2.6.4/solox/static/js/sweetalert2.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/js/tabler.demo.min.js` & `solox-2.6.4/solox/static/js/tabler.demo.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/js/tabler.min.js` & `solox-2.6.4/solox/static/js/tabler.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/static/logo/logo.png` & `solox-2.6.4/solox/static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/templates/404.html` & `solox-2.6.4/solox/templates/404.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/templates/500.html` & `solox-2.6.4/solox/templates/500.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/templates/analysis.html` & `solox-2.6.4/solox/templates/analysis.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/templates/analysis_compare.html` & `solox-2.6.4/solox/templates/analysis_compare.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/templates/analysis_pk.html` & `solox-2.6.4/solox/templates/analysis_pk.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/templates/base.html` & `solox-2.6.4/solox/templates/base.html`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                     <ul class="list-inline list-inline-dots mb-0">
                         <li class="list-inline-item">
                             Copyright &copy; <label id="curYear"></label>
                             <a href="https://github.com/smart-test-ti" class="link-secondary">SoloX</a>.{% if lan == 'cn' %} 保留所有权利 {% else %} All rights reserved {% endif %}
                         </li>
                         <li class="list-inline-item">
                             <a href="https://github.com/smart-test-ti/SoloX/releases" target="_blank" class="link-secondary" rel="noopener">
-                                {% if lan == 'cn' %} 版本 {% else %} Releases {% endif %} . V2.6.3
+                                {% if lan == 'cn' %} 版本 {% else %} Releases {% endif %} . V2.6.4
                             </a>
                         </li>
                     </ul>
                 </div>
             </div>
         </div>
     </footer>
```

#### html2text {}

```diff
@@ -24,15 +24,15 @@
 ***** {% block page_title %} {% endblock %} *****
 {% block ms_auto %}{% endblock %}
 {% block page_body %}{% endblock %}
     * {%_if_lan_==_'cn'_%}_ææ¡£_{%_else_%}_Documentation_{%_endif_%}
     * {%_if_lan_==_'cn'_%}_æºç _{%_else_%}_Source_code_{%_endif_%}
     * Copyright ©  SoloX.{% if lan == 'cn' %} ä¿çæææå© {% else %} All
       rights reserved {% endif %}
-    * {%_if_lan_==_'cn'_%}_çæ¬_{%_else_%}_Releases_{%_endif_%}_._V2.6.3
+    * {%_if_lan_==_'cn'_%}_çæ¬_{%_else_%}_Releases_{%_endif_%}_._V2.6.4
 *****  {% if lan == 'cn' %} è®¾ç½® {% else %} Setting {% endif %} *****
     * Warning_Value
     * Timer
     * Agent_ _{%_if_lan_==_'en'_%}_?_{%_else_%}_?_{%_endif_%}
 {% if lan == 'cn' %} CPUåè­¦å¼ {% else %} CPU warning value {% endif %} [{
 { cpuWarning }}    ]
 {% if lan == 'cn' %} åå­åè­¦å¼ {% else %} Memory warning value {% endif
```

### Comparing `solox-2.6.3/solox/templates/index.html` & `solox-2.6.4/solox/templates/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1367,26 +1367,30 @@
 
     function stopTask(){
         stop = true;
         var wifi_switch = $('#net-switch').is(':checked');
         $('#run-apm').show();
         $('#stop-apm').hide();
         window.clearTimeout(timerQ);
+        var process = '';
+        if(platform == 'Android'){
+            process = $('.select-pid').val()
+        }
         $.ajax({
             url: "/apm/create/report",
             type: "GET",
             async: true,
             cache: false,
             data:{
                 platform:platform,
                 model:'normal',
                 app:$('.select-app').val(),
                 devices:$('.select-device').val(),
                 wifi_switch:wifi_switch,
-                process:$('.select-pid').val()
+                process:process
             },
             beforeSend: function () {
                 
                 if(lan == 'cn'){
                     SwalLoading('保存数据','正在保存数据生成报告, 请不要离开页面.')
                 }else{
                     SwalLoading('Save data','Saving data to generate report, please do not leave.')
```

### Comparing `solox-2.6.3/solox/templates/pk.html` & `solox-2.6.4/solox/templates/pk.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/templates/report.html` & `solox-2.6.4/solox/templates/report.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/view/apis.py` & `solox-2.6.4/solox/view/apis.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/view/pages.py` & `solox-2.6.4/solox/view/pages.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox/web.py` & `solox-2.6.4/solox/web.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.3/solox.egg-info/PKG-INFO` & `solox-2.6.4/solox.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solox
-Version: 2.6.3
+Version: 2.6.4
 Summary: SoloX - Real-time collection tool for Android/iOS performance data.
 Home-page: https://github.com/smart-test-ti/SoloX
 Author: Rafa Chen
 Author-email: rafacheninc@gamil.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -33,15 +33,15 @@
 
 ## 🔎Preview
 
 SoloX - Real-time collection tool for Android/iOS performance data.
 
 We are committed to solving inefficient, cumbersome test execution, and our goal is Simple Test In SoloX!
 
-<img src="https://cdn.nlark.com/yuque/0/2022/png/153412/1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0"  width="100%" >
+![preview](https://github.com/smart-test-ti/SoloX/assets/24454096/6941452f-6410-4730-a532-0d69d0f7fdb8)
 
 ## 📦Requirements
 
 - Install Python 3.10 + [**Download**](https://www.python.org/downloads/)
 - Install adb and configure environment variables (SoloX's  adb may not necessarily fit your computer) [**Download**](https://developer.android.com/studio/releases/platform-tools)
 
 💡 Python 3.6 ~ 3.9 , please download a version of solox lower than 2.5.4. 
@@ -138,15 +138,15 @@
 * **Data Integrality:** We provide the data about CPU, GPU, Memory, Battery, Network,FPS, Jank, etc., which you may easy to get.
 * **Beautiful Report:** A beautiful and detailed report analysis, where to store, visualize, edit, manage, and download all the test cases collected with SoloX no matter where you are or when is it.
 * **Useful Monitoring Settings:** Support setting alarm values, collecting duration, and accessing mobile devices on other PC machines during the monitoring process.
 * **PK Model:** Supports simultaneous comparative testing of two mobile devices.
   - 🌱2-devices: test the same app on two different phones.
   - 🌱2-apps: test two different apps on two phones with the same configuration.
 
-* **Collect in python/API:** Support Python and API to collect performance data, helping users easily integrate into automated testing processes.
+* **Collect In Python/API:** Support Python and API to collect performance data, helping users easily integrate into automated testing processes.
 
 ## Browser
 
 <img src="https://cdn.nlark.com/yuque/0/2023/png/153412/1677553244198-96ce5709-f33f-4038-888f-f330d1f74450.png" alt="Chrome" width="50px" height="50px" />
 
 ## Terminal
```

### Comparing `solox-2.6.3/solox.egg-info/SOURCES.txt` & `solox-2.6.4/solox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

