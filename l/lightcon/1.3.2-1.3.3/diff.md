# Comparing `tmp/lightcon-1.3.2.tar.gz` & `tmp/lightcon-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightcon-1.3.2.tar", last modified: Wed Dec 28 13:38:43 2022, max compression
+gzip compressed data, was "lightcon-1.3.3.tar", last modified: Mon May 29 15:06:35 2023, max compression
```

## Comparing `lightcon-1.3.2.tar` & `lightcon-1.3.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2022-12-28 13:38:43.243604 lightcon-1.3.2/
--rw-rw-rw-   0        0        0     1082 2022-12-28 13:37:23.000000 lightcon-1.3.2/LICENCE
--rw-rw-rw-   0        0        0     6247 2022-12-28 13:38:43.243604 lightcon-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     5605 2022-12-28 13:37:23.000000 lightcon-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2022-12-28 13:38:43.212358 lightcon-1.3.2/lightcon/
--rw-rw-rw-   0        0        0        0 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/__config__.py
--rw-rw-rw-   0        0        0       21 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/__init__.py
--rw-rw-rw-   0        0        0        0 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/_globals.py
-drwxrwxrwx   0        0        0        0 2022-12-28 13:38:43.212358 lightcon-1.3.2/lightcon/beam_alignment/
--rw-rw-rw-   0        0        0       47 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/beam_alignment/__init__.py
--rw-rw-rw-   0        0        0     2105 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/beam_alignment/beam_alignment.py
-drwxrwxrwx   0        0        0        0 2022-12-28 13:38:43.227979 lightcon-1.3.2/lightcon/calculate/
--rw-rw-rw-   0        0        0      113 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/calculate/__init__.py
--rw-rw-rw-   0        0        0     2997 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/calculate/beam_profiling_gauss.py
--rw-rw-rw-   0        0        0     3393 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/calculate/beam_profiling_iso.py
--rw-rw-rw-   0        0        0     1407 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/calculate/calculate_motor_parameters.py
-drwxrwxrwx   0        0        0        0 2022-12-28 13:38:43.227979 lightcon-1.3.2/lightcon/camera_app_client/
--rw-rw-rw-   0        0        0       40 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/camera_app_client/__init__.py
--rw-rw-rw-   0        0        0     2965 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/camera_app_client/camera_app_client.py
-drwxrwxrwx   0        0        0        0 2022-12-28 13:38:43.227979 lightcon-1.3.2/lightcon/common/
--rw-rw-rw-   0        0        0      324 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/common/__init__.py
--rw-rw-rw-   0        0        0      931 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/common/converters.py
--rw-rw-rw-   0        0        0     3060 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/common/http_methods.py
--rw-rw-rw-   0        0        0     5606 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/common/leprecan_provider.py
--rw-rw-rw-   0        0        0    20146 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/common/motor_parameters.py
--rw-rw-rw-   0        0        0     1042 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/common/serial_tools.py
--rw-rw-rw-   0        0        0      177 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/common/stage_parameters.py
--rw-rw-rw-   0        0        0     5151 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/common/udp_locator.py
-drwxrwxrwx   0        0        0        0 2022-12-28 13:38:43.227979 lightcon-1.3.2/lightcon/eth_motor_board/
--rw-rw-rw-   0        0        0       44 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/eth_motor_board/__init__.py
--rw-rw-rw-   0        0        0    15093 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/eth_motor_board/eth_motor_board.py
--rw-rw-rw-   0        0        0     1918 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/eth_motor_board/eth_motor_board_leprecan_provider.py
-drwxrwxrwx   0        0        0        0 2022-12-28 13:38:43.227979 lightcon-1.3.2/lightcon/fast_daq/
--rw-rw-rw-   0        0        0    70144 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/fast_daq/FTD2XX_NET.dll
--rw-rw-rw-   0        0        0    25088 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/fast_daq/LightConversion.Abstractions.dll
--rw-rw-rw-   0        0        0    23552 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/fast_daq/LightConversion.Hardware.FastDaq.dll
--rw-rw-rw-   0        0        0    29600 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/fast_daq/System.Threading.dll
--rw-rw-rw-   0        0        0       60 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/fast_daq/__init__.py
--rw-rw-rw-   0        0        0     5442 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/fast_daq/fast_daq.py
-drwxrwxrwx   0        0        0        0 2022-12-28 13:38:43.227979 lightcon-1.3.2/lightcon/harpia/
--rw-rw-rw-   0        0        0      138 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/harpia/__init__.py
--rw-rw-rw-   0        0        0    24801 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/harpia/harpia.py
--rw-rw-rw-   0        0        0     2220 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/harpia/harpia_leprecan_provider.py
--rw-rw-rw-   0        0        0     8813 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/harpia/harpia_model_decoder.py
-drwxrwxrwx   0        0        0        0 2022-12-28 13:38:43.243604 lightcon-1.3.2/lightcon/harpia_daq/
--rw-rw-rw-   0        0        0    70144 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/harpia_daq/FTD2XX_NET.dll
--rw-rw-rw-   0        0        0    17920 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/harpia_daq/LightConversion.Abstractions.dll
--rw-rw-rw-   0        0        0    26624 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/harpia_daq/LightConversion.Hardware.HarpiaDaq.dll
--rw-rw-rw-   0        0        0    29600 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/harpia_daq/System.Threading.dll
--rw-rw-rw-   0        0        0       40 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/harpia_daq/__init__.py
--rw-rw-rw-   0        0        0     5744 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/harpia_daq/harpia_daq.py
-drwxrwxrwx   0        0        0        0 2022-12-28 13:38:43.243604 lightcon-1.3.2/lightcon/laser_clients/
--rw-rw-rw-   0        0        0       42 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/laser_clients/__init__.py
--rw-rw-rw-   0        0        0     8633 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/laser_clients/laser_clients.py
-drwxrwxrwx   0        0        0        0 2022-12-28 13:38:43.243604 lightcon-1.3.2/lightcon/style/
--rw-rw-rw-   0        0        0      100 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/style/__init__.py
--rw-rw-rw-   0        0        0    48590 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/style/lclogo.png
--rw-rw-rw-   0        0        0     4585 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/style/lcstyle.mplstyle
--rw-rw-rw-   0        0        0     7839 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/style/plotstyle_1d.py
-drwxrwxrwx   0        0        0        0 2022-12-28 13:38:43.243604 lightcon-1.3.2/lightcon/timing_controller/
--rw-rw-rw-   0        0        0      101 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/timing_controller/__init__.py
--rw-rw-rw-   0        0        0     6325 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/timing_controller/timing_controller.py
--rw-rw-rw-   0        0        0     7233 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/timing_controller/timing_controller_v2.py
-drwxrwxrwx   0        0        0        0 2022-12-28 13:38:43.243604 lightcon-1.3.2/lightcon/wintopas/
--rw-rw-rw-   0        0        0       30 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/wintopas/__init__.py
--rw-rw-rw-   0        0        0     1567 2022-12-28 13:37:23.000000 lightcon-1.3.2/lightcon/wintopas/wintopas.py
-drwxrwxrwx   0        0        0        0 2022-12-28 13:38:43.212358 lightcon-1.3.2/lightcon.egg-info/
--rw-rw-rw-   0        0        0     6247 2022-12-28 13:38:43.000000 lightcon-1.3.2/lightcon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2105 2022-12-28 13:38:43.000000 lightcon-1.3.2/lightcon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-28 13:38:43.000000 lightcon-1.3.2/lightcon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2022-12-28 13:38:43.000000 lightcon-1.3.2/lightcon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-12-28 13:38:43.000000 lightcon-1.3.2/lightcon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-28 13:38:43.243604 lightcon-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0     2524 2022-12-28 13:37:23.000000 lightcon-1.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-28 13:38:43.243604 lightcon-1.3.2/tests/
--rw-rw-rw-   0        0        0        0 2022-12-28 13:37:23.000000 lightcon-1.3.2/tests/__init__.py
--rw-rw-rw-   0        0        0      820 2022-12-28 13:37:23.000000 lightcon-1.3.2/tests/test_leprecan_providers.py
--rw-rw-rw-   0        0        0     1444 2022-12-28 13:37:23.000000 lightcon-1.3.2/tests/test_motor_parameters.py
--rw-rw-rw-   0        0        0      105 2022-12-28 13:37:23.000000 lightcon-1.3.2/tests/test_style.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.938265 lightcon-1.3.3/
+-rw-rw-rw-   0        0        0     1082 2023-05-29 15:04:59.000000 lightcon-1.3.3/LICENCE
+-rw-rw-rw-   0        0        0     6247 2023-05-29 15:06:35.938265 lightcon-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5605 2023-05-29 15:04:59.000000 lightcon-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.343361 lightcon-1.3.3/lightcon/
+-rw-rw-rw-   0        0        0        0 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/__config__.py
+-rw-rw-rw-   0        0        0       21 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/_globals.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.358984 lightcon-1.3.3/lightcon/beam_alignment/
+-rw-rw-rw-   0        0        0       47 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/beam_alignment/__init__.py
+-rw-rw-rw-   0        0        0     2105 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/beam_alignment/beam_alignment.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.358984 lightcon-1.3.3/lightcon/calculate/
+-rw-rw-rw-   0        0        0      113 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/calculate/__init__.py
+-rw-rw-rw-   0        0        0     2997 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/calculate/beam_profiling_gauss.py
+-rw-rw-rw-   0        0        0     3393 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/calculate/beam_profiling_iso.py
+-rw-rw-rw-   0        0        0     1407 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/calculate/calculate_motor_parameters.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.358984 lightcon-1.3.3/lightcon/camera_app_client/
+-rw-rw-rw-   0        0        0       40 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/camera_app_client/__init__.py
+-rw-rw-rw-   0        0        0     2965 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/camera_app_client/camera_app_client.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.358984 lightcon-1.3.3/lightcon/common/
+-rw-rw-rw-   0        0        0      324 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/common/__init__.py
+-rw-rw-rw-   0        0        0      931 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/common/converters.py
+-rw-rw-rw-   0        0        0     3155 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/common/http_methods.py
+-rw-rw-rw-   0        0        0     5606 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/common/leprecan_provider.py
+-rw-rw-rw-   0        0        0    20146 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/common/motor_parameters.py
+-rw-rw-rw-   0        0        0     1042 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/common/serial_tools.py
+-rw-rw-rw-   0        0        0      506 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/common/stage_parameters.py
+-rw-rw-rw-   0        0        0     5151 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/common/udp_locator.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.358984 lightcon-1.3.3/lightcon/eth_motor_board/
+-rw-rw-rw-   0        0        0       44 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/eth_motor_board/__init__.py
+-rw-rw-rw-   0        0        0    15094 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/eth_motor_board/eth_motor_board.py
+-rw-rw-rw-   0        0        0     1918 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/eth_motor_board/eth_motor_board_leprecan_provider.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.358984 lightcon-1.3.3/lightcon/fast_daq/
+-rw-rw-rw-   0        0        0    70144 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/fast_daq/FTD2XX_NET.dll
+-rw-rw-rw-   0        0        0    25088 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/fast_daq/LightConversion.Abstractions.dll
+-rw-rw-rw-   0        0        0    23552 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/fast_daq/LightConversion.Hardware.FastDaq.dll
+-rw-rw-rw-   0        0        0    29600 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/fast_daq/System.Threading.dll
+-rw-rw-rw-   0        0        0       60 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/fast_daq/__init__.py
+-rw-rw-rw-   0        0        0     5442 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/fast_daq/fast_daq.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.374611 lightcon-1.3.3/lightcon/harpia/
+-rw-rw-rw-   0        0        0      138 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/harpia/__init__.py
+-rw-rw-rw-   0        0        0    24801 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/harpia/harpia.py
+-rw-rw-rw-   0        0        0     2220 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/harpia/harpia_leprecan_provider.py
+-rw-rw-rw-   0        0        0     8813 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/harpia/harpia_model_decoder.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.938265 lightcon-1.3.3/lightcon/harpia_daq/
+-rw-rw-rw-   0        0        0    70144 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/harpia_daq/FTD2XX_NET.dll
+-rw-rw-rw-   0        0        0    17920 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/harpia_daq/LightConversion.Abstractions.dll
+-rw-rw-rw-   0        0        0    26624 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/harpia_daq/LightConversion.Hardware.HarpiaDaq.dll
+-rw-rw-rw-   0        0        0    29600 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/harpia_daq/System.Threading.dll
+-rw-rw-rw-   0        0        0       40 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/harpia_daq/__init__.py
+-rw-rw-rw-   0        0        0     5744 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/harpia_daq/harpia_daq.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.938265 lightcon-1.3.3/lightcon/laser_clients/
+-rw-rw-rw-   0        0        0       42 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/laser_clients/__init__.py
+-rw-rw-rw-   0        0        0     8633 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/laser_clients/laser_clients.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.938265 lightcon-1.3.3/lightcon/style/
+-rw-rw-rw-   0        0        0      100 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/style/__init__.py
+-rw-rw-rw-   0        0        0    48590 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/style/lclogo.png
+-rw-rw-rw-   0        0        0     4585 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/style/lcstyle.mplstyle
+-rw-rw-rw-   0        0        0     7839 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/style/plotstyle_1d.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.938265 lightcon-1.3.3/lightcon/timing_controller/
+-rw-rw-rw-   0        0        0      101 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/timing_controller/__init__.py
+-rw-rw-rw-   0        0        0     6325 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/timing_controller/timing_controller.py
+-rw-rw-rw-   0        0        0     7233 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/timing_controller/timing_controller_v2.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.938265 lightcon-1.3.3/lightcon/wintopas/
+-rw-rw-rw-   0        0        0       30 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/wintopas/__init__.py
+-rw-rw-rw-   0        0        0     1567 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/wintopas/wintopas.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.358984 lightcon-1.3.3/lightcon.egg-info/
+-rw-rw-rw-   0        0        0     6247 2023-05-29 15:06:35.000000 lightcon-1.3.3/lightcon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2105 2023-05-29 15:06:35.000000 lightcon-1.3.3/lightcon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 15:06:35.000000 lightcon-1.3.3/lightcon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-05-29 15:06:35.000000 lightcon-1.3.3/lightcon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-29 15:06:35.000000 lightcon-1.3.3/lightcon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 15:06:35.938265 lightcon-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     2524 2023-05-29 15:04:59.000000 lightcon-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.938265 lightcon-1.3.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-29 15:04:59.000000 lightcon-1.3.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      820 2023-05-29 15:04:59.000000 lightcon-1.3.3/tests/test_leprecan_providers.py
+-rw-rw-rw-   0        0        0     1444 2023-05-29 15:04:59.000000 lightcon-1.3.3/tests/test_motor_parameters.py
+-rw-rw-rw-   0        0        0      105 2023-05-29 15:04:59.000000 lightcon-1.3.3/tests/test_style.py
```

### Comparing `lightcon-1.3.2/LICENCE` & `lightcon-1.3.3/LICENCE`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/PKG-INFO` & `lightcon-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightcon
-Version: 1.3.2
+Version: 1.3.3
 Summary: A set of APIs to Light Conversion devices
 Home-page: https://bitbucket.org/harpiasoftware/light-conversion-apis.git
 Author: Vytautas Butkus
 Author-email: vytautas.butkus@lightcon.com
 Project-URL: Examples, https://bitbucket.org/harpiasoftware/light-conversion-apis/src/master/examples/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lightcon-1.3.2/README.md` & `lightcon-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/beam_alignment/beam_alignment.py` & `lightcon-1.3.3/lightcon/beam_alignment/beam_alignment.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/calculate/beam_profiling_gauss.py` & `lightcon-1.3.3/lightcon/calculate/beam_profiling_gauss.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/calculate/beam_profiling_iso.py` & `lightcon-1.3.3/lightcon/calculate/beam_profiling_iso.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/calculate/calculate_motor_parameters.py` & `lightcon-1.3.3/lightcon/calculate/calculate_motor_parameters.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/camera_app_client/camera_app_client.py` & `lightcon-1.3.3/lightcon/camera_app_client/camera_app_client.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/common/converters.py` & `lightcon-1.3.3/lightcon/common/converters.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/common/http_methods.py` & `lightcon-1.3.3/lightcon/common/http_methods.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #==========================================================================
-# 
+#
 #--------------------------------------------------------------------------
 # Copyright (c) 2022 Light Conversion, UAB
 # All rights reserved.
 # www.lightcon.com
 #==========================================================================
 import json
 import urllib
 import urllib.error
 import urllib.request
 import urllib.parse
 import time
 import http
 
-class HTTP_methods:    
+class HTTP_methods:
     retry_on_incomplete_read = True
+    print_full_http_response_on_failure = True
 
     def _open(self, page_url):
         return urllib.request.urlopen(self.url+page_url).read().decode('utf-8')
-        
+
     def _get (self, command):
         time_init = time.perf_counter()
         cont = True
 
         while cont:
             try:
                 data = json.loads(urllib.request.urlopen(self.url+command).read().decode('utf-8'))
@@ -33,50 +34,52 @@
                 error_string = e.read().decode('utf-8', 'ignore')
                 print (error_string)
                 return error_string
             except http.client.IncompleteRead:
                 cont = True and self.retry_on_incomplete_read
                 if not self.silent:
                     print ('Incomplete read')
-        
+
         if not self.silent:
             print (command + " : {:.3f} ms".format((time.perf_counter()-time_init)*1000))
         return data
-        
+
     def _put (self, command, data):
         time_init = time.perf_counter()
         try:
             post_url = urllib.request.Request(url=self.url+command, data=data.encode('utf-8'), method='PUT')
-    
+
             post_url.add_header('Content-Type', 'application/json')
-            
+
             with urllib.request.urlopen(post_url) as f:
                 pass
             if not self.silent:
                 print (command + " : {:.3f} ms".format((time.perf_counter()-time_init)*1000))
-            return f.status            
+            return f.status
         except urllib.error.HTTPError as e:
+            print("Exception while PUT to {:} with data {:}".format(post_url.full_url, data))
             error_string = e.read().decode('utf-8', 'ignore')
-            print (error_string)
+            if self.print_full_http_response_on_failure:
+                print(error_string)
             return error_string
-        
+
         if not self.silent:
             print (command + " : {:.3f} ms".format((time.perf_counter()-time_init)*1000))
         return 200
-    
-        
+
+
     def _post (self, command, details={}):
         time_init = time.perf_counter()
         try:
             post_details = urllib.parse.urlencode(details).encode('UTF-8')
-            
+
             post_url = urllib.request.Request(self.url+command, post_details)
-            
+
             res = urllib.request.urlopen(post_url).read().decode('utf-8', 'ignore')
         except urllib.error.HTTPError as e:
             error_string = e.read().decode('utf-8', 'ignore')
             print (error_string)
             return error_string
-        
+
         if not self.silent:
             print (command + " : {:.3f} ms".format((time.perf_counter()-time_init)*1000))
         return res
```

### Comparing `lightcon-1.3.2/lightcon/common/leprecan_provider.py` & `lightcon-1.3.3/lightcon/common/leprecan_provider.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/common/motor_parameters.py` & `lightcon-1.3.3/lightcon/common/motor_parameters.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/common/serial_tools.py` & `lightcon-1.3.3/lightcon/common/serial_tools.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/common/udp_locator.py` & `lightcon-1.3.3/lightcon/common/udp_locator.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/eth_motor_board/eth_motor_board.py` & `lightcon-1.3.3/lightcon/eth_motor_board/eth_motor_board.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         info_dict = {
             'Acc': 'ACC', 'Dec': 'DEC', 'FnSlpAcc': 'FN_SLP_ACC',
             'FnSlpDec': 'FN_SLP_DEC', 'IntSpeed': 'INT_SPEED',
             'KTherm': 'K_THERM', 'KvalAcc': 'KVAL_ACC', 'KvalDec': 'KVAL_DEC',
             'KvalHold': 'KVAL_HOLD', 'KvalRun': 'KVAL_RUN',
             'MaxSpeed': 'MAX_SPEED', 'MinSpeed': 'MIN_SPEED',
             'OcdTh': 'OCD_TH', 'StSlp': 'ST_SLP', 'StallTh': 'STALL_TH',
-            'StepMode': 'STEP_MODE', 'ls_enble': 'LS_ENABLE',
+            'StepMode': 'STEP_MODE', 'ls_enable': 'LS_ENABLE',
             'ls_invert': 'LS_INVERT', 'ls_swap': 'LS_SWAP'}
 
         motor_name = motor_cfg.get('MotorName', '')
         print("Configuring motor {:} on port {:d}".format(motor_name,
                                                           motor_index))
 
         self.send('HIZ {:} HARD'.format(1 << motor_index))
```

### Comparing `lightcon-1.3.2/lightcon/eth_motor_board/eth_motor_board_leprecan_provider.py` & `lightcon-1.3.3/lightcon/eth_motor_board/eth_motor_board_leprecan_provider.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/fast_daq/FTD2XX_NET.dll` & `lightcon-1.3.3/lightcon/fast_daq/FTD2XX_NET.dll`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/fast_daq/LightConversion.Abstractions.dll` & `lightcon-1.3.3/lightcon/fast_daq/LightConversion.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/fast_daq/LightConversion.Hardware.FastDaq.dll` & `lightcon-1.3.3/lightcon/fast_daq/LightConversion.Hardware.FastDaq.dll`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/fast_daq/System.Threading.dll` & `lightcon-1.3.3/lightcon/fast_daq/System.Threading.dll`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/fast_daq/fast_daq.py` & `lightcon-1.3.3/lightcon/fast_daq/fast_daq.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/harpia/harpia.py` & `lightcon-1.3.3/lightcon/harpia/harpia.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/harpia/harpia_leprecan_provider.py` & `lightcon-1.3.3/lightcon/harpia/harpia_leprecan_provider.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/harpia/harpia_model_decoder.py` & `lightcon-1.3.3/lightcon/harpia/harpia_model_decoder.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/harpia_daq/FTD2XX_NET.dll` & `lightcon-1.3.3/lightcon/harpia_daq/FTD2XX_NET.dll`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/harpia_daq/LightConversion.Abstractions.dll` & `lightcon-1.3.3/lightcon/harpia_daq/LightConversion.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/harpia_daq/LightConversion.Hardware.HarpiaDaq.dll` & `lightcon-1.3.3/lightcon/harpia_daq/LightConversion.Hardware.HarpiaDaq.dll`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/harpia_daq/System.Threading.dll` & `lightcon-1.3.3/lightcon/harpia_daq/System.Threading.dll`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/harpia_daq/harpia_daq.py` & `lightcon-1.3.3/lightcon/harpia_daq/harpia_daq.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/laser_clients/laser_clients.py` & `lightcon-1.3.3/lightcon/laser_clients/laser_clients.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/style/lclogo.png` & `lightcon-1.3.3/lightcon/style/lclogo.png`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/style/lcstyle.mplstyle` & `lightcon-1.3.3/lightcon/style/lcstyle.mplstyle`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/style/plotstyle_1d.py` & `lightcon-1.3.3/lightcon/style/plotstyle_1d.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/timing_controller/timing_controller.py` & `lightcon-1.3.3/lightcon/timing_controller/timing_controller.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/timing_controller/timing_controller_v2.py` & `lightcon-1.3.3/lightcon/timing_controller/timing_controller_v2.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon/wintopas/wintopas.py` & `lightcon-1.3.3/lightcon/wintopas/wintopas.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/lightcon.egg-info/PKG-INFO` & `lightcon-1.3.3/lightcon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightcon
-Version: 1.3.2
+Version: 1.3.3
 Summary: A set of APIs to Light Conversion devices
 Home-page: https://bitbucket.org/harpiasoftware/light-conversion-apis.git
 Author: Vytautas Butkus
 Author-email: vytautas.butkus@lightcon.com
 Project-URL: Examples, https://bitbucket.org/harpiasoftware/light-conversion-apis/src/master/examples/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lightcon-1.3.2/lightcon.egg-info/SOURCES.txt` & `lightcon-1.3.3/lightcon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/setup.py` & `lightcon-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/tests/test_leprecan_providers.py` & `lightcon-1.3.3/tests/test_leprecan_providers.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.2/tests/test_motor_parameters.py` & `lightcon-1.3.3/tests/test_motor_parameters.py`

 * *Files identical despite different names*

