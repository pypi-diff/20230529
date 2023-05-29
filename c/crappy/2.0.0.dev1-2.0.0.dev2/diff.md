# Comparing `tmp/crappy-2.0.0.dev1.tar.gz` & `tmp/crappy-2.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crappy-2.0.0.dev1.tar", last modified: Fri Mar 10 15:34:21 2023, max compression
+gzip compressed data, was "crappy-2.0.0.dev2.tar", last modified: Mon May 29 16:31:50 2023, max compression
```

## Comparing `crappy-2.0.0.dev1.tar` & `crappy-2.0.0.dev2.tar`

### file list

```diff
@@ -1,289 +1,292 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.819821 crappy-2.0.0.dev1/
--rw-rw-r--   0 root         (0) root         (0)    18047 2020-11-20 10:50:04.000000 crappy-2.0.0.dev1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      215 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4875 2023-03-10 15:34:21.819821 crappy-2.0.0.dev1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3445 2022-12-01 14:12:00.000000 crappy-2.0.0.dev1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.803821 crappy-2.0.0.dev1/docs/
--rw-rw-r--   0 root         (0) root         (0)      858 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.803821 crappy-2.0.0.dev1/docs/source/
--rw-rw-r--   0 root         (0) root         (0)      271 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/docs/source/api.rst
--rw-rw-r--   0 root         (0) root         (0)      165 2022-12-01 14:12:00.000000 crappy-2.0.0.dev1/docs/source/bugs.rst
--rw-rw-r--   0 root         (0) root         (0)     1237 2022-12-01 14:12:00.000000 crappy-2.0.0.dev1/docs/source/citing.rst
--rw-rw-r--   0 root         (0) root         (0)     6653 2023-03-10 15:33:50.000000 crappy-2.0.0.dev1/docs/source/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.803821 crappy-2.0.0.dev1/docs/source/crappy_docs/
--rw-rw-r--   0 root         (0) root         (0)     2010 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/docs/source/crappy_docs/actuators.rst
--rw-rw-r--   0 root         (0) root         (0)     5813 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/docs/source/crappy_docs/blocks.rst
--rw-rw-r--   0 root         (0) root         (0)     2644 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/docs/source/crappy_docs/cameras.rst
--rw-rw-r--   0 root         (0) root         (0)     4150 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/docs/source/crappy_docs/inouts.rst
--rw-rw-r--   0 root         (0) root         (0)      150 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/docs/source/crappy_docs/links.rst
--rw-rw-r--   0 root         (0) root         (0)     1458 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/docs/source/crappy_docs/modifiers.rst
--rw-rw-r--   0 root         (0) root         (0)     3812 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/docs/source/crappy_docs/tools.rst
--rw-rw-r--   0 root         (0) root         (0)    11265 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/docs/source/developers.rst
--rw-rw-r--   0 root         (0) root         (0)     5846 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/docs/source/documentation.rst
--rw-rw-r--   0 root         (0) root         (0)    32752 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/docs/source/embedded.rst
--rw-rw-r--   0 root         (0) root         (0)    20010 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/docs/source/features.rst
--rw-rw-r--   0 root         (0) root         (0)      346 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/docs/source/index.rst
--rw-rw-r--   0 root         (0) root         (0)     7250 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/docs/source/installation.rst
--rw-rw-r--   0 root         (0) root         (0)      278 2022-12-01 14:12:00.000000 crappy-2.0.0.dev1/docs/source/license.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.803821 crappy-2.0.0.dev1/docs/source/tutorials/
--rw-rw-r--   0 root         (0) root         (0)    20455 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/docs/source/tutorials/c_modules.rst
--rw-rw-r--   0 root         (0) root         (0)    52003 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/docs/source/tutorials/custom_blocks.rst
--rw-rw-r--   0 root         (0) root         (0)    40231 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/docs/source/tutorials/getting_started.rst
--rw-rw-r--   0 root         (0) root         (0)      137 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/docs/source/tutorials.rst
--rw-rw-r--   0 root         (0) root         (0)     3967 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/docs/source/what_is_crappy.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.799821 crappy-2.0.0.dev1/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.803821 crappy-2.0.0.dev1/examples/other_examples/
--rw-rw-r--   0 root         (0) root         (0)     1133 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/other_examples/daqmx_thermocouple.py
--rw-rw-r--   0 root         (0) root         (0)     1736 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/other_examples/dio_daqmx.py
--rw-rw-r--   0 root         (0) root         (0)     3072 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/other_examples/gpu_correl_advanced.py
--rw-rw-r--   0 root         (0) root         (0)      708 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/other_examples/gpu_correl_basic.py
--rw-rw-r--   0 root         (0) root         (0)     3183 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/other_examples/gpu_correl_fake_test.py
--rw-rw-r--   0 root         (0) root         (0)      765 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/other_examples/labjack_t7_stream.py
--rw-rw-r--   0 root         (0) root         (0)     2841 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/other_examples/labjack_t7_tensile_1.py
--rw-rw-r--   0 root         (0) root         (0)     3719 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/other_examples/labjack_t7_tensile_2.py
--rw-rw-r--   0 root         (0) root         (0)      661 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/other_examples/labjack_t7_thermocouple.py
--rw-rw-r--   0 root         (0) root         (0)      861 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/other_examples/microcontroller_example.py
--rw-rw-r--   0 root         (0) root         (0)     1725 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/other_examples/spectrum.py
--rw-rw-r--   0 root         (0) root         (0)      821 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/other_examples/video_extenso_auto_drive.py
--rw-rw-r--   0 root         (0) root         (0)     2280 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/other_examples/video_extenso_auto_drive_full.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.807821 crappy-2.0.0.dev1/examples/ready_to_run/
--rw-rw-r--   0 root         (0) root         (0)     2336 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/custom_actuator.py
--rw-rw-r--   0 root         (0) root         (0)     2386 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/custom_block.py
--rw-rw-r--   0 root         (0) root         (0)     2054 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/custom_camera.py
--rw-rw-r--   0 root         (0) root         (0)     1691 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/custom_in.py
--rw-rw-r--   0 root         (0) root         (0)     1473 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/custom_out.py
--rw-rw-r--   0 root         (0) root         (0)     2913 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/dic_ve_fake_test.py
--rw-rw-r--   0 root         (0) root         (0)     1452 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/dic_ve_simple.py
--rw-rw-r--   0 root         (0) root         (0)      627 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/dis_correl_basic.py
--rw-rw-r--   0 root         (0) root         (0)     3083 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/dis_correl_fake_test.py
--rw-rw-r--   0 root         (0) root         (0)     4555 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/dis_correl_fake_test_strain_controlled.py
--rw-rw-r--   0 root         (0) root         (0)     1014 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/displayer.py
--rw-rw-r--   0 root         (0) root         (0)     2117 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/drawing.py
--rw-rw-r--   0 root         (0) root         (0)      942 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/fake_test.py
--rw-rw-r--   0 root         (0) root         (0)     2393 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/furnace_simulation.py
--rw-rw-r--   0 root         (0) root         (0)     1631 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/generator.py
--rw-rw-r--   0 root         (0) root         (0)     1666 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/generator_steps.py
--rw-rw-r--   0 root         (0) root         (0)      907 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/mean.py
--rw-rw-r--   0 root         (0) root         (0)     1956 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/modifiers.py
--rw-rw-r--   0 root         (0) root         (0)     1394 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/multiplexer.py
--rw-rw-r--   0 root         (0) root         (0)      511 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/photo.py
--rw-rw-r--   0 root         (0) root         (0)     2283 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/pid.py
--rw-rw-r--   0 root         (0) root         (0)      758 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/read.py
--rw-rw-r--   0 root         (0) root         (0)      909 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/read_write.py
--rw-rw-r--   0 root         (0) root         (0)     2997 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/video_extenso_fake_test.py
--rw-rw-r--   0 root         (0) root         (0)      680 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/ready_to_run/video_extenso_simple.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.807821 crappy-2.0.0.dev1/examples/real_setups_scripts/
--rw-rw-r--   0 root         (0) root         (0)     1219 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/real_setups_scripts/biaxe.py
--rw-rw-r--   0 root         (0) root         (0)     2326 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/real_setups_scripts/biotens.py
--rw-rw-r--   0 root         (0) root         (0)     4403 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/examples/real_setups_scripts/furnace.py
--rw-rw-r--   0 root         (0) root         (0)       94 2023-01-20 15:26:30.000000 crappy-2.0.0.dev1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-10 15:34:21.819821 crappy-2.0.0.dev1/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     5686 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.799821 crappy-2.0.0.dev1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.807821 crappy-2.0.0.dev1/src/crappy/
--rw-rw-r--   0 root         (0) root         (0)     1780 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       44 2023-03-10 15:33:50.000000 crappy-2.0.0.dev1/src/crappy/__version__.py
--rw-rw-r--   0 root         (0) root         (0)     2703 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/_global.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.807821 crappy-2.0.0.dev1/src/crappy/actuator/
--rw-rw-r--   0 root         (0) root         (0)      489 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/actuator/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2316 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/actuator/biaxe.py
--rw-rw-r--   0 root         (0) root         (0)     7901 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/actuator/biotens.py
--rw-rw-r--   0 root         (0) root         (0)     3462 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/actuator/cm_drive.py
--rw-rw-r--   0 root         (0) root         (0)     2664 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/actuator/fake_motor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.807821 crappy-2.0.0.dev1/src/crappy/actuator/ft232h/
--rw-rw-r--   0 root         (0) root         (0)       71 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/actuator/ft232h/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8496 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/actuator/ft232h/motor_kit_pump_ft232h.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.807821 crappy-2.0.0.dev1/src/crappy/actuator/meta_actuator/
--rw-rw-r--   0 root         (0) root         (0)       62 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/actuator/meta_actuator/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3338 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/actuator/meta_actuator/actuator.py
--rw-rw-r--   0 root         (0) root         (0)      766 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/actuator/meta_actuator/meta_actuator.py
--rw-rw-r--   0 root         (0) root         (0)     9135 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/actuator/motor_kit_pump.py
--rw-rw-r--   0 root         (0) root         (0)     5927 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/actuator/oriental.py
--rw-rw-r--   0 root         (0) root         (0)    48301 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/actuator/pololu_tic.py
--rw-rw-r--   0 root         (0) root         (0)     5466 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/actuator/servostar.py
--rw-rw-r--   0 root         (0) root         (0)     4163 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/actuator/tra6ppd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.811821 crappy-2.0.0.dev1/src/crappy/blocks/
--rw-rw-r--   0 root         (0) root         (0)     1018 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5426 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/auto_drive.py
--rw-rw-r--   0 root         (0) root         (0)    15251 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/camera.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.811821 crappy-2.0.0.dev1/src/crappy/blocks/camera_processes/
--rw-rw-r--   0 root         (0) root         (0)      316 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/camera_processes/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7325 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/camera_processes/camera_process.py
--rw-rw-r--   0 root         (0) root         (0)     2927 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/camera_processes/dic_ve.py
--rw-rw-r--   0 root         (0) root         (0)     2462 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/camera_processes/dis_correl.py
--rw-rw-r--   0 root         (0) root         (0)     8318 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/camera_processes/display.py
--rw-rw-r--   0 root         (0) root         (0)     3753 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/camera_processes/gpu_correl.py
--rw-rw-r--   0 root         (0) root         (0)     3652 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/camera_processes/gpu_ve.py
--rw-rw-r--   0 root         (0) root         (0)     5000 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/camera_processes/record.py
--rw-rw-r--   0 root         (0) root         (0)     2980 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/camera_processes/video_extenso.py
--rw-rw-r--   0 root         (0) root         (0)    16741 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/client_server.py
--rw-rw-r--   0 root         (0) root         (0)     4116 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/dashboard.py
--rw-rw-r--   0 root         (0) root         (0)     4846 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/dic_ve.py
--rw-rw-r--   0 root         (0) root         (0)     5039 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/dis_correl.py
--rw-rw-r--   0 root         (0) root         (0)     7834 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/drawing.py
--rw-rw-r--   0 root         (0) root         (0)     5745 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/fake_machine.py
--rw-rw-r--   0 root         (0) root         (0)     8574 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/generator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.811821 crappy-2.0.0.dev1/src/crappy/blocks/generator_path/
--rw-rw-r--   0 root         (0) root         (0)      280 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/generator_path/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2812 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/generator_path/conditional.py
--rw-rw-r--   0 root         (0) root         (0)     1451 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/generator_path/constant.py
--rw-rw-r--   0 root         (0) root         (0)     2036 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/generator_path/custom.py
--rw-rw-r--   0 root         (0) root         (0)     3998 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/generator_path/cyclic.py
--rw-rw-r--   0 root         (0) root         (0)     4542 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/generator_path/cyclic_ramp.py
--rw-rw-r--   0 root         (0) root         (0)     3378 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/generator_path/integrator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.811821 crappy-2.0.0.dev1/src/crappy/blocks/generator_path/meta_path/
--rw-rw-r--   0 root         (0) root         (0)      172 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/generator_path/meta_path/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      557 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/generator_path/meta_path/meta_path.py
--rw-rw-r--   0 root         (0) root         (0)     3983 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/generator_path/meta_path/path.py
--rw-rw-r--   0 root         (0) root         (0)     1894 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/generator_path/ramp.py
--rw-rw-r--   0 root         (0) root         (0)     1842 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/generator_path/sine.py
--rw-rw-r--   0 root         (0) root         (0)     3893 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/gpu_correl.py
--rw-rw-r--   0 root         (0) root         (0)     3455 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/gpu_ve.py
--rw-rw-r--   0 root         (0) root         (0)     8519 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/grapher.py
--rw-rw-r--   0 root         (0) root         (0)     3658 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/gui.py
--rw-rw-r--   0 root         (0) root         (0)     5908 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/hdf_recorder.py
--rw-rw-r--   0 root         (0) root         (0)    11145 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/ioblock.py
--rw-rw-r--   0 root         (0) root         (0)     9773 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/machine.py
--rw-rw-r--   0 root         (0) root         (0)     2857 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/mean.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.811821 crappy-2.0.0.dev1/src/crappy/blocks/meta_block/
--rw-rw-r--   0 root         (0) root         (0)       76 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/meta_block/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    39099 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/meta_block/block.py
--rw-rw-r--   0 root         (0) root         (0)      553 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/meta_block/meta_block.py
--rw-rw-r--   0 root         (0) root         (0)     5373 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/multiplex.py
--rw-rw-r--   0 root         (0) root         (0)     5046 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/pid.py
--rw-rw-r--   0 root         (0) root         (0)     1558 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/reader.py
--rw-rw-r--   0 root         (0) root         (0)     4633 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/recorder.py
--rw-rw-r--   0 root         (0) root         (0)      564 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/sink.py
--rw-rw-r--   0 root         (0) root         (0)    14698 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/ucontroller.py
--rw-rw-r--   0 root         (0) root         (0)     3969 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/blocks/video_extenso.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.811821 crappy-2.0.0.dev1/src/crappy/camera/
--rw-rw-r--   0 root         (0) root         (0)      615 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/camera/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.815821 crappy-2.0.0.dev1/src/crappy/camera/cameralink/
--rw-rw-r--   0 root         (0) root         (0)      112 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/camera/cameralink/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9458 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/camera/cameralink/bispectral.py
--rw-rw-r--   0 root         (0) root         (0)     3970 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/camera/cameralink/cameralink.py
--rw-rw-r--   0 root         (0) root         (0)     3712 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/camera/cameralink/jai.py
--rw-rw-r--   0 root         (0) root         (0)     2096 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/camera/fake_camera.py
--rw-rw-r--   0 root         (0) root         (0)     6021 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/camera/file_reader.py
--rw-rw-r--   0 root         (0) root         (0)    23060 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/camera/gstreamer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.815821 crappy-2.0.0.dev1/src/crappy/camera/meta_camera/
--rw-rw-r--   0 root         (0) root         (0)      109 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/camera/meta_camera/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11944 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/camera/meta_camera/camera.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.815821 crappy-2.0.0.dev1/src/crappy/camera/meta_camera/camera_setting/
--rw-rw-r--   0 root         (0) root         (0)      218 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/camera/meta_camera/camera_setting/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      800 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/camera/meta_camera/camera_setting/camera_bool_setting.py
--rw-rw-r--   0 root         (0) root         (0)     1019 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/camera/meta_camera/camera_setting/camera_choice_setting.py
--rw-rw-r--   0 root         (0) root         (0)     2202 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/camera/meta_camera/camera_setting/camera_scale_setting.py
--rw-rw-r--   0 root         (0) root         (0)     2046 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/camera/meta_camera/camera_setting/camera_setting.py
--rw-rw-r--   0 root         (0) root         (0)      758 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/camera/meta_camera/meta_camera.py
--rw-rw-r--   0 root         (0) root         (0)     7628 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/camera/opencv.py
--rw-rw-r--   0 root         (0) root         (0)     8881 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/camera/pi_camera.py
--rw-rw-r--   0 root         (0) root         (0)    10572 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/camera/seek_thermal_pro.py
--rw-rw-r--   0 root         (0) root         (0)     2156 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/camera/webcam.py
--rw-rw-r--   0 root         (0) root         (0)     4940 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/camera/xiapi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.815821 crappy-2.0.0.dev1/src/crappy/inout/
--rw-rw-r--   0 root         (0) root         (0)     1087 2023-03-10 12:42:27.000000 crappy-2.0.0.dev1/src/crappy/inout/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    12638 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/ads1115.py
--rw-rw-r--   0 root         (0) root         (0)     2968 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/agilent_34420A.py
--rw-rw-r--   0 root         (0) root         (0)    10223 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/comedi.py
--rw-rw-r--   0 root         (0) root         (0)    10922 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/daqmx.py
--rw-rw-r--   0 root         (0) root         (0)     1737 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/fake_inout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.815821 crappy-2.0.0.dev1/src/crappy/inout/ft232h/
--rw-rw-r--   0 root         (0) root         (0)      286 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/ft232h/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9086 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/ft232h/ads1115_ft232h.py
--rw-rw-r--   0 root         (0) root         (0)     2238 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/ft232h/gpio_switch_ft232h.py
--rw-rw-r--   0 root         (0) root         (0)    12724 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/ft232h/mcp9600_ft232h.py
--rw-rw-r--   0 root         (0) root         (0)     4413 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/ft232h/mprls_ft232h.py
--rw-rw-r--   0 root         (0) root         (0)    13603 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/ft232h/nau7802_ft232h.py
--rw-rw-r--   0 root         (0) root         (0)    14127 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/ft232h/waveshare_ad_da_ft232h.py
--rw-rw-r--   0 root         (0) root         (0)     4694 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/gpio_pwm.py
--rw-rw-r--   0 root         (0) root         (0)     3886 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/gpio_switch.py
--rw-rw-r--   0 root         (0) root         (0)     4271 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/gsm.py
--rw-rw-r--   0 root         (0) root         (0)     4545 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/kollmorgen.py
--rw-rw-r--   0 root         (0) root         (0)    16933 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/labjack_t7.py
--rw-rw-r--   0 root         (0) root         (0)    10687 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/labjack_t7_streamer.py
--rw-rw-r--   0 root         (0) root         (0)     5039 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/labjack_ue9.py
--rw-rw-r--   0 root         (0) root         (0)    15589 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/mcp9600.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.815821 crappy-2.0.0.dev1/src/crappy/inout/meta_inout/
--rw-rw-r--   0 root         (0) root         (0)       73 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/meta_inout/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8100 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/meta_inout/inout.py
--rw-rw-r--   0 root         (0) root         (0)      744 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/meta_inout/meta_inout.py
--rw-rw-r--   0 root         (0) root         (0)     7201 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/mprls.py
--rw-rw-r--   0 root         (0) root         (0)    13701 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/nau7802.py
--rwxrwxr-x   0 root         (0) root         (0)    14701 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/ni_daqmx.py
--rw-rw-r--   0 root         (0) root         (0)     1879 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/opsens.py
--rw-rw-r--   0 root         (0) root         (0)     8343 2023-03-10 12:43:01.000000 crappy-2.0.0.dev1/src/crappy/inout/pijuice_hat.py
--rw-rw-r--   0 root         (0) root         (0)     5971 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/spectrum.py
--rw-rw-r--   0 root         (0) root         (0)    13577 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/waveshare_ad_da.py
--rw-rw-r--   0 root         (0) root         (0)    12000 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/inout/waveshare_high_precision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.815821 crappy-2.0.0.dev1/src/crappy/links/
--rw-rw-r--   0 root         (0) root         (0)       46 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/links/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6947 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/links/link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.819821 crappy-2.0.0.dev1/src/crappy/modifier/
--rw-rw-r--   0 root         (0) root         (0)      479 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/modifier/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3229 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/modifier/demux.py
--rw-rw-r--   0 root         (0) root         (0)     1785 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/modifier/differentiate.py
--rw-rw-r--   0 root         (0) root         (0)     1838 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/modifier/integrate.py
--rw-rw-r--   0 root         (0) root         (0)     1749 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/modifier/mean.py
--rw-rw-r--   0 root         (0) root         (0)     1747 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/modifier/median.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.819821 crappy-2.0.0.dev1/src/crappy/modifier/meta_modifier/
--rw-rw-r--   0 root         (0) root         (0)       88 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/modifier/meta_modifier/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      650 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/modifier/meta_modifier/meta_modifier.py
--rw-rw-r--   0 root         (0) root         (0)      925 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/modifier/meta_modifier/modifier.py
--rw-rw-r--   0 root         (0) root         (0)     1525 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/modifier/moving_avg.py
--rw-rw-r--   0 root         (0) root         (0)     1525 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/modifier/moving_med.py
--rw-rw-r--   0 root         (0) root         (0)     2790 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/modifier/offset.py
--rw-rw-r--   0 root         (0) root         (0)     1328 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/modifier/trig_on_change.py
--rw-rw-r--   0 root         (0) root         (0)     1305 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/modifier/trig_on_value.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.819821 crappy-2.0.0.dev1/src/crappy/tool/
--rw-rw-r--   0 root         (0) root         (0)      120 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.819821 crappy-2.0.0.dev1/src/crappy/tool/bindings/
--rw-rw-r--   0 root         (0) root         (0)       16 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/bindings/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3065 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/bindings/comedi_bind.py
--rw-rw-r--   0 root         (0) root         (0)     4588 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/bindings/pyspcm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.819821 crappy-2.0.0.dev1/src/crappy/tool/camera_config/
--rw-rw-r--   0 root         (0) root         (0)      310 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/camera_config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    34136 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/camera_config/camera_config.py
--rw-rw-r--   0 root         (0) root         (0)     2959 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/camera_config/camera_config_boxes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.819821 crappy-2.0.0.dev1/src/crappy/tool/camera_config/config_tools/
--rw-rw-r--   0 root         (0) root         (0)      139 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/camera_config/config_tools/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2097 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/camera_config/config_tools/box.py
--rw-rw-r--   0 root         (0) root         (0)     2814 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/camera_config/config_tools/spots_boxes.py
--rw-rw-r--   0 root         (0) root         (0)     5491 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/camera_config/config_tools/spots_detector.py
--rw-rw-r--   0 root         (0) root         (0)     3076 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/camera_config/config_tools/zoom.py
--rw-rw-r--   0 root         (0) root         (0)     5874 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/camera_config/dic_ve_config.py
--rw-rw-r--   0 root         (0) root         (0)     5521 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/camera_config/dis_correl_config.py
--rw-rw-r--   0 root         (0) root         (0)     6439 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/camera_config/video_extenso_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.819821 crappy-2.0.0.dev1/src/crappy/tool/data/
--rw-rw-r--   0 root         (0) root         (0)     7405 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/data/no_image.png
--rw-rw-r--   0 root         (0) root         (0)    23499 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/data/pad.png
--rw-rw-r--   0 root         (0) root         (0)   190859 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/data/speckle.png
--rw-rw-r--   0 root         (0) root         (0)   128817 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/data/ve_markers.tif
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.819821 crappy-2.0.0.dev1/src/crappy/tool/ft232h/
--rw-rw-r--   0 root         (0) root         (0)      182 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/ft232h/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    69476 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/ft232h/ft232h.py
--rw-rw-r--   0 root         (0) root         (0)    32735 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/ft232h/ft232h_server.py
--rw-rw-r--   0 root         (0) root         (0)     2838 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/ft232h/i2c_message.py
--rw-rw-r--   0 root         (0) root         (0)    15892 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/ft232h/usb_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.819821 crappy-2.0.0.dev1/src/crappy/tool/image_processing/
--rw-rw-r--   0 root         (0) root         (0)      182 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/image_processing/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    14814 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/image_processing/dic_ve.py
--rw-rw-r--   0 root         (0) root         (0)     5951 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/image_processing/dis_correl.py
--rw-rw-r--   0 root         (0) root         (0)     3119 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/image_processing/fields.py
--rw-rw-r--   0 root         (0) root         (0)    32296 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/image_processing/gpu_correl.py
--rw-rw-r--   0 root         (0) root         (0)     4017 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/image_processing/kernels.cu
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.819821 crappy-2.0.0.dev1/src/crappy/tool/image_processing/video_extenso/
--rw-rw-r--   0 root         (0) root         (0)       96 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/image_processing/video_extenso/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8717 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/image_processing/video_extenso/tracker.py
--rw-rw-r--   0 root         (0) root         (0)    11590 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/image_processing/video_extenso/video_extenso.py
--rw-rw-r--   0 root         (0) root         (0)     3929 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/src/crappy/tool/microcontroller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.807821 crappy-2.0.0.dev1/src/crappy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4875 2023-03-10 15:34:21.000000 crappy-2.0.0.dev1/src/crappy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9263 2023-03-10 15:34:21.000000 crappy-2.0.0.dev1/src/crappy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-10 15:34:21.000000 crappy-2.0.0.dev1/src/crappy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-20 15:26:35.000000 crappy-2.0.0.dev1/src/crappy.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      370 2023-03-10 15:34:21.000000 crappy-2.0.0.dev1/src/crappy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-03-10 15:34:21.000000 crappy-2.0.0.dev1/src/crappy.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:34:21.819821 crappy-2.0.0.dev1/util/
--rw-rw-r--   0 root         (0) root         (0)      549 2023-03-08 13:59:00.000000 crappy-2.0.0.dev1/util/set_ft232h_serial_nr.py
--rwxrwxr-x   0 root         (0) root         (0)     2768 2022-12-01 14:12:00.000000 crappy-2.0.0.dev1/util/udev_rule_setter.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.166662 crappy-2.0.0.dev2/
+-rw-rw-r--   0 root         (0) root         (0)    18047 2020-11-20 10:50:04.000000 crappy-2.0.0.dev2/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      215 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5259 2023-05-29 16:31:50.166662 crappy-2.0.0.dev2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3445 2022-12-01 14:12:00.000000 crappy-2.0.0.dev2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.134662 crappy-2.0.0.dev2/docs/
+-rw-rw-r--   0 root         (0) root         (0)      858 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.138661 crappy-2.0.0.dev2/docs/source/
+-rw-rw-r--   0 root         (0) root         (0)      298 2023-03-29 16:07:37.000000 crappy-2.0.0.dev2/docs/source/api.rst
+-rw-rw-r--   0 root         (0) root         (0)      165 2022-12-01 14:12:00.000000 crappy-2.0.0.dev2/docs/source/bugs.rst
+-rw-rw-r--   0 root         (0) root         (0)     1237 2022-12-01 14:12:00.000000 crappy-2.0.0.dev2/docs/source/citing.rst
+-rw-rw-r--   0 root         (0) root         (0)     6679 2023-05-21 15:34:37.000000 crappy-2.0.0.dev2/docs/source/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.138661 crappy-2.0.0.dev2/docs/source/crappy_docs/
+-rw-rw-r--   0 root         (0) root         (0)     2024 2023-04-14 14:57:21.000000 crappy-2.0.0.dev2/docs/source/crappy_docs/actuators.rst
+-rw-rw-r--   0 root         (0) root         (0)     5848 2023-05-21 20:36:40.000000 crappy-2.0.0.dev2/docs/source/crappy_docs/blocks.rst
+-rw-rw-r--   0 root         (0) root         (0)     2781 2023-04-21 17:12:47.000000 crappy-2.0.0.dev2/docs/source/crappy_docs/cameras.rst
+-rw-rw-r--   0 root         (0) root         (0)     4238 2023-05-01 15:06:18.000000 crappy-2.0.0.dev2/docs/source/crappy_docs/inouts.rst
+-rw-rw-r--   0 root         (0) root         (0)      150 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/docs/source/crappy_docs/links.rst
+-rw-rw-r--   0 root         (0) root         (0)     1338 2023-04-16 19:28:12.000000 crappy-2.0.0.dev2/docs/source/crappy_docs/modifiers.rst
+-rw-rw-r--   0 root         (0) root         (0)     5436 2023-05-18 12:10:41.000000 crappy-2.0.0.dev2/docs/source/crappy_docs/tools.rst
+-rw-rw-r--   0 root         (0) root         (0)    11265 2023-03-08 13:59:00.000000 crappy-2.0.0.dev2/docs/source/developers.rst
+-rw-rw-r--   0 root         (0) root         (0)     5846 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/docs/source/documentation.rst
+-rw-rw-r--   0 root         (0) root         (0)    32763 2023-04-18 15:26:27.000000 crappy-2.0.0.dev2/docs/source/embedded.rst
+-rw-rw-r--   0 root         (0) root         (0)    20377 2023-05-01 09:23:05.000000 crappy-2.0.0.dev2/docs/source/features.rst
+-rw-rw-r--   0 root         (0) root         (0)      346 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/docs/source/index.rst
+-rw-rw-r--   0 root         (0) root         (0)     7250 2023-03-08 13:59:00.000000 crappy-2.0.0.dev2/docs/source/installation.rst
+-rw-rw-r--   0 root         (0) root         (0)      278 2022-12-01 14:12:00.000000 crappy-2.0.0.dev2/docs/source/license.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.138661 crappy-2.0.0.dev2/docs/source/tutorials/
+-rw-rw-r--   0 root         (0) root         (0)    20455 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/docs/source/tutorials/c_modules.rst
+-rw-rw-r--   0 root         (0) root         (0)    52003 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/docs/source/tutorials/custom_blocks.rst
+-rw-rw-r--   0 root         (0) root         (0)    40231 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/docs/source/tutorials/getting_started.rst
+-rw-rw-r--   0 root         (0) root         (0)      137 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/docs/source/tutorials.rst
+-rw-rw-r--   0 root         (0) root         (0)     3967 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/docs/source/what_is_crappy.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.134662 crappy-2.0.0.dev2/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.142661 crappy-2.0.0.dev2/examples/other_examples/
+-rw-rw-r--   0 root         (0) root         (0)     1133 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/examples/other_examples/daqmx_thermocouple.py
+-rw-rw-r--   0 root         (0) root         (0)     1736 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/examples/other_examples/dio_daqmx.py
+-rw-rw-r--   0 root         (0) root         (0)     3072 2023-05-29 15:26:58.000000 crappy-2.0.0.dev2/examples/other_examples/gpu_correl_advanced.py
+-rw-rw-r--   0 root         (0) root         (0)      708 2023-05-29 15:26:58.000000 crappy-2.0.0.dev2/examples/other_examples/gpu_correl_basic.py
+-rw-rw-r--   0 root         (0) root         (0)     3183 2023-05-29 15:26:58.000000 crappy-2.0.0.dev2/examples/other_examples/gpu_correl_fake_test.py
+-rw-rw-r--   0 root         (0) root         (0)      765 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/examples/other_examples/labjack_t7_stream.py
+-rw-rw-r--   0 root         (0) root         (0)     2841 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/examples/other_examples/labjack_t7_tensile_1.py
+-rw-rw-r--   0 root         (0) root         (0)     3721 2023-03-13 16:36:34.000000 crappy-2.0.0.dev2/examples/other_examples/labjack_t7_tensile_2.py
+-rw-rw-r--   0 root         (0) root         (0)      661 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/examples/other_examples/labjack_t7_thermocouple.py
+-rw-rw-r--   0 root         (0) root         (0)      861 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/examples/other_examples/microcontroller_example.py
+-rw-rw-r--   0 root         (0) root         (0)     1732 2023-05-01 09:23:05.000000 crappy-2.0.0.dev2/examples/other_examples/spectrum.py
+-rw-rw-r--   0 root         (0) root         (0)      768 2023-03-29 15:40:27.000000 crappy-2.0.0.dev2/examples/other_examples/video_extenso_auto_drive.py
+-rw-rw-r--   0 root         (0) root         (0)     2227 2023-03-29 15:40:27.000000 crappy-2.0.0.dev2/examples/other_examples/video_extenso_auto_drive_full.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.146662 crappy-2.0.0.dev2/examples/ready_to_run/
+-rw-rw-r--   0 root         (0) root         (0)     2331 2023-04-18 07:23:30.000000 crappy-2.0.0.dev2/examples/ready_to_run/custom_actuator.py
+-rw-rw-r--   0 root         (0) root         (0)     2386 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/examples/ready_to_run/custom_block.py
+-rw-rw-r--   0 root         (0) root         (0)     2054 2023-04-18 07:35:44.000000 crappy-2.0.0.dev2/examples/ready_to_run/custom_camera.py
+-rw-rw-r--   0 root         (0) root         (0)     1691 2023-04-18 07:26:14.000000 crappy-2.0.0.dev2/examples/ready_to_run/custom_in.py
+-rw-rw-r--   0 root         (0) root         (0)     1473 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/examples/ready_to_run/custom_out.py
+-rw-rw-r--   0 root         (0) root         (0)     2913 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/examples/ready_to_run/dic_ve_fake_test.py
+-rw-rw-r--   0 root         (0) root         (0)     1452 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/examples/ready_to_run/dic_ve_simple.py
+-rw-rw-r--   0 root         (0) root         (0)      627 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/examples/ready_to_run/dis_correl_basic.py
+-rw-rw-r--   0 root         (0) root         (0)     3083 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/examples/ready_to_run/dis_correl_fake_test.py
+-rw-rw-r--   0 root         (0) root         (0)     4586 2023-03-24 10:20:48.000000 crappy-2.0.0.dev2/examples/ready_to_run/dis_correl_fake_test_strain_controlled.py
+-rw-rw-r--   0 root         (0) root         (0)     1014 2023-04-26 20:38:22.000000 crappy-2.0.0.dev2/examples/ready_to_run/displayer.py
+-rw-rw-r--   0 root         (0) root         (0)      942 2023-05-02 20:02:07.000000 crappy-2.0.0.dev2/examples/ready_to_run/fake_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2395 2023-04-14 15:17:38.000000 crappy-2.0.0.dev2/examples/ready_to_run/furnace_simulation.py
+-rw-rw-r--   0 root         (0) root         (0)     1631 2023-04-18 07:32:39.000000 crappy-2.0.0.dev2/examples/ready_to_run/generator.py
+-rw-rw-r--   0 root         (0) root         (0)     1666 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/examples/ready_to_run/generator_steps.py
+-rw-rw-r--   0 root         (0) root         (0)      907 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/examples/ready_to_run/mean.py
+-rw-rw-r--   0 root         (0) root         (0)     2000 2023-04-14 15:57:41.000000 crappy-2.0.0.dev2/examples/ready_to_run/modifiers.py
+-rw-rw-r--   0 root         (0) root         (0)     1402 2023-04-14 15:17:38.000000 crappy-2.0.0.dev2/examples/ready_to_run/multiplexer.py
+-rw-rw-r--   0 root         (0) root         (0)      511 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/examples/ready_to_run/photo.py
+-rw-rw-r--   0 root         (0) root         (0)     2294 2023-03-24 10:17:56.000000 crappy-2.0.0.dev2/examples/ready_to_run/pid.py
+-rw-rw-r--   0 root         (0) root         (0)      758 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/examples/ready_to_run/read.py
+-rw-rw-r--   0 root         (0) root         (0)      909 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/examples/ready_to_run/read_write.py
+-rw-rw-r--   0 root         (0) root         (0)     2997 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/examples/ready_to_run/video_extenso_fake_test.py
+-rw-rw-r--   0 root         (0) root         (0)      680 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/examples/ready_to_run/video_extenso_simple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.146662 crappy-2.0.0.dev2/examples/real_setups_scripts/
+-rw-rw-r--   0 root         (0) root         (0)     1219 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/examples/real_setups_scripts/biaxe.py
+-rw-rw-r--   0 root         (0) root         (0)     2330 2023-03-29 15:48:51.000000 crappy-2.0.0.dev2/examples/real_setups_scripts/biotens.py
+-rw-rw-r--   0 root         (0) root         (0)     4408 2023-04-14 15:17:38.000000 crappy-2.0.0.dev2/examples/real_setups_scripts/furnace.py
+-rw-rw-r--   0 root         (0) root         (0)       94 2023-01-20 15:26:30.000000 crappy-2.0.0.dev2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 16:31:50.166662 crappy-2.0.0.dev2/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     6240 2023-05-01 15:53:44.000000 crappy-2.0.0.dev2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.134662 crappy-2.0.0.dev2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.146662 crappy-2.0.0.dev2/src/crappy/
+-rw-rw-r--   0 root         (0) root         (0)     2493 2023-04-17 15:59:31.000000 crappy-2.0.0.dev2/src/crappy/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       44 2023-04-14 15:10:01.000000 crappy-2.0.0.dev2/src/crappy/__version__.py
+-rw-rw-r--   0 root         (0) root         (0)     4104 2023-05-15 21:34:04.000000 crappy-2.0.0.dev2/src/crappy/_global.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.146662 crappy-2.0.0.dev2/src/crappy/actuator/
+-rw-rw-r--   0 root         (0) root         (0)      538 2023-04-14 14:55:47.000000 crappy-2.0.0.dev2/src/crappy/actuator/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7531 2023-05-10 20:27:29.000000 crappy-2.0.0.dev2/src/crappy/actuator/adafruit_dc_motor_hat.py
+-rw-rw-r--   0 root         (0) root         (0)     2663 2023-04-14 14:50:28.000000 crappy-2.0.0.dev2/src/crappy/actuator/fake_motor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.150662 crappy-2.0.0.dev2/src/crappy/actuator/ft232h/
+-rw-rw-r--   0 root         (0) root         (0)       69 2023-04-14 14:19:30.000000 crappy-2.0.0.dev2/src/crappy/actuator/ft232h/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6405 2023-05-10 20:27:29.000000 crappy-2.0.0.dev2/src/crappy/actuator/ft232h/adafruit_dc_motor_hat.py
+-rw-rw-r--   0 root         (0) root         (0)     7937 2023-03-29 16:58:21.000000 crappy-2.0.0.dev2/src/crappy/actuator/jvl_mac_140.py
+-rw-rw-r--   0 root         (0) root         (0)     5732 2023-05-10 20:31:47.000000 crappy-2.0.0.dev2/src/crappy/actuator/kollmorgen_servostar_300.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.150662 crappy-2.0.0.dev2/src/crappy/actuator/meta_actuator/
+-rw-rw-r--   0 root         (0) root         (0)       62 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/src/crappy/actuator/meta_actuator/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6731 2023-05-10 21:03:14.000000 crappy-2.0.0.dev2/src/crappy/actuator/meta_actuator/actuator.py
+-rw-rw-r--   0 root         (0) root         (0)      754 2023-05-10 20:31:47.000000 crappy-2.0.0.dev2/src/crappy/actuator/meta_actuator/meta_actuator.py
+-rw-rw-r--   0 root         (0) root         (0)     4202 2023-05-10 20:31:47.000000 crappy-2.0.0.dev2/src/crappy/actuator/newport_tra6ppd.py
+-rw-rw-r--   0 root         (0) root         (0)     5973 2023-05-10 20:31:47.000000 crappy-2.0.0.dev2/src/crappy/actuator/oriental_ard_k.py
+-rw-rw-r--   0 root         (0) root         (0)    48197 2023-03-29 16:58:21.000000 crappy-2.0.0.dev2/src/crappy/actuator/pololu_tic.py
+-rw-rw-r--   0 root         (0) root         (0)     3436 2023-03-29 16:58:21.000000 crappy-2.0.0.dev2/src/crappy/actuator/schneider_mdrive_23.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.150662 crappy-2.0.0.dev2/src/crappy/blocks/
+-rw-rw-r--   0 root         (0) root         (0)     1061 2023-03-13 16:41:26.000000 crappy-2.0.0.dev2/src/crappy/blocks/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5840 2023-05-23 20:27:28.000000 crappy-2.0.0.dev2/src/crappy/blocks/auto_drive_video_extenso.py
+-rw-rw-r--   0 root         (0) root         (0)     4407 2023-05-23 20:27:28.000000 crappy-2.0.0.dev2/src/crappy/blocks/button.py
+-rw-rw-r--   0 root         (0) root         (0)    29340 2023-05-29 13:15:25.000000 crappy-2.0.0.dev2/src/crappy/blocks/camera.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.150662 crappy-2.0.0.dev2/src/crappy/blocks/camera_processes/
+-rw-rw-r--   0 root         (0) root         (0)      316 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/src/crappy/blocks/camera_processes/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    15224 2023-05-24 21:16:16.000000 crappy-2.0.0.dev2/src/crappy/blocks/camera_processes/camera_process.py
+-rw-rw-r--   0 root         (0) root         (0)     8992 2023-05-25 20:13:00.000000 crappy-2.0.0.dev2/src/crappy/blocks/camera_processes/dic_ve.py
+-rw-rw-r--   0 root         (0) root         (0)     7320 2023-05-24 21:32:57.000000 crappy-2.0.0.dev2/src/crappy/blocks/camera_processes/dis_correl.py
+-rw-rw-r--   0 root         (0) root         (0)    12330 2023-05-25 20:16:50.000000 crappy-2.0.0.dev2/src/crappy/blocks/camera_processes/display.py
+-rw-rw-r--   0 root         (0) root         (0)    10303 2023-05-29 15:52:18.000000 crappy-2.0.0.dev2/src/crappy/blocks/camera_processes/gpu_correl.py
+-rw-rw-r--   0 root         (0) root         (0)     8119 2023-05-25 21:07:17.000000 crappy-2.0.0.dev2/src/crappy/blocks/camera_processes/gpu_ve.py
+-rw-rw-r--   0 root         (0) root         (0)     9570 2023-05-28 17:10:36.000000 crappy-2.0.0.dev2/src/crappy/blocks/camera_processes/record.py
+-rw-rw-r--   0 root         (0) root         (0)     5793 2023-05-25 21:25:51.000000 crappy-2.0.0.dev2/src/crappy/blocks/camera_processes/video_extenso.py
+-rw-rw-r--   0 root         (0) root         (0)     8539 2023-05-23 20:27:28.000000 crappy-2.0.0.dev2/src/crappy/blocks/canvas.py
+-rw-rw-r--   0 root         (0) root         (0)    17911 2023-05-23 20:27:28.000000 crappy-2.0.0.dev2/src/crappy/blocks/client_server.py
+-rw-rw-r--   0 root         (0) root         (0)     5093 2023-05-23 20:27:28.000000 crappy-2.0.0.dev2/src/crappy/blocks/dashboard.py
+-rw-rw-r--   0 root         (0) root         (0)    22136 2023-05-29 15:12:15.000000 crappy-2.0.0.dev2/src/crappy/blocks/dic_ve.py
+-rw-rw-r--   0 root         (0) root         (0)    20085 2023-05-29 15:52:18.000000 crappy-2.0.0.dev2/src/crappy/blocks/dis_correl.py
+-rw-rw-r--   0 root         (0) root         (0)     6615 2023-05-23 20:27:28.000000 crappy-2.0.0.dev2/src/crappy/blocks/fake_machine.py
+-rw-rw-r--   0 root         (0) root         (0)     8717 2023-05-23 20:27:28.000000 crappy-2.0.0.dev2/src/crappy/blocks/generator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.154662 crappy-2.0.0.dev2/src/crappy/blocks/generator_path/
+-rw-rw-r--   0 root         (0) root         (0)      280 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/src/crappy/blocks/generator_path/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2917 2023-05-21 15:18:06.000000 crappy-2.0.0.dev2/src/crappy/blocks/generator_path/conditional.py
+-rw-rw-r--   0 root         (0) root         (0)     1520 2023-05-21 15:23:26.000000 crappy-2.0.0.dev2/src/crappy/blocks/generator_path/constant.py
+-rw-rw-r--   0 root         (0) root         (0)     2068 2023-05-21 15:23:26.000000 crappy-2.0.0.dev2/src/crappy/blocks/generator_path/custom.py
+-rw-rw-r--   0 root         (0) root         (0)     4153 2023-05-21 15:25:05.000000 crappy-2.0.0.dev2/src/crappy/blocks/generator_path/cyclic.py
+-rw-rw-r--   0 root         (0) root         (0)     4697 2023-05-21 15:27:36.000000 crappy-2.0.0.dev2/src/crappy/blocks/generator_path/cyclic_ramp.py
+-rw-rw-r--   0 root         (0) root         (0)     3441 2023-05-21 15:42:02.000000 crappy-2.0.0.dev2/src/crappy/blocks/generator_path/integrator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.154662 crappy-2.0.0.dev2/src/crappy/blocks/generator_path/meta_path/
+-rw-rw-r--   0 root         (0) root         (0)      172 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/src/crappy/blocks/generator_path/meta_path/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      750 2023-05-21 14:27:55.000000 crappy-2.0.0.dev2/src/crappy/blocks/generator_path/meta_path/meta_path.py
+-rw-rw-r--   0 root         (0) root         (0)     7356 2023-05-21 15:09:45.000000 crappy-2.0.0.dev2/src/crappy/blocks/generator_path/meta_path/path.py
+-rw-rw-r--   0 root         (0) root         (0)     1958 2023-05-21 15:30:00.000000 crappy-2.0.0.dev2/src/crappy/blocks/generator_path/ramp.py
+-rw-rw-r--   0 root         (0) root         (0)     1904 2023-05-21 15:30:00.000000 crappy-2.0.0.dev2/src/crappy/blocks/generator_path/sine.py
+-rw-rw-r--   0 root         (0) root         (0)    17898 2023-05-29 16:26:09.000000 crappy-2.0.0.dev2/src/crappy/blocks/gpu_correl.py
+-rw-rw-r--   0 root         (0) root         (0)    15405 2023-05-29 16:26:09.000000 crappy-2.0.0.dev2/src/crappy/blocks/gpu_ve.py
+-rw-rw-r--   0 root         (0) root         (0)     9242 2023-05-23 20:27:28.000000 crappy-2.0.0.dev2/src/crappy/blocks/grapher.py
+-rw-rw-r--   0 root         (0) root         (0)     6529 2023-05-23 20:41:08.000000 crappy-2.0.0.dev2/src/crappy/blocks/hdf_recorder.py
+-rw-rw-r--   0 root         (0) root         (0)    14618 2023-05-23 20:42:54.000000 crappy-2.0.0.dev2/src/crappy/blocks/ioblock.py
+-rw-rw-r--   0 root         (0) root         (0)     2536 2023-05-23 20:27:28.000000 crappy-2.0.0.dev2/src/crappy/blocks/link_reader.py
+-rw-rw-r--   0 root         (0) root         (0)    12550 2023-05-23 20:46:23.000000 crappy-2.0.0.dev2/src/crappy/blocks/machine.py
+-rw-rw-r--   0 root         (0) root         (0)     4201 2023-05-23 20:27:28.000000 crappy-2.0.0.dev2/src/crappy/blocks/mean.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.154662 crappy-2.0.0.dev2/src/crappy/blocks/meta_block/
+-rw-rw-r--   0 root         (0) root         (0)       76 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/src/crappy/blocks/meta_block/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    42039 2023-05-23 21:32:31.000000 crappy-2.0.0.dev2/src/crappy/blocks/meta_block/block.py
+-rw-rw-r--   0 root         (0) root         (0)      749 2023-05-21 14:27:55.000000 crappy-2.0.0.dev2/src/crappy/blocks/meta_block/meta_block.py
+-rw-rw-r--   0 root         (0) root         (0)     6642 2023-05-23 20:47:10.000000 crappy-2.0.0.dev2/src/crappy/blocks/multiplexer.py
+-rw-rw-r--   0 root         (0) root         (0)     7931 2023-05-23 20:47:36.000000 crappy-2.0.0.dev2/src/crappy/blocks/pid.py
+-rw-rw-r--   0 root         (0) root         (0)     5628 2023-05-23 20:36:30.000000 crappy-2.0.0.dev2/src/crappy/blocks/recorder.py
+-rw-rw-r--   0 root         (0) root         (0)     1243 2023-05-23 20:27:28.000000 crappy-2.0.0.dev2/src/crappy/blocks/sink.py
+-rw-rw-r--   0 root         (0) root         (0)    15384 2023-05-23 20:37:48.000000 crappy-2.0.0.dev2/src/crappy/blocks/ucontroller.py
+-rw-rw-r--   0 root         (0) root         (0)    18516 2023-05-29 15:12:33.000000 crappy-2.0.0.dev2/src/crappy/blocks/video_extenso.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.154662 crappy-2.0.0.dev2/src/crappy/camera/
+-rw-rw-r--   0 root         (0) root         (0)      602 2023-04-18 20:31:14.000000 crappy-2.0.0.dev2/src/crappy/camera/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.154662 crappy-2.0.0.dev2/src/crappy/camera/cameralink/
+-rw-rw-r--   0 root         (0) root         (0)      147 2023-04-18 20:26:55.000000 crappy-2.0.0.dev2/src/crappy/camera/cameralink/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5208 2023-05-10 21:18:36.000000 crappy-2.0.0.dev2/src/crappy/camera/cameralink/basler_ironman_cameralink.py
+-rw-rw-r--   0 root         (0) root         (0)     5650 2023-05-10 21:18:36.000000 crappy-2.0.0.dev2/src/crappy/camera/cameralink/jai_go_5000c_pmcl.py
+-rw-rw-r--   0 root         (0) root         (0)     2104 2023-04-23 18:43:19.000000 crappy-2.0.0.dev2/src/crappy/camera/fake_camera.py
+-rw-rw-r--   0 root         (0) root         (0)     6067 2023-05-10 21:18:36.000000 crappy-2.0.0.dev2/src/crappy/camera/file_reader.py
+-rw-rw-r--   0 root         (0) root         (0)    24847 2023-05-10 21:18:36.000000 crappy-2.0.0.dev2/src/crappy/camera/gstreamer_camera.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.154662 crappy-2.0.0.dev2/src/crappy/camera/meta_camera/
+-rw-rw-r--   0 root         (0) root         (0)      109 2023-04-18 16:19:15.000000 crappy-2.0.0.dev2/src/crappy/camera/meta_camera/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    21319 2023-05-14 21:14:38.000000 crappy-2.0.0.dev2/src/crappy/camera/meta_camera/camera.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.154662 crappy-2.0.0.dev2/src/crappy/camera/meta_camera/camera_setting/
+-rw-rw-r--   0 root         (0) root         (0)      218 2023-04-18 16:19:15.000000 crappy-2.0.0.dev2/src/crappy/camera/meta_camera/camera_setting/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      891 2023-05-18 11:50:08.000000 crappy-2.0.0.dev2/src/crappy/camera/meta_camera/camera_setting/camera_bool_setting.py
+-rw-rw-r--   0 root         (0) root         (0)     2852 2023-05-18 11:50:08.000000 crappy-2.0.0.dev2/src/crappy/camera/meta_camera/camera_setting/camera_choice_setting.py
+-rw-rw-r--   0 root         (0) root         (0)     3640 2023-05-18 11:50:08.000000 crappy-2.0.0.dev2/src/crappy/camera/meta_camera/camera_setting/camera_scale_setting.py
+-rw-rw-r--   0 root         (0) root         (0)     3338 2023-05-18 11:50:08.000000 crappy-2.0.0.dev2/src/crappy/camera/meta_camera/camera_setting/camera_setting.py
+-rw-rw-r--   0 root         (0) root         (0)      758 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/src/crappy/camera/meta_camera/meta_camera.py
+-rw-rw-r--   0 root         (0) root         (0)     9422 2023-05-10 21:18:36.000000 crappy-2.0.0.dev2/src/crappy/camera/opencv_camera.py
+-rw-rw-r--   0 root         (0) root         (0)     2187 2023-05-10 21:18:36.000000 crappy-2.0.0.dev2/src/crappy/camera/opencv_camera_basic.py
+-rw-rw-r--   0 root         (0) root         (0)     9182 2023-04-23 19:12:22.000000 crappy-2.0.0.dev2/src/crappy/camera/raspberry_pi_camera.py
+-rw-rw-r--   0 root         (0) root         (0)    10656 2023-04-23 19:12:22.000000 crappy-2.0.0.dev2/src/crappy/camera/seek_thermal_pro.py
+-rw-rw-r--   0 root         (0) root         (0)     6793 2023-04-24 20:52:29.000000 crappy-2.0.0.dev2/src/crappy/camera/ximea_xiapi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.158662 crappy-2.0.0.dev2/src/crappy/inout/
+-rw-rw-r--   0 root         (0) root         (0)     1127 2023-05-01 15:04:49.000000 crappy-2.0.0.dev2/src/crappy/inout/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    12251 2023-05-21 16:06:27.000000 crappy-2.0.0.dev2/src/crappy/inout/ads1115.py
+-rw-rw-r--   0 root         (0) root         (0)     2877 2023-05-01 12:34:02.000000 crappy-2.0.0.dev2/src/crappy/inout/agilent_34420A.py
+-rw-rw-r--   0 root         (0) root         (0)    10902 2023-05-21 16:08:36.000000 crappy-2.0.0.dev2/src/crappy/inout/comedi.py
+-rw-rw-r--   0 root         (0) root         (0)    11733 2023-05-21 16:08:36.000000 crappy-2.0.0.dev2/src/crappy/inout/daqmx.py
+-rw-rw-r--   0 root         (0) root         (0)     1822 2023-05-01 14:59:40.000000 crappy-2.0.0.dev2/src/crappy/inout/fake_inout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.158662 crappy-2.0.0.dev2/src/crappy/inout/ft232h/
+-rw-rw-r--   0 root         (0) root         (0)      244 2023-05-15 21:34:04.000000 crappy-2.0.0.dev2/src/crappy/inout/ft232h/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9159 2023-05-21 16:10:08.000000 crappy-2.0.0.dev2/src/crappy/inout/ft232h/ads1115.py
+-rw-rw-r--   0 root         (0) root         (0)     2501 2023-05-08 21:42:39.000000 crappy-2.0.0.dev2/src/crappy/inout/ft232h/gpio_switch.py
+-rw-rw-r--   0 root         (0) root         (0)    13110 2023-05-08 21:39:39.000000 crappy-2.0.0.dev2/src/crappy/inout/ft232h/mcp9600.py
+-rw-rw-r--   0 root         (0) root         (0)     4425 2023-05-08 21:42:39.000000 crappy-2.0.0.dev2/src/crappy/inout/ft232h/mprls.py
+-rw-rw-r--   0 root         (0) root         (0)    13765 2023-05-21 16:10:08.000000 crappy-2.0.0.dev2/src/crappy/inout/ft232h/nau7802.py
+-rw-rw-r--   0 root         (0) root         (0)    14011 2023-05-21 16:10:08.000000 crappy-2.0.0.dev2/src/crappy/inout/ft232h/waveshare_ad_da.py
+-rw-rw-r--   0 root         (0) root         (0)     4688 2023-05-01 12:12:01.000000 crappy-2.0.0.dev2/src/crappy/inout/gpio_pwm.py
+-rw-rw-r--   0 root         (0) root         (0)     3579 2023-05-01 12:34:02.000000 crappy-2.0.0.dev2/src/crappy/inout/gpio_switch.py
+-rw-rw-r--   0 root         (0) root         (0)     4552 2023-05-15 21:34:04.000000 crappy-2.0.0.dev2/src/crappy/inout/kollmorgen_akd_pdmm.py
+-rw-rw-r--   0 root         (0) root         (0)    17103 2023-05-21 16:06:41.000000 crappy-2.0.0.dev2/src/crappy/inout/labjack_t7.py
+-rw-rw-r--   0 root         (0) root         (0)    10853 2023-05-21 16:08:36.000000 crappy-2.0.0.dev2/src/crappy/inout/labjack_t7_streamer.py
+-rw-rw-r--   0 root         (0) root         (0)     5652 2023-05-21 16:08:36.000000 crappy-2.0.0.dev2/src/crappy/inout/labjack_ue9.py
+-rw-rw-r--   0 root         (0) root         (0)    15487 2023-05-01 13:04:45.000000 crappy-2.0.0.dev2/src/crappy/inout/mcp9600.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.158662 crappy-2.0.0.dev2/src/crappy/inout/meta_inout/
+-rw-rw-r--   0 root         (0) root         (0)       73 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/src/crappy/inout/meta_inout/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    14291 2023-05-10 21:46:28.000000 crappy-2.0.0.dev2/src/crappy/inout/meta_inout/inout.py
+-rw-rw-r--   0 root         (0) root         (0)      744 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/src/crappy/inout/meta_inout/meta_inout.py
+-rw-rw-r--   0 root         (0) root         (0)     6901 2023-05-01 13:32:55.000000 crappy-2.0.0.dev2/src/crappy/inout/mprls.py
+-rw-rw-r--   0 root         (0) root         (0)    13802 2023-05-21 16:08:36.000000 crappy-2.0.0.dev2/src/crappy/inout/nau7802.py
+-rwxrwxr-x   0 root         (0) root         (0)    14837 2023-05-15 21:34:04.000000 crappy-2.0.0.dev2/src/crappy/inout/ni_daqmx.py
+-rw-rw-r--   0 root         (0) root         (0)     1899 2023-05-01 14:19:45.000000 crappy-2.0.0.dev2/src/crappy/inout/opsens_handysens.py
+-rw-rw-r--   0 root         (0) root         (0)     8303 2023-05-01 15:18:24.000000 crappy-2.0.0.dev2/src/crappy/inout/pijuice_hat.py
+-rw-rw-r--   0 root         (0) root         (0)     4377 2023-05-15 21:34:04.000000 crappy-2.0.0.dev2/src/crappy/inout/sim868.py
+-rw-rw-r--   0 root         (0) root         (0)     6134 2023-05-15 21:34:04.000000 crappy-2.0.0.dev2/src/crappy/inout/spectrum_m2i4711.py
+-rw-rw-r--   0 root         (0) root         (0)    13452 2023-05-21 16:08:36.000000 crappy-2.0.0.dev2/src/crappy/inout/waveshare_ad_da.py
+-rw-rw-r--   0 root         (0) root         (0)    12079 2023-05-21 16:08:36.000000 crappy-2.0.0.dev2/src/crappy/inout/waveshare_high_precision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.158662 crappy-2.0.0.dev2/src/crappy/lamcube/
+-rw-rw-r--   0 root         (0) root         (0)      383 2023-04-18 20:26:55.000000 crappy-2.0.0.dev2/src/crappy/lamcube/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2608 2023-05-15 20:18:31.000000 crappy-2.0.0.dev2/src/crappy/lamcube/biaxe.py
+-rw-rw-r--   0 root         (0) root         (0)      339 2023-05-15 20:18:31.000000 crappy-2.0.0.dev2/src/crappy/lamcube/biotens.py
+-rw-rw-r--   0 root         (0) root         (0)    10664 2023-05-15 20:18:31.000000 crappy-2.0.0.dev2/src/crappy/lamcube/bispectral.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.158662 crappy-2.0.0.dev2/src/crappy/links/
+-rw-rw-r--   0 root         (0) root         (0)       46 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/src/crappy/links/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7714 2023-05-15 21:34:04.000000 crappy-2.0.0.dev2/src/crappy/links/link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.158662 crappy-2.0.0.dev2/src/crappy/modifier/
+-rw-rw-r--   0 root         (0) root         (0)      479 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/src/crappy/modifier/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3758 2023-05-16 22:01:39.000000 crappy-2.0.0.dev2/src/crappy/modifier/demux.py
+-rw-rw-r--   0 root         (0) root         (0)     1797 2023-05-16 21:46:21.000000 crappy-2.0.0.dev2/src/crappy/modifier/differentiate.py
+-rw-rw-r--   0 root         (0) root         (0)     1865 2023-05-16 21:46:21.000000 crappy-2.0.0.dev2/src/crappy/modifier/integrate.py
+-rw-rw-r--   0 root         (0) root         (0)     1763 2023-05-16 21:46:21.000000 crappy-2.0.0.dev2/src/crappy/modifier/mean.py
+-rw-rw-r--   0 root         (0) root         (0)     1762 2023-05-16 21:46:21.000000 crappy-2.0.0.dev2/src/crappy/modifier/median.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.162662 crappy-2.0.0.dev2/src/crappy/modifier/meta_modifier/
+-rw-rw-r--   0 root         (0) root         (0)       88 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/src/crappy/modifier/meta_modifier/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      650 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/src/crappy/modifier/meta_modifier/meta_modifier.py
+-rw-rw-r--   0 root         (0) root         (0)     2373 2023-05-16 21:20:12.000000 crappy-2.0.0.dev2/src/crappy/modifier/meta_modifier/modifier.py
+-rw-rw-r--   0 root         (0) root         (0)     1540 2023-05-16 21:46:21.000000 crappy-2.0.0.dev2/src/crappy/modifier/moving_avg.py
+-rw-rw-r--   0 root         (0) root         (0)     1540 2023-05-16 21:46:21.000000 crappy-2.0.0.dev2/src/crappy/modifier/moving_med.py
+-rw-rw-r--   0 root         (0) root         (0)     2756 2023-05-16 22:04:20.000000 crappy-2.0.0.dev2/src/crappy/modifier/offset.py
+-rw-rw-r--   0 root         (0) root         (0)     1331 2023-05-16 21:46:21.000000 crappy-2.0.0.dev2/src/crappy/modifier/trig_on_change.py
+-rw-rw-r--   0 root         (0) root         (0)     1417 2023-05-16 22:01:40.000000 crappy-2.0.0.dev2/src/crappy/modifier/trig_on_value.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.162662 crappy-2.0.0.dev2/src/crappy/tool/
+-rw-rw-r--   0 root         (0) root         (0)      120 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/src/crappy/tool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.162662 crappy-2.0.0.dev2/src/crappy/tool/bindings/
+-rw-rw-r--   0 root         (0) root         (0)       16 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/src/crappy/tool/bindings/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3125 2023-05-17 21:04:16.000000 crappy-2.0.0.dev2/src/crappy/tool/bindings/comedi_bind.py
+-rw-rw-r--   0 root         (0) root         (0)     4657 2023-05-17 21:04:16.000000 crappy-2.0.0.dev2/src/crappy/tool/bindings/pyspcm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.162662 crappy-2.0.0.dev2/src/crappy/tool/camera_config/
+-rw-rw-r--   0 root         (0) root         (0)      310 2023-04-17 11:54:51.000000 crappy-2.0.0.dev2/src/crappy/tool/camera_config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    36905 2023-05-18 11:48:47.000000 crappy-2.0.0.dev2/src/crappy/tool/camera_config/camera_config.py
+-rw-rw-r--   0 root         (0) root         (0)     3817 2023-05-18 11:36:02.000000 crappy-2.0.0.dev2/src/crappy/tool/camera_config/camera_config_boxes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.162662 crappy-2.0.0.dev2/src/crappy/tool/camera_config/config_tools/
+-rw-rw-r--   0 root         (0) root         (0)      187 2023-04-17 11:54:51.000000 crappy-2.0.0.dev2/src/crappy/tool/camera_config/config_tools/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1934 2023-05-17 21:33:07.000000 crappy-2.0.0.dev2/src/crappy/tool/camera_config/config_tools/box.py
+-rw-rw-r--   0 root         (0) root         (0)     5779 2023-05-17 21:42:45.000000 crappy-2.0.0.dev2/src/crappy/tool/camera_config/config_tools/histogram_process.py
+-rw-rw-r--   0 root         (0) root         (0)     3187 2023-05-17 21:46:09.000000 crappy-2.0.0.dev2/src/crappy/tool/camera_config/config_tools/spots_boxes.py
+-rw-rw-r--   0 root         (0) root         (0)     8551 2023-05-17 21:53:43.000000 crappy-2.0.0.dev2/src/crappy/tool/camera_config/config_tools/spots_detector.py
+-rw-rw-r--   0 root         (0) root         (0)     3111 2023-05-17 21:54:30.000000 crappy-2.0.0.dev2/src/crappy/tool/camera_config/config_tools/zoom.py
+-rw-rw-r--   0 root         (0) root         (0)     7035 2023-05-18 11:32:36.000000 crappy-2.0.0.dev2/src/crappy/tool/camera_config/dic_ve_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6406 2023-05-18 12:40:45.000000 crappy-2.0.0.dev2/src/crappy/tool/camera_config/dis_correl_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7344 2023-05-18 11:26:26.000000 crappy-2.0.0.dev2/src/crappy/tool/camera_config/video_extenso_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.162662 crappy-2.0.0.dev2/src/crappy/tool/data/
+-rw-rw-r--   0 root         (0) root         (0)     7405 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/src/crappy/tool/data/no_image.png
+-rw-rw-r--   0 root         (0) root         (0)    23499 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/src/crappy/tool/data/pad.png
+-rw-rw-r--   0 root         (0) root         (0)   190859 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/src/crappy/tool/data/speckle.png
+-rw-rw-r--   0 root         (0) root         (0)   128817 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/src/crappy/tool/data/ve_markers.tif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.162662 crappy-2.0.0.dev2/src/crappy/tool/ft232h/
+-rw-rw-r--   0 root         (0) root         (0)      182 2023-04-17 12:39:00.000000 crappy-2.0.0.dev2/src/crappy/tool/ft232h/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    69663 2023-05-18 12:22:15.000000 crappy-2.0.0.dev2/src/crappy/tool/ft232h/ft232h.py
+-rw-rw-r--   0 root         (0) root         (0)    34130 2023-05-17 21:29:34.000000 crappy-2.0.0.dev2/src/crappy/tool/ft232h/ft232h_server.py
+-rw-rw-r--   0 root         (0) root         (0)     2926 2023-05-17 21:22:56.000000 crappy-2.0.0.dev2/src/crappy/tool/ft232h/i2c_message.py
+-rw-rw-r--   0 root         (0) root         (0)    19200 2023-05-17 21:18:26.000000 crappy-2.0.0.dev2/src/crappy/tool/ft232h/usb_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.166662 crappy-2.0.0.dev2/src/crappy/tool/image_processing/
+-rw-rw-r--   0 root         (0) root         (0)      182 2023-04-17 12:39:00.000000 crappy-2.0.0.dev2/src/crappy/tool/image_processing/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    15122 2023-05-18 12:39:33.000000 crappy-2.0.0.dev2/src/crappy/tool/image_processing/dic_ve.py
+-rw-rw-r--   0 root         (0) root         (0)     6303 2023-05-18 12:37:58.000000 crappy-2.0.0.dev2/src/crappy/tool/image_processing/dis_correl.py
+-rw-rw-r--   0 root         (0) root         (0)     3393 2023-05-18 12:31:29.000000 crappy-2.0.0.dev2/src/crappy/tool/image_processing/fields.py
+-rw-rw-r--   0 root         (0) root         (0)    32790 2023-05-29 15:52:18.000000 crappy-2.0.0.dev2/src/crappy/tool/image_processing/gpu_correl.py
+-rw-rw-r--   0 root         (0) root         (0)     4017 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/src/crappy/tool/image_processing/kernels.cu
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.166662 crappy-2.0.0.dev2/src/crappy/tool/image_processing/video_extenso/
+-rw-rw-r--   0 root         (0) root         (0)       96 2023-05-18 12:05:12.000000 crappy-2.0.0.dev2/src/crappy/tool/image_processing/video_extenso/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10045 2023-05-18 11:56:32.000000 crappy-2.0.0.dev2/src/crappy/tool/image_processing/video_extenso/tracker.py
+-rw-rw-r--   0 root         (0) root         (0)    12814 2023-05-18 12:07:27.000000 crappy-2.0.0.dev2/src/crappy/tool/image_processing/video_extenso/video_extenso.py
+-rw-rw-r--   0 root         (0) root         (0)     3929 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/src/crappy/tool/microcontroller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.146662 crappy-2.0.0.dev2/src/crappy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5259 2023-05-29 16:31:50.000000 crappy-2.0.0.dev2/src/crappy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9478 2023-05-29 16:31:50.000000 crappy-2.0.0.dev2/src/crappy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 16:31:50.000000 crappy-2.0.0.dev2/src/crappy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-20 15:26:35.000000 crappy-2.0.0.dev2/src/crappy.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      384 2023-05-29 16:31:50.000000 crappy-2.0.0.dev2/src/crappy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-29 16:31:50.000000 crappy-2.0.0.dev2/src/crappy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:31:50.166662 crappy-2.0.0.dev2/util/
+-rw-rw-r--   0 root         (0) root         (0)      549 2023-03-10 21:52:22.000000 crappy-2.0.0.dev2/util/set_ft232h_serial_nr.py
+-rwxrwxr-x   0 root         (0) root         (0)     2768 2022-12-01 14:12:00.000000 crappy-2.0.0.dev2/util/udev_rule_setter.sh
```

### Comparing `crappy-2.0.0.dev1/LICENSE` & `crappy-2.0.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/PKG-INFO` & `crappy-2.0.0.dev2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 Metadata-Version: 2.1
 Name: crappy
-Version: 2.0.0.dev1
-Summary: Command and Real-time Acquisition Parallelized in Python
+Version: 2.0.0.dev2
+Summary: Command and Real-time Acquisition in Parallelized Python
 Home-page: https://github.com/LaboratoireMecaniqueLille/crappy
+Download-URL: https://pypi.org/project/crappy/#files
 Author: LaMcube
 Author-email: antoine.weisrock1@centralelille.fr
+Maintainer: Antoine Weisrock
+Maintainer-email: antoine.weisrock@gmail.com
 License: GPL V2
 Project-URL: Documentation, https://crappy.readthedocs.io/en/latest/index.html
-Keywords: control command acquisition multiprocessing
+Keywords: control,command,acquisition,multiprocessing
 Classifier: Development Status :: 4 - Beta 
 Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Embedded Systems
+Requires-Python: >=3.7
 Provides-Extra: SBC
 Provides-Extra: image
 Provides-Extra: hardware
 Provides-Extra: main
 License-File: LICENSE
 
 =================
```

### Comparing `crappy-2.0.0.dev1/README.md` & `crappy-2.0.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/docs/Makefile` & `crappy-2.0.0.dev2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/docs/source/citing.rst` & `crappy-2.0.0.dev2/docs/source/citing.rst`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/docs/source/conf.py` & `crappy-2.0.0.dev2/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
 from time import asctime
-__version__ = '2.0.0.dev1'
+__version__ = '2.0.0.dev2'
 
 sys.path.insert(0, os.path.abspath('../..'))
 sys.setrecursionlimit(1500)
 
 # -- Project information -----------------------------------------------------
 
 project = 'Crappy'
@@ -50,15 +50,16 @@
     'sphinx.ext.autodoc',
     'sphinx.ext.intersphinx',
     'sphinx.ext.ifconfig',
     'sphinx.ext.viewcode',
     'sphinx.ext.githubpages',
     'sphinx.ext.autosectionlabel',
     'sphinx_rtd_theme',
-    'sphinx.ext.napoleon'
+    'sphinx.ext.napoleon',
+    'sphinx.ext.mathjax'
 ]
 
 # Napoleon settings
 napoleon_google_docstring = True
 napoleon_numpy_docstring = True
 napoleon_include_init_with_doc = True
 napoleon_include_private_with_doc = False
```

### Comparing `crappy-2.0.0.dev1/docs/source/crappy_docs/actuators.rst` & `crappy-2.0.0.dev2/docs/source/crappy_docs/actuators.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,71 @@
 =========
 Actuators
 =========
 
 Regular Actuators
 -----------------
 
-Biaxe
-+++++
-.. autoclass:: crappy.actuator.Biaxe
+Adafruit DC Motor Hat
++++++++++++++++++++++
+.. autoclass:: crappy.actuator.DCMotorHat
    :members: open, set_speed, stop, close
    :special-members: __init__
 
-Biotens
-+++++++
-.. autoclass:: crappy.actuator.Biotens
+Fake Motor
+++++++++++
+.. autoclass:: crappy.actuator.FakeMotor
+   :members: open, get_speed, get_position, set_speed, stop, close
+   :special-members: __init__
+
+JVL Mac140
+++++++++++
+.. autoclass:: crappy.actuator.JVLMac140
    :members: open, get_position, set_speed, set_position, reset_position,
              stop, close
    :special-members: __init__
 
-CM Drive
-++++++++
-.. autoclass:: crappy.actuator.CMDrive
-   :members: open, get_position, set_speed, set_position, stop, close
+Kollmorgen ServoStar 300
+++++++++++++++++++++++++
+.. autoclass:: crappy.actuator.ServoStar300
+   :members: open, get_position, set_position, stop, close
    :special-members: __init__
 
-Fake Motor
-++++++++++
-.. autoclass:: crappy.actuator.FakeMotor
-   :members: open, get_speed, get_position, set_speed, stop, close
+Newport TRA6PPD
++++++++++++++++
+.. autoclass:: crappy.actuator.NewportTRA6PPD
+   :members: open, get_position, set_position, stop, close
    :special-members: __init__
 
-Motor kit pump
+Oriental ARD-K
 ++++++++++++++
-.. autoclass:: crappy.actuator.MotorKitPump
-   :members: open, set_speed, stop, close
-   :special-members: __init__
-
-Oriental
-++++++++
-.. autoclass:: crappy.actuator.Oriental
+.. autoclass:: crappy.actuator.OrientalARDK
    :members: open, get_position, set_speed, set_position, stop, close
    :special-members: __init__
 
 Pololu Tic
 ++++++++++
 .. autoclass:: crappy.actuator.PololuTic
    :members: open, get_speed, get_position, set_speed, set_position, stop,
              close
    :special-members: __init__
 
-ServoStar
-+++++++++
-.. autoclass:: crappy.actuator.ServoStar
-   :members: open, get_position, set_position, stop, close
-   :special-members: __init__
-
-TRA6PPD
-+++++++
-.. autoclass:: crappy.actuator.TRA6PPD
-   :members: open, get_position, set_position, stop, close
+Schneider MDrive 23
++++++++++++++++++++
+.. autoclass:: crappy.actuator.SchneiderMDrive23
+   :members: open, get_position, set_speed, set_position, stop, close
    :special-members: __init__
 
 FT232H Actuators
 ----------------
 
-Motor kit pump FT232H
-+++++++++++++++++++++
+Adafruit DC Motor Hat FT232H
+++++++++++++++++++++++++++++
 
-.. autoclass:: crappy.actuator.MotorKitPumpFT232H
+.. autoclass:: crappy.actuator.DCMotorHatFT232H
    :members: open, set_speed, stop, close
    :special-members: __init__
 
 Parent Actuator
 ---------------
 
 Actuator
```

### Comparing `crappy-2.0.0.dev1/docs/source/crappy_docs/blocks.rst` & `crappy-2.0.0.dev2/docs/source/crappy_docs/blocks.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,36 @@
 ======
 
 Regular Blocks
 --------------
 
 Auto Drive
 ++++++++++
-.. autoclass:: crappy.blocks.AutoDrive
+.. autoclass:: crappy.blocks.AutoDriveVideoExtenso
    :members: __init__, prepare, loop, finish
    :special-members: __init__
 
+Button
+++++++
+.. autoclass:: crappy.blocks.Button
+   :members: prepare, begin, loop, finish
+   :special-members: __init__
+
 Camera Block
 ++++++++++++
 .. autoclass:: crappy.blocks.Camera
    :members: prepare, begin, loop, finish
    :special-members: __init__
 
+Canvas
++++++++
+.. autoclass:: crappy.blocks.Canvas
+   :members: prepare, loop, finish
+   :special-members: __init__
+
 Client Server
 +++++++++++++
 .. autoclass:: crappy.blocks.ClientServer
    :members: prepare, loop, finish
    :special-members: __init__
 
 Dashboard
@@ -31,26 +43,20 @@
 
 DIS Correl
 ++++++++++
 .. autoclass:: crappy.blocks.DISCorrel
    :members: prepare
    :special-members: __init__
 
-DIS VE
+DIC VE
 ++++++
 .. autoclass:: crappy.blocks.DICVE
    :members: prepare
    :special-members: __init__
 
-Drawing
-+++++++
-.. autoclass:: crappy.blocks.Drawing
-   :members: prepare, loop, finish
-   :special-members: __init__
-
 Fake Machine
 ++++++++++++
 .. autoclass:: crappy.blocks.FakeMachine
    :members: prepare, begin, loop
    :special-members: __init__
 
 Generator
@@ -73,62 +79,56 @@
 
 Grapher
 +++++++
 .. autoclass:: crappy.blocks.Grapher
    :members: prepare, loop, finish
    :special-members: __init__
 
-GUI
-+++
-.. autoclass:: crappy.blocks.GUI
-   :members: prepare, begin, loop, finish
-   :special-members: __init__
-
 HDF Recorder
 ++++++++++++
 .. autoclass:: crappy.blocks.HDFRecorder
    :members: prepare, loop, finish
    :special-members: __init__
 
 IOBlock
 +++++++
 .. autoclass:: crappy.blocks.IOBlock
    :members: prepare, loop, finish
    :special-members: __init__
 
+Link Reader
++++++++++++
+.. autoclass:: crappy.blocks.LinkReader
+   :members: loop
+   :special-members: __init__
+
 Machine
 +++++++
 .. autoclass:: crappy.blocks.Machine
    :members: prepare, loop, finish
    :special-members: __init__
 
 Mean Block
 ++++++++++
 .. autoclass:: crappy.blocks.MeanBlock
    :members: prepare, begin, loop
    :special-members: __init__
 
 Multiplexer
 +++++++++++
-.. autoclass:: crappy.blocks.Multiplex
+.. autoclass:: crappy.blocks.Multiplexer
    :members: loop
    :special-members: __init__
 
 PID
 +++
 .. autoclass:: crappy.blocks.PID
    :members: loop
    :special-members: __init__
 
-Reader
-++++++
-.. autoclass:: crappy.blocks.Reader
-   :members: loop
-   :special-members: __init__
-
 Recorder
 ++++++++
 .. autoclass:: crappy.blocks.Recorder
    :members: prepare, loop
    :special-members: __init__
 
 Sink
@@ -149,14 +149,20 @@
    :members: prepare
    :special-members: __init__
 
 Generator Paths
 ---------------
 There are several types of path available for the generator block.
 
+Conditional
++++++++++++
+.. autoclass:: crappy.blocks.generator_path.Conditional
+   :members: get_cmd
+   :special-members: __init__
+
 Constant
 ++++++++
 .. autoclass:: crappy.blocks.generator_path.Constant
    :members: get_cmd
    :special-members: __init__
 
 Custom
@@ -179,20 +185,14 @@
 
 Integrator
 ++++++++++
 .. autoclass:: crappy.blocks.generator_path.Integrator
    :members: get_cmd
    :special-members: __init__
 
-Conditional
-+++++++++++
-.. autoclass:: crappy.blocks.generator_path.Conditional
-   :members: get_cmd
-   :special-members: __init__
-
 Ramp
 ++++
 .. autoclass:: crappy.blocks.generator_path.Ramp
    :members: get_cmd
    :special-members: __init__
 
 Sine
@@ -200,25 +200,25 @@
 .. autoclass:: crappy.blocks.generator_path.Sine
    :members: get_cmd
    :special-members: __init__
 
 Parent Path
 +++++++++++
 
+Meta Path
+"""""""""
+.. autoclass:: crappy.blocks.generator_path.meta_path.MetaPath
+   :special-members: __init__
+
 Path
 """"
 .. autoclass:: crappy.blocks.generator_path.meta_path.Path
    :members: get_cmd, parse_condition, log
    :special-members: __init__
 
-Meta Path
-"""""""""
-.. autoclass:: crappy.blocks.generator_path.meta_path.MetaPath
-   :special-members: __init__
-
 Camera Processes
 ----------------
 
 Camera Process
 ++++++++++++++
 .. autoclass:: crappy.blocks.camera_processes.CameraProcess
    :members: set_shared, run
```

### Comparing `crappy-2.0.0.dev1/docs/source/crappy_docs/cameras.rst` & `crappy-2.0.0.dev2/docs/source/crappy_docs/cameras.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 =======
 Cameras
 =======
 
 Regular Cameras
 ---------------
 
-Fake Camera
-+++++++++++
-.. autoclass:: crappy.camera.FakeCamera
-   :members: open, get_image
-   :special-members: __init__
-
-File Reader
-+++++++++++
-.. autoclass:: crappy.camera.FileReader
-   :members: open, get_image
-   :special-members: __init__
-
 Camera GStreamer
 ++++++++++++++++
 .. autoclass:: crappy.camera.CameraGstreamer
    :members: open, get_image, close
    :special-members: __init__
 
 Camera OpenCV
 +++++++++++++
 .. autoclass:: crappy.camera.CameraOpencv
    :members: open, get_image, close
    :special-members: __init__
 
-PiCamera
-++++++++
-.. autoclass:: crappy.camera.PiCamera
+Fake Camera
++++++++++++
+.. autoclass:: crappy.camera.FakeCamera
+   :members: open, get_image
+   :special-members: __init__
+
+File Reader
++++++++++++
+.. autoclass:: crappy.camera.FileReader
+   :members: open, get_image
+   :special-members: __init__
+
+Raspberry Pi Camera
++++++++++++++++++++
+.. autoclass:: crappy.camera.RaspberryPiCamera
    :members: open, get_image, close
    :special-members: __init__
 
 Seek Thermal Pro
 ++++++++++++++++
 .. autoclass:: crappy.camera.SeekThermalPro
    :members: open, get_image, close
@@ -52,70 +52,66 @@
 .. autoclass:: crappy.camera.XiAPI
    :members: open, get_image, close
    :special-members: __init__
 
 CameraLink Cameras
 ------------------
 
-Bi Spectral
-+++++++++++
-.. autoclass:: crappy.camera.cameralink.BiSpectral
-   :members: open, get_image
-   :special-members: __init__
-
-Camera Link
-+++++++++++
-.. autoclass:: crappy.camera.cameralink.CLCamera
+Basler Ironman Camera Link
+++++++++++++++++++++++++++
+.. autoclass:: crappy.camera.cameralink.BaslerIronmanCameraLink
    :members: open, get_image, close
    :special-members: __init__
 
-JAI
-+++
-.. autoclass:: crappy.camera.cameralink.Jai
+JAI GO-5000C-PMCL
++++++++++++++++++
+.. autoclass:: crappy.camera.cameralink.JaiGO5000CPMCL
    :members: open, get_image
    :special-members: __init__
 
-JAI 8
-+++++
-.. autoclass:: crappy.camera.cameralink.Jai8
+JAI GO-5000C-PMCL 8 bits
+++++++++++++++++++++++++
+.. autoclass:: crappy.camera.cameralink.JaiGO5000CPMCL8Bits
    :members: open
    :special-members: __init__
 
 Parent Camera
 -------------
 
 Camera
 ++++++
 .. autoclass:: crappy.camera.Camera
    :members: open, get_image, close, log, add_bool_setting, add_choice_setting,
-             add_scale_setting, add_trigger_setting, set_all
+             add_scale_setting, add_trigger_setting, add_software_roi,
+             reload_software_roi, apply_soft_roi, set_all
    :special-members: __init__, __getattr__, __setattr__
 
 Meta Camera
 +++++++++++
 .. autoclass:: crappy.camera.MetaCamera
    :special-members: __init__
 
 Camera Settings
 +++++++++++++++
 
 Camera Setting
 """"""""""""""
 .. autoclass:: crappy.camera.meta_camera.camera_setting.CameraSetting
-   :members: value, log
+   :members: value, log, reload
    :special-members: __init__
 
 Camera Bool Setting
 """""""""""""""""""
 .. autoclass:: crappy.camera.meta_camera.camera_setting.CameraBoolSetting
    :special-members: __init__
 
 Camera Choice Setting
 """""""""""""""""""""
 .. autoclass:: crappy.camera.meta_camera.camera_setting.CameraChoiceSetting
+   :members: reload
    :special-members: __init__
 
 Camera Scale Setting
 """"""""""""""""""""
 .. autoclass:: crappy.camera.meta_camera.camera_setting.CameraScaleSetting
-   :members: value
+   :members: value, reload
    :special-members: __init__
```

### Comparing `crappy-2.0.0.dev1/docs/source/crappy_docs/inouts.rst` & `crappy-2.0.0.dev2/docs/source/crappy_docs/inouts.rst`

 * *Files 2% similar despite different names*

```diff
@@ -43,23 +43,17 @@
 
 GPIO Switch
 +++++++++++
 .. autoclass:: crappy.inout.GPIOSwitch
    :members: open, set_cmd, close
    :special-members: __init__
 
-GSM
-+++
-.. autoclass:: crappy.inout.GSM
-   :members: open, set_cmd, close
-   :special-members: __init__
-
-Kollmorgen
-++++++++++
-.. autoclass:: crappy.inout.Koll
+Kollmorgen AKD PDMM
++++++++++++++++++++
+.. autoclass:: crappy.inout.KollmorgenAKDPDMM
    :members: open, set_cmd, get_data, close
    :special-members: __init__
 
 Labjack T7
 ++++++++++
 .. autoclass:: crappy.inout.LabjackT7
    :members: open, set_cmd, get_data, close, make_zero
@@ -99,29 +93,35 @@
 NI DAQmx
 ++++++++
 .. autoclass:: crappy.inout.NIDAQmx
    :members: open, set_cmd, get_data, start_stream, get_stream, stop_stream,
              close
    :special-members: __init__
 
-OpSens
-++++++
-.. autoclass:: crappy.inout.OpSens
+OpSens HandySens
+++++++++++++++++
+.. autoclass:: crappy.inout.HandySens
    :members: open, get_data, close
    :special-members: __init__
 
 PiJuice
 +++++++
 .. autoclass:: crappy.inout.PiJuice
    :members: open, get_data, close
    :special-members: __init__
 
-Spectrum
-++++++++
-.. autoclass:: crappy.inout.Spectrum
+Sim868
+++++++
+.. autoclass:: crappy.inout.Sim868
+   :members: open, set_cmd, close
+   :special-members: __init__
+
+Spectrum M2I 4711
++++++++++++++++++
+.. autoclass:: crappy.inout.SpectrumM2I4711
    :members: open, start_stream, get_stream, stop_stream, close
    :special-members: __init__
 
 Waveshare AD/DA
 +++++++++++++++
 .. autoclass:: crappy.inout.WaveshareADDA
    :members: open, set_cmd, get_data, close
```

### Comparing `crappy-2.0.0.dev1/docs/source/developers.rst` & `crappy-2.0.0.dev2/docs/source/developers.rst`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/docs/source/documentation.rst` & `crappy-2.0.0.dev2/docs/source/documentation.rst`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/docs/source/embedded.rst` & `crappy-2.0.0.dev2/docs/source/embedded.rst`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 - `Adafruit's MPRLS <https://www.adafruit.com/product/3965>`_ pressure sensor
 - `SparkFun's NAU7802 <https://www.sparkfun.com/products/15242>`_ load cell
   conditioner
 - `The PiJuice <https://uk.pi-supply.com/products/pijuice-standard>`_ Raspberry
   Pi power platform
 - `Waveshare's AD/DA <https://www.waveshare.com/high-precision-ad-da-
   board.htm>`_ ADC and DAC HAT
-- `The PiCamera <https://www.raspberrypi.com/products/camera-module-v2/>`_
+- `The Raspberry Pi Camera <https://www.raspberrypi.com/products/camera-module-v2/>`_
 - `Pololu's Tic <https://www.pololu.com/product/3140>`_ stepper motor
   controllers
 
 These devices can be integrated in two different ways into setups driven with
 Crappy. These two options are presented below.
 
 Using the GPIOs of an SBC
```

### Comparing `crappy-2.0.0.dev1/docs/source/features.rst` & `crappy-2.0.0.dev2/docs/source/features.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,32 +15,32 @@
 - :ref:`Grapher`
 
   Plots real-time 2D graphs. Possible to plot several data sets on a same graph.
 
   Most of the `examples <https://github.com/LaboratoireMecaniqueLille/crappy/
   tree/master/Examples>`_ include a Grapher block, refer to them for a use case.
 
-- :ref:`Drawing`
+- :ref:`Canvas`
 
   Displays data on top of a static image, e.g. for having a real-time
   temperature map.
 
   Refer to the `drawing.py <https://github.com/LaboratoireMecaniqueLille/
   crappy/blob/master/Examples/drawing.py>`_ example for a use case.
 
-- :ref:`Reader`
+- :ref:`Link Reader`
 
   Prints the received values in the terminal. Mostly useful for debugging.
 
-  No example featuring a Reader block is currently distributed.
+  No example featuring a Link Reader block is currently distributed.
 
 - :ref:`Dashboard`
 
   Prints received values in a popup window and with a nicer formatting than
-  :ref:`Reader`.
+  :ref:`Link Reader`.
 
   No example featuring a Dashboard block is currently distributed.
 
 Data recording
 ++++++++++++++
 
 - :ref:`Recorder`
@@ -109,26 +109,26 @@
 
   Performs real-time video-extensometry on two to four dots and returns the `x`
   and `y` strains.
 
   Refer to the `ve_fake_test.py <https://github.com/LaboratoireMecaniqueLille/
   crappy/blob/master/Examples/ve_fake_test.py>`_ example for a use case.
 
-- :ref:`DIS VE`
+- :ref:`DIC VE`
 
   Performs DIS correlation just like :ref:`DIS Correl` but only on the areas
   selected by the user, and returns the `x` and `y` displacement for each area.
   Can be used to replace :ref:`Video Extenso` on speckled samples, each area
   playing the same role as a dot.
 
   No example featuring a Disve block is currently distributed.
 
 - :ref:`GPU VE`
 
-  Same as :ref:`DIS VE` except the computation is done on a Cuda-compatible GPU.
+  Same as :ref:`DIC VE` except the computation is done on a Cuda-compatible GPU.
 
   No example featuring a GPUve block is currently distributed.
 
 - :ref:`Auto Drive`
 
   Allows moving a camera performing video-extensometry and mounted on an
   actuator, so that the barycenter of the dots remains in the center of the
@@ -143,20 +143,20 @@
 
   Generates a signal following a predefined pattern. See :ref:`the tutorials
   <2. Adding signal generators>` for information on how to use it.
 
   Refer to the `generator.py <https://github.com/LaboratoireMecaniqueLille/
   crappy/blob/master/Examples/generator.py>`_ example for a use case.
 
-- :ref:`GUI`
+- :ref:`Button`
 
   Generates a signal when the user clicks on a button in a GUI. Useful for
   triggering a behavior during an assay.
 
-  No example featuring a GUI block is currently distributed.
+  No example featuring a Button block is currently distributed.
 
 - :ref:`PID`
 
   Generates a signal based on the target and measured inputs according to a PID
   controller logic.
 
   Refer to the `pid.py <https://github.com/LaboratoireMecaniqueLille/crappy/
@@ -259,15 +259,15 @@
 - :ref:`Camera OpenCV`
 
   This camera object opens video streams using OpenCV. It allows tuning the
   device number, as well as the image format and the number of channels. It is
   mostly compatible with USB cameras, and its dependencies are straightforward
   to install.
 
-- :ref:`Camera Link`
+- :ref:`Basler Ironman Camera Link`
 
   Allows reading from a camera communicating over Camera Link plugged to a
   `microEnable 5 ironman AD8-PoCL <https://www.baslerweb.com/en/products/
   acquisition-cards/microenable-5-ironman/>`_ PCIexpress board. May as well
   work with similar boards.
 
   .. Important::
@@ -284,30 +284,31 @@
   Doesn't require any hardware, used mainly for debugging and prototyping.
 
 - :ref:`File Reader`
 
   Successively reads images already saved in a folder, and returns them. No
   image acquisition is performed and no hardware is required.
 
-- :ref:`JAI`
+- :ref:`JAI GO-5000C-PMCL`
 
   Allows reading from a `Jai GO-5000M-PMCL <https://www.jai.com/products/
-  go-5000c-pmcl>`_ camera. It relies on the :ref:`Camera Link` object.
+  go-5000c-pmcl>`_ camera. It relies on the :ref:`Basler Ironman Camera Link`
+  object.
 
   .. Important::
      This camera object relies on C++ libraries, which are not distributed with
      ``pip``. They are only available using a ``setup`` install, see
      :ref:`Installation` for details.
 
   .. Important::
      This camera object hasn't been tested on recent releases !
 
-- :ref:`PiCamera`
+- :ref:`Raspberry Pi Camera`
 
-  Allows reading images from a PiCamera, using a Raspberry Pi.
+  Allows reading images from a Raspberry Pi Camera, using a Raspberry Pi.
 
   .. Important:: Can only be run on a Raspberry Pi !
 
 - :ref:`Seek Thermal Pro`
 
   Allows reading images from a Seek Thermal `Compact Pro <https://www.thermal.
   com/compact-series.html>`_ infrared camera.
@@ -334,25 +335,25 @@
   /drives/servo/s300/>`_ servomotor conditioner in speed. May as well work on
   other conditioners from the same brand, although it hasn't been tested.
 
   .. Important::
      This actuator was written for a specific application, so it may not be
      usable as-is in the general case.
 
-- :ref:`Biotens`
+- :ref:`JVL Mac140`
 
   Drives JVL's `MAC140 <https://www.jvl.dk/276/integrated-servo-motors-mac050
   -141>`_ integrated servomotor in speed or in position. Probably works with
   other integrated servomotors from JVL, although it hasn't been tested.
 
   .. Important::
      This actuator was written for a specific application, so it may not be
      usable as-is in the general case.
 
-- :ref:`CM Drive`
+- :ref:`Schneider MDrive 23`
 
   Drives Schneider Electric's `MDrive 23 <https://www.novantaims.com/downloads
   /quickreference/mdi23plus_qr.pdf>`_ stepper motor in speed or in position.
   Probably works with other stepper motors in the same range of products,
   although it hasn't been tested.
 
   .. Important::
@@ -360,24 +361,27 @@
      usable as-is in the general case.
 
 - :ref:`Fake Motor`
 
   Emulates the dynamic behavior of a DC motor, but doesn't drive any hardware.
   Used in the examples, may also be used for prototyping or debugging.
 
-- :ref:`Motor kit pump`
+- :ref:`Adafruit DC Motor Hat`
 
-  Drives Adafruit's `DC & Stepper Motor HAT for Raspberry Pi <https://www.
-  adafruit.com/product/2348>`_ in Volts, using Adafruit's Blinka library.
+  Drives up to 4 DC motors using Adafruit's `DC & Stepper Motor HAT for
+  Raspberry Pi <https://www.adafruit.com/product/2348>`_, using either
+  Adafruit's Blinka library or :mod:`smbus2` if driven from a Raspberry Pi.
+  Although this component can also drive stepper motors, this feature was not
+  implemented.
 
   .. Important::
      This actuator was written for a specific application, so it may not be
      usable as-is in the general case.
 
-- :ref:`Oriental`
+- :ref:`Oriental ARD-K`
 
   Drives Oriental Motor's `ARD-K <https://catalog.orientalmotor.com/item/s-
   closed-loop-stepper-motor-drivers-dc-input/ard-closed-loop-stepper-driver-
   pulse-input-dc/ard-k>`_ stepper motor driver in speed or in position. Probably
   works with other stepper motor drivers in the same range of products, although
   it hasn't been tested.
 
@@ -387,49 +391,50 @@
 
 - :ref:`Pololu Tic`
 
   Drives Pololu's `Tic <https://www.pololu.com/category/212/tic-stepper-motor-
   controllers>`_ stepper motor drivers in speed or in position. Designed for
   driving all the Tic drivers, but tested only on the 36v4 model.
 
-- :ref:`Servostar`
+- :ref:`Kollmorgen ServoStar 300`
 
   Drives Kollmorgen's `Servostar 300 <https://www.kollmorgen.com/en-us/products
   /drives/servo/s300/>`_ servomotor conditioner in position or sets it to the
   analog driving mode. This is the same conditioner as for the :ref:`Biaxe`
   actuator, but this object was designed for an other application.
 
   .. Important::
      This actuator was written for a specific application, so it may not be
      usable as-is in the general case.
 
-- :ref:`TRA6PPD`
+- :ref:`Newport TRA6PPD`
 
   Drives Newport's `TRA6PPD <https://www.newport.com/p/TRA6PPD>`_ miniature
   linear stepper motor actuator, in speed or in position.
 
 Supported Sensors and outputs
 +++++++++++++++++++++++++++++
 
 Acquisition boards
 """"""""""""""""""
 
 - :ref:`Labjack T7`
 
-  Controls Labjack's `T7 <https://labjack.com/products/t7>`_ acquisition board.
+  Controls Labjack's `T7 <https://labjack.com/products/labjack-t7>`_
+  acquisition board.
 
 - :ref:`Labjack UE9`
 
   Controls Labjack's `UE9 <https://labjack.com/products/calibration-service-
   with-cert-u6-ue9-t7>`_ acquisition board.
 
 - :ref:`Labjack T7 Streamer`
 
-  Controls Labjack's `T7 <https://labjack.com/products/t7>`_ acquisition board
-  in streaming mode.
+  Controls Labjack's `T7 <https://labjack.com/products/labjack-t7>`_
+  acquisition board in streaming mode.
 
 - :ref:`Waveshare AD/DA`
 
   Controls Waveshare's `AD/DA <https://www.waveshare.com/product/raspberry-pi/
   hats/ad-da-audio-sensors/high-precision-ad-da-board.htm>`_ Raspberry Pi
   acquisition hat. May be used from any device with a proper wiring, but more
   convenient to use from a Raspberry Pi. Communicates over SPI.
@@ -454,16 +459,16 @@
 
   Reads voltages from Adafruit's `ADS 1115 <https://www.adafruit.com/product/
   1085>`_ ADC. Communicates over I2C.
 
 - :ref:`Agilent 34420A`
 
   Reads voltages or resistances from Agilent's `34420A <https://www.keysight.
-  com/us/en/product/34420A/micro-ohm-meter.html>`_ precision multimeter.
-  Communicates over serial.
+  com/us/en/product/34420A/micro-ohm-meter.html?&cc=FR&lc=fre>`_ precision
+  multimeter. Communicates over serial.
 
 - :ref:`MCP9600`
 
   Reads temperatures from Adafruit's `MCP9600 <https://www.adafruit.com/product
   /4101>`_ thermocouple amplifier. Communicates over I2C.
 
 - :ref:`MPRLS`
@@ -482,22 +487,22 @@
   www.kubii.fr/14-chargeurs-alimentations-raspberry/2019-pijuice-hat-kubii-
   3272496008793.html>`_ Raspberry Pi power supply.
 
   .. Important::
      This inout was written for a specific application, so it may not be
      usable as-is in the general case.
 
-- :ref:`OpSens`
+- :ref:`OpSens HandySens`
 
   Reads data from OpSens' `single channel signal conditioner <https://opsens-
-  solutions.com/products/signal-conditioners-oem-boards/picosens/>`_ for
+  solutions.com/products/signal-conditioners-oem-boards/handysens-w/>`_ for
   fiber-optics temperature, strain, pressure or position measurement.
   Communicates over serial.
 
-- :ref:`Spectrum`
+- :ref:`Spectrum M2I 4711`
 
   Reads voltages from Spectrum's `M2i 4711 EXP <https://spectrum-
   instrumentation.com/products/details/M2i4711.php>`_ high-speed ADC
   communicating over PCIexpress.
 
 Multi-device drivers
 """"""""""""""""""""
@@ -533,29 +538,29 @@
 
 - :ref:`GPIO PWM`
 
   Controls a PWM output on a single GPIO of a Raspberry Pi.
 
   .. Important:: Only works on a Raspberry Pi !
 
-- :ref:`GSM`
+- :ref:`Sim868`
 
   Uses Waveshare's `GSM/GPRS/GNSS/Bluetooth hat <https://www.waveshare.com/
   gsm-gprs-gnss-hat.htm>`_ for sending SMS. The other functionalities are not
   implemented. Usable from any device with a proper wiring, but more convenient
   to use with a Raspberry Pi. Communicates over serial.
 
   .. Important::
      This inout was written for a specific application, so it may not be
      usable as-is in the general case.
 
 Enhanced actuators
 """"""""""""""""""
 
-- :ref:`Kollmorgen`
+- :ref:`Kollmorgen AKD PDMM`
 
   Drives Kollmorgen's `AKD PDMM <https://www.kollmorgen.com/en-us/products/
   drives/servo/akd-pdmm/akd-pdmm-programmable-drive-multi-axis-master/>`_
   servomotor controller. As this device supports many settings, it was decided
   to consider it as an inout to fully take advantage of its versatility.
 
   .. Important::
```

### Comparing `crappy-2.0.0.dev1/docs/source/installation.rst` & `crappy-2.0.0.dev2/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/docs/source/tutorials/c_modules.rst` & `crappy-2.0.0.dev2/docs/source/tutorials/c_modules.rst`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/docs/source/tutorials/custom_blocks.rst` & `crappy-2.0.0.dev2/docs/source/tutorials/custom_blocks.rst`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/docs/source/tutorials/getting_started.rst` & `crappy-2.0.0.dev2/docs/source/tutorials/getting_started.rst`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/docs/source/what_is_crappy.rst` & `crappy-2.0.0.dev2/docs/source/what_is_crappy.rst`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/other_examples/daqmx_thermocouple.py` & `crappy-2.0.0.dev2/examples/other_examples/daqmx_thermocouple.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/other_examples/dio_daqmx.py` & `crappy-2.0.0.dev2/examples/other_examples/dio_daqmx.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/other_examples/gpu_correl_advanced.py` & `crappy-2.0.0.dev2/examples/other_examples/gpu_correl_advanced.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/other_examples/gpu_correl_basic.py` & `crappy-2.0.0.dev2/examples/other_examples/gpu_correl_basic.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/other_examples/gpu_correl_fake_test.py` & `crappy-2.0.0.dev2/examples/other_examples/gpu_correl_fake_test.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/other_examples/labjack_t7_stream.py` & `crappy-2.0.0.dev2/examples/other_examples/labjack_t7_stream.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/other_examples/labjack_t7_tensile_1.py` & `crappy-2.0.0.dev2/examples/other_examples/labjack_t7_tensile_1.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/other_examples/labjack_t7_tensile_2.py` & `crappy-2.0.0.dev2/examples/other_examples/labjack_t7_tensile_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
   rec_ve = crappy.blocks.Recorder('results_ve.csv')
   crappy.link(ve, rec_ve)
   # Quick remark on recorders: we used two separate blocks for daq and ve.
   # This is because they can only take a SINGLE INPUT. Because the input blocks
   # may run at different frequencies, it is not possible to build a csv file
   # simply from two or more separate sources.
   # We could interpolate them in the same
-  # timebase (see block Multiplex) but this means loosing the raw data. It is
+  # timebase (see block Multiplexer) but this means loosing the raw data. It is
   # much better to perform this interpolation in post-processing if necessary
 
   # Our force against time plot
   graph_f = crappy.blocks.Grapher(('t(s)', 'F(N)'))
   # Adding a Mean modifier to average the points
   # It lowers the frequency and makes the graph smoother
   crappy.link(daq, graph_f, modifier=crappy.modifier.Mean(10))
```

### Comparing `crappy-2.0.0.dev1/examples/other_examples/labjack_t7_thermocouple.py` & `crappy-2.0.0.dev2/examples/other_examples/labjack_t7_thermocouple.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/other_examples/microcontroller_example.py` & `crappy-2.0.0.dev2/examples/other_examples/microcontroller_example.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/other_examples/spectrum.py` & `crappy-2.0.0.dev2/examples/other_examples/spectrum.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   ranges = [10000] * len(channels)  # -10/+10V (in mV)
   # This will NOT apply the gain to the stream, only save a key in the h5
   gains = [1] * len(channels)
   save_file = "./out.h5"
 
   chan_names = [f'ch{i}' for i in channels]
 
-  spectrum = crappy.blocks.IOBlock('Spectrum',
+  spectrum = crappy.blocks.IOBlock('SpectrumM2I4711',
                                    ranges=ranges,
                                    channels=channels,
                                    streamer=True,
                                    labels=['t(s)', 'stream'])
 
   graph = crappy.blocks.Grapher(*[('t(s)', i) for i in chan_names])
```

### Comparing `crappy-2.0.0.dev1/examples/other_examples/video_extenso_auto_drive.py` & `crappy-2.0.0.dev2/examples/other_examples/video_extenso_auto_drive.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 if __name__ == '__main__':
 
   # The Block acquiring the images and performing video-extensometry
   ve = crappy.blocks.VideoExtenso(camera='XiAPI', display_images=True)
 
   # The Block driving the Actuator for following the spots
-  auto_drive = crappy.blocks.AutoDrive(actuator={'name': 'CMDrive',
-                                                 'port': '/dev/ttyUSB0'},
-                                       direction='X-')
+  auto_drive = crappy.blocks.AutoDriveVideoExtenso(
+      actuator={'name': 'SchneiderMDrive23', 'port': '/dev/ttyUSB0'},
+      direction='X-')
   crappy.link(ve, auto_drive)
 
   # The Block displaying the strain in real-time
   graph_extenso = crappy.blocks.Grapher(('t(s)', 'Exx(%)'), ('t(s)', 'Eyy(%)'))
   crappy.link(ve, graph_extenso)
 
   # Starting the test
```

### Comparing `crappy-2.0.0.dev1/examples/other_examples/video_extenso_auto_drive_full.py` & `crappy-2.0.0.dev2/examples/other_examples/video_extenso_auto_drive_full.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 if __name__ == '__main__':
 
   # The Block acquiring the images and performing video-extensometry
   ve = crappy.blocks.VideoExtenso(camera='XiAPI', display_images=True,
                                   white_spots=False, freq=30)
 
   # The Block driving the Actuator for following the spots
-  auto_drive = crappy.blocks.AutoDrive(actuator={'name': 'CMDrive',
-                                                 'port': '/dev/ttyUSB0'},
-                                       direction='X-')
+  auto_drive = crappy.blocks.AutoDriveVideoExtenso(
+      actuator={'name': 'SchneiderMDrive23', 'port': '/dev/ttyUSB0'},
+      direction='X-')
   crappy.link(ve, auto_drive)
 
   # The Block driving the extension of the test sample
   gen = crappy.blocks.Generator(
     path=[{'type': 'CyclicRamp', 'condition1': 'Exx(%)>20', 'speed1': 20 / 60,
            'condition2': 'F(N)<.1', 'speed2': -20 / 60, 'cycles': 5}])
   crappy.link(ve, gen)
```

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/custom_actuator.py` & `crappy-2.0.0.dev2/examples/ready_to_run/custom_actuator.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     print("Closing device...")
     sleep(.5)
     print("Device closed")
 
   # At least one of the two following methods (set_speed and set_position)
   # needs to be defined. Getters (get_speed and get_position) can be defined
   # too if the actuator supports it.
-  def set_position(self, target, _=None):
+  def set_position(self, target, _):
     self.pos = target
 
   def get_position(self):
     return self.pos + 0.1  # To illustrate the difference with the target
 
   def stop(self):
     """Called before closing, should stop the actuator."""
```

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/custom_block.py` & `crappy-2.0.0.dev2/examples/ready_to_run/custom_block.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/custom_camera.py` & `crappy-2.0.0.dev2/examples/ready_to_run/custom_camera.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/custom_in.py` & `crappy-2.0.0.dev2/examples/ready_to_run/custom_in.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/custom_out.py` & `crappy-2.0.0.dev2/examples/ready_to_run/custom_out.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/dic_ve_fake_test.py` & `crappy-2.0.0.dev2/examples/ready_to_run/dic_ve_fake_test.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/dic_ve_simple.py` & `crappy-2.0.0.dev2/examples/ready_to_run/dic_ve_simple.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/dis_correl_basic.py` & `crappy-2.0.0.dev2/examples/ready_to_run/dis_correl_basic.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/dis_correl_fake_test.py` & `crappy-2.0.0.dev2/examples/ready_to_run/dis_correl_fake_test.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/dis_correl_fake_test_strain_controlled.py` & `crappy-2.0.0.dev2/examples/ready_to_run/dis_correl_fake_test_strain_controlled.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,16 @@
 
   # The PID block takes TWO inputs: the setpoint and the feedback
   # Here the setpoint is coming from the generator (target_Exx(%))
   # and the feedback is the strain measured with the DIC (measured_Exx(%))
   # The output is the command sent to the machine
   # In a real-world scenario, consider using out_min and out_max
   # to clamp the output value and i_limit to prevent over_integration.
-  pid = crappy.blocks.PID(kp=0.5, ki=2, kd=0.05, target_label='target_Exx(%)',
+  pid = crappy.blocks.PID(kp=0.5, ki=1.0, kd=0.025,
+                          setpoint_label='target_Exx(%)',
                           input_label='measured_Exx(%)', send_terms=True)
 
   # We link the two inputs and the output
   # The order does not matter, the inputs are identified thanks to the
   # keywords target_label (setpoint) and input_label (feedback)
   crappy.link(generator, pid)
   crappy.link(dis, pid)
```

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/displayer.py` & `crappy-2.0.0.dev2/examples/ready_to_run/displayer.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/fake_test.py` & `crappy-2.0.0.dev2/examples/ready_to_run/fake_test.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/furnace_simulation.py` & `crappy-2.0.0.dev2/examples/ready_to_run/furnace_simulation.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 No hardware required.
 """
 
 import crappy
 
 SPEED = 20  # Speed multiplier of the simulation
 
-P = .1
-I = .1 * SPEED
-D = 10 / SPEED
+P = 0.1
+I = 0.01 * SPEED
+D = 1 / SPEED
 
 
 class Delay(crappy.Modifier):
   """Class to add a delay on the feedback."""
 
   def __init__(self, delay):
     super().__init__()
     self.delay = delay
     self.t = 't(s)'
     self.v = 'T'
     self.hist = []
 
-  def evaluate(self, data):
+  def __call__(self, data):
     self.hist.append(data)
     r = dict(data)
     while self.hist and self.hist[0][self.t] + self.delay <= r[self.t]:
       del self.hist[0]
     v_table = [d[self.v] for d in self.hist]
     r[self.v] = sum(v_table) / len(v_table)
     return r
```

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/generator.py` & `crappy-2.0.0.dev2/examples/ready_to_run/generator.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/generator_steps.py` & `crappy-2.0.0.dev2/examples/ready_to_run/generator_steps.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/mean.py` & `crappy-2.0.0.dev2/examples/ready_to_run/mean.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/modifiers.py` & `crappy-2.0.0.dev2/examples/ready_to_run/modifiers.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 No hardware required.
 """
 
 import crappy
 
 
 # Example of class used as a Modifier
-class My_offset_modifier:
+class My_offset_modifier(crappy.Modifier):
   def __init__(self, offset):
+    super().__init__()
     self.offset = offset
 
-  def evaluate(self, data):
+  def __call__(self, data):
     """Method returning the modified values.
 
     Remember: data is ALWAYS a :obj:`dict`.
     Returning :obj:`None` will drop the data.
     """
 
     for k in data:
@@ -54,14 +55,14 @@
                 crappy.modifier.MovingAvg(100),
                 # Will add an offset
                 My_offset_modifier(5),
                 # Will multiply the result by 10
                 mul_by_10])
 
   # This block will simply print "Triggered" followed by the received data
-  r = crappy.blocks.Reader('Triggered')
+  r = crappy.blocks.LinkReader('Triggered')
 
   # Only forward data when the label "cycle" changed its value
   crappy.link(generator, r,
               modifier=crappy.modifier.TrigOnChange('cycle'))
 
   crappy.start()
```

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/multiplexer.py` & `crappy-2.0.0.dev2/examples/ready_to_run/multiplexer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # coding: utf-8
 
 """
-Example demonstrating the use of ``crappy.blocks.Multiplex``.
+Example demonstrating the use of ``crappy.blocks.Multiplexer``.
 
 This block interpolates data from several parents in a common timebase.
 
 No required hardware.
 """
 
 import crappy
 
 
 class Delay(crappy.modifier.Modifier):
-  """Modifier to add a delay to one of the inputs, demonstrating how Multiplex
-  will wait for data."""
+  """Modifier to add a delay to one of the inputs, demonstrating how
+  Multiplexer will wait for data."""
 
   def __init__(self, n):
     super().__init__()
     self.n = n
     self.hist = []
 
-  def evaluate(self, data):
+  def __call__(self, data):
     self.hist.append(data)
     if len(self.hist) >= self.n:
       return self.hist.pop(0)
 
 
 if __name__ == "__main__":
   g1 = crappy.blocks.Generator([
@@ -32,16 +32,16 @@
       ], freq=100, cmd_label='cmd1')
 
   g2 = crappy.blocks.Generator([
     dict(type='CyclicRamp', speed2=-1, speed1=1,
          condition1='cmd2>1', condition2='cmd2<-1', cycles=0, init_value=0)
       ], freq=50, cmd_label='cmd2')
 
-  mul = crappy.blocks.Multiplex(display_freq=True,
-                                out_labels=['cmd1', 'cmd2'])
+  mul = crappy.blocks.Multiplexer(display_freq=True,
+                                  out_labels=['cmd1', 'cmd2'])
 
   # crappy.link(g1, mul)
   crappy.link(g1, mul, modifier=Delay(50))
   crappy.link(g2, mul)
 
   graph = crappy.blocks.Grapher(('t(s)', 'cmd1'), ('t(s)', 'cmd2'))
```

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/pid.py` & `crappy-2.0.0.dev2/examples/ready_to_run/pid.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,16 @@
   crappy.link(mot, graph_m, modifier=crappy.modifier.Mean(10))
   crappy.link(g, graph_m, modifier=crappy.modifier.Mean(10))
   # To see what happens without PID
   # crappy.link(g, mot)
   # crappy.start()
 
   p = 38 / kv
-  i = 2
-  d = .05
+  i = 76 / kv
+  d = 1.9 / kv
 
   pid = crappy.blocks.PID(kp=p,
                           ki=i,
                           kd=d,
                           out_max=10,
                           out_min=-10,
                           i_limit=(-5, 5),
```

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/read.py` & `crappy-2.0.0.dev2/examples/ready_to_run/read.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/read_write.py` & `crappy-2.0.0.dev2/examples/ready_to_run/read_write.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/video_extenso_fake_test.py` & `crappy-2.0.0.dev2/examples/ready_to_run/video_extenso_fake_test.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/ready_to_run/video_extenso_simple.py` & `crappy-2.0.0.dev2/examples/ready_to_run/video_extenso_simple.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/real_setups_scripts/biaxe.py` & `crappy-2.0.0.dev2/examples/real_setups_scripts/biaxe.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/examples/real_setups_scripts/biotens.py` & `crappy-2.0.0.dev2/examples/real_setups_scripts/biotens.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import crappy
 
 save_path = Path(f"biotens_data/{strftime('%a %b %d %H_%M_%S', gmtime())}")
 
 if __name__ == '__main__':
 
   # Quick hack for resetting the position of the clamps
-  biotens_init = crappy.actuator.Biotens()
+  biotens_init = crappy.actuator.JVLMac140()
   biotens_init.open()
   biotens_init.reset_position()
   biotens_init.set_position(5, 50)
 
   # The Block providing the signal for driving the tensile test machine
   generator = crappy.blocks.Generator([{'type': 'Constant',
                                         'condition': 'F(N)>90',
@@ -30,15 +30,15 @@
   # The Block acquiring the force from the load cell
   effort = crappy.blocks.IOBlock("Comedi", channels=[0], gain=[-48.8],
                                  labels=['t(s)', 'F(N)'])
   # This link enables feedback from the setup to the Generator
   crappy.link(effort, generator)
 
   # The Block driving the tensile test machine
-  biotens = crappy.blocks.Machine([{'type': 'Biotens',
+  biotens = crappy.blocks.Machine([{'type': 'JVLMac140',
                                     'port': '/dev/ttyUSB0',
                                     'position_label': 'position1',
                                     'cmd_label': 'cmd'}])
   crappy.link(generator, biotens)
 
   # The Block acquiring images from the setup and performing video-extensometry
   extenso = crappy.blocks.VideoExtenso(camera="XiAPI")
```

### Comparing `crappy-2.0.0.dev1/examples/real_setups_scripts/furnace.py` & `crappy-2.0.0.dev2/examples/real_setups_scripts/furnace.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 heating element of each section of the furnace. The temperature of each section
 is measured using a thermocouple.
 """
 
 import crappy
 
 # The parameters of the PID
-P = .25
-I = .03
-D = 20
+P = 0.25
+I = 0.0075
+D = 5.0
 
 # The frequency of the PWM
 FREQ = 100
 # Parameters for averaging the signals
 MED = 20
 MEAN = 50
 
@@ -41,15 +41,15 @@
 
   def __init__(self, label):
     """Initializes the parent class and sets the argument."""
 
     super().__init__()
     self._label = label
 
-  def evaluate(self, data):
+  def __call__(self, data):
     """Converts the value received on the given label from a DC voltage to a
     number of clock cycles."""
 
     if data[self._label] < 0.01:
       cmd = 0
     elif data[self._label] > .99:
       cmd = 1
```

### Comparing `crappy-2.0.0.dev1/setup.py` & `crappy-2.0.0.dev2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 """A setuptools based setup module.
 
 See:
 https://packaging.python.org/en/latest/distributing.html
 https://github.com/pypa/sampleproject
 """
 
-from setuptools import find_namespace_packages
+from setuptools import find_namespace_packages, setup, Extension
 from os import popen, walk
-from distutils.core import setup, Extension
 import platform
 
 # Reading version from __version__.py file
 with open('src/crappy/__version__.py') as file:
   for line in file:
     if line.startswith('__version__'):
       __version__ = line.split("'")[1]
@@ -91,61 +90,62 @@
     if input("would you like to install CameraLink module? ([y]/n)") != "n":
       extensions.append(cl_module)
   else:
     print("Can't find microEnable4 Device driver, clModule will not be "
           "compiled")
 
 setup(
+  # Description of the project
   name='crappy',
-
   version=__version__,
-
-  description='Command and Real-time Acquisition Parallelized in Python',
-
+  description='Command and Real-time Acquisition in Parallelized Python',
   long_description=long_description,
-
-  url='https://github.com/LaboratoireMecaniqueLille/crappy',
-
-  project_urls={'Documentation':
-                'https://crappy.readthedocs.io/en/latest/index.html'},
-
-  author='LaMcube',
-  author_email='antoine.weisrock1@centralelille.fr',
-
+  keywords='control,command,acquisition,multiprocessing',
   license='GPL V2',
-
-  zip_safe=False,
-
   classifiers=['Development Status :: 4 - Beta ',
                'Intended Audience :: Science/Research',
-               'Topic :: Software Development :: Build Tools',
                'License :: OSI Approved :: GNU General Public License v2 or '
                'later (GPLv2+)',
-               'Programming Language :: Python :: 3.6',
                'Natural Language :: English',
-               'Operating System :: OS Independent'],
+               'Operating System :: OS Independent',
+               'Programming Language :: Python :: 3.7',
+               'Programming Language :: Python :: 3.8',
+               'Programming Language :: Python :: 3.9',
+               'Programming Language :: Python :: 3.10',
+               'Topic :: Scientific/Engineering',
+               'Topic :: Software Development :: Build Tools',
+               'Topic :: Software Development :: Embedded Systems'],
+
+  # URLs of the project
+  url='https://github.com/LaboratoireMecaniqueLille/crappy',
+  download_url='https://pypi.org/project/crappy/#files',
+  project_urls={'Documentation':
+                'https://crappy.readthedocs.io/en/latest/index.html'},
 
-  keywords='control command acquisition multiprocessing',
+  # Information on the author
+  author='LaMcube',
+  author_email='antoine.weisrock1@centralelille.fr',
+  maintainer='Antoine Weisrock',
+  maintainer_email='antoine.weisrock@gmail.com',
 
+  # Packaging information
   packages=find_namespace_packages(where="src",
                                    exclude=['contrib', 'docs', 'tests*']),
-
   package_dir={"": "src"},
-
-  python_requires=">=3.6",
-
+  include_package_data=True,
   ext_package='crappy',
   ext_modules=extensions,
 
+  # Installation requirements
+  python_requires=">=3.7",
   install_requires=["numpy>=1.21.0"],
-
   extras_require={'SBC': ['smbus2',
                           'spidev',
                           'Adafruit-Blinka',
-                          'Adafruit-ADS1x15',
+                          'adafruit-circuitpython-ads1x15',
                           'adafruit-circuitpython-motorkit',
                           'adafruit-circuitpython-mprls',
                           'adafruit-circuitpython-busdevice'],
                   'image': ['opencv-python>=4.0',
                             'Pillow>=8.0.0',
                             'matplotlib>=3.3.0',
                             'SimpleITK>=2.0.0',
@@ -153,9 +153,10 @@
                   'hardware': ['pyusb>=1.1.0',
                                'pyserial>=3.4',
                                'pyyaml>=5.3'],
                   'main': ['matplotlib>=3.3.0',
                            'opencv-python>=4.0',
                            'pyserial>=3.4']},
 
-  include_package_data=True,
+  # Others
+  zip_safe=False,
 )
```

### Comparing `crappy-2.0.0.dev1/src/crappy/actuator/biaxe.py` & `crappy-2.0.0.dev2/src/crappy/lamcube/biaxe.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 ﻿# coding: utf-8
 
 import logging
-from .meta_actuator import Actuator
+from ..actuator import Actuator
 from .._global import OptionalModule
 
 try:
   import serial
 except (ModuleNotFoundError, ImportError):
   serial = OptionalModule("pyserial")
 
 
 class Biaxe(Actuator):
-  """This class can drive a Kollmorgen ServoStar 300 conditioner in speed."""
+  """This class can drive a Kollmorgen ServoStar 300 conditioner in speed.
+
+  It is used at the LaMcube for driving a bi-axial tensile test machine, hence
+  its name. The :class:`~crappy.actuator.ServoStar300` Actuator can drive the
+  same hardware, but only in position.
+  """
 
   def __init__(self,
                port: str = '/dev/ttyUSB0',
                baudrate: int = 38400,
                timeout: float = 1) -> None:
     """Sets the instance attributes.
 
@@ -33,15 +38,15 @@
     self._port = port
     self._baudrate = baudrate
     self._timeout = timeout
 
     self._speed = None
 
   def open(self) -> None:
-    """"""
+    """Opens the serial connection to the ServoStar."""
 
     self.log(logging.INFO, f"Opening the serial port {self._port} with "
                            f"baudrate {self._baudrate}")
     self._ser = serial.Serial(self._port, self._baudrate,
                               serial.EIGHTBITS, serial.PARITY_EVEN,
                               serial.STOPBITS_ONE, self._timeout)
     self._clear_errors()
@@ -55,21 +60,21 @@
     if speed != self._speed:
       self.log(logging.DEBUG, f"Writing b'J{ {speed}}\\r\\n' on port "
                               f"{self._port}")
       self._ser.write(f'J {speed}\r\n'.encode('ASCII'))
       self._speed = speed
 
   def stop(self) -> None:
-    """"""
+    """Sets the speed of the motor to `0`"""
 
     if self._ser is not None:
       self.set_speed(0)
 
   def close(self) -> None:
-    """Closes the serial connection."""
+    """Closes the serial connection to the ServoStar."""
 
     if self._ser is not None:
       self.log(logging.INFO, f"Closing the serial port {self._port}")
       self._ser.close()
 
   def _clear_errors(self) -> None:
     """Clears the errors on the ServoStar."""
```

### Comparing `crappy-2.0.0.dev1/src/crappy/actuator/biotens.py` & `crappy-2.0.0.dev2/src/crappy/actuator/jvl_mac_140.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 cmd_header = b'\x52\x52\x52\xFF\x00'
 cmd_tail = b'\xAA\xAA\x50\x50\x50\xFF\x00'
 msg_tail_last = b'\xAA\xAA'
 msg_tail_not_last = b'\xAA\xAA+'
 
 
-class Biotens(Actuator):
+class JVLMac140(Actuator):
   """This class allows driving JVL's MAC140 integrated servomotor in speed or
   in position.
 
   It interfaces with the servomotor over a serial connection.
   """
 
   def __init__(self,
@@ -71,27 +71,26 @@
     command = self._make_cmd((2, 2, 1, 2), ('B', 'B', 'h', 'B'), True)
 
     # Writing the command values to the motor registers
     cmd = [set_speed, set_torque, set_acc, command]
     self.log(logging.DEBUG, f"Writing {cmd} to port {self._port}")
     self._ser.writelines(cmd)
 
-  def set_position(self,
-                   position: float,
-                   speed: Optional[float] = None) -> None:
-    """Sets the desired target position on the actuator.
+  def set_position(self, position: float, speed: Optional[float]) -> None:
+    """Sets the desired target position on the servomotor.
 
     Args:
       position: The target position, in `mm`.
       speed: The target speed for reaching the desired position, in `mm/min`.
+        The speed must be given, otherwise an exception is raised.
     """
 
     if speed is None:
-      raise ValueError("The Biotens actuator needs both a position and a speed"
-                       " command when driven in position mode !")
+      raise ValueError("The JVLMac140 actuator needs both a position and a "
+                       "speed command when driven in position mode !")
 
     # For the conversions, there are 4096 counts/motor revolution, 1/16 encoder
     # counts/sample, and the screw thread is 5
     pos = int(round(position * 4096 / 5))
     speed = int(round(16 * 4096 * speed / (520.8 * 60 * 5)))
     acc = int(round(16 * 4096 * 10000 / (520.8 * 520.8 * 5)))
 
@@ -105,15 +104,15 @@
 
     # Writing the command values to the motor registers
     cmd = [set_position, set_speed, set_torque, set_acc, command]
     self.log(logging.DEBUG, f"Writing {cmd} to port {self._port}")
     self._ser.writelines(cmd)
 
   def get_position(self) -> float:
-    """Reads and returns the current position of the actuator, in `mm`."""
+    """Reads and returns the current position of the servomotor, in `mm`."""
 
     # We have 20 attempts for reading the position
     for _ in range(20):
       try:
         # Emptying the read buffer
         self._ser.readlines()
         # Sending command to return position
@@ -131,26 +130,26 @@
         return unpack('i', position[9:17:2])[0] * 5 / 4096.
       # Catching serial errors
       except serial.SerialException:
         pass
       sleep(0.1)
 
     # In case no value was received after 20 attempts
-    raise IOError("Could not read the position for the Biotens actuator!")
+    raise IOError("Could not read the position for the JVLMac140 actuator!")
 
   def stop(self) -> None:
-    """Sends a command for stopping the actuator."""
+    """Sends a command for stopping the servomotor."""
 
     if self._ser is not None:
       cmd = self._make_cmd((2, 2, 0, 2), ('B', 'B', 'h', 'B'), True)
       self.log(logging.DEBUG, f"Writing {cmd} to port {self._port}")
       self._ser.write(cmd)
 
   def close(self) -> None:
-    """Closes the serial connection to the actuator."""
+    """Closes the serial connection to the servomotor."""
 
     if self._ser is not None:
       self.log(logging.INFO, f"Closing the serial port {self._port}")
       self._ser.close()
 
   def reset_position(self) -> None:
     """Makes the servomotor reach its limit position, in order to re-calibrate
```

### Comparing `crappy-2.0.0.dev1/src/crappy/actuator/cm_drive.py` & `crappy-2.0.0.dev2/src/crappy/actuator/schneider_mdrive_23.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 try:
   import serial
 except (ModuleNotFoundError, ImportError):
   serial = OptionalModule("pyserial")
 
 
-class CMDrive(Actuator):
+class SchneiderMDrive23(Actuator):
   """This class can drive Schneider Electric MDrive 23 stepper motor in speed
   and in position.
 
   It communicates with the motor over a serial connection.
   """
 
   def __init__(self,
@@ -33,22 +33,22 @@
 
     super().__init__()
 
     self._port = port
     self._baudrate = baudrate
 
   def open(self) -> None:
-    """Opens the serial connection to the actuator."""
+    """Opens the serial connection to the stepper motor."""
 
     self.log(logging.INFO, f"Opening the serial port {self._port} with "
                            f"baudrate {self._baudrate}")
     self._ser = serial.Serial(self._port, self._baudrate, timeout=0.1)
 
   def set_speed(self, speed: float) -> None:
-    """Sets the target speed on the actuator.
+    """Sets the target speed of the stepper motor.
 
     Args:
       speed: The target speed to set, in `mm/min`.
     """
 
     # Closing and reopening to get rid of errors
     self._ser.close()
@@ -59,22 +59,20 @@
       self.log(logging.DEBUG, f"Writing b'SL {int(speed)}\\r' to port "
                               f"{self._port}")
       self._ser.write(f'SL {int(speed)}\r')
       self._ser.read(self._ser.inWaiting())
     else:
       self.log(logging.WARNING, "Maximum speed exceeded, not setting speed")
 
-  def set_position(self,
-                   position: float,
-                   _: Optional[float] = None) -> None:
-    """Sets the target position for the actuator.
+  def set_position(self, position: float, _: Optional[float]) -> None:
+    """Sets the target position for the stepper motor.
 
     Args:
       position: The target position to reach, in `mm`.
-      _: If also given, the speed is ignored.
+      _: The speed argument is ignored.
     """
 
     # Closing and reopening to get rid of errors
     self._ser.close()
     self._ser.open()
 
     # Sending the position command
```

### Comparing `crappy-2.0.0.dev1/src/crappy/actuator/fake_motor.py` & `crappy-2.0.0.dev2/src/crappy/actuator/fake_motor.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 
     Args:
       inertia: The inertia of the motor, in `kg.m²`.
       torque: A constant torque applied on the shaft of the motor in `N.m`.
       kv: The electrical constant of the motor, in`t/min/V`.
       rv: The internal solid friction coefficient of the motor, no unit.
       fv: The internal fluid friction coefficient of the motor, no unit.
-      simulation_speed: Speed factor of the simulation, to speed it up or slow it
-        down.
+      simulation_speed: Speed factor of the simulation, to speed it up or slow
+        it down.
       initial_speed: The initial speed of the motor, in RPM.
-      initial_pos: The initial position of the motor, in rounds.
+      initial_pos: The initial position of the motor, in turns.
     """
 
     super().__init__()
 
     self._inertia = inertia
     self._torque = torque
     self._kv = kv
```

### Comparing `crappy-2.0.0.dev1/src/crappy/actuator/ft232h/motor_kit_pump_ft232h.py` & `crappy-2.0.0.dev2/src/crappy/actuator/adafruit_dc_motor_hat.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 # coding: utf-8
 
 from struct import pack_into
 from time import sleep
-from typing import Union, List, Optional
+from typing import Union, Tuple
 import logging
 
-from ..meta_actuator import Actuator
-from ..._global import OptionalModule
-from ...tool.ft232h import FT232HServer as FT232H, USBArgsType
+from .meta_actuator import Actuator
+from .._global import OptionalModule
+
+try:
+  from adafruit_motorkit import MotorKit
+except (ImportError, ModuleNotFoundError):
+  MotorKit = OptionalModule('adafruit_motorkit',
+                            'Adafrfuit Motorkit module (adafruit_motorkit) is '
+                            'required to use this actuator')
+
+try:
+  import board
+except (ImportError, ModuleNotFoundError):
+  board = OptionalModule('board', 'Blinka is necessary to use the I2C bus')
 
 try:
   from smbus2 import SMBus
 except (ImportError, ModuleNotFoundError):
   SMBus = OptionalModule('smbus2')
 
 motor_hat_ctrl = {1: 0x26,
@@ -26,232 +37,186 @@
 
 motor_hat_neg = {1: 0x2E,
                  2: 0x36,
                  3: 0x16,
                  4: 0x1E}
 
 motor_hat_0xFF = [0x00, 0x10, 0x00, 0x00]
-motor_hat_backends = ['Pi4', 'blinka', 'ft232h']
+motor_hat_backends = ['Pi4', 'blinka']
 motor_hat_max_volt = 12
 
 
-class DCMotorHat:
+class DCMotorHat(Actuator):
   """Class for driving Adafruit's DC motor HAT.
 
-  This class serves as a basis for building Actuators in Crappy, but is not one
-  itself. It is used by the :class:`Motorkit_pump` Actuator.
+  It can drive up to four DC motors in speed only. The acquisition of the speed
+  has not been implemented so far. It can either rely on Adafruit's Blinka
+  library, or on :mod:`smbus2` if used from a Raspberry Pi.
+
+  Important:
+    As this Actuator can drive up to 4 motors simultaneously, it takes a
+    :obj:`tuple` as a command, see :meth:`set_speed`. Regular Actuators receive
+    their commands as :obj:`float`. A :class:`~crappy.modifier.Modifier` can be
+    used for converting a :obj:`float` command from a
+    :class:`~crappy.blocks.Generator` to a :obj:`tuple`.
 
   Note:
-    This device can also drive stepper motors, but this feature isn't included
-    here.
-
-  It is intended for Raspberry Pis but can also be used from any other device
-  interfacing over I2C assuming a proper wiring.
+    The DC Motor Hat can also drive stepper motors, but this feature isn't
+    included here.
   """
 
   def __init__(self,
-               motor_nrs: List[int],
+               backend: str,
                device_address: int = 0x60,
-               i2c_port: int = 1,
-               bus: Optional[FT232H] = None) -> None:
-    """Resets the HAT and initializes it.
-
-    Args:
-      motor_nrs: The list of the motors to drive. Its elements should be
-        integers between 1 and 4, corresponding to the indexes of the motors to
-        drive.
-      device_address: The I2C address of the HAT. The default address is
-        `0x60`, but it is possible to change this setting by cutting traces on
-        the board.
-      i2c_port: The I2C port over which the HAT should communicate. On most
-        Raspberry Pi models the default I2C port is `1`.
-      bus: If given, the I2C commands are sent by the corresponding
-        :class:`ft232h_server` instance, in the situation when the hat is
-        controlled from a PC through an FT232H.
-    """
-
-    if not all(i in range(1, 5) for i in motor_nrs):
-      raise ValueError("The DC motor hat can only drive up to 4 DC motors at "
-                       "a time !")
-
-    if not isinstance(device_address, int):
-      raise TypeError("device_address should be an integer between 0 and 127.")
-    self._address = device_address
-
-    if not isinstance(i2c_port, int):
-      raise TypeError("i2c_port should be an integer !")
-
-    if not bus:
-      self._bus = SMBus(i2c_port)
-    else:
-      self._bus = bus
-
-    self._buf = bytearray(4)
-
-    # Reset
-    self._write_i2c(0x00, [0x00])
-    sleep(0.01)
-
-    # Sleep & restart, also setting the frequency to 1526Hz
-    self._write_i2c(0x00, [0x10])
-    prescale = int(25E6 / 4096.0 / 1600.0 + 0.5)
-    self._write_i2c(0xFE, [prescale])
-    sleep(0.01)
-    self._write_i2c(0x00, [0x00])
-    sleep(0.01)
-    self._write_i2c(0x00, [0xA0])
-
-    # Initializing the motors
-    for i in motor_nrs:
-      self._write_i2c(motor_hat_ctrl[i], motor_hat_0xFF)
-
-  def set_motor(self, nr: int, cmd: float) -> None:
-    """Sets the PWMs associated with a given motor.
+               i2c_port: int = 1) -> None:
+    """Checks the validity of the arguments.
 
     Args:
-      nr: The index of the motor to drive.
-      cmd: The command as a :obj:`float`, that should be between -1 and 1.
-    """
-
-    # Validity checks
-    if nr not in range(1, 5):
-      raise ValueError("It is only possible to drive up to 4 motors.")
-    if not -1.0 <= cmd <= 1.0:
-      raise ValueError("The command for the motor should be between -1 and 1.")
-
-    # Special settings for the extreme values
-    if cmd == 0:
-      self._write_i2c(motor_hat_pos[nr], motor_hat_0xFF)
-      self._write_i2c(motor_hat_neg[nr], motor_hat_0xFF)
-    elif cmd == 1.0:
-      self._write_i2c(motor_hat_pos[nr], motor_hat_0xFF)
-      self._write_i2c(motor_hat_neg[nr], [0x00 for _ in range(4)])
-    elif cmd == -1.0:
-      self._write_i2c(motor_hat_pos[nr], [0x00 for _ in range(4)])
-      self._write_i2c(motor_hat_neg[nr], motor_hat_0xFF)
-
-    # The positive line is driven for positive commands, and reversely
-    elif cmd > 0:
-      duty_cycle = (int(0xFFFF * cmd) + 1) >> 4
-      pack_into("<HH", self._buf, 0, *(0, duty_cycle))
-      self._write_i2c(motor_hat_pos[nr], self._buf)
-      self._write_i2c(motor_hat_neg[nr], [0x00 for _ in range(4)])
-    else:
-      duty_cycle = (int(0xFFFF * abs(cmd)) + 1) >> 4
-      pack_into("<HH", self._buf, 0, *(0, duty_cycle))
-      self._write_i2c(motor_hat_pos[nr], [0x00 for _ in range(4)])
-      self._write_i2c(motor_hat_neg[nr], self._buf)
-
-  def close(self) -> None:
-    """Closes the I2C bus."""
+      backend: Should be one of :
+        ::
 
-    self._bus.close()
+          'Pi4', 'blinka'
 
-  def _write_i2c(self, register: int, buf: Union[list, bytearray]) -> None:
-    """Thin wrapper to reduce verbosity."""
-
-    self._bus.write_i2c_block_data(self._address, register, list(buf))
-
-
-class MotorKitPumpFT232H(Actuator):
-  """Class for controlling two DC air pumps and a valve.
-
-  It uses Adafruit's DC motor HAT. The motor 1 controls the inflation pump,
-  the motor 2 controls a valve, and the motor 3 controls a deflation pump.
-  """
-
-  ft232h = True
-
-  def __init__(self,
-               device_address: int = 0x60,
-               i2c_port: int = 1,
-               _ft232h_args: USBArgsType = tuple()) -> None:
-    """Checks the validity of the arguments.
-
-    Args:
+        The `'Pi4'` backend is optimized but only works on boards supporting
+        the :mod:`smbus2` module, like the Raspberry Pis. The `'blinka'`
+        backend may be less performant and requires installing
+        :mod:`adafruit-circuitpython-motorkit` and :mod:`Adafruit-Blinka`, but
+        these modules are compatible with and maintained on a wide variety of
+        boards.
       device_address: The I2C address of the HAT. The default address is
         `0x60`, but it is possible to change this setting by cutting traces on
         the board.
       i2c_port: The I2C port over which the HAT should communicate. On most
         Raspberry Pi models the default I2C port is `1`.
     """
 
-    self._hat = None
-
-    super().__init__()
+    self._bus = None
+    self._buf = bytearray(4)
 
-    (block_index, block_lock, command_file, answer_file, shared_lock,
-     current_block) = _ft232h_args
+    if not isinstance(backend, str) or backend not in motor_hat_backends:
+      raise ValueError("backend should be in {}".format(motor_hat_backends))
+    self._backend = backend
 
-    self._bus = FT232H(mode='I2C',
-                       block_index=block_index,
-                       current_block=current_block,
-                       command_file=command_file,
-                       answer_file=answer_file,
-                       block_lock=block_lock,
-                       shared_lock=shared_lock)
+    super().__init__()
 
     if not isinstance(device_address, int):
       raise TypeError("device_address should be an integer between 0 and 127.")
     self._address = device_address
 
     if not isinstance(i2c_port, int):
       raise TypeError("i2c_port should be an integer !")
     self._port = i2c_port
 
   def open(self) -> None:
-    """Initializes the generic HAT object."""
-
-    self.log(logging.INFO, "Opening the Motorkit with an USB connection "
-                           "over FT232H")
-    self._hat = DCMotorHat([1, 2, 3], self._address, self._port, self._bus)
+    """Opens the connection to the motor hat and initializes it."""
 
-  def set_speed(self, volt: float) -> None:
-    """Inflates or deflates the setup according to the command.
+    if self._backend == 'blinka':
+      self.log(logging.INFO, "Opening with the Adafruit library")
+      self._bus = MotorKit(i2c=board.I2C())
+
+    elif self._backend == 'Pi4':
+      self.log(logging.INFO, "Opening with the SMBus library")
+
+      self._bus = SMBus(self._port)
+
+      # Reset
+      self._write_i2c(0x00, [0x00])
+      sleep(0.01)
+
+      # Sleep & restart, also setting the frequency to 1526Hz
+      self._write_i2c(0x00, [0x10])
+      self._write_i2c(0xFE, [int(25E6 / 4096.0 / 1600.0 + 0.5)])
+      sleep(0.01)
+      self._write_i2c(0x00, [0x00])
+      sleep(0.01)
+      self._write_i2c(0x00, [0xA0])
+
+      # Initializing the motors
+      for i in range(1, 5):
+        self._write_i2c(motor_hat_ctrl[i], motor_hat_0xFF)
+
+  def set_speed(self, cmd: Tuple[int, float]) -> None:
+    """Sets the desired voltage on the selected motor.
+
+    The provided voltage should be between `-12` and `12V` which are the limits
+    of the motor hat. If not, it will be silently clamped in this interval.
+
+    Warning:
+      Unlike most Actuators, this one takes :obj:`tuple` as commands instead
+      of :obj:`float`.
 
     Args:
-      volt: The voltage to supply to the pumps. If positive, will inflate, if
-        negative will deflate, and if `0` won't do anything. The voltage is
-        clamped between `-12` and `12` Volts, as it is the limit of the HAT.
+      cmd: A :obj:`tuple` containing first the index of the motor to drive as
+        an :obj:`int` between 1 and 5, and second the voltage to apply to the
+        selected motor as a :obj:`float`.
     """
 
-    volt_clamped = min(abs(volt) / motor_hat_max_volt, 1.0)
-
-    # Stops all the motors
-    if volt == 0:
-      self.log(logging.DEBUG, "Setting motor 1 to 0.0")
-      self._hat.set_motor(1, 0.0)
-      self.log(logging.DEBUG, "Setting motor 2 to 0.0")
-      self._hat.set_motor(2, 0.0)
-      self.log(logging.DEBUG, "Setting motor 3 to 0.0")
-      self._hat.set_motor(3, 0.0)
-
-    # Drives the inflating pump
-    elif volt > 0:
-      self.log(logging.DEBUG, f"Setting motor 1 to {volt_clamped}")
-      self._hat.set_motor(1, volt_clamped)
-      self.log(logging.DEBUG, "Setting motor 2 to 0.0")
-      self._hat.set_motor(2, 0.0)
-      self.log(logging.DEBUG, "Setting motor 3 to 0.0")
-      self._hat.set_motor(3, 0.0)
-
-    # Drives the deflating pump and opens the valve
-    elif volt < 0:
-      self.log(logging.DEBUG, "Setting motor 1 to 0.0")
-      self._hat.set_motor(1, 0.0)
-      self.log(logging.DEBUG, "Setting motor 2 to 1.0")
-      self._hat.set_motor(2, 1.0)
-      self.log(logging.DEBUG, f"Setting motor 3 to {volt_clamped}")
-      self._hat.set_motor(3, volt_clamped)
+    try:
+      motor_nr, volts = cmd
+    except (TypeError, ValueError):
+      raise ValueError("The DCMotorHat receives commands as tuples, with first"
+                       " the index of the motor and second the voltage "
+                       "command")
+
+    if motor_nr not in range(1, 5):
+      raise ValueError("The index of the motor to drive should be an integer "
+                       "between 1 and 5")
+
+    volt_clamped = min(abs(volts) / motor_hat_max_volt, 1.0)
+    self.log(logging.DEBUG, f"Setting motor {motor_nr} to {volt_clamped}V")
+    self._set_motor(motor_nr, volt_clamped)
 
   def stop(self) -> None:
-    """"""
+    """Simply sets the command to `0` to stop the motors."""
 
-    if self._hat is not None:
-      self.set_speed(0)
+    if self._bus is not None:
+      for i in range(1, 5):
+        self.set_speed((i, 0))
 
   def close(self) -> None:
-    """Stops the pumps and closes the HAT object."""
+    """Closes the I2C connection to the motor hat."""
 
-    if self._hat is not None:
-      self.log(logging.INFO, "Closing the connection to the Motorkit")
-      self._hat.close()
+    if self._bus is not None and self._backend == 'Pi4':
+      self.log(logging.INFO, "Closing the connection to the Motor Hat")
+      self._bus.close()
+
+  def _set_motor(self, nr: int, cmd: float) -> None:
+    """Sets the PWMs associated with a given motor.
+
+    Args:
+      nr: The index of the motor to drive.
+      cmd: The command as a :obj:`float`, that should be between -1 and 1.
+    """
+
+    if self._backend == 'Pi4':
+
+      # Special settings for the extreme values
+      if cmd == 0:
+        self._write_i2c(motor_hat_pos[nr], motor_hat_0xFF)
+        self._write_i2c(motor_hat_neg[nr], motor_hat_0xFF)
+      elif cmd == 1.0:
+        self._write_i2c(motor_hat_pos[nr], motor_hat_0xFF)
+        self._write_i2c(motor_hat_neg[nr], [0x00 for _ in range(4)])
+      elif cmd == -1.0:
+        self._write_i2c(motor_hat_pos[nr], [0x00 for _ in range(4)])
+        self._write_i2c(motor_hat_neg[nr], motor_hat_0xFF)
+
+      # The positive line is driven for positive commands, and reversely
+      elif cmd > 0:
+        duty_cycle = (int(0xFFFF * cmd) + 1) >> 4
+        pack_into("<HH", self._buf, 0, *(0, duty_cycle))
+        self._write_i2c(motor_hat_pos[nr], self._buf)
+        self._write_i2c(motor_hat_neg[nr], [0x00 for _ in range(4)])
+      else:
+        duty_cycle = (int(0xFFFF * abs(cmd)) + 1) >> 4
+        pack_into("<HH", self._buf, 0, *(0, duty_cycle))
+        self._write_i2c(motor_hat_pos[nr], [0x00 for _ in range(4)])
+        self._write_i2c(motor_hat_neg[nr], self._buf)
+
+    # Blinka handles all the job internally
+    elif self._backend == 'blinka':
+      setattr(getattr(self._bus, f'motor{nr}'), 'throttle', cmd)
+
+  def _write_i2c(self, register: int, buf: Union[list, bytearray]) -> None:
+    """Thin wrapper to reduce verbosity."""
+
+    self._bus.write_i2c_block_data(self._address, register, list(buf))
```

### Comparing `crappy-2.0.0.dev1/src/crappy/actuator/meta_actuator/meta_actuator.py` & `crappy-2.0.0.dev2/src/crappy/actuator/meta_actuator/meta_actuator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 from ..._global import DefinitionError
 
 
 class MetaActuator(type):
-  """Metaclass ensuring that two Actuators don't have the same name, and that
-  all Actuators define the required methods. Also keeps track of all the
-  Actuator classes, including the custom user-defined ones."""
+  """Metaclass ensuring that two Actuators don't have the same name, and
+  keeping track of all the :class:`~crappy.actuator.Actuator` classes. It also
+  allows including the user-defined Actuators."""
 
   classes = {}
 
   def __new__(mcs, name: str, bases: tuple, dct: dict) -> type:
     return super().__new__(mcs, name, bases, dct)
 
   def __init__(cls, name: str, bases: tuple, dct: dict) -> None:
```

### Comparing `crappy-2.0.0.dev1/src/crappy/actuator/motor_kit_pump.py` & `crappy-2.0.0.dev2/src/crappy/blocks/canvas.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,272 +1,253 @@
 # coding: utf-8
 
-from struct import pack_into
-from time import sleep
-from typing import Union, List
+from __future__ import annotations
+from datetime import timedelta
+from time import time
+from typing import Tuple, Dict, Any, Optional, Iterable
 import logging
 
-from .meta_actuator import Actuator
+from .meta_block import Block
 from .._global import OptionalModule
 
-try:
-  from adafruit_motorkit import MotorKit
-except (ImportError, ModuleNotFoundError):
-  MotorKit = OptionalModule('adafruit_motorkit',
-                            'Adafrfuit Motorkit module (adafruit_motorkit) is '
-                            'required to use this actuator')
-
-try:
-  import board
-except (ImportError, ModuleNotFoundError):
-  board = OptionalModule('board', 'Blinka is necessary to use the I2C bus')
-
-try:
-  from smbus2 import SMBus
-except (ImportError, ModuleNotFoundError):
-  SMBus = OptionalModule('smbus2')
-
-motor_hat_ctrl = {1: 0x26,
-                  2: 0x3A,
-                  3: 0x0E,
-                  4: 0x22}
-
-motor_hat_pos = {1: 0x2A,
-                 2: 0x32,
-                 3: 0x12,
-                 4: 0x1A}
-
-motor_hat_neg = {1: 0x2E,
-                 2: 0x36,
-                 3: 0x16,
-                 4: 0x1E}
-
-motor_hat_0xFF = [0x00, 0x10, 0x00, 0x00]
-motor_hat_backends = ['Pi4', 'blinka']
-motor_hat_max_volt = 12
-
-
-class DCMotorHat:
-  """Class for driving Adafruit's DC motor HAT.
-
-  This class serves as a basis for building Actuators in Crappy, but is not one
-  itself. It is used by the :class:`Motorkit_pump` Actuator.
-
-  Note:
-    This device can also drive stepper motors, but this feature isn't included
-    here.
+plt = OptionalModule('matplotlib.pyplot', lazy_import=True)
+mpl = OptionalModule('matplotlib', lazy_import=True)
 
-  It is intended for Raspberry Pis but can also be used from any other device
-  interfacing over I2C assuming a proper wiring.
-  """
+
+class Text:
+  """Displays a simple text line on the drawing."""
 
   def __init__(self,
-               motor_nrs: List[int],
-               device_address: int = 0x60,
-               i2c_port: int = 1) -> None:
-    """Resets the HAT and initializes it.
+               _: Canvas,
+               coord: Tuple[int, int],
+               text: str,
+               label: str,
+               **__: str) -> None:
+    """Sets the arguments.
 
     Args:
-      motor_nrs: The list of the motors to drive. Its elements should be
-        integers between 1 and 4, corresponding to the indexes of the motors to
-        drive.
-      device_address: The I2C address of the HAT. The default address is
-        `0x60`, but it is possible to change this setting by cutting traces on
-        the board.
-      i2c_port: The I2C port over which the HAT should communicate. On most
-        Raspberry Pi models the default I2C port is `1`.
+      _: The parent drawing Block.
+      coord: The coordinates of the text on the drawing.
+      text: The text to display.
+      label: The label carrying the information for updating the text.
+      **__: Other unused arguments.
     """
 
-    if not all(i in range(1, 5) for i in motor_nrs):
-      raise ValueError("The DC motor hat can only drive up to 4 DC motors at "
-                       "a time !")
-
-    if not isinstance(device_address, int):
-      raise TypeError("device_address should be an integer between 0 and 127.")
-    self._address = device_address
-
-    if not isinstance(i2c_port, int):
-      raise TypeError("i2c_port should be an integer !")
-
-    self._bus = SMBus(i2c_port)
-    self._buf = bytearray(4)
-
-    # Reset
-    self._write_i2c(0x00, [0x00])
-    sleep(0.01)
-
-    # Sleep & restart, also setting the frequency to 1526Hz
-    self._write_i2c(0x00, [0x10])
-    prescale = int(25E6 / 4096.0 / 1600.0 + 0.5)
-    self._write_i2c(0xFE, [prescale])
-    sleep(0.01)
-    self._write_i2c(0x00, [0x00])
-    sleep(0.01)
-    self._write_i2c(0x00, [0xA0])
-
-    # Initializing the motors
-    for i in motor_nrs:
-      self._write_i2c(motor_hat_ctrl[i], motor_hat_0xFF)
+    x, y = coord
+    self._text = text
+    self._label = label
+
+    self._txt = plt.text(x, y, text)
+
+  def update(self, data: Dict[str, float]) -> None:
+    """Updates the text according to the received values."""
+
+    if self._label in data:
+      self._txt.set_text(self._text % data[self._label])
+
 
-  def set_motor(self, nr: int, cmd: float) -> None:
-    """Sets the PWMs associated with a given motor.
+class DotText:
+  """Like :class:`Text`, but with a colored dot to visualize a numerical value.
+  """
+
+  def __init__(self,
+               drawing: Canvas,
+               coord: Tuple[int, int],
+               text: str,
+               label: str,
+               **__: str) -> None:
+    """Sets the arguments.
 
     Args:
-      nr: The index of the motor to drive.
-      cmd: The command as a :obj:`float`, that should be between -1 and 1.
+      drawing: The parent drawing Block.
+      coord: The coordinates of the text and the color dot on the drawing.
+      text: The text to display.
+      label: The label carrying the information for updating the text and the
+        color of the dot.
+      **__: Other unused arguments.
+
+    Important:
+      The value received in label must be a numeric value. It will be
+      normalized on the ``crange`` of the Block and the dot will change
+      color from blue to red depending on this value.
     """
 
-    # Validity checks
-    if nr not in range(1, 5):
-      raise ValueError("It is only possible to drive up to 4 motors.")
-    if not -1.0 <= cmd <= 1.0:
-      raise ValueError("The command for the motor should be between -1 and 1.")
-
-    # Special settings for the extreme values
-    if cmd == 0:
-      self._write_i2c(motor_hat_pos[nr], motor_hat_0xFF)
-      self._write_i2c(motor_hat_neg[nr], motor_hat_0xFF)
-    elif cmd == 1.0:
-      self._write_i2c(motor_hat_pos[nr], motor_hat_0xFF)
-      self._write_i2c(motor_hat_neg[nr], [0x00 for _ in range(4)])
-    elif cmd == -1.0:
-      self._write_i2c(motor_hat_pos[nr], [0x00 for _ in range(4)])
-      self._write_i2c(motor_hat_neg[nr], motor_hat_0xFF)
-
-    # The positive line is driven for positive commands, and reversely
-    elif cmd > 0:
-      duty_cycle = (int(0xFFFF * cmd) + 1) >> 4
-      pack_into("<HH", self._buf, 0, *(0, duty_cycle))
-      self._write_i2c(motor_hat_pos[nr], self._buf)
-      self._write_i2c(motor_hat_neg[nr], [0x00 for _ in range(4)])
-    else:
-      duty_cycle = (int(0xFFFF * abs(cmd)) + 1) >> 4
-      pack_into("<HH", self._buf, 0, *(0, duty_cycle))
-      self._write_i2c(motor_hat_pos[nr], [0x00 for _ in range(4)])
-      self._write_i2c(motor_hat_neg[nr], self._buf)
-
-  def close(self) -> None:
-    """Closes the I2C bus."""
-
-    self._bus.close()
-
-  def _write_i2c(self, register: int, buf: Union[list, bytearray]) -> None:
-    """Thin wrapper to reduce verbosity."""
+    x, y = coord
+    self._text = text
+    self._label = label
 
-    self._bus.write_i2c_block_data(self._address, register, list(buf))
+    self._txt = plt.text(x + 40, y + 20, text, size=16)
+    self._dot = plt.Circle(coord, 20)
 
+    drawing.ax.add_artist(self._dot)
+    low, high = drawing.color_range
 
-class MotorKitPump(Actuator):
-  """Class for controlling two DC air pumps and a valve.
+    self._amp = high - low
+    self._low = low
 
-  It uses Adafruit's DC motor HAT. The motor 1 controls the inflation pump,
-  the motor 2 controls a valve, and the motor 3 controls a deflation pump.
-  """
+  def update(self, data: Dict[str, float]) -> None:
+    """Updates the text and the color dot according to the received values."""
 
-  def __init__(self,
-               backend: str,
-               device_address: int = 0x60,
-               i2c_port: int = 1) -> None:
-    """Checks the validity of the arguments.
+    if self._label in data:
+      self._txt.set_text(self._text % data[self._label])
+      self._dot.set_color(mpl.cm.coolwarm((data[self._label] -
+                                           self._low) / self._amp))
 
-    Args:
-      backend: Should be one of :
-        ::
 
-          'Pi4', 'blinka', 'ft232h'
+class Time:
+  """Displays a time counter on the drawing, starting at the beginning of the
+  test."""
 
-        The `'Pi4'` backend is optimized but only works on boards supporting
-        the :mod:`smbus2` module, like the Raspberry Pis. The `'blinka'`
-        backend may be less performant and requires installing Adafruit's
-        modules, but these modules are compatible with and maintained on a wide
-        variety of boards. The `'ft232h'` backend allows controlling the hat
-        from a PC using Adafruit's FT232H USB to I2C adapter. See
-        :ref:`Crappy for embedded hardware` for details.
-      device_address: The I2C address of the HAT. The default address is
-        `0x60`, but it is possible to change this setting by cutting traces on
-        the board.
-      i2c_port: The I2C port over which the HAT should communicate. On most
-        Raspberry Pi models the default I2C port is `1`.
-    """
+  def __init__(self, drawing: Canvas, coord: Tuple[int, int], **__) -> None:
+    """Sets the arguments.
 
-    self._hat = None
+    Args:
+      drawing: The parent drawing Block.
+      coord: The coordinates of the time counter on the drawing.
+      **__: Other unused arguments.
+    """
 
-    if not isinstance(backend, str) or backend not in motor_hat_backends:
-      raise ValueError("backend should be in {}".format(motor_hat_backends))
-    self._backend = backend
+    self._block = drawing
+    x, y = coord
 
-    super().__init__()
+    self._txt = plt.text(x, y, "00:00", size=38)
 
-    if not isinstance(device_address, int):
-      raise TypeError("device_address should be an integer between 0 and 127.")
-    self._address = device_address
+  def update(self, _: Dict[str, float]) -> None:
+    """Updates the time counter, independently of the received values."""
 
-    if not isinstance(i2c_port, int):
-      raise TypeError("i2c_port should be an integer !")
-    self._port = i2c_port
+    self._txt.set_text(str(timedelta(seconds=int(time() - self._block.t0))))
 
-  def open(self) -> None:
-    """Initializes the generic HAT object."""
 
-    if self._backend == 'blinka':
-      self.log(logging.INFO, "Opening the Motorkit with the Adafruit library")
-      self._hat = MotorKit(i2c=board.I2C())
+class Canvas(Block):
+  """This Block allows displaying a real-time visual representation of data.
 
-      def set_motor(nr: int, cmd: float) -> None:
-        setattr(getattr(self._hat, f'motor{nr}'), 'throttle', cmd)
+  It displays the data on top of a background image and updates it according to
+  the values received through the incoming :class:`~crappy.links.Link`. The
+  background image and the data overlay are displayed in a new window.
 
-      self._hat.set_motor = set_motor
+  It is possible to display a simple text, a time counter, or text associated
+  with a color dot evolving depending on a predefined color bar and the
+  received values.
 
-    else:
-      self.log(logging.INFO, "Opening the Motorkit with the SMBus library")
-      self._hat = DCMotorHat([1, 2, 3], self._address, self._port)
+  This Block is mostly useful for displaying a user-friendly and fine-tuned
+  representation of data. For simpler displays, the
+  :class:`~crappy.blocks.Dashboard`, :class:`~crappy.blocks.Grapher` and
+  :class:`~crappy.blocks.LinkReader` Blocks should be preferred.
+  """
 
-  def set_speed(self, volt: float) -> None:
-    """Inflates or deflates the setup according to the command.
+  def __init__(self,
+               image_path: str,
+               draw: Optional[Iterable[Dict[str, Any]]] = None,
+               color_range: Tuple[float, float] = (20, 300),
+               title: str = "Canvas",
+               window_size: Tuple[int, int] = (7, 5),
+               backend: str = "TkAgg",
+               freq: Optional[float] = 2,
+               display_freq: bool = False,
+               debug: Optional[bool] = False) -> None:
+    """Sets the arguments and initializes the parent class.
 
     Args:
-      volt: The voltage to supply to the pumps. If positive, will inflate, if
-        negative will deflate, and if `0` won't do anything. The voltage is
-        clamped between `-12` and `12` Volts, as it is the limit of the HAT.
+      image_path: Path to the image that will be the background of the canvas,
+        as a :obj:`str`.
+      draw: An iterable (like a :obj:`list` or a :obj:`tuple`) of :obj:`dict`
+        defining what to draw. See below for more details.
+      color_range: A :obj:`tuple` containing the lowest and highest values for
+        the color bar.
+      title: The title of the window containing the drawing.
+      window_size: The `x` and `y` dimension of the window, following
+        :mod:`matplotlib` nomenclature.
+      backend: The :mod:`matplotlib` backend to use.
+      freq: The target looping frequency for the Block. If :obj:`None`, loops
+        as fast as possible.
+      display_freq: If :obj:`True`, displays the looping frequency of the
+        Block.
+      debug: If :obj:`True`, displays all the log messages including the
+        :obj:`~logging.DEBUG` ones. If :obj:`False`, only displays the log
+        messages with :obj:`~logging.INFO` level or higher. If :obj:`None`,
+        disables logging for this Block.
+
+    Note:
+      - Information about the ``draw`` keys:
+
+        - ``type``: Mandatory, the type of drawing to display. It can be either
+          `'text'`, `'dot_text'` or `'time'`.
+
+        - ``coord``: Mandatory, a :obj:`tuple` containing the `x` and `y`
+          coordinates where the element should be displayed on the drawing.
+
+        - ``text``: Mandatory for `'text'` and `'dot_text'` only, the text to
+          display on the drawing. It must follow the %-formatting, and contain
+          exactly one %-field. Ex: `'T0 = %f'`. This field will be updated
+          using the value carried by ``label``.
+
+        - ``label``: Mandatory for `'text'` and `'dot_text'` only, the label of
+          the data to display. It will try to retrieve this data in the
+          incoming Links. The ``text`` will then be updated with this data.
     """
 
-    volt_clamped = min(abs(volt) / motor_hat_max_volt, 1.0)
+    super().__init__()
+    self.freq = freq
+    self.display_freq = display_freq
+    self.debug = debug
+
+    self._image = image_path
+    self._draw = [] if draw is None else list(draw)
+    self.color_range = color_range
+    self._title = title
+    self._window_size = window_size
+    self._backend = backend
+
+    self._fig = None
+    self.ax = None
+    self._drawing_elements = None
+
+  def prepare(self) -> None:
+    """Initializes the different elements of the drawing."""
+
+    self.log(logging.INFO, "Opening the drawing windows")
+
+    # Initializing the window and the background image
+    plt.switch_backend(self._backend)
+    self._fig, self.ax = plt.subplots(figsize=self._window_size)
+    image = self.ax.imshow(plt.imread(self._image), cmap=mpl.cm.coolwarm)
+    image.set_clim(-0.5, 1)
+
+    # Initializing the color bar
+    cbar = self._fig.colorbar(image, ticks=[-0.5, 1], fraction=0.061,
+                              orientation='horizontal', pad=0.04)
+    cbar.set_label('Temperatures(C)')
+    cbar.ax.set_xticklabels(self.color_range)
+
+    # Setting the title and the axes
+    self.ax.set_title(self._title)
+    self.ax.set_axis_off()
+
+    # Adding the elements to the drawing
+    self._drawing_elements = []
+    for dic in self._draw:
+      if dic['type'] == 'text':
+        self._drawing_elements.append(Text(self, **dic))
+      elif dic['type'] == 'dot_text':
+        self._drawing_elements.append(DotText(self, **dic))
+      elif dic['type'] == 'time':
+        self._drawing_elements.append(Time(self, **dic))
+
+  def loop(self) -> None:
+    """Receives the latest data from upstream Blocks and updates the drawing
+    accordingly."""
+
+    data = self.recv_last_data(fill_missing=False)
+    if not data:
+      return
+
+    for elt in self._drawing_elements:
+      elt.update(data)
+    self.log(logging.DEBUG, "Updating the drawing window")
+    self._fig.canvas.draw()
+    plt.pause(0.001)
+
+  def finish(self) -> None:
+    """Closes the window containing the drawing."""
 
-    # Stops all the motors
-    if volt == 0:
-      self.log(logging.DEBUG, "Setting motor 1 to 0.0")
-      self._hat.set_motor(1, 0.0)
-      self.log(logging.DEBUG, "Setting motor 2 to 0.0")
-      self._hat.set_motor(2, 0.0)
-      self.log(logging.DEBUG, "Setting motor 3 to 0.0")
-      self._hat.set_motor(3, 0.0)
-
-    # Drives the inflating pump
-    elif volt > 0:
-      self.log(logging.DEBUG, f"Setting motor 1 to {volt_clamped}")
-      self._hat.set_motor(1, volt_clamped)
-      self.log(logging.DEBUG, "Setting motor 2 to 0.0")
-      self._hat.set_motor(2, 0.0)
-      self.log(logging.DEBUG, "Setting motor 3 to 0.0")
-      self._hat.set_motor(3, 0.0)
-
-    # Drives the deflating pump and opens the valve
-    elif volt < 0:
-      self.log(logging.DEBUG, "Setting motor 1 to 0.0")
-      self._hat.set_motor(1, 0.0)
-      self.log(logging.DEBUG, "Setting motor 2 to 1.0")
-      self._hat.set_motor(2, 1.0)
-      self.log(logging.DEBUG, f"Setting motor 3 to {volt_clamped}")
-      self._hat.set_motor(3, volt_clamped)
-
-  def stop(self) -> None:
-    """"""
-
-    if self._hat is not None:
-      self.set_speed(0)
-
-  def close(self) -> None:
-    """Stops the pumps and closes the HAT object."""
-
-    if self._hat is not None and self._backend == 'Pi4':
-      self.log(logging.INFO, "Closing the connection to the Motorkit")
-      self._hat.close()
+    self.log(logging.INFO, "Closing the drawing windows")
+    plt.close()
```

### Comparing `crappy-2.0.0.dev1/src/crappy/actuator/oriental.py` & `crappy-2.0.0.dev2/src/crappy/actuator/oriental_ard_k.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # coding: utf-8
 
 from typing import Optional
 import logging
+
 from .meta_actuator import Actuator
 from .._global import OptionalModule
 
 try:
   from serial import Serial
 except (ModuleNotFoundError, ImportError):
   Serial = OptionalModule("pyserial")
 
 
-class Oriental(Actuator):
-  """This class can drive an Oriental Motor's ARD-K stepper motor in speed or
-  in position.
+class OrientalARDK(Actuator):
+  """This class can drive an Oriental Motor's ARD-K stepper motor driver in
+  speed or in position.
 
   It communicates with the stepper motor over a serial connection. This class
-  was designed so that the :ref:`Machine` block drives several of its instances
-  at a time, corresponding to different axes to drive.
+  was designed so that the :class:`~crappy.blocks.Machine` Block drives several
+  of its instances at a time, corresponding to different axes to drive.
   """
 
   def __init__(self,
                baudrate: int = 115200,
                port: str = '/dev/ttyUSB0',
                gain: float = 1/.07) -> None:
     """Sets the instance attributes and initializes the parent class.
 
     Args:
-      baudrate: the baudrate to use for serial communication.
+      baudrate: The baudrate to use for the serial communication.
       port: The path to the serial port to use for communication.
       gain: The gain to apply to speed commands, in `mm/min`. The default value
         corresponds to `0.07mm/min` for a command value of `1`.
     """
 
     self._ser = None
 
@@ -116,27 +117,25 @@
     else:
       self.log(logging.DEBUG, f"Writing b'MCN\\n' to port {self._port}")
       self._ser.write(b"MCN\n")
 
     # Storing the written value
     self._prev_set_speed = signed_speed
 
-  def set_position(self,
-                   position: float,
-                   speed: Optional[float] = None) -> None:
+  def set_position(self, position: float, speed: Optional[float]) -> None:
     """Sets the target position for the motor.
 
     Args:
       position: The target position to reach, in arbitrary units.
-      speed: The speed to use for reching the target position, in arbitrary
-        units.
+      speed: The speed to use for reaching the target position, in arbitrary
+        units. A speed must be given, otherwise an exception is raised.
     """
 
     if speed is None:
-      raise ValueError("The Oriental actuator needs both a position and a "
+      raise ValueError("The OrientalARDK actuator needs both a position and a "
                        "speed command when driven in position mode !")
 
     self.log(logging.DEBUG, f"Writing b'VR {abs(speed)}' to port {self._port}")
     self._ser.write(f'VR {abs(speed)}'.encode())
     self.log(logging.DEBUG, f"Writing b'MA {position}' to port {self._port}")
     self._ser.write(f'MA {position}'.encode())
 
@@ -161,18 +160,18 @@
     """Sends a command for stopping the motor."""
 
     if self._ser is not None:
       self.log(logging.DEBUG, f"Writing b'SSTOP\\n' to port {self._port}")
       self._ser.write(b"SSTOP\n")
 
   def close(self) -> None:
-    """Closes the serial connection to the actuator."""
+    """Closes the serial connection to the motor."""
 
     if self._ser is not None:
       self.log(logging.INFO, f"Closing the serial port {self._port}")
       self._ser.close()
 
   def _clear_errors(self) -> None:
-    """Sends a command for clearing any serial error on the actuator."""
+    """Sends a command for clearing any serial error from the motor."""
 
     self.log(logging.DEBUG, f"Writing b'ALMCLR\\n' to port {self._port}")
     self._ser.write(b"ALMCLR\n")
```

### Comparing `crappy-2.0.0.dev1/src/crappy/actuator/pololu_tic.py` & `crappy-2.0.0.dev2/src/crappy/actuator/pololu_tic.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
   def __call__(self, device) -> bool:
     return device.serial_number == self.serial_number
 
 
 class PololuTic(Actuator):
   """Class for controlling Pololu's Tic stepper motor divers.
 
-  The Pololu_tic Actuator block is meant for controlling a Pololu Tic stepper
+  The PololuTic Actuator block is meant for controlling a Pololu Tic stepper
   motor driver. It can be driven in both speed and position. Several Tic models
   are supported. The length unit is the millimeter (`mm`), and time unit is the
   second (`s`).
 
   Important:
     **Only for Linux users:** In order to drive the Tic, the appropriate udev
     rule should be set. This is done automatically when installing `ticcmd`,
@@ -296,28 +296,27 @@
         It is usually around `1A` for small stepper motors, and can go up to a
         few Amps. The maximum allowed ``current_limit`` value depends on the
         Tic model. The Tic 36v4 default maximum current limit can be increased
         using the ``unrestricted_current_limit`` parameter.
       step_mode: Sets the number of microsteps used for driving the motor. This
         number is always a power of `2`. The minimum number of microsteps is
         `1` (full steps), and the maximum depends on the Tic model. All models
-        however support modes `1` to `8`. The block manages speed and length
-        conversions so that changing the step mode doesn't affect the motor
-        behaviour.
+        however support modes `1` to `8`. The speed and length conversions are
+        managed automatically so that changing the step mode doesn't affect the
+        motor behaviour.
       max_accel: The maximum allowed acceleration for the motor, in `mm/s²`.
         When asked to reach a given speed or position, the motor accelerates at
         this rate. It also corresponds to the maximum allowed deceleration.
         Usually doesn't need to be changed.
-      t_shutoff: The :class:`Pololu_tic` class features an auto-shutoff thread
-        that deenergizes the motor after a period of `t_shutoff` seconds of
-        inactivity. The timer counts in steps of `0.1s`, which is thus the
-        maximum precision for this setting. When set to `0`, this feature is
-        disabled and the motor remains energized until the :meth:`close` method
-        is called.
-      config_file: The path of the config file to be loaded to the Tic. It only
+      t_shutoff: This class features an auto-shutoff thread that deenergizes
+        the motor after a period of `t_shutoff` seconds of inactivity. The
+        timer counts in steps of `0.1s`, which is thus the maximum precision
+        for this setting. When set to `0`, this feature is disabled and the
+        motor remains energized until the :meth:`close` method is called.
+      config_file: The path to the config file to be loaded to the Tic. It only
         works if ``backend`` is 'ticcmd'. The config file contains some
         specific settings that can only be accessed this way using the 'ticcmd'
         backend. Not necessary for most applications.
       serial_number: The serial number of the Tic to be controlled. It must be
         given as a :obj:`str`, and it is an 8-digits number. Allows to control
         the right device if several Tic of the same model are connected.
         Otherwise, an error is raised.
@@ -329,16 +328,16 @@
         Allows to control the right device if several Tic of different models
         are connected. Otherwise, an error is raised.
       reset_command_timeout: Enables or disables the `reset_command_timeout`
         thread. It can only be disabled if ``backend`` is 'USB'. This thread
         pings the Tic every `0.5s`, so that it doesn't block due to a Command
         Timeout error. This feature is a safety to prevent the motor from
         running indefinitely if the USB connection is down, so it is better not
-        to disable it. When disabled the Tic never raises Command Timeout
-        errors, and a bit of memory if freed because of the thread not running.
+        to disable it. When disabled, the Tic never raises Command Timeout
+        errors.
       backend: The backend for communicating with the Tic. Available backends
         are:
         ::
 
           'USB', 'ticcmd'
 
         They both communicate over USB, but 'ticcmd' requires Pololu's firmware
@@ -403,15 +402,15 @@
       - ``step_mode``:
         Increasing the number of microsteps allows to reduce the noise, the
         vibrations, and improve the precision. However, the more microsteps,
         the lower the maximum achievable speed for the motor. Chances that the
         motor misses microsteps are also higher when the number of microsteps
         is high.
       - ``t_shutoff``:
-        This functionality was originally added for long assays in temperature
+        This functionality was originally added for long tests in temperature
         controlled environments, so that the motor doesn't unnecessarily heat
         the setup when inactive. In other assays, it may still be useful for
         reducing the noise, the electromagnetic interference, or the energy
         consumption.
       - ``serial_number``:
         Serial numbers can be accessed using the `lsusb` command in Linux
         shell, or running ``ticcmd --list`` if `ticcmd` is installed. This
@@ -420,15 +419,15 @@
       - ``model``:
         The model is written on the Tic board, and can be accessed by running
         ``ticcmd --list`` in a shell if `ticcmd` is installed. It is also
         displayed during :meth:`__init__` if only one device is connected and
         ``model`` is :obj:`None`.
       - **Pins settings**:
         The pin functions and polarity can also be set independently of
-        ``crappy`` before starting the assay, in the `ticgui`.
+        ``crappy`` before starting the test, in the `ticgui`.
     """
 
     super().__init__()
 
     if backend not in Tic_backends:
       raise ValueError("backend should be in {}".format(Tic_backends))
     else:
@@ -699,15 +698,15 @@
       self.log(logging.INFO, "Starting the thread managing the auto shutoff")
       self._thrd_shutoff.start()
 
   def get_speed(self) -> float:
     """Reads the current motor speed.
 
         Returns:
-          :obj:`float`: The speed in mm/s
+          The speed in `mm/s`
         """
 
     if self._backend == 'ticcmd':
       return self._to_mm(yaml.load(self._ticcmd('-s'), Loader=yaml.FullLoader)
                          ['Current velocity'] / 10000) if full_loader else \
         self._to_mm(yaml.load(self._ticcmd('-s'))['Current velocity'] / 10000)
     elif self._backend == 'USB':
@@ -719,15 +718,15 @@
         byteorder='little',
         signed=True) / 10000)
 
   def get_position(self) -> float:
     """Reads the current motor position.
 
     Returns:
-      :obj:`float`: The position in mm
+      The position in `mm`
     """
 
     if self._backend == 'ticcmd':
       return self._to_mm(yaml.load(self._ticcmd('-s'), Loader=yaml.FullLoader)
                          ['Current position']) if full_loader else \
         self._to_mm(yaml.load(self._ticcmd('-s'))['Current position'])
     elif self._backend == 'USB':
@@ -735,23 +734,22 @@
         self._usb_command(request_type=Tic_usb_request['Var'],
                           request=Tic_cmd['Get_variable'],
                           index=Tic_var['Current_position'],
                           data_or_length=4),
         byteorder='little',
         signed=True))
 
-  def set_position(self,
-                   position: float,
-                   speed: Optional[float] = None) -> None:
+  def set_position(self, position: float, speed: Optional[float]) -> None:
     """Sends a position command to the motor.
 
     Args:
-      position (:obj:`float`): The position to reach in `mm`
-      speed (:obj:`float`, optional): The speed at which the motor should move
-        to the given position, in `mm/s`
+      position: The position to reach in `mm`
+      speed: The speed at which the motor should move to the given position,
+        in `mm/s` Giving a speed other than :obj:`None` will set the maximum
+        speed of the motor to that speed.
 
     Note:
       - ``speed``:
         The only way to reach a position at a given speed is to change the
         maximum speed. The Tic will try to accelerate to the maximum speed but
         may remain slower if it doesn't have time to do so before reaching the
         given position.
@@ -772,15 +770,15 @@
     # Sending the position command
     self._set_position(position)
 
   def set_speed(self, speed: float) -> None:
     """Sends a speed command to the motor.
 
     Args:
-      speed (:obj:`float`): The speed the motor should reach
+      speed: The speed the motor should reach
     """
 
     # Changing the maximum speed if needed
     max_speed = self._get_max_speed()
     if abs(speed) > max_speed:
       self._set_max_speed(speed)
```

### Comparing `crappy-2.0.0.dev1/src/crappy/actuator/servostar.py` & `crappy-2.0.0.dev2/src/crappy/actuator/kollmorgen_servostar_300.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,31 +8,35 @@
 
 try:
   import serial
 except (ModuleNotFoundError, ImportError):
   serial = OptionalModule("pyserial")
 
 
-class ServoStar(Actuator):
-  """This class can drive Kollmorgen's ServoStar 300 servomotor conditioner in
+class ServoStar300(Actuator):
+  """This class can drive a Kollmorgen ServoStar 300 servomotor conditioner in
   position, and set it to the analog or serial driving mode.
 
-  It communicates with the servomotor over a serial connection.
+  It communicates with the servomotor over a serial connection. The
+  :class:`~crappy.lamcube.Biaxe` Actuator can drive the same hardware, but only
+  in speed.
   """
 
   def __init__(self,
                port: str,
                baudrate: int = 38400,
                mode: str = "serial") -> None:
     """Sets the instance attributes and initializes the parent class.
 
     Args:
-      port (:obj:`str`): Path to connect to the serial port.
-      baudrate (:obj:`int`, optional): Set the corresponding baud rate.
-      mode (:obj:`str`, optional): Can be `'analog'` or `'serial'`.
+      port: Path to the serial port used for communication.
+      baudrate: The serial baud rate to use, as an :obj:`int`.
+      mode: The driving mode to use when starting the test. Can be `'analog'`
+        or `'serial'`. It can be changed afterward while the test is running,
+        by sending the right command.
     """
 
     self._ser = None
 
     super().__init__()
 
     self._port = port
@@ -63,26 +67,27 @@
     self.log(logging.DEBUG, f"Writing b'EN\\r\\n' to port {self._port}")
     self._ser.write('EN\r\n')
     self.log(logging.DEBUG, f"Writing b'MH\\r\\n' to port {self._port}")
     self._ser.write('MH\r\n')
 
   def set_position(self,
                    pos: Union[float, bool],
-                   speed: Optional[float] = None) -> None:
+                   speed: Optional[float]) -> None:
     """Sets the target position for the motor.
 
     Also allows switching to the serial or analog driving mode if the target
     position is a :obj:`bool`. The acceleration and deceleration are set to
     `200`.
 
     Args:
       pos: The target position to reach, as a :obj:`float`. Alternatively, a
         value of :obj:`True` sets the driving mode to serial, and :obj:`False`
         sets the driving mode to analog.
       speed: The speed at which the actuator should reach its target position.
+        If no speed is specified, the default is `20000`.
     """
 
     if speed is None:
       speed = 20000
 
     # Nothing to do if the command is the same as the previous
     if self._last_pos == pos:
```

### Comparing `crappy-2.0.0.dev1/src/crappy/actuator/tra6ppd.py` & `crappy-2.0.0.dev2/src/crappy/actuator/newport_tra6ppd.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,34 +9,34 @@
 
 try:
   from serial import Serial
 except (ModuleNotFoundError, ImportError):
   Serial = OptionalModule('pyserial')
 
 
-class TRA6PPD(Actuator):
-  """Drives the TRA6PPD linear actuator in position.
+class NewportTRA6PPD(Actuator):
+  """Drives the Newport TRA6PPD linear actuator in position.
 
   Warning:
     This actuator cannot handle a high serial messages rate. It is recommended
-    to set the frequency of the corresponding :ref:`Machine` block to a few
-    dozen Hz at most.
+    to set the frequency of the corresponding :class:`~crappy.blocks.Machine`
+    Block to a few dozen `Hz` at most.
 
   Note:
-    This actuator ignores new position commands while it is moving.
+    This Actuator ignores new position commands while it is moving.
   """
 
   def __init__(self,
                baudrate: int = 57600,
                port: str = '/dev/ttyUSB0') -> None:
     """Sets the instance attributes and initializes the parent class.
 
     Args:
       baudrate: The baudrate for the serial connection.
-      port: Path to the port to use for seria lcommunication.
+      port: Path to the port to use for serial communication.
     """
 
     self._ser = None
 
     super().__init__()
 
     self._max_speed = 0.2
@@ -61,25 +61,23 @@
     # Then, perform homing (may take up to 45s)
     self.log(logging.DEBUG, f"Writing b'10R\\r\\n' to port {self._port}")
     self._ser.write(b'1OR\r\n')
     for i in range(5, 0, -1):
       self.log(logging.INFO, f"Performing homing, {10 * i} seconds left")
       sleep(10)
 
-  def set_position(self,
-                   position: float,
-                   speed: Optional[float] = None) -> None:
+  def set_position(self, position: float, speed: Optional[float]) -> None:
     """Sends the actuator a command to reach a given position.
 
     The command is ignored if the actuator is already moving.
 
     Args:
       position: The position to reach. Should be between `0` and `6 mm`.
       speed: The speed at which the actuator should move. Should be between `0`
-        and `0.2 mm/s`.
+        and `0.2 mm/s`. If :obj:`None` is received, the default is `0.2 mm/s`.
     """
 
     if speed is None:
       speed = 0.2
 
     # Clamping the speed command into the allowed interval
     speed_clamped = max(min(self._max_speed, speed), 0)
@@ -112,15 +110,15 @@
 
     # Using a regular expression to parse the answer
     ret = self._ser.readline()
     self.log(logging.DEBUG, f"Read {ret} on port {self._port}")
     return float(findall(r'\d\.\d+', ret.decode())[0])
 
   def close(self) -> None:
-    """Just closes the serial port."""
+    """Closes the serial port."""
 
     if self._ser is not None:
       self.log(logging.INFO, f"Closing the serial port {self._port}")
       self._ser.close()
 
   def stop(self) -> None:
     """Stops the motor and sets the device to "disable" state."""
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/__init__.py` & `crappy-2.0.0.dev2/src/crappy/blocks/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # coding: utf-8
 # Blocks are classes, running indefinitely in a single process.
 # Some of them are already implemented (see the reference manual),
 # but you can also implement your own.
 
-from .auto_drive import AutoDrive
+from .auto_drive_video_extenso import AutoDriveVideoExtenso
 from .meta_block import Block
 from .camera import Camera
 from .client_server import ClientServer
 from .dashboard import Dashboard
 from .dis_correl import DISCorrel
 from .dic_ve import DICVE
-from .drawing import Drawing
+from .canvas import Canvas
 from .fake_machine import FakeMachine
 from .generator import Generator
 from .gpu_correl import GPUCorrel
 from .gpu_ve import GPUVE
 from .grapher import Grapher
-from .gui import GUI
+from .button import Button
 from .hdf_recorder import HDFRecorder
 from .ioblock import IOBlock
 from .machine import Machine
 from .mean import MeanBlock
-from .multiplex import Multiplex
+from .multiplexer import Multiplexer
 from .pid import PID
-from .reader import Reader
+from .link_reader import LinkReader
 from .recorder import Recorder
 from .sink import Sink
 from .ucontroller import UController
 from .video_extenso import VideoExtenso
 
 from . import generator_path
 from . import camera_processes
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/auto_drive.py` & `crappy-2.0.0.dev2/src/crappy/blocks/auto_drive_video_extenso.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,106 +5,113 @@
 import logging
 
 from .meta_block import Block
 from ..actuator import actuator_dict, Actuator
 from ..tool.ft232h import USBServer
 
 
-class AutoDrive(Block):
-  """This block is meant to drive an actuator on which a camera performing
-  videoextensometry is mounted so that the spots stay centered on the image.
-
-  It takes the output of a :ref:`Video Extenso` block and uses the coordinates
-  of the spots to drive the actuator. The actuator can only be driven in speed,
-  not in position.
+class AutoDriveVideoExtenso(Block):
+  """This Block is meant to drive an :class:`~crappy.actuator.Actuator` on 
+  which a :class:`~crappy.camera.Camera` performing video-extensometry is 
+  mounted, so that the spots stay centered on the image.
+
+  It takes the output of a :class:`~crappy.blocks.VideoExtenso` Block and uses 
+  the coordinates of the spots to drive the Actuator. The Actuator can only be 
+  driven in speed, not in position.
 
   It also outputs the difference between the center of the image and the middle
   of the spots, along with a timestamp, over the ``'t(s)'`` and ``'diff(pix)'``
-  labels. It can then be used by downstream blocks.
+  labels. It can then be used by downstream Blocks.
   """
 
   def __init__(self,
-               actuator: Optional[Dict[str, Any]] = None,
+               actuator: Dict[str, Any],
                gain: float = 2000,
                direction: str = 'Y-',
                pixel_range: int = 2048,
                max_speed: float = 200000,
                ft232h_ser_num: Optional[str] = None,
-               freq: float = 200,
+               freq: Optional[float] = 200,
                display_freq: bool = False,
                debug: Optional[bool] = False) -> None:
-    """Sets the args and initializes the parent class.
+    """Sets the arguments and initializes the parent class.
 
     Args:
-      actuator: A :obj:`dict` for initializing the actuator to drive. It
-        should contain the name of the actuator under the key ``'name'``, and
-        all the arguments to pass to the actuator as key/value pairs. The
-        default actuator if this argument is not set is the :ref:`CM Drive`
-        with its default arguments.
-      gain: The gain for driving the actuator in speed. The speed command is
+      actuator: A :obj:`dict` for initializing the 
+        :class:`~crappy.actuator.Actuator` to drive. Refer to the documentation
+        of the :class:`~crappy.blocks.Machine` Block for more information on
+        the mandatory and optional keys.
+      gain: The gain for driving the Actuator in speed. The speed command is
         simply the difference in pixels between the center of the image and the
         center of the spots, multiplied by this gain.
-      direction: Indicates which axis to consider for driving the actuator, and
+      direction: Indicates which axis to consider for driving the Actuator, and
         whether the action should be inverted. The first character is the axis
         (`X` or `Y`) and second character is the inversion (`+` or `-`). The
-        inversion depends on whether a positive speed will make bring the spots
-        closer or farther, you have to try !
+        inversion depends on whether a positive speed will bring the spots
+        closer or farther.
       pixel_range: The size of the image (in pixels) along the chosen axis.
       max_speed: The absolute maximum speed value that can be sent to the
-        actuator.
-      freq: The block will try to loop at this frequency.
+        Actuator.
+      freq: The target looping frequency for the Block. If :obj:`None`, loops
+        as fast as possible.
       display_freq: If :obj:`True`, displays the looping frequency of the
-        block.
+        Block.
+      debug: If :obj:`True`, displays all the log messages including the
+        :obj:`~logging.DEBUG` ones. If :obj:`False`, only displays the log
+        messages with :obj:`~logging.INFO` level or higher. If :obj:`None`,
+        disables logging for this Block.
     """
 
     self._device: Optional[Actuator] = None
     self._ft232h_args = None
 
     super().__init__()
     self.labels = ['t(s)', 'diff(pix)']
     self.freq = freq
     self.display_freq = display_freq
     self.debug = debug
 
-    self._actuator = {'name': 'CM_drive'} if actuator is None else actuator
+    self._actuator = actuator
     self._gain = -gain if '-' in direction else gain
     self._direction = direction
     self._pixel_range = pixel_range
     self._max_speed = max_speed
 
     # Checking whether the Actuator communicates through an FT232H
     if actuator_dict[actuator['name']].ft232h:
       self._ft232h_args = USBServer.register(ft232h_ser_num)
 
   def prepare(self) -> None:
-    """Checks the consistency of the linking and initializes the actuator to
-    drive."""
+    """Checks the consistency of the linking and initializes the 
+    :class:`~crappy.actuator.Actuator` to drive."""
 
     # Checking that there's exactly one input link
     if not self.inputs:
-      raise IOError("The AutoDrive block should have an input link !")
+      raise IOError("The AutoDriveVideoExtenso block should have an input "
+                    "link !")
     elif len(self.inputs) > 1:
-      raise IOError("The AUtoDrive block can only have one input link !")
+      raise IOError("The AutoDriveVideoExtenso block can only have one input "
+                    "link !")
 
     # Opening and initializing the actuator to drive
     actuator_name = self._actuator.pop('name')
     if self._ft232h_args is None:
       self._device = actuator_dict[actuator_name](**self._actuator)
     else:
       self._device = actuator_dict[actuator_name](
         **self._actuator, _ft232h_args=self._ft232h_args)
     self.log(logging.INFO, f"Opening the {type(self._device).__name__} "
                            f"actuator")
     self._device.open()
     self._device.set_speed(0)
 
   def loop(self) -> None:
-    """Receives the latest data from the VideoExtenso block, calculates the
-    center coordinate in the chosen direction, and sets the actuator speed
-    accordingly."""
+    """Receives the latest data from the :class:`~crappy.blocks.VideoExtenso` 
+    Block, calculates the center coordinate in the chosen direction, and sets 
+    the :class:`~crappy.actuator.Actuator` speed accordingly."""
 
     # Receiving the latest data
     data = self.recv_last_data(fill_missing=False)
     if not data:
       return
 
     # Extracting the coordinates of the spots
@@ -125,15 +132,15 @@
     # Setting the speed and sending to downstream blocks
     self.log(logging.DEBUG, f"Setting the speed: {speed} on the "
                             f"{type(self._device).__name__} actuator.")
     self._device.set_speed(speed)
     self.send([t - self.t0, diff])
 
   def finish(self) -> None:
-    """Simply sets the device speed to `0`."""
+    """Stops the :class:`~crappy.actuator.Actuator` and closes it."""
 
     if self._device is not None:
       self.log(logging.INFO, f"Stopping the {type(self._device).__name__} "
                              f"actuator")
       self._device.stop()
       self.log(logging.INFO, f"Closing the {type(self._device).__name__} "
                              f"actuator")
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/camera_processes/camera_process.py` & `crappy-2.0.0.dev2/src/crappy/camera/ximea_xiapi.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,245 +1,216 @@
 # coding: utf-8
 
-from multiprocessing import Process, managers, get_start_method, \
-  current_process
-from multiprocessing.synchronize import Event, RLock, Barrier
-from multiprocessing.sharedctypes import SynchronizedArray
-from multiprocessing.connection import Connection
-from multiprocessing.queues import Queue
-from threading import BrokenBarrierError
+# TODO:
+#  Add downsampling ( self.cam.set_downsampling('XI_DWN_2x2') )
+#  Add region of interest selection
+#  Add possibility to adjust the timeout
+
+from time import time
+from typing import Optional, Tuple
 import numpy as np
-from typing import Optional, Tuple, List, Union, Dict, Any
 import logging
-import logging.handlers
-from select import select
-from time import time
 
-from ...links import Link
-from ..._global import LinkDataError
-from ...tool.camera_config import SpotsBoxes
+from .meta_camera import Camera
+from .._global import OptionalModule
+
+try:
+  from ximea import xiapi
+except (ModuleNotFoundError, ImportError):
+  xiapi = OptionalModule("ximea", "To use XiAPI cameras, please install the "
+                         "official ximea Python module")
+
+
+class XiAPI(Camera):
+  """This class can read images from any of the Ximea cameras.
+
+  It heavily relies on the :mod:`ximea` module, distributed by Ximea, which is
+  itself a wrapper around the XiAPI low-level library.
 
+  Note:
+    Both the Python module and the camera drivers have to be installed from
+    Ximea's website in order for this class to run.
+  """
 
-class CameraProcess(Process):
-  """"""
-
-  def __init__(self,
-               log_queue: Queue,
-               log_level: Optional[int] = 20,
-               display_freq: bool = False) -> None:
-    """"""
+  def __init__(self) -> None:
+    """Instantiates a Ximea Camera and a Ximea Image object."""
 
     super().__init__()
-    self.name = f"{current_process().name}.{type(self).__name__}"
 
-    self._log_queue = log_queue
-    self._logger: Optional[logging.Logger] = None
-    self._log_level = log_level
-
-    self._img_array: Optional[SynchronizedArray] = None
-    self._data_dict: Optional[managers.DictProxy] = None
-    self._lock: Optional[RLock] = None
-    self._cam_barrier: Optional[Barrier] = None
-    self._stop_event: Optional[Event] = None
-    self._shape: Optional[Tuple[int, int]] = None
-    self._box_conn: Optional[Connection] = None
-    self._outputs: List[Link] = list()
-    self._labels: List[str] = list()
-
-    self._img: Optional[np.ndarray] = None
-    self._dtype = None
-    self._metadata = {'ImageUniqueID': None}
-    self._img0_set = False
-
-    self._last_warn = time()
-    self.fps_count = 0
-    self.display_freq = display_freq
-    self._last_fps = time()
-
-  def set_shared(self,
-                 array: SynchronizedArray,
-                 data_dict: managers.DictProxy,
-                 lock: RLock,
-                 barrier: Barrier,
-                 event: Event,
-                 shape: Tuple[int, int],
-                 dtype,
-                 box_conn: Optional[Connection],
-                 outputs: List[Link],
-                 labels: List[str]) -> None:
-    """"""
-
-    self._img_array = array
-    self._data_dict = data_dict
-    self._lock = lock
-    self._cam_barrier = barrier
-    self._stop_event = event
-    self._shape = shape
-    self._dtype = dtype
-    self._box_conn = box_conn
-    self._outputs = outputs
-    self._labels = labels
-
-    self._img = np.empty(shape=shape, dtype=dtype)
-
-  def run(self) -> None:
-    """"""
-
-    try:
-      self._set_logger()
-      self._log(logging.INFO, "Logger configured")
-
-      try:
-        self._init()
-      except (Exception,):
-        self._cam_barrier.abort()
-        self._log(logging.ERROR, "Breaking the barrier due to caught exception"
-                                 " while preparing")
-        raise
-
-      self._log(logging.INFO, "Waiting for the other Camera processes to be "
-                              "ready")
-      self._cam_barrier.wait()
-      self._log(logging.INFO, "All Camera processes ready now")
-
-      self._last_fps = time()
-
-      while not self._stop_event.is_set():
-        self._loop()
-
-        if self.display_freq:
-          t = time()
-          if t - self._last_fps > 2:
-            self._log(logging.INFO, f"Images processed /s: "
-                                    f"{self.fps_count / (t - self._last_fps)}")
-            self._last_fps = t
-            self.fps_count = 0
-
-      self._log(logging.INFO, "Stop event set, stopping the processing")
-
-    except KeyboardInterrupt:
-      self._log(logging.INFO, "KeyboardInterrupt caught, stopping the "
-                              "processing")
-
-    except BrokenBarrierError:
-      self._log(logging.WARNING,
-                "Exception raised in another Camera process while waiting "
-                "for all Camera processes to be ready, stopping")
-
-    except (Exception,) as exc:
-      self._logger.exception("Exception caught wile running !", exc_info=exc)
-      self._log(logging.ERROR, "Setting the stop event to stop the other "
-                               "Camera processes")
-      self._stop_event.set()
-      raise
-
-    finally:
-      self._finish()
-
-  def _init(self) -> None:
-    """"""
-
-    ...
-
-  def _get_data(self) -> bool:
-    """"""
-
-    with self._lock:
-
-      if 'ImageUniqueID' not in self._data_dict:
-        return False
-
-      if self._data_dict['ImageUniqueID'] == self._metadata['ImageUniqueID']:
-        return False
-
-      self._metadata = self._data_dict.copy()
-
-      self._log(logging.DEBUG, f"Got new image to process with id "
-                               f"{self._metadata['ImageUniqueID']}")
-
-      np.copyto(self._img,
-                np.frombuffer(self._img_array.get_obj(),
-                              dtype=self._dtype).reshape(self._shape))
-
-    return True
-
-  def _loop(self) -> None:
-    """"""
-
-    ...
-
-  def _finish(self) -> None:
-    """"""
-
-    ...
-
-  def _send(self, data: Union[list, Dict[str, Any]]) -> None:
-    """"""
-
-    # Building the dict to send from the data and labels if the data is a list
-    if isinstance(data, list):
-      if not self._labels:
-        self._logger.log(logging.ERROR, "trying to send data as a list but no "
-                                        "labels are specified ! Please add a "
-                                        "self.labels attribute.")
-        raise LinkDataError
-      self._logger.log(logging.DEBUG, f"Converting {data} to dict before "
-                                      f"sending")
-      data = dict(zip(self._labels, data))
-
-    # Making sure the data is being sent as a dict
-    elif not isinstance(data, dict):
-      self._logger.log(logging.ERROR, f"Trying to send a {type(data)} in a "
-                                      f"Link !")
-      raise LinkDataError
-
-    # Sending the data to the downstream blocks
-    for link in self._outputs:
-      self._logger.log(logging.DEBUG, f"Sending {data} to Link {link}")
-      link.send(data)
-
-  def _send_box(self, boxes: SpotsBoxes) -> None:
-    """"""
+    self._cam = None
+    self._started = False
 
-    if self._box_conn is None:
-      return
+    self._cam = xiapi.Camera()
+    self._img = xiapi.Image()
 
-    self._log(logging.DEBUG, "Sending the box(es) to the displayer process")
+    # Stores the last requested or read trigger mode value
+    self._trig = 'Free run'
 
-    if select([], [self._box_conn], [], 0)[1]:
-      self._box_conn.send(boxes)
-    else:
-      if time() - self._last_warn > 1:
-        self._last_warn = time()
-        self._log(logging.WARNING, f"Cannot send the box(es) to draw to the "
-                                   f"Displayer process, the Pipe is full !")
-
-  def _set_logger(self) -> None:
-    """"""
-
-    logger = logging.getLogger(self.name)
-
-    # Disabling logging if requested
-    if self._log_level is not None:
-      logger.setLevel(self._log_level)
+  def open(self, serial_number: Optional[str] = None, **kwargs) -> None:
+    """Opens the connection to the camera, instantiates the available settings
+    and starts the acquisition.
+
+    Also sets custom values for the settings if provided by the user, otherwise
+    sets them to their default.
+
+    Args:
+      serial_number: A :obj:`str` containing the serial number of the camera to
+        open, in case several cameras are connected. If not provided and
+        several cameras are available, one of them will be opened randomly.
+      **kwargs: Values of the settings to set before opening the camera. Mostly
+       useful if the configuration window is not used.
+    """
+
+    if serial_number is not None:
+      self.log(logging.INFO, f"Opening the connection to the camera with "
+                             f"serial number {serial_number}")
+      self._cam.open_device_by_SN(serial_number)
     else:
-      logging.disable()
+      self.log(logging.INFO, "Opening the connection to the camera")
+      self._cam.open_device()
 
-    # On Windows, the messages need to be sent through a Queue for logging
-    if get_start_method() == "spawn" and self._log_level is not None:
-      queue_handler = logging.handlers.QueueHandler(self._log_queue)
-      queue_handler.setLevel(min(self._log_level, logging.INFO))
-      logger.addHandler(queue_handler)
+    self.add_scale_setting('width', 1, self._get_w(), self._get_w, self._set_w,
+                           self._get_w())
+    self.add_scale_setting('height', 1, self._get_h(), self._get_h,
+                           self._set_h, self._get_h())
+    self.add_scale_setting('xoffset', 0, self._get_w(), self._get_ox,
+                           self._set_ox, 0)
+    self.add_scale_setting('yoffset', 0, self._get_h(), self._get_oy,
+                           self._set_oy, 0)
+    self.add_scale_setting('exposure', 28, 500000, self._get_exp,
+                           self._set_exp, 10000)
+    self.add_scale_setting('gain', 0., 6., self._get_gain, self._set_gain)
+    self.add_bool_setting('AEAG', self._get_aeag, self._set_aeag, False)
+    self.add_trigger_setting(self._get_extt, self._set_ext_trig)
 
-    self._logger = logger
+    self.set_all(**kwargs)
+    self.log(logging.INFO, "Starting the image acquisition")
+    
+    self._cam.start_acquisition()
+    self._started = True
 
-  def _log(self, level: int, msg: str) -> None:
-    """Sends a log message to the logger.
+  def get_image(self) -> Tuple[float, np.ndarray]:
+    """Reads a frame from the camera, and returns it along with its
+    timestamp."""
 
-    Args:
-      level: The logging level, as an :obj:`int`.
-      msg: The message to log, as a :obj:`str`.
+    self._cam.get_image(self._img)
+    return time(), self._img.get_image_data_numpy()
+
+  def close(self) -> None:
+    """Closes the connection to the camera and releases the resources."""
+
+    if self._cam is not None:
+      self.log(logging.INFO, "Closing the connection to the camera")
+      self._cam.close_device()
+
+  def _get_w(self) -> int:
+    """Returns the width in pixels for selecting a region of interest."""
+
+    return self._cam.get_width()
+
+  def _get_h(self) -> int:
+    """Returns the height in pixels for selecting a region of interest."""
+
+    return self._cam.get_height()
+
+  def _get_ox(self) -> int:
+    """Returns the `x` offset in pixels for selecting a region of interest."""
+
+    return self._cam.get_offsetX()
+
+  def _get_oy(self) -> int:
+    """Returns the `y` offset in pixels for selecting a region of interest."""
+
+    return self._cam.get_offsetY()
+
+  def _get_gain(self) -> float:
+    """Returns the gain, in dB."""
+
+    return self._cam.get_gain()
+
+  def _get_exp(self) -> float:
+    """Returns the exposure time, in microseconds."""
+
+    return self._cam.get_exposure()
+
+  def _get_aeag(self) -> bool:
+    """Returns the auto exposure / auto gain parameter.
+
+    It is either :obj:`True` or :obj:`False`.
+    """
+
+    return self._cam.get_param('aeag')
+
+  def _get_extt(self) -> str:
+    """Returns the current trigger mode value, and updates the last read
+    trigger mode value if needed.
+
+    The possible values for the trigger mode are `'Hardware'`, `'Free run'`,
+    and `'Hdw after config'`.
+    """
+
+    r = self._cam.get_trigger_source()
+    if r == 'XI_TRG_OFF' and self._trig == 'Hardware':
+      self._trig = 'Free run'
+    elif r != 'XI_TRG_OFF' and self._trig != 'Hardware':
+      self._trig = 'Hardware'
+    return self._trig
+
+  def _set_w(self, width: int) -> None:
+    """Sets the width in pixels for selecting a region of interest."""
+
+    self._cam.set_width(width)
+
+  def _set_h(self, height: int) -> None:
+    """Sets the height in pixels for selecting a region of interest."""
+
+    self._cam.set_height(height)
+
+  def _set_ox(self, x_offset: int) -> None:
+    """Sets the `x` offset in pixels for selecting a region of interest."""
+
+    self._cam.set_offsetX(x_offset)
+
+  def _set_oy(self, y_offset: int) -> None:
+    """Sets the `y` offset in pixels for selecting a region of interest."""
+
+    self._cam.set_offsetY(y_offset)
+
+  def _set_gain(self, gain: float) -> None:
+    """Sets the gain, in dB."""
+
+    self._cam.set_gain(gain)
+
+  def _set_exp(self, exposure: float) -> None:
+    """Sets the exposure time, in microseconds."""
+
+    self._cam.set_exposure(exposure)
+
+  def _set_aeag(self, aeag: bool) -> None:
+    """Sets the auto exposure / auto gain parameter.
+
+    It is either :obj:`True` or :obj:`False`.
     """
 
-    if self._logger is None:
-      return
-    self._logger.log(level, msg)
+    self._cam.set_param('aeag', int(aeag))
+
+  def _set_ext_trig(self, trig: str) -> None:
+    """Sets the requested trigger mode value, and updates the last requested
+    trigger mode value.
+
+    The possible values for the trigger mode are `'Hardware'`, `'Free run'`,
+    and `'Hdw after config'`.
+    """
+
+    if self._started:
+      self._cam.stop_acquisition()
+
+    if trig == 'Hardware':
+      self._cam.set_gpi_mode('XI_GPI_TRIGGER')
+      self._cam.set_trigger_source('XI_TRG_EDGE_RISING')
+    else:
+      self._cam.set_gpi_mode('XI_GPI_OFF')
+      self._cam.set_trigger_source('XI_TRG_OFF')
+      
+    self._trig = trig
+    if self._started:
+      self._cam.start_acquisition()
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/camera_processes/record.py` & `crappy-2.0.0.dev2/src/crappy/blocks/button.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,158 +1,138 @@
 # coding: utf-8
 
-from multiprocessing.queues import Queue
-from csv import DictWriter
-from time import strftime, gmtime
-import numpy as np
-from typing import Optional, Union
-from pathlib import Path
+from time import time
 import logging
-import logging.handlers
+from typing import Optional
 
-from .camera_process import CameraProcess
-from ..._global import OptionalModule
+from .meta_block import Block
+from .._global import OptionalModule
 
 try:
-  import SimpleITK as Sitk
+  import tkinter as tk
 except (ModuleNotFoundError, ImportError):
-  Sitk = OptionalModule("SimpleITK")
+  tk = OptionalModule("tkinter")
 
-try:
-  import PIL
-  from PIL.ExifTags import TAGS
-  TAGS_INV = {val: key for key, val in TAGS.items()}
-except (ModuleNotFoundError, ImportError):
-  PIL = OptionalModule("Pillow")
-  TAGS = TAGS_INV = OptionalModule("Pillow")
-
-try:
-  import cv2
-except (ModuleNotFoundError, ImportError):
-  cv2 = OptionalModule("opencv-python")
 
-
-class ImageSaver(CameraProcess):
-  """"""
+class Button(Block):
+  """This Block allows the user to send a signal to downstream Blocks upon
+  clicking on a button in a Graphical User Interface.
+
+  It sends an integer value, that starts from `0` and is incremented every time
+  the user clicks on the button. This Block relies on a :obj:`~tkinter.Tk`
+  window for the graphical interface.
+
+  This Block is mostly useful for incorporating user feedback in a script, i.e.
+  triggering actions based on an experimenter's decision. It can be handy for
+  taking pictures at precise moments, or when an action should only begin after
+  the experimenter has completed a task, for example.
+  """
 
   def __init__(self,
-               log_queue: Queue,
-               log_level: int = 20,
-               img_extension: str = "tiff",
-               save_folder: Optional[Union[str, Path]] = None,
-               save_period: int = 1,
-               save_backend: Optional[str] = None,
-               display_freq: bool = False) -> None:
-    """"""
-
-    super().__init__(log_queue=log_queue,
-                     log_level=log_level,
-                     display_freq=display_freq)
-
-    # Trying the different possible backends and checking if the given one
-    # is correct
-    if save_backend is None:
-      if not isinstance(Sitk, OptionalModule):
-        self._save_backend = 'sitk'
-      elif not isinstance(PIL, OptionalModule):
-        self._save_backend = 'cv2'
-      elif not isinstance(PIL, OptionalModule):
-        self._save_backend = 'pil'
-      else:
-        raise ModuleNotFoundError("Neither SimpleITK, opencv-python nor "
-                                  "Pillow could be imported, no backend "
-                                  "found for saving the images")
-    elif save_backend in ('sitk', 'pil', 'cv2'):
-      self._save_backend = save_backend
-    else:
-      raise ValueError("The save_backend argument should be either 'sitk', "
-                       "'pil' or 'cv2' !")
-
-    self._img_extension = img_extension
-
-    # Setting a default save folder if not given
-    if save_folder is None:
-      self._save_folder = Path.cwd() / 'Crappy_images'
-    else:
-      self._save_folder = Path(save_folder)
-
-    self._save_period = int(save_period)
-
-    self._csv_created = False
-    self._csv_path = None
-
-  def _init(self) -> None:
-    """"""
-
-    if self._save_folder is not None and not self._save_folder.exists():
-      self._log(logging.INFO, f"Creating the folder for saving images at: "
-                              f"{self._save_folder}")
-      Path.mkdir(self._save_folder, exist_ok=True, parents=True)
-
-  def _get_data(self) -> bool:
-    """"""
-
-    with self._lock:
-
-      if 'ImageUniqueID' not in self._data_dict:
-        return False
-
-      if self._data_dict['ImageUniqueID'] == self._metadata['ImageUniqueID']:
-        return False
-
-      if self._metadata['ImageUniqueID'] is not None and \
-          self._data_dict['ImageUniqueID'] - self._metadata['ImageUniqueID'] \
-          < self._save_period:
-        return False
-
-      self._metadata = self._data_dict.copy()
-
-      self._log(logging.DEBUG, f"Got new image to process with id "
-                               f"{self._metadata['ImageUniqueID']}")
-
-      np.copyto(self._img,
-                np.frombuffer(self._img_array.get_obj(),
-                              dtype=self._dtype).reshape(self._shape))
-
-    return True
+               send_0: bool = False,
+               label: str = 'step',
+               time_label: str = 't(s)',
+               freq: Optional[float] = 50,
+               spam: bool = False,
+               display_freq: bool = False,
+               debug: Optional[bool] = False) -> None:
+    """Sets the arguments and initializes the parent class.
+
+    Args:
+      send_0: If :obj:`True`, the value `0` will be sent automatically when
+        starting the Block. Otherwise, `1` will be sent at the first click.
+        Only relevant when ``spam`` is :obj:`False`.
+      label: The label carrying the information on the number of clicks,
+        default is ``'step'``.
+      time_label: The label carrying the time information, default is
+        ``'t(s)'``.
+      freq: The target looping frequency for the Block. If :obj:`None`, loops
+        as fast as possible.
+      spam: If :obj:`True`, sends the current step value at each loop,
+        otherwise only sends it at each click.
+      display_freq: If :obj:`True`, displays the looping frequency of the
+        Block.
+      debug: If :obj:`True`, displays all the log messages including the
+        :obj:`~logging.DEBUG` ones. If :obj:`False`, only displays the log
+        messages with :obj:`~logging.INFO` level or higher. If :obj:`None`,
+        disables logging for this Block.
+    """
+
+    self._root: Optional[tk.Tk] = None
+
+    super().__init__()
+    self.freq = freq
+    self.labels = [time_label, label]
+    self.display_freq = display_freq
+    self.debug = debug
+
+    self._spam = spam
+    self._send_0 = send_0
+
+    self._step = None
+    self._text = None
+    self._label = None
+    self._button = None
+
+  def prepare(self) -> None:
+    """Creates the graphical interface and sets its layout and callbacks."""
+
+    self.log(logging.INFO, "Creating the GUI")
+
+    self._root = tk.Tk()
+    self._root.title("Button block")
+    self._root.resizable(False, False)
+
+    self._step = tk.IntVar()
+    self._step.trace_add('write', self._update_text)
+    self._text = tk.StringVar(value=f'step: {self._step.get()}')
+
+    self._label = tk.Label(self._root, textvariable=self._text)
+    self._label.pack(padx=7, pady=7)
+
+    self._button = tk.Button(self._root,
+                             text='Next step',
+                             command=self._next_step)
+    self._button.pack(padx=25, pady=7)
+
+    self._root.update()
+
+  def begin(self) -> None:
+    """Sends the value of the first step (`0`) if required."""
+
+    if self._send_0:
+      self.send([time() - self.t0, self._step.get()])
+
+  def loop(self) -> None:
+    """Updates the interface, and sends the current step value if ``spam`` is
+    :obj:`True`. """
+
+    try:
+      self._root.update()
+      self.log(logging.DEBUG, "GUI updated")
+    except tk.TclError:
+      return
 
-  def _loop(self) -> None:
-    """"""
+    if self._spam:
+      self.send([time() - self.t0, self._step.get()])
 
-    if not self._get_data():
-      return
-    self.fps_count += 1
+  def finish(self) -> None:
+    """Closes the interface window."""
 
-    if not self._csv_created:
-      self._csv_path = (self._save_folder /
-                        f'metadata_'
-                        f'{strftime("%d_%m_%y %H:%M:%S", gmtime())}.csv')
-
-      self._log(logging.INFO, f"Creating file for saving the metadata: "
-                              f"{self._csv_path}")
-
-      with open(self._csv_path, 'w') as csvfile:
-        writer = DictWriter(csvfile, fieldnames=self._metadata.keys())
-        writer.writeheader()
-
-      self._csv_created = True
-
-    self._log(logging.DEBUG, f"Saving metadata: {self._metadata}")
-    with open(self._csv_path, 'a') as csvfile:
-      writer = DictWriter(csvfile, fieldnames=self._metadata.keys())
-      writer.writerow({**self._metadata, 't(s)': self._metadata['t(s)']})
-
-    path = str(self._save_folder / f"{self._metadata['ImageUniqueID']}_"
-                                   f"{self._metadata['t(s)']:.3f}."
-                                   f"{self._img_extension}")
-
-    self._log(logging.DEBUG, "Saving image")
-    if self._save_backend == 'sitk':
-      Sitk.WriteImage(Sitk.GetImageFromArray(self._img), path)
-
-    elif self._save_backend == 'cv2':
-      cv2.imwrite(path, self._img)
-
-    elif self._save_backend == 'pil':
-      PIL.Image.fromarray(self._img).save(
-        path, exif={TAGS_INV[key]: val for key, val in self._metadata.items()
-                    if key in TAGS_INV})
+    self.log(logging.INFO, "closing the GUI")
+    try:
+      if self._root is not None:
+        self._root.destroy()
+    except tk.TclError:
+      pass
+
+  def _update_text(self, _, __, ___) -> None:
+    """Simply updates the displayed text."""
+
+    self._text.set(f'step: {self._step.get()}')
+
+  def _next_step(self) -> None:
+    """Increments the step counter and sends the corresponding signal."""
+
+    self.log(logging.DEBUG, "Next step on the GUI")
+    self._step.set(self._step.get() + 1)
+    self.send([time() - self.t0, self._step.get()])
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/client_server.py` & `crappy-2.0.0.dev2/src/crappy/blocks/client_server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 from .meta_block import Block
 from .._global import OptionalModule
-from typing import Dict, List, Union, Tuple, Any, Optional
+from typing import Dict, Union, Any, Optional, Iterable, List, Tuple
 from time import time, sleep
 from subprocess import Popen, PIPE, STDOUT, TimeoutExpired
 from threading import Thread
 from queue import Queue, Empty
 from ast import literal_eval
 from pickle import loads, dumps, UnpicklingError
 from socket import timeout, gaierror
@@ -14,103 +14,118 @@
 import logging
 
 try:
   import paho.mqtt.client as mqtt
 except (ModuleNotFoundError, ImportError):
   mqtt = OptionalModule("paho.mqtt.client")
 
-Topics_type = List[Union[str, Tuple[str, ...]]]
+TopicsType = Iterable[Union[str, Iterable[str]]]
 
 
 class ClientServer(Block):
-  """Block for exchanging data on a local network using the MQTT protocol.
-
-  This block can send data to an MQTT broker, receive data from this broker by
-  subscribing to its topics, and also launch the Mosquitto broker.
+  """This Block can exchange data on a local network using the MQTT protocol.
+  
+  It communicates with an MQTT broker, from which it can receive data by
+  subscribing to topics, and to which it can send data by publishing in topics.
+  This Block can also manage the execution of a Mosquitto broker, so that the
+  broker doesn't need to be manually started before running the Crappy script.
+
+  This Block is intended for communication with remote devices, that may run
+  Crappy scripts or other scripts handling data with the correct syntax.
+  Potential uses include acquisition from battery-powered devices (e.g.
+  microcontrollers) acquiring data in enclosed areas or rotating parts, data
+  transfer between machines to delegate processing, communication with other
+  programs on a same machine, etc.
   """
 
   def __init__(self,
                broker: bool = False,
                address: str = 'localhost',
                port: int = 1883,
                init_output: Optional[Dict[str, Any]] = None,
-               topics: Optional[Topics_type] = None,
-               cmd_labels: Optional[Topics_type] = None,
-               labels_to_send: Optional[Topics_type] = None,
+               topics: Optional[TopicsType] = None,
+               cmd_labels: Optional[TopicsType] = None,
+               labels_to_send: Optional[TopicsType] = None,
                display_freq: bool = False,
-               freq: float = 200,
+               freq: Optional[float] = 200,
                spam: bool = False,
                debug: Optional[bool] = False) -> None:
-    """Checks arguments validity and sets the instance attributes.
+    """Checks the validity of the arguments and sets the instance attributes.
 
     Args:
       broker: If :obj:`True`, starts the Mosquitto broker during the prepare
         loop and stops it during the finish loop. If Mosquitto is not installed
         a :exc:`FileNotFoundError` is raised.
-      address (optional): The network address on which the MQTT broker is
-        running.
-      port (:obj:`int`, optional): A network port on which the MQTT broker is
-        listening.
-      init_output (:obj:`dict`, optional): A :obj:`dict` containing for labels
-        in ``topics`` the first value to be sent in the output links. Should be
-        given in case the data comes from several sources and data for all
-        labels may not be available during the first loops.
-      topics (:obj:`list`, optional): A :obj:`list` of :obj:`str` and/or 
-        :obj:`tuple` of :obj:`str`. Each string corresponds to the name of a 
-        crappy label to be received from the broker. Each element of the list 
-        is considered to be the name of an MQTT topic, to which the client 
-        subscribes. After a message has been received on that topic, the block 
-        returns for each label in the topic (i.e. each string in the tuple) the
-        corresponding data from the message. It also returns the current
-        timestamp in the label `'t(s)'`.
-      cmd_labels (:obj:`list`, optional): A :obj:`list` of :obj:`str` and/or 
-        :obj:`tuple` of :obj:`str`. Each string corresponds to the name of a 
-        crappy label to send to the broker. Each element of the list is 
-        considered to be the name of an MQTT topic, in which the client 
-        publishes. Grouping labels in a same topic (i.e. strings in a same 
-        tuple) allows to keep the synchronization between signals coming from a
-        same block, as they will be published together in a same message. This 
-        is mostly useful for sending a signal along with its timeframe.
-      labels_to_send (:obj:`list`, optional): A :obj:`list` of :obj:`str` 
-        and/or :obj:`tuple` of :obj:`str`. Allows to rename the labels before 
-        publishing data. The structure of ``labels_to_send`` should be the 
-        exact same as ``cmd_labels``, with each label in ``labels_to_send`` 
-        replacing the corresponding one in ``cmd_labels``. This is especially 
-        useful for transferring several signals along with their timestamps, as
-        the label ``'t(s)'`` should not appear more than once in the topics 
-        list of the receiving block.
+      address: The network address on which the MQTT broker is running, as a
+        :obj:`str`.
+      port: A network port on which the MQTT broker is listening, as an 
+        :obj:`int`.
+      init_output: A :obj:`dict` containing for each label in ``topics`` the 
+        first value to be sent in the output Links. Should be given in case the 
+        data comes from several sources and data for all labels may not be 
+        available during the first loops. 
+      topics: An iterable (like a :obj:`list` or a :obj:`tuple`) containing
+        :obj:`str` and/or iterables of :obj:`str`. Each string corresponds to
+        the name of a label in Crappy. Each element in the iterable (string or
+        iterable of strings) is considered to be the name of an MQTT topic, to
+        which the client subscribes. After a message has been received on that
+        topic, the Block returns for each label in the topic (just the given
+        string or each string in the iterable) the corresponding data from the
+        message. It also returns the current timestamp in the label `'t(s)'`.
+      cmd_labels: An iterable (like a :obj:`list` or a :obj:`tuple`) containing
+        :obj:`str` and/or iterables of :obj:`str`. Each string corresponds to
+        the name of a label in Crappy. Each element in the iterable (string or
+        iterable of strings) is considered to be the name of an MQTT topic, in
+        which the client publishes. Grouping labels in a same topic (i.e.
+        strings in a same iterable) allows to keep the synchronization between
+        signals coming from a same Block, as they will be published together in
+        a same message. This is mostly useful for sending a signal along with
+        its timeframe.
+      labels_to_send: An iterable (like a :obj:`list` or a :obj:`tuple`)
+        containing :obj:`str` and/or iterables of :obj:`str`. Allows to rename
+        the labels before publishing data. The structure of ``labels_to_send``
+        should be the exact same as ``cmd_labels``, with each label in
+        ``labels_to_send`` replacing the corresponding one in ``cmd_labels``.
+        This is especially useful for transferring several signals along with
+        their timestamps, as the label ``'t(s)'`` should not appear more than
+        once in the topics.
       display_freq: If :obj:`True`, displays the looping frequency of the
-        block.
-      freq: The block will try to loop at this frequency.
+        Block.
+      freq: The target looping frequency for the Block. If :obj:`None`, loops
+        as fast as possible.
       spam: If :obj:`True`, sends the last received values at each loop even if
         no new values were received from the broker.
+      debug: If :obj:`True`, displays all the log messages including the
+        :obj:`~logging.DEBUG` ones. If :obj:`False`, only displays the log
+        messages with :obj:`~logging.INFO` level or higher. If :obj:`None`,
+        disables logging for this Block.
 
     Note:
       - ``broker``:
-        In order for the block to run, an MQTT broker must be running at the
+        In order for the Block to run, an MQTT broker must be running at the
         specified address on the specified port. If not, an
         :exc:`ConnectionRefusedError` is raised. The broker can be started and
-        stopped manually by the user independently of the execution of crappy.
+        stopped manually by the user independently of the execution of Crappy.
         It also doesn't need to be Mosquitto, any other MQTT broker can be
         used.
 
       - ``topics``:
         The presence of the same label in multiple topics will most likely lead
         to a data loss.
 
       - ``cmd_labels``:
-        It is not possible to group signals coming from different blocks in a
+        It is not possible to group signals coming from different Blocks in a
         same topic.
 
       - ``labels_to_send``:
         Differences in the structure of ``labels_to_send`` and ``cmd_labels``
         will not always raise an error, but may lead to a data loss.
 
-      - **Single-value tuples**:
-        Single-value tuples can be shortened as strings.
+      - **Single-value iterables**:
+        Single-value iterables can be shortened as strings.
         ::
 
           topics=[('cmd1',), ('cmd2',)]
           cmd_labels=[('cmd1',), ('cmd2',)]
           labels_to_send=[('cmd1',), ('cmd2',)]
 
         is equivalent to
@@ -130,15 +145,15 @@
 
         the client will subscribe to the topics
         ::
 
           ('t1', 'cmd1')
           ('sign',)
 
-        The block will return data associated with the labels
+        The Block will return data associated with the labels
         ::
 
           't1', 'cmd1'
           'sign'
 
 
       - ``cmd_labels``:
@@ -212,49 +227,49 @@
     # Instantiating the client
     self._client = mqtt.Client(str(time()))
     self._client.on_connect = self._on_connect
     self._client.on_message = self._on_message
     self._client.reconnect_delay_set(max_delay=10)
     
     # These attributes may be set later
-    self._topics = None
-    self._last_out_val = {}
-    self._buffer_output = None
-    self._cmd_labels = None
-    self._labels_to_send = None
+    self._topics: Optional[List[Tuple[str, ...]]] = None
+    self._last_out_val: Dict[str, Any] = dict()
+    self._buffer_output: Optional[Dict[Tuple[str, ...], Queue]] = None
+    self._cmd_labels: Optional[List[Tuple[str, ...]]] = None
+    self._labels_to_send: Optional[List[Tuple[str, ...]]] = None
 
     if topics is None and cmd_labels is None:
       self.log(logging.WARNING, "The Client-server Block is neither an input "
                                 "nor an output !")
 
     # Preparing for receiving data
     if topics is not None:
       # Replacing strings with tuples
-      self._topics = [topic if isinstance(topic, tuple) else (topic,) for
+      self._topics = [(topic,) if isinstance(topic, str) else tuple(topic) for
                       topic in topics]
 
       # The last out vals are given for each label, not each topic
       self._last_out_val = {label: None for label in chain(*self._topics)}
 
       # The buffer for received data is a dictionary of queues
-      self._buffer_output = {topic: Queue() for topic in topics}
+      self._buffer_output = {topic: Queue() for topic in self._topics}
 
     # Preparing for publishing data
     if cmd_labels is not None:
       # Replacing strings with tuples
-      self._cmd_labels = [topic if isinstance(topic, tuple) else (topic,)
+      self._cmd_labels = [(topic,) if isinstance(topic, str) else tuple(topic)
                           for topic in cmd_labels]
 
       if labels_to_send is not None:
         # Replacing strings with tuples
-        labels_to_send = [topic if isinstance(topic, tuple) else (topic,)
+        labels_to_send = [(topic,) if isinstance(topic, str) else tuple(topic)
                           for topic in labels_to_send]
 
         # Making sure the labels to send have the correct syntax
-        if len(labels_to_send) != len(cmd_labels):
+        if len(labels_to_send) != len(self._cmd_labels):
           raise ValueError("Either a label_to_send should be given for "
                            "every cmd_label, or none should be given ")
 
         # Preparing to rename labels to send using a dictionary
         self._labels_to_send = {cmd_label: label_to_send for
                                 cmd_label, label_to_send in
                                 zip(self._cmd_labels, labels_to_send)}
@@ -300,15 +315,15 @@
 
     self.log(logging.INFO, "Starting the client loop")
     self._client.loop_start()
 
   def loop(self) -> None:
     """Receives data from the broker and/or sends data to the broker.
 
-    The received data is then sent to the crappy blocks connected to this one.
+    The received data is then sent to the crappy Blocks connected to this one.
     """
 
     """Loop for receiving data
     Each queue in the buffer is checked once: if not empty then the first list 
     of data is popped. This data is then associated to the corresponding 
     labels in dict_out. dict_out is finally returned if not empty. All the 
     labels should be returned at each loop iteration, so a buffer stores the
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/dashboard.py` & `crappy-2.0.0.dev2/src/crappy/blocks/dashboard.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 
-from typing import List, Optional
+from typing import List, Optional, Iterable, Union
 import tkinter as tk
 import logging
 
 from .meta_block import Block
 
 
 class DashboardWindow(tk.Tk):
@@ -46,60 +46,77 @@
       self._tk_values[label] = tk.Label(self, borderwidth=15,
                                         textvariable=self.tk_var[label],
                                         font=("Courier bold", 48))
       self._tk_values[label].grid(row=row, column=1)
 
 
 class Dashboard(Block):
-  """The Dashboard receives data from a :ref:`Link`, and displays it on a new
-  popped window.
+  """This Block generates an interface displaying data as text in a dedicated
+  window.
 
-  It can only display data coming from one block.
+  It can only display data coming from one Block. It relies on a
+  :obj:`~tkinter.Tk` window for the graphical interface.
+
+  In the window, the left column contains the names of the labels to display
+  and the right column contains the latest received values for these labels.
+  For each label, only the last value is therefore displayed.
+
+  This Block provides a nicer display than the raw
+  :class:`~crappy.blocks.LinkReader` Block. For displaying the evolution of a
+  label over time, the :class:`~crappy.blocks.Grapher` Block should be used
+  instead.
   """
 
   def __init__(self,
-               labels: List[str],
+               labels: Union[str, Iterable[str]],
                nb_digits: int = 2,
                display_freq: bool = False,
-               freq: float = 30,
+               freq: Optional[float] = 30,
                debug: Optional[bool] = False) -> None:
-    """Sets the args and initializes parent class.
+    """Sets the arguments and initializes the parent class.
 
     Args:
       labels: Only the data from these labels will be displayed on the window.
       nb_digits: Number of decimals to show.
       display_freq: If :obj:`True`, displays the looping frequency of the
-        block.
-      freq: If set, the block will try to loop at this frequency.
+        Block.
+      freq: The target looping frequency for the Block. If :obj:`None`, loops
+        as fast as possible.
+      debug: If :obj:`True`, displays all the log messages including the
+        :obj:`~logging.DEBUG` ones. If :obj:`False`, only displays the log
+        messages with :obj:`~logging.INFO` level or higher. If :obj:`None`,
+        disables logging for this Block.
     """
 
     self._dashboard: Optional[DashboardWindow] = None
 
     super().__init__()
     self.display_freq = display_freq
     self.freq = freq
     self.debug = debug
 
-    self._labels = labels
+    self._labels = [labels] if isinstance(labels, str) else list(labels)
     self._nb_digits = nb_digits
 
   def prepare(self) -> None:
-    """Checks that there's only one incoming link, and starts the GUI."""
+    """Checks that there's only one incoming :class:`~crappy.links.Link`, and
+    starts the GUI."""
 
     if len(self.inputs) == 0:
       raise IOError("No link pointing towards the Dashboard block !")
     elif len(self.inputs) > 1:
       raise IOError("Too many links pointing towards the Dashboard block !")
 
     self.log(logging.INFO, "Creating the dashboard window")
     self._dashboard = DashboardWindow(self._labels)
     self._dashboard.update()
 
   def loop(self) -> None:
-    """Receives the data from the incoming link and displays it."""
+    """Receives the data from the incoming :class:`~crappy.links.Link` and
+    displays it."""
 
     data = self.recv_last_data(fill_missing=False)
 
     for label, value in data.items():
       # Only displays the required labels
       if label in self._labels:
         # Possibility to display str values carried by the links
@@ -115,15 +132,15 @@
     # In case the GUI has been destroyed, don't raise an error
     try:
       self._dashboard.update()
     except tk.TclError:
       pass
 
   def finish(self) -> None:
-    """"""
+    """Closes the display."""
 
     # In case the GUI has been destroyed, don't raise an error
     try:
       if self._dashboard is not None:
         self.log(logging.INFO, "Closing the dashboard window")
         self._dashboard.destroy()
     except tk.TclError:
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/drawing.py` & `crappy-2.0.0.dev2/src/crappy/blocks/camera_processes/gpu_ve.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,243 +1,188 @@
 # coding: utf-8
 
-from __future__ import annotations
-from datetime import timedelta
-from time import time
-from typing import Tuple, List, Dict, Any, Optional
+from multiprocessing.queues import Queue
+import numpy as np
+from typing import Optional, Tuple, List, Union
+from pathlib import Path
 import logging
+import logging.handlers
 
-from .meta_block import Block
-from .._global import OptionalModule
-
-plt = OptionalModule('matplotlib.pyplot', lazy_import=True)
-mpl = OptionalModule('matplotlib', lazy_import=True)
-
-
-class Text:
-  """Displays a simple text line on the drawing."""
-
-  def __init__(self,
-               _: Drawing,
-               coord: Tuple[int, int],
-               text: str,
-               label: str,
-               **__: str) -> None:
-    """Simply sets the args.
-
-    Args:
-      _: The parent drawing block.
-      coord: The coordinates of the text on the drawing.
-      text: The text to display.
-      label: The label carrying the information for updating the text.
-      **__: Other unused arguments.
-    """
-
-    x, y = coord
-    self._text = text
-    self._label = label
-
-    self._txt = plt.text(x, y, text)
-
-  def update(self, data: Dict[str, float]) -> None:
-    """Updates the text according to the received values."""
-
-    if self._label in data:
-      self._txt.set_text(self._text % data[self._label])
-
-
-class DotText:
-  """Like :class:`Text`, but with a colored dot to visualize a numerical value.
+from .camera_process import CameraProcess
+from ...tool.image_processing import GPUCorrelTool
+from ...tool.camera_config import SpotsBoxes
+from ..._global import OptionalModule
+
+try:
+  import pycuda.tools
+  import pycuda.driver
+except (ModuleNotFoundError, ImportError):
+  pycuda = OptionalModule("pycuda")
+
+
+class GPUVEProcess(CameraProcess):
+  """This :class:`~crappy.blocks.camera_processes.CameraProcess` can perform
+  GPU-accelerated video-extensometry by tracking patches using digital image
+  correlation. It then returns the position of the tracked patches.
+
+  It is used by the :class:`~crappy.blocks.GPUVE` Block to parallelize the
+  image processing and the image acquisition. It delegates most of the
+  computation to the :class:`~crappy.tool.image_processing.GPUCorrelTool`. It
+  is from this class that the output values are sent to the downstream Blocks,
+  and that the :class:`~crappy.tool.camera_config.config_tools.SpotsBoxes` are
+  sent to the :class:`~crappy.blocks.camera_processes.Displayer` CameraProcess
+  for display.
   """
 
   def __init__(self,
-               drawing: Drawing,
-               coord: Tuple[int, int],
-               text: str,
-               label: str,
-               **__: str) -> None:
-    """Simply sets the args.
+               patches: List[Tuple[int, int, int, int]],
+               log_queue: Queue,
+               log_level: int = 20,
+               verbose: int = 0,
+               kernel_file: Optional[Union[str, Path]] = None,
+               iterations: int = 4,
+               img_ref: Optional[np.ndarray] = None,
+               mul: float = 3) -> None:
+    """Sets the arguments and initializes the parent class.
 
     Args:
-      drawing: The parent drawing block.
-      coord: The coordinates of the text and the color dot on the drawing.
-      text: The text to display.
-      label: The label carrying the information for updating the text and the
-        color of the dot.
-      **__: Other unused arguments.
-
-        Important:
-          The value received in label must be a numeric value. It will be
-          normalized on the ``crange`` of the block and the dot will change
-          color from blue to red depending on this value.
+      patches: A :obj:`list` containing the coordinates of the patches to
+        track, as a :obj:`tuple` for each patch. Each tuple should contain
+        exactly `4` elements, giving in pixels the `y` origin, `x` origin,
+        height and width of the patch.
+      log_queue: A :obj:`~multiprocessing.Queue` for sending the log messages
+        to the main :obj:`~logging.Logger`, only used in Windows.
+      log_level: The minimum logging level of the entire Crappy script, as an
+        :obj:`int`.
+      verbose: The verbose level as an integer, between `0` and `3`. At level
+        `0` no information is displayed, and at level `3` so much information
+        is displayed that is slows the code down. This argument is passed to
+        the :class:`~crappy.tool.image_processing.GPUCorrelTool` and not used
+        in this class.
+      kernel_file: The path to the file containing the kernels to use for the
+        correlation. Can be a :obj:`pathlib.Path` object or a :obj:`str`. If
+        not provided, the default :ref:`GPU Kernels` are used. This argument is
+        passed to the :class:`~crappy.tool.image_processing.GPUCorrelTool` and
+        not used in this class.
+      iterations: The maximum number of iterations to run before returning the
+        results. The results may be returned before if the residuals start
+        increasing. This argument is passed to the
+        :class:`~crappy.tool.image_processing.GPUCorrelTool` and not used in
+        this class.
+      img_ref: A reference image for the correlation, given as a 2D
+        :obj:`numpy.array` with `dtype` :obj:`numpy.float32`. If not given, the
+        first acquired frame will be used as the reference image instead. This
+        argument is passed to the
+        :class:`~crappy.tool.image_processing.GPUCorrelTool` and not used in
+        this class.
+      mul: The scalar by which the direction will be multiplied before being
+        added to the solution. If it's too high, the convergence will be fast
+        but there's a risk to go past the solution and to diverge. If it's too
+        low, the convergence will be slower and require more iterations. `3`
+        was found to be an acceptable value in most cases, but it is
+        recommended to tune this value for each application so that the
+        convergence is neither too slow nor too fast. This argument is passed
+        to the :class:`~crappy.tool.image_processing.GPUCorrelTool` and not
+        used in this class.
     """
 
-    x, y = coord
-    self._text = text
-    self._label = label
-
-    self._txt = plt.text(x + 40, y + 20, text, size=16)
-    self._dot = plt.Circle(coord, 20)
-
-    drawing.ax.add_artist(self._dot)
-    low, high = drawing.color_range
-
-    self._amp = high - low
-    self._low = low
-
-  def update(self, data: Dict[str, float]) -> None:
-    """Updates the text and the color dot according to the received values."""
-
-    if self._label in data:
-      self._txt.set_text(self._text % data[self._label])
-      self._dot.set_color(mpl.cm.coolwarm((data[self._label] -
-                                           self._low) / self._amp))
-
+    super().__init__(log_queue=log_queue, log_level=log_level,
+                     display_freq=bool(verbose))
 
-class Time:
-  """Displays a time counter on the drawing, starting at the beginning of the
-  test."""
-
-  def __init__(self, drawing: Drawing, coord: Tuple[int, int], **__) -> None:
-    """Simply sets the args.
-
-    Args:
-      drawing: The parent drawing block.
-      coord: The coordinates of the time counter on the drawing.
-      **__: Other unused arguments.
+    # Making a CUDA context common to all the patches
+    pycuda.driver.init()
+    context = pycuda.tools.make_default_context()
+
+    self._gpu_ve_kw = dict(context=context,
+                           verbose=verbose,
+                           levels=1,
+                           resampling_factor=2,
+                           kernel_file=kernel_file,
+                           iterations=iterations,
+                           fields=['x', 'y'],
+                           ref_img=img_ref,
+                           mask=None,
+                           mul=mul)
+
+    self._correls: Optional[List[GPUCorrelTool]] = None
+    self._patches = patches
+    self._img_ref = img_ref
+
+    self._spots = SpotsBoxes()
+    self._spots.set_spots(patches)
+
+    self._img0_set = img_ref is not None
+
+  def _init(self) -> None:
+    """Initializes the GPUCorrelTool instances, and set their reference image
+    if a ``img_ref`` argument was provided."""
+
+    # Instantiating the GPUCorrelTool instances
+    self._log(logging.INFO, "Instantiating the GPUCorrel tool instances")
+    self._gpu_ve_kw.update(logger_name=self.name)
+    self._correls = [GPUCorrelTool(**self._gpu_ve_kw) for _ in self._patches]
+
+    # We can already set the sizes of the images as they are already known
+    self._log(logging.INFO, "Setting the sizes of the patches")
+    for correl, (_, __, h, w) in zip(self._correls, self._patches):
+      correl.set_img_size((h, w))
+
+    # Setting the reference image if it was given as an argument
+    if self._img_ref is not None:
+      self._log(logging.INFO, "Initializing the GPUCorrel tool instances "
+                              "with the given reference image and preparing "
+                              "them")
+      for correl, (oy, ox, h, w) in zip(self._correls, self._patches):
+        correl.set_orig(
+          self._img_ref[oy:oy + h, ox:ox + w].astype(np.float32))
+        correl.prepare()
+
+  def _loop(self) -> None:
+    """This method grabs the latest frame and gives it for processing to the
+    several instances of :class:`~crappy.tool.image_processing.GPUCorrelTool`.
+    Then sends the displacement data to the downstream Blocks.
+
+    If there's no new frame grabbed, doesn't do anything. On the first acquired
+    frame, does not process it but initializes the instances of GPUCorrelTool
+    with it instead if no reference image was given as argument. Also sends the
+    patches for display to the
+    :class:`~crappy.blocks.camera_processes.Displayer` CameraProcess.
     """
 
-    self._block = drawing
-    x, y = coord
-
-    self._txt = plt.text(x, y, "00:00", size=38)
-
-  def update(self, _: Dict[str, float]) -> None:
-    """Updates the time counter, independently of the received values."""
-
-    self._txt.set_text(str(timedelta(seconds=int(time() - self._block.t0))))
-
-
-class Drawing(Block):
-  """This block allows displaying a real-time visual representation of data.
-
-  It displays the data on top of a background image and updates it according to
-  the values received through the incoming links.
-
-  It is possible to display simple text, a time counter, ot text associated
-  with a color dot evolving depending on a predefined color bar and the
-  received values.
-  """
-
-  def __init__(self,
-               image_path: str,
-               draw: Optional[List[Dict[str, Any]]] = None,
-               color_range: Tuple[float, float] = (20, 300),
-               title: str = "Drawing",
-               window_size: Tuple[int, int] = (7, 5),
-               backend: str = "TkAgg",
-               freq: float = 2,
-               display_freq: bool = False,
-               debug: Optional[bool] = False) -> None:
-    """Sets the args and initializes the parent class.
-
-    Args:
-      image_path: Path to the image that will be the background of the canvas,
-        as a :obj:`str`.
-      draw: A :obj:`list` of :obj:`dict` defining what to draw. See below for
-        more details.
-      color_range: A :obj:`tuple` containing the lowest and highest values for
-        the color bar.
-      title: The title of the window containing the drawing.
-      window_size: The x and y dimension of the window, following
-        :mod:`matplotlib` nomenclature.
-      backend: The :mod:`matplotlib` backend to use.
-      freq: The block will try to loop at this frequency.
-      display_freq: If :obj:`True`, displays the looping frequency of the
-        block.
-
-    Note:
-      - Information about the ``draw`` keys:
-
-        - ``type``: Mandatory, the type of drawing to display. It can be either
-          `'text'`, `'dot_text'` or `'time'`.
-
-        - ``coord``: Mandatory, a :obj:`tuple` containing the `x` and `y`
-          coordinates where the element should be displayed on the drawing.
-
-        - ``text``: Mandatory for :class:`Text` and :class:`DotText` only, the
-          text to display on the drawing. It must follow the %-formatting, and
-          contain exactly one %-field. This field will be updated using the
-          value carried by ``label``.
-
-        - ``label``: Mandatory for :class:`Text` and :class:`DotText` only,
-          the label of the data to display. It will try to retrieve this data
-          in the incoming links. The ``text`` will then be updated with this
-          data.
-    """
-
-    super().__init__()
-    self.freq = freq
-    self.display_freq = display_freq
-    self.debug = debug
-
-    self._image = image_path
-    self._draw = [] if draw is None else draw
-    self.color_range = color_range
-    self._title = title
-    self._window_size = window_size
-    self._backend = backend
-
-    self._fig = None
-    self.ax = None
-    self._drawing_elements = None
-
-  def prepare(self) -> None:
-    """Initializes the different elements of the drawing."""
-
-    self.log(logging.INFO, "Opening the drawing windows")
-
-    # Initializing the window and the background image
-    plt.switch_backend(self._backend)
-    self._fig, self.ax = plt.subplots(figsize=self._window_size)
-    image = self.ax.imshow(plt.imread(self._image), cmap=mpl.cm.coolwarm)
-    image.set_clim(-0.5, 1)
-
-    # Initializing the color bar
-    cbar = self._fig.colorbar(image, ticks=[-0.5, 1], fraction=0.061,
-                              orientation='horizontal', pad=0.04)
-    cbar.set_label('Temperatures(C)')
-    cbar.ax.set_xticklabels(self.color_range)
-
-    # Setting the title and the axes
-    self.ax.set_title(self._title)
-    self.ax.set_axis_off()
-
-    # Adding the elements to the drawing
-    self._drawing_elements = []
-    for dic in self._draw:
-      if dic['type'] == 'text':
-        self._drawing_elements.append(Text(self, **dic))
-      elif dic['type'] == 'dot_text':
-        self._drawing_elements.append(DotText(self, **dic))
-      elif dic['type'] == 'time':
-        self._drawing_elements.append(Time(self, **dic))
-
-  def loop(self) -> None:
-    """Receives the latest data from upstream blocks and updates the drawing
-    accordingly."""
-
-    data = self.recv_last_data(fill_missing=False)
-    if not data:
+    # Nothing to do if no new frame was grabbed
+    if not self._get_data():
       return
 
-    for elt in self._drawing_elements:
-      elt.update(data)
-    self.log(logging.DEBUG, "Updating the drawing window")
-    self._fig.canvas.draw()
-    plt.pause(0.001)
+    self.fps_count += 1
 
-  def finish(self) -> None:
-    """Simply closes the window containing the drawing."""
+    # Setting the reference image with the first received frame if it was not
+    # given as an argument
+    if not self._img0_set:
+      self._log(logging.INFO, "Setting the reference image")
+      for correl, (oy, ox, h, w) in zip(self._correls, self._patches):
+        correl.set_orig(self._img[oy:oy + h,
+                        ox:ox + w].astype(np.float32))
+        correl.prepare()
+      self._img0_set = True
+      return
 
-    self.log(logging.INFO, "Closing the drawing windows")
-    plt.close()
+    # Performing the image correlation
+    self._log(logging.DEBUG, "Processing the received image")
+    data = [self._metadata['t(s)'], self._metadata]
+    for correl, (oy, ox, h, w) in zip(self._correls, self._patches):
+      data.extend(correl.get_disp(
+        self._img[oy:oy + h, ox:ox + w].astype(np.float32)).tolist())
+
+    # Sending the data to downstream Blocks
+    self._send(data)
+
+    # Sending the patches to the Displayer for display
+    self._send_box(self._spots)
+
+  def _finish(self) -> None:
+    """Performs cleanup on the several
+    :class:`~crappy.tool.image_processing.GPUCorrelTool` used."""
+
+    if self._correls is not None:
+      self._log(logging.INFO, "Cleaning up the GPUCorrel instances")
+      for correl in self._correls:
+        correl.clean()
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/fake_machine.py` & `crappy-2.0.0.dev2/src/crappy/blocks/fake_machine.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,58 +13,71 @@
 
   if v > yield_strain:
     return rate * ((((v - yield_strain) / rate) ** 2 + 1) ** .5 - 1)
   return 0
 
 
 class FakeMachine(Block):
-  """This block simulates the behavior of a tensile test machine.
-
-  It should be used to simulate tensile teste, not compression tests. By
-  default, it assumes a plastic behavior of the material. The main mechanical
+  """This Block emulates the behavior of a tensile test machine.
+  
+  It can emulate tensile tests, **not compression tests**. By default, it 
+  assumes an elasto-plastic behavior of the tested sample. The main mechanical
   parameters of the material are tunable.
-
-  This block is meant to be driven like the :ref:`Machine` block. However, its
-  outputs are different and are : ``t(s), F(N), x(mm), Exx(%), Eyy(%)``.
+  
+  This Block is meant to be driven like a :class:`~crappy.blocks.Machine` 
+  Block. It receives speed or position commands from upstream Blocks, and 
+  modifies the behavior of the emulated machine accordingly. Its outputs are
+  however different from the Machine Blocks, as it outputs the current force, 
+  position, and strain of the emulated tensile test machine. The labels
+  carrying this data are : ``t(s), F(N), x(mm), Exx(%), Eyy(%)``.
+  
+  This Block was originally designed for proposing examples that do not require
+  any hardware to run, but still display the possibilities of Crappy. It can
+  also be used to test a script without actually interacting with hardware.
   """
 
   def __init__(self,
                rigidity: float = 8.4E6,
                l0: float = 200,
                max_strain: float = 1.51,
                sigma: Optional[Dict[str, float]] = None,
                nu: float = 0.3,
                plastic_law: Callable[[float], float] = plastic,
                max_speed: float = 5,
                mode: str = 'speed',
                cmd_label: str = 'cmd',
-               freq: float = 100,
+               freq: Optional[float] = 100,
                display_freq: bool = False,
                debug: Optional[bool] = False) -> None:
-    """Sets the args and initializes the parent class.
+    """Sets the arguments and initializes the parent class.
 
     Args:
-      rigidity: The rigidity of the material, in N, so that
-        ``force = k x strain``.
+      rigidity: The rigidity of the material, in N, so that 
+        :math:`force = k * strain`.
       l0: The initial length of the fake sample to test, in mm.
       max_strain: The maximum strain the material can withstand before
         breaking.
       mode: Whether the command sent to the fake machine is a speed or a
         position command. Can be ``'speed'`` or ``'position'``.
       plastic_law: A callable taking the maximum reached strain and returning
         the proportion of the current strain caused by plastic deformation.
       sigma: A :obj:`dict` containing for each label the standard deviation for
         adding noise to the signal. Can be given for part or all of the labels.
         The deviation should be given not normalized, in the same unit as the
         label to which it applies.
       nu: Poisson's ratio of the material.
       cmd_label: The label carrying the command of the fake machine.
-      freq: The block will try to loop at this frequency.
+      freq: The target looping frequency for the Block. If :obj:`None`, loops 
+        as fast as possible.
       display_freq: If :obj:`True`, displays the looping frequency of the
-        block.
+        Block.
+      debug: If :obj:`True`, displays all the log messages including the
+        :obj:`~logging.DEBUG` ones. If :obj:`False`, only displays the log
+        messages with :obj:`~logging.INFO` level or higher. If :obj:`None`,
+        disables logging for this Block.
     """
 
     super().__init__()
     self.freq = freq
     self.display_freq = display_freq
     self.debug = debug
 
@@ -93,15 +106,15 @@
 
     self._prev_t = self.t0
     self._send_values()
 
   def loop(self) -> None:
     """Receives the latest command value, calculates the new speed and position
     from it, checks whether the sample broke and what the plastic elongation
-    is, and finally returns the data"""
+    is, and finally returns the data."""
 
     # Getting the latest command
     data = self.recv_last_data(fill_missing=True)
     if self._cmd_label not in data:
       return
     else:
       cmd = data[self._cmd_label]
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/generator.py` & `crappy-2.0.0.dev2/src/crappy/blocks/generator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 from time import time, sleep
-from typing import Dict, List, Any, Optional, Iterator
+from typing import Dict, Any, Optional, Iterator, Iterable
 from itertools import cycle
 from copy import deepcopy
 import logging
 
 from .meta_block import Block
 from .generator_path.meta_path import paths_dict
 from .._global import GeneratorStop
@@ -13,73 +13,75 @@
 
 class GeneratorNoStop(Exception):
   """A custom exception for handling the case when the Generator should not
   raise a :exc:`CrappyStop` exception when it terminates."""
 
 
 class Generator(Block):
-  """This block generates a signal following a user-defined path.
+  """This Block generates a signal following a user-defined assembly of
+  :class:`~crappy.blocks.generator_path.meta_path.Path`.
+  
+  The generated signal is just a waveform that can serve any purpose. It can
+  for example be used for driving a :class:`~crappy.blocks.Machine` Block, or 
+  for triggering a :class:`~crappy.blocks.Camera` Block.
 
-  One Generator block can only generate one signal. Use multiple blocks if
+  One Generator Block can only generate one signal. Use multiple Blocks if
   several signals are needed. Note that the default behavior of a Generator
-  is to stop the entire script when it ends.
+  is to stop the entire script when it reaches the end of all the Paths.
 
-  It should be used as an input for other blocks, for example for driving a
-  :ref:`Machine` or an :ref:`IOBlock`. It can also accept inputs, to make the
-  path dependent on data coming from other blocks.
+  This Block can also accept inputs from other Blocks, as these inputs may be
+  used by a :class:`~crappy.blocks.generator_path.meta_path.Path`. The most
+  common use of this feature is to have the stop condition of a Path depend on
+  the received values of a label.
   """
 
   def __init__(self,
-               path: List[Dict[str, Any]],
-               freq: float = 200,
+               path: Iterable[Dict[str, Any]],
+               freq: Optional[float] = 200,
                cmd_label: str = 'cmd',
                cycle_label: str = 'cycle',
                repeat: bool = False,
                spam: bool = False,
                display_freq: bool = False,
                end_delay: Optional[float] = 2,
                safe_start: bool = False,
                debug: Optional[bool] = False) -> None:
-    """Sets the args and initializes the parent class.
+    """Sets the arguments and initializes the parent class.
 
     Args:
-      path: It must be a :obj:`list` of :obj:`dict`, each dict providing the
-        parameters to generate the path. Refer to the Note below for more
-        information.
-      freq: The looping frequency this block will try to achieve. Note that the
-        higher this value, the more accurate the path will be. It will also
-        consume more resources.
-      cmd_label: The label of the signal sent to the downstream blocks.
-      cycle_label: In addition to the `cmd_label`, this label holds the index
-        of the current dict in the ``path`` list. Useful to trig a block  upon
-        change in the current dict.
+      path: An iterable (like a :obj:`list` or a :obj:`tuple`) of :obj:`dict`,
+        each dict providing the parameters to generate a 
+        :class:`~crappy.blocks.generator_path.meta_path.Path`. The Paths are
+        generated in the order in which they are given, and the stop condition
+        of each Path is used for determining when to switch to the next one.
+      freq: The target looping frequency for the Block. If :obj:`None`, loops 
+        as fast as possible.
+      cmd_label: The label of the signal sent to the downstream Blocks.
+      cycle_label: In addition to the ``cmd_label``, this label holds the index
+        of the current :class:`~crappy.blocks.generator_path.meta_path.Path`.
+        Useful to trigger a Block when the current Path changes, as the output
+        value might not necessarily change.
       repeat: If :obj:`True`, the ``path`` will loop forever instead of
-        stopping when the list of dicts is exhausted.
+        stopping when it reaches the last Path.
       spam: If :obj:`True`, the signal value will be sent on each loop. Else,
         it will only be sent if it is different from the previous or if the
-        ``path`` switched to a new dict.
-      display_freq: if :obj:`True`, displays the loop frequency of the block
-        and a message when switching to the next dict of ``path``.
-      end_delay: When all the dicts in ``path`` are exhausted, waits this many
-        seconds before stopping the entire program. Can be set to :obj:`None`,
+        Block switched to the next Path.
+      display_freq: if :obj:`True`, displays the looping frequency of the 
+        Block.
+      end_delay: When all the Paths are exhausted, waits this many seconds
+        before stopping the entire script. Can be set to :obj:`None`,
         in which case the Generator won't stop the program when finishing.
-      safe_start: Ensures the first dict in ``path`` waits for at least one
-        data point from upstream blocks before sending the first value of the
-        signal. Otherwise, the first value might be sent without checking the
-        associated condition if its depends on labels from other blocks.
-
-    Note:
-      The different types of signals that can be generated by the Generator
-      can be found at `generator path`. The ``path`` list contains one dict per
-      signal shape to generate. They are generated in the order in which they
-      appear in the list.
-
-      Each dict contains information on the signal shape to generate, like its
-      type, any applicable parameter(s), and the stop condition(s). Refer to
-      the documentation of each signal shape to which information to give.
+      safe_start: Ensures the first Path waits for at least one data point from
+        upstream Blocks before sending the first value of the signal.
+        Otherwise, the first value might be sent without checking the
+        associated condition if its depends on labels from other Blocks.
+      debug: If :obj:`True`, displays all the log messages including the
+        :obj:`~logging.DEBUG` ones. If :obj:`False`, only displays the log
+        messages with :obj:`~logging.INFO` level or higher. If :obj:`None`,
+        disables logging for this Block.
     """
 
     super().__init__()
 
     # Instantiating a few attributes based on the arguments
     self.niceness = -5
     self.freq = freq
@@ -89,46 +91,40 @@
 
     self._end_delay = end_delay
     self._spam = spam
     self._safe_start = safe_start
     self._safe_started = False
 
     # The path is an iterable object
+    path = list(path)
     self._path = cycle(path) if repeat else iter(path)
 
     # More attributes
     self._ended_no_raise = False
     self._last_cmd = None
     self._last_id = None
     self._last_t = None
     self._current_path = None
     self._path_id = None
 
-  def prepare(self) -> None:
-    """Checks the validity of the provided path."""
-
     # Checking the validity of the path
-    try:
-      self._check_path_validity(iter(deepcopy(self._path)))
-    except (Exception,):
-      self.log(logging.ERROR, "Exception raised while parsing the generator "
-                              "path !")
-      raise
+    self._check_path_validity(iter(deepcopy(self._path)))
 
   def begin(self) -> None:
-    """Initializes the first path and runs a :meth:`loop`, that may be
-    blocking."""
+    """Initializes the first
+    :class:`~crappy.blocks.generator_path.meta_path.Path`."""
 
     self._update_path()
 
   def loop(self) -> None:
-    """First reads data from upstream blocks, then gets the next command to
-    send, and finally sends it to downstream blocks.
+    """First reads data from upstream Blocks, then gets the next command to
+    send, and finally sends it to downstream Blocks.
 
-    It also manages the transitions between the paths.
+    It also manages the transitions between the
+    :class:`~crappy.blocks.generator_path.meta_path.Path`.
     """
 
     # Case when the Generator shouldn't raise CrappyStop after it ended
     if self._ended_no_raise:
       return
 
     # If self start requested, do nothing until the first values are received
@@ -166,17 +162,17 @@
     if cmd != self._last_cmd or self._last_id != self._path_id or self._spam:
       self._last_cmd = cmd
       self._last_id = self._path_id
       # Actually sending the command
       self.send([self._last_t - self.t0, cmd, self._path_id])
 
   def _update_path(self) -> None:
-    """Gets the next path from the list of paths and instantiates it.
+    """Gets the next Path from the list of Paths and instantiates it.
 
-    Also manages the case when the last path of the list was reached.
+    Also manages the case when the last Path of the list was reached.
     """
 
     try:
       # Getting the next path from the list of paths
       next_path_dict = deepcopy(next(self._path))
       # Updating the path index
       if self._path_id is not None:
@@ -195,31 +191,34 @@
         raise GeneratorNoStop
 
     self.log(logging.INFO, f"Next generator path (id: {self._path_id}): "
                            f"{next_path_dict['type']}")
 
     # Instantiating the next generator path object
     path_name = next_path_dict.pop('type')
-    if path_name in paths_dict:
-      path_type = paths_dict[path_name]
-    else:
-      raise ValueError(f"No Generator path called {path_name}! The available"
-                       f" generator paths are : {tuple(paths_dict.keys())}")
+    self._check_path_exists(path_name)
+    path_type = paths_dict[path_name]
     self._current_path = path_type(
       _last_time=self._last_t if self._last_t is not None else self.t0,
       _last_cmd=self._last_cmd,
       **next_path_dict)
 
-  @staticmethod
-  def _check_path_validity(path: Iterator[Dict[str, Any]]) -> None:
-    """Simply instantiates all the paths in a row to check no error is
+  def _check_path_validity(self, path: Iterator[Dict[str, Any]]) -> None:
+    """Simply instantiates all the Paths in a row to check no error is
     raised."""
 
     for i, next_dict in enumerate(path):
       next_dict = deepcopy(next_dict)
       path_name = next_dict.pop('type')
-      if path_name in paths_dict:
-        path_type = paths_dict[path_name]
-      else:
-        raise ValueError(f"No Generator path called {path_name}! The available"
-                         f" generator paths are : {tuple(paths_dict.keys())}")
+      self._check_path_exists(path_name)
+      path_type = paths_dict[path_name]
       path_type(_last_time=0, _last_cmd=None if i == 0 else 0, **next_dict)
+
+  @staticmethod
+  def _check_path_exists(name: str) -> None:
+    """Checks that the provided Generator Path is a valid one, and raises an
+    error if not."""
+
+    if name not in paths_dict:
+      possible = ', '.join(sorted(paths_dict.keys()))
+      raise ValueError(f"Unknown Generator path type : {name} ! "
+                       f"The possible types are : {possible}")
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/generator_path/conditional.py` & `crappy-2.0.0.dev2/src/crappy/blocks/generator_path/conditional.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from typing import Union, Dict
 import logging
 
 from .meta_path import Path, ConditionType
 
 
 class Conditional(Path):
-  """Depending on two different conditions checked at each loop, this path can
-  output one between 3 constant values.
+  """This Path returns one of three possible output values, based on two given
+  conditions.
 
   It is especially useful for controlling processes that need to behave
-  differently based on given conditions, e.g. for preventing a heating element
-  from overheating or a motor from driving too far.
+  differently based on input values, e.g. for preventing a heating element
+  from overheating, or a motor from driving too far.
   """
 
   def __init__(self,
                _last_time: float,
                _last_cmd: float,
                condition1: Union[str, ConditionType],
                condition2: Union[str, ConditionType],
@@ -26,41 +26,43 @@
     """Sets the args and initializes the parent class.
 
     Args:
       _last_time: The last timestamp when a command was generated. For internal
         use only, do not overwrite.
       _last_cmd: The last sent command. For internal use only, do not
         overwrite.
-      condition1: The first condition checked by the path. Refer to
-        :ref:`Path` for more info.
+      condition1: The first condition checked by the Path. Refer to
+        :class:`~crappy.blocks.generator_path.meta_path.Path` for more
+        information.
       condition2: The second condition checked by the path. Refer to
-        :ref:`Path` for more info.
+        :class:`~crappy.blocks.generator_path.meta_path.Path` for more
+        information.
       value1: Value to send when ``condition1`` is met.
       value2: Value to send when ``condition2`` is met and ``condition1`` is
         not met.
       value0: Value to send when neither ``condition1`` nor ``condition2`` are
         met.
 
     Note:
-      This generator path never ends, it doesn't have a stop condition.
+      This Generator Path never ends, it doesn't have a stop condition.
     """
 
     super().__init__(_last_time, _last_cmd)
 
     # Setting the attributes
     self._value0 = value0
     self._value1 = value1
     self._value2 = value2
     self._condition1 = self.parse_condition(condition1)
     self._condition2 = self.parse_condition(condition2)
     self._prev = self._value0
 
   def get_cmd(self, data: Dict[str, list]) -> float:
-    """Sends either value1 if condition1 is met, or value2 if only condition2
-    is met, or value0 if none of the conditions are met."""
+    """Sends either ``value1`` if ``condition1`` is met, or ``value2`` if only
+    ``condition2`` is met, or ``value0`` if none of the conditions are met."""
 
     # Case when data has been received
     if any(data.values()):
 
       # Send value1 if the first condition is met
       if self._condition1(data):
         self.log(logging.DEBUG, "Condition 1 met")
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/generator_path/constant.py` & `crappy-2.0.0.dev2/src/crappy/blocks/generator_path/constant.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,32 +3,33 @@
 from typing import Union, Dict
 import logging
 
 from .meta_path import Path, ConditionType
 
 
 class Constant(Path):
-  """The simplest path, simply sends the same value until the condition is
-  met."""
+  """The simplest Path, outputs the same constant value until the stop 
+  condition is met."""
 
   def __init__(self,
                _last_time: float,
                _last_cmd: float,
                condition: Union[str, ConditionType],
                value: float = None) -> None:
     """Sets the args and initializes the parent class.
 
     Args:
       _last_time: The last timestamp when a command was generated. For internal
         use only, do not overwrite.
       _last_cmd: The last sent command. For internal use only, do not
         overwrite.
-      condition: The condition for switching to the next path. Refer to
-        :ref:`Path` for more info.
-      value: The value to send.
+      condition: The condition for switching to the next Path. Refer to
+        :class:`~crappy.blocks.generator_path.meta_path.Path` for more
+        information.
+      value: The value to output.
     """
 
     super().__init__(_last_time, _last_cmd)
 
     self._condition = self.parse_condition(condition)
 
     if value is None and _last_cmd is None:
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/generator_path/custom.py` & `crappy-2.0.0.dev2/src/crappy/blocks/generator_path/custom.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,39 +6,39 @@
 import pathlib
 import logging
 
 from .meta_path import Path
 
 
 class Custom(Path):
-  """Generates a custom path from a text file, until the file is exhausted.
+  """Generates a custom Path from a text file, until the file is exhausted.
 
   The file can be in any text format, including the most common `.csv` and
   `.txt` extensions.
   """
 
   def __init__(self,
                _last_time: float,
                _last_cmd: float,
                file_name: Union[str, pathlib.Path],
                delimiter: str = ',') -> None:
-    """Loads the file and sets the args.
+    """Loads the file and sets the arguments.
 
     The stop condition is simply to reach the last timestamp given in the
     file.
 
     Args:
       _last_time: The last timestamp when a command was generated. For internal
         use only, do not overwrite.
       _last_cmd: The last sent command. For internal use only, do not
         overwrite.
-      file_name: Path to the file to read the path from. Can be either a
-        :obj:`str` or a :mod:`pathlib` Path. The file must contain two columns:
-        the first one containing timestamps (starting from 0), the other one
-        containing the values.
+      file_name: Path to the file containing the information on the Generator
+        Path. Can be either a :obj:`str` or a :obj:`pathlib.Path`. The file
+        must contain two columns: the first one containing timestamps (starting
+        from 0), the other one containing the values.
       delimiter: The delimiter between columns in the file, usually a coma.
     """
 
     super().__init__(_last_time, _last_cmd)
 
     self.log(logging.DEBUG, f"Extracting data from file {file_name}")
     array = loadtxt(pathlib.Path(file_name), delimiter=delimiter)
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/generator_path/cyclic.py` & `crappy-2.0.0.dev2/src/crappy/blocks/generator_path/cyclic.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,58 +5,61 @@
 from itertools import cycle, islice
 import logging
 
 from .meta_path import Path, ConditionType
 
 
 class Cyclic(Path):
-  """The path cyclically alternates between two constant values, based on two
+  """This Path cyclically alternates between two constant values, based on two
   different conditions.
 
   It can for example be used as a trigger, or used to drive an actuator
-  cyclically. It is equivalent to a succession of :ref:`constant` paths.
+  cyclically. It is equivalent to a succession of 
+  :class:`~crappy.blocks.generator_path.Constant` Paths.
   """
 
   def __init__(self,
                _last_time: float,
                _last_cmd: float,
                condition1: Union[str, ConditionType],
                condition2: Union[str, ConditionType],
                value1: float,
                value2: float,
                cycles: float = 1) -> None:
-    """Sets the args and initializes the parent class.
+    """Sets the arguments and initializes the parent class.
 
-    The path always starts with ``value1``, and then switches to ``value2``.
+    The Path always starts with ``value1``, and then switches to ``value2``.
 
     Args:
       _last_time: The last timestamp when a command was generated. For internal
         use only, do not overwrite.
       _last_cmd: The last sent command. For internal use only, do not
         overwrite.
       condition1: The condition for switching to ``value2``. Refer to
-        :ref:`Path` for more info.
+        :class:`~crappy.blocks.generator_path.meta_path.Path` for more
+        information.
       condition2: The condition for switching to ``value1``. Refer to
-        :ref:`Path` for more info.
+        :class:`~crappy.blocks.generator_path.meta_path.Path` for more
+        information.
       value1: First value to send.
       value2: Second value to send.
       cycles: Number of cycles. Half cycles are accepted. If `0`, loops
         forever.
 
     Note:
       ::
 
-        [{'type': 'cyclic', 'value1': 1, 'condition1': 'AIN0>2',
+        [{'type': 'Cyclic', 'value1': 1, 'condition1': 'AIN0>2',
         'value2': 0, 'condition2': 'AIN1<1', 'cycles': 5}]
 
       is equivalent to
       ::
 
-        [{'type': 'constant', 'value': 1,'condition': 'AIN0>2'},
-        {'type': 'constant', 'value': 0, 'condition': 'AIN1<1'}] * 5
+        [{'type': 'Constant', 'value': 1,'condition': 'AIN0>2'},
+        {'type': 'Constant', 'value': 0, 'condition': 'AIN1<1'}] * 5
     """
 
     super().__init__(_last_time, _last_cmd)
 
     # Creates an interator object with a given length
     if cycles > 0:
       cycles = int(2 * cycles)
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/generator_path/cyclic_ramp.py` & `crappy-2.0.0.dev2/src/crappy/blocks/generator_path/cyclic_ramp.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,61 +5,64 @@
 from itertools import cycle, islice
 import logging
 
 from .meta_path import Path, ConditionType
 
 
 class CyclicRamp(Path):
-  """The path cyclically alternates between two ramps with different slopes,
+  """This Pth cyclically alternates between two ramps with different slopes,
   based on two different conditions.
 
-  It is equivalent to a succession of :ref:`ramp` paths.
+  It is equivalent to a succession of 
+  :class:`~crappy.blocks.generator_path.Ramp` Paths.
   """
 
   def __init__(self,
                _last_time: float,
                _last_cmd: float,
                condition1: Union[str, ConditionType],
                condition2: Union[str, ConditionType],
                speed1: float,
                speed2: float,
                cycles: float = 1,
                init_value: Optional[float] = None) -> None:
-    """Sets the args and initializes the parent class.
+    """Sets the arguments and initializes the parent class.
 
     The path always starts with ``speed1``, and then switches to ``speed2``.
 
     Args:
       _last_time: The last timestamp when a command was generated. For internal
         use only, do not overwrite.
       _last_cmd: The last sent command. For internal use only, do not
         overwrite.
       condition1: The condition for switching to ``speed2``. Refer to
-        :ref:`Path` for more info.
+        :class:`~crappy.blocks.generator_path.meta_path.Path` for more
+        information.
       condition2: The condition for switching to ``speed1``. Refer to
-        :ref:`Path` for more info.
+        :class:`~crappy.blocks.generator_path.meta_path.Path` for more
+        information.
       speed1: Slope of the first generated ramp, in `units/s`.
       speed2: Slope of the second generated ramp, in `units/s`.
       cycles: Number of cycles. Half cycles are accepted. If `0`, loops
         forever.
       init_value: If given, overwrites the last value of the signal as the
-        starting point for the first ramp. In the specific case when this path
-        is the first one in the list of dicts, this argument must be given !
+        starting point for the first ramp. In the specific case when this Path
+        is the first one in the Generator Paths, this argument must be given !
 
     Note:
       ::
 
-        [{'type': 'cyclic_ramp', 'speed1': 5, 'condition1': 'AIN0>2',
+        [{'type': 'CyclicRamp', 'speed1': 5, 'condition1': 'AIN0>2',
         'speed2': -2, 'condition2': 'AIN1<1', 'cycles': 5}]
 
       is equivalent to
       ::
 
-        [{'type': 'ramp', 'speed': 5,'condition': 'AIN0>2'},
-        {'type': 'ramp', 'value': -2, 'condition': 'AIN1<1'}] * 5
+        [{'type': 'Ramp', 'speed': 5,'condition': 'AIN0>2'},
+        {'type': 'Ramp', 'value': -2, 'condition': 'AIN1<1'}] * 5
     """
 
     super().__init__(_last_time, _last_cmd)
 
     if init_value is None and _last_cmd is None:
       raise ValueError('For the first path, an init_value must be given !')
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/generator_path/integrator.py` & `crappy-2.0.0.dev2/src/crappy/blocks/generator_path/integrator.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,52 +4,50 @@
 from typing import Union, Dict
 import logging
 
 from .meta_path import Path, ConditionType
 
 
 class Integrator(Path):
-  """This path integrates an incoming label over time and returns the
+  """This Path integrates an incoming label over time and returns the
   integration as an output signal.
 
   Let `f(t)` be the input signal, `v(t)` the value of the output, `m` the
-  inertia and `t0` the timestamp of the beginning of this path.
-
-  Then the output value for this path will be:
-  ::
-
-    v(t) = v(t0) - [I(t0 -> t)f(t)dt] / m
+  inertia and `t0` the timestamp of the beginning of this Path.
 
+  Then the output value for this Path will be
+  :math:`v(t) = v(t0) - [I(t0 -> t)f(t)dt] / m`.
   """
 
   def __init__(self,
                _last_time: float,
                _last_cmd: float,
                condition: Union[str, ConditionType],
                inertia: float,
                func_label: str,
                time_label: str = 't(s)',
                init_value: float = None) -> None:
-    """Sets the args and initializes the parent class.
+    """Sets the arguments and initializes the parent class.
 
     Args:
       _last_time: The last timestamp when a command was generated. For internal
         use only, do not overwrite.
       _last_cmd: The last sent command. For internal use only, do not
         overwrite.
-      condition: The condition for switching to the next path. Refer to
-        :ref:`Path` for more info.
+      condition: The condition for switching to the next Path. Refer to
+        :class:`~crappy.blocks.generator_path.meta_path.Path` for more
+        information.
       inertia: Value of the equivalent inertia to use for driving the signal.
         In the above formula, it is the value of `m`. The larger this value,
         the slower the changes in the signal value.
       func_label: The name of the label of the input value to integrate.
       time_label: The name of the time label for the integration.
       init_value: If given, overwrites the last value of the signal as the
         starting point for the inertia path. In the specific case when this
-        path is the first one in the list of dicts, this argument must be
+        path is the first one in the Generator Paths, this argument must be
         given !
     """
 
     super().__init__(_last_time, _last_cmd)
 
     if init_value is None and _last_cmd is None:
       raise ValueError('For the first path, an init_value must be given !')
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/generator_path/meta_path/meta_path.py` & `crappy-2.0.0.dev2/src/crappy/modifier/meta_modifier/meta_modifier.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # coding: utf-8
 
-from ...._global import DefinitionError
+from ..._global import DefinitionError
 
 
-class MetaPath(type):
-  """"""
+class MetaModifier(type):
+  """Metaclass keeping track of all the Modifiers, including the custom
+  user-defined ones."""
 
-  classes = dict()
+  classes = {}
 
   def __new__(mcs, name: str, bases: tuple, dct: dict) -> type:
     return super().__new__(mcs, name, bases, dct)
 
   def __init__(cls, name: str, bases: tuple, dct: dict) -> None:
     super().__init__(name, bases, dct)
 
-    # Checking that a Path with the same name doesn't already exist
+    # Checking that a Modifier with the same name doesn't already exist
     if name in cls.classes:
-      raise DefinitionError(f"The {name} Generator Path is already defined !")
+      raise DefinitionError(f"The {name} class is already defined !")
 
-    # Saving the name
+    # Otherwise, saving the class
     cls.classes[name] = cls
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/generator_path/ramp.py` & `crappy-2.0.0.dev2/src/crappy/blocks/generator_path/ramp.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,27 +13,28 @@
 
   def __init__(self,
                _last_time: float,
                _last_cmd: float,
                condition: Union[str, ConditionType],
                speed: float,
                init_value: Optional[float] = None):
-    """Sets the args and initializes the parent class.
+    """Sets the arguments and initializes the parent class.
 
     Args:
       _last_time: The last timestamp when a command was generated. For internal
         use only, do not overwrite.
       _last_cmd: The last sent command. For internal use only, do not
         overwrite.
-      condition: The condition for switching to the next path. Refer to
-        :ref:`Path` for more info.
+      condition: The condition for switching to the next Path. Refer to
+        :class:`~crappy.blocks.generator_path.meta_path.Path` for more
+        information.
       speed: The slope of the ramp, in `units/s`.
       init_value: If given, overwrites the last value of the signal as the
         starting point for the ramp. In the specific case when this path is the
-        first one in the list of dicts, this argument must be given !
+        first one in the Generator Paths, this argument must be given !
     """
 
     super().__init__(_last_time, _last_cmd)
 
     if init_value is None and _last_cmd is None:
       raise ValueError('For the first path, an init_value must be given !')
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/generator_path/sine.py` & `crappy-2.0.0.dev2/src/crappy/blocks/generator_path/sine.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,34 +5,35 @@
 from typing import Union, Dict
 import logging
 
 from .meta_path import Path, ConditionType
 
 
 class Sine(Path):
-  """This path generates a sine wave varying with time until the stop condition
+  """This Path generates a sine wave varying with time until the stop condition
   is met."""
 
   def __init__(self,
                _last_time: float,
                _last_cmd: float,
                condition: Union[str, ConditionType],
                freq: float,
                amplitude: float,
                offset: float = 0,
                phase: float = 0) -> None:
-    """Sets the args and initializes the parent class.
+    """Sets the arguments and initializes the parent class.
 
     Args:
       _last_time: The last timestamp when a command was generated. For internal
         use only, do not overwrite.
       _last_cmd: The last sent command. For internal use only, do not
         overwrite.
-      condition: The condition for switching to the next path. Refer to
-        :ref:`Path` for more info.
+      condition: The condition for switching to the next Path. Refer to
+        :class:`~crappy.blocks.generator_path.meta_path.Path` for more
+        information.
       freq: The frequency of the sine in `Hz`.
       amplitude: The amplitude of the sine wave (peak to peak).
       offset: The offset of the sine (average value).
       phase: The phase of the sine (in radians).
     """
 
     super().__init__(_last_time, _last_cmd)
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/grapher.py` & `crappy-2.0.0.dev2/src/crappy/blocks/grapher.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,73 +5,83 @@
 import logging
 from _tkinter import TclError
 
 from .meta_block import Block
 from .._global import OptionalModule
 
 plt = OptionalModule('matplotlib.pyplot', lazy_import=True)
-wdg = OptionalModule('matplotlib.widgets', lazy_import=True)
 
 
 class Grapher(Block):
-  """The grapher receive data from a block and plots it.
-
-  Multiple curves can be plotted on a same graph, and the data can come from
-  different blocks.
-
-  Note:
-    To reduce the memory and CPU usage of graphs, try lowering the ``maxpt``
-    parameter (2-3000 is already enough to follow a short test), or set the
-    ``length`` parameter to a non-zero value (again, 2-3000 is fine). Lowering
-    the ``freq`` is also a good option to limit the CPU use.
+  """This Block can display data in a 2D graph in a persistent way.
+  
+  The graph is displayed in an independent window. It iis updated each time new
+  data is received from upstream Blocks. The displayed data can come from 
+  different Blocks.
+  
+  The user can choose which labels are plotted on the `x` and `y` axes. It is
+  therefore possible to plot a label versus time, or a label versus another 
+  label. A single graph is displayed, but multiple curves can be plotted on
+  this graph.
+  
+  The Grapher Block is known for being very CPU-intensive. For displaying only 
+  the last values of given labels, the :class:`~crappy.blocks.LinkReader` and 
+  :class:`~crappy.blocks.Dashboard` Blocks are simpler solutions that go much
+  easier on the CPU. 
   """
 
   def __init__(self,
                *labels: Tuple[str, str],
                length: int = 0,
-               freq: float = 2,
+               freq: Optional[float] = 2,
                max_pt: int = 20000,
                window_size: Tuple[int, int] = (8, 8),
                window_pos: Optional[Tuple[int, int]] = None,
                interp: bool = True,
                backend: str = "TkAgg",
                display_freq: bool = False,
                debug: Optional[bool] = False) -> None:
-    """Sets the args and initializes the parent class.
+    """Sets the arguments and initializes the parent class.
 
     Args:
       *labels: Each :obj:`tuple` corresponds to a curve to plot, and should
-        contain two values: the first will be the label of the `x`values, the
+        contain two values: the first will be the label of the `x` values, the
         second the label of the `y` values. There's no limit to the number of
         curves. Note that all the curves are displayed in a same graph.
       length: If `0` the graph is static and displays all data from the start
-        of the assay. Else only displays the last ``length`` received chunks,
+        of the assay. Else, only displays the last ``length`` received chunks,
         and drops the previous ones.
-      freq: The refresh rate of the graph. May cause high CPU use if set too
-        high.
+      freq: The target looping frequency for the Block. If :obj:`None`, loops 
+        as fast as possible.
       max_pt: The maximum number of points displayed on the graph. When
-        reaching this limit, the block deletes one point out of two to avoid
-        using too  much memory and CPU.
+        reaching this limit, the Block deletes one point out of two to avoid
+        using too much memory and CPU.
       window_size: The size of the graph, in inches.
       window_pos: The position of the graph in pixels. The first value is for
         the `x` direction, the second for the `y` direction. The origin is the
         top-left corner. Works with multiple screens.
       interp: If :obj:`True`, the data points are linked together by straight
         lines. Else, only the points are displayed.
       backend: The :mod:`matplotlib` backend to use. Performance may vary
         according to the chosen backend. Also, every backend may not be
         available depending on your machine.
-      display_freq: To display the loop frequency of the block.
+      display_freq: if :obj:`True`, displays the looping frequency of the
+        Block.
+      debug: If :obj:`True`, displays all the log messages including the
+        :obj:`~logging.DEBUG` ones. If :obj:`False`, only displays the log
+        messages with :obj:`~logging.INFO` level or higher. If :obj:`None`,
+        disables logging for this Block.
 
     Example:
       ::
 
         graph = Grapher(('t(s)', 'F(N)'), ('t(s)', 'def(%)'))
 
-      will plot a dynamic graph with two lines plot (`F=f(t)` and `def=f(t)`).
+      will plot a dynamic graph with two lines plot (:math:`F=f(t)` and
+      :math:`def=f(t)`).
       ::
 
         graph = Grapher(('def(%)', 'F(N)'), length=0)
 
       will plot a static graph.
       ::
 
@@ -111,14 +121,17 @@
       self.log(logging.INFO, f"Setting matplotlib backend to {self._backend}")
       plt.switch_backend(self._backend)
 
     # Create the figure and the subplot
     self._figure = plt.figure(figsize=self._window_size)
     self._canvas = self._figure.canvas
     self._ax = self._figure.add_subplot(111)
+    self._figure.canvas.mpl_connect('key_press_event', self._on_press)
+    self._ax.set_title('(Press c to clear the graph)',
+                       fontsize='small', loc='right')
 
     # Add the lines or the dots
     self._lines = []
     for _ in self._labels:
       if self._interp:
         self._lines.append(self._ax.plot([], [])[0])
       else:
@@ -135,25 +148,22 @@
                ncol=len(legend), mode="expand", borderaxespad=1)
     plt.xlabel(self._labels[0][0])
     plt.ylabel(self._labels[0][1])
 
     # Add a grid
     plt.grid()
 
-    # Adds a button for clearing the graph
-    self._clear_button = wdg.Button(plt.axes([.8, .02, .15, .05]), 'Clear')
-    self._clear_button.on_clicked(self._clear)
-
     # Set the dimensions if required
     if self._window_pos:
       mng = plt.get_current_fig_manager()
       mng.window.wm_geometry("+%s+%s" % self._window_pos)
 
     # Ready to show the window
     self.log(logging.INFO, "Configured the matplotlib window, displaying it")
+    plt.tight_layout()
     plt.show(block=False)
     plt.pause(.001)
 
   def loop(self) -> None:
     """Receives the upcoming data, puts in the display buffer and updates the
     graph."""
 
@@ -220,22 +230,26 @@
       try:
         self._canvas.draw()
       except TclError:
         pass
       self._canvas.flush_events()
 
   def finish(self) -> None:
-    """Closes all the opened Matplotlib windows."""
+    """Closes all the opened :mod:`matplotlib` windows."""
 
     self.log(logging.INFO, "Closing all matplotlib windows")
     plt.close("all")
 
-  def _clear(self, *_, **__) -> None:
-    """Resets the display by emptying the data buffers."""
-    
-    for line in self._lines:
-      line.set_xdata([])
-      line.set_ydata([])
-    self.factor = [1 for _ in self._labels]
-    self.counter = [0 for _ in self._labels]
+  def _on_press(self, event) -> None:
+    """Callback catching the keyboard press events.
+
+    When called, resets the display by emptying the data buffers.
+    """
+
+    if event.key == 'c':
+      for line in self._lines:
+        line.set_xdata([])
+        line.set_ydata([])
+      self.factor = [1 for _ in self._labels]
+      self.counter = [0 for _ in self._labels]
 
-    self.log(logging.INFO, "Cleared the matplotlib window")
+      self.log(logging.INFO, "Cleared the matplotlib window")
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/hdf_recorder.py` & `crappy-2.0.0.dev2/src/crappy/blocks/hdf_recorder.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,53 +12,63 @@
   import tables
 except ModuleNotFoundError:
   tables = OptionalModule("tables", "HDFRecorder needs the tables module to "
                           "write hdf files.")
 
 
 class HDFRecorder(Block):
-  """This block saves data efficiently into a hdf5 file.
-
-  This block is meant to save data coming as arrays at a high rate
-  (`>1kHz`). It relies on the module :mod:`tables`.
-
-  Important:
-    Do not forget to specify the type of data to be saved (see ``atom``
-    parameter) to avoid casting the data into another type, as this could
-    result in data loss or inefficient saving.
+  """This Block records data efficiently into a HDF5 file.
+  
+  It expects data as :obj:`numpy.array` from exactly one upstream Block, that
+  should be an :class:`~crappy.blocks.IOBlock` in `streamer` mode. It then 
+  saves this data in a HDF5 file using the :mod:`tables` module.
+  
+  This Block is intended for high-speed data recording from 
+  :class:`~crappy.inout.InOut` in `streamer` mode. For regular data recording,
+  the :class:`~crappy.blocks.Recorder` Block should be used instead.
+  
+  Warning:
+    Corrupted HDF5 files are not readable at all ! If anything goes wrong 
+    during a test, especially during the finish phase, it is not guaranteed 
+    that the recorded data will be readable.
   """
 
   def __init__(self,
                filename: Union[str, Path],
                node: str = 'table',
                expected_rows: int = 10**8,
                atom=None,
                label: str = 'stream',
                metadata: Optional[dict] = None,
                freq: Optional[float] = None,
                display_freq: bool = False,
                debug: Optional[bool] = False) -> None:
-    """Sets the args and initializes the parent class.
+    """Sets the arguments and initializes the parent class.
 
     Args:
       filename: Path to the output file, either relative or absolute. If the
         parent folders of the file do not exist, they will be created. If the
         file already exists, the actual file where data will be written will be
         renamed with a trailing index to avoid overriding it.
       expected_rows: The number of expected rows in the file. It is used to
         optimize the dumping.
       atom: This represents the type of data to be stored in the table. It can
-        be given as a :class:`tables.Atom` instance, as a :class:`numpy.array`
+        be given as a :obj:`tables.Atom` instance, as a :obj:`numpy.array`
         or as a :obj:`str`.
       label: The label carrying the data to be saved
       metadata: A :obj:`dict` containing additional information to save in the
-        `hdf5` file.
-      freq: The block will try to loop at this frequency.
-      display_freq: If :obj:`True`, displays the looping frequency of the
-        block.
+        `HDF5` file.
+      freq: The target looping frequency for the Block. If :obj:`None`, loops 
+        as fast as possible.
+      display_freq: if :obj:`True`, displays the looping frequency of the 
+        Block.
+      debug: If :obj:`True`, displays all the log messages including the
+        :obj:`~logging.DEBUG` ones. If :obj:`False`, only displays the log
+        messages with :obj:`~logging.INFO` level or higher. If :obj:`None`,
+        disables logging for this Block.
     """
 
     self._hfile = None
 
     super().__init__()
     self.freq = freq
     self.display_freq = display_freq
@@ -75,15 +85,15 @@
       self._atom = tables.Atom.from_dtype(np.dtype(atom))
     else:
       self._atom = atom
 
     self._array_initialized = False
 
   def prepare(self) -> None:
-    """Checking that the block has the right number of inputs, creates the
+    """Checks that the Block has the right number of inputs, creates the
     folder containing the file if it doesn't already exist, changes the name of
     the file if it already exists, and initializes the HDF file."""
 
     # Making sure there's the right number of incoming links
     if not self.inputs:
       raise ValueError('The HDF Recorder block does not have inputs !')
     elif len(self.inputs) > 1:
@@ -113,15 +123,15 @@
     # Initializing the file to save data to
     self.log(logging.INFO, "Initializing the HDF5 file")
     self._hfile = tables.open_file(str(self._path), "w")
     for name, value in self._metadata.items():
       self._hfile.create_array(self._hfile.root, name, value)
 
   def loop(self) -> None:
-    """Simply receives data from the upstream block and saves it.
+    """Receives data from the upstream Block and saves it.
 
     Also creates the array for recording data when the first values are
     received.
     """
 
     # Do nothing until the first value to save are received
     if not self._array_initialized:
@@ -134,15 +144,15 @@
     data = self.recv_all_data()
 
     if self._label in data:
       for elt in data[self._label]:
         self._array.append(elt)
 
   def finish(self) -> None:
-    """Simply closes the HDF file."""
+    """Closes the HDF file."""
 
     if self._hfile is not None:
       self.log(logging.INFO, "Closing the HDF5 file")
       self._hfile.close()
 
   def _first_loop(self) -> None:
     """Initializes the array for saving data."""
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/ioblock.py` & `crappy-2.0.0.dev2/src/crappy/blocks/ioblock.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,85 +1,104 @@
 # coding: utf-8
 
-from typing import Union, List, Optional
+from typing import Union, Optional, Iterable, Any
 import logging
 
 from .meta_block import Block
 from ..inout import inout_dict, InOut
 from ..tool.ft232h import USBServer
 
 
 class IOBlock(Block):
-  """This block is meant to drive :ref:`In / Out` objects. It can acquire data,
-  and/or set commands. One IOBlock can only drive a single InOut.
+  """This Block is meant to drive :class:`~crappy.inout.InOut` objects. It can
+  acquire data, and/or set commands. One IOBlock can only drive a single InOut.
 
-  If it has incoming links, it will set the commands received over the labels
-  given in ``cmd_labels``. Additional commands to set at the very beginning or
-  the very end of the test can also be specified.
-
-  If it has outgoing links, it will acquire data and send it downstream over
-  the labels given in ``labels``. It is possible to trigger the acquisition
-  using a predefined label.
+  If it has incoming :class:`~crappy.links.Link`, it will set the commands 
+  received over the labels given in ``cmd_labels`` by calling the 
+  :meth:`~crappy.inout.InOut.set_cmd` method of the InOut. Additional commands 
+  to set at the very beginning or the very end of the test can also be 
+  specified.
+
+  If it has outgoing :class:`~crappy.links.Link`, it will acquire data using 
+  the :meth:`~crappy.inout.InOut.get_data` method of the InOut and send it
+  downstream over the labels given in ``labels``. It is possible to trigger the
+  acquisition using a predefined label.
+
+  The ``streamer`` argument allows using the "streamer" mode of InOuts
+  supporting it, instead of the regular acquisition mode. Finally, the
+  ``make_zero_delay`` argument allows offsetting the acquired values to zero at
+  the beginning of the test. Refer to the documentation of each argument for a
+  more detailed description.
   """
 
   def __init__(self,
                name: str,
-               labels: Optional[List[str]] = None,
-               cmd_labels: Optional[List[str]] = None,
+               labels: Optional[Union[str, Iterable[str]]] = None,
+               cmd_labels: Optional[Union[str, Iterable[str]]] = None,
                trigger_label: Optional[str] = None,
                streamer: bool = False,
-               initial_cmd: Optional[Union[list]] = None,
-               exit_cmd: Optional[list] = None,
+               initial_cmd: Optional[Union[Any, Iterable[Any]]] = None,
+               exit_cmd: Optional[Union[Any, Iterable[Any]]] = None,
                make_zero_delay: Optional[float] = None,
                ft232h_ser_num: Optional[str] = None,
                spam: bool = False,
                freq: Optional[float] = 200,
                display_freq: bool = False,
                debug: Optional[bool] = False,
                **kwargs) -> None:
-    """Sets the args and initializes the parent class.
+    """Sets the arguments and initializes the parent class.
 
     Args:
-      name: The name of the :ref:`In / Out` class to instantiate.
-      labels: A :obj:`list` containing the output labels for InOuts that
-        acquire data. They correspond to the values returned by the InOut's
-        :meth:`get_data` method, so there should be as many labels as values
-        returned, and given in the appropriate order. The first label must
-        always be the timestamp, preferably called ``'t(s)'``. This argument
-        can be omitted if :meth:`get_data` returns a :obj:`dict` instead of a
-        :obj:`list`. Ignored if the block has no output link.
-      cmd_labels: A :obj:`list` of the labels considered as inputs for this
-        block, for InOuts that set commands. The values received from these
-        labels will be passed to the InOut's :meth:`set_cmd` method, in the
-        same order as the labels are given. Usually, time is not part of the
-        cmd_labels. Ignored if the block has no input link.
-      trigger_label: If given, the block will only read data whenever a value
-        (can be any value) is received on this label. Ignored if the block has
-        no output link. A trigger label can also be a cmd label.
-      streamer: If :obj:`False`, the :meth:`get_data` method of the InOut
-        object is called for acquiring data, else it's the :meth:`get_stream`
-        method.
+      name: The name of the :class:`~crappy.inout.InOut` class to instantiate.
+      labels: An iterable (e.g. a :obj:`list` or a :obj:`tuple`) containing the
+        output labels for InOuts that acquire data. They correspond to the
+        values returned by the InOut's :meth:`~crappy.inout.InOut.get_data`
+        method, so there should be as many labels as returned values, and given
+        in the appropriate order. The first label must always be the time
+        label, preferably called ``'t(s)'``. This argument can be omitted if
+        :meth:`~crappy.inout.InOut.get_data` returns a :obj:`dict`. Ignored if
+        the Block has no output Link.
+      cmd_labels: An iterable (e.g. a :obj:`list` or a :obj:`tuple`) containing
+        the labels considered as inputs of this Block, for InOuts that set
+        commands. The values received from these labels will be passed to the
+        InOut's :meth:`~crappy.inout.InOut.set_cmd` method, in the same order
+        as the labels are given. Usually, time is not part of the
+        ``cmd_labels``. Ignored if the Block has no input Link.
+      trigger_label: If given, the Block will only read data whenever a value
+        is received on this label (can be any value). Ignored if the Block has
+        no output Link. A trigger label can also be a cmd label.
+      streamer: If :obj:`False`, the :meth:`~crappy.inout.InOut.get_data`
+        method of the InOut is called for acquiring data, else it is the
+        :meth:`~crappy.inout.InOut.get_stream` method. Refer to the
+        documentation of these methods for more information.
       initial_cmd: An initial command for the InOut, set during
         :meth:`prepare`. If given, there must be as many values as in
-        cmd_labels.
-      exit_cmd: A final command for the InOut, set during :obj:`finish`. If
-        given, there must be as many values as in cmd_labels.
+        ``cmd_labels``. Must be given as an iterable (e.g. a :obj:`list` or a
+        :obj:`tuple`).
+      exit_cmd: A final command for the InOut, set during :meth:`finish`. If
+        given, there must be as many values as in ``cmd_labels``. Must be given
+        as an iterable (e.g. a :obj:`list` or a :obj:`tuple`).
       make_zero_delay: If set, will acquire data before the beginning of the
         test and use it to offset all the labels to zero. The data will be
-        acquired during the given number of seconds. Ignored if the block has
-        no output links.
-      spam: If :obj:`False`, the block will call :meth:`set_cmd` on the
-        InOut object only if the current command is different from the
-        previous. Otherwise, it will call the method each time a command is
-        received.
-      freq: The block will try to loop as this frequency, or as fast as
-        possible if no value is given.
+        acquired during the given number of seconds. Ignored if the Block has
+        no output Links. Does not work for InOuts that acquire values other
+        than numbers (:obj:`str` for example).
+      spam: If :obj:`False`, the Block will call
+        :meth:`~crappy.inout.InOut.set_cmd` on the InOut object only if the
+        current command is different from the previous. Otherwise, it will call
+        the method each time a command is received.
+      freq: The target looping frequency for the Block. If :obj:`None`, loops 
+        as fast as possible.
       display_freq: If :obj:`True`, displays the looping frequency of the
-        block.
-      **kwargs: The arguments to be passed to the :ref:`In / Out` class.
+        Block while running.
+      debug: If :obj:`True`, displays all the log messages including the
+        :obj:`~logging.DEBUG` ones. If :obj:`False`, only displays the log
+        messages with :obj:`~logging.INFO` level or higher. If :obj:`None`,
+        disables logging for this Block.
+      **kwargs: The arguments to be passed to the :class:`~crappy.inout.InOut`.
     """
 
     self._device: Optional[InOut] = None
     self._ft232h_args = None
     self._read: bool = False
     self._write: bool = False
 
@@ -88,35 +107,65 @@
     self.freq = freq
     self.display_freq = display_freq
     self.debug = debug
 
     # The label argument can be omitted for streaming
     if labels is None and streamer:
       self.labels = ['t(s)', 'stream']
+    # Forcing the labels into a list
+    elif labels is not None and isinstance(labels, str):
+      self.labels = [labels]
+    elif labels is not None:
+      self.labels = list(labels)
     else:
-      self.labels = labels
+      self.labels = None
 
-    # The labels to get
-    self._cmd_labels = cmd_labels
-    self._trig_label = trigger_label
+    # Forcing the cmd_labels into a list or None
+    if cmd_labels is not None and isinstance(cmd_labels, str):
+      self._cmd_labels = [cmd_labels]
+    elif cmd_labels is not None:
+      self._cmd_labels = list(cmd_labels)
+    else:
+      self._cmd_labels = None
+
+    # Forcing the initial_cmd into a list
+    if initial_cmd is not None and isinstance(initial_cmd, str):
+      self._initial_cmd = [initial_cmd]
+    elif initial_cmd is not None:
+      self._initial_cmd = list(initial_cmd)
+    else:
+      self._initial_cmd = None
+
+    # Forcing the exit_cmd into a list
+    if exit_cmd is not None and isinstance(exit_cmd, str):
+      self._exit_cmd = [exit_cmd]
+    elif exit_cmd is not None:
+      self._exit_cmd = list(exit_cmd)
+    else:
+      self._exit_cmd = None
 
     # Checking that the initial_cmd and exit_cmd length are consistent
-    if cmd_labels is not None:
-      if initial_cmd is not None and len(initial_cmd) != len(cmd_labels):
+    if self._cmd_labels is not None:
+      if self._initial_cmd is not None \
+          and len(self._initial_cmd) != len(self._cmd_labels):
         raise ValueError("There should be as many values in initial_cmd as "
                          "there are in cmd_labels !")
-      if exit_cmd is not None and len(exit_cmd) != len(cmd_labels):
+      if self._exit_cmd is not None \
+          and len(self._exit_cmd) != len(self._cmd_labels):
         raise ValueError("There should be as many values in exit_cmd as "
                          "there are in cmd_labels !")
 
-    self._initial_cmd = initial_cmd
-    self._exit_cmd = exit_cmd
+    self._trig_label = trigger_label
 
+    # Checking that all the given actuators are valid
     if name not in inout_dict:
-      raise ValueError(f"No InOut object called {name} !")
+      possible = ', '.join(sorted(inout_dict.keys()))
+      raise ValueError(f"Unknown InOut type : {name} ! "
+                       f"The possible types are : {possible}")
+
     self._io_name = name
     self._inout_kwargs = kwargs
 
     self._streamer = streamer
     self._spam = spam
     self._make_zero_delay = make_zero_delay
 
@@ -125,16 +174,20 @@
     self._prev_values = dict()
 
     # Checking whether the InOut communicates through an FT232H
     if inout_dict[self._io_name].ft232h:
       self._ft232h_args = USBServer.register(ft232h_ser_num)
 
   def prepare(self) -> None:
-    """Checks the consistency of the link layout, opens the device and sets the
-    initial command if required."""
+    """Checks the consistency of the Link layout, opens the InOut and sets the
+    initial command if required.
+
+    This method mainly calls the :meth:`~crappy.inout.InOut.open` method of the
+    driven InOut.
+    """
 
     # Instantiating the device in a regular way
     if self._ft232h_args is None:
       self._device = inout_dict[self._io_name](**self._inout_kwargs)
     # Instantiating the device and the connection to the FT232H
     else:
       self.log(logging.INFO, "The InOut to open communicates over an FT232H")
@@ -169,19 +222,30 @@
       self.log(logging.INFO, f"Sending the initial command to the "
                              f"{type(self._device).__name__} InOut")
       self._device.set_cmd(*self._initial_cmd)
       self._last_cmd = self._initial_cmd
       self._prev_values.update(zip(self._cmd_labels, self._initial_cmd))
 
   def loop(self) -> None:
-    """Gets the latest command, reads data from the device and sets the
-    command.
+    """Reads data from the InOut and/or sets the received commands.
 
-    Also handles the trig label if one was given, and manages the buffer for
-    the previously received commands.
+    Data is read from the InOut **only** if this Block has outgoing Links. If
+    the ``trigger_label`` is given, data is read only if a trigger is received
+    over the given trigger label.
+
+    A command is set on the InOut **only** if this Block has incoming Links,
+    and if data is received over these Links. Depending on the value of the
+    ``spam`` argument, a command might not be set if it is similar to the
+    previous one.
+
+    The data is read from the InOut either by calling its
+    :meth:`~crappy.inout.InOut.return_data` or its
+    :meth:`~crappy.inout.InOut.return_stream` method, depending if the
+    ``streamer`` argument is :obj:`True` of :obj:`False`. The commands are
+    always set by calling the :meth:`~crappy.inout.InOut.set_cmd` method.
     """
 
     # Receiving all the latest data waiting in the links
     data = self.recv_last_data(fill_missing=False)
 
     # Reading data from the device if there's no trig_label or if data has been
     # received on this trig_label
@@ -199,34 +263,40 @@
     if self._write:
       # The missing values are completed here, because the trig label must not
       # be artificially created
       self._prev_values.update(data)
       data.update(self._prev_values)
 
       # Keeping only the labels in cmd_labels
-      cmd = [val for label, val in data.items()
-             if label in self._cmd_labels]
+      data = {key: val for key, val in data.items() if key in self._cmd_labels}
 
       # If not all cmd_labels have a value, returning without calling set_cmd
-      if len(cmd) != len(self._cmd_labels):
+      if len(data) != len(self._cmd_labels):
         self.log(logging.WARNING, f"Not enough values received in the "
                                   f"{type(self._device).__name__} InOut to"
                                   f" set the cmd, cmd not set !")
         return
 
+      # Grouping the command values in a list before passing them to set_cmd
+      cmd = [data[label] for label in self._cmd_labels]
+
       # Setting the command if it's different from the previous or spam is True
       if cmd != self._last_cmd or self._spam:
         self.log(logging.DEBUG, f"Writing the command {cmd} to the "
                                 f"{type(self._device).__name__} InOut")
         self._device.set_cmd(*cmd)
         self._last_cmd = cmd
 
   def finish(self) -> None:
     """Stops the stream, sets the exit command if necessary, and closes the
-    device."""
+    InOut.
+
+    This method mainly calls the :meth:`~crappy.inout.InOut.close` method of
+    the driven InOut.
+    """
 
     # Stopping the stream
     if self._streamer and self._device is not None:
       self.log(logging.INFO, f"Stopping stream on the "
                              f"{type(self._device).__name__} InOut")
       self._device.stop_stream()
 
@@ -241,15 +311,15 @@
       self.log(logging.INFO, f"Closing the {type(self._device).__name__} "
                              f"InOut")
       self._device.close()
       self.log(logging.INFO, f"{type(self._device).__name__} InOut closed")
 
   def _read_data(self) -> None:
     """Reads the data or the stream, offsets the timestamp and sends the data
-    to downstream blocks."""
+    to downstream Blocks."""
 
     if self._streamer:
       # Starting the stream if needed
       if not self._stream_started:
         self.log(logging.INFO, f"Starting stream on the "
                                f"{type(self._device).__name__} InOut")
         self._device.start_stream()
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/machine.py` & `crappy-2.0.0.dev2/src/crappy/blocks/machine.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,118 @@
 # coding: utf-8
 
 from time import time
-from typing import Dict, List, Any, Optional
+from typing import Dict, List, Any, Optional, Iterable
 from dataclasses import dataclass, fields
 import logging
 
 from .meta_block import Block
 from ..actuator import actuator_dict, Actuator
 from ..tool.ft232h import USBServer
 
 
 @dataclass
 class ActuatorInstance:
-  """"""
+  """This class holds all the information that can be associated to an
+  Actuator."""
 
   actuator: Actuator
   speed: Optional[float] = None
   position_label: Optional[str] = None
   speed_label: Optional[str] = None
   mode: str = 'speed'
   cmd_label: str = 'cmd'
   speed_cmd_label: Optional[str] = None
 
 
 class Machine(Block):
-  """This block is meant to drive one or several :ref:`Actuators`.
+  """This Block is meant to drive one or several
+  :class:`~crappy.actuator.Actuator`. It can set speed or position commands on
+  hardware actuators.
 
-  The possibility to drive several Actuators from a unique block is given so
+  The possibility to drive several Actuators from a unique Block is given so
   that they can be driven in a synchronized way. If synchronization is not
-  needed, it is preferable to drive the Actuators from separate Machine blocks.
+  needed, it is preferable to drive the Actuators from separate Machine Blocks.
+
+  This Block takes the speed or position commands for the Actuators  as inputs,
+  and can optionally read and output the current speed and/or positions of the
+  Actuators. The speed and position commands are set respectively by calling
+  the :meth:`~crappy.actuator.Actuator.set_position` and
+  :meth:`~crappy.actuator.Actuator.set_speed` methods of the Actuators, and the
+  current speed and position values are acquired by calling the
+  :meth:`~crappy.actuator.Actuator.get_position` and
+  :meth:`~crappy.actuator.Actuator.get_speed` methods of the Actuators.
+
+  It is possible to tune for each Actuator the label over which it receives its
+  commands, and optionally the labels over which it sends its current speed
+  and/or position. The driving mode (`'speed'` or `'position'`) can also be set
+  independently for each Actuator.
   """
 
   def __init__(self,
-               actuators: List[Dict[str, Any]],
+               actuators: Iterable[Dict[str, Any]],
                common: Optional[Dict[str, Any]] = None,
                time_label: str = 't(s)',
                ft232h_ser_num: Optional[str] = None,
                spam: bool = False,
-               freq: float = 200,
+               freq: Optional[float] = 200,
                display_freq: bool = False,
                debug: Optional[bool] = False) -> None:
-    """Sets the args and initializes the parent class.
+    """Sets the arguments and initializes the parent class.
 
     Args:
-      actuators: The :obj:`list` of all the :ref:`Actuators` this block needs
-        to drive. It contains one :obj:`dict` for every Actuator, with
-        mandatory and optional keys. The keys providing information on how to
-        drive the Actuator are listed below. Any other key will be passed to
-        the Actuator object as argument when instantiating it.
+      actuators: An iterable (like a :obj:`list` or a :obj:`tuple`) of all the
+        :class:`~crappy.actuator.Actuator` this Block needs to drive. It 
+        contains one :obj:`dict` for every Actuator, with mandatory and 
+        optional keys. The keys providing information on how to drive the 
+        Actuator are listed below. Any other unrecognized key will be passed to 
+        the Actuator as argument when instantiating it.
       common: The keys of this :obj:`dict` will be common to all the Actuators.
-        If it conflicts with an existing key for an Actuator, the common one
-        will prevail.
+        If one key conflicts with an existing key for an Actuator, the common 
+        one will prevail.
       time_label: If reading speed or position from one or more Actuators, the
         time information will be carried by this label.
-      spam: If :obj:`True`, a command is sent to the Actuators on each loop of
-        the block, else it is sent every time a new command is received.
-      freq: The block will try to loop at this frequency.
+      spam: If :obj:`True`, a command is sent to the Actuators at each loop of
+        the Block, else it is sent every time a new command is received.
+      freq: The target looping frequency for the Block. If :obj:`None`, loops 
+        as fast as possible.
       display_freq: If :obj:`True`, displays the looping frequency of the
-        block.
+        Block.
+      debug: If :obj:`True`, displays all the log messages including the
+        :obj:`~logging.DEBUG` ones. If :obj:`False`, only displays the log
+        messages with :obj:`~logging.INFO` level or higher. If :obj:`None`,
+        disables logging for this Block.
 
     Note:
       - ``actuators`` keys:
 
-        - ``type``: The name of the Actuator class to instantiate. This key is
-          mandatory.
+        - ``type``: The name of the :class:`~crappy.actuator.Actuator` class to 
+          instantiate. This key is mandatory.
         - ``cmd_label``: The label carrying the command for driving the
           Actuator. It defaults to `'cmd'`.
-        - ``mode``: Can be either `'speed'` or `'position'`. Will either call
-          :meth:`set_speed` or :meth:`set_position` to drive the actuator. When
-          driven in `'position'` mode, the speed of the actuator can also be
-          adjusted, see the ``speed_cmd_label`` key. The default mode is
+        - ``mode``: Can be either `'speed'` or `'position'`. Either
+          :meth:`~crappy.actuator.Actuator.set_speed` or
+          :meth:`~crappy.actuator.Actuator.set_position` is called to drive the
+          Actuator, depending on the selected mode. When driven in `'position'` 
+          mode, the speed of the actuator can also be adjusted, see the 
+          ``speed`` and ``speed_cmd_label`` keys. The default mode is 
           `'speed'`.
         - ``speed``: If mode is `'position'`, the speed at which the Actuator
           should move. This speed is passed as second argument to the
-          :meth:`set_position` method of the Actuator. If the
-          ``speed_cmd_label`` key is not specified, this speed will remain the
-          same for the entire test. This key is not mandatory.
-        - ``position_label``: If given, the block will return the value of
-          :meth:`get_position` under this label. This key is not mandatory.
-        - ``speed_label``: If given, the block will return the value of
-          :meth:`get_speed` under this label. This key is not mandatory.
+          :meth:`~crappy.actuator.Actuator.set_position` method of the
+          Actuator. If the ``speed_cmd_label`` key is not specified, this speed
+          will remain the same for the entire test. This key is not mandatory.
+        - ``position_label``: If given, the Block will return the value of
+          :meth:`~crappy.actuator.Actuator.get_position` under this label. This
+          key is not mandatory.
+        - ``speed_label``: If given, the Block will return the value of
+          :meth:`~crappy.actuator.Actuator.get_speed` under this label. This
+          key is not mandatory.
         - ``speed_cmd_label``: The label carrying the speed to set when driving
-          in position mode. Each time a value is received, the stored speed
+          in `'position'` mode. Each time a value is received, the stored speed
           value is updated. It will also overwrite the ``speed`` key if given.
 
     """
 
     self._actuators: List[ActuatorInstance] = list()
     self._ft232h_args = None
 
@@ -113,19 +140,21 @@
     # The names of the possible settings, to avoid typos and reduce verbosity
     actuator_settings = [field.name for field in fields(ActuatorInstance)
                          if field.type is not Actuator]
 
     # The list of all the Actuator types to instantiate
     self._types = [actuator['type'] for actuator in actuators]
 
+    # Checking that all the given actuators are valid
     if not all(type_ in actuator_dict for type_ in self._types):
-      unknown = tuple(type_ for type_ in self._types if type_
-                      not in actuator_dict)
-      raise ValueError(f"[Machine] Unknown actuator type(s) : {unknown}\n"
-                       f"The possible types are : {actuator_dict.keys()}")
+      unknown = ', '.join(tuple(type_ for type_ in self._types if type_
+                          not in actuator_dict))
+      possible = ', '.join(sorted(actuator_dict.keys()))
+      raise ValueError(f"Unknown actuator type(s) : {unknown} ! "
+                       f"The possible types are : {possible}")
 
     # The settings that won't be passed to the Actuator objects
     self._settings = [{key: value for key, value in actuator.items()
                        if key in actuator_settings}
                       for actuator in actuators]
 
     # The settings that will be passed as kwargs to the Actuator objects
@@ -135,15 +164,19 @@
 
     # Checking whether the Actuators communicate through an FT232H
     if any(actuator_dict[type_].ft232h for type_ in self._types):
       self._ft232h_args = USBServer.register(ft232h_ser_num)
 
   def prepare(self) -> None:
     """Checks the validity of the linking and initializes all the Actuator
-    objects to drive."""
+    objects to drive.
+
+    This method calls the :meth:`~crappy.actuator.Actuator.open` method of each
+    Actuator.
+    """
 
     # Instantiating the actuators and storing them
     self._actuators = [ActuatorInstance(
       actuator=actuator_dict[type_](**actuator_kw)
       if not actuator_dict[type_].ft232h else
       actuator_dict[type_](**actuator_kw, _ft232h_args=self._ft232h_args),
       **setting)
@@ -160,17 +193,31 @@
       self.log(logging.INFO, f"Opening the {type(actuator.actuator).__name__}"
                              f"Actuator")
       actuator.actuator.open()
       self.log(logging.INFO, f"Opened the {type(actuator.actuator).__name__}"
                              f"Actuator")
 
   def loop(self) -> None:
-    """Receives the commands from upstream blocks, sets them on the actuators
-    to drive, and sends the read positions and speed to the downstream
-    blocks."""
+    """Sets the received position and speed commands, and reads the current 
+    speed and position from the :class:`~crappy.actuator.Actuator`.
+    
+    For each Actuator, a command is set **only** if a new one was received or 
+    if the ``spam`` argument is :obj:`True`. It is set using either 
+    :meth:`~crappy.actuator.Actuator.set_position` or
+    :meth:`~crappy.actuator.Actuator.set_speed` depending on the selected
+    driving mode.
+    
+    For each Actuator, a speed and/or position value is read **only** if the 
+    ``speed_label`` and/or the ``position_label`` was set. If so, these values
+    are read at each loop and sent to downstream Blocks over the given labels.
+    This is independent of the chosen driving mode. The
+    :meth:`~crappy.actuator.Actuator.get_position` and
+    :meth:`~crappy.actuator.Actuator.get_speed` are called for acquiring the
+    position and speed values respectively.
+    """
 
     # Receiving the latest command
     recv = self.recv_last_data(fill_missing=self._spam)
 
     # Iterating over the actuators for setting the commands
     if recv:
       for actuator in self._actuators:
@@ -216,19 +263,23 @@
 
     # Sending the speed and position values if any
     if to_send:
       to_send[self._time_label] = time() - self.t0
       self.send(to_send)
 
   def finish(self) -> None:
-    """Stops and closes all the actuators to drive."""
+    """Stops and closes all the Actuators to drive.
+
+    This method calls the :meth:`~crappy.actuator.Actuator.stop` and
+    :meth:`~crappy.actuator.Actuator.close` method of each Actuator.
+    """
 
     for actuator in self._actuators:
       self.log(logging.INFO, f"Stopping the {type(actuator.actuator).__name__}"
                              f"Actuator")
       actuator.actuator.stop()
     for actuator in self._actuators:
       self.log(logging.INFO, f"Closing the {type(actuator.actuator).__name__}"
                              f"Actuator")
       actuator.actuator.close()
-      self.log(logging.INFO, f"closed the {type(actuator.actuator).__name__}"
+      self.log(logging.INFO, f"Closed the {type(actuator.actuator).__name__}"
                              f"Actuator")
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/meta_block/block.py` & `crappy-2.0.0.dev2/src/crappy/blocks/meta_block/block.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,43 +5,44 @@
   get_start_method
 from multiprocessing.sharedctypes import Synchronized
 from multiprocessing import synchronize, queues
 from threading import BrokenBarrierError, Thread
 from queue import Empty
 import logging
 import logging.handlers
-from time import sleep, time
+from time import sleep, time, time_ns
 from weakref import WeakSet
-from typing import Union, Optional, List, Dict, Any
+from typing import Union, Optional, List, Dict, Any, Iterable
 from collections import defaultdict
 import subprocess
 from sys import stdout, stderr, argv
 from pathlib import Path
 
 from .meta_block import MetaBlock
 from ...links import Link
 from ..._global import LinkDataError, StartTimeout, PrepareError, \
   T0NotSetError, GeneratorStop, ReaderStop, CameraPrepareError, \
-  CameraRuntimeError
+  CameraRuntimeError, CameraConfigError
 from ...tool.ft232h import USBServer
 
-# Todo:
-#  Add a clean way to stop the blocks, using the keyboard or a button
-
 
 class Block(Process, metaclass=MetaBlock):
   """This class constitutes the base object in Crappy.
 
-  It is extremely versatile, an can perform a wide variety of actions during a
+  It is extremely versatile, and can perform a wide variety of actions during a
   test. Many Blocks are already defined in Crappy, but it is possible to define
   custom ones for specific purposes.
 
   It is a subclass of :obj:`multiprocessing.Process`, and is thus an
   independent process in Python. It communicates with other Blocks via
   :mod:`multiprocessing` objects.
+
+  This class also contains the class methods that allow driving a script with
+  Crappy. They are always called in the `__main__` Process, and drive the
+  execution of all the children Blocks.
   """
 
   instances = WeakSet()
   names: List[str] = list()
   log_level: Optional[int] = logging.DEBUG
 
   # The synchronization objects will be set later
@@ -64,15 +65,15 @@
 
     # The lists of input and output links
     self.outputs: List[Link] = list()
     self.inputs: List[Link] = list()
 
     # Various objects that should be set by child classes
     self.niceness: int = 0
-    self.labels: Optional[List[str]] = None
+    self.labels: Optional[Iterable[str]] = None
     self.freq = None
     self.display_freq = False
     self.name = self.get_name(type(self).__name__)
 
     # The synchronization objects will be set later
     self._instance_t0: Optional[Synchronized] = None
     self._ready_barrier: Optional[synchronize.Barrier] = None
@@ -89,81 +90,87 @@
     self._last_t: Optional[float] = None
     self._last_fps: Optional[float] = None
     self._n_loops: int = 0
 
     self._last_values = None
 
   def __new__(cls, *args, **kwargs):
-    """Called when instantiating a new instance of a Block. Adds itself to
-    the WeakSet of all blocks."""
+    """Called when instantiating a new instance of a Block.
+
+    Adds itself to the :obj:`~weakref.WeakSet` listing all the instantiated
+    Blocks.
+    """
 
     instance = super().__new__(cls)
     cls.instances.add(instance)
     return instance
 
   @classmethod
   def get_name(cls, name: str) -> str:
-    """"""
+    """Method attributing to each new Block a unique name, based on the name of
+    the class and the number of existing instances for this class."""
 
     i = 1
     while f"crappy.{name}-{i}" in cls.names:
       i += 1
 
     cls.names.append(f"crappy.{name}-{i}")
     return f"crappy.{name}-{i}"
 
   @classmethod
   def start_all(cls,
                 allow_root: bool = False,
                 log_level: Optional[int] = logging.DEBUG) -> None:
     """Method for starting a script with Crappy.
 
-    It sets the synchronization objects for all the blocks, renices the
-    corresponding processes and starts the blocks.
+    It sets the synchronization objects for all the Blocks, renices the
+    corresponding :obj:`~multiprocessing.Process` and starts the Blocks.
 
     The call to this method is blocking until Crappy finishes.
 
     Note:
       It is possible to have a finer grained control of the start of a Crappy
       script with the methods :meth:`prepare_all`, :meth:`renice_all` and
       :meth:`launch_all`.
 
     Args:
-      allow_root: If set tu :obj:`True`, tries to renice the processes niceness
-        with sudo privilege in Linux. It requires the Python script to be run
+      allow_root: If set to :obj:`True`, tries to renice the Processes with
+        sudo privilege in Linux. It requires the Python script to be run
         with sudo privilege, otherwise it has no effect.
       log_level: The maximum logging level that will be handled by Crappy. By
-        default, it is set to the lowest level (DEBUG) so that all messages are
-        handled. If set to a higher level, the levels specified for each Block
-        with the ``debug`` argument may be ignored. If set to :obj:`None`,
-        logging is totally disabled. Refer to the documentation of the
-        :mod:`logging` module for information on the possible levels.
+        default, it is set to the lowest level (:obj:`~logging.DEBUG`) so that
+        all messages are handled. If set to a higher level, the levels
+        specified for each Block with the ``debug`` argument may be ignored. If
+        set to :obj:`None`, logging is totally disabled. Refer to the
+        documentation of the :mod:`logging` module for information on the
+        possible levels.
     """
 
     cls.prepare_all(log_level)
     cls.renice_all(allow_root)
     cls.launch_all()
 
   @classmethod
   def prepare_all(cls, log_level: Optional[int] = logging.DEBUG) -> None:
-    """Creates the synchronization objects, shares them with the blocks, and
-    starts the processes associated to the blocks.
+    """Creates the synchronization objects, shares them with the Blocks, and
+    starts the :obj:`~multiprocessing.Process` associated to the Blocks.
 
-    Also initializes the logger for the Crappy script.
+    Also initializes the :obj:`~logging.Logger` for the Crappy script.
 
-    Once started with this method, the blocks will call their :meth:`prepare`
+    Once started with this method, the Blocks will call their :meth:`prepare`
     method and then be blocked by a :obj:`multiprocessing.Barrier`.
 
     Args:
       log_level: The maximum logging level that will be handled by Crappy. By
-        default, it is set to the lowest level (DEBUG) so that all messages are
-        handled. If set to a higher level, the levels specified for each Block
-        with the ``debug`` argument may be ignored. If set to :obj:`None`,
-        logging is totally disabled. Refer to the documentation of the
-        :mod:`logging` module for information on the possible levels.
+        default, it is set to the lowest level (:obj:`~logging.DEBUG`) so that 
+        all messages are handled. If set to a higher level, the levels 
+        specified for each Block with the ``debug`` argument may be ignored. If 
+        set to :obj:`None`, logging is totally disabled. Refer to the 
+        documentation of the :mod:`logging` module for information on the 
+        possible levels.
     """
 
     try:
 
       if cls.prepared_all:
         cls.cls_log(logging.ERROR,
                     "The method prepare_all was already called ! Stop the "
@@ -235,22 +242,23 @@
     except KeyboardInterrupt:
       cls.cls_log(logging.INFO, 'KeyboardInterrupt caught while running '
                                 'prepare_all')
       cls._exception()
 
   @classmethod
   def renice_all(cls, allow_root: bool) -> None:
-    """On Linux and MacOS, renices the processes associated with the blocks.
+    """On Linux and macOS, renices the :obj:`~multiprocessing.Process` 
+    associated with the Blocks.
 
     On Windows, does nothing.
 
     Args:
-      allow_root: If set tu :obj:`True`, tries to renice the processes niceness
-        with sudo privilege in Linux. It requires the Python script to be run
-        with sudo privilege, otherwise it has no effect.
+      allow_root: If set to :obj:`True`, tries to renice the Processes with 
+        sudo privilege in Linux. It requires the Python script to be run with 
+        sudo privilege, otherwise it has no effect.
     """
 
     try:
       # Making sure the prepare method has already been called
       if not cls.prepared_all:
         cls.cls_log(logging.ERROR, "Cannot call renice before calling "
                                    "prepare ! Aborting")
@@ -287,22 +295,24 @@
     except KeyboardInterrupt:
       cls.cls_log(logging.INFO, 'KeyboardInterrupt caught while running '
                                 'renice_all')
       cls._exception()
 
   @classmethod
   def launch_all(cls) -> None:
-    """The final method being called by the main process running a Crappy
-    script.
+    """The final method being called by the main
+    :obj:`~multiprocessing.Process` running a script with Crappy.
 
-    It unlocks all the Blocks by releasing the synchronization barrier, sets
-    the shared t0 value, and then waits for all the Blocks to finish.
-
-    In case an exception is raised, sets the stop event for warning the Blocks,
-    waits for the Blocks to finish, and if they don't, terminates them.
+    It unlocks all the Blocks by releasing the synchronization
+    :obj:`~multiprocessing.Barrier`, sets the shared t0
+    :obj:`~multiprocessing.Value`, and then waits for all the Blocks to finish.
+
+    In case an exception is raised, sets the stop :obj:`~multiprocessing.Event`
+    for warning the Blocks, waits for the Blocks to finish, and if they don't,
+    terminates them.
     """
 
     try:
       # Making sure the prepare method has already been called
       if not cls.prepared_all:
         cls.cls_log(logging.ERROR, "Cannot call launch_all before calling "
                                    "prepare ! Aborting")
@@ -319,64 +329,52 @@
       # prepare_all and launch_all methods can be used separately for a finer
       # grained control
       cls.cls_log(logging.INFO, 'Waiting for all Blocks to be ready')
       cls.ready_barrier.wait()
       cls.cls_log(logging.INFO, 'All Blocks ready now')
 
       # Setting t0 and telling all the block to start
-      cls.shared_t0.value = time()
+      cls.shared_t0.value = time_ns() / 1e9
       cls.cls_log(logging.INFO, f'Start time set to {cls.shared_t0.value}s')
       cls.start_event.set()
       cls.cls_log(logging.INFO, 'Start event set, all Blocks can now start')
 
       # The main process mustn't finish before all the blocks are done running
       cls.cls_log(logging.INFO, 'Main process done, waiting for all Blocks to '
                                 'finish')
       for inst in cls.instances:
         inst.join()
         cls.cls_log(logging.INFO, f'{inst.name} finished by itself')
 
-      # Stopping the USB server if required
-      if USBServer.initialized:
-        cls.cls_log(logging.INFO, "Stopping the USB server")
-        USBServer.stop_server()
-
-      if get_start_method() == 'spawn':
-        cls.thread_stop = True
-        cls.log_thread.join(timeout=0.1)
-
-      if cls.log_thread.is_alive():
-        cls.cls_log(logging.WARNING, "The thread reading the log messages did "
-                                     "not terminate in time !")
-      else:
-        cls.cls_log(logging.INFO, 'All Blocks done, Crappy terminated '
-                                  'gracefully\n')
-
     # A Block crashed while preparing
     except BrokenBarrierError:
-      cls.cls_log(logging.ERROR, "Exception raised in a Block while  waiting "
+      cls.cls_log(logging.ERROR, "Exception raised in a Block while waiting "
                                  "for all Blocks to be ready, stopping")
       cls._exception()
     # The user ended the script while preparing
     except KeyboardInterrupt:
       cls.cls_log(logging.INFO, 'KeyboardInterrupt caught while running '
                                 'launch_all')
       cls._exception()
     # Another exception occurred
     except (Exception,) as exc:
       cls.logger.exception("Caught exception while running launch_all, "
                            "aborting", exc_info=exc)
       cls._exception()
 
+    # Performing the cleanup actions before exiting
+    finally:
+      cls._cleanup()
+
   @classmethod
   def _exception(cls) -> None:
-    """This method is called when an exception is caught in the main process.
+    """This method is called when an exception is caught in the main Process.
 
     It waits for all the Blocks to end, and kills them if they don't stop by
-    themselves. Also stops the thread managing the logging.
+    themselves. Also stops the Thread managing the logging.
     """
 
     cls.stop_event.set()
     cls.cls_log(logging.INFO, 'Stop event set, waiting for all Blocks to '
                               'finish')
     t = time()
 
@@ -393,29 +391,60 @@
         for inst in cls.instances:
           if inst.is_alive():
             inst.terminate()
             cls.cls_log(logging.WARNING, f'Block {inst.name} terminated')
           else:
             cls.cls_log(logging.INFO, f'Block {inst.name} done')
 
-    if get_start_method() == 'spawn':
-      cls.thread_stop = True
-      cls.log_thread.join(timeout=0.1)
-
-    if cls.log_thread.is_alive():
-      cls.cls_log(logging.WARNING, "The thread reading the log messages did "
-                                   "not terminate in time !")
+        break
 
-    else:
-      cls.cls_log(logging.INFO, 'All Blocks done, Crappy terminated '
-                                'gracefully\n')
+  @classmethod
+  def _cleanup(cls) -> None:
+    """Method called at the very end of every script execution.
+
+    It stops, if relevant, the USBServer and the log_thread, and warns the user
+    in case Processes would still be running.
+    """
+
+    try:
+      # Stopping the USB server if required
+      if USBServer.initialized:
+        cls.cls_log(logging.INFO, "Stopping the USB server")
+        USBServer.stop_server()
+
+      # Stopping the log thread if required
+      if get_start_method() == 'spawn':
+        cls.thread_stop = True
+        cls.log_thread.join(timeout=0.1)
+
+      # Warning in case the log thread did not stop correctly
+      if cls.log_thread.is_alive():
+        cls.cls_log(logging.WARNING, "The thread reading the log messages did "
+                                     "not terminate in time !")
+
+      # Checking whether all Blocks terminated gracefully
+      if cls.instances and any(inst.is_alive() for inst in cls.instances):
+        running = ', '.join(inst.name for inst in cls.instances
+                            if inst.is_alive())
+        cls.cls_log(logging.ERROR, f"Crappy failed to finish gracefully, "
+                                   f"Block(s) {running} still running !")
+      else:
+        cls.cls_log(logging.INFO, 'All Blocks done, Crappy terminated '
+                                  'gracefully\n')
+
+    except KeyboardInterrupt:
+      cls.cls_log(logging.INFO, "Caught KeyboardInterrupt while cleaning up, "
+                                "ignoring it")
+    except (Exception,) as exc:
+      cls.logger.exception("Caught exception while cleaning up !",
+                           exc_info=exc)
 
   @classmethod
   def _set_logger(cls) -> None:
-    """Initializes the logging for the main process.
+    """Initializes the logging for the main Process.
 
     It creates two Stream Loggers, one for the info and debug levels displaying
     on stdout and one for the other levels displaying on stderr. It also
     creates a File Logger for saving the log to a log file.
 
     The levels WARNING and above are always being displayed in the terminal, no
     matter what the user chooses. Similarly, the INFO log level and above are
@@ -478,26 +507,27 @@
       if file_handler is not None:
         crappy_log.addHandler(file_handler)
 
     cls.logger = crappy_log
 
   @classmethod
   def stop_all(cls) -> None:
-    """Method for stopping all the Blocks by setting the stop event."""
+    """Method for stopping all the Blocks by setting the stop
+    :obj:`~multiprocessing.Event`."""
 
     if cls.stop_event is not None:
       cls.stop_event.set()
       cls.cls_log(logging.INFO, 'Stop event set after a call to stop(), all '
                                 'Blocks should now finish')
 
   @classmethod
   def reset(cls) -> None:
-    """Resets Crappy by emptying the WeakSet containing references to all the
-    Blocks. Only useful for restarting Crappy from a script where Crappy was
-    already started."""
+    """Resets Crappy by emptying the :obj:`~weakref.WeakSet` containing
+    references to all the Blocks. Only useful for restarting Crappy from a
+    script where Crappy was already started."""
 
     cls.instances = WeakSet()
     cls.names = list()
     cls.thread_stop = False
     cls.prepared_all = False
     cls.launched_all = False
 
@@ -507,29 +537,29 @@
     cls.stop_event = None
 
     if cls.logger is not None:
       cls.cls_log(logging.INFO, 'Crappy was reset by the reset() command')
   
   @classmethod
   def cls_log(cls, level: int, msg: str) -> None:
-    """Wrapper for logging messages in the main process.
+    """Wrapper for logging messages in the main Process.
     
-    Ensures the logger exists before trying to log, thus avoiding potential 
+    Ensures the Logger exists before trying to log, thus avoiding potential 
     errors.
     """
     
     if cls.logger is None:
       return
     cls.logger.log(level=level, msg=msg)
 
   @classmethod
   def _log_target(cls) -> None:
-    """This method is the target to the logger Thread.
+    """This method is the target to the Logger Thread.
 
-    It reads log messages from a Queue and passes them to the logger for
+    It reads log messages from a Queue and passes them to the Logger for
     handling.
     """
 
     while not cls.thread_stop:
       try:
         record = cls.log_queue.get(block=True, timeout=0.05)
       except Empty:
@@ -542,22 +572,23 @@
   def _stdout_filter(rec: logging.LogRecord) -> bool:
     """Returns :obj:`True` if the input log message has level INFO or DEBUG,
     :obj:`False` otherwise."""
 
     return rec.levelno in (logging.DEBUG, logging.INFO)
 
   def run(self) -> None:
-    """The method run by the Blocks when their process is started.
+    """The method run by the Blocks when their :obj:`~multiprocessing.Process` 
+    is started.
 
     It first calls :meth:`prepare`, then waits at the
-    :obj:`multiprocessing.Barrier` for all Blocks to be ready, then calls
+    :obj:`~multiprocessing.Barrier` for all Blocks to be ready, then calls
     :meth:`begin`, then :meth:`main`, and finally :meth:`finish`.
     
-    If an exception is raised, sets the shared stop event to warn all the other
-    Blocks.
+    If an exception is raised, sets the shared stop 
+    :obj:`~multiprocessing.Event` to warn all the other Blocks.
     """
 
     try:
       # Initializes the logger for the Block
       self._set_block_logger()
       self.log(logging.INFO, "Block launched")
 
@@ -589,15 +620,15 @@
         self.log(logging.INFO, "Start time set, Block starting")
 
       # Running the first loop
       self.log(logging.INFO, "Calling begin method")
       self.begin()
 
       # Setting the attributes for counting the performance
-      self._last_t = time()
+      self._last_t = time_ns() / 1e9
       self._last_fps = self._last_t
       self._n_loops = 0
 
       # Running the main loop until told to stop
       self.log(logging.INFO, "Entering main loop")
       self.main()
       self.log(logging.INFO, "Exiting main loop after stop event was set")
@@ -606,14 +637,18 @@
     except LinkDataError:
       self.log(logging.ERROR, "Tried to send a wrong data type through a Link,"
                               " stopping !")
     # An error occurred in another Block while preparing
     except PrepareError:
       self.log(logging.ERROR, "Exception raised in another Block while waiting"
                               " for all Blocks to be ready, stopping")
+    # An error occurred in the CameraConfig window while preparing
+    except CameraConfigError:
+      self.log(logging.ERROR, "Exception raised in a configuration window, "
+                              "stopping")
     # An error occurred in a Camera process while preparing
     except CameraPrepareError:
       self.log(logging.ERROR, "Exception raised in a Camera process while "
                               "preparing, stopping")
       # An error occurred in a Camera process while running
     except CameraRuntimeError:
       self.log(logging.ERROR, "Exception raised in a Camera process while "
@@ -670,16 +705,16 @@
     """This method should perform any action required for initializing the
     Block before the test starts.
 
     For example, it can open a network connection, create a file, etc. It is
     also fine for this method not to be overriden if there's no particular
     action to perform.
 
-    Note that this method is called once the process associated to the Block
-    has been started.
+    Note that this method is called once the :obj:`~multiprocessing.Process`
+    associated to the Block has been started.
     """
 
     ...
 
   def begin(self) -> None:
     """This method can be considered as the first loop of the test, and is
     called before the :meth:`loop` method.
@@ -690,16 +725,16 @@
 
     ...
 
   def loop(self) -> None:
     """This method is the core of the Block. It is called repeatedly during the
     test, until the test stops or an error occurs.
 
-    Only in this method should data be sent to downstream blocks, or received
-    from upstream blocks.
+    Only in this method should data be sent to downstream Blocks, or received
+    from upstream Blocks.
 
     Although it is possible not to override this method, that has no practical
     interest and this method should always be rewritten.
     """
 
     self.log(logging.WARNING, f"Loop method not defined, this block does "
                               f"nothing !")
@@ -709,16 +744,16 @@
     """This method should perform any action required for properly ending the
     test.
 
     For example, it can close a file or disconnect from a network. It is also
     fine for this method not to be overriden if no particular action needs to
     be performed.
 
-    Note that this method should normally be called even in case an error
-    occurs, although that cannot be guaranteed.
+    Note that this method will normally be called even in case an error occurs,
+    although that cannot be guaranteed.
     """
 
     ...
 
   def stop(self) -> None:
     """This method stops all the running Blocks.
 
@@ -743,43 +778,43 @@
 
     It also displays the looping frequency of the Block if requested by the
     user. If no looping frequency is specified, the Block will loop as fast as
     possible.
     """
 
     self._n_loops += 1
+    t = time_ns() / 1e9
 
     # Only handling frequency if requested
     if self.freq is not None:
-      t = time()
 
       # Correcting the error of the sleep function through a recursive approach
       # The last 2 milliseconds are in free loop
       remaining = self._last_t + 1 / self.freq - t
       while remaining > 0:
-        t = time()
+        t = time_ns() / 1e9
         remaining = self._last_t + 1 / self.freq - t
         sleep(max(0., remaining / 2 - 2e-3))
 
-      self._last_t = t
+    self._last_t = t
 
     # Displaying frequency every 2 seconds
     if self.display_freq and self._last_t - self._last_fps > 2:
       self.log(
         logging.INFO,
         f"loops/s: {self._n_loops / (self._last_t - self._last_fps)}")
 
       self._n_loops = 0
       self._last_fps = self._last_t
 
   def _set_block_logger(self) -> None:
-    """Initializes the logger for the Block.
+    """Initializes the Logger for the Block.
 
     If the :mod:`multiprocessing` start method is `spawn` (mostly on Windows),
-    redirects the log messages to a Queue for passing them to the main process.
+    redirects the log messages to a Queue for passing them to the main Process.
     """
 
     logger = logging.getLogger(self.name)
 
     # Adjusting logging to the desired level
     if self._log_level is not None:
       logger.setLevel(self._log_level)
@@ -794,18 +829,19 @@
 
     self._logger = logger
 
   @property
   def debug(self) -> Optional[bool]:
     """Indicates whether the debug information should be displayed or not.
 
-    If :obj:`False` (the default), only displays the INFO logging level. If
-    :obj:`True`, displays the DEBUG logging level for the Block. And if
-    :obj:`None`, displays only the CRITICAL logging level, which is equivalent
-    to no information at all.
+    If :obj:`False` (the default), only displays the :obj:`~logging.INFO`
+    logging level. If :obj:`True`, displays the :obj:`~logging.DEBUG` logging
+    level for the Block. And if :obj:`None`, displays only the
+    :obj:`~logging.CRITICAL` logging level, which is equivalent to no
+    information at all.
     """
 
     return self._debug
 
   @debug.setter
   def debug(self, val: Optional[bool]) -> None:
     if val is not None:
@@ -827,20 +863,22 @@
     if self._instance_t0 is not None and self._instance_t0.value > 0:
       self.log(logging.DEBUG, "Start time value requested")
       return self._instance_t0.value
     else:
       raise T0NotSetError
 
   def add_output(self, link: Link) -> None:
-    """Adds an output link to the list of output links of the Block."""
+    """Adds an output :class:`~crappy.links.Link` to the list of output Links
+    of the Block."""
 
     self.outputs.append(link)
 
   def add_input(self, link: Link) -> None:
-    """Adds an input link to the list of input links of the Block."""
+    """Adds an input :class:`~crappy.links.Link` to the list of input Links of
+    the Block."""
 
     self.inputs.append(link)
 
   def log(self, log_level: int, msg: str) -> None:
     """Method for recording log messages from the Block. This option should be
     preferred to calling :func:`print`.
 
@@ -849,57 +887,79 @@
       msg: The message to log, as a :obj:`str`.
     """
 
     if self._logger is None:
       return
     self._logger.log(log_level, msg)
 
-  def send(self, data: Union[Dict[str, Any], List[Any]]) -> None:
-    """Ensures that the data to send is formatted as a :obj:`dict`, and sends
-    it in all the downstream links."""
-
-    # Building the dict to send from the data and labels if the data is a list
-    if isinstance(data, list):
-      if not self.labels:
-        self.log(logging.ERROR, "trying to send data as a list but no labels "
-                                "are specified ! Please add a self.labels "
-                                "attribute.")
+  def send(self, data: Optional[Union[Dict[str, Any], Iterable[Any]]]) -> None:
+    """Method for sending data to downstream Blocks.
+
+    The exact same :obj:`dict` is sent to every downstream Block.
+
+    This method accepts the data to send either as a :obj:`dict` or as another
+    type of iterable (like a :obj:`list` or a :obj:`tuple`). If data is
+    provided as a dict, it is sent as is. The keys of the dict then correspond
+    to the labels. Otherwise, the values given as an iterable are first
+    converted to a dict using the ``self.labels`` attribute containing the
+    labels to use.
+
+    It is up to the user to match the order of the values in the iterable with
+    the order of the labels in ``self.labels``. If the number of labels and the
+    number of values to send do not match, no error is raised but some data
+    might not get sent.
+    """
+
+    # Just in case, not handling non-existing data
+    if data is None:
+      return
+
+    # Case when the data to send is not given as a dict
+    if not isinstance(data, dict):
+      # First, checking that labels are provided
+      if self.labels is None or not self.labels:
+        self.log(logging.ERROR, "Trying to send data as an iterable, but no "
+                                "labels are specified ! Please add a "
+                                "self.labels attribute.")
         raise LinkDataError
-      self.log(logging.DEBUG, f"Converting {data} to dict before sending")
-      data = dict(zip(self.labels, data))
 
-    # Making sure the data is being sent as a dict
-    elif not isinstance(data, dict):
-      self.log(logging.ERROR, f"Trying to send a {type(data)} in a Link !")
-      raise LinkDataError
+      # Trying to convert iterable data to dict using the given labels
+      try:
+        self.log(logging.DEBUG, f"Converting {data} to dict before sending")
+        data = dict(zip(self.labels, data))
+      except TypeError:
+        self.log(logging.ERROR, f"Cannot convert data to send (of type "
+                                f"{type(data)}) to dict ! Please ensure that "
+                                f"the data is given as an iterable, as well as"
+                                f" self.labels.")
 
-    # Sending the data to the downstream blocks
+    # Sending the data to the downstream Blocks
     for link in self.outputs:
       self.log(logging.DEBUG, f"Sending {data} to Link {link.name}")
       link.send(data)
 
   def data_available(self) -> bool:
     """Returns :obj:`True` if there's data available for reading in at least
-    one of the input Links."""
+    one of the input :class:`~crappy.links.Link`."""
 
     self.log(logging.DEBUG, "Data availability requested")
     return self.inputs and any(link.poll() for link in self.inputs)
 
   def recv_data(self) -> Dict[str, Any]:
-    """Reads the first available values from each incoming Link and returns
-    them all in a single dict.
+    """Reads the first available values from each incoming
+    :class:`~crappy.links.Link` and returns them all in a single dict.
 
     The returned :obj:`dict` might not always have a fixed number of keys,
     depending on the availability of incoming data.
 
-    Also, the returned values are the oldest available in the links. See
+    Also, the returned values are the oldest available in the Links. See
     :meth:`recv_last_data` for getting the newest available values.
 
     Important:
-      If data is received over a same label from different links, part of it
+      If data is received over a same label from different Links, part of it
       will be lost ! Always avoid using a same label twice in a Crappy script.
 
     Returns:
       A :obj:`dict` whose keys are the received labels and with a single value
       for each key (usually a :obj:`float` or a :obj:`str`).
     """
 
@@ -908,29 +968,29 @@
     for link in self.inputs:
       ret.update(link.recv())
 
     self.log(logging.DEBUG, f"Called recv_data, got {ret}")
     return ret
 
   def recv_last_data(self, fill_missing: bool = True) -> Dict[str, Any]:
-    """Reads all the available values from each incoming Link, and returns
-    the newest ones in a single dict.
+    """Reads all the available values from each incoming
+    :class:`~crappy.links.Link`, and returns the newest ones in a single dict.
 
     The returned :obj:`dict` might not always have a fixed number of keys,
     depending on the availability of incoming data.
 
     Important:
-      If data is received over a same label from different links, part of it
+      If data is received over a same label from different Links, part of it
       will be lost ! Always avoid using a same label twice in a Crappy script.
 
     Args:
       fill_missing: If :obj:`True`, fills up the missing data for the known
         labels. This way, the last value received from all known labels is
         always returned. It can of course not fill up missing data for labels
-        that haven(t been received yet.
+        that haven't been received yet.
 
     Returns:
       A :obj:`dict` whose keys are the received labels and with a single value
       for each key (usually a :obj:`float` or a :obj:`str`).
     """
 
     # Initializing the buffer storing the last received values
@@ -952,22 +1012,22 @@
 
     self.log(logging.DEBUG, f"Called recv_last_data, got {ret}")
     return ret
 
   def recv_all_data(self,
                     delay: Optional[float] = None,
                     poll_delay: float = 0.1) -> Dict[str, List[Any]]:
-    """Reads all the available values from each incoming Link, and returns
-    them all in a single dict.
+    """Reads all the available values from each incoming
+    :class:`~crappy.links.Link`, and returns them all in a single dict.
 
     The returned :obj:`dict` might not always have a fixed number of keys,
     depending on the availability of incoming data.
 
     Important:
-      If data is received over a same label from different links, part of it
+      If data is received over a same label from different Links, part of it
       will be lost ! Always avoid using a same label twice in a Crappy script.
       See the :meth:`recv_all_data_raw` method for receiving data with no loss.
 
     Warning:
       As the time label is (normally) shared between all Blocks, the values
       returned for this label will be inconsistent and shouldn't be used !
 
@@ -979,15 +1039,15 @@
       poll_delay: If the ``delay`` argument is given, the Links will be polled
         once every this value seconds. It ensures that the method doesn't spam
         the CPU in vain.
 
     Returns:
       A :obj:`dict` whose keys are the received labels and with a :obj:`list`
       of received values for each key. The first item in the list is the oldest
-      one available in the link, the last item is the newest available.
+      one available in the Link, the last item is the newest available.
     """
 
     ret = defaultdict(list)
     t0 = time()
 
     # If simple recv_all, just receiving from all input links
     if delay is None:
@@ -1009,16 +1069,17 @@
     # Returning a dict, not a defaultdict
     self.log(logging.DEBUG, f"Called recv_all_data, got {dict(ret)}")
     return dict(ret)
 
   def recv_all_data_raw(self,
                         delay: Optional[float] = None,
                         poll_delay: float = 0.1) -> List[Dict[str, List[Any]]]:
-    """Reads all the available values from each incoming Link, and returns
-    them separately in a list of dicts.
+    """Reads all the available values from each incoming
+    :class:`~crappy.links.Link`, and returns them separately in a list of
+    dicts.
 
     Unlike :meth:`recv_all_data` this method does not fuse the received data
     into a single :obj:`dict`, so it is guaranteed to return all the available
     data with no loss.
 
     Args:
       delay: If given specifies a delay, as a :obj:`float`, during which the
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/meta_block/meta_block.py` & `crappy-2.0.0.dev2/src/crappy/blocks/meta_block/meta_block.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # coding: utf-8
 
 from ..._global import DefinitionError
 
 
 class MetaBlock(type):
-  """"""
+  """Metaclass ensuring that two Blocks don't have the same name, and that all
+  Blocks define the required methods. Also keeps track of all the Block
+  classes, including the custom user-defined ones."""
 
   existing = list()
 
   def __new__(mcs, name: str, bases: tuple, dct: dict) -> type:
     return super().__new__(mcs, name, bases, dct)
 
   def __init__(cls, name: str, bases: tuple, dct: dict) -> None:
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/multiplex.py` & `crappy-2.0.0.dev2/src/crappy/blocks/multiplexer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,69 +1,91 @@
 # coding: utf-8
+import logging
 
 import numpy as np
-from typing import Dict, Optional, List
+from typing import Dict, Optional, Iterable, Union
 from collections import defaultdict
 
 from .meta_block import Block
 
 
-class Multiplex(Block):
-  """This block takes data from upstream blocks as input and interpolates it to
-  output all labels in a common time basis.
-
-  It is useful for synchronizing data acquired from different sensors, e.g. to
-  plot a real-time stress-strain curve. This block is however quite
-  resource-consuming, so it is preferable to perform interpolation in
+class Multiplexer(Block):
+  """This Block takes data from upstream Blocks as input and interpolates it to
+  output all the labels in a common time basis.
+
+  It can take any number of inputs, provided that they all share a common time
+  label. It is also possible to choose which labels are considered for
+  multiplexing and which are dropped. The interpolation is performed using the
+  :obj:`numpy.interp` method.
+
+  This Block is useful for synchronizing data acquired from different sensors,
+  e.g. to plot a real-time stress-strain curve with position data coming from a
+  :class:`~crappy.blocks.Machine` Block and force data coming from a
+  :class:`~crappy.blocks.IOBlock` Block. Multiplexing is however quite
+  resource-consuming, so it is preferable to perform interpolation when
   post-processing if real-time is not needed.
 
   Note:
-    This block doesn't truly output data in real-time as it needs to wait for
-    data from all the upstream blocks before performing the interpolation.
-    So it should only be used with care when it is an input of a
-    decision-making block. This is especially true when the upstream blocks
-    have very different sample rates.
+    This Block doesn't truly output data in real-time as it needs to wait for
+    data from all the upstream Blocks before performing the interpolation. It
+    should only be used with care as an input to a decision-making Block. This
+    is especially true when the upstream Blocks have very different sampling
+    rates.
   """
 
   def __init__(self,
                time_label: str = 't(s)',
-               out_labels: Optional[List[str]] = None,
+               out_labels: Optional[Union[str, Iterable[str]]] = None,
                interp_freq: float = 200,
-               freq: float = 50,
+               freq: Optional[float] = 50,
                display_freq: bool = False,
                debug: Optional[bool] = False) -> None:
-    """Sets the args and initializes the parent class.
+    """Sets the arguments and initializes the parent class.
 
     Args:
       time_label: The label carrying the time information.
-      out_labels: If given, the Block won't output anything until data has been
-        received on all these labels. The time label should not be included in
-        this list, as it is already given in the ``time_label`` argument. It is
-        recommended to always specify this argument.
-      freq : The sample rate for the interpolation, and the target looping
-        frequency for the block. If this value is set too high and your machine
-        cannot keep up, the block will most likely lag.
-      display_freq: If :obj:`True`, displays information about the looping
-        frequency of the block.
+      out_labels: An iterable (like a :obj:`list` or a :obj:`tuple`) containing
+        the labels to multiplex, except for the time label that is given
+        separately in the ``time_label`` argument. The Block also doesn't
+        output anything until data has been received on all these labels. If
+        left to :obj:`None`, all the received labels are considered. **It is
+        recommended to always set this argument !** It is also possible to
+        give this argument as a single :obj:`str` (i.e. not in an iterable),
+        although multiplexing a single label is of limited interest.
+      freq: The target looping frequency for the Block. If :obj:`None`, loops 
+        as fast as possible.
+      display_freq: If :obj:`True`, displays the looping frequency of the
+        Block.
+      debug: If :obj:`True`, displays all the log messages including the
+        :obj:`~logging.DEBUG` ones. If :obj:`False`, only displays the log
+        messages with :obj:`~logging.INFO` level or higher. If :obj:`None`,
+        disables logging for this Block.
     """
 
     super().__init__()
     self.freq = freq
     self.display_freq = display_freq
     self.debug = debug
 
     # Initializing the attributes
     self._time_label = time_label
-    self._out_labels = out_labels
     self._interp_freq = interp_freq
     self._data: Dict[str, np.ndarray] = defaultdict(self._default_array)
 
+    # Forcing the out_labels into a list
+    if out_labels is not None and isinstance(out_labels, str):
+      self._out_labels = [out_labels]
+    elif out_labels is not None:
+      self._out_labels = list(out_labels)
+    else:
+      self._out_labels = None
+
   def loop(self) -> None:
     """Receives data, interpolates it, and sends it to the downstream
-    blocks."""
+    Blocks."""
 
     # Receiving all the upcoming data
     data = self.recv_all_data_raw()
 
     # Iterating over all the links
     for link_data in data:
       # Only data associated with a time label can be multiplexed
@@ -93,16 +115,17 @@
     if self._out_labels is not None:
       if not all(label in self._data for label in self._out_labels):
         return
       elif not all(np.any(self._data[label]) for label in self._out_labels):
         return
 
     # Making sure there's data for all the labels
-    if not self ._data or all(not np.any(data)
-                              for data in self._data.values()):
+    if not self._data or any(not np.any(data) for data in self._data.values()):
+      self.log(logging.DEBUG, "At least one label doesn't have a value in "
+                              "buffer, not returning anything for this loop")
       return
 
     # Getting the minimum time for the interpolation
     min_t = min(np.min(data[0]) for data in self._data.values())
     # Correcting to the closest lower multiple of the time interval
     min_t = min_t - min_t % (1 / self._interp_freq)
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/reader.py` & `crappy-2.0.0.dev2/src/crappy/blocks/sink.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,41 @@
 # coding: utf-8
 
 from typing import Optional
-import logging
 
 from .meta_block import Block
 
 
-class Reader(Block):
-  """Reads and displays the data flowing through the input :ref:`Link`."""
-
-  _index = 0
+class Sink(Block):
+  """This Block drops all the data it receives, and does nothing else.
+  
+  It is only useful for debugging, e.g. with Blocks like the
+  :class:`~crappy.blocks.IOBlock` that have a different behavior when they have
+  output Links.
+  """
 
   def __init__(self,
-               name: Optional[str] = None,
-               freq: float = 50,
                display_freq: bool = False,
+               freq: Optional[float] = 10,
                debug: Optional[bool] = False) -> None:
-    """Sets the arg and initializes the parent class.
-
+    """Sets the arguments and initializes the parent class.
+    
     Args:
-      name: If set, will be displayed to identify the reader.
-      freq: The block will try to loop at this frequency.
-      display_freq: If :obj:`True`, the looping frequency will be displayed
-        every 2s.
+      display_freq: If :obj:`True`, displays the looping frequency of the
+        Block.
+      freq: The target looping frequency for the Block. If :obj:`None`, loops 
+        as fast as possible.
+      debug: If :obj:`True`, displays all the log messages including the
+        :obj:`~logging.DEBUG` ones. If :obj:`False`, only displays the log
+        messages with :obj:`~logging.INFO` level or higher. If :obj:`None`,
+        disables logging for this Block.
     """
 
     super().__init__()
-    self.freq = freq
     self.display_freq = display_freq
+    self.freq = freq
     self.debug = debug
 
-    self._reader_name = name if name is not None else f'Reader ' \
-                                                      f'{self._get_index()}'
-
-  def __new__(cls, *args, **kwargs):
-    """"""
-
-    cls._index += 1
-    return super().__new__(cls)
-
-  @classmethod
-  def _get_index(cls) -> int:
-    """Returns the current number of instantiates Links, as an :obj:`int`."""
-
-    return cls._index
-
   def loop(self) -> None:
-    """Simply flushes the link and displays its data."""
+    """Drops all the received data."""
 
-    data = self.recv_all_data_raw()
-    for link_data in data:
-      for dic in (dict(i) for i in
-                  zip(*([(key, value) for value in values]
-                        for key, values in link_data.items()))):
-        self.log(logging.INFO, f'{self._reader_name} got: {dic}')
+    self.recv_all_data_raw()
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/recorder.py` & `crappy-2.0.0.dev2/src/crappy/blocks/recorder.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,84 @@
 # coding: utf-8
 
-from typing import List, Optional, Union
+from typing import Iterable, Optional, Union
 from pathlib import Path
 import logging
 
 from .meta_block import Block
 
 
 class Recorder(Block):
-  """Saves data from an upstream block to a text file, with values separated by
-  a coma and lines by a newline character.
+  """This Block saves data from an upstream Block to a text file, with values 
+  separated by a coma and lines by a newline character.
 
-  The first row of the file contains the names of the saved labels.
-  This block can only save data coming from one upstream block. To save data
-  from multiple blocks, use several instances of Recorder (recommended) or a
-  :ref:`Multiplexer` block.
+  The first row of the file contains the names of the saved labels. This Block 
+  can only save data coming from exactly one upstream Block. To save data
+  from multiple Blocks, use several instances of Recorder (recommended) or a
+  :class:`~crappy.blocks.Multiplexer` Block.
+  
+  This Block cannot directly record data from "streams", i.e. coming from an
+  :class:`~crappy.blocks.IOBlock` Block with the ``'streamer'`` argument set to
+  :obj:`True`. To do so, the :class:`~crappy.blocks.HDFRecorder` Block should
+  be used instead. Alternatively, a :class:`~crappy.modifier.Demux` Modifier 
+  can be placed between the IOBlock and the Recorder, but most of the acquired
+  data won't be saved.
   """
 
   def __init__(self,
                file_name: Union[str, Path],
                delay: float = 2,
-               labels: Optional[List[str]] = None,
+               labels: Optional[Union[str, Iterable[str]]] = None,
                time_label: str = 't(s)',
-               freq: float = 200,
-               display_freq: bool = True,
+               freq: Optional[float] = 200,
+               display_freq: bool = False,
                debug: Optional[bool] = False) -> None:
-    """Sets the args and initializes the parent class.
+    """Sets the arguments and initializes the parent class.
 
     Args:
       file_name: Path to the output file, either relative or absolute. If the
         parent folders of the file do not exist, they will be created. If the
         file already exists, the actual file where data will be written will be
         renamed with a trailing index to avoid overriding it.
       delay: Delay between each write in seconds.
       labels: If provided, only the data carried by these labels will be saved.
         Otherwise, all the received data is saved.
       time_label: The label carrying the time information, by default `'t(s)'`.
-      freq: The block will try to loop at this frequency.
+      freq: The target looping frequency for the Block. If :obj:`None`, loops 
+        as fast as possible.
       display_freq: If :obj:`True`, displays the looping frequency of the
-        block.
+        Block.
+      debug: If :obj:`True`, displays all the log messages including the 
+        :obj:`~logging.DEBUG` ones. If :obj:`False`, only displays the log
+        messages with :obj:`~logging.INFO` level or higher. If :obj:`None`,
+        disables logging for this Block.
     """
 
     super().__init__()
     self.niceness = -5
     self.freq = freq
     self.display_freq = display_freq
     self.debug = debug
 
     self._delay = delay
     self._path = Path(file_name)
-    self._labels = labels
     self._time_label = time_label
 
+    # Forcing the labels into a list
+    if labels is not None and isinstance(labels, str):
+      self._labels = [labels]
+    elif labels is not None:
+      self._labels = list(labels)
+    else:
+      self._labels = None
+
     self._file_initialized = False
 
   def prepare(self) -> None:
-    """Checking that the block has the right number of inputs, creates the
+    """Checks that the Block has the right number of inputs, creates the
     folder containing the file if it doesn't already exist, and changes the
     name of the file if it already exists."""
 
     # Making sure there's the right number of incoming links
     if not self.inputs:
       raise ValueError('The Recorder block does not have inputs !')
     elif len(self.inputs) > 1:
@@ -82,15 +101,15 @@
       while Path.exists(parent_folder / f'{stem}_{i:05d}{suffix}'):
         i += 1
       self._path = parent_folder / f'{stem}_{i:05d}{suffix}'
       self.log(logging.WARNING, f"Writing data to the file {self._path} "
                                 f"instead !")
 
   def loop(self) -> None:
-    """Simply receives data from the upstream block and saves it."""
+    """Receives data from the upstream Block and saves it."""
 
     if not self._file_initialized:
       if self.data_available():
 
         data = self.recv_all_data(delay=self._delay)
 
         # If no labels are given, save everything that's received
```

### Comparing `crappy-2.0.0.dev1/src/crappy/blocks/ucontroller.py` & `crappy-2.0.0.dev2/src/crappy/blocks/ucontroller.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 from struct import unpack
 from time import time
-from typing import Optional, List, Dict, Callable
+from typing import Optional, Dict, Callable, Iterable, Union
 import logging
 
 from .meta_block import Block
 from .._global import OptionalModule
 
 try:
   from serial import Serial
@@ -17,63 +17,72 @@
 
 
 class UController(Block):
   """Block for interfacing over serial with an external device, written mostly
   for communication with microcontrollers.
 
   It can send labeled commands to the device, and/or receive labeled data from
-  it. This block is meant to be used along with the MicroController.py
+  it. This Block is meant to be used along with the `microcontroller.py`
   MicroPython template located in the `tool` folder of Crappy, even though it
   is not mandatory. A given syntax needs to be followed for any data to be
   exchanged.
   """
 
   def __init__(self,
-               labels: Optional[List[str]] = None,
-               cmd_labels: Optional[List[str]] = None,
+               labels: Optional[Union[str, Iterable[str]]] = None,
+               cmd_labels: Optional[Union[str, Iterable[str]]] = None,
                init_output: Optional[Dict[str, float]] = None,
                post_process: Optional[Dict[str,
                                            Callable[[float], float]]] = None,
                t_device: bool = False,
                port: str = '/dev/ttyUSB0',
                baudrate: int = 115200,
                display_freq: bool = False,
-               freq: float = 100,
+               freq: Optional[float] = 100,
                debug: Optional[bool] = False) -> None:
     """Checks the validity of the arguments.
 
     Args:
-      labels (:obj:`list`, optional): The list of the labels to get from the
-        device. Only these labels should be given as argument to the
-        :meth:`send_to_pc` method in the MicroPython script. If this argument
-        is not :obj:`None`, then the``init_output`` argument should be given as
-        well. No more than 9 labels should be given.
-      cmd_labels (:obj:`list`, optional): The list of the command labels that
-        will be sent to the device upon reception from an upstream block. The
-        variables in the MicroPython script should have these exact names. No
-        more than 9 cmd_labels should be given.
-      init_output (:obj:`dict`, optional): If the ``labels`` argument is not
-        :obj:`None`, the values to output to downstream blocks for each label
-        as long as no value has been received from the device. An initial
-        output value must be given for each label.
-      post_process (:obj:`dict`, optional): Optionally allows applying a
-        function to the data of a label before transmitting it to downstream
-        blocks. It is possible to give functions for only part of the labels.
-      t_device (:obj:`bool`, optional): It :obj:`True`, the timestamp returned
-        under the label `'t(s)'` is the one of the device, not the one of
-        Crappy. It may reduce the maximum achievable sample rate, as more bytes
-        have to be transmitted, but it is also far more precise.
-      port (:obj:`str`, optional): The serial port to open for communicating
-        with the device. In Windows, they are usually called `COMx`, whereas in
-        Linux and Mac they're called `/dev/ttyxxxx`.
-      baudrate (:obj:`int`, optional): The baudrate for serial communication.
-        It depends on the capabilities of the device.
-      display_freq (:obj:`bool`, optional): If :obj:`True`, displays the
-        looping frequency of the block.
-      freq (:obj:`float`, optional): The looping frequency of the block.
+      labels: An iterable (like a :obj:`list` or a :obj:`tuple`) containing the
+        labels to get from the device (as :obj:`str`). Only these labels should
+        be given as argument to the :meth:`send_to_pc` method in the
+        MicroPython script. If this argument is not :obj:`None`, then the
+        ``init_output`` argument should be given as well. No more than 9 labels
+        should be given. If there's only one label to acquire, it can be given
+        directly as a :obj:`str` and not in an iterable.
+      cmd_labels: An iterable (like a :obj:`list` or a :obj:`tuple`) containing
+        the command labels that will be sent to the device upon reception from
+        an upstream Block. The variables in the MicroPython script should have
+        these exact names. Not more than 9 cmd_labels should be given. If
+        there's only one command label, it can be given directly as a
+        :obj:`str` and not in an iterable.
+      init_output: If the ``labels`` argument is not :obj:`None`, the values to 
+        output to downstream Blocks for each label as long as no value has been 
+        received from the device. An initial output value must be given for 
+        each label.
+      post_process: Optionally allows applying a function to the data of a 
+        label before transmitting it to downstream Blocks. It is possible to 
+        give functions for only part of the labels.
+      t_device: It :obj:`True`, the timestamp returned under the label `'t(s)'` 
+        is the one of the device, not the one of Crappy. It may reduce the 
+        maximum achievable sample rate, as more bytes have to be transmitted, 
+        but it is also far more precise.
+      port: The serial port to open for communicating with the device. In 
+        Windows, they are usually called `COMx`, whereas in Linux and Mac 
+        they're called `/dev/ttyxxxx`.
+      baudrate: The baudrate for serial communication. It depends on the 
+        capabilities of the device.
+      display_freq: If :obj:`True`, displays the looping frequency of the
+        Block.
+      freq: The target looping frequency for the Block. If :obj:`None`, loops 
+        as fast as possible.
+      debug: If :obj:`True`, displays all the log messages including the
+        :obj:`~logging.DEBUG` ones. If :obj:`False`, only displays the log
+        messages with :obj:`~logging.INFO` level or higher. If :obj:`None`,
+        disables logging for this Block.
     """
 
     self._bus = None
 
     super().__init__()
     self.debug = debug
 
@@ -93,33 +102,43 @@
       raise TypeError("port should be a string !")
     self._port = port
 
     if not isinstance(baudrate, int) or baudrate < 0:
       raise ValueError("baudrate should be a positive integer !")
     self._baudrate = baudrate
 
-    if labels is not None and not isinstance(labels, list):
-      raise TypeError('labels should be a list !')
-    if labels is not None and len(labels) > 9:
+    # Forcing the labels into a list
+    if labels is not None and isinstance(labels, str):
+      self._labels = [labels]
+    elif labels is not None:
+      self._labels = list(labels)
+    else:
+      self._labels = None
+
+    # Forcing the cmd_labels into a list
+    if cmd_labels is not None and isinstance(cmd_labels, str):
+      self._cmd_labels = [cmd_labels]
+    elif cmd_labels is not None:
+      self._cmd_labels = list(cmd_labels)
+    else:
+      self._cmd_labels = None
+
+    if self._labels is not None and len(self._labels) > 9:
       raise ValueError("Sorry, a maximum of 9 labels is allowed !")
-    if cmd_labels is not None and not isinstance(cmd_labels, list):
-      raise TypeError('cmd_labels should be a list !')
-    if cmd_labels is not None and len(cmd_labels) > 9:
+    if self._cmd_labels is not None and len(self._cmd_labels) > 9:
       raise ValueError("Sorry, a maximum of 9 cmd_labels is allowed !")
-    self._labels = labels
-    self._cmd_labels = cmd_labels
 
     if self._cmd_labels is not None:
       self._prev_cmd = {cmd_label: None for cmd_label in self._cmd_labels}
 
     if init_output is not None and not isinstance(init_output, dict):
       raise TypeError("init_output should be a dict !")
-    if labels is not None and not all(label in (init_output if init_output
-                                                is not None else {})
-                                      for label in labels):
+    if self._labels is not None and not all(
+        label in (init_output if init_output is not None else dict())
+        for label in self._labels):
       raise ValueError("Every label should have an init_output value !")
     self._out = init_output
 
     if post_process is not None and (not isinstance(post_process, dict) or
                                      not all(callable(func) for func
                                              in post_process.values())):
       raise TypeError("post_process should be a dict of callables !")
@@ -223,16 +242,16 @@
         self._bus.write(msg)
         self.log(logging.DEBUG, f"Sent {msg} on the port {self._port}")
       except SerialException:
         raise IOError(f"Writing to the device on port {self._port} failed, "
                       f"it may have been disconnected.")
 
   def loop(self) -> None:
-    """First sends the commands from upstream blocks to the device, then reads
-    the data from the device and sends it to the downstream blocks.
+    """First sends the commands from upstream Blocks to the device, then reads
+    the data from the device and sends it to the downstream Blocks.
 
     Important:
       The precision of the commands sent to the device is limited to 3 digits
       after the decimal point, to limit the traffic on the bus. Adapt the range
       of the command values consequently.
 
     Note:
```

### Comparing `crappy-2.0.0.dev1/src/crappy/camera/__init__.py` & `crappy-2.0.0.dev2/src/crappy/camera/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # coding: utf-8
 
 from typing import Dict, Type
 
-# Parent class
-from .meta_camera import Camera, MetaCamera, camera_setting
-# Virtual cameras
 from .fake_camera import FakeCamera
 from .file_reader import FileReader
-# Physical cameras
-from .webcam import Webcam
-from .xiapi import XiAPI
-from .pi_camera import PiCamera
-from .gstreamer import CameraGstreamer
-from .opencv import CameraOpencv
-# Cameralink cameras
-from .cameralink import CLCamera
-from .cameralink import BiSpectral
-from .cameralink import Jai, Jai8
+from .gstreamer_camera import CameraGstreamer
+from .opencv_camera import CameraOpencv
+from .opencv_camera_basic import Webcam
+from .raspberry_pi_camera import RaspberryPiCamera
 from .seek_thermal_pro import SeekThermalPro
+from .ximea_xiapi import XiAPI
+
+from .cameralink import BaslerIronmanCameraLink
+from .cameralink import JaiGO5000CPMCL, JaiGO5000CPMCL8Bits
+
+from .meta_camera import Camera, MetaCamera, camera_setting
 
 camera_dict: Dict[str, Type[Camera]] = MetaCamera.classes
```

### Comparing `crappy-2.0.0.dev1/src/crappy/camera/cameralink/bispectral.py` & `crappy-2.0.0.dev2/src/crappy/lamcube/bispectral.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 
 import numpy as np
 from typing import Tuple
 import logging
 
-from .cameralink import CLCamera
+from ..camera.cameralink import BaslerIronmanCameraLink
 
 table = (0x0000, 0xC0C1, 0xC181, 0x0140, 0xC301, 0x03C0, 0x0280, 0xC241,
          0xC601, 0x06C0, 0x0780, 0xC741, 0x0500, 0xC5C1, 0xC481, 0x0440,
          0xCC01, 0x0CC0, 0x0D80, 0xCD41, 0x0F00, 0xCFC1, 0xCE81, 0x0E40,
          0x0A00, 0xCAC1, 0xCB81, 0x0B40, 0xC901, 0x09C0, 0x0880, 0xC841,
          0xD801, 0x18C0, 0x1980, 0xD941, 0x1B00, 0xDBC1, 0xDA81, 0x1A40,
          0x1E00, 0xDEC1, 0xDF81, 0x1F40, 0xDD01, 0x1DC0, 0x1C80, 0xDC41,
@@ -45,216 +45,239 @@
 
     for ch in st:
         crc = (crc >> 8) ^ table[(crc ^ ord(ch)) & 0xFF]
     return crc
 
 
 def add_crc(s: str) -> str:
+  """Wrapper for adding a CRC to a serial command."""
+
   return s + hex(calc_string(s, 0xFFFF)).split('x')[1].upper().rjust(4, '0')
 
 
 def check_crc(s: str) -> bool:
+  """Wrapper for checking whether a CRC is valid."""
+
   r = s[:-4]
   return add_crc(r) == s
 
 
 def hexlify(n: int) -> str:
+  """Converts an integer to its hexadecimal representation."""
+
   return hex(n).split('x')[1].rjust(2, '0').upper()
 
 
-class BiSpectral(CLCamera):
-  """"""
+class BiSpectral(BaslerIronmanCameraLink):
+  """This class allows driving a bi-chromatic infrared camera, through a Basler
+  microEnable 5 Ironman AD8 PoCL acquisition board.
+
+  It is a child of the
+  :class:`~crappy.camera.cameralink.BaslerIronmanCameraLink` Camera. It can set
+  various settings on the camera, including the ROI or the trigger mode.
+
+  The bi-chromatic camera is a very specific setup, and won't certainly be ever
+  used outside the LaMcube laboratory. This is why it is stored in the LaMcube
+  submodule.
+
+  Warning:
+    This Camera relies on a custom-written C library that hasn't been tested in
+    a long time. It might not be functional anymore. This Camera also requires
+    proprietary drivers to be installed.
+  """
 
   def __init__(self) -> None:
-    """"""
+    """Adds the various setting for the Camera."""
 
     super().__init__()
     self.add_scale_setting('width', 1, 640, self._get_w, self._set_w, 640)
     self.add_scale_setting('height', 1, 512, self._get_h, self._set_h, 512)
     self.add_scale_setting('xoffset', 0, 1278, self._get_ox, self._set_ox, 0)
     self.add_scale_setting('yoffset', 0, 511, self._get_oy, self._set_oy, 0)
     self.add_scale_setting('IT1', 10, 10000, self._get_it1, self._set_it1)
     self.add_scale_setting('IT2', 10, 10000, self._get_it2, self._set_it2)
-    self.add_scale_setting('fps', 1., 150., self.get_trigg_freq,
-                           self.set_trigg_freq)
-    self.add_trigger_setting(setter=self.set_external_trigger)
+    self.add_scale_setting('fps', 1., 150., self._get_trigg_freq,
+                           self._set_trigg_freq)
+    self.add_trigger_setting(setter=self._set_external_trigger)
 
   def open(self,
            camera_type: str = 'SingleAreaGray2DShading',
            **kwargs) -> None:
-    """"""
+    """Opens the Camera and sends initialization commands."""
 
     super().open(camera_type=camera_type, **kwargs)
 
-    self.send_cmd('@W1A084')  # Restore unwindowed Mode
-    self.send_cmd('@W10012')  # Make sure the image is not inverted
+    self._send_cmd('@W1A084')  # Restore unwindowed Mode
+    self._send_cmd('@W10012')  # Make sure the image is not inverted
 
   def get_image(self) -> Tuple[float, np.ndarray]:
-    """"""
+    """Grabs an image using the parent class' method, transforms it, and
+    returns it."""
 
-    metadata, frame = super().get_image()
+    t, frame = super().get_image()
     img = np.ones((self.height, self.width * 2), dtype=np.uint8)
     img[::, :self.width:2] = frame[::, ::4]
     img[::, 1:self.width:2] = frame[::, 1::4]
     img[::, self.width::2] = frame[::, 2::4]
     img[::, self.width + 1::2] = frame[::, 3::4]
-    return metadata, img
-
-  def _set_w(self, val: int) -> None:
-    super()._set_w(val * 2)
-    self.set_roi(self.xoffset, self.yoffset, self.xoffset + self.width - 1,
-                 self.yoffset + self.height - 1)
+    return t, img
 
-  def _get_w(self) -> int:
-    return int(super()._get_w() / 2)
-
-  def _set_h(self, val: int) -> None:
-    super()._set_h(val)
-    self.set_roi(self.xoffset, self.yoffset, self.xoffset + self.width - 1,
-                 self.yoffset + self.height - 1)
-
-  def _set_ox(self, val: int) -> None:
-    self.set_roi(val, self.yoffset, val + self.width - 1,
-                 self.yoffset + self.height - 1)
-
-  def _set_oy(self, val: int) -> None:
-    self.set_roi(self.xoffset, val, self.xoffset + self.width - 1,
-                 val + self.height - 1)
+  def _send_cmd(self, cmd: str) -> str:
+    """Wrapper for sending a command to the Camera."""
 
-  def _get_ox(self) -> int:
-    return self.get_roi()[0]
-
-  def _get_oy(self) -> int:
-    return self.get_roi()[1]
-
-  def _get_it1(self) -> int:
-    return int(self.get_itT()[0])
-
-  def _get_it2(self) -> int:
-    return int(self.get_it()[1])
-
-  def _set_it1(self, val: int) -> None:
-    self.set_it(val, self._get_it2())
-
-  def _set_it2(self, val: int) -> None:
-    self.set_it(self._get_it1(), val)
-
-  def send_cmd(self, cmd: str) -> str:
     self.log(logging.DEBUG, f"Sending command {cmd}")
-    r = self.cap.serialWrite(add_crc(cmd))
+    r = self._cap.serialWrite(add_crc(cmd))
     if not check_crc(r) or r[1] != 'Y':
       self.log(logging.WARNING, f"Incorrect reply {r}")
     return r[2:4]
 
-  def set_external_trigger(self, val: str) -> None:
+  def _set_external_trigger(self, val: str) -> None:
     """Sets the external trigger to val by toggling the value of the 3rd bit
     of register 102."""
 
     if val == 'Hardware':
-      self.send_cmd('@W1027C')  # 3rd bit to 1
+      self._send_cmd('@W1027C')  # 3rd bit to 1
     else:
-      self.send_cmd('@W10274')  # 3rd bit to 0
+      self._send_cmd('@W10274')  # 3rd bit to 0
 
-  def get_roi(self) -> Tuple[int, int, int, int]:
-    x1min_lsb = self.send_cmd("@R1D0")
-    x1min_msb = self.send_cmd("@R1D1")
-    y1min_lsb = self.send_cmd("@R1D2")
-    y1min_msb = self.send_cmd("@R1D3")
-    x1max_lsb = self.send_cmd("@R1D4")
-    x1max_msb = self.send_cmd("@R1D5")
-    y1max_lsb = self.send_cmd("@R1D6")
-    y1max_msb = self.send_cmd("@R1D7")
+  def _get_roi(self) -> Tuple[int, int, int, int]:
+    """Returns the minimum and maximum x and y coordinates of the current
+    ROI."""
+
+    x1min_lsb = self._send_cmd("@R1D0")
+    x1min_msb = self._send_cmd("@R1D1")
+    y1min_lsb = self._send_cmd("@R1D2")
+    y1min_msb = self._send_cmd("@R1D3")
+    x1max_lsb = self._send_cmd("@R1D4")
+    x1max_msb = self._send_cmd("@R1D5")
+    y1max_lsb = self._send_cmd("@R1D6")
+    y1max_msb = self._send_cmd("@R1D7")
     xmin = int(x1min_msb + x1min_lsb, 16)
     xmax = int(x1max_msb + x1max_lsb, 16)
     ymin = int(y1min_msb + y1min_lsb, 16)
     ymax = int(y1max_msb + y1max_lsb, 16)
     return xmin, ymin, xmax, ymax
 
-  def set_roi(self, xmin: int, ymin: int, xmax: int, ymax: int) -> None:
+  def _set_roi(self, xmin: int, ymin: int, xmax: int, ymax: int) -> None:
+    """Sets the minimum and maximum x and y coordinates of the ROI."""
+
     if (xmin, xmax, ymin, ymax) != (0, 0, 639, 511):
-      self.send_cmd('@W1A080')  # Set to windowed mode
+      self._send_cmd('@W1A080')  # Set to windowed mode
     else:
-      self.send_cmd('@W1A084')
+      self._send_cmd('@W1A084')
       self.log(logging.INFO, f"D set ROI to {xmin}, {ymin}, {xmax}, {ymax}")
     lsb_xmin = hexlify(xmin % 256)
     msb_xmin = hexlify(xmin // 256)
     lsb_xmax = hexlify(xmax % 256)
     msb_xmax = hexlify(xmax // 256)
     lsb_ymin = hexlify(ymin % 256)
     msb_ymin = hexlify(ymin // 256)
     lsb_ymax = hexlify(ymax % 256)
     msb_ymax = hexlify(ymax // 256)
-    self.send_cmd("@W1D0" + lsb_xmin)
-    self.send_cmd("@W1D1" + msb_xmin)
-    self.send_cmd("@W1D2" + lsb_ymin)
-    self.send_cmd("@W1D3" + msb_ymin)
-    self.send_cmd("@W1D4" + lsb_xmax)
-    self.send_cmd("@W1D5" + msb_xmax)
-    self.send_cmd("@W1D6" + lsb_ymax)
-    self.send_cmd("@W1D7" + msb_ymax)
+    self._send_cmd("@W1D0" + lsb_xmin)
+    self._send_cmd("@W1D1" + msb_xmin)
+    self._send_cmd("@W1D2" + lsb_ymin)
+    self._send_cmd("@W1D3" + msb_ymin)
+    self._send_cmd("@W1D4" + lsb_xmax)
+    self._send_cmd("@W1D5" + msb_xmax)
+    self._send_cmd("@W1D6" + lsb_ymax)
+    self._send_cmd("@W1D7" + msb_ymax)
+
+  def _get_it(self) -> Tuple[float, float]:
+    """Reads the integration time from the Camera and returns it."""
 
-  def get_it(self) -> Tuple[float, float]:
     mc = 10.35  # MHz
-    it1_lsb = self.send_cmd("@R1B4")
-    it1_mid = self.send_cmd("@R1B5")
-    it1_msb = self.send_cmd("@R1B6")
-    it2_lsb = self.send_cmd("@R1B8")
-    it2_mid = self.send_cmd("@R1B9")
-    it2_msb = self.send_cmd("@R1BA")
+    it1_lsb = self._send_cmd("@R1B4")
+    it1_mid = self._send_cmd("@R1B5")
+    it1_msb = self._send_cmd("@R1B6")
+    it2_lsb = self._send_cmd("@R1B8")
+    it2_mid = self._send_cmd("@R1B9")
+    it2_msb = self._send_cmd("@R1BA")
     it1 = int(it1_msb + it1_mid + it1_lsb, 16)  # Number of clock cycles
     it2 = int(it2_msb + it2_mid + it2_lsb, 16)
     return it1 / mc, it2 / mc  # IT in µs
 
-  def set_it(self, it1: int, it2: int) -> None:
+  def _set_it(self, it1: int, it2: int) -> None:
+    """Sets the integration time on the Camera."""
+
     mc = 10.35
     it1 = int(mc * it1)
     it2 = int(mc * it2)
     it1_lsb = hexlify(it1 % 256)
     it1 -= it1 % 256
     it1 //= 256
     it1_mid = hexlify(it1 % 256)
     it1_msb = hexlify(it1 // 256)
     it2_lsb = hexlify(it2 % 256)
     it2 -= it2 % 256
     it2 //= 256
     it2_mid = hexlify(it2 % 256)
     it2_msb = hexlify(it2 // 256)
-    self.send_cmd("@W1B4" + it1_lsb)
-    self.send_cmd("@W1B5" + it1_mid)
-    self.send_cmd("@W1B6" + it1_msb)
-    self.send_cmd("@W1B8" + it2_lsb)
-    self.send_cmd("@W1B9" + it2_mid)
-    self.send_cmd("@W1BA" + it2_msb)
+    self._send_cmd("@W1B4" + it1_lsb)
+    self._send_cmd("@W1B5" + it1_mid)
+    self._send_cmd("@W1B6" + it1_msb)
+    self._send_cmd("@W1B8" + it2_lsb)
+    self._send_cmd("@W1B9" + it2_mid)
+    self._send_cmd("@W1BA" + it2_msb)
+
+  def _get_trigg_freq(self) -> float:
+    """Reads the trigger frequency from the Camera."""
 
-  def get_trigg_freq(self) -> float:
     mc = 10350000  # Hz
-    p_lsb = self.send_cmd("@R1B0")
-    p_mid = self.send_cmd("@R1B1")
-    p_msb = self.send_cmd("@R1B2")
+    p_lsb = self._send_cmd("@R1B0")
+    p_mid = self._send_cmd("@R1B1")
+    p_msb = self._send_cmd("@R1B2")
     p = int(p_msb + p_mid + p_lsb, 16)
     return mc / p
 
-  def set_trigg_freq(self, freq: float) -> None:
+  def _set_trigg_freq(self, freq: float) -> None:
+    """Sets the trigger frequency on the Camera."""
+
     mc = 10350000  # Hz
     period = int(mc / freq)
     p_lsb = hexlify(period % 256)
     period -= period % 256
     period //= 256
     p_mid = hexlify(period % 256)
     p_msb = hexlify(period // 256)
-    self.send_cmd("@W1B0" + p_lsb)
-    self.send_cmd("@W1B1" + p_mid)
-    self.send_cmd("@W1B2" + p_msb)
-
-  def get_sensor_temperature(self) -> float:
-    """Returns sensor temperature in Kelvin."""
-
-    gain = .01
-    lsb = self.send_cmd('@R160')
-    msb = self.send_cmd('@R161')
-    return int(msb + lsb, 16) * gain
+    self._send_cmd("@W1B0" + p_lsb)
+    self._send_cmd("@W1B1" + p_mid)
+    self._send_cmd("@W1B2" + p_msb)
+
+  def _set_w(self, val: int) -> None:
+    super()._set_w(val * 2)
+    self._set_roi(self.xoffset, self.yoffset, self.xoffset + self.width - 1,
+                  self.yoffset + self.height - 1)
+
+  def _get_w(self) -> int:
+    return int(super()._get_w() / 2)
+
+  def _set_h(self, val: int) -> None:
+    super()._set_h(val)
+    self._set_roi(self.xoffset, self.yoffset, self.xoffset + self.width - 1,
+                  self.yoffset + self.height - 1)
+
+  def _set_ox(self, val: int) -> None:
+    self._set_roi(val, self.yoffset, val + self.width - 1,
+                  self.yoffset + self.height - 1)
+
+  def _set_oy(self, val: int) -> None:
+    self._set_roi(self.xoffset, val, self.xoffset + self.width - 1,
+                  val + self.height - 1)
+
+  def _get_ox(self) -> int:
+    return self._get_roi()[0]
+
+  def _get_oy(self) -> int:
+    return self._get_roi()[1]
 
-  def get_ambiant_temperature(self) -> float:
-    """Returns temperature of the board in °C."""
+  def _get_it1(self) -> int:
+    return int(self.get_itT()[0])
+
+  def _get_it2(self) -> int:
+    return int(self._get_it()[1])
 
-    t = self.send_cmd('@R173')
-    return int(t, 16)
+  def _set_it1(self, val: int) -> None:
+    self._set_it(val, self._get_it2())
+
+  def _set_it2(self, val: int) -> None:
+    self._set_it(self._get_it1(), val)
```

### Comparing `crappy-2.0.0.dev1/src/crappy/camera/fake_camera.py` & `crappy-2.0.0.dev2/src/crappy/camera/fake_camera.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,39 +10,39 @@
 
 class FakeCamera(Camera):
   """This camera class generates images without requiring any actual camera or
   existing image file.
 
   The generated images are just a gradient of grey levels, with a line moving
   as a function of time. It is possible to tune the dimension of the image, the
-  frame rate and the speed of the line.
+  frame rate and the speed of the moving line.
   """
 
   def __init__(self) -> None:
     """Initializes the parent class and instantiates the settings."""
 
     super().__init__()
     self._frame_nr = -1
 
     self.add_scale_setting('width', 1, 4096, None, self._gen_image, 1280)
     self.add_scale_setting('height', 1, 4096, None, self._gen_image, 1024)
     self.add_scale_setting('speed', 0., 800., None, None, 100.)
     self.add_scale_setting('fps', 0.1, 100., None, None, 50.)
 
+    self._t0 = time()
+    self._t = self._t0
+
   def open(self, **kwargs) -> None:
     """Sets the settings, generates the first image and initializes the time
     counter."""
 
     self.set_all(**kwargs)
 
     self._gen_image()
 
-    self._t0 = time()
-    self._t = self._t0
-
   def get_image(self) -> Tuple[float, np.ndarray]:
     """Returns the updated image, depending only on the current timestamp.
 
     Also includes a waiting loop in order to achieve the right frame rate.
     """
 
     # Waiting in order to achieve the right frame rate
@@ -54,13 +54,13 @@
 
     # Splitting the image to make a moving line
     row = int(self.speed * (self._t - self._t0)) % self.height
     return self._t, np.concatenate((self._img[row:], self._img[:row]), axis=0)
 
   def _gen_image(self, _: Optional[float] = None) -> None:
     """Generates the base gradient image, that will be split and returned
-    in the :meth:`get_image` method"""
+    in the :meth:`get_image` method."""
 
     self.log(logging.DEBUG, "Generating the image")
     self._img = np.arange(self.height) * 255. / self.height
     self._img = np.repeat(self._img.reshape(self.height, 1),
                           self.width, axis=1).astype(np.uint8)
```

### Comparing `crappy-2.0.0.dev1/src/crappy/camera/file_reader.py` & `crappy-2.0.0.dev2/src/crappy/camera/file_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 
 
 class FileReader(Camera):
   """This Camera class reads existing images from a given folder, in the same
   order in which they were acquired.
 
   The name of the images to read must follow the following pattern :
-  ``<frame_nr> <frame_seconds>.<frame_subseconds>.<file_extension>``. This
-  pattern is the same as used for recording images with Crappy, so images
-  recorded via Crappy are readily readable an don't need to be re-named.
+  ``<frame_nr>_<frame_seconds>.<frame_subseconds>.<file_extension>``. This
+  pattern is the same as used for recording images with the
+  :class:`~crappy.blocks.Camera` of Crappy, so images recorded via Crappy are
+  readily readable and don't need to be re-named.
 
   This class tries to read the images at the same framerate as they were
   recorded, although the control of the framerate is not so precise. It might
   be that the images cannot be read fast enough to match the original
   framerate, in which case the images are read as fast as possible and the
   delay keeps growing.
   """
@@ -60,17 +61,17 @@
       reader_backend: The backend to use for reding the images. Should be one
         of :
         ::
 
           'sitk' or 'cv2'
 
         If not given, SimpleITK is preferred over OpenCV if available.
-      stop_at_end: If :obj:`True` (the default), stops the Crappy test once the
-        available images are all exhausted. Otherwise, simply does nothing
-        while waiting for the test to end.
+      stop_at_end: If :obj:`True` (the default), stops the Crappy script once
+        the available images are all exhausted. Otherwise, simply remains idle
+        while waiting for the test to finish.
     """
 
     # Selecting an  available backend between first sitk and then cv2
     if reader_backend is None:
       if not isinstance(Sitk, OptionalModule):
         self._backend = 'sitk'
       elif not isinstance(cv2, OptionalModule):
@@ -118,15 +119,15 @@
     """Reads the next image in the image folder, and returns it at the right
     time so that the achieved framerate matches the original framerate.
 
     If the original framerate cannot be achieved, just reads the image as fast
     as possible.
 
     By default, stops the test when there's no image left to read. If specified
-    otherwise, just does nothing until the test ends.
+    otherwise, just remains idle until the test ends.
     """
 
     # Setting the approximate start time (potentially not well synced with the
     # actual t0 of Crappy's blocks)
     if self._t0 is None:
       self._t0 = time()
```

### Comparing `crappy-2.0.0.dev1/src/crappy/camera/gstreamer.py` & `crappy-2.0.0.dev2/src/crappy/camera/gstreamer_camera.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # coding: utf-8
 
 from time import time, sleep
 from numpy import uint8, ndarray, uint16, copy, squeeze
-from typing import Tuple, Optional, Union
+from typing import Tuple, Optional, Union, List
 from subprocess import Popen, PIPE, run
 from platform import system
 from re import findall, split, search
 import logging
+from fractions import Fraction
 
 from .meta_camera import Camera
 from .._global import OptionalModule
 
 try:
   import cv2
 except (ImportError, ModuleNotFoundError):
@@ -22,49 +23,60 @@
   require_version('Gst', '1.0')
   require_version('GstApp', '1.0')
   from gi.repository import Gst, GstApp
 except (ImportError, ModuleNotFoundError, ValueError):
   Gst = GstApp = OptionalModule('gi', 'You need to install the python bindings'
                                       ' for GStreamer ! ')
 
-# Todo: Error with a getter
-
 
 class CameraGstreamer(Camera):
   """A class for reading images from a video device using Gstreamer.
 
   It can read images from the default video source, or a video device can be
   specified. In this case, the user has access to a range of parameters for
   tuning the image. Alternatively, it is possible to give a custom GStreamer
-  pipeline to the block. In this case no settings are available, and it is up
+  pipeline as an argument. In this case no settings are available, and it is up
   to the user to ensure the validity of the pipeline.
 
   This class uses less resources and is compatible with more cameras than the
-  :ref:`Camera OpenCV` camera, that relies on OpenCV. The installation of
-  GStreamer of however less straightforward than the one of OpenCV.
+  :class:`~crappy.camera.CameraOpencv` camera, that relies on OpenCV. The
+  installation of GStreamer is however less straightforward than the one of
+  OpenCV.
 
   Note:
     For a better performance of this class in Linux, it is recommended to have
     `v4l-utils` installed.
+
+  Note:
+    This Camera requires the module :mod:`gst-python3-1.0` to be installed, as
+    well as GStreamer.
   """
 
   def __init__(self) -> None:
     """Simply initializes the instance attributes."""
 
     super().__init__()
 
-    self._exposure_mode = None
-    self._pipeline = None
-    self._process: Optional[Popen] = None
-
     Gst.init(None)
-
     self._last_frame_nr = 0
     self._frame_nr = 0
-    self._img = None
+
+    # These attributes will be set later
+    self._exposure_mode: Optional[str] = None
+    self._pipeline = None
+    self._process: Optional[Popen] = None
+    self._img: Optional[ndarray] = None
+    self._device: Optional[Union[str, int]] = None
+    self._user_pipeline: Optional[str] = None
+    self._nb_channels: int = 3
+    self._img_depth: int = 8
+    self._exposure_setting: str = ''
+    self._exposure_auto: str = ''
+    self._formats: List[str] = list()
+    self._app_sink = None
 
   def open(self,
            device: Optional[Union[int, str]] = None,
            user_pipeline: Optional[str] = None,
            nb_channels: Optional[int] = None,
            img_depth: Optional[int] = None,
            **kwargs) -> None:
@@ -102,27 +114,25 @@
 videoconvert ! autovideosink
 
     Args:
       device: The video device to open, if the device opened by default isn't
         the right one. In Linux, should be a path like `/dev/video0`. In
         Windows and Mac, should be the index of the video device. This argument
         is ignored if a ``user_pipeline`` is given.
-      user_pipeline (:obj:`str`, optional): A custom pipeline that can
-        optionally be given. If given, the ``device`` argument is ignored. The
-        pipeline should be given as it would be in a terminal.
-      nb_channels (:obj:`int`, optional): The number of channels expected in
-        the acquired images, in case a custom pipeline is given. Otherwise,
-        this argument is ignored. For now, Crappy only manages 1- and 3-channel
-        images.
-      img_depth (:obj:`int`, optional): The bit depth of each channel of the
-        acquired images, in case a custom pipeline is given. Otherwise, this
-        argument is ignored. For now, Crappy only manages 8- and 16-bits deep
-        images.
+      user_pipeline: A custom pipeline that can optionally be given as a
+        :obj:`str`. If given, the ``device`` argument is ignored. The pipeline
+        should be given as it would be in a terminal.
+      nb_channels: The number of channels expected in the acquired images, in
+        case a custom pipeline is given. Otherwise, this argument is ignored.
+        For now, Crappy only manages 1- and 3-channel images.
+      img_depth: The bit depth of each channel of the acquired images, in case
+        a custom pipeline is given. Otherwise, this argument is ignored. For
+        now, Crappy only manages 8- and 16-bits deep images.
       **kwargs: Allows specifying values for the settings even before
-        displaying the graphical interface.
+        displaying the configuration window.
     """
 
     # Checking the validity of the arguments
     if device is not None and system() == 'Linux' and not isinstance(device,
                                                                      str):
       raise ValueError("In Linux, device should be a string !")
     elif device is not None and system() in ['Darwin', 'Windows'] and not \
@@ -195,40 +205,46 @@
           self.log(logging.WARNING, "The performance of the CameraOpencv "
                                     "class could be improved if v4l-utils "
                                     "was installed !")
           check = None
         check = check.stdout if check is not None else ''
 
         # Trying to find the exposure parameters in the returned string
-        expo = search(r'exposure\s0x[\dA-Fa-f]+\s\(\w+\)\s+:\s'
-                      r'min=(?P<min>\d+)\smax=(?P<max>\d+)', check)
-        expo_auto = search(r'exposure_auto\s0x[\dA-Fa-f]+\s\(\w+\)\s+:\s'
-                           r'min=(?P<min>\d+)\smax=(?P<max>\d+)', check)
-        expo_abso = search(r'exposure_absolute\s0x[\dA-Fa-f]+\s\(\w+\)\s+:\s'
-                           r'min=(?P<min>\d+)\smax=(?P<max>\d+)', check)
+        expo = search(r'(?=.*\sexposure\s.*).+min=(?P<min>\d+)\s'
+                      r'max=(?P<max>\d+).+default=(\d+)',
+                      check)
+        expo_auto = search(r'(?=.*exposure.*)(?=.*auto.*)(?=.*menu.*)\s+'
+                           r'\s(\w+)\s', check)
+        expo_abso = search(r'(?=.*absolute.*)(?=.*exposure.*)(?=.*int.*)\s+'
+                           r'\s(\w+)\s.+min=(\d+)\smax=(\d+).+default=(\d+)',
+                           check)
 
         # If there's an exposure parameter, getting its upper and lower limits
         if expo:
-          expo_min, expo_max = map(int, expo.groups())
+          expo_min, expo_max, default = map(int, expo.groups())
           self._exposure_mode = 'direct'
+          self._exposure_setting = 'exposure'
 
         # If there's an exposure parameter, getting its upper and lower limits
         elif expo_auto and expo_abso:
-          expo_min, expo_max = map(int, expo_abso.groups())
-          self._exposure_mode = 'auto'
+          self._exposure_mode = 'manual'
+          self._exposure_setting = expo_abso.groups()[0]
+          self._exposure_auto = expo_auto.groups()[0]
+          expo_min, expo_max, default = map(int, expo_abso.groups()[1:])
 
         else:
           expo_min = None
           expo_max = None
+          default = None
 
         # Creating the parameter if applicable
         if expo_min is not None:
           self.add_scale_setting(name='exposure', lowest=expo_min,
                                  highest=expo_max, getter=self._get_exposure,
-                                 setter=self._set_exposure)
+                                 setter=self._set_exposure, default=default)
 
       # Then, trying to get the available image encodings and formats
       if system() == 'Linux':
 
         self._formats = []
 
         # Trying to run v4l2-ctl to get the available formats
@@ -251,18 +267,21 @@
           check = []
 
         if check:
           for img_format in check:
             # For each encoding, finding its name
             name, *_ = search(r"'(\w+)'", img_format).groups()
             sizes = findall(r'\d+x\d+', img_format)
+            fps_sections = split(r'\d+x\d+', img_format)[1:]
 
             # For each name, finding the available sizes
-            for size in sizes:
-              self._formats.append(f'{name} {size}')
+            for size, fps_section in zip(sizes, fps_sections):
+              fps_list = findall(r'\((\d+\.\d+)\sfps\)', fps_section)
+              for fps in fps_list:
+                self._formats.append(f'{name} {size} ({fps} fps)')
 
         else:
           # If v4l-utils is not installed, proposing two encodings without
           # further detail
           self._formats = ['Default', 'MJPG']
 
       # For Windows and Mac proposing two encodings without further detail
@@ -289,14 +308,19 @@
       self.add_scale_setting(name='contrast', lowest=0., highest=2.,
                              setter=self._set_contrast, default=1.)
       self.add_scale_setting(name='hue', lowest=-1., highest=1.,
                              setter=self._set_hue, default=0.)
       self.add_scale_setting(name='saturation', lowest=0., highest=2.,
                              setter=self._set_saturation, default=1.)
 
+      # Adding the software ROI selection settings
+      if self._formats and ' ' in self._formats[0]:
+        width, height = search(r'(\d+)x(\d+)', self._get_format()).groups()
+        self.add_software_roi(int(width), int(height))
+
     # Setting up GStreamer and the callback
     self.log(logging.INFO, "Initializing the GST pipeline")
     self.log(logging.DEBUG, f"The pipeline is {self._get_pipeline()}")
     self._pipeline = Gst.parse_launch(self._get_pipeline())
     self._app_sink = self._pipeline.get_by_name('sink')
     self._app_sink.set_property("emit-signals", True)
     self._app_sink.connect("new-sample", self._on_new_sample)
@@ -331,15 +355,15 @@
     while self._last_frame_nr == self._frame_nr:
       if time() - t0 > 2:
         raise TimeoutError("Waited too long for the next image !")
       sleep(0.01)
 
     self._last_frame_nr = self._frame_nr
 
-    return time(), copy(self._img)
+    return time(), self.apply_soft_roi(copy(self._img))
 
   def close(self) -> None:
     """Simply stops the image acquisition."""
 
     if self._pipeline is not None:
       self.log(logging.INFO, "Stopping the GST pipeline")
       self._pipeline.set_state(Gst.State.NULL)
@@ -352,16 +376,16 @@
 
   def _restart_pipeline(self,
                         pipeline: str,
                         exposure: Optional[int] = None) -> None:
     """Stops the current pipeline, redefines it, and restarts it.
 
     Args:
-      pipeline (:obj:`str`): The new pipeline to use.
-      exposure (:obj:`int`, optional): The new exposure value to set.
+      pipeline: The new pipeline to use, as a :obj:`str`.
+      exposure: The new exposure value to set, as an :obj:`int`.
     """
 
     # Stops the previous pipeline
     self.log(logging.INFO, "Stopping the GST pipeline")
     self._pipeline.set_state(Gst.State.NULL)
 
     # Redefines the pipeline and the callbacks
@@ -377,17 +401,17 @@
             self._exposure_mode is not None:
       # Two different ways of setting the exposure
       if self._exposure_mode == 'direct':
         extra_args = (f"controls,"
                       f"""exposure={exposure if exposure is not None 
                                 else self.exposure}""")
       else:
-        extra_args = (f"controls,exposure_auto=1,"
-                      f"""exposure_absolute={exposure if exposure is not None
-                                         else self.exposure}""")
+        extra_args = (f"controls,{self._exposure_auto}=1,"
+                      f"{self._exposure_setting}="
+                      f"{exposure if exposure is not None else self.exposure}")
 
       # Setting the exposure is done via the 'extra-controls' property of the
       # 'v4l2src' source
       self._app_source = self._pipeline.get_by_name('source')
       structure, _ = Gst.Structure.from_string(extra_args)
       self._app_source.set_property('extra-controls', structure)
 
@@ -397,25 +421,27 @@
 
   def _get_pipeline(self,
                     brightness: Optional[float] = None,
                     contrast: Optional[float] = None,
                     hue: Optional[float] = None,
                     saturation: Optional[float] = None,
                     img_format: Optional[int] = None) -> str:
-    """Method that generates a pipeline, according to the settings.
+    """Method that generates a pipeline, according to the given settings.
 
     If a user-defined pipeline was given, it will always be returned.
 
     Args:
-      brightness: The brightness value to set, as a float between -1 and 1.
-      contrast: The contrast value to set, as a float between 0 and 2.
-      hue: The hue value to set, as a float between -1 and 1.
-      saturation: The saturation value to set, as a float between 0 and 2.
-      img_format: The image format to set, as a string containing the name of
-        the encoding and optionally both the width and height in pixels.
+      brightness: The brightness value to set, as a :obj:`float` between -1 and
+        1.
+      contrast: The contrast value to set, as a :obj:`float` between 0 and 2.
+      hue: The hue value to set, as a :obj:`float` between -1 and 1.
+      saturation: The saturation value to set, as a :obj:`float` between 0 and
+        2.
+      img_format: The image format to set, as a :obj:`str` containing the name
+        of the encoding and optionally both the width and height in pixels.
 
     Returns:
       A pipeline matching the current settings values.
     """
 
     # Returns the custom pipeline if any
     if self._user_pipeline is not None:
@@ -439,33 +465,39 @@
     else:
       device = ''
 
     # Getting the format index
     img_format = img_format if img_format is not None else self.format
 
     try:
-      format_name, img_size = img_format.split(' ')
+      format_name, img_size, fps = findall(r"(\w+)\s(\w+)\s\((\d+.\d+) fps\)",
+                                           img_format)[0]
     except ValueError:
-      format_name, img_size = img_format, None
+      format_name, img_size, fps = img_format, None, None
 
     # Adding a mjpeg decoder to the pipeline if needed
     img_format = '! jpegdec' if format_name == 'MJPG' else ''
 
     # Getting the width and height from the second half of the string
     if img_size is not None:
       width, height = map(int, img_size.split('x'))
     else:
       width, height = None, None
 
-    # Including the dimensions in the pipeline
+    # Including the dimensions and the fps in the pipeline
     img_size = f',width={width},height={height}' if width else ''
+    if fps is not None:
+      fps = Fraction(fps)
+      fps_str = f',framerate={fps.numerator}/{fps.denominator}'
+    else:
+      fps_str = ''
 
     # Finally, generate a single pipeline containing all the user settings
     return f"""{source} {device} name=source {img_format} ! videoconvert ! 
-           video/x-raw,format=BGR{img_size} ! 
+           video/x-raw,format=BGR{img_size}{fps_str} ! 
            videobalance 
            brightness={brightness if brightness is not None 
                        else self.brightness:.3f} 
            contrast={contrast if contrast is not None else self.contrast:.3f} 
            hue={hue if hue is not None else self.hue:.3f}
            saturation={saturation if saturation is not None 
                        else self.saturation:.3f} ! 
@@ -552,53 +584,56 @@
     """Returns the current exposure value.
 
     Only works when the platform is Linux.
     """
 
     # Trying to run v4l2-ctl to get the exposure value
     if self._device is not None:
-      command = ['v4l2-ctl', '-d', self._device, '-C',
-                 'exposure_absolute' if self._exposure_mode == 'auto' else
-                 'exposure']
+      command = ['v4l2-ctl', '-d', self._device, '--all']
     else:
-      command = ['v4l2-ctl', '-C',
-                 'exposure_absolute' if self._exposure_mode == 'auto' else
-                 'exposure']
+      command = ['v4l2-ctl', '--all']
     try:
       self.log(logging.DEBUG, f"Getting exposure with command {command}")
       expo = run(command, capture_output=True, text=True)
     except FileNotFoundError:
       expo = None
 
     # Extracting the exposure from the returned string
     expo = expo.stdout if expo is not None else ''
-    expo = search(r'\d+', expo)
+    expo = search(rf'(?=.*\s{self._exposure_setting}\s.*).+value=(\d+)', expo)
     if expo:
-      return int(expo[0])
+      return int(expo.groups()[0])
     else:
       raise IOError("Couldn't read exposure value from v4l2 !")
 
   def _set_format(self, img_format) -> None:
     """Sets the image encoding and dimensions."""
 
     self._restart_pipeline(self._get_pipeline(img_format=img_format))
 
+    # Reloading the software ROI selection settings
+    if self._soft_roi_set and self._formats and ' ' in self._formats[0]:
+      sleep(0.1)
+      width, height = search(r'(\d+)x(\d+)', self._get_format()).groups()
+      self.reload_software_roi(int(width), int(height))
+
   def _get_format(self) -> str:
-    """Parses the v4l2-ctl -V command to get the current image format as an
+    """Parses the ``v4l2-ctl -V`` command to get the current image format as an
     index."""
 
     # Sending the v4l2-ctl command
     if self._device is not None:
-      command = ['v4l2-ctl', '-d', str(self._device), '-V']
+      command = ['v4l2-ctl', '-d', str(self._device), '--all']
     else:
-      command = ['v4l2-ctl', '-V']
-    self.log(logging.DEBUG, f"Getting image format with command {command}")
+      command = ['v4l2-ctl', '--all']
     check = run(command, capture_output=True, text=True).stdout
 
     # Parsing the answer
-    format_ = width = height = ''
-    if search(r"'(\w+)'", check) is not None:
-      format_, *_ = search(r"'(\w+)'", check).groups()
-    if search(r"(\d+)/(\d+)", check):
-      width, height = search(r"(\d+)/(\d+)", check).groups()
+    format_ = width = height = fps = ''
+    if search(r"Pixel Format\s*:\s*'(\w+)'", check) is not None:
+      format_, *_ = search(r"Pixel Format\s*:\s*'(\w+)'", check).groups()
+    if search(r"Width/Height\s*:\s*(\d+)/(\d+)", check) is not None:
+      width, height = search(r"Width/Height\s*:\s*(\d+)/(\d+)", check).groups()
+    if search(r"Frames per second\s*:\s*(\d+.\d+)", check) is not None:
+      fps, *_ = search(r"Frames per second\s*:\s*(\d+.\d+)", check).groups()
 
-    return f'{format_} {width}x{height}'
+    return f'{format_} {width}x{height} ({fps} fps)'
```

### Comparing `crappy-2.0.0.dev1/src/crappy/camera/meta_camera/camera.py` & `crappy-2.0.0.dev2/src/crappy/tool/image_processing/video_extenso/tracker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,270 +1,277 @@
 # coding: utf-8
 
-from typing import Callable, Optional, Tuple, Union, Any, Dict
-from time import sleep
+from multiprocessing import Process, get_start_method
+from multiprocessing.connection import Connection
+from multiprocessing.queues import Queue
 import numpy as np
-from multiprocessing import current_process
+from typing import Optional, Union
+from time import time
+from select import select
 import logging
+import logging.handlers
+from platform import system
 
-from .meta_camera import MetaCamera
-from .camera_setting import CameraSetting, CameraBoolSetting, \
-  CameraScaleSetting, CameraChoiceSetting
+from ...camera_config import Box
+from ...._global import OptionalModule
 
-NbrType = Union[int, float]
+try:
+  import cv2
+except (ModuleNotFoundError, ImportError):
+  cv2 = OptionalModule("opencv-python")
+try:
+  from skimage.filters import threshold_otsu
+except (ModuleNotFoundError, ImportError):
+  threshold_otsu = OptionalModule("skimage", "Please install scikit-image to "
+                                             "use Video-extenso")
+
+
+class LostSpotError(Exception):
+  """Exception raised when a spot is lost, or when there's too much
+  overlapping."""
+
+
+class Tracker(Process):
+  """:obj:`multiprocessing.Process` whose task is to track a spot on an image.
+
+  It receives a subframe centered on the last known position of the spot, and
+  returns the updated position of the detected spot. It is meant to be used in
+  association with the 
+  :class:`~crappy.tool.image_processing.video_extenso.VideoExtensoTool`.
+  """
 
+  names = list()
 
-class Camera(metaclass=MetaCamera):
-  """Base class for every camera object.
+  def __init__(self,
+               pipe: Connection,
+               logger_name: str,
+               log_level: Optional[int],
+               log_queue: Queue,
+               white_spots: bool = False,
+               thresh: Optional[int] = None,
+               blur: Optional[float] = 5) -> None:
+    """Sets the arguments.
 
-  It contains all the methods shared by these classes and sets MetaCam as their
-  metaclass.
-  """
+    Args:
+      pipe: The :obj:`~multiprocessing.connection.Connection` object through
+        which the image is received and the updated coordinates of the spot
+        are sent back.
+      logger_name: The name of the parent :obj:`~logging.Logger` as a 
+        :obj:`str`, used for naming the Logger in this class.
+      log_level: The minimum logging level of the entire Crappy script, as an
+        :obj:`int`.
+      log_queue: A :obj:`multiprocessing.Queue` for sending the log messages to 
+        the main :obj:`~logging.Logger`, only used in Windows.
+      white_spots: If :obj:`True`, detects white objects on a black background,
+        else black objects on a white background.
+      thresh: If given, this threshold value will always be used for isolating
+        the spot from the background. If not given (:obj:`None`), a new
+        threshold is recalculated for each new subframe. Spots are less likely
+        to be lost with an adaptive threshold, but it takes a bit more time.
+      blur: If not :obj:`None`, the subframe is first blurred before trying to
+        detect the spot. This argument gives the size of the kernel to use for
+        blurring. Better results are obtained with blurring, but it takes a bit
+        more time.
+    """
 
-  def __init__(self, *_, **__) -> None:
-    """Simply sets the dict containing the settings and the name of the
-    trigger setting."""
+    super().__init__()
+    self.name = self.get_name(logger_name, type(self).__name__)
+    self._system = system()
+
+    self._pipe = pipe
+    self._white_spots = white_spots
+    self._thresh = thresh
+    self._blur = blur
 
-    self.settings: Dict[str, CameraSetting] = dict()
-    self.trigger_name = 'trigger'
     self._logger: Optional[logging.Logger] = None
+    self._log_level = log_level
+    self._log_queue = log_queue
 
-  def log(self, level: int, msg: str) -> None:
-    """"""
-
-    if self._logger is None:
-      self._logger = logging.getLogger(
-        f"{current_process().name}.{type(self).__name__}")
-
-    self._logger.log(level, msg)
+    self._n = 0
+    self._last_warn = time()
 
-  def open(self, **kwargs) -> None:
-    """This method should initialize the connection to the camera, configure
-    the camera, and start the image acquisition.
-
-    This method also takes as arguments all the kwargs that were passed to the
-    Camera block but not used by it. Some may be used directly, e.g. for
-    choosing which camera to open out of several possible ones, and the others
-    should indicate values to set for available settings. It is fine not to
-    provide any values for the settings here, as each setting has a default.
-
-    To effectively set the setting values, the method :meth:`set_all` has to
-    be called at the end of open (e.g. ``self.set_all(**kwargs)``). This is
-    true even if no value to set was given in the kwargs. If it is not called,
-    the settings won't actually be set on the camera.
-
-    If some camera settings require values from the camera for their
-    instantiation (e.g.
-    ``self.add_setting(..., highest=self.cam.max_width(), ...)``), they should
-    be instantiated here. And of course before calling :meth:`set_all`.
-    """
+  @classmethod
+  def get_name(cls, logger_name: str, self_name: str) -> str:
+    """Method for naming the Tracker processes so that each of them has a
+    unique name.
 
-    self.set_all(**kwargs)
+    Args:
+      logger_name: The name of the parent :obj:`~logging.Logger`, as a 
+        :obj:`str`.
+      self_name: The name of the current class.
 
-  def get_image(self) -> Optional[Union[Tuple[Dict[str, Any], float],
-                                        np.ndarray]]:
-    """Acquires an image and returns it along with its metadata or timestamp.
-
-    It is also fine for this method to return :obj:`None`. The image should be
-    returned as a numpy array, and the metadata as a :obj:`dict` or the
-    timestamp as a :obj:`float`. The keys of the metadata dictionary should
-    preferably be valid Exif tags, so that the metadata can be embedded into
-    the image file when saving.
-
-    In order for the recording of images to run, the metadata dict must
-    contain at least the ``'t(s)'`` and ``''ImageUniqueID''`` keys, whose
-    values should be the timestamp when the frame was acquired (as returned by
-    ``time.time()``) and the frame number as an :obj:`int`.
+    Returns:
+      The chosen name for the current Tracker process, as a :obj:`str`.
     """
 
-    self.log(logging.WARNING, "The get_img method was called but is not "
-                              "defined !\nNo image can be acquired if this "
-                              "method isn't defined")
-    sleep(1)
-    return
-
-  def close(self) -> None:
-    """This method should perform any action required for properly stopping the
-    image acquisition and/or closing the connection to the camera.
-
-    This step is usually extremely important in order for the camera resources
-    to be released. Otherwise, it might be impossible to re-open the camera
-    from Crappy without resetting the hardware connection with it.
+    i = 1
+    while f"{logger_name}.{self_name}-{i}" in cls.names:
+      i += 1
+
+    cls.names.append(f"{logger_name}.{self_name}-{i}")
+    return f"{logger_name}.{self_name}-{i}"
+
+  def run(self) -> None:
+    """Continuously reads incoming subframes, tries to detect a spot and sends
+    back the coordinates of the detected spot.
+
+    Can only be stopped either with a :exc:`KeyboardInterrupt` or when
+    receiving a text message from the 
+    :class:`~crappy.tool.image_processing.video_extenso.VideoExtensoTool`.
     """
 
-    ...
+    # Looping forever for receiving data
+    try:
+      self._set_logger()
 
-  def add_bool_setting(self,
-                       name: str,
-                       getter: Optional[Callable[[], bool]] = None,
-                       setter: Optional[Callable[[bool], None]] = None,
-                       default: bool = True) -> None:
-    """Adds a boolean setting, whose value is either :obj:`True` or
-    :obj:`False`.
+      while True:
+        # Making sure the call to recv is not blocking
+        if self._pipe.poll(0.5):
+          y_start, x_start, img = self._pipe.recv()
+          self._log(logging.DEBUG, "Received data from pipe")
+          self._n += 1
+
+          # If a string is received, always means the process has to stop
+          if isinstance(img, str):
+            break
+
+          # Simply sending back the new Box containing the spot
+          try:
+            self._log(logging.DEBUG, "Sending back data through pipe")
+            self._send(self._evaluate(x_start, y_start, img))
+
+          # If the caught exception is a KeyboardInterrupt, simply stopping
+          except KeyboardInterrupt:
+            self._log(logging.INFO, "Caught KeyboardInterrupt, stopping the "
+                                    "process")
+            break
+          # Sending back the exception if anything else unexpected happened
+          except (Exception,) as exc:
+            self._logger.exception("Caught exception while tracking spot",
+                                   exc_info=exc)
+            self._send('stop')
+            break
+
+    # In case the user presses CTRL+C, simply stopping the process
+    except KeyboardInterrupt:
+      self._log(logging.INFO, "Caught KeyboardInterrupt, stopping the process")
+
+  def _evaluate(self, x_start: int, y_start: int, img: np.ndarray) -> Box:
+    """Takes a sub-image, applies a threshold on it and tries to detect the new
+    position of the spot.
 
     Args:
-      name: The name of the setting, that will be displayed in the GUI and can
-        be used to directly get the value of the setting by calling
-        ``self.<name>``
-      getter: The method for getting the current value of the setting. If not
-        given, the returned value is simply the last one that was set.
-      setter: The method for setting the current value of the setting. If not
-        given, the value to be set is simply stored.
-      default: The default value to assign to the setting.
+      x_start: The x position of the top left pixel of the subframe on the
+        entire image.
+      y_start: The y position of the top left pixel of the subframe on the
+        entire image.
+      img: The subframe on which to search for a spot.
+
+    Returns:
+      A :class:`~crappy.tool.camera_config.config_tools.Box` object containing 
+      the x and y start and end positions of the detected spot, as well as the 
+      coordinates of the centroid.
     """
 
-    # Checking if the given name is valid
-    if name == self.trigger_name:
-      raise ValueError(f"The name {self.trigger_name} is reserved for the "
-                       f"trigger setting !")
-    if name in self.settings:
-      raise ValueError('This setting already exists !')
-    self.log(logging.INFO, f"Adding the {name} bool setting")
-    self.settings[name] = CameraBoolSetting(name, getter, setter, default)
-
-  def add_scale_setting(self,
-                        name: str,
-                        lowest: NbrType,
-                        highest: NbrType,
-                        getter: Optional[Callable[[], NbrType]] = None,
-                        setter: Optional[Callable[[NbrType], None]] = None,
-                        default: Optional[NbrType] = None) -> None:
-    """Adds a scale setting, whose value is an :obj:`int` or a :obj:`float`
-    clamped between two boundaries.
-
-    Note:
-      If any of ``lowest`` or ``highest`` is a :obj:`float`, then the setting
-      is considered to be of type float and can take float values. Otherwise,
-      it is considered of type int and can only take integer values.
+    # First, blurring the image if asked to
+    if self._blur is not None and self._blur > 1:
+      img = cv2.medianBlur(img, self._blur)
+
+    # Determining the best threshold for the image if required
+    thresh = self._thresh if self._thresh is not None else threshold_otsu(img)
+
+    # Getting all pixels superior or inferior to threshold
+    if self._white_spots:
+      black_white = (img > thresh).astype('uint8')
+    else:
+      black_white = (img <= thresh).astype('uint8')
 
-    Args:
-      name: The name of the setting, that will be displayed in the GUI and can
-        be used to directly get the value of the setting by calling
-        ``self.<name>``
-      lowest: The lowest possible value for the setting.
-      highest: The highest possible value for the setting.
-      getter: The method for getting the current value of the setting. If not
-        given, the returned value is simply the last one that was set.
-      setter: The method for setting the current value of the setting. If not
-        given, the value to be set is simply stored.
-      default: The default value to assign to the setting. If not given, will
-        be the average of ``lowest`` and ``highest``.
-    """
+    # Checking that the detected spot is large enough
+    if np.count_nonzero(black_white) < 0.1 * img.size:
 
-    # Checking if the given name is valid
-    if name == self.trigger_name:
-      raise ValueError(f"The name {self.trigger_name} is reserved for the "
-                       f"trigger setting !")
-    if name in self.settings:
-      raise ValueError('This setting already exists !')
-    self.log(logging.INFO, f"Adding the {name} scale setting")
-    self.settings[name] = CameraScaleSetting(name, lowest, highest, getter,
-                                             setter, default)
-
-  def add_choice_setting(self,
-                         name: str,
-                         choices: Tuple[str, ...],
-                         getter: Optional[Callable[[], str]] = None,
-                         setter: Optional[Callable[[str], None]] = None,
-                         default: Optional[str] = None) -> None:
-    """Adds a choice setting, that can take a limited number of predefined
-    :obj:`str` values.
+      # If the threshold is pre-defined, trying again with an updated one
+      if self._thresh is not None:
+        self._log(logging.WARNING,
+                  "Detected spot too small compared with overall box size, "
+                  "recalculating threshold")
+        thresh = threshold_otsu(img)
+        if self._white_spots:
+          black_white = (img > thresh).astype('uint8')
+        else:
+          black_white = (img <= thresh).astype('uint8')
+
+        # If the spot still cannot be detected, aborting
+        if np.count_nonzero(black_white) < 0.1 * img.size:
+          self._log(logging.ERROR,
+                    "Couldn't detect spot with adaptive threshold, aborting !")
+          raise LostSpotError
+
+      # If an adaptive threshold is already used, nothing more can be done
+      else:
+        self._log(logging.ERROR,
+                  "Couldn't detect spot with adaptive threshold, aborting !")
+        raise LostSpotError
 
-    Args:
-      name: The name of the setting, that will be displayed in the GUI and can
-        be used to directly get the value of the setting by calling
-        ``self.<name>``
-      choices: A :obj:`tuple` containing the possible values for the setting.
-      getter: The method for getting the current value of the setting. If not
-        given, the returned value is simply the last one that was set.
-      setter: The method for setting the current value of the setting. If not
-        given, the value to be set is simply stored.
-      default: The default value to assign to the setting. If not given, will
-        be the fist item in ``choices``.
-    """
+    # Calculating the coordinates of the centroid using the image moments
+    moments = cv2.moments(black_white)
+    try:
+      x = moments['m10'] / moments['m00']
+      y = moments['m01'] / moments['m00']
+    except ZeroDivisionError:
+      raise ZeroDivisionError("Couldn't compute the centroid because the "
+                              "moment of order 0, 0 is zero !")
+
+    # Getting the updated centroid and coordinates of the spot
+    x_min, y_min, width, height = cv2.boundingRect(black_white)
+    return Box(x_start=x_start + x_min,
+               y_start=y_start + y_min,
+               x_end=x_start + x_min + width,
+               y_end=y_start + y_min + height,
+               x_centroid=x_start + x,
+               y_centroid=y_start + y)
+
+  def _send(self, val: Union[Box, str]) -> None:
+    """Sends a message to the 
+    :class:`~crappy.tool.image_processing.video_extenso.VideoExtensoTool`, and 
+    in Linux checks that the :obj:`multiprocessing.Pipe` is not full before 
+    sending."""
+
+    if self._system == 'Linux':
+      if select([], [self._pipe], [], 0)[1]:
+        self._pipe.send(val)
+      elif time() - self._last_warn > 1:
+          self._last_warn = time()
+          self._log(logging.WARNING, f"Cannot send the detected spot to the "
+                                     f"VideoExtenso tool, the Pipe is full !")
+    else:
+      self._pipe.send(val)
 
-    # Checking if the given name is valid
-    if name == self.trigger_name:
-      raise ValueError(f"The name {self.trigger_name} is reserved for the "
-                       f"trigger setting !")
-    if name in self.settings:
-      raise ValueError('This setting already exists !')
-    self.log(logging.INFO, f"Adding the {name} choice setting")
-    self.settings[name] = CameraChoiceSetting(name, choices, getter, setter,
-                                              default)
-
-  def add_trigger_setting(self,
-                          getter: Optional[Callable[[], str]] = None,
-                          setter: Optional[Callable[[str], None]] = None
-                          ) -> None:
-    """Adds a specific choice setting for controlling the trigger mode of the
-    camera. The reserved name for this setting is ``'Trigger'``.
-
-    This setting is mainly intended for cameras that can run either in free run
-    mode or in hardware trig mode. The three possible choices for this setting
-    are : ``'Free run'``, ``'Hdw after config'`` and ``'Hardware'``. Default is
-    ``'Free run'``.
-
-    The setter method is expected to set the camera to free run mode in
-    ``'Free run'`` and ``'Hdw after config'`` choices, and to hardware trigger
-    mode in the ``'Hardware'`` choice. The getter method should return either
-    ``'Free run'`` or ``'Hdw after config'`` in free run mode, depending on the
-    last set value for the setting, and ``'Hardware'`` in hardware trig mode.
-    It can also be left to :obj:`None`.
-
-    The rationale behind the ``'Hdw after config'`` choice is to allow the user
-    to tune settings in the configuration window with the camera in free run
-    mode, and to switch afterwards to the hardware trigger mode for the actual
-    test. It proves extremely useful if the hardware triggers are generated
-    from Crappy, as they're not started yet when the configuration window is
-    running.
+  def _set_logger(self) -> None:
+    """Instantiates and sets up the logger for the instance."""
 
-    Args:
-      getter: The method for getting the current value of the setting. If not
-        given, the returned value is simply the last one that was set.
-      setter: The method for setting the current value of the setting. If not
-        given, the value to be set is simply stored.
-    """
+    logger = logging.getLogger(self.name)
+
+    # Disabling logging if requested
+    if self._log_level is not None:
+      logger.setLevel(self._log_level)
+    else:
+      logging.disable()
 
-    if self.trigger_name in self.settings:
-      raise ValueError("There can only be one trigger setting per camera !")
+    # On Windows, the messages need to be sent through a Queue for logging
+    if get_start_method() == "spawn" and self._log_level is not None:
+      queue_handler = logging.handlers.QueueHandler(self._log_queue)
+      queue_handler.setLevel(self._log_level)
+      logger.addHandler(queue_handler)
 
-    self.log(logging.INFO, f"Adding the {self.trigger_name} trigger setting")
-    self.settings[self.trigger_name] = CameraChoiceSetting(
-      name=self.trigger_name, choices=('Free run',
-                                       'Hdw after config',
-                                       'Hardware'),
-      getter=getter, setter=setter, default='Free run')
-
-  def set_all(self, **kwargs) -> None:
-    """Checks if the kwargs are valid, sets them, and for settings that are not
-    in kwargs sets them to their default value."""
-
-    unexpected = tuple(kwarg for kwarg in kwargs if kwarg not in self.settings)
-    if unexpected:
-      raise ValueError(f'Unexpected argument(s) {", ".join(unexpected)} for '
-                       f'camera {type(self).__name__}.')
-
-    self.log(logging.INFO, "Setting all the setting values")
-    for name, setting in self.settings.items():
-      setting.value = kwargs[name] if name in kwargs else setting.default
-
-  def __getattr__(self, item: str) -> Any:
-    """Method for getting the value of a setting directly by calling
-    ``self.<setting name>``.
+    self._logger = logger
 
-    It is called in case __getattribute__ doesn't work properly, and tries to
-    return the corresponding setting value."""
+  def _log(self, level: int, msg: str) -> None:
+    """Sends a log message to the :obj:`~logging.Logger`.
 
-    try:
-      return self.settings[item].value
-    except (AttributeError, KeyError):
-      raise AttributeError(f'No attribute nor setting named {item}')
-
-  def __setattr__(self, key: str, val: Any) -> None:
-    """Method for setting the value of a setting directly by calling
-    ``self.<setting name> = <value>``."""
+    Args:
+      level: The logging level, as an :obj:`int`.
+      msg: The message to log, as a :obj:`str`.
+    """
 
-    if key != 'settings' and key in self.settings:
-      self.settings[key].value = val
-    else:
-      super().__setattr__(key, val)
+    if self._logger is None:
+      return
+    self._logger.log(level, msg)
```

### Comparing `crappy-2.0.0.dev1/src/crappy/camera/meta_camera/camera_setting/camera_scale_setting.py` & `crappy-2.0.0.dev2/src/crappy/camera/meta_camera/camera_setting/camera_scale_setting.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,16 +8,21 @@
 NbrType = Union[int, float]
 
 
 class CameraScaleSetting(CameraSetting):
   """Camera setting that can take any value between a lower and an upper
   boundary.
 
+  It is a child of
+  :class:`~crappy.camera.meta_camera.camera_setting.CameraSetting`.
+
   This class can handle settings that should only take :obj:`int` values as
-  well as settings that can take :obj:`float` value.
+  well as settings that can take :obj:`float` value. The type used is
+  :obj:`int` is both of the given lowest or highest values are :obj:`int`,
+  otherwise :obj:`float` is used.
   """
 
   def __init__(self,
                name: str,
                lowest: NbrType,
                highest: NbrType,
                getter: Optional[Callable[[], NbrType]] = None,
@@ -36,21 +41,29 @@
 
     self.lowest = lowest
     self.highest = highest
     self.type = int if isinstance(lowest + highest, int) else float
 
     if default is None:
       default = self.type((lowest + highest) / 2)
+    else:
+      default = self.type(default)
 
     super().__init__(name, getter, setter, default)
 
   @property
   def value(self) -> NbrType:
     """Returns the current value of the setting, by calling the getter if one
-    was provided or else by returning the stored value."""
+    was provided or else by returning the stored value.
+
+    When the getter is called, calls the setter if one was provided and updates
+    the sored value. After calling the setter, checks that the value was set
+    by calling the getter and displays a warning message if the target and
+    actual values don't match.
+    """
 
     if self._getter is not None:
       return self.type(min(max(self._getter(), self.lowest), self.highest))
     else:
       return self.type(self._value_no_getter)
 
   @value.setter
@@ -59,9 +72,36 @@
     self.log(logging.DEBUG, f"Setting the setting {self.name} to {val}")
 
     self._value_no_getter = self.type(val)
     if self._setter is not None:
       self._setter(self.type(val))
 
     if self.value != val:
+      # Double-checking, got strange behavior sometimes probably because of
+      # delays in lower level APIs
+      if self.value == val:
+        return
       self.log(logging.WARNING, f"Could not set {self.name} to {val}, the "
                                 f"value is {self.value} !")
+
+  def reload(self,
+             lowest: NbrType,
+             highest: NbrType,
+             default: Optional[NbrType] = None) -> None:
+    """Allows modifying the limits of the scale bar once it is already
+    instantiated."""
+
+    self.log(logging.DEBUG, f"Reloading the setting {self.name}")
+
+    # Updating the lowest, highest, and default values
+    self.lowest = lowest
+    self.highest = highest
+    if default is not None:
+      self.default = self.type(default)
+    else:
+      self.default = self.type((lowest + highest) / 2)
+
+    # Updating the slider limits and the setting value
+    if self.tk_obj is not None:
+      self.tk_obj.configure(to=self.highest, from_=self.lowest)
+    if self.tk_var is not None:
+      self.tk_var.set(self.value)
```

### Comparing `crappy-2.0.0.dev1/src/crappy/camera/meta_camera/camera_setting/camera_setting.py` & `crappy-2.0.0.dev2/src/crappy/camera/meta_camera/camera_setting/camera_setting.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,17 +4,24 @@
 from multiprocessing import current_process
 import logging
 
 NbrType = Union[int, float]
 
 
 class CameraSetting:
-  """Base class for each camera setting.
+  """Base class for each Camera setting.
 
   It is meant to be subclassed and should not be used as is.
+
+  The Camera setting classes hold all the information needed to read and set a
+  setting of a :class:`~crappy.camera.Camera` object. Several types of settings
+  are defined, as children of this class :
+  :class:`~crappy.camera.meta_camera.camera_setting.CameraBoolSetting`,
+  :class:`~crappy.camera.meta_camera.camera_setting.CameraChoiceSetting`,
+  and :class:`~crappy.camera.meta_camera.camera_setting.CameraScaleSetting`.
   """
 
   def __init__(self,
                name: str,
                getter: Callable[[], Any],
                setter: Callable[[Any], None],
                default: Any) -> None:
@@ -39,35 +46,61 @@
     # Attributes for internal use only
     self._value_no_getter = default
     self._getter = getter
     self._setter = setter
     self._logger: Optional[logging.Logger] = None
 
   def log(self, level: int, msg: str) -> None:
-    """"""
+    """Records log messages for the CameraSetting.
+
+    Also instantiates the logger when logging the first message.
+
+    Args:
+      level: An :obj:`int` indicating the logging level of the message.
+      msg: The message to log, as a :obj:`str`.
+    """
 
     if self._logger is None:
       self._logger = logging.getLogger(
         f"{current_process().name}.{type(self).__name__}")
 
     self._logger.log(level, msg)
 
   @property
   def value(self) -> Any:
     """Returns the current value of the setting, by calling the getter if one
-    was provided or else by returning the stored value."""
+    was provided or else by returning the stored value.
+
+    When the getter is called, calls the setter if one was provided and updates
+    the sored value. After calling the setter, checks that the value was set
+    by calling the getter and displays a warning message if the target and
+    actual values don't match.
+    """
 
     if self._getter is not None:
       return self._getter()
     else:
       return self._value_no_getter
 
   @value.setter
   def value(self, val: Any) -> None:
     self.log(logging.DEBUG, f"Setting the setting {self.name} to {val}")
     self._value_no_getter = val
     if self._setter is not None:
       self._setter(val)
 
     if self.value != val:
+      # Double-checking, got strange behavior sometimes probably because of
+      # delays in lower level APIs
+      if self.value == val:
+        return
       self.log(logging.WARNING, f"Could not set {self.name} to {val}, the "
                                 f"value is {self.value} !")
+
+  def reload(self, *_, **__) -> None:
+    """Allows modifying a setting once it is already being displayed in the
+    GUI.
+
+    Mostly helpful for adjusting the ranges of sliders.
+    """
+
+    ...
```

### Comparing `crappy-2.0.0.dev1/src/crappy/camera/meta_camera/meta_camera.py` & `crappy-2.0.0.dev2/src/crappy/camera/meta_camera/meta_camera.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/src/crappy/camera/opencv.py` & `crappy-2.0.0.dev2/src/crappy/tool/camera_config/video_extenso_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,226 +1,211 @@
 # coding: utf-8
 
-from time import time
-from typing import Tuple
-from numpy import ndarray
-from platform import system
-from subprocess import run
-from re import findall, split, search
+import tkinter as tk
+from tkinter.messagebox import showerror
+from typing import Optional
+import numpy as np
+from io import BytesIO
+from pkg_resources import resource_string
+from time import sleep
 import logging
+from multiprocessing.queues import Queue
 
-from .meta_camera import Camera
-from .._global import OptionalModule
+from .camera_config_boxes import CameraConfigBoxes
+from .config_tools import Box, SpotsDetector
+from ...camera.meta_camera import Camera
+from ..._global import OptionalModule
 
 try:
-  import cv2
+  from PIL import Image
 except (ModuleNotFoundError, ImportError):
-  cv2 = OptionalModule("opencv-python")
+  Image = OptionalModule("pillow")
 
-# Todo: Manage frame rate
 
-
-class CameraOpencv(Camera):
-  """A class for reading images from any camera able to interface with OpenCv.
-
-  The number of the video device to read images from can be specified. It is
-  then also possible to tune the encoding format and the size.
-
-  This camera class is less performant than the :ref:`Camera GStreamer` one
-  that relies on GStreamer, but the installation of OpenCv is way easier than
-  the one of GStreamer.
-
-  Note:
-    For a better performance of this class in Linux, it is recommended to have
-    `v4l-utils` installed.
+class VideoExtensoConfig(CameraConfigBoxes):
+  """Class similar to :class:`~crappy.tool.camera_config.CameraConfig` but also
+  displaying the bounding boxes of the detected spots, and allowing to select
+  the area where to detect the spots by drawing a box with the left mouse
+  button.
+
+  It relies on the :class:`~crappy.tool.camera_config.config_tools.Box` and
+  :class:`~crappy.tool.camera_config.config_tools.SpotsDetector` tools. It is
+  meant to be used for configuring the :class:`~crappy.blocks.VideoExtenso`
+  Block.
   """
 
-  def __init__(self) -> None:
-    """Sets variables and adds the channels setting."""
-
-    super().__init__()
-
-    self._cap = None
-
-    self.add_choice_setting(name="channels",
-                            choices=('1', '3'),
-                            default='1')
-
-  def open(self, device_num: int = 0, **kwargs) -> None:
-    """Opens the video stream and sets any user-specified settings.
+  def __init__(self,
+               camera: Camera,
+               log_queue: Queue,
+               log_level: Optional[int],
+               detector: SpotsDetector) -> None:
+    """Sets the args and initializes the parent class.
 
     Args:
-      device_num (:obj:`int`, optional): The number of the device to open.
-      **kwargs: Any additional setting to set before opening the graphical
-        interface.
+      camera: The :class:`~crappy.camera.Camera` object in charge of acquiring
+      the images.
+      log_queue: A :obj:`multiprocessing.Queue` for sending the log messages to
+        the main :obj:`~logging.Logger`, only used in Windows.
+      log_level: The minimum logging level of the entire Crappy script, as an
+        :obj:`int`.
+      detector: An instance of
+        :class:`~crappy.tool.camera_config.config_tools.SpotsDetector` used for
+        detecting spots on the images received from the
+        :class:`~crappy.camera.Camera`.
     """
 
-    if not isinstance(device_num, int) or device_num < 0:
-      raise ValueError("device_num should be an integer !")
+    super().__init__(camera, log_queue, log_level)
+    self._detector = detector
+    self._spots = detector.spots
+
+  def finish(self) -> None:
+    """Method called when the user tries to close the configuration window.
+
+    Checks that spots were detected on the image. If not, warns the user and
+    prevents him from exiting except with CTRL+C. Also, saves the initial
+    length if not already done by the user.
+    """
 
-    # Opening the videocapture device
-    self.log(logging.INFO, "Opening the image stream from the camera")
-    self._cap = cv2.VideoCapture(device_num)
-    self._device_num = device_num
-    fourcc = self._get_fourcc()
-
-    if system() == 'Linux':
-      self._formats = []
-
-      # Trying to run v4l2-ctl to get the available formats
-      command = ['v4l2-ctl', '-d', str(device_num), '--list-formats-ext']
-      try:
-        self.log(logging.INFO, f"Getting the available image formats with "
-                               f"command {command}")
-        check = run(command, capture_output=True, text=True)
-      except FileNotFoundError:
-        self.log(logging.WARNING, "The performance of the CameraOpencv class "
-                                  "could be improved if v4l-utils was "
-                                  "installed !")
-        check = None
-      check = check.stdout if check is not None else ''
-
-      # Splitting the returned string to isolate each encoding
-      if findall(r'\[\d+]', check):
-        check = split(r'\[\d+]', check)[1:]
-      elif findall(r'Pixel\sFormat', check):
-        check = split(r'Pixel\sFormat', check)[1:]
-      else:
-        check = []
+    if self._detector.spots.empty():
+      self.log(logging.WARNING, "No spots were selected ! Not exiting the "
+                                "configuration window")
+      showerror("Error !",
+                message="Please select spots before exiting the config "
+                        "window !\nOr hit CTRL+C to exit Crappy")
+      return
+
+    if self._detector.spots.x_l0 is None or self._detector.spots.y_l0 is None:
+      self._detector.spots.save_length()
+      self.log(logging.INFO,
+               f"Successfully saved L0 ! L0 x : {self._detector.spots.x_l0}, "
+               f"L0 y : {self._detector.spots.y_l0}")
+
+    super().stop()
+
+  def _set_bindings(self) -> None:
+    """Binds the left mouse button click for drawing the box in which the spots
+    will be searched."""
+
+    super()._set_bindings()
+
+    self._img_canvas.bind('<ButtonPress-1>', self._start_box)
+    self._img_canvas.bind('<B1-Motion>', self._extend_box)
+    self._img_canvas.bind('<ButtonRelease-1>', self._stop_box)
+
+  def _create_buttons(self) -> None:
+    """Compared with the parent class, creates an extra button for saving the
+    original position of the spots."""
+
+    self._update_button = tk.Button(self._sets_frame, text="Apply Settings",
+                                    command=self._update_settings)
+    self._update_button.pack(expand=False, fill='none', ipadx=5, ipady=5,
+                             padx=5, pady=5, anchor='n', side='top')
+
+    self._update_button = tk.Button(self._sets_frame, text="Save L0",
+                                    command=self._save_l0)
+    self._update_button.pack(expand=False, fill='none', ipadx=5, ipady=5,
+                             padx=5, pady=5, anchor='n', side='top')
+
+  def _stop_box(self, _: tk.Event) -> None:
+    """When the user releases the mouse, searches for spots in the selected
+    area and displays them if any were found."""
+
+    # If it's just a regular click with no dragging, do nothing
+    if self._img is None or self._select_box.no_points():
+      self._select_box.reset()
+      return
+
+    # The sides need to be sorted before slicing numpy array
+    y_left, y_right, x_top, x_bottom = self._select_box.sorted()
+
+    # If the box is flat, resetting it
+    if y_left == y_right or x_top == x_bottom:
+      self._select_box.reset()
+      return
+
+    # Now actually trying to detect the spots
+    try:
+      self._detector.detect_spots(self._original_img[x_top: x_bottom,
+                                                     y_left: y_right],
+                                  x_top, y_left)
+    except IndexError:
+      # Highly unlikely but always better to be careful
+      self._detector.spots.reset()
+      return
 
-      if check:
-        for img_format in check:
-          # For each encoding, finding its name
-          name, *_ = search(r"'(\w+)'", img_format).groups()
-          sizes = findall(r'\d+x\d+', img_format)
-
-          # For each name, finding the available sizes
-          for size in sizes:
-            self._formats.append(f'{name} {size}')
+    # This box is not needed anymore
+    self._select_box.reset()
 
-      else:
-        # If v4l-utils is not installed, proposing two encodings without
-        # further detail
-        self._formats = [fourcc, 'MJPG']
-
-        # Still letting the user choose the size
-        self.add_scale_setting(name='width', lowest=1, highest=1920,
-                               getter=self._get_width, setter=self._set_width)
-        self.add_scale_setting(name='height', lowest=1, highest=1080,
-                               getter=self._get_height,
-                               setter=self._set_height)
+  def _save_l0(self) -> None:
+    """Saves the original positions of the spots on the image."""
 
+    if self._detector.spots.empty():
+      self.log(logging.WARNING, "Cannot save L0, there are no spots !")
     else:
-      # On Windows the fourcc management is even messier than on Linux
-      self._formats = []
-
-      # Still letting the user choose the size
-      self.add_scale_setting(name='width', lowest=1, highest=1920,
-                             getter=self._get_width, setter=self._set_width)
-      self.add_scale_setting(name='height', lowest=1, highest=1080,
-                             getter=self._get_height, setter=self._set_height)
-
-    if self._formats:
-      # The format integrates the size selection
-      if ' ' in self._formats[0]:
-        self.add_choice_setting(name='format',
-                                choices=tuple(self._formats),
-                                getter=self._get_format_size,
-                                setter=self._set_format)
-      # The size is independent of the format
+      self._detector.spots.save_length()
+      self.log(logging.INFO,
+               f"Successfully saved L0 ! L0 x : {self._detector.spots.x_l0}, "
+               f"L0 y : {self._detector.spots.y_l0}")
+
+  def _on_img_resize(self, _: Optional[tk.Event] = None) -> None:
+    """Same as in the parent class except it also draws the patches and the
+    select box on top of the displayed image."""
+
+    self.log(logging.DEBUG, "The image canvas was resized")
+
+    self._draw_box(self._select_box)
+    self._draw_spots()
+    self._resize_img()
+    self._display_img()
+    self.update()
+
+  def _update_img(self) -> None:
+    """Same as in the parent class except it also draws the patches and the
+    select box on top of the displayed image."""
+
+    self.log(logging.DEBUG, "Updating the image")
+
+    ret = self._camera.get_image()
+
+    # If no frame could be grabbed from the camera
+    if ret is None:
+      # If it's the first call, generate error image to initialize the window
+      if not self._n_loops:
+        self.log(logging.WARNING, "Could not get an image from the camera, "
+                                  "displaying an error image instead")
+        ret = None, np.array(Image.open(BytesIO(resource_string(
+          'crappy', 'tool/data/no_image.png'))))
+      # Otherwise, just pass
       else:
-        self.add_choice_setting(name='format',
-                                choices=tuple(self._formats),
-                                getter=self._get_fourcc,
-                                setter=self._set_format)
-
-    # Setting the kwargs if any
-    self.set_all(**kwargs)
-
-  def get_image(self) -> Tuple[float, ndarray]:
-    """Grabs a frame from the videocapture object and returns it along with a
-    timestamp."""
-
-    # Grabbing the frame and the timestamp
-    t = time()
-    ret, frame = self._cap.read()
-
-    # Checking the integrity of the frame
-    if not ret:
-      raise IOError("Error reading the camera")
-
-    # Returning the image in the right format, and its timestamp
-    if self.channels == '1':
-      return t, cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
-    else:
-      return t, frame
-
-  def close(self) -> None:
-    """Releases the videocapture object."""
-
-    if self._cap is not None:
-      self.log(logging.INFO, "Closing the image stream from the camera")
-      self._cap.release()
+        self.log(logging.DEBUG, "No image returned by the camera")
+        self.update()
+        sleep(0.001)
+        return
 
-  def _get_fourcc(self) -> str:
-    """Returns the current fourcc string of the video encoding."""
+    self._n_loops += 1
+    _, img = ret
 
-    fcc = int(self._cap.get(cv2.CAP_PROP_FOURCC))
-    return f"{fcc & 0xFF:c}{(fcc >> 8) & 0xFF:c}" \
-           f"{(fcc >> 16) & 0xFF:c}{(fcc >> 24) & 0xFF:c}"
+    if img.dtype != self.dtype:
+      self.dtype = img.dtype
+    if self.shape != img.shape:
+      self.shape = img.shape
 
-  def _get_width(self) -> int:
-    """Returns the current image width."""
+    self._cast_img(img)
+    self._draw_box(self._select_box)
+    self._draw_spots()
+    self._resize_img()
 
-    return self._cap.get(cv2.CAP_PROP_FRAME_WIDTH)
+    self._calc_hist()
+    self._resize_hist()
 
-  def _get_height(self) -> int:
-    """Returns the current image height."""
+    self._display_img()
+    self._display_hist()
 
-    return self._cap.get(cv2.CAP_PROP_FRAME_HEIGHT)
+    self._update_pixel_value()
 
-  def _set_width(self, width: int) -> None:
-    """Tries to set the image width."""
+    self.update()
 
-    self._cap.set(cv2.CAP_PROP_FRAME_WIDTH, width)
-
-  def _set_height(self, height: int) -> None:
-    """Tries to set the image height."""
-
-    self._cap.set(cv2.CAP_PROP_FRAME_HEIGHT, height)
-
-  def _set_format(self, img_format: str) -> None:
-    """Sets the format of the image according to the user's choice."""
-
-    # The format might be made of a name and a dimension, or just a name
-    try:
-      format_name, img_size = img_format.split(' ')
-    except ValueError:
-      format_name, img_size = img_format, None
-
-    # Setting the format
-    self._cap.set(cv2.CAP_PROP_FOURCC, cv2.VideoWriter_fourcc(*format_name))
-
-    if img_size is not None:
-      # Getting the width and height from the second half of the string
-      width, height = map(int, img_size.split('x'))
-
-      # Setting the size
-      self._set_width(width),
-      self._set_height(height)
-
-  def _get_format_size(self) -> str:
-    """Parses the v4l2-ctl -V command to get the current image format as an
-    index."""
-
-    # Sending the v4l2-ctl command
-    command = ['v4l2-ctl', '-d', str(self._device_num), '-V']
-    check = run(command, capture_output=True, text=True).stdout
-
-    # Parsing the answer
-    format_ = width = height = ''
-    if search(r"'(\w+)'", check) is not None:
-      format_, *_ = search(r"'(\w+)'", check).groups()
-    if search(r"(\d+)/(\d+)", check):
-      width, height = search(r"(\d+)/(\d+)", check).groups()
+  def _handle_box_outside_img(self, _: Box) -> None:
+    """If a patch is outside the image, it means that the image size has been
+    modified. Simply resetting the spots then."""
 
-    return f'{format_} {width}x{height}'
+    self._spots.reset()
```

### Comparing `crappy-2.0.0.dev1/src/crappy/camera/pi_camera.py` & `crappy-2.0.0.dev2/src/crappy/camera/raspberry_pi_camera.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # coding: utf-8
 
 from time import time, sleep
 from typing import Tuple, Any, Optional
 import numpy as np
 from threading import Thread, RLock
 import logging
+
 from .meta_camera import Camera
 from .._global import OptionalModule
 
 try:
   import cv2
 except (ModuleNotFoundError, ImportError):
   cv2 = OptionalModule("opencv-python")
@@ -17,21 +18,26 @@
   from picamera import PiCamera as PiCameraRPi
   from picamera.array import PiRGBArray
 except (ModuleNotFoundError, ImportError, OSError):
   PiCameraRPi = OptionalModule("picamera")
 
 picamera_iso = [0, 100, 200, 320, 400, 500, 640, 800]
 
+# TODO:
+#   Update to picamera2 when available
+
+
+class RaspberryPiCamera(Camera):
+  """Class for reading images from a Raspberry Pi Camera.
 
-class PiCamera(Camera):
-  """Class for reading images from a PiCamera.
+  The RaspberryPiCamera Camera block is meant for reading images from a
+  Raspberry Pi Camera. It uses the :mod:`picamera` module for capturing images,
+  and :mod:`cv2` for converting BGR images to black and white.
 
-  The PiCamera Camera block is meant for reading images from a PiCamera.
-  It uses the :mod:`picamera` module for capturing images, and :mod:`cv2` for
-  converting bgr images to black and white.
+  It can read images from the PiCamera V1, V2 and HQ models indifferently.
 
   Warning:
     Only works on Raspberry Pi, with the picamera API. On the latest OS release
     "Bullseye", it has to be specifically activated in the configuration menu.
   """
 
   def __init__(self) -> None:
@@ -73,17 +79,19 @@
                            self._set_crop_height, 1.0)
 
     self._frame_grabber = Thread(target=self._grab_frame)
     self._lock = RLock()
     self._frame = None
     self._stop = False
     self._started = False
+    self._stream = None
 
   def open(self, **kwargs: Any) -> None:
-    """Sets the settings to their default values and starts the thread."""
+    """Sets the settings to their default values and starts the image
+    acquisition thread."""
 
     self.set_all(**kwargs)
 
     # Starting the video stream
     self._capture = PiRGBArray(self._cam, (self._get_width(),
                                            self._get_height()))
     self.log(logging.INFO, "Starting the frame stream")
@@ -91,28 +99,65 @@
                                                 use_video_port=True)
 
     self.log(logging.INFO, "Starting the frame grabber thread")
     self._frame_grabber.start()
     sleep(1)
     self._started = True
 
+  def get_image(self) -> Tuple[float, np.ndarray]:
+    """Simply returns the last image in the acquisition buffer.
+
+    The captured image is in GBR format, and converted into black and white if
+    needed.
+
+    Returns:
+      The timeframe and the image.
+    """
+
+    t = time()
+    with self._lock:
+      output = self._frame
+    if self.Black_and_white:
+      output = cv2.cvtColor(output, cv2.COLOR_BGR2GRAY)
+    return t, output
+
+  def close(self) -> None:
+    """Joins the image acquisition thread, and closes the stream and the
+    :class:`picamera.PiCamera` object."""
+
+    self._stop = True
+    if self._frame_grabber is not None:
+      self.log(logging.INFO, "Stopping the frame grabber thread")
+      self._frame_grabber.join(0.2)
+      if self._frame_grabber.is_alive():
+        self.log(logging.WARNING, "The frame grabber thread didn't stop "
+                                  "properly !")
+
+    if self._capture is not None:
+      self.log(logging.INFO, "Stopping the frame stream")
+      self._capture.close()
+
+    if self._cam is not None:
+      self.log(logging.INFO, "Opening the connection to the camera")
+      self._cam.close()
+
   def _stop_stream(self) -> None:
-    """Stops the video stream before changing the image size."""
+    """Stops the video stream. Called before changing the image size."""
 
     if not self._started:
       return
 
     self._stop = True
     self.log(logging.INFO, "Stopping the frame grabber thread")
     self._frame_grabber.join()
     self.log(logging.INFO, "Stopping the frame stream")
     self._capture.close()
 
   def _restart_stream(self) -> None:
-    """Restarts the video stream after a change in the image size."""
+    """Restarts the video stream. Called after a change in the image size."""
 
     if not self._started:
       return
 
     self._stop = False
     self._frame_grabber = Thread(target=self._grab_frame)
     self._capture = PiRGBArray(self._cam, (self._get_width(),
@@ -121,63 +166,26 @@
     self._stream = self._cam.capture_continuous(self._capture, format='bgr',
                                                 use_video_port=True)
 
     self.log(logging.INFO, "Starting the frame grabber thread")
     self._frame_grabber.start()
     sleep(1)
 
-  def get_image(self) -> Tuple[float, np.ndarray]:
-    """Simply returns the last image in the buffer.
-
-    The captured image is in bgr format, and converted into black and white if
-    needed.
-
-    Returns:
-      The timeframe and the image.
-    """
-
-    t = time()
-    with self._lock:
-      output = self._frame
-    if self.Black_and_white:
-      output = cv2.cvtColor(output, cv2.COLOR_BGR2GRAY)
-    return t, output
-
   def _grab_frame(self) -> None:
-    """Thread for grabbing the last image in the video stream and putting it in
-    the buffer."""
+    """Target of a thread for grabbing the last image in the video stream and
+    putting it in a buffer."""
 
     for frame in self._stream:
       with self._lock:
         self.log(logging.DEBUG, "Got new frame from stream")
         self._frame = frame.array
       self._capture.truncate(0)
       if self._stop:
         break
 
-  def close(self) -> None:
-    """Joins the thread and closes the stream and the
-    :class:`picamera.PiCamera` object."""
-
-    self._stop = True
-    if self._frame_grabber is not None:
-      self.log(logging.INFO, "Stopping the frame grabber thread")
-      self._frame_grabber.join(0.2)
-      if self._frame_grabber.is_alive():
-        self.log(logging.WARNING, "The frame grabber thread didn't stop "
-                                  "properly !")
-
-    if self._capture is not None:
-      self.log(logging.INFO, "Stopping the frame stream")
-      self._capture.close()
-
-    if self._cam is not None:
-      self.log(logging.INFO, "Opening the connection to the camera")
-      self._cam.close()
-
   def _get_width(self) -> int:
     return self._cam.resolution[0]
 
   def _get_height(self) -> int:
     return self._cam.resolution[1]
 
   def _get_iso(self) -> int:
@@ -207,27 +215,27 @@
   def _get_crop_width(self) -> float:
     return self._cam.zoom[2]
 
   def _get_crop_height(self) -> float:
     return self._cam.zoom[3]
 
   def _set_width(self, width: float) -> None:
-    # The PiCamera only accepts width that are multiples of 32
+    # The Raspberry Pi Camera only accepts width that are multiples of 32
     self._stop_stream()
     self._cam.resolution = (32 * (width // 32), self._get_height())
     self._restart_stream()
 
   def _set_height(self, height: float) -> None:
-    # The PiCamera only accepts heights that are multiples of 32
+    # The Raspberry Pi Camera only accepts heights that are multiples of 32
     self._stop_stream()
     self._cam.resolution = (self._get_width(), 32 * (height // 32))
     self._restart_stream()
 
   def _set_iso(self, iso: float) -> None:
-    # The PiCamera only accepts a limited range of iso values
+    # The Raspberry Pi Camera only accepts a limited range of iso values
     self._cam.iso = min(picamera_iso, key=lambda x: abs(x - iso))
 
   def _set_brightness(self, brightness: float) -> None:
     self._cam.brightness = brightness
 
   def _set_contrast(self, contrast: float) -> None:
     self._cam.contrast = contrast
```

### Comparing `crappy-2.0.0.dev1/src/crappy/camera/seek_thermal_pro.py` & `crappy-2.0.0.dev2/src/crappy/camera/seek_thermal_pro.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # coding: utf-8
 
 from typing import Tuple, List, Any
 import numpy as np
 from time import time
 import logging
+
 from .meta_camera import Camera
 from .._global import OptionalModule
 
 try:
   import usb.util
   import usb.core
 
@@ -41,19 +42,19 @@
 Seek_thermal_pro_dimensions = {'Width': 320,
                                'Height': 240,
                                'Raw width': 342,
                                'Raw height': 260}
 
 
 class SeekThermalPro(Camera):
-  """Class for reading the Seek Thermal Pro infrared camera.
+  """Class for reading images from the Seek Thermal Pro infrared camera.
 
-  The SeekThermalPro Camera block is meant for reading images from a Seek
+  The SeekThermalPro Camera is meant for reading images from a Seek
   Thermal Pro infrared camera. It communicates over USB, and gets images by
-  converting the received bytearrays into numpy arrays.
+  converting the received bytearrays into :mod:`numpy` arrays.
 
   Important:
     **Only for Linux users:** In order to drive the Seek Thermal Pro, the
     appropriate udev rule should be set. This can be done using the
     `udev_rule_setter` utility in ``crappy``'s `util` folder. It is also
     possible to add it manually by running:
     ::
@@ -67,14 +68,15 @@
   def __init__(self) -> None:
     """Selects the right USB device."""
 
     super().__init__()
 
     self._dev = None
     self._calib = None
+    self._dead_pixels = []
 
     # Listing all the matching USB devices
     devices = usb.core.find(find_all=True,
                             idVendor=Seek_thermal_pro_vendor,
                             idProduct=Seek_thermal_pro_product)
     devices = list(devices)
 
@@ -84,15 +86,15 @@
                     "differentiate between them")
     elif len(devices) == 0:
       raise IOError("No matching camera found")
     else:
       self._dev = devices[0]
 
   def open(self) -> None:
-    """Sets the USB communication and device."""
+    """Sets the USB communication and initializes the device."""
 
     # Setting the USB configuration on the camera
     try:
       self.log(logging.INFO, f"Setting configuration on USB device "
                              f"{self._dev}")
       self._dev.set_configuration()
     except usb.core.USBError:
@@ -132,15 +134,14 @@
     for i in range(5):
       status, ret = self._grab()
       if status == 4:
         self._dead_pixels = self._get_dead_pixels_list(ret)
         break
       elif i == 4:
         self.log(logging.WARNING, "Could not get the dead pixels frame")
-        self._dead_pixels = []
 
     # Acquiring the calibration image and calibrating the camera
     self.log(logging.INFO, "Calibrating the camera")
     for i in range(10):
       status, img = self._grab()
       if status == 1:
         self._calib = self._crop(img) - 1600
@@ -148,15 +149,15 @@
       elif i == 9:
         raise TimeoutError("Could not set the camera")
 
   def get_image(self) -> Tuple[float, np.ndarray]:
     """Reads a single image from the camera.
 
     Returns:
-      The dict containing the metadata, and the captured image
+      The captured image as well as a timestamp.
     """
 
     count = 0
     # Looping until a valid frame is acquired
     while True:
 
       # Capturing one frame
@@ -187,15 +188,15 @@
       self.log(logging.INFO, "Releasing the USB resources")
       usb.util.dispose_resources(self._dev)
 
   def _grab(self) -> [bytes, np.ndarray]:
     """Captures a raw image from the camera.
 
     Returns:
-      The status information and the raw image
+      The status information and the raw image.
     """
 
     # Sending the read command
     self._write_data(Seek_thermal_pro_commands['Start get image transfer'],
                      b'\x58\x5b\x01\x00')
 
     to_read = 2 * \
@@ -220,18 +221,18 @@
     else:
       return status, None
 
   def _get_dead_pixels_list(self, data: np.ndarray) -> List[Tuple[Any]]:
     """Identifies the dead pixels on an image.
 
     Args:
-      data: The image
+      data: The image to identify dead pixels on.
 
     Returns:
-      The list of dead pixels
+      A :obj:`list` containing the indexes of the dead pixels.
     """
 
     img = self._crop(np.frombuffer(data, dtype=np.uint16).reshape(
       Seek_thermal_pro_dimensions['Raw height'],
       Seek_thermal_pro_dimensions['Raw width']))
     return list(zip(*np.where(img < 100)))
 
@@ -244,26 +245,26 @@
 
   def _correct_dead_pixels(self, img: np.ndarray) -> np.ndarray:
     """Corrects the dead pixels values.
 
     The new value is the average value of the surrounding pixels.
 
     Args:
-      img: The image to correct
+      img: The image to correct.
 
     Returns:
-      The corrected image
+      The corrected image.
     """
 
     for i, j in self._dead_pixels:
       img[i, j] = np.median(img[max(0, i - 1): i + 2, max(0, j - 1): j + 2])
     return img
 
   def _write_data(self, request: int, data: bytes) -> int:
-    """Wrapper for writing over USB."""
+    """Wrapper for sending USB messages."""
 
     self.log(logging.DEBUG, f"Sending USB command with request type "
                             f"{Seek_therm_usb_req['Write']}, request "
                             f"{request}, value {0}, index {0},length or "
                             f"data {data}")
 
     try:
@@ -273,15 +274,15 @@
                                      wIndex=0,
                                      data_or_wLength=data,
                                      timeout=None)
     except usb.core.USBError:
       raise IOError("An error occurred during USB communication")
 
   def _read_data(self, request: int, data: bytes) -> int:
-    """Wrapper for reading over USB."""
+    """Wrapper for reading USB messages."""
 
     self.log(logging.DEBUG, f"Sending USB command with request type "
                             f"{Seek_therm_usb_req['Read']}, request {request},"
                             f" value {0}, index {0},length or data {data}")
 
     try:
       return self._dev.ctrl_transfer(bmRequestType=Seek_therm_usb_req['Read'],
```

### Comparing `crappy-2.0.0.dev1/src/crappy/camera/webcam.py` & `crappy-2.0.0.dev2/src/crappy/camera/opencv_camera_basic.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,18 @@
   cv2 = OptionalModule("opencv-python")
 
 
 class Webcam(Camera):
   """A basic class for reading images from a USB camera (including webcams).
 
   It relies on the OpenCv library. Note that it was purposely kept extremely
-  simple as it is mainly used as a demo. See :ref:`Camera OpenCV` and
-  :ref:`Camera GStreamer` for classes giving a finer control over the device.
+  simple as it is mainly used as a demo. See
+  :class:`~crappy.camera.CameraOpencv` and
+  :class:`~crappy.camera.CameraGstreamer` for classes giving a finer control
+  over the camera.
   """
 
   def __init__(self) -> None:
     """Sets variables and adds the channels setting."""
 
     super().__init__()
 
@@ -32,17 +34,17 @@
                             choices=('1', '3'),
                             default='1')
 
   def open(self, device_num: Optional[int] = 0, **kwargs) -> None:
     """Opens the video stream and sets any user-specified settings.
 
     Args:
-      device_num (:obj:`int`, optional): The number of the device to open.
-      **kwargs: Any additional setting to set before opening the graphical
-        interface.
+      device_num: The index of the device to open, as an :obj:`int`.
+      **kwargs: Any additional setting to set before opening the configuration
+        window.
     """
 
     # Opening the videocapture device
     self.log(logging.INFO, "Opening the image stream from the camera")
     self._cap = cv2.VideoCapture(device_num)
 
     # Setting the kwargs if any
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/__init__.py` & `crappy-2.0.0.dev2/src/crappy/inout/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 # coding: utf-8
 
 from typing import Dict, Type
 
-from .meta_inout import InOut, MetaIO
-
-from .ft232h import ADS1115FT232H
-from .ft232h import GPIOSwitchFT232H
-from .ft232h import MCP9600FT232H
-from .ft232h import MPRLSFT232H
-from .ft232h import NAU7802FT232H
-from .ft232h import WaveshareADDAFT232H
-
 from .ads1115 import ADS1115
 from .agilent_34420A import Agilent34420a
 from .comedi import Comedi
+from .daqmx import DAQmx
 from .fake_inout import FakeInout
 from .gpio_pwm import GPIOPWM
 from .gpio_switch import GPIOSwitch
-from .gsm import GSM
-from .kollmorgen import Koll
+from .kollmorgen_akd_pdmm import KollmorgenAKDPDMM
 from .labjack_t7 import LabjackT7
+from .labjack_t7_streamer import T7Streamer
 from .labjack_ue9 import LabjackUE9
 from .mcp9600 import MCP9600
 from .mprls import MPRLS
 from .nau7802 import NAU7802
 from .ni_daqmx import NIDAQmx
-from .opsens import OpSens
+from .opsens_handysens import HandySens
 from .pijuice_hat import PiJuice
-from .spectrum import Spectrum
-from .labjack_t7_streamer import T7Streamer
+from .sim868 import Sim868
+from .spectrum_m2i4711 import SpectrumM2I4711
 from .waveshare_ad_da import WaveshareADDA
 from .waveshare_high_precision import WaveshareHighPrecision
 
-# Win specific
-from .daqmx import DAQmx
+from .ft232h import ADS1115FT232H
+from .ft232h import GPIOSwitchFT232H
+from .ft232h import MCP9600FT232H
+from .ft232h import MPRLSFT232H
+from .ft232h import NAU7802FT232H
+from .ft232h import WaveshareADDAFT232H
+
+from .meta_inout import InOut, MetaIO
 
 # All the inout objects
 inout_dict: Dict[str, Type[InOut]] = MetaIO.classes
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/ads1115.py` & `crappy-2.0.0.dev2/src/crappy/inout/ads1115.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 from time import time
 from re import findall
-from typing import Union, List, Optional
+from typing import List, Optional
 import logging
 
 from .meta_inout import InOut
 from .._global import OptionalModule
 
 try:
   from smbus2 import SMBus
@@ -77,94 +77,84 @@
 
 Ads1115_backends = ['Pi4', 'blinka']
 
 
 class ADS1115(InOut):
   """A class for controlling Adafruit's ADS1115 16-bits ADC.
 
-  The ADS1115 InOut block is meant for reading output values from a 16-bits
+  The ADS1115 InOut is meant for reading conversion values from a 16-bits
   ADS1115 ADC, using the I2C protocol. The output is in Volts by default, but a
   ``gain`` and an ``offset`` can be specified.
+
+  Various settings can be adjusted, like the sample rate, the input mode or the
+  voltage range.
   """
 
   def __init__(self,
                backend: str,
                device_address: int = 0x48,
                i2c_port: int = 1,
                sample_rate: int = 128,
                v_range: float = 2.048,
                multiplexer: str = 'A1',
-               dry_pin: Optional[Union[str, int]] = None,
+               dry_pin: Optional[int] = None,
                gain: float = 1,
                offset: float = 0) -> None:
-    """Checks arguments validity.
+    """Checks the validity of the arguments.
 
     Args:
-      backend (:obj:`str`): The backend for communicating with the ADS1115.
-        Should be one of:
+      backend: The backend for communicating with the ADS1115. Should be one
+        of:
         ::
 
-          'Pi4', 'ft232h', 'blinka'
+          'Pi4', 'blinka'
 
         The `'Pi4'` backend is optimized but only works on boards supporting
         the :mod:`smbus2` module, like the Raspberry Pis. The `'blinka'`
-        backend may be less performant and requires installing Adafruit's
-        modules, but these modules are compatible with and maintained on a wide
-        variety of boards. The `'ft232h'` backend allows controlling the
-        ADS1115 from a PC using Adafruit's FT232H USB to I2C adapter. See
-        :ref:`Crappy for embedded hardware` for details.
-      device_address (:obj:`int`, optional): The I2C address of the ADS1115.
-        The default address is `0x48`, but it is possible to change this
-        setting using the `ADDR` pin.
-      i2c_port (:obj:`int`, optional): The I2C port over which the ADS1115
-        should communicate. On most Raspberry Pi models the default I2C port is
-        `1`.
-      sample_rate (:obj:`int`, optional): The sample rate for data conversion
-        (in SPS). Available sample rates are:
+        backend may be less performant and requires installing
+        :mod:`Adafruit-Blinka` and :mod:`adafruit-circuitpython-ads1x15`, but
+        these modules are compatible with and maintained on a wide variety of
+        boards.
+      device_address: The I2C address of the ADS1115. The default address is
+        `0x48`, but it is possible to change this setting using the `ADDR` pin.
+      i2c_port: The I2C port over which the ADS1115 should communicate. On most
+        Raspberry Pi models the default I2C port is `1`.
+      sample_rate: The sample rate for data conversion (in SPS). The available
+        sample rates are:
         ::
 
           8, 16, 32, 64, 128, 250, 475, 860
 
-      v_range (:obj:`float`, optional): The value (in Volts) of the measured
-        signal corresponding to the `0x7FFF` output in bits, i.e. that
-        saturates the sensor. A signal of ``-v_range`` Volts gives a `0x8000`
-        output in bits. Available ``v_range`` values are:
+      v_range: The value (in Volts) of the measured signal corresponding to the
+        `0x7FFF` output in bits, i.e. that saturates the sensor. A signal of
+        ``-v_range`` Volts gives a `0x8000` output in bits. Available
+        ``v_range`` values are:
         ::
 
           0.256, 0.512, 1.024, 2.048, 4.096, 6.144
 
-      multiplexer (:obj:`str`, optional): Choice of the inputs to consider.
-        Single-input modes actually measure `Ax - GND`. The available
-        ``multiplexer`` values are:
+      multiplexer: Choice of the inputs to consider. Single-input modes
+        actually measure `Ax - GND`. The available ``multiplexer`` values are:
         ::
 
           'A0', 'A1', 'A2', 'A3',
           'A0 - A1',
           'A0 - A3',
           'A1 - A3',
           'A2 - A3'
 
-      dry_pin (:obj:`int` or :obj:`str`, optional): Optionally, reads the end
-        of conversion signal from a GPIO rather than from an I2C message.
-        Speeds up the reading and decreases the traffic on the bus, but
-        requires one extra wire. With the backend `'Pi4'`, give the index of
-        the GPIO in BCM convention. With the `'ft232h'` backend, give the name
-        of the GPIO in the format `Dx` or `Cx`. This feature is not available
-        with the `'blinka'` backend.
-      gain (:obj:`float`, optional): Allows to tune the output value according
-        to the formula:
-        ::
-
-          output = gain * tension + offset.
-
-      offset (:obj:`float`, optional): Allows to tune the output value
-        according to the formula:
-        ::
-
-          output = gain * tension + offset.
+      dry_pin: Optionally, reads the end of conversion signal from a GPIO
+        rather than from an I2C message. Speeds up the reading and decreases
+        the traffic on the I2C bus, but requires one extra wire. With the
+        backend `'Pi4'`, give the index of the GPIO in BCM convention. This
+        feature is not available with the `'blinka'` backend.
+      gain: Allows to tune the output value according to the formula :
+        :math:`output = gain * tension + offset`.
+      offset: Allows to tune the output value according to the formula :
+        :math:`output = gain * tension + offset`.
 
     Warning:
       AINx voltages should not be higher than `VDD+0.3V` nor lower than
       `GND-0.3V`. Setting high ``v_range`` values does not allow measuring
       voltages higher than `VDD` !!
     """
 
@@ -211,20 +201,21 @@
         raise TypeError('int_pin should be an int when using the Pi4 '
                         'backend !')
       elif backend == 'blinka' and dry_pin is not None:
         self.log(logging.WARNING, "Getting the end of conversion information "
                                   "from the DRY pin is not supported by the "
                                   "blinka backend")
     self._dry_pin = dry_pin
+    self._chan = None
 
     self._gain = gain
     self._offset = offset
 
   def open(self) -> None:
-    """Sets the I2C communication and device."""
+    """Initializes the I2C communication and the device."""
 
     if self._backend == 'blinka':
       self._ads.gain = Ads1115_blinka_gain[self._v_range]
       self._ads.data_rate = self._sample_rate
       chan_nr = findall(r'\d', self._multiplexer)
       self.log(logging.INFO, "Opening the ADS1115 with backend blinka")
       if len(chan_nr) == 1:
@@ -262,15 +253,15 @@
 
   def get_data(self) -> List[float]:
     """Reads the registers containing the conversion result.
 
     The output is in Volts, unless a gain and offset are applied.
 
     Returns:
-      :obj:`list`: A list containing the timeframe and the voltage value
+      A :obj:`list` containing the timestamp and the voltage value.
     """
 
     if self._backend == 'blinka':
       out = [time()]
       value = self._chan.voltage
 
     else:
@@ -304,15 +295,15 @@
         value_raw -= 2 ** 16
       value = value_raw * self._v_range / 2 ** 15
 
     out.append(self._offset + self._gain * value)
     return out
 
   def close(self) -> None:
-    """Closes the I2C bus"""
+    """Closes the I2C bus."""
 
     if self._backend == 'Pi4' and self._bus is not None:
       self.log(logging.INFO, "Closing the ADS1115")
       self._bus.close()
 
     if self._backend == 'Pi4' and self._dry_pin is not None:
       self.log(logging.INFO, "CCleaning up the GPIOs")
@@ -327,15 +318,15 @@
     self._bus.write_i2c_block_data(self._device_address, register_address,
                                    [(value >> 8) & 0xFF, value & 0xFF])
 
   def _is_connected(self) -> bool:
     """Tries reading a byte from the device.
 
     Returns:
-      :obj:`bool`: :obj:`True` if reading was successful, else :obj:`False`
+      :obj:`True` if reading was successful, else :obj:`False`.
     """
 
     try:
       self._bus.read_byte(self._device_address)
       return True
     except IOError:
       return False
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/agilent_34420A.py` & `crappy-2.0.0.dev2/src/crappy/inout/opsens_handysens.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,82 +9,59 @@
 
 try:
   import serial
 except (ModuleNotFoundError, ImportError):
   serial = OptionalModule("pyserial")
 
 
-class Agilent34420a(InOut):
-  """Sensor class for Agilent34420A devices.
+class HandySens(InOut):
+  """This class allows reading data from an OpSens HandySens fiber optics
+  signal conditioner.
 
-  This class contains method to measure values of resistance or voltage on
-  Agilent34420A devices.
-
-  Note:
-    May work for other devices too, but not tested.
-
-    If you have issues with this class returning a lot of `'bad serial'`, make
-    sure you have the last version of :mod:`serial`.
+  It can read data from various fiber optics sensors like temperature,
+  pressure, position or strain.
   """
 
   def __init__(self,
-               mode: bytes = b"VOLT",
-               device: str = '/dev/ttyUSB0',
-               baudrate: int = 9600,
-               timeout: float = 1) -> None:
-    """Sets the args and initializes parent class.
+               device: str = '/dev/ttyUSB0') -> None:
+    """Sets the argument and initializes the parent class.
 
     Args:
-      mode: Desired value to measure. Should be either `b'VOLT'` or `b'RES'`.
-      device: Path to the device to open, as a :obj:`str`.
-      baudrate: Desired baudrate for serial communication.
-      timeout: Timeout for the serial connection, as a :obj:`float`.
+      device: Address of the serial connection for communicating with the
+        OpSens.
     """
 
-    self._ser = None
+    self._dev = None
 
     super().__init__()
 
-    self._device = device
-    self._baudrate = baudrate
-    self._timeout = timeout
-    self._mode = mode
+    self._addr = device
 
   def open(self) -> None:
-    """Opens the serial connection, resets the Agilent and configures it to the
-    desired mode."""
+    """Opens the serial connection and configures the OpSens."""
 
-    self.log(logging.INFO, f"Opening the serial port {self._device} with "
-                           f"baudrate {self._baudrate}")
-    self._ser = serial.Serial(port=self._device, baudrate=self._baudrate,
-                              timeout=self._timeout)
-    self.log(logging.DEBUG, f"Writing b'*RST;*CLS;*OPC?\\n' to port "
-                            f"{self._device}")
-    self._ser.write(b"*RST;*CLS;*OPC?\n")
-    self.log(logging.DEBUG, f"Writing b'SENS:FUNC \"{self._mode}\";  \\n' "
-                            f"to port {self._device}")
-    self._ser.write(b"SENS:FUNC \"" + self._mode + b"\";  \n")
-    self.log(logging.DEBUG, f"Writing b'SENS:{self._mode}:NPLC 2  \\n' "
-                            f"to port {self._device}")
-    self._ser.write(b"SENS:" + self._mode + b":NPLC 2  \n")
-    self.log(logging.DEBUG, f"Writing b'SYST:REM\\n' to port {self._device}")
-    self._ser.write(b"SYST:REM\n")
+    self.log(logging.INFO, f"Opening the serial connection on port "
+                           f"{self._addr} with baudrate 57600")
+    self._dev = serial.Serial(port=self._addr, baudrate=57600, timeout=0.1)
+    self._send_cmd("meas:rate min")
 
   def get_data(self) -> List[float]:
-    """Asks the Agilent to acquire a reading and returns it, except if an error
-    occurs in which case `0` is returned."""
+    """Reads data from the OpSens and returns it."""
 
-    self.log(logging.DEBUG, f"Writing b'READ?  \\n' to port {self._device}")
-    self._ser.write(b"READ?  \n")
-    t = time()
-    try:
-      return [t, float(self._ser.readline())]
-    except (serial.SerialException, ValueError):
-      self._ser.flush()
-      return [t, 0]
+    return [time(), float(self._send_cmd("ch1:data? 1")[:-3])]
 
   def close(self) -> None:
-    """Closes the serial port."""
+    """Closes the serial connection, if it was opened."""
 
-    if self._ser is not None:
-      self.log(logging.INFO, f"Closing the serial port {self._device}")
-      self._ser.close()
+    if self._dev is not None:
+      self.log(logging.INFO, f"Closing the serial connection on port "
+                             f"{self._addr}")
+      self._dev.close()
+
+  def _send_cmd(self, cmd: str) -> str:
+    """Wrapper for sending a command and returning the received answer."""
+
+    self.log(logging.DEBUG, f"Writing b'{cmd}\\n' to port {self._addr}")
+    self._dev.write(cmd + '\n')
+    ret = self._dev.read_until(b'\x04\n').decode()
+    self.log(logging.DEBUG, f"Read {ret} on port {self._addr}")
+    return ret
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/comedi.py` & `crappy-2.0.0.dev2/src/crappy/inout/comedi.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 from time import time
-from typing import Optional, List
+from typing import Optional, List, Iterable
 from dataclasses import dataclass
 import logging
 
 from .meta_inout import InOut
 from ..tool.bindings import comedi_bind as comedi
 
 
@@ -26,111 +26,115 @@
 class Comedi(InOut):
   """This class can control acquisition boards relying on the Comedi driver.
 
   It can read data from ADCs on input channels, and set voltages of DACs on
   output channels. Each channel can be tuned independently in terms of range,
   gan, offset, and for input channels it's possible to decide whether they
   should be offset to `0` at the beginning of the test.
+
+  Communicates over serial. This class was implemented and tested on a USB-DUX
+  sigma device. IT should work with other devices as well, but that was not
+  tested.
+
+  Note:
+    This class requires the `libcomedi` library to be installed on the
+    computer.
   """
 
   def __init__(self,
                device: str = '/dev/comedi0',
                sub_device: int = 0,
-               channels: Optional[List[int]] = None,
-               range_num: Optional[List[int]] = None,
-               gain: Optional[List[float]] = None,
-               offset: Optional[List[float]] = None,
-               make_zero: Optional[List[bool]] = None,
+               channels: Optional[Iterable[int]] = None,
+               range_num: Optional[Iterable[int]] = None,
+               gain: Optional[Iterable[float]] = None,
+               offset: Optional[Iterable[float]] = None,
+               make_zero: Optional[Iterable[bool]] = None,
                out_sub_device: int = 1,
-               out_channels: Optional[List[int]] = None,
-               out_range_num: Optional[List[int]] = None,
-               out_gain: Optional[List[float]] = None,
-               out_offset: Optional[List[float]] = None) -> None:
-    """Sets the args and initializes the parent class.
+               out_channels: Optional[Iterable[int]] = None,
+               out_range_num: Optional[Iterable[int]] = None,
+               out_gain: Optional[Iterable[float]] = None,
+               out_offset: Optional[Iterable[float]] = None) -> None:
+    """Sets the arguments and initializes the parent class.
 
     Args:
       device: The address of the device, as a :obj:`str`.
       sub_device: The id of the subdevice to use for input channels, as an
         :obj:`int`.
-      channels: A :obj:`list` containing the indexes of the channels to use as
-        inputs, given as :obj:`int`.
-      range_num: A :obj:`list` containing for each input channel the index of
-        the range to set for that channel, as an :obj:`int`. Refer to the
-        documentation of the board to get the correspondence between range
-        indexes and Volts. If not given, all input channels will be set to the
-        range `0`.
-      gain: A :obj:`list` containing for each input channel the gain to apply
-        to the measured voltage, as a :obj:`float`. The returned voltage is
-        calculated as follows :
-        ::
-
-          returned_voltage = gain * measured_voltage + offset
-
-        If not given, no gain is applied to the measured values.
-      offset: A :obj:`list` containing for each input channel the offset to
-        apply to the measured voltage, as a :obj:`float`. The returned voltage
-        is calculated as follows :
-        ::
-
-          returned_voltage = gain * measured_voltage + offset
-
-        If not given, no offset is applied to the measured values.
-      make_zero: A :obj:`list` containing for each input channel a :obj:`bool`
-        indicating whether the channel should be zeroed or not. If so, data
-        will be acquired on this channel before the test starts, and a
-        compensation value will be deduced so that the offset of this channel
-        is `0`. **It will only take effect if the ``make_zero_delay`` argument
-        of the :ref:`IOBlock` controlling the Comedi is set** ! If not given,
-        the channels are by default not zeroed.
+      channels: An iterable (like a :obj:`list` or a :obj:`tuple`) containing
+        the indexes of the channels to use as inputs, given as :obj:`int`.
+      range_num: An iterable (like a :obj:`list` or a :obj:`tuple`) containing
+        for each input channel the index of the range to set for that channel,
+        as an :obj:`int`. Refer to the documentation of the board to get the
+        correspondence between range indexes and Volts. If not given, all input
+        channels will be set to the range `0`.
+      gain: An iterable (like a :obj:`list` or a :obj:`tuple`) containing for
+        each input channel the gain to apply to the measured voltage, as a
+        :obj:`float`. The returned voltage is calculated as follows :
+        :math:`returned\_voltage = gain * measured\_voltage + offset`. If not
+        given, no gain is applied to the measured values.
+      offset: An iterable (like a :obj:`list` or a :obj:`tuple`) containing for
+        each input channel the offset to apply to the measured voltage, as a
+        :obj:`float`. The returned voltage is calculated as follows :
+        :math:`returned\_voltage = gain * measured\_voltage + offset`. If not
+        given, no offset is applied to the measured values.
+      make_zero: An iterable (like a :obj:`list` or a :obj:`tuple`) containing
+        for each input channel a :obj:`bool` indicating whether the channel
+        should be zeroed or not. If so, data will be acquired on this channel
+        before the test starts, and a compensation value will be deduced so
+        that the offset of this channel is `0`. **It will only take effect if
+        the** ``make_zero_delay`` **argument of the**
+        :class:`~crappy.blocks.IOBlock` **controlling the Comedi is set** ! If
+        not given, the channels are by default not zeroed.
       out_sub_device: The id of the subdevice to use for output channels, as an
         :obj:`int`.
-      out_channels: A :obj:`list` containing the indexes of the channels to use
-        as outputs, given as :obj:`int`.
-      out_range_num: A :obj:`list` containing for each output channel the index
-        of the range to set for that channel, as an :obj:`int`. Refer to the
-        documentation of the board to get the correspondence between range
-        indexes and Volts. If not given, all output channels will be set to the
-        range `0`.
-      out_gain: A :obj:`list` containing for each output channel the gain to
-        apply to the command voltage, as a :obj:`float`. The set voltage is
-        calculated as follows :
-        ::
+      out_channels: An iterable (like a :obj:`list` or a :obj:`tuple`)
+        containing the indexes of the channels to use as outputs, given as
+        :obj:`int`.
+      out_range_num: An iterable (like a :obj:`list` or a :obj:`tuple`)
+        containing for each output channel the index of the range to set for
+        that channel, as an :obj:`int`. Refer to the documentation of the board
+        to get the correspondence between range indexes and Volts. If not
+        given, all output channels will be set to the range `0`.
+      out_gain: An iterable (like a :obj:`list` or a :obj:`tuple`) containing
+        for each output channel the gain to apply to the command voltage, as a
+        :obj:`float`. The set voltage is calculated as follows :
+        .. math::
 
           set_voltage = out_gain * command_voltage + out_offset
 
         If not given, no gain is applied to the command values.
-      out_offset: A :obj:`list` containing for each output channel the offset
-        to apply to the command voltage, as a :obj:`float`. The set voltage is
-        calculated as follows :
-        ::
+      out_offset: An iterable (like a :obj:`list` or a :obj:`tuple`) containing
+        for each output channel the offset to apply to the command voltage, as
+        a :obj:`float`. The set voltage is calculated as follows :
+        .. math::
 
           set_voltage = out_gain * command_voltage + out_offset
 
         If not given, no offset is applied to the command values.
 
     Note:
-      All the :obj:`list` given as arguments for the input channels should have
+      All the iterables given as arguments for the input channels should have
       the same length, and same for the output channels. If that's not the
-      case, all the given lists are treated as if they had the same length
-      as the shortest given list.
+      case, all the given iterables are treated as if they had the same length
+      as the shortest given one.
     """
 
     self._device = None
 
     super().__init__()
 
     self._device_name = device.encode()
     self._sub_device = sub_device
     self._out_sub_device = out_sub_device
 
     # Setting the defaults for arguments that are not given
     if channels is None:
       channels = list()
     if out_channels is None:
-      channels = list()
+      out_channels = list()
 
     if range_num is None:
       range_num = [0 for _ in channels]
     if gain is None:
       gain = [1 for _ in channels]
     if offset is None:
       offset = [0 for _ in channels]
@@ -182,16 +186,16 @@
                                                 self._out_sub_device,
                                                 chan.num)
       chan.range_ds = comedi.comedi_get_range(self._device,
                                               self._out_sub_device,
                                               chan.num, chan.range_num)
 
   def make_zero(self, delay: float) -> None:
-    """Overriding of the method of the parent class, because the user can
-    choose which channels should be zeroed or not.
+    """Overriding the method of the parent class, because the user can choose
+    which channels should be zeroed or not.
 
     It simply performs the regular zeroing, and resets the compensation to
     zero for the channels that shouldn't be zeroed.
     """
 
     # No need to acquire data if no channel should be zeroed
     if any(chan.make_zero for chan in self._channels):
@@ -224,16 +228,16 @@
 
       # Sending the command
       self.log(logging.DEBUG, f"Writing value {out_a} to channel {chan.num}")
       comedi.comedi_data_write(self._device, self._out_sub_device, chan.num,
                                chan.range_num, comedi.AREF_GROUND, out_a)
 
   def get_data(self) -> List[float]:
-    """Simply reads and returns the value of each channel, adjusted with the
-    given gain and offset."""
+    """Reads and returns the value of each channel, adjusted with the given
+    gain and offset."""
 
     data = [time()]
 
     for chan in self._channels:
 
       # Reading the numeric values
       data_read = comedi.comedi_data_read(self._device, self._sub_device,
@@ -245,13 +249,13 @@
       val = comedi.comedi_to_phys(data_read, chan.range_ds, chan.max_data)
 
       # Adjusting with the provided gain and offset
       data.append(val * chan.gain + chan.offset)
     return data
 
   def close(self) -> None:
-    """Simply closes the Comedi board and warns the user in case of failure."""
+    """Closes the Comedi board and warns the user in case of failure."""
 
     if self._device is not None:
       self.log(logging.INFO, "Closing the connection to the Comedi device")
       if comedi.comedi_close(self._device):
         self.log(logging.WARNING, "Closing device failed !")
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/daqmx.py` & `crappy-2.0.0.dev2/src/crappy/inout/daqmx.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 import numpy as np
 from time import time
-from typing import List, Optional
+from typing import List, Optional, Iterable
 from dataclasses import dataclass
 import logging
 
 from .meta_inout import InOut
 from .._global import OptionalModule
 try:
   import PyDAQmx
@@ -23,116 +23,116 @@
   range_num: float = 5
   gain: float = 1
   offset: float = 0
   make_zero: bool = False
 
 
 class DAQmx(InOut):
-  """"""
+  """This class can drive data acquisition hardware from National Instruments.
+
+  It is similar to :class:`~crappy.inout.NIDAQmx` InOut, except it relies on
+  the :mod:`PyDAQmx` module. It was written and tested on a USB 6008 DAQ board,
+  but should work with other instruments as well.
+
+  Note:
+    This class requires the NIDAQmx C driver to be installed, as well as the
+    :mod:`PyDAQmx` module.
+  """
 
   def __init__(self,
                device: str = 'Dev1',
-               channels: Optional[List[str]] = None,
-               gain: Optional[List[float]] = None,
-               offset: Optional[List[float]] = None,
-               ranges: Optional[List[float]] = None,
-               make_zero: Optional[List[bool]] = True,
+               channels: Optional[Iterable[str]] = None,
+               gain: Optional[Iterable[float]] = None,
+               offset: Optional[Iterable[float]] = None,
+               ranges: Optional[Iterable[float]] = None,
+               make_zero: Optional[Iterable[bool]] = True,
                sample_rate: float = 10000,
-               out_channels: Optional[List[str]] = None,
-               out_gain: Optional[List[float]] = None,
-               out_offset: Optional[List[float]] = None,
-               out_ranges: Optional[List[float]] = None) -> None:
-    """Sets the args and initializes the parent class.
+               out_channels: Optional[Iterable[str]] = None,
+               out_gain: Optional[Iterable[float]] = None,
+               out_offset: Optional[Iterable[float]] = None,
+               out_ranges: Optional[Iterable[float]] = None) -> None:
+    """Sets the arguments and initializes the parent class.
 
     Args:
       device: The name of the device to open, as a :obj:`str`.
-      channels: A :obj:`list` containing the names of the channels to use as
-        inputs, given as :obj:`str`. Typical names for inputs are ``'aiX'```,
-        with `X` an integer.
-      gain: A :obj:`list` containing for each input channel the gain to apply
-        to the measured voltage, as a :obj:`float`. The returned voltage is
-        calculated as follows :
-        ::
-
-          returned_voltage = gain * measured_voltage + offset
-
-        If not given, no gain is applied to the measured values.
-      offset: A :obj:`list` containing for each input channel the offset to
-        apply to the measured voltage, as a :obj:`float`. The returned voltage
-        is calculated as follows :
-        ::
-
-          returned_voltage = gain * measured_voltage + offset
-
-        If not given, no offset is applied to the measured values.
-      ranges: A :obj:`list` containing for each input channel the range to set
-        for that channel, as an :obj:`float`. The possible range values are :
+      channels: An iterable (like a :obj:`list` or a :obj:`tuple`) containing
+        the names of the channels to use as inputs, given as :obj:`str`.
+        Typical names for inputs are ``'aiX'```, with `X` an integer.
+      gain: An iterable (like a :obj:`list` or a :obj:`tuple`) containing for
+        each input channel the gain to apply to the measured voltage, as a
+        :obj:`float`. The returned voltage is calculated as follows
+        :math:`returned\_voltage = gain * measured\_voltage + offset`. If not
+        given, no gain is applied to the measured values.
+      offset: An iterable (like a :obj:`list` or a :obj:`tuple`) containing for
+        each input channel the offset to apply to the measured voltage, as a
+        :obj:`float`. The returned voltage is calculated as follows
+        :math:`returned\_voltage = gain * measured\_voltage + offset`. If not
+        given, no offset is applied to the measured values.
+      ranges: An iterable (like a :obj:`list` or a :obj:`tuple`) containing for
+        each input channel the range to set for that channel, as a
+        :obj:`float`. The possible range values are :
         ::
 
           0.5, 1., 2.5, 5.
 
         If not given, all input channels will be set to the range `5`.
-      make_zero: A :obj:`list` containing for each input channel a :obj:`bool`
-        indicating whether the channel should be zeroed or not. If so, data
-        will be acquired on this channel before the test starts, and a
-        compensation value will be deduced so that the offset of this channel
-        is `0`. **It will only take effect if the ``make_zero_delay`` argument
-        of the :ref:`IOBlock` controlling the Comedi is set** ! If not given,
-        the channels are by default not zeroed.
+      make_zero: An iterable (like a :obj:`list` or a :obj:`tuple`) containing
+        for each input channel a :obj:`bool` indicating whether the channel
+        should be zeroed or not. If so, data will be acquired on this channel
+        before the test starts, and a compensation value will be deduced so
+        that the offset of this channel is `0`. **It will only take effect if
+        the** ``make_zero_delay`` **argument of the**
+        :class:`~crappy.blocks.IOBlock` **controlling the DAQ is set** ! If not
+        given, the channels are by default not zeroed.
       sample_rate: The frequency of the acquisition, as a :obj:`float`. The
         higher this number, the more noise there is on the signal but the
         higher the acquisition frequency.
-      out_channels: A :obj:`list` containing the names of the channels to use
-        as outputs, given as :obj:`str`. Typical names for outputs are
-        ``'aoX'``, with `X` an integer.
-      out_gain: A :obj:`list` containing for each output channel the gain to
-        apply to the command voltage, as a :obj:`float`. The set voltage is
-        calculated as follows :
-        ::
-
-          set_voltage = out_gain * command_voltage + out_offset
-
-        If not given, no gain is applied to the command values.
-      out_offset: A :obj:`list` containing for each output channel the offset
-        to apply to the command voltage, as a :obj:`float`. The set voltage is
-        calculated as follows :
-        ::
-
-          set_voltage = out_gain * command_voltage + out_offset
-
-        If not given, no offset is applied to the command values.
-      out_ranges: A :obj:`list` containing for each output channel the range to
-        set for that channel, as an :obj:`float`. The possible range values
-        are :
+      out_channels: An iterable (like a :obj:`list` or a :obj:`tuple`)
+        containing the names of the channels to use as outputs, given as
+        :obj:`str`. Typical names for outputs are ``'aoX'``, with `X` an
+        integer.
+      out_gain: An iterable (like a :obj:`list` or a :obj:`tuple`) containing
+        for each output channel the gain to apply to the command voltage, as a
+        :obj:`float`. The set voltage is calculated as follows :
+        :math:`set\_voltage = out\_gain * command\_voltage + out\_offset`. If
+        not given, no gain is applied to the command values.
+      out_offset: An iterable (like a :obj:`list` or a :obj:`tuple`) containing
+        for each output channel the offset to apply to the command voltage, as
+        a :obj:`float`. The set voltage is calculated as follows :
+        :math:`set\_voltage = out\_gain * command\_voltage + out\_offset`. If
+        not given, no offset is applied to the command values.
+      out_ranges: An iterable (like a :obj:`list` or a :obj:`tuple`) containing
+        for each output channel the range to set for that channel, as a
+        :obj:`float`. The possible range values are :
         ::
 
           0.5, 1., 2.5, 5.
 
         If not given, all output channels will be set to the range `5`.
 
     Note:
-      All the :obj:`list` given as arguments for the input channels should have
+      All the iterables given as arguments for the input channels should have
       the same length, and same for the output channels. If that's not the
-      case, all the given lists are treated as if they had the same length
-      as the shortest given list.
+      case, all the given iterables are treated as if they had the same length
+      as the shortest given one.
     """
 
     self._handle = None
     self._out_handle = None
 
     super().__init__()
 
     self._device = device
     self._sample_rate = sample_rate
 
     # Setting the defaults for arguments that are not given
     if channels is None:
       channels = list()
     if out_channels is None:
-      channels = list()
+      out_channels = list()
 
     if ranges is None:
       ranges = [5 for _ in channels]
     if gain is None:
       gain = [1 for _ in channels]
     if offset is None:
       offset = [0 for _ in channels]
@@ -197,16 +197,16 @@
         PyDAQmx.DAQmxCreateAOVoltageChan(self._out_handle, 
                                          f"{self._device}/{chan.name}", '', 0, 
                                          chan.range_num, 
                                          PyDAQmx.DAQmx_Val_Volts, None)
         PyDAQmx.DAQmxStartTask(self._out_handle)
   
   def make_zero(self, delay: float) -> None:
-    """Overriding of the method of the parent class, because the user can
-    choose which channels should be zeroed or not.
+    """Overriding the method of the parent class, because the user can choose
+    which channels should be zeroed or not.
 
     It simply performs the regular zeroing, and resets the compensation to
     zero for the channels that shouldn't be zeroed.
     """
 
     # No need to acquire data if no channel should be zeroed
     if any(chan.make_zero for chan in self._channels):
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/fake_inout.py` & `crappy-2.0.0.dev2/src/crappy/inout/fake_inout.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 # coding: utf-8
 
 from time import time
-from typing import List
+from typing import List, Optional
 
 from .meta_inout import InOut
 from .._global import OptionalModule
 
 try:
   from psutil import virtual_memory
 except (ModuleNotFoundError, ImportError):
   virtual_memory = OptionalModule("psutil")
 
 
 class FakeInout(InOut):
-  """A class demonstrating the usage of an inout abject without requiring any
-  hardware.
+  """This class is a demonstration InOut object that does not require any
+  hardware to run.
 
-  It can read and/or modify the current memory usage on the computer.
+  It can read and/or modify (to a certain extent) the memory usage of the
+  computer.
   """
 
   def __init__(self) -> None:
-    """Not much to do here."""
+    """Initializes the parent class."""
 
-    self._buf = None
+    self._buf: Optional[list] = None
 
     super().__init__()
 
   def open(self) -> None:
     """Creates the buffer allowing to modify the memory usage."""
 
     self._buf = list()
 
   def set_cmd(self, *cmd: float) -> None:
-    """Modifies the computer memory usage.
+    """Modifies the memory usage of the computer.
 
-    If the command is lower than the current, empties the buffer.
     If the command is higher than the current, adds big lists to the buffer in
     order to use more memory.
+    If the command is lower than the current, empties the buffer.
 
     Args:
-      *cmd (:obj:`float`): The target memory usage to set.
+      *cmd: The target memory usage to set, in percent as a :obj:`float`.
     """
 
     if not isinstance(cmd[0], float) and not isinstance(cmd[0], int):
       raise TypeError("Not the right command type for the FakeInout !")
     if not 0 <= cmd[0] <= 100:
       raise ValueError("Command should be a percentage of memory usage !")
 
@@ -53,15 +54,15 @@
       try:
         # If there's nothing to delete, abort
         del self._buf[-1]
       except IndexError:
         return
 
   def get_data(self) -> List[float]:
-    """Just returns time and the current memory usage."""
+    """Just returns the timestamp and the current memory usage."""
 
     return [time(), virtual_memory().percent]
 
   def close(self) -> None:
     """Deletes the buffer."""
 
     del self._buf
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/ft232h/ads1115_ft232h.py` & `crappy-2.0.0.dev2/src/crappy/inout/ft232h/ads1115.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 from time import time
-from typing import Union, List, Optional
+from typing import List, Optional
 import logging
 
 from ..meta_inout import InOut
 from ...tool.ft232h import FT232HServer as FT232H, USBArgsType
 
 # Register and other configuration values:
 Ads1115_pointer_conversion = 0x00
@@ -36,81 +36,79 @@
                      128: 0x0080,
                      250: 0x00A0,
                      475: 0x00C0,
                      860: 0x00E0}
 
 
 class ADS1115FT232H(InOut):
-  """A class for controlling Adafruit's ADS1115 16-bits ADC.
+  """A class for controlling Adafruit's ADS1115 16-bits ADC through an FT232H.
 
-  The ADS1115 InOut block is meant for reading output values from a 16-bits
+  It is similar to the :class:`~crappy.inout.ADS1115` class, except this class
+  is specific for use with an :class:`~crappy.tool.ft232h.FT232H` USB to I2C
+  converter.
+
+  The ADS1115 InOut is meant for reading conversion values from a 16-bits
   ADS1115 ADC, using the I2C protocol. The output is in Volts by default, but a
   ``gain`` and an ``offset`` can be specified.
+
+  Various settings can be adjusted, like the sample rate, the input mode or the
+  voltage range.
   """
 
   ft232h = True
 
   def __init__(self,
                device_address: int = 0x48,
                sample_rate: int = 128,
                v_range: float = 2.048,
                multiplexer: str = 'A1',
-               dry_pin: Optional[Union[str, int]] = None,
+               dry_pin: Optional[str] = None,
                gain: float = 1,
                offset: float = 0,
                _ft232h_args: USBArgsType = tuple()) -> None:
-    """Checks arguments validity.
+    """Checks the validity of the arguments.
 
     Args:
-      device_address (:obj:`int`, optional): The I2C address of the ADS1115.
-        The default address is `0x48`, but it is possible to change this
-        setting using the `ADDR` pin.
-      sample_rate (:obj:`int`, optional): The sample rate for data conversion
-        (in SPS). Available sample rates are:
+      device_address: The I2C address of the ADS1115. The default address is
+        `0x48`, but it is possible to change this setting using the `ADDR` pin.
+      sample_rate: The sample rate for data conversion (in SPS). The available
+        sample rates are:
         ::
 
           8, 16, 32, 64, 128, 250, 475, 860
 
-      v_range (:obj:`float`, optional): The value (in Volts) of the measured
-        signal corresponding to the `0x7FFF` output in bits, i.e. that
-        saturates the sensor. A signal of ``-v_range`` Volts gives a `0x8000`
-        output in bits. Available ``v_range`` values are:
+      v_range: The value (in Volts) of the measured signal corresponding to the
+        `0x7FFF` output in bits, i.e. that saturates the sensor. A signal of
+        ``-v_range`` Volts gives a `0x8000` output in bits. Available
+        ``v_range`` values are:
         ::
 
           0.256, 0.512, 1.024, 2.048, 4.096, 6.144
 
-      multiplexer (:obj:`str`, optional): Choice of the inputs to consider.
-        Single-input modes actually measure `Ax - GND`. The available
-        ``multiplexer`` values are:
+      multiplexer: Choice of the inputs to consider. Single-input modes
+        actually measure `Ax - GND`. The available ``multiplexer`` values are:
         ::
 
           'A0', 'A1', 'A2', 'A3',
           'A0 - A1',
           'A0 - A3',
           'A1 - A3',
           'A2 - A3'
 
-      dry_pin (:obj:`int` or :obj:`str`, optional): Optionally, reads the end
-        of conversion signal from a GPIO rather than from an I2C message.
-        Speeds up the reading and decreases the traffic on the bus, but
-        requires one extra wire. With the backend `'Pi4'`, give the index of
-        the GPIO in BCM convention. With the `'ft232h'` backend, give the name
-        of the GPIO in the format `Dx` or `Cx`. This feature is not available
-        with the `'blinka'` backend.
-      gain (:obj:`float`, optional): Allows to tune the output value according
-        to the formula:
-        ::
-
-          output = gain * tension + offset.
-
-      offset (:obj:`float`, optional): Allows to tune the output value
-        according to the formula:
-        ::
-
-          output = gain * tension + offset.
+      dry_pin: Optionally, reads the end of conversion signal from a GPIO
+        rather than from an I2C message. Speeds up the reading and decreases
+        the traffic on the I2C bus, but requires one extra wire. Give the name
+        of the GPIO in the format `Dx` or `Cx`.
+      gain: Allows to tune the output value according to the formula :
+        :math:`output = gain * tension + offset`.
+      offset: Allows to tune the output value according to the formula :
+        :math:`output = gain * tension + offset`.
+      _ft232h_args: This argument is meant for internal use only and should not
+        be provided by the user. It contains the information necessary for
+        setting up the FT232H.
 
     Warning:
       AINx voltages should not be higher than `VDD+0.3V` nor lower than
       `GND-0.3V`. Setting high ``v_range`` values does not allow measuring
       voltages higher than `VDD` !!
     """
 
@@ -153,15 +151,15 @@
       raise TypeError('int_pin should be a string !')
     self._dry_pin = dry_pin
 
     self._gain = gain
     self._offset = offset
 
   def open(self) -> None:
-    """Sets the I2C communication and device."""
+    """Initializes the I2C communication and the device."""
 
     if not self._is_connected():
       raise IOError("The ADS1115 is not connected")
 
     # Setting the configuration register according to the user values
     init_value = Ads1115_config_mux[self._multiplexer]
     init_value |= Ads1115_config_gain[self._v_range]
@@ -181,15 +179,15 @@
 
   def get_data(self) -> List[float]:
     """Reads the registers containing the conversion result.
 
     The output is in Volts, unless a gain and offset are applied.
 
     Returns:
-      :obj:`list`: A list containing the timeframe and the voltage value
+      A :obj:`list` containing the timestamp and the voltage value.
     """
 
     # Reading the config register, and setting it so that the ADS1115 starts
     # a conversion
     ms_byte, ls_byte = self._bus.read_i2c_block_data(self._device_address,
                                                      Ads1115_pointer_config,
                                                      2)
@@ -218,15 +216,15 @@
       value_raw -= 2 ** 16
     value = value_raw * self._v_range / 2 ** 15
 
     out.append(self._offset + self._gain * value)
     return out
 
   def close(self) -> None:
-    """Closes the I2C bus"""
+    """Closes the I2C bus."""
 
     if self._bus is not None:
       self.log(logging.INFO, "Closing the ADS1115")
       self._bus.close()
 
   def _set_register(self, register_address: int, value: int) -> None:
     """Thin wrapper for writing data to the registers."""
@@ -237,27 +235,27 @@
     self._bus.write_i2c_block_data(self._device_address, register_address,
                                    [(value >> 8) & 0xFF, value & 0xFF])
 
   def _is_connected(self) -> bool:
     """Tries reading a byte from the device.
 
     Returns:
-      :obj:`bool`: :obj:`True` if reading was successful, else :obj:`False`
+      :obj:`True` if reading was successful, else :obj:`False`.
     """
 
     try:
       self._bus.read_byte(self._device_address)
       return True
     except IOError:
       return False
 
   def _data_available(self) -> bool:
     """Returns :obj:`True` if data is available, :obj:`False` otherwise."""
 
     # EOC signal from the I2C communication
     if self._dry_pin is None:
-      return self._bus.read_i2c_block_data(self._device_address,
-                                           Ads1115_pointer_config,
-                                           1)[0] & 0x80
+      return bool(self._bus.read_i2c_block_data(self._device_address,
+                                                Ads1115_pointer_config,
+                                                1)[0] & 0x80)
     # EOC signal from a GPIO
     else:
       return not bool(self._bus.get_gpio(self._dry_pin))
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/ft232h/gpio_switch_ft232h.py` & `crappy-2.0.0.dev2/src/crappy/inout/ft232h/gpio_switch.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,35 +3,40 @@
 from typing import Union
 
 from ..meta_inout import InOut
 from ...tool.ft232h import FT232HServer as FT232H, ft232h_pin_nr, USBArgsType
 
 
 class GPIOSwitchFT232H(InOut):
-  """Class for setting a GPIO high or low.
+  """This class can drive a GPIO high or low on a FT232H.
 
-  The GPIOSwitch InOut block is meant for switching a GPIO high or low
-  according to the input signal value. When the input signal is `1` the
-  GPIO is turned high, when the signal is `0` it is turned low. Any value other
-  than `0` and `1` raises an error.
+  It is similar to the :class:`~crappy.inout.GPIOSwitch` class, except this
+  class is specific for use with an :class:`~crappy.tool.ft232h.FT232H` USB to
+  GPIO converter.
+
+  When the command value is `1` the GPIO is turned high, when the command is
+  `0` it is turned low. Any value other than `0` and `1` raises an error.
   """
 
   ft232h = True
 
   def __init__(self,
                pin_out: Union[int, str],
                _ft232h_args: USBArgsType = tuple()) -> None:
-    """Checks the argument validity.
+    """Checks the validity of the arguments.
 
     Args:
       pin_out: The GPIO pin to be controlled. On Raspberry Pi, should be an
         integer corresponding to a GPIO in BCM convention. On FT232H, should be
         a string corresponding to the name of a GPIO. With the `'blinka'`
         backend, should be a string holding the name of the pin. Refer to
         blinka's specific documentation for each board for more information.
+      _ft232h_args: This argument is meant for internal use only and should not
+        be provided by the user. It contains the information necessary for
+        setting up the FT232H.
     """
 
     self._ft232h = None
     self._pin_out = None
 
     # Checking that the given pin is valid
     if pin_out not in ft232h_pin_nr:
@@ -52,15 +57,15 @@
 
     self._pin_out = pin_out
 
   def set_cmd(self, *cmd: int) -> None:
     """Drives the GPIO according to the command.
 
     Args:
-      cmd (:obj:`int`): 1 for driving the GPIO high, 0 for driving it low
+      cmd: 1 for driving the GPIO high, 0 for driving it low.
     """
 
     if cmd[0] not in [0, 1]:
       raise ValueError("The GPIO input can only be 0 or 1")
 
     self._ft232h.set_gpio(self._pin_out, cmd[0])
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/ft232h/mcp9600_ft232h.py` & `crappy-2.0.0.dev2/src/crappy/inout/ft232h/mcp9600.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,74 +57,82 @@
 Mcp9600_modes = ['Hot Junction Temperature',
                  'Junction Temperature Delta',
                  'Cold Junction Temperature',
                  'Raw Data ADC']
 
 
 class MCP9600FT232H(InOut):
-  """Class for controlling Adafruit's MCP9600 thermocouple reader.
+  """This class can read temperature values from an MCP9600 thermocouple
+  reader through an FT232H.
 
-  The MCP9600 InOut block is meant for reading temperature from an MCP9600
-  board, using the I2C protocol. The output is in `°C`, except for one
-  operating mode that returns Volts.
+  It is similar to the :class:`~crappy.inout.MCP9600` class, except this class
+  is specific for use with an :class:`~crappy.tool.ft232h.FT232H` USB to I2C
+  converter.
+
+  It communicates over the I2C protocol. The output is in `°C`, except for one
+  operating mode that returns Volts. Several parameters can be tuned, like the
+  thermocouple type, the reading resolution or the filter coefficient. Note
+  that the MCP9600 can only achieve a data rate of a few Hz.
   """
 
   ft232h = True
 
   def __init__(self,
                thermocouple_type: str,
                device_address: int = 0x67,
                adc_resolution: int = 18,
                sensor_resolution: float = 0.0625,
                filter_coefficient: int = 0,
                mode: str = 'Hot Junction Temperature',
                _ft232h_args: USBArgsType = tuple()) -> None:
-    """Checks arguments validity.
+    """Checks the validity of the arguments.
 
     Args:
-      thermocouple_type (:obj:`str`): The type of thermocouple plugged in the
-        MCP9600. The available types are:
+      thermocouple_type: The type of thermocouple connected to the MCP9600. The
+        possible types are:
         ::
 
           'J', 'K', 'T', 'N', 'S', 'E', 'B', 'R'
 
-      device_address(:obj:`int`, optional): The I2C address of the MCP9600. The
-        default address is `0x67`, but it is possible to change this setting
-        using a specific setup involving the `ADDR` pin.
-      adc_resolution(:obj:`int`, optional): The number of bits the ADC output
-        is encoded on. The greater the resolution, the lower the sample rate.
-        The available resolutions are:
+      device_address: The I2C address of the MCP9600. The default address is
+        `0x67`, but it is possible to change this setting using a specific
+        setup involving the `ADDR` pin.
+      adc_resolution: The number of bits the ADC output is encoded on. The
+        greater the resolution, the lower the sample rate. The available
+        resolutions are:
         ::
 
           12, 14, 16, 18
 
-      sensor_resolution(:obj:`float`, optional): The temperature measurement
-        resolution in `°C`. It should be either `0.0625` or `0.25`. Setting the
-        resolution to `0.25` will increase the sample rate, but the output
-        temperature will be encoded on two bits less.
-      filter_coefficient(:obj:`int`, optional): The MCP9600 features an
-        integrated filter (see its documentation for the exact filter formula).
-        When set to `0`, the filter is inactive. It is maximal when set to `7`.
-        When active, the filter will prohibit fast temperature changes, thus
-        limiting noise and smoothening the signal.
-      mode(:obj:`str`, optional): Four different values can be accessed when
-        measuring a temperature: the temperature of the thermocouple (hot
-        junction temperature), the temperature of the MCP9600 board (cold
-        junction temperature), the temperature calculated from the ADC data and
-        thermocouple type but not yet cold junction-compensated (junction
-        temperature delta), and the raw ADC measurement of the voltage
-        difference in the thermocouple (raw data ADC, in Volts). The available
-        modes are thus:
+      sensor_resolution: The temperature measurement resolution in `°C`. It
+        should be either `0.0625` or `0.25`. Setting the resolution to `0.25`
+        will increase the sample rate, but the output temperature will be
+        encoded on two bits less.
+      filter_coefficient: The MCP9600 features an integrated filter (see its
+        documentation for the exact filter formula). When set to `0`, the
+        filter is inactive. It is maximal when set to `7`. When active, the
+        filter will prohibit fast temperature changes, thus limiting noise and
+        smoothening the signal.
+      mode: Four different values can be accessed when measuring a temperature:
+        the temperature of the thermocouple (hot junction temperature), the
+        temperature of the MCP9600 board (cold junction temperature), the
+        temperature calculated from the ADC data and thermocouple type but not
+        yet cold junction-compensated (junction temperature delta), and the raw
+        ADC measurement of the voltage difference in the thermocouple (raw data
+        ADC, in Volts). The available modes are thus:
         ::
 
           'Hot Junction Temperature',
           'Junction Temperature Delta',
           'Cold Junction Temperature',
           'Raw Data ADC'
 
+      _ft232h_args: This argument is meant for internal use only and should not
+        be provided by the user. It contains the information necessary for
+        setting up the FT232H.
     """
 
     self._bus = None
 
     super().__init__()
 
     (block_index, block_lock, command_file, answer_file, shared_lock,
@@ -167,15 +175,15 @@
 
     if mode not in Mcp9600_modes:
       raise ValueError("mode should be in {}".format(Mcp9600_modes))
     else:
       self._mode = mode
 
   def open(self) -> None:
-    """Sets the I2C communication and device."""
+    """Initializes the I2C communication and the device."""
 
     if not self._is_connected():
       raise IOError("The MCP9600 is not connected")
     self.log(logging.INFO, "Setting up the MCP9600")
 
     # Setting the sensor according to the user parameters
     config_sensor = Mcp9600_filter_coefficients[self._filter_coefficient]
@@ -203,15 +211,15 @@
   def get_data(self) -> List[float]:
     """Reads the registers containing the conversion result.
 
     The output is in `°C` for all modes except the raw data ADC one, which
     outputs Volts.
 
     Returns:
-      :obj:`list`: A list containing the timeframe and the output value
+      A :obj:`list`: containing the timestamp and the output value.
     """
 
     # Starting a conversion
     value = self._bus.read_i2c_block_data(self._device_address,
                                           Mcp9600_registers['Status'], 1)[0]
     self.log(logging.DEBUG, f"Read {value} from register "
                             f"{Mcp9600_registers['Status']} at address "
@@ -265,15 +273,15 @@
         value_raw -= 2 ** 18
 
       out.append(value_raw * 2E-6)
 
     return out
 
   def close(self) -> None:
-    """Switches the MCP9600 to shut down mode and closes the I2C bus.."""
+    """Switches the MCP9600 to shutdown mode and closes the I2C bus."""
 
     if self._bus is not None:
       # Switching to shut down mode, keeping configuration
       value = self._bus.read_i2c_block_data(self._device_address,
                                             Mcp9600_registers[
                                              'Device Configuration'], 1)[0]
       self.log(logging.DEBUG, f"Read {value} from register "
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/ft232h/mprls_ft232h.py` & `crappy-2.0.0.dev2/src/crappy/inout/ft232h/mprls.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,40 +9,43 @@
 
 mprls_status_bits = {'busy': 0x20,
                      'memory error': 0x04,
                      'math saturation': 0x01}
 
 
 class MPRLSFT232H(InOut):
-  """The MPRLS inout is meant for reading pressure from Adafruit's MPRLS
-    pressure sensor.
+  """This class can read values from an MPRLS pressure sensor through an
+  FT232H.
 
-    It communicates over I2C with the sensor.
-    """
+  It is similar to the :class:`~crappy.inout.MPRLS` class, except this class is
+  specific for use with an :class:`~crappy.tool.ft232h.FT232H` USB to I2C
+  converter.
+
+  It communicates over I2C with the sensor.
+  """
 
   ft232h = True
 
   def __init__(self,
                eoc_pin: Optional[str] = None,
                device_address: int = 0x18,
                _ft232h_args: USBArgsType = tuple()) -> None:
     """Initializes the parent class and opens the I2C bus.
 
     Args:
-      eoc_pin (:obj:`int` or :obj:`str`, optional): Optionally, reads the end
-        of conversion signal from a GPIO rather than from an I2C message.
-        Speeds up the reading and decreases the traffic on the bus, but
-        requires one extra wire. With the backend `'Pi4'`, give the index of
-        the GPIO in BCM convention. With the `'ft232h'` backend, give the name
-        of the GPIO in the format `Dx` or `Cx`. With the backend `'blinka'`,
-        it should be a string but the syntax varies according to the board.
-        Refer to blinka's documentation for more information.
-      device_address (:obj:`int`, optional): The I2C address of the MPRLS.
-        The address of the devices sold by Adafruit is `0x18`, but other
-        suppliers may sell it with another address.
+      eoc_pin: Optionally, reads the end of conversion signal from the polarity
+        of a GPIO rather than from an I2C register. Speeds up the reading and
+        decreases the traffic on the bus, but requires one extra wire. Give the
+        name of the GPIO in the format `Dx` or `Cx`.
+      device_address: The I2C address of the MPRLS. The address of the devices
+        sold by Adafruit is `0x18`, but other suppliers may sell it with
+        another address.
+      _ft232h_args: This argument is meant for internal use only and should not
+        be provided by the user. It contains the information necessary for
+        setting up the FT232H.
     """
 
     self._bus = None
 
     super().__init__()
 
     (block_index, block_lock, command_file, answer_file, shared_lock,
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/ft232h/nau7802_ft232h.py` & `crappy-2.0.0.dev2/src/crappy/inout/ft232h/nau7802.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 from time import time, sleep
-from typing import Union, Optional, List
+from typing import Optional, List
 import logging
 
 from ..meta_inout import InOut
 from ...tool.ft232h import FT232HServer as FT232H, USBArgsType
 
 # Register Map
 NAU7802_Scale_Registers = {'PU_CTRL': 0x00,
@@ -91,69 +91,67 @@
                       'CAL_IN_PROGRESS': 1,
                       'CAL_FAILURE': 2}
 
 NAU7802_VREF = 3.3
 
 
 class NAU7802FT232H(InOut):
-  """Class for controlling Sparkfun's NAU7802 load cell conditioner.
+  """This class can read values from a NAU7802 load cell conditioner.
 
-  The NAU7802 InOut block is meant for reading output values from a NAU7802
-  load cell conditioner, using the I2C protocol. The output is in Volts by
-  default, but can be converted to Newtons using ``gain`` and ``offset``.
+  It is similar to the :class:`~crappy.inout.NAU7802` class, except this class 
+  is specific for use with an :class:`~crappy.tool.ft232h.FT232H` USB to I2C
+  converter.
+
+  This load cell conditioner is a low-cost 24-bits, single-channel conditioner,
+  that can read up to 320 samples per second. It communicates over the I2C
+  protocol. The returned value of the InOut is in Volts by default, but can be
+  converted to Newtons using the ``gain`` and ``offset`` arguments.
   """
 
   ft232h = True
 
   def __init__(self,
                device_address: int = 0x2A,
                gain_hardware: int = 128,
                sample_rate: int = 80,
-               int_pin: Optional[Union[str, int]] = None,
+               int_pin: Optional[str] = None,
                gain: float = 1,
                offset: float = 0,
                _ft232h_args: USBArgsType = tuple()) -> None:
-    """Checks the validity of the arguments..
+    """Checks the validity of the arguments.
 
     Args:
-      device_address (:obj:`int`, optional): The I2C address of the NAU7802. It
-        is impossible to change this address, so it is not possible to have
-        several NAU7802 on the same i2c bus.
-      gain_hardware (:obj:`int`, optional): The gain to be used by the
-        programmable gain amplifier. Setting a high gain allows reading small
-        voltages with a better precision, but it might saturate the sensor for
-        higher voltages. Available gains are:
+      device_address: The I2C address of the NAU7802. It is impossible to
+        change this address, so it is not possible to have several NAU7802
+        connected on the same I2C bus.
+      gain_hardware: The gain to be used by the programmable gain amplifier.
+        Setting a high gain allows reading small voltages with a better
+        precision, but it might saturate the sensor for higher voltages.
+        Available gains are:
         ::
 
           1, 2, 4, 8, 16, 32, 64, 128
 
-      sample_rate (:obj:`int`, optional): The sample rate for data conversion.
-        The higher the rate, the greater the noise. Available sample rates are:
+      sample_rate: The sample rate for data conversion. The higher the rate,
+        the greater the noise. Available sample rates are:
         ::
 
           10, 20, 40, 80, 320
 
-      int_pin (:obj:`int` or :obj:`str`, optional): Optionally, reads the end
-        of conversion signal from a GPIO rather than from an I2C message.
-        Speeds up the reading and decreases the traffic on the bus, but
-        requires one extra wire. With the backend `'Pi4'`, give the index of
-        the GPIO in BCM convention. With the `'ft232h'` backend, give the name
-        of the GPIO in the format `Dx` or `Cx`.
-      gain (:obj:`float`, optional): Allows to tune the output value according
-        to the formula:
-        ::
-
-          output = gain * tension + offset.
-
-      offset (:obj:`float`, optional): Allows to tune the output value
-        according to the formula:
-        ::
-
-          output = gain * tension + offset.
-
+      int_pin: Optionally, reads the end of conversion signal from the polarity
+        of a GPIO rather than from an I2C register. Speeds up the reading and
+        decreases the traffic on the bus, but requires one extra wire. Give the
+        name of the GPIO in the format `Dx` or `Cx`.
+      gain: Allows to tune the output value according to the formula :
+        :math:`output = gain * tension + offset`.
+      offset: Allows to tune the output value according to the formula :
+        :math:`output = gain * tension + offset`.
+      _ft232h_args: This argument is meant for internal use only and should not
+        be provided by the user. It contains the information necessary for
+        setting up the FT232H.
     """
 
     self._bus = None
 
     super().__init__()
 
     (block_index, block_lock, command_file, answer_file, shared_lock,
@@ -186,15 +184,15 @@
                       'backend !')
     self._int_pin = int_pin
 
     self._gain = gain
     self._offset = offset
 
   def open(self) -> None:
-    """Sets the I2C communication and device."""
+    """Initializes the I2C communication and the device."""
 
     if not self._is_connected():
       raise IOError("The NAU7802 is not connected")
 
     self.log(logging.INFO, "Setting up the NAU7802")
 
     # Resetting the device
@@ -250,15 +248,15 @@
   def get_data(self) -> List[float]:
     """Reads the registers containing the conversion result.
 
     The output is in Volts by default, and can be converted to Newtons using
     gain and offset.
 
     Returns:
-      :obj:`list`: A list containing the timeframe and the output value
+      A :obj:`list` containing the timeframe and the output value.
     """
 
     # Waiting for data to be ready
     t0 = time()
     while not self._data_available():
       if time() - t0 > 0.5:
         raise TimeoutError('Waited too long for data to be ready !')
@@ -295,15 +293,15 @@
       self.log(logging.INFO, "Closing the I2C connection to the NAU7802")
       self._bus.close()
 
   def _is_connected(self) -> bool:
     """Tries reading a byte from the device.
 
     Returns:
-      :obj:`bool`: :obj:`True` if reading was successful, else :obj:`False`
+      :obj:`True` if reading was successful, else :obj:`False`
     """
 
     try:
       self._bus.read_byte(self._device_address)
       return True
     except IOError:
       return False
@@ -322,17 +320,17 @@
   def _set_bit(self,
                bit_number: int,
                register_address: int,
                bit: int) -> None:
     """Sets a given bit in the specified register.
 
     Args:
-      bit_number (:obj:`int`): Position of the bit in the register
-      register_address (:obj:`int`): Index of the register
-      bit (:obj:`int`): Value of the bit
+      bit_number: Position of the bit in the register, as an :obj:`int`.
+      register_address: Index of the register, as an :obj:`int`.
+      bit: Value of the bit, as an :obj:`int`.
     """
 
     value = self._bus.read_i2c_block_data(self._device_address,
                                           register_address, 1)[0]
     self.log(logging.DEBUG, f"Read {value} from register {register_address}"
                             f" at address {self._device_address}")
     if bit:
@@ -345,33 +343,33 @@
 
   def _get_bit(self,
                bit_number: int,
                register_address: int) -> bool:
     """Reads a given bit in the specified register.
 
     Args:
-      bit_number (:obj:`int`): Position of the bit in the register
-      register_address (:obj:`int`): Index of the register
+      bit_number: Position of the bit in the register, as an :obj:`int`.
+      register_address: Index of the register, as an :obj:`int`.
 
     Returns:
-      :obj:`bool`: True if the bit value is 1, else False
+      :obj:`True` if the bit value is 1, else :obj:`False`.
     """
 
     value = self._bus.read_i2c_block_data(self._device_address,
                                           register_address, 1)[0]
     self.log(logging.DEBUG, f"Read {value} from register {register_address}"
                             f" at address {self._device_address}")
     value = value >> bit_number & 1
     return bool(value)
 
   def _cal_afe_status(self) -> int:
     """Reads the calibration status bits.
 
     Returns:
-      :obj:`int`: The int value corresponding to the current calibration status
+      The :obj:`int` value corresponding to the current calibration status.
     """
 
     if self._get_bit(NAU7802_CTRL2_Bits['CTRL2_CAL_ERROR'],
                      NAU7802_Scale_Registers['CTRL2']):
       return NAU7802_Cal_Status['CAL_FAILURE']
     elif self._get_bit(NAU7802_CTRL2_Bits['CTRL2_CALS'],
                        NAU7802_Scale_Registers['CTRL2']):
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/ft232h/waveshare_ad_da_ft232h.py` & `crappy-2.0.0.dev2/src/crappy/inout/ft232h/waveshare_ad_da.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 from time import time, sleep
 from re import fullmatch, findall
-from typing import List, Union, Optional
+from typing import List, Union, Optional, Iterable
 import logging
 
 from ..meta_inout import InOut
 from ...tool.ft232h import FT232HServer as FT232H, USBArgsType
 
 # ADS1256 gain channel
 Ads1256_gain = {1: 0b000,
@@ -64,106 +64,94 @@
                'CMD_STANDBY': 0xFD,
                'CMD_RESET': 0xFE}
 
 # Dac8532 channels definition
 Dac8532_chan = {0: 0x10,
                 1: 0x24}
 
-# Waveshare AD/DA pins definition
-AD_DA_pins = {'RST_PIN_ADS': 18,
-              'CS_PIN_ADS': 22,
-              'DRDY_PIN_ADS': 17,
-              'CS_PIN_DAC': 23}
-
 
 class WaveshareADDAFT232H(InOut):
-  """Class for controlling Waveshare's AD/DA hat from an FTDI FT232H.
+  """Class for controlling Waveshare's AD/DA Raspberry Pi hat through an
+  FT232H.
 
-  The WaveshareADDA InOut block is meant for communicating with Waveshare's
-  AD/DA Raspberry Pi hat from an FT232H, using the SPI protocol and the GPIOs.
-  It allows reading values from the 8-channels ADC and/or to set the 2-channels
-  DAC.
-
-  Warning:
-    This class is specifically meant to be used with an FT232H. See
-    :ref:`Waveshare AD/DA` for use with a Raspberry Pi.
+  It is similar to the :class:`~crappy.inout.WaveshareADDA` class, except this
+  class is specific for use with an :class:`~crappy.tool.ft232h.FT232H` USB to
+  I2C converter.
+
+  It communicates over the SPI protocol and the GPIOs. It allows to
+  read values from the 8-channels ADC and/or to set the 2-channels DAC. The hat
+  can acquire up to 30000 samples per second, although this data rate is
+  impossible to achieve using Crappy.
   """
 
   ft232h = True
 
   def __init__(self,
-               dac_channels: Optional[List[str]] = None,
-               adc_channels: Optional[List[str]] = None,
+               dac_channels: Optional[Iterable[str]] = None,
+               adc_channels: Optional[Iterable[str]] = None,
                gain_hardware: int = 1,
                v_ref: float = 3.3,
                gain: float = 1,
                offset: float = 0,
                sample_rate: Union[int, float] = 100,
                _ft232h_args: USBArgsType = tuple(),
                rst_pin_ads: str = 'D7',
                cs_pin_ads: str = 'D4',
                drdy_pin_ads: str = 'D6',
                cs_pin_dac: str = 'D5') -> None:
     """Checks the validity of the arguments.
 
     Args:
-      dac_channels (:obj:`list`, optional): A :obj:`list` of :obj:`str`
-        representing the channels to be set. The syntax for each string is
-        'DACi' with i being either `0` or `1`.
-      adc_channels (:obj:`list`, optional): A :obj:`list` of :obj:`str`
-        representing the channels to read. The syntax for all strings is
-        either:
+      dac_channels: An iterable (like a :obj:`list` or a :obj:`tuple`) of
+        :obj:`str` representing the channels to be set. The syntax for each
+        string is 'DACi' with i being either `0` or `1`.
+      adc_channels: An iterable (like a :obj:`list` or a :obj:`tuple`) of
+        :obj:`str` representing the channels to read. The syntax for all the
+        strings is either:
         ::
 
           'ADi' (i in range(8))
 
         or else:
         ::
 
           'ADi - ADj' (i, j in range(8))
 
-      gain_hardware (:obj:`int`, optional): The gain to be used by the
-        programmable gain amplifier. Setting a high gain allows reading small
-        voltages with a better precision, but it might saturate the sensor for
-        higher voltages. The available gain values are:
+      gain_hardware: The gain to be used by the programmable gain amplifier.
+        Setting a high gain allows to read small voltages with a better
+        precision, but it might saturate the sensor for higher voltages. The
+        available gain values are:
         ::
 
           1, 2, 4, 8, 16, 32, 64
 
-      v_ref (:obj:`float`, optional): The voltage reference set by the `VREF`
-        jumper. When reading single inputs, ``v_ref`` is the value the ADC
-        compares the signals with. In a similar way, the maximum output voltage
-        of the DAC is ``v_ref``. `3.3` and `5` are the only possible values for
-        this setting, as the Raspberry Pi can only provide `3.3V` and `5V`.
-      gain (:obj:`float`, optional): Allows to tune the output values of the
-        DAC according to the formula:
-        ::
-
-          output = gain * tension + offset.
-
-        The same gain applies to all the outputs.
-      offset (:obj:`float`, optional): Allows to tune the output values of the
-        ADC according to the formula:
-        ::
-
-          output = gain * tension + offset.
-
-        The same offset applies to all the outputs.
-      sample_rate (optional): The ADC data output rate in SPS. The available
-        values are:
+      v_ref: The voltage reference set by the `VREF` jumper. When reading
+        single inputs, ``v_ref`` is the value the ADC compares the signals
+        with. In a similar way, the maximum output voltage of the DAC is
+        ``v_ref``. `3.3` and `5` are the only possible values for this setting,
+        as the FT232H can only provide `3.3V` and `5V`.
+      gain: Allows to tune the output values of the ADC according to the
+        formula : :math:`output = gain * tension + offset`. The same gain
+        applies to all the outputs.
+      offset: Allows to tune the output values of the ADC according to the
+        formula : :math:`output = gain * tension + offset`. The same offset
+        applies to all the outputs.
+      sample_rate: The ADC data output rate in SPS. The available values are:
         ::
 
           2.5, 5, 10, 15, 25, 30, 50, 60, 100, 500,
           1000, 2000, 3750, 7500, 15000, 30000
 
-      rst_pin_ads (:obj:`str`, optional): The pin for resetting the ADS1256.
-      cs_pin_ads (:obj:`str`, optional): The chip select pin for the ADS1256.
-      drdy_pin_ads (:obj:`str`, optional): The pin for knowing when a
-        conversion result in ready.
-      cs_pin_dac (:obj:`str`, optional): The chip select pin for the DAC8552.
+      _ft232h_args: This argument is meant for internal use only and should not
+        be provided by the user. It contains the information necessary for
+        setting up the FT232H.
+      rst_pin_ads: The pin for resetting the ADS1256.
+      cs_pin_ads: The chip select pin for the ADS1256.
+      drdy_pin_ads: The pin for knowing when a conversion result in ready.
+      cs_pin_dac: The chip select pin for the DAC8552.
 
     Warning:
       - ``adc_channels``:
         For reading single inputs the `JMP_AGND` jumper should normally be
         connected, whereas it should be disconnected for reading differential
         inputs. It is however possible to set a different reference than `AGND`
         for single input measurements, in which case the `JMP_AGND` jumper
@@ -295,16 +283,16 @@
   def get_data(self) -> List[float]:
     """Reads data from all the user-specified ADC channels, in a sequential
     way.
 
     Data is returned in Volts, but this can be tuned using gain and offset.
 
     Returns:
-      :obj:`list`: A list containing the timeframe, and then the values for
-      each channel to read
+      A :obj:`list` containing the timestamp, and then the values for each
+      channel to read.
     """
 
     out = [time()]
 
     # The values are read one channel after the other, not simultaneously
     for chan in self._channels_read:
       self._bus.set_gpio(self._cs_pin_ads, False)
@@ -346,15 +334,15 @@
 
     return out
 
   def set_cmd(self, *cmd: float) -> None:
     """Sets the user-specified DAC channels according to the input values.
 
     Args:
-      cmd (:obj:`float`): The input values, in Volts
+      cmd: The input values as :obj:`float`, in Volts.
     """
 
     # The values are set one channel after the other, not simultaneously
     for val, channel in zip(cmd, self._channels_write):
       if not 0 <= val <= self._v_ref:
         raise ValueError("Desired output voltage should be between 0 and "
                          "v_ref")
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/gpio_pwm.py` & `crappy-2.0.0.dev2/src/crappy/inout/gpio_pwm.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,58 +9,56 @@
 try:
   import RPi.GPIO as GPIO
 except (ModuleNotFoundError, ImportError):
   GPIO = OptionalModule("RPi.GPIO")
 
 
 class GPIOPWM(InOut):
-  """ Class for performing PWM on a Raspberry Pi.
+  """This class can drive a PWM output on a Raspberry Pi.
 
-  The Gpio_pwn InOut block is meant for controlling a PWM output from a
-  Raspberry Pi GPIO. It allows to control the duty cycle, the frequency, or
-  both at the same time. When controlling both, the duty cycle should be first
-  and the frequency second in the list of inputs.
+  It allows controlling the duty cycle, the frequency, or both at the same
+  time. When controlling both, the duty cycle should be first and the frequency
+  second in the given commands.
 
   Warning:
     Only works on Raspberry Pi !
   """
 
   def __init__(self,
                pin_out: int,
                duty_cycle: Optional[float] = None,
                frequency: Optional[float] = None) -> None:
-    """Checks the argument validity.
+    """Checks the validity of the arguments.
 
     Args:
-      pin_out (:obj:`int`): The GPIO pin to be controlled (BCM convention).
-      duty_cycle (:obj:`float`): If provided, sets a fixed duty cycle for the
-        entire assay. Only the frequency can then be tuned. If not provided,
-        the block will expect the duty cycle values to be given as the first
-        input. It will also start the PWM with a duty cycle of `0%` before the
-        first value is received and set.
-      frequency (:obj:`float`): If provided, sets a fixed PWM frequency for the
-        entire assay. Only the duty cycle can then be tuned. If not provided,
-        the block will expect the frequency values to be given as the first
-        input if the ``duty_cycle`` argument is provided, or else as the second
-        input. It will also start the PWM with a frequency of `10kHz` before
-        the first value is received and set.
+      pin_out: The index of GPIO pin to drive in BCM convention, as an
+        :obj:`int`.
+      duty_cycle: If provided (as a :obj:`float`, in percent), sets a fixed
+        duty cycle for the entire test. Only the frequency can then be tuned.
+        If not provided, the duty cycle can be set as a command. The duty cycle
+        will also be set to `0%` until a first value is received.
+      frequency: If provided (as a :obj:`float`, in Hz), sets a fixed PWM
+        frequency for the entire test. Only the duty cycle can then be tuned.
+        If not provided, the frequency can be set as a command. The frequency
+        will also be set to `10kHz` until a first value is received. Note that
+        the frequency inputs are clamped between `10Hz` and `1MHz`.
 
     Note:
-      - ``duty_cycle``:
-        The duty cycle inputs are clamped between `0` and `100`.
+      Several values can be passed at once as a command. If both ``duty_cycle``
+      and ``frequency`` are provided, all the values are ignored. If only
+      ``frequency`` is provided, the first command value sets the duty cycle
+      and any other value is ignored. Same goes if only ``duty_cycle`` is
+      provided. If none of the two arguments are provided, the first command
+      value should set the duty cycle and the second command value should set
+      the frequency.
 
-      - ``frequency``:
-        The frequency inputs are clamped between `10Hz` and `1MhZ`. Sending
-        other values to the bloc doesn't raise any error, but the assay may not
-        run as expected.
-
-      - **Hardware PWM pins**:
-        On the Raspberry Pi 4, only the GPIO pins `12`, `13`, `18` and `19`
-        support hardware PWM. Trying to get a PWM output from other pins might
-        work but may decrease the available frequency range.
+    Note:
+      On the Raspberry Pi 4, only the GPIO pins `12`, `13`, `18` and `19`
+      support hardware PWM. Trying to get a PWM output from other pins might
+      work but may decrease the available frequency range.
     """
 
     self._pwm = None
 
     super().__init__()
 
     if pin_out not in range(2, 28):
@@ -100,40 +98,40 @@
     else:
       self._pwm.start(0)
 
   def set_cmd(self, *cmd: float) -> None:
     """Modifies the PWM frequency and/or duty cycle.
 
     Args:
-      *cmd (:obj:`float`): Values of duty cycle and/or frequency to set
+      *cmd: Values of duty cycle and/or frequency to set.
     """
 
     # If both frequency and duty cycle are fixed by the user, nothing to do
     if self._duty_cycle is not None and self._frequency is not None:
-      pass
+      return
 
     # If only frequency is fixed, setting the duty cycle
     elif self._frequency is not None:
-      dc = min(100, max(0, cmd[0]))
+      dc = min(100., max(0., cmd[0]))
       self._pwm.ChangeDutyCycle(dc)
 
     # If only the duty cycle is fixed, setting the frequency
     elif self._duty_cycle is not None:
-      freq = min(1000000, max(10, cmd[0]))
+      freq = min(1000000., max(10., cmd[0]))
       self._pwm.ChangeFrequency(freq)
 
     # If neither duty cycle nor frequency are fixed, setting both
     else:
-      dc = min(100, max(0, cmd[0]))
-      freq = min(1000000, max(10, cmd[1]))
+      dc = min(100., max(0., cmd[0]))
+      freq = min(1000000., max(10., cmd[1]))
       self._pwm.ChangeFrequency(freq)
       self._pwm.ChangeDutyCycle(dc)
 
   def close(self) -> None:
-    """Stops PWM and releases GPIOs."""
+    """Stops the PWM and releases the GPIOs."""
 
     if self._pwm is not None:
       self.log(logging.INFO, "Stopping the PWM")
       self._pwm.stop()
 
     self.log(logging.INFO, "Cleaning up the GPIOs")
     GPIO.cleanup()
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/gpio_switch.py` & `crappy-2.0.0.dev2/src/crappy/inout/gpio_switch.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,43 +22,39 @@
   digitalio = OptionalModule('digitalio',
                              'Blinka is necessary to access the GPIOs')
 
 gpio_switch_backends = ['Pi4', 'blinka']
 
 
 class GPIOSwitch(InOut):
-  """Class for setting a GPIO high or low.
+  """This class can drive a GPIO high or low on a single board computer.
 
-  The GPIOSwitch InOut block is meant for switching a GPIO high or low
-  according to the input signal value. When the input signal is `1` the
-  GPIO is turned high, when the signal is `0` it is turned low. Any value other
-  than `0` and `1` raises an error.
+  When the command value is `1` the GPIO is turned high, when the command is
+  `0` it is turned low. Any value other than `0` and `1` raises an error.
   """
 
   def __init__(self,
                pin_out: Union[int, str],
                backend: str) -> None:
-    """Checks the argument validity.
+    """Checks the validity of the arguments.
 
     Args:
       pin_out: The GPIO pin to be controlled. On Raspberry Pi, should be an
-        integer corresponding to a GPIO in BCM convention. On FT232H, should be
-        a string corresponding to the name of a GPIO. With the `'blinka'`
-        backend, should be a string holding the name of the pin. Refer to
-        blinka's specific documentation for each board for more information.
+        :obj:`int` corresponding to a GPIO in BCM convention. With the
+        `'blinka'` backend, should be a string holding the name of the pin.
+        Refer to blinka's specific documentation for each board for more
+        information.
       backend: Should be one of :
         ::
 
-          'Pi4', 'blinka', 'ft232h'
+          'Pi4', 'blinka'
 
         The `'Pi4'` backend only works on the Raspberry Pis. The `'blinka'`
-        backend requires installing Adafruit's modules, but is compatible with
-        and maintained on a wide variety of boards. The `'ft232h'` backend
-        allows controlling the GPIO from a PC using Adafruit's FT232H USB to
-        I2C adapter. See :ref:`Crappy for embedded hardware` for details.
+        backend requires installing :mod:`Adafruit-Blinka`, but this module is
+        compatible with and maintained on a wide variety of boards.
     """
 
     self._pin_out = None
 
     # Checking that the backend is valid
     if not isinstance(backend, str) or backend not in gpio_switch_backends:
       raise ValueError("backend should be in {}".format(gpio_switch_backends))
@@ -78,29 +74,29 @@
     # Instantiating the pin object
     if backend == 'Pi4':
       self._pin_out = pin_out
     elif backend == 'blinka':
       self._pin_out = digitalio.DigitalInOut(getattr(board, pin_out))
 
   def open(self) -> None:
-    """Sets the GPIO."""
+    """Initializes the GPIO."""
 
     if self._backend == 'Pi4':
       self.log(logging.INFO, "Setting up the GPIOs")
       GPIO.setmode(GPIO.BCM)
       GPIO.setup(self._pin_out, GPIO.OUT)
 
     elif self._backend == 'blinka':
       self._pin_out.direction = digitalio.Direction.OUTPUT
 
   def set_cmd(self, *cmd: int) -> None:
     """Drives the GPIO according to the command.
 
     Args:
-      cmd (:obj:`int`): 1 for driving the GPIO high, 0 for driving it low
+      cmd: 1 for driving the GPIO high, 0 for driving it low.
     """
 
     if cmd[0] not in [0, 1]:
       raise ValueError("The GPIO input can only be 0 or 1")
 
     if self._backend == 'Pi4':
       GPIO.output(self._pin_out, cmd[0])
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/gsm.py` & `crappy-2.0.0.dev2/src/crappy/inout/sim868.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 # coding: utf-8
 
 from time import sleep
-from typing import List
+from typing import Iterable
 import logging
 
 from .meta_inout import InOut
 from .._global import OptionalModule
 
 try:
   from serial import Serial
   from serial.serialutil import SerialException
 except (ModuleNotFoundError, ImportError):
   serial = OptionalModule("serial", "Please install the module serial to use "
-                          "the GSM InOut: pip install pyserial")
+                          "the Sim868 InOut: pip install pyserial")
 
 
-class GSM(InOut):
-  """Block for sending messages by SMS to given phone numbers.
+class Sim868(InOut):
+  """This class can drive a SIM868 cellular module so that it sends SMS to
+  given phone numbers.
 
   Important:
-    This block should be associated with a modifier to manage the messages
-    to send.
+    This InOut should be associated with a :class:`~crappy.modifier.Modifier`
+    to manage the messages to send.
   """
 
   def __init__(self,
-               numbers: List[str],
+               numbers: Iterable[str],
                port: str = "/dev/ttyUSB0",
                baudrate: int = 115200) -> None:
-    """Checks arguments validity.
+    """Checks the validity of the arguments.
 
     Args:
-      numbers(:obj:`list`): The list of numbers the messages will be sent to.
-        The syntax is the following :
+      numbers: An iterable (like a :obj:`list` or a :obj:`tuple`) of numbers
+        the messages will be sent to. The syntax is the following :
         ::
 
           ["0611223344"]
 
-      port (:obj:`str`, optional): Serial port the GSM is connected to.
-      baudrate(:obj:`int`, optional): Serial baudrate, between 1200 and 115200.
+      port: Serial port the Sim868 is connected to.
+      baudrate: Serial baudrate, between `1200` and `115200`.
     """
 
     self._ser = None
 
     super().__init__()
 
     self._port = port
     self._baudrate = baudrate
 
     # Change the type of numbers to bytes rather than string
     self._numbers = [number.encode('utf-8') for number in numbers]
 
   def open(self) -> None:
-    """Sends ``"AT"`` to the GSM and waits for the response : ``"OK"``. """
+    """Sends ``"AT"`` to the Sim868 and waits for the response : ``"OK"``. """
 
     try:
       self.log(logging.INFO, f"Opening the serial port {self._port} with "
                              f"baudrate {self._baudrate}")
       self._ser = Serial(self._port, self._baudrate)
     except SerialException:
-      raise SerialException("GSM not connected or wrong port")
+      raise SerialException("Sim868 not connected or wrong port")
 
     self.log(logging.DEBUG, f"Writing b'AT\\r\\n' to port {self._port}")
     self._ser.write(b'AT' + b'\r\n')
     count = 0
     while count <= 2:
       sleep(0.1)
       data = ""
       while self._ser.inWaiting() > 0:
         data += self._ser.read(self._ser.inWaiting()).decode()
       self.log(logging.DEBUG, f"Read {data} from port {self._port}")
       if "OK" in data:
         return
       count += 1
-    raise TimeoutError("GSM is not responding")
+    raise TimeoutError("Sim868 is not responding")
 
   def set_cmd(self, *cmd: str) -> None:
     """Sends an SMS whose text is the :obj:`str` received as command to all the
     phone numbers.
 
     Doesn't send anything if the string is empty, and raises a :exc:`TypeError`
     if the command is not a :obj:`str`.
@@ -84,18 +85,18 @@
 
     if not isinstance(cmd[0], str):
       raise TypeError("Message should be a string")
     if cmd[0] != "":
       self._send_mess(cmd[0])
 
   def _send_mess(self, message: str) -> None:
-    """Commands the GSM to send a message to all the phone numbers.
+    """Commands the Sim868 to send a message to all the phone numbers.
 
     Args:
-      message: The text message to send.
+      message: The text message to send, as a :obj:`str`.
     """
 
     for number in self._numbers:
       count = 0
       self.log(logging.DEBUG, f"Writing b'AT\\r\\n' to port {self._port}")
       self._ser.write(b'AT' + b'\r\n')
       w_buff = [b"AT+CMGF=1\r\n",
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/kollmorgen.py` & `crappy-2.0.0.dev2/src/crappy/inout/kollmorgen_akd_pdmm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 from time import time
 from struct import pack, unpack
-from typing import List
+from typing import List, Iterable
 import logging
 
 from .meta_inout import InOut
 from .._global import OptionalModule
 try:
   from pymodbus.client.tcp import ModbusTcpClient
 except (ModuleNotFoundError, ImportError):
@@ -29,47 +29,46 @@
             'direction': 8}
 
 input_reg_addr = {'act_speed': 0,
                   'act_position': 2,
                   'axis_state': 4}
 
 
-class Koll(InOut):
+class KollmorgenAKDPDMM(InOut):
   """This class can communicate with a KollMorgen AKD PDMM programmable
    multi-axis controller.
 
    It can either drive it in speed or in position. Multiple axes can be driven.
    The values of the current speeds or positions can also be retrieved.
    """
 
   def __init__(self,
-               axes: List[int],
+               axes: Iterable[int],
                mode: str = 'position',
                host: str = '192.168.0.109',
                port: int = 502) -> None:
-    """Sets the args and initializes the parent class.
+    """Sets the arguments and initializes the parent class.
 
     Args:
-      axes: A :obj:`list` containing the motors/axes to drive, given as
-        :obj:`int`.
-      mode: Should be either `'speed'` or `'position'`. Whether the axes
-        should be driven in speed or in position.
+      axes: An iterable (like a :obj:`list` or a :obj:`tuple`) containing the
+        motors/axes to drive, given as :obj:`int`.
+      mode: The driving mode, should be either `'speed'` or `'position'`.
       host: The IP address of the variator, given as a :obj:`str`.
       port: The network port over which to communicate with the variator, as
         an :obj:`int`.
     """
 
     self._variator = None
 
     super().__init__()
 
     # Making sure the given mode is correct
     if mode not in ('speed', 'position'):
-      raise ValueError("[KollMorgen] the mode argument should be either "
-                       "'speed' or 'position' !")
+      raise ValueError("The mode argument should be either 'speed' or "
+                       "'position' !")
 
     self._axes = axes
     self._mode = mode
     self._host = host
     self._port = port
 
   def open(self) -> None:
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/labjack_t7.py` & `crappy-2.0.0.dev2/src/crappy/inout/labjack_t7.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 from time import time
-from typing import List, Optional, Dict, Any, Union, Tuple
+from typing import List, Optional, Dict, Any, Union, Tuple, Iterable
 from itertools import chain
 from dataclasses import dataclass, field
 from multiprocessing import current_process
 import logging
 
 from .meta_inout import InOut
 from .._global import OptionalModule
@@ -22,15 +22,15 @@
 
 @dataclass
 class _Channel:
   """This class is a simple structure holding all the attributes a Labjack
   channel can have.
 
   Not all the attributes are used by every channel, but they all have a use for
-  at least on type of channel.
+  at least one type of channel.
   """
 
   name: Union[str, int]
 
   direction: bool = True
   dtype: Optional[int] = None
   address: int = 1
@@ -54,40 +54,41 @@
       else:
         logger = logging.getLogger(
           f"{current_process().name}.LabjackT7.Channel_{self.name}")
         logger.log(logging.WARNING, f"Unknown channel key : {key}, ignoring")
 
 
 class LabjackT7(InOut):
-  """This InOut object allows controlling a Labjack T7 device. It can use any
-  channel as input/output.
+  """This InOut allows controlling a Labjack T7 device. It can use any channel
+  as input/output.
 
   The Labjack T7 is a very complete DAQ board. It features several ADC, several
   DAC, as well as multiple GPIOs. It can also read thermocouples, and run LUA
   code on an integrated microcontroller. These features can all be controlled
   from Crappy.
 
   This class is not capable of streaming. For higher frequency, refer to the
-  :ref:`Labjack T7 Streamer` class.
+  :class:`~crappy.inout.T7Streamer` class.
   """
 
   def __init__(self,
-               channels: List[Dict[str, Any]],
+               channels: Iterable[Dict[str, Any]],
                device: str = 'ANY',
                connection: str = 'ANY',
                identifier: str = 'ANY',
-               write_at_open: Optional[List[tuple]] = None,
+               write_at_open: Optional[Iterable[tuple]] = None,
                no_led: bool = False) -> None:
-    """Sets the args and initializes the parent class.
+    """Sets the arguments and initializes the parent class.
 
     Args:
-      channels: A :obj:`list` of the channels to interface with on the Labjack.
-        Each object in this list should be a :obj:`dict` representing a single
-        channel, and whose keys provide information on the channel to use.
-        Refer to the note below for more information on the possible keys.
+      channels: An iterable (like a :obj:`list` or a :obj:`tuple`) of the
+        channels to interface with on the Labjack. Each object in this iterable
+        should be a :obj:`dict` representing a single channel, and whose keys
+        provide information on the channel to use. Refer to the note below for
+        more information on the possible keys.
       device: The type of Labjack to open. Possible values include :
         ::
 
           'ANY', 'T7', 'T4', 'DIGIT'
 
         Only tested with `'T7'` in Crappy.
       connection: The type of connection used for interfacing with the Labjack.
@@ -95,17 +96,18 @@
         ::
 
           'ANY', 'TCP', 'USB', 'ETHERNET', 'WIFI'
 
       identifier: Any extra information allowing to further identify the
         Labjack to open, like a serial number, an IP address, or a device name.
       write_at_open: If specific names or registers have to be written when
-        opening the channel, they can be given here as a :obj:`list` of
-        :obj:`tuple`. They will be written in the same order as in the given
-        list. Refer to the note below for the accepted formats.
+        opening the channel, they can be given here as an iterable (like a
+        :obj:`list` or a :obj:`tuple`) of :obj:`tuple`. They will be written in
+        the same order as in the given iterable. Refer to the note below for
+        the accepted formats.
       no_led: If :obj:`True`, turns off the LED on the Labjack. This led can
         generate noise on the channels `AIN0` and `AIN1`.
 
     Note:
       - ``channels`` keys:
 
         - name: The name of the channel to interface with, as written on the
@@ -121,43 +123,31 @@
               can be specified. It is always an output.
             - `(E/F/C/M IOx)`: Digital inputs/outputs. A gain and an offset
               can be specified. It can be either an input or an output, the
               default is output.
 
         - gain: If the channel is an input, the measured value will be
           modified directly by the Labjack as follows :
-          ::
-
-            returned_value = gain * measured_value + offset
-
-          If the channel is an output, the command value will be modified in
-          Crappy as follows before being sent to the Labjack :
-          ::
-
-            sent_value = gain * command + offset.
-
+          :math:`returned\_value = gain * measured\_value + offset`. If the
+          channel is an output, the command value will be modified in Crappy as
+          follows before being sent to the Labjack :
+          :math:`sent\_value = gain * command + offset`.
         - offset: If the channel is an input, the measured value will be
           modified directly by the Labjack as follows :
-          ::
-
-            returned_value = gain * measured_value + offset
-
-          If the channel is an output, the command value will be modified in
-          Crappy as follows before being sent to the Labjack :
-          ::
-
-            sent_value = gain * command + offset
-
+          :math:`returned\_value = gain * measured\_value + offset`. If the
+          channel is an output, the command value will be modified in Crappy as
+          follows before being sent to the Labjack :
+          :math:`sent\_value = gain * command + offset`.
         - make_zero: If :obj:`True`, data will be acquired on this channel
           before the test starts, and a compensation value will be deduced
           so that the offset of this channel is `0`. The compensation is
           performed directly by the Labjack. This setting only has effect for
-          `AIN` channels defined as inputs. **It will only take effect if the
-          ``make_zero_delay`` argument of the :ref:`IOBlock` controlling the
-          Labjack is set** !
+          `AIN` channels defined as inputs. **It will only take effect if the**
+          ``make_zero_delay`` **argument of the**
+          :class:`~crappy.blocks.IOBlock` **controlling the Labjack is set** !
 
         - direction: If :obj:`True`, the channel is considered as an output,
           else as an input. Only has effect for `IO` channels, the default is
           output.
 
         - resolution: The resolution of the acquisition as an integer, refer to
           Labjack documentation for more details. The higher this value the
@@ -207,28 +197,28 @@
 
     # Identifiers for the device to open
     self._device = device
     self._connection = connection
     self._identifier = identifier
 
     # List of commands to send when opening the Labjack
-    self._write_at_open = [] if write_at_open is None else write_at_open
+    self._write_at_open = [] if write_at_open is None else list(write_at_open)
     if no_led:
       self._write_at_open.append(('POWER_LED', 0))
 
     self._channels_in = list()
     self._channels_out = list()
 
     # Parsing the setting dict given for each channel
     for channel in channels:
 
       # Checking that the name was given as it's the most important attribute
       if 'name' not in channel:
-        raise AttributeError("[Labjack T7] The given channels must contain "
-                             "the 'name' key !")
+        raise AttributeError("The given channels must contain the 'name' "
+                             "key !")
       name = channel['name']
 
       # Modbus registers
       if isinstance(name, int):
         chan = _Channel(name=name, dtype=ljm.constants.FLOAT32)
         chan.update(channel)
 
@@ -293,30 +283,30 @@
         # Can be either input or output, the user has to specify
         if chan.direction:
           self._channels_out.append(chan)
         else:
           self._channels_in.append(chan)
 
       else:
-        raise AttributeError(f"[Labjack T7] Invalid chan name: {name}")
+        raise AttributeError(f"Invalid chan name: {name}")
 
     self.log(logging.DEBUG, f"Input channels: {self._channels_in}")
     self.log(logging.DEBUG, f"Output channels: {self._channels_out}")
 
     # Extracting the addresses and data types from all channels
     self._read_addresses = [chan.address for chan in self._channels_in]
     self._read_types = [chan.dtype for chan in self._channels_in]
     self._write_addresses = [chan.address for chan in self._channels_out]
     self._write_types = [chan.dtype for chan in self._channels_out]
 
     # These attributes will come in use later
     self._last_sent_val = [None for _ in self._write_addresses]
 
   def open(self) -> None:
-    """Opening the Labjack, parsing the commands to write at open, and sending
+    """Opens the Labjack, parses the commands to write at open, and sends
     them."""
 
     # Opening the Labjack
     self.log(logging.INFO, "Opening the connection to the Labjack")
     self._handle = ljm.openS(self._device, self._connection, self._identifier)
 
     # Gathering all the data to write at open
@@ -340,19 +330,19 @@
       ljm.eWriteAddresses(handle=self._handle,
                           numFrames=len(reg),
                           aAddresses=reg,
                           aDataTypes=types,
                           aValues=values)
 
   def make_zero(self, delay: float) -> None:
-    """Overriding of the method of the parent class, because the Labjack T7
+    """Overriding the method of the parent class, because the Labjack T7
     allows setting offsets directly on the board.
 
     Setting the offsets on the Labjack is slightly quicker than correcting the
-    received values afterwards.
+    received values afterward.
 
     Args:
       delay: The delay during which the data should be acquired for determining
         the offset.
     """
 
     # No need to acquire data if no channel should be zeroed
@@ -378,27 +368,28 @@
                         aNames=names,
                         aValues=values)
 
         # Resetting the software offsets to avoid double compensation
         self._compensations = list()
 
   def get_data(self) -> List[float]:
-    """Read the signal on all pre-defined input channels."""
+    """Reads the signal on all pre-defined input channels, and returns the
+    values along with a timestamp.."""
 
     return [time()] + ljm.eReadAddresses(handle=self._handle,
                                          numFrames=len(self._read_addresses),
                                          aAddresses=self._read_addresses,
                                          aDataTypes=self._read_types)
 
   def set_cmd(self, *cmd: float) -> None:
     """Sets the tension commands on the output channels.
 
     The given gain and offset are first applied, then the commands are clamped
     to the given limits. The commands are then written to the Labjack, only if
-    they differ from the last ones.
+    they differ from the last written ones.
     """
 
     # First, applying the given gain and offsets to the commands
     cmd = [chan.gain * val + chan.offset
            for val, chan in zip(cmd, self._channels_out)]
 
     # Then, clamping the commands if limits were given
@@ -427,15 +418,15 @@
         ljm.eWriteAddresses(handle=self._handle,
                             numFrames=len(addresses),
                             aAddresses=addresses,
                             aDataTypes=types,
                             aValues=values)
 
   def close(self) -> None:
-    """Closes the Labjack."""
+    """Closes the connection to the Labjack."""
 
     if self._handle is not None:
       self.log(logging.INFO, "Closing the connection to the Labjack")
       ljm.close(self._handle)
 
   @staticmethod
   def _parse(name: str) -> Tuple[int, int]:
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/labjack_t7_streamer.py` & `crappy-2.0.0.dev2/src/crappy/inout/labjack_t7_streamer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 from time import time
 import numpy as np
-from typing import List, Dict, Any, Optional, Tuple
+from typing import List, Dict, Any, Optional, Tuple, Iterable
 from dataclasses import dataclass, field
 from itertools import chain
 from multiprocessing import current_process
 import logging
 
 from .meta_inout import InOut
 from .._global import OptionalModule
@@ -43,18 +43,18 @@
       else:
         logger = logging.getLogger(
           f"{current_process().name}.LabjackT7.Channel_{self.name}")
         logger.log(logging.WARNING, f"Unknown channel key : {key}, ignoring")
 
 
 class T7Streamer(InOut):
-  """This InOut object allows controlling a Labjack T7 device in stream mode.
+  """This InOut allows controlling a Labjack T7 device in stream mode.
 
   It can only acquire data on the `AIN` channels. For single point mode, and
-  acquisition on all channels, use the :ref:`Labjack T7` InOut.
+  acquisition on all channels, use the :class:`~crappy.inout.LabjackT7` InOut.
 
   Compared with single point acquisition, the streaming mode can achieve much
   higher data rates and has a much greater regularity in the frequency of the
   acquisition. However, fewer options are available and not all types of
   channels can be read in the streamer mode.
 
   For each channel, the voltage range can be tuned, and a gain and offset can
@@ -64,28 +64,29 @@
   Important:
     The ``streamer`` argument of the IOBlock controlling this InOut must be set
     to :obj:`True` to enable streaming in this class. Otherwise, only single
     point acquisition can be performed.
   """
 
   def __init__(self,
-               channels: List[Dict[str, Any]],
+               channels: Iterable[Dict[str, Any]],
                device: str = 'ANY',
                connection: str = 'ANY',
                identifier: str = 'ANY',
                scan_rate: int = 100000,
                scan_per_read: int = 10000,
                resolution: int = 1) -> None:
-    """Sets the args and initializes the parent class.
+    """Sets the arguments and initializes the parent class.
 
     Args:
-      channels: A :obj:`list` of the channels to interface with on the Labjack.
-        Each object in this list should be a :obj:`dict` representing a single
-        channel, and whose keys provide information on the channel to use.
-        Refer to the note below for more information on the possible keys.
+      channels: An iterable (like a :obj:`list` or a :obj:`tuple`) of the
+        channels to interface with on the Labjack. Each object in this iterable
+        should be a :obj:`dict` representing a single channel, and whose keys
+        provide information on the channel to use. Refer to the note below for
+        more information on the possible keys.
       device: The type of Labjack to open. Possible values include :
         ::
 
           'ANY', 'T7', 'T4', 'DIGIT'
 
         Only tested with `'T7'` in Crappy.
       connection: The type of connection used for interfacing with the Labjack.
@@ -110,42 +111,40 @@
       - ``channels`` keys:
 
         - name: The name of the channel to interface with, as written on the
           Labjack's case. Ex: `'AIN0'`. In streamer mode, only the `AIN`
           channels, i.e. the analog inputs, are available.
 
         - gain: The measured value will be modified in Crappy as follows :
-          ::
-
-            returned_value = gain * measured_value + offset
+          :math:`returned\_value = gain * measured\_value + offset`.
 
         - offset: The measured value will be modified in Crappy as follows :
-          ::
-
-            returned_value = gain * measured_value + offset
+          :math:`returned\_value = gain * measured\_value + offset`
 
         - make_zero: If :obj:`True`, data will be acquired on this channel
           before the test starts, and a compensation value will be deduced
           so that the offset of this channel is `0`. **It will only take effect
-          if the ``make_zero_delay`` argument of the :ref:`IOBlock` controlling
-          the Labjack is set** !
+          if the** ``make_zero_delay`` **argument of the**
+          :class:`~crappy.blocks.IOBlock` **controlling the Labjack is set** !
 
         - range: The range of the acquisition in Volts. A range of `x` means
           that values can be read  between `-x` and `x` Volts. The possible
           values are :
           ::
 
             0.01, 0.1, 1, 10
 
     """
 
     self._handle = None
 
     super().__init__()
 
+    channels = list(channels)
+
     if len(channels) * scan_rate > 100000:
       scan_rate = 100000 / len(channels)
       self.log(logging.WARNING,
                f"scan_rate is too high! Sample rate cannot exceed 100kS/s, "
                f"lowering samplerate to {scan_rate} samples/s")
 
     self._device = device
@@ -158,16 +157,16 @@
     self._channels = list()
 
     # Parsing the setting dict given for each channel
     for channel in channels:
 
       # Checking that the name was given as it's the most important attribute
       if 'name' not in channel:
-        raise AttributeError("[Labjack T7] The given channels must contain "
-                             "the 'name' key !")
+        raise AttributeError("The given channels must contain the 'name' "
+                             "key !")
 
       # Instantiating the channel and its attributes
       chan = _Channel(name=channel['name'])
       chan.update(channel)
       chan.write_at_open.append((f"{chan.name}_RANGE", chan.range))
       chan.address, _ = ljm.nameToAddress(chan.name)
 
@@ -179,15 +178,15 @@
     self._n_points = 0
     self._stream_t0 = 0
     self._stream_started = False
 
   def open(self) -> None:
     """Opens the Labjack, parses the commands to write at open, and sends them.
 
-    Also checks whether the scan rate chose nby the Labjack is the same as
+    Also checks whether the scan rate chosen by the Labjack is the same as
     requested by the user.
     """
 
     # Opening the Labjack
     self.log(logging.INFO, "Opening the connection to the Labjack")
     self._handle = ljm.openS(self._device, self._connection, self._identifier)
 
@@ -207,16 +206,16 @@
     scan_rate = ljm.eReadName(handle=self._handle, name="STREAM_SCANRATE_HZ")
     if scan_rate != self._scan_rate:
       self.log(logging.WARNING, f"Actual scan_rate: {scan_rate} instead of "
                                 f"requested {self._scan_rate}")
       self._scan_rate = scan_rate
 
   def make_zero(self, delay: float) -> None:
-    """Overriding of the method of the parent class, because the user can
-    choose which channels should be zeroed or not.
+    """Overriding the method of the parent class, because the user can choose
+    which channels should be zeroed or not.
 
     It simply performs the regular zeroing, and resets the compensation for the
     channels that shouldn't be zeroed.
     """
 
     # No need to acquire data if no channel should be zeroed
     if any(chan.make_zero for chan in self._channels):
@@ -228,27 +227,28 @@
       if self._compensations:
 
         # Resetting the compensation for channels that shouldn't be zeroed
         self._compensations = [comp if chan.make_zero else 0 for comp, chan
                                in zip(self._compensations, self._channels)]
 
   def start_stream(self) -> None:
-    """Starts the stream, and saves the timestamp chen the stream started."""
+    """Starts the stream, and saves the timestamp of the moment when the stream
+    started."""
 
     ljm.eStreamStart(handle=self._handle,
                      scansPerRead=self._scan_per_read,
                      numAddresses=len(self._channels),
                      aScanList=[chan.address for chan in self._channels],
                      scanRate=self._scan_rate)
     self._stream_t0 = time()
     self._stream_started = True
 
   def get_data(self) -> List[float]:
     """Reads single data points, applies the given gains and offsets, and
-    returns the data."""
+    returns the data along with a timestamp."""
 
     data = ljm.eReadNames(handle=self._handle,
                           numFrames=len(self._channels),
                           aNames=[chan.name for chan in self._channels])
 
     return [time()] + [val * chan.gain + chan.offset for chan, val
                        in zip(self._channels, data)]
@@ -273,18 +273,18 @@
     t = self._stream_t0 + np.arange(self._n_points, self._n_points +
                                     data.shape[0]) / self._scan_rate
     self._n_points += data.shape[0]
 
     return [t[:, np.newaxis], data]
 
   def stop_stream(self) -> None:
-    """Stops the stream if it was started."""
+    """Stops the stream, if it was started."""
 
     if self._stream_started:
       ljm.eStreamStop(self._handle)
 
   def close(self) -> None:
-    """Closes the Labjack if it was opened."""
+    """Closes the connection to the Labjack, if it was opened."""
 
     if self._handle is not None:
       self.log(logging.INFO, "Closing the connection to the Labjack")
       ljm.close(self._handle)
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/labjack_ue9.py` & `crappy-2.0.0.dev2/src/crappy/inout/labjack_ue9.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 from time import time
-from typing import Optional, List
+from typing import Optional, List, Iterable
 from dataclasses import dataclass
 import logging
 
 from .meta_inout import InOut
 from .._global import OptionalModule
 
 try:
@@ -23,60 +23,63 @@
   range_num: int = 12
   gain: float = 1
   offset: float = 0
   make_zero: bool = False
 
 
 class LabjackUE9(InOut):
-  """"""
+  """This class can read the analog input channels from a Labjack UE9 device.
+
+  It cannot read nor drive any of the other inout or output channels on the
+  UE9. The UE9 model has been discontinued, and replaced by the T7 model (see
+  :class:`~crappy.inout.LabjackT7`). It is thus likely that this class won't be
+  further improved in the future.
+  """
 
   def __init__(self,
-               channels: List[int],
-               gain: Optional[List[float]] = None,
-               offset: Optional[List[float]] = None,
-               make_zero: Optional[List[bool]] = None,
-               resolution: Optional[List[int]] = None) -> None:
-    """Sets the args and initializes the parent class.
+               channels: Iterable[int],
+               gain: Optional[Iterable[float]] = None,
+               offset: Optional[Iterable[float]] = None,
+               make_zero: Optional[Iterable[bool]] = None,
+               resolution: Optional[Iterable[int]] = None) -> None:
+    """Sets the arguments and initializes the parent class.
 
     Args:
-      channels: A :obj:`list` containing all the channels to read, given as
-        :obj:`int`. Only the `AIN` channels can be read by this class, so to
-        read the channel `AIN2` the integer `2` should be added to the list.
-      gain: A :obj:`list` containing for each channel the gain to apply to the
-        measured voltage, as a :obj:`float`. The returned voltage is
-        calculated as follows :
-        ::
-
-          returned_voltage = gain * measured_voltage + offset
-
-        If not given, no gain is applied to the measured values.
-      offset: A :obj:`list` containing for each channel the offset to apply to
-        the measured voltage, as a :obj:`float`. The returned voltage is
-        calculated as follows :
-        ::
-
-          returned_voltage = gain * measured_voltage + offset
-
-        If not given, no offset is applied to the measured values.
-      make_zero: A :obj:`list` containing for each channel a :obj:`bool`
-        indicating whether the channel should be zeroed or not. If so, data
-        will be acquired on this channel before the test starts, and a
-        compensation value will be deduced so that the offset of this channel
-        is `0`. **It will only take effect if the ``make_zero_delay`` argument
-        of the :ref:`IOBlock` controlling the Labjack is set** ! If not given,
-        the channels are by default not zeroed.
-      resolution: A :obj:`list` containing for each channel the resolution of
-        the acquisition as an integer. Refer to Labjack documentation for more
-        details. The higher this value the better the resolution, but the lower
-        the speed. The possible range is `1` to `12`, and the default is `12`.
+      channels: An iterable (like a :obj:`list` or a :obj:`tuple`) containing
+        all the channels to read, given as :obj:`int`. Only the `AIN` channels
+        can be read by this class, so to read the channel `AIN2` the integer
+        `2` should be added to the iterable.
+      gain: An iterable (like a :obj:`list` or a :obj:`tuple`) containing for
+        each channel the gain to apply to the measured voltage, as a
+        :obj:`float`. The returned voltage is calculated as follows :
+        :math:`returned\_voltage = gain * measured\_voltage + offset`. If not
+        given, no gain is applied to the measured values.
+      offset: An iterable (like a :obj:`list` or a :obj:`tuple`) containing for
+        each channel the offset to apply to the measured voltage, as a
+        :obj:`float`. The returned voltage is calculated as follows :
+        :math:`returned\_voltage = gain * measured\_voltage + offset`. If not
+        given, no offset is applied to the measured values.
+      make_zero: An iterable (like a :obj:`list` or a :obj:`tuple`) containing
+        for each channel a :obj:`bool` indicating whether the channel should be
+        zeroed or not. If so, data will be acquired on this channel before the
+        test starts, and a compensation value will be deduced so that the
+        offset of this channel is `0`. **It will only take effect if the**
+        ``make_zero_delay`` **argument of the** :class:`~crappy.blocks.IOBlock`
+        **controlling the Labjack is set** ! If not given, the channels are by
+        default not zeroed.
+      resolution: An iterable (like a :obj:`list` or a :obj:`tuple`) containing
+        for each channel the resolution of the acquisition as an integer. Refer
+        to Labjack documentation for more details. The higher this value the
+        better the resolution, but the lower the speed. The possible range is
+        `1` to `12`, and the default is `12`.
 
     Note:
-      All the :obj:`list` given as arguments for the channels should have the
-      same length. If that's not the case, all the given lists are treated as
-      if they had the same length as the shortest given list.
+      All the :iterables given as arguments for the channels should have the
+      same length. If that's not the case, all the given iterables are treated
+      as if they had the same length as the shortest given one.
     """
 
     self._handle = None
 
     super().__init__()
 
     # Setting the defaults for arguments that are not given
@@ -92,22 +95,22 @@
     self._channels = [_Channel(num=chan, range_num=r_num, gain=g,
                                offset=off, make_zero=make_z)
                       for chan, r_num, g, off, make_z in
                       zip(channels, resolution, gain, offset, make_zero)]
     self.log(logging.DEBUG, f"Input channels: {self._channels}")
 
   def open(self) -> None:
-    """Simply opens the connection to the Labjack."""
+    """Opens the connection to the Labjack."""
 
     self.log(logging.INFO, "Opening the connection to the Labjack")
     self._handle = UE9()
 
   def make_zero(self, delay: float) -> None:
-    """Overriding of the method of the parent class, because the user can
-    choose which channels should be zeroed or not.
+    """Overriding the method of the parent class, because the user can choose
+    which channels should be zeroed or not.
 
     It simply performs the regular zeroing, and resets the compensation to
     zero for the channels that shouldn't be zeroed.
     """
 
     # No need to acquire data if no channel should be zeroed
     if any(chan.make_zero for chan in self._channels):
@@ -118,19 +121,19 @@
       # Proceed only if the acquisition went fine
       if self._compensations:
         # Resetting the compensation for channels that shouldn't be zeroed
         self._compensations = [comp if chan.make_zero else 0 for comp, chan
                                in zip(self._compensations, self._channels)]
 
   def get_data(self) -> List[float]:
-    """Simply reads sequentially the channels and returns the acquired values,
+    """Reads sequentially the channels and returns the acquired values,
     corrected by the given gains and offsets."""
 
     return [time()] + [self._handle.getAIN(chan.num, Resolution=chan.range_num)
                        * chan.gain + chan.offset for chan in self._channels]
 
   def close(self) -> None:
-    """Closes the Labjack if it was already opened."""
+    """Closes the connection to the Labjack, if it was already opened."""
 
     if self._handle is not None:
       self.log(logging.INFO, "Closing the connection to the Labjack")
       self._handle.close()
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/mcp9600.py` & `crappy-2.0.0.dev2/src/crappy/inout/mcp9600.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,92 +86,92 @@
                  'Cold Junction Temperature',
                  'Raw Data ADC']
 
 Mcp9600_backends = ['Pi4', 'blinka']
 
 
 class MCP9600(InOut):
-  """Class for controlling Adafruit's MCP9600 thermocouple reader.
+  """This class can read temperature values from an MCP9600 thermocouple
+  reader.
 
-  The MCP9600 InOut block is meant for reading temperature from an MCP9600
-  board, using the I2C protocol. The output is in `°C`, except for one
-  operating mode that returns Volts.
+  It communicates over the I2C protocol. The output is in `°C`, except for one
+  operating mode that returns Volts. Several parameters can be tuned, like the
+  thermocouple type, the reading resolution or the filter coefficient. Note
+  that the MCP9600 can only achieve a data rate of a few Hz.
   """
 
   def __init__(self,
                backend: str,
                thermocouple_type: str,
                i2c_port: int = 1,
                device_address: int = 0x67,
                adc_resolution: int = 18,
                sensor_resolution: float = 0.0625,
                filter_coefficient: int = 0,
                mode: str = 'Hot Junction Temperature') -> None:
-    """Checks arguments validity.
+    """Checks the validity of the arguments.
 
     Args:
-      backend (:obj:`str`): The backend for communicating with the MCP9600.
+      backend: The backend for communicating with the MCP9600.
         Should be one of:
         ::
 
-          'Pi4', 'ft232h', 'blinka'
+          'Pi4', 'blinka'
 
         The `'Pi4'` backend is optimized but only works on boards supporting
         the :mod:`smbus2` module, like the Raspberry Pis. The `'blinka'`
-        backend may be less performant and requires installing Adafruit's
-        modules, but these modules are compatible with and maintained on a wide
-        variety of boards. The `'ft232h'` backend allows controlling the
-        ADS1115 from a PC using Adafruit's FT232H USB to I2C adapter. See
-        :ref:`Crappy for embedded hardware` for details.
-      thermocouple_type (:obj:`str`): The type of thermocouple plugged in the
-        MCP9600. The available types are:
+        backend may be less performant and requires installing
+        :mod:`Adafruit-Blinka`, :mod:`adafruit-circuitpython-busdevice` and
+        :mod:`adafruit-circuitpython-mcp9600`, but these modules are compatible
+        with and maintained on a wide variety of boards.
+      thermocouple_type: The type of thermocouple connected to the MCP9600. The
+        possible types are:
         ::
 
           'J', 'K', 'T', 'N', 'S', 'E', 'B', 'R'
 
-      i2c_port(:obj:`int`, optional): The I2C port over which the MCP9600
-        should communicate. On most Raspberry Pi models the default I2C port is
-        `1`.
-      device_address(:obj:`int`, optional): The I2C address of the MCP9600. The
-        default address is `0x67`, but it is possible to change this setting
-        using a specific setup involving the `ADDR` pin.
-      adc_resolution(:obj:`int`, optional): The number of bits the ADC output
-        is encoded on. The greater the resolution, the lower the sample rate.
-        The available resolutions are:
+      i2c_port: The I2C port over which the MCP9600 should communicate. On most
+        Raspberry Pi models the default I2C port is `1`.
+      device_address: The I2C address of the MCP9600. The default address is
+        `0x67`, but it is possible to change this setting using a specific
+        setup involving the `ADDR` pin.
+      adc_resolution: The number of bits the ADC output is encoded on. The
+        greater the resolution, the lower the sample rate. The available
+        resolutions are:
         ::
 
           12, 14, 16, 18
 
-      sensor_resolution(:obj:`float`, optional): The temperature measurement
-        resolution in `°C`. It should be either `0.0625` or `0.25`. Setting the
-        resolution to `0.25` will increase the sample rate, but the output
-        temperature will be encoded on two bits less.
-      filter_coefficient(:obj:`int`, optional): The MCP9600 features an
-        integrated filter (see its documentation for the exact filter formula).
-        When set to `0`, the filter is inactive. It is maximal when set to `7`.
-        When active, the filter will prohibit fast temperature changes, thus
-        limiting noise and smoothening the signal.
-      mode(:obj:`str`, optional): Four different values can be accessed when
-        measuring a temperature: the temperature of the thermocouple (hot
-        junction temperature), the temperature of the MCP9600 board (cold
-        junction temperature), the temperature calculated from the ADC data and
-        thermocouple type but not yet cold junction-compensated (junction
-        temperature delta), and the raw ADC measurement of the voltage
-        difference in the thermocouple (raw data ADC, in Volts). The available
-        modes are thus:
+      sensor_resolution: The temperature measurement resolution in `°C`. It
+        should be either `0.0625` or `0.25`. Setting the resolution to `0.25`
+        will increase the sample rate, but the output temperature will be
+        encoded on two bits less.
+      filter_coefficient: The MCP9600 features an integrated filter (see its
+        documentation for the exact filter formula). When set to `0`, the
+        filter is inactive. It is maximal when set to `7`. When active, the
+        filter will prohibit fast temperature changes, thus limiting noise and
+        smoothening the signal.
+      mode: Four different values can be accessed when measuring a temperature:
+        the temperature of the thermocouple (hot junction temperature), the
+        temperature of the MCP9600 board (cold junction temperature), the
+        temperature calculated from the ADC data and thermocouple type but not
+        yet cold junction-compensated (junction temperature delta), and the raw
+        ADC measurement of the voltage difference in the thermocouple (raw data
+        ADC, in Volts). The available modes are thus:
         ::
 
           'Hot Junction Temperature',
           'Junction Temperature Delta',
           'Cold Junction Temperature',
           'Raw Data ADC'
 
     """
 
     self._bus = None
+    self._mcp = None
 
     if not isinstance(backend, str) or backend not in Mcp9600_backends:
       raise ValueError("backend should be in {}".format(Mcp9600_backends))
     self._backend = backend
 
     super().__init__()
 
@@ -214,15 +214,15 @@
     elif mode == 'Raw Data ADC' and backend == 'blinka':
       raise ValueError('The Raw Data ADC mode is not available using the '
                        'backend blinka.')
     else:
       self._mode = mode
 
   def open(self) -> None:
-    """Sets the I2C communication and device."""
+    """Initializes the I2C communication and the device."""
 
     if self._backend == 'blinka':
       self.log(logging.INFO, "Connecting the the MCP9600 with backend blinka")
       self._mcp = MCP9600Adafruit(self._i2c,
                                   address=self._device_address,
                                   tctype=self._thermocouple_type,
                                   tcfilter=self._filter_coefficient)
@@ -259,15 +259,15 @@
   def get_data(self) -> List[float]:
     """Reads the registers containing the conversion result.
 
     The output is in `°C` for all modes except the raw data ADC one, which
     outputs Volts.
 
     Returns:
-      :obj:`list`: A list containing the timeframe and the output value
+      A :obj:`list`: containing the timestamp and the output value.
     """
 
     if self._backend == 'blinka':
       out = [time()]
       if self._mode == 'Hot Junction Temperature':
         out.append(self._mcp.temperature)
       elif self._mode == 'Junction Temperature Delta':
@@ -331,15 +331,15 @@
           value_raw -= 2 ** 18
 
         out.append(value_raw * 2E-6)
 
     return out
 
   def close(self) -> None:
-    """Switches the MCP9600 to shut down mode and closes the I2C bus.."""
+    """Switches the MCP9600 to shutdown mode and closes the I2C bus."""
 
     if self._backend != 'blinka' and self._bus is not None:
       # Switching to shut down mode, keeping configuration
       value = self._bus.read_i2c_block_data(self._device_address,
                                             Mcp9600_registers[
                                              'Device Configuration'], 1)[0]
       self.log(logging.DEBUG, f"Read {value} from register "
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/meta_inout/inout.py` & `crappy-2.0.0.dev2/src/crappy/blocks/generator_path/meta_path/path.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,233 +1,194 @@
 # coding: utf-8
 
 from time import time, sleep
-from typing import Optional, Dict, Any, Union, List
-import numpy as np
+from typing import Callable, Union, Dict, Optional
+from re import split, IGNORECASE, match
 import logging
 from multiprocessing import current_process
 
-from .meta_inout import MetaIO
+from .meta_path import MetaPath
 
+ConditionType = Callable[[Dict[str, list]], bool]
 
-class InOut(metaclass=MetaIO):
-  """Base class for all InOut objects. Implements methods shared by all the
-  these objects, and ensures their dataclass is MetaIO."""
 
-  ft232h: bool = False
+class Path(metaclass=MetaPath):
+  """Base class for all the Generator Path objects.
 
-  def __init__(self, *_, **__) -> None:
-    """Sets the attributes."""
+  The Path object are used by the :class:`~crappy.blocks.Generator` Block to
+  generate signals.
+  """
 
-    self._compensations = list()
-    self._logger: Optional[logging.Logger] = None
+  def __init__(self,
+               _last_time: float,
+               _last_cmd: Optional[float] = None,
+               *_,
+               **__) -> None:
+    """Here, the arguments given to the Path should be handled.
 
-  def log(self, level: int, msg: str) -> None:
-    """"""
+    If the Path accepts one or more conditions, (e.g. stop conditions for
+    switching to the next
+    :class:`~crappy.blocks.generator_path.meta_path.Path`), they can be parsed
+    here using the :meth:`parse_condition` method. See the code of
+    :class:`~crappy.blocks.generator_path.Constant` for an example.
 
-    if self._logger is None:
-      self._logger = logging.getLogger(
-        f"{current_process().name}.{type(self).__name__}")
+    The ``self.t0`` attribute stores the time when the last command of the
+    previous :class:`~crappy.blocks.generator_path.meta_path.Path` was sent,
+    and the ``self.last_cmd`` stores the value of the last command of the
+    previous :class:`~crappy.blocks.generator_path.meta_path.Path`.
+    """
 
-    self._logger.log(level, msg)
+    self.t0 = _last_time
+    self.last_cmd = _last_cmd if _last_cmd is not None else 0
+    self._logger: Optional[logging.Logger] = None
 
-  def open(self) -> None:
-    """This method should perform any action that's required for initializing
-    the hardware and the communication with it.
-
-    Communication with hardware should be avoided in the :meth:`__init__`
-    method, and this method is where it should start happening. This method is
-    called after Crappy's processes start, i.e. when the associated IOBlock
-    already runs separately from all the other blocks.
-    """
+  def get_cmd(self, data: Dict[str, list]) -> float:
+    """This method is called by the :class:`~crappy.blocks.Generator` Block to
+    get the next command to send.
+
+    It takes as input a :obj:`dict` containing the data received by the
+    Generator Block since the last command was sent. Refer to
+    :meth:`~crappy.blocks.Block.recv_all_data` for more information on the
+    format of this dict.
+
+    This method should output the next command that will be sent by the
+    Generator Block, as a numeric value. This value can be calculated based on
+    one or several of :
+
+    * the input data (see the code of 
+      :class:`~crappy.blocks.generator_path.Conditional`)
+    * the current time and the ``self.t0`` attribute (see the code of
+      :class:`~crappy.blocks.generator_path.Ramp`)
+    * the last sent value, using the ``self.last_cmd`` attribute 
+    * any other criteria
+
+    Alternatively, if the :class:`~crappy.blocks.generator_path.meta_path.Path`
+    is done and should hand over to the next one, it must raise a
+    :exc:`StopIteration` exception. Again, the choice to raise that exception
+    can be motivated by the current time, a condition as generated by
+    :meth:`parse_condition`, or any other criteria.
+    """
+
+    self.log(logging.WARNING, "The get_cmd was called but is not defined ! "
+                              "Please define a get_cmd method for your "
+                              "Generator path ! Returning the last sent "
+                              "command")
+    sleep(1)
+    return self.last_cmd
 
-    ...
+  def log(self, level: int, msg: str) -> None:
+    """Records log messages for the Path.
 
-  def get_data(self) -> Optional[Union[list, Dict[str, Any]]]:
-    """This method should acquire data from a device and return it in a
-    :obj:`list` along with a timestamp.
-
-    The timestamp must always be the first returned value, and there can be any
-    number of other acquired channels. The same number of values should always
-    be returned, and they should be in the same order.
-
-    Alternatively, the values can be returned in a :obj:`dict`. In that case,
-    the ``labels`` argument of the IOBlock is ignored and the returned labels
-    correspond to the keys of the dict.
+    Also instantiates the :obj:`~logging.Logger` when logging the first
+    message.
 
-    It is alright for this method to return :obj:`None` if there's no data to
-    acquire.
+    Args:
+      level: An :obj:`int` indicating the logging level of the message.
+      msg: The message to log, as a :obj:`str`.
     """
 
-    self.log(logging.WARNING,
-             "The get_data method was called but is not defined !\n To get "
-             "rid of this warning, define a get_data method, or remove all "
-             "the downstream links and make sure the make_zero_delay argument "
-             "of the IOBlock is set to None")
-    sleep(1)
-    return
-
-  def set_cmd(self, *cmd) -> None:
-    """This method should handle commands received from the upstream blocks.
+    if self._logger is None:
+      self._logger = logging.getLogger(
+        f"{current_process().name}.{type(self).__name__}")
 
-    Usually the command is meant to be set on a device, but any other behavior
-    is possible. The commands will be passed to this method as `args` (not
-    `kwargs`), in the same order as the ``cmd_labels`` are given in the
-    IOBlock.
-
-    If the expected number of commands is always the same, you can simply put
-    as many `args` to your ``set_cmd`` method as there are commands. For
-    example for three commands:
-    ::
+    self._logger.log(level, msg)
 
-      def set_cmd(self, cmd0, cmd1, cmd2):
-        ...
+  def parse_condition(self,
+                      condition: Optional[Union[str, ConditionType]]
+                      ) -> ConditionType:
+    """This method returns a function allowing to check whether a given 
+    condition is met or not.
+    
+    This returned function takes as an input a :obj:`dict` containing the data
+    received by the :class:`~crappy.blocks.Generator` Block since it sent the
+    last command. See :meth:`~crappy.blocks.Block.recv_all_data` for
+    information on the structure of this data. Based on the input data, it
+    returns :obj:`True` if the condition is met, and :obj:`False` otherwise.
+    
+    The condition can be given already as a function (or a callable), as 
+    :obj:`None` or more conveniently as a :obj:`str` to parse. If it is given 
+    as a function / callable, this callable is directly returned. If it is
+    given as :obj:`None`, a function always returning :obj:`False` is returned.
 
-    Alternatively, or if the number of commands may vary from one test to
-    another, you can get all the commands at once in a :obj:`tuple` by putting
-    a single unpacking argument. Example:
+    If the condition is given as a string, the supported condition types are :
     ::
 
-      def set_cmd(self, *cmds):
-        number_of_commands = len(cmds)
-        cmd0 = cmds[0]
-        ...
-
-    """
-
-    self.log(logging.WARNING,
-             "The set_cmd method was called but is not defined ! The data "
-             "received from the incoming links is discarded")
-    sleep(1)
-    return
+      '<var> > <threshold>'
+      '<var> < <threshold>'
+      'delay = <your_delay>'
 
-  def start_stream(self) -> None:
-    """This method should start the acquisition of the stream."""
+    With ``<var>``, ``<threshold>`` and ``<your_delay>`` to be replaced
+    respectively with the label on which the condition applies, the threshold
+    for the condition to become :obj:`True`, and the delay before switching to
+    the next :class:`~crappy.blocks.generator_path.meta_path.Path`.
 
-    self.log(logging.WARNING, "The start_stream method was called but is not "
-                              "defined !")
+    In the case when a :obj:`str` to parse is given as the condition, a
+    function performing the check is generated and returned. This way, the user
+    doesn't have to understand the internals of data transfers in Crappy to
+    handle custom conditions.
+    """
 
-  def get_stream(self) -> Optional[List[np.ndarray]]:
-    """This method should acquire a stream as a numpy array, and return it in a
-    :obj:`list` along with an array carrying the timestamps.
+    if not isinstance(condition, str):
+      # First case, the condition is None
+      if condition is None:
+        self.log(logging.DEBUG, "Condition is None")
 
-    The time array must be the first element of the list, the stream array the
-    second element. The time array should have only one column, the stream
-    array can have any number of columns representing the different channels
-    acquired.
+        def cond(_: Dict[str, list]) -> bool:
+          """Condition always returning False."""
 
-    It is also possible to return the two arrays in a :obj:`dict`, in which
-    case the ``labels`` argument is ignored and the keys of the dict set the
-    returned labels.
+          return False
 
-    It is alright for this method to return :obj:`None` if there's no data to
-    acquire.
-    """
+        return cond
+      # Second case, the condition is already a Callable
+      elif isinstance(condition, Callable):
+        self.log(logging.DEBUG, "Condition is a callable")
+        return condition
 
-    self.log(logging.WARNING, "The get_stream method was called but is not "
-                              "defined ! No data sent to downstream links")
-    sleep(1)
-    return
+    # Third case, the condition is a string containing '<'
+    if '<' in condition:
+      self.log(logging.DEBUG, "Condition is of type var < thresh")
+      var, thresh = split(r'\s*<\s*', condition)
 
-  def stop_stream(self) -> None:
-    """This method should stop the acquisition of the stream."""
+      # Return a function that checks if received data is inferior to threshold
+      def cond(data: Dict[str, list]) -> bool:
+        """Condition checking that the label values are below a given
+        threshold."""
 
-    self.log(logging.WARNING, "The stop_stream method was called but is not "
-                              "defined !")
+        if var in data:
+          return any((val < float(thresh) for val in data[var]))
+        return False
 
-  def close(self) -> None:
-    """This method should perform any action required for properly ending the
-    test and closing the communication with hardware.
-
-    It will be called when the associated IOBlock receives the order to stop,
-    either because the user hit CTRL+C, or because a Generator block reached
-    the end of its path, or because an exception was raised in any of the
-    blocks.
-    """
+      return cond
 
-    ...
+    # Fourth case, the condition is a string containing '>'
+    elif '>' in condition:
+      self.log(logging.DEBUG, "Condition is of type var > thresh")
+      var, thresh = split(r'\s*>\s*', condition)
 
-  def make_zero(self, delay: float) -> None:
-    """Acquires data for a given delay, averages it for each channel, and
-    stores the average.
+      # Return a function that checks if received data is superior to threshold
+      def cond(data: Dict[str, list]) -> bool:
+        """Condition checking that the label values are above a given
+        threshold."""
 
-    Does not work for pure streams, as it requires a :meth:`get_data` for
-    acquiring the data.
+        if var in data:
+          return any((val > float(thresh) for val in data[var]))
+        return False
 
-    The average values will then be used to remove the offset of the acquired
-    data during the test.
-    """
+      return cond
 
-    buf = []
-    t0 = time()
+    # Fifth case, it is a delay condition
+    elif match(r'delay', condition, IGNORECASE) is not None:
+      self.log(logging.DEBUG, "Condition is of type delay=xx")
+      delay = float(split(r'=\s*', condition)[1])
 
-    # Acquiring data for a given delay
-    while time() < t0 + delay:
-      data = self.get_data()
-      if data is not None and len(data) > 1:
-        buf.append(data[1:])
-
-    # If no data could be acquired, abort
-    if not buf:
-      self.log(logging.WARNING, "No data acquired when zeroing the channels, "
-                                "aborting the zeroing")
-      return
-
-    # Averaging the values and storing them
-    for values in zip(*buf):
-      try:
-        self._compensations.append(-sum(values) / len(values))
-      except TypeError:
-        # If something goes wrong, just forget about the offsetting
-        self._compensations = list()
-        self.log(logging.WARNING,
-                 "Cannot calculate the offset !\nPossible reasons are that the"
-                 " InOut doesn't return only numbers, or that it returns a "
-                 "dict instead of the expected list")
-        return
-
-  def return_data(self) -> Optional[Union[list, Dict[str, Any]]]:
-    """Returns the data from :meth:`get_data`, corrected by an offset if the
-    ``make_zero_delay`` argument of the IOBlock is set."""
-
-    data = self.get_data()
-
-    # If there's no offsetting, just return the data
-    if data is None or not self._compensations:
-      return data
-
-    # Otherwise, offset the acquired data except for time
-    elif len(data[1:]) == len(self._compensations):
-      try:
-        return [data[0]] + [val + comp for val, comp in
-                            zip(data[1:], self._compensations)]
-      # Shouldn't happen but doesn't harm to be careful
-      except TypeError:
-        return data
+      # Return a function that checks if the delay is expired
+      def cond(_: Dict[str, list]) -> bool:
+        """Condition checking if a given delay is expired."""
 
-    # Should also not happen
-    else:
-      raise ValueError("The number of offsets doesn't match the number of "
-                       "acquired values.")
+        return time() - self.t0 > delay
 
-  def return_stream(self) -> Optional[List[np.ndarray]]:
-    """Returns the data from :meth:`get_stream`, corrected by an offset if the
-    ``make_zero_delay`` argument of the IOBlock is set."""
-
-    data = self.get_stream()
-
-    # If there's no offsetting, just return the data
-    if data is None or not self._compensations:
-      return data
-
-    # Otherwise, offset the acquired data except for time
-    elif data[1].shape[1] == len(self._compensations):
-      try:
-        return [data[0], data[1] + self._compensations]
-      # Shouldn't happen but doesn't harm to be careful
-      except TypeError:
-        return data
+      return cond
 
-    # There's a problem with the shape of the output data
+    # Otherwise, it's an invalid syntax
     else:
-      raise ValueError("The number of offsets doesn't match the shape of the "
-                       "acquired array.")
+      raise ValueError("Wrong syntax for the condition, please refer to the "
+                       "documentation")
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/meta_inout/meta_inout.py` & `crappy-2.0.0.dev2/src/crappy/inout/meta_inout/meta_inout.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/mprls.py` & `crappy-2.0.0.dev2/src/crappy/inout/mprls.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,58 +36,56 @@
 mprls_status_bits = {'busy': 0x20,
                      'memory error': 0x04,
                      'math saturation': 0x01}
 mprls_backends = ['Pi4', 'blinka']
 
 
 class MPRLS(InOut):
-  """The MPRLS inout is meant for reading pressure from Adafruit's MPRLS
-    pressure sensor.
+  """This class can read values from an MPRLS pressure sensor.
 
-    It communicates over I2C with the sensor.
-    """
+  It communicates over I2C with the sensor.
+  """
 
   def __init__(self,
                backend: str,
                eoc_pin: Optional[Union[str, int]] = None,
                device_address: int = 0x18,
                i2c_port: int = 1) -> None:
     """Initializes the parent class and opens the I2C bus.
 
     Args:
-      backend (:obj:`str`): Should be one of :
+      backend: Should be one of :
         ::
 
-          'Pi4', 'blinka', 'ft232h'
+          'Pi4', 'blinka'
 
         The `'Pi4'` backend is optimized but only works on boards supporting
         the :mod:`smbus2` module, like the Raspberry Pis. The `'blinka'`
-        backend may be less performant and requires installing Adafruit's
-        modules, but these modules are compatible with and maintained on a wide
-        variety of boards. The `'ft232h'` backend allows controlling the
-        MPRLS from a PC using Adafruit's FT232H USB to I2C adapter. See
-        :ref:`Crappy for embedded hardware` for details.
-      eoc_pin (:obj:`int` or :obj:`str`, optional): Optionally, reads the end
-        of conversion signal from a GPIO rather than from an I2C message.
-        Speeds up the reading and decreases the traffic on the bus, but
-        requires one extra wire. With the backend `'Pi4'`, give the index of
-        the GPIO in BCM convention. With the `'ft232h'` backend, give the name
-        of the GPIO in the format `Dx` or `Cx`. With the backend `'blinka'`,
-        it should be a string but the syntax varies according to the board.
-        Refer to blinka's documentation for more information.
-      device_address (:obj:`int`, optional): The I2C address of the MPRLS.
-        The address of the devices sold by Adafruit is `0x18`, but other
-        suppliers may sell it with another address.
-      i2c_port (:obj:`int`, optional): The I2C port over which the MPRLS
-        should communicate. On most Raspberry Pi models the default I2C port is
-        `1`.
+        backend may be less performant and requires installing
+        :mod:`Adafruit-Blinka` and :mod:`adafruit-circuitpython-mprls`, but
+        these modules are compatible with and maintained on a wide
+        variety of boards.
+      eoc_pin: Optionally, reads the end of conversion signal from the polarity
+        of a GPIO rather than from an I2C register. Speeds up the reading and
+        decreases the traffic on the bus, but requires one extra wire. With the
+        backend `'Pi4'`, give the index of the GPIO in BCM convention. With the
+        backend `'blinka'`, it should be a string but the syntax varies
+        according to the board. Refer to blinka's documentation for more
+        information.
+      device_address: The I2C address of the MPRLS. The address of the devices
+        sold by Adafruit is `0x18`, but other suppliers may sell it with
+        another address.
+      i2c_port: The I2C port over which the MPRLS should communicate. On most
+        Raspberry Pi models the default I2C port is `1`.
     """
 
     self._bus = None
     self._eoc_pin = None
+    self._mpr = None
+    self._i2c_msg = None
 
     if not isinstance(backend, str) or backend not in mprls_backends:
       raise ValueError("backend should be in {}".format(mprls_backends))
     self._backend = backend
 
     super().__init__()
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/nau7802.py` & `crappy-2.0.0.dev2/src/crappy/inout/nau7802.py`

 * *Files 10% similar despite different names*

```diff
@@ -101,70 +101,60 @@
                       'CAL_IN_PROGRESS': 1,
                       'CAL_FAILURE': 2}
 
 NAU7802_VREF = 3.3
 
 
 class NAU7802(InOut):
-  """Class for controlling Sparkfun's NAU7802 load cell conditioner.
+  """This class can read values from a NAU7802 load cell conditioner.
 
-  The NAU7802 InOut block is meant for reading output values from a NAU7802
-  load cell conditioner, using the I2C protocol. The output is in Volts by
-  default, but can be converted to Newtons using ``gain`` and ``offset``.
+  This load cell conditioner is a low-cost 24-bits, single-channel conditioner,
+  that can read up to 320 samples per second. It communicates over the I2C
+  protocol. The returned value of the InOut is in Volts by default, but can be
+  converted to Newtons using the ``gain`` and ``offset`` arguments.
   """
 
   def __init__(self,
                i2c_port: int = 1,
                device_address: int = 0x2A,
                gain_hardware: int = 128,
                sample_rate: int = 80,
                int_pin: Optional[int] = None,
                gain: float = 1,
                offset: float = 0) -> None:
-    """Checks the validity of the arguments..
+    """Checks the validity of the arguments.
 
     Args:
-      i2c_port (:obj:`int`, optional): The I2C port over which the NAU7802
-        should communicate. On most Raspberry Pi models the default I2C port is
-        `1`.
-      device_address (:obj:`int`, optional): The I2C address of the NAU7802. It
-        is impossible to change this address, so it is not possible to have
-        several NAU7802 on the same i2c bus.
-      gain_hardware (:obj:`int`, optional): The gain to be used by the
-        programmable gain amplifier. Setting a high gain allows reading small
-        voltages with a better precision, but it might saturate the sensor for
-        higher voltages. Available gains are:
+      i2c_port: The I2C port over which the NAU7802 should communicate. On most
+        Raspberry Pi models the default I2C port is `1`.
+      device_address: The I2C address of the NAU7802. It is impossible to
+        change this address, so it is not possible to have several NAU7802
+        connected on the same I2C bus.
+      gain_hardware: The gain to be used by the programmable gain amplifier.
+        Setting a high gain allows reading small voltages with a better
+        precision, but it might saturate the sensor for higher voltages.
+        Available gains are:
         ::
 
           1, 2, 4, 8, 16, 32, 64, 128
 
-      sample_rate (:obj:`int`, optional): The sample rate for data conversion.
-        The higher the rate, the greater the noise. Available sample rates are:
+      sample_rate: The sample rate for data conversion. The higher the rate,
+        the greater the noise. Available sample rates are:
         ::
 
           10, 20, 40, 80, 320
 
-      int_pin (:obj:`int` or :obj:`str`, optional): Optionally, reads the end
-        of conversion signal from a GPIO rather than from an I2C message.
-        Speeds up the reading and decreases the traffic on the bus, but
-        requires one extra wire. With the backend `'Pi4'`, give the index of
-        the GPIO in BCM convention. With the `'ft232h'` backend, give the name
-        of the GPIO in the format `Dx` or `Cx`.
-      gain (:obj:`float`, optional): Allows to tune the output value according
-        to the formula:
-        ::
-
-          output = gain * tension + offset.
-
-      offset (:obj:`float`, optional): Allows to tune the output value
-        according to the formula:
-        ::
-
-          output = gain * tension + offset.
-
+      int_pin: Optionally, reads the end of conversion signal from the polarity
+        of a GPIO rather than from an I2C register. Speeds up the reading and
+        decreases the traffic on the bus, but requires one extra wire. Give the
+        index of the GPIO in BCM convention, as an :obj:`int`.
+      gain: Allows to tune the output value according to the formula :
+        :math:`output = gain * tension + offset`.
+      offset: Allows to tune the output value according to the formula :
+        :math:`output = gain * tension + offset`.
     """
 
     self._bus = None
     self._int_pin = None
 
     super().__init__()
 
@@ -186,17 +176,18 @@
 
     if int_pin is not None and not isinstance(int_pin, int):
       raise TypeError('int_pin should be an int !')
     self._int_pin = int_pin
 
     self._gain = gain
     self._offset = offset
+    self._retries = 5
 
   def open(self) -> None:
-    """Sets the I2C communication and device."""
+    """Initializes the I2C communication and the device."""
 
     if not self._is_connected():
       raise IOError("The NAU7802 is not connected")
 
     self.log(logging.INFO, "Setting up the NAU7802")
 
     # Resetting the device
@@ -257,29 +248,41 @@
   def get_data(self) -> List[float]:
     """Reads the registers containing the conversion result.
 
     The output is in Volts by default, and can be converted to Newtons using
     gain and offset.
 
     Returns:
-      :obj:`list`: A list containing the timeframe and the output value
+      A :obj:`list` containing the timeframe and the output value.
     """
 
     # Waiting for data to be ready
     t0 = time()
     while not self._data_available():
       if time() - t0 > 0.5:
         raise TimeoutError('Waited too long for data to be ready !')
 
     out = [time()]
 
-    # Reading the output data
-    block = self._bus.read_i2c_block_data(self._device_address,
-                                          NAU7802_Scale_Registers['ADCO_B2'],
-                                          3)
+    # Reading the output data, and handling I2C errors
+    i = 0
+    block = None
+    while i < self._retries:
+      try:
+        block = self._bus.read_i2c_block_data(
+            self._device_address, NAU7802_Scale_Registers['ADCO_B2'], 3)
+        break
+      # If an I2C error is caught, retrying to get the value or raising
+      except OSError:
+        if i == self._retries:
+          self.log(logging.ERROR, "Retries count exhausted !")
+          raise
+        i += 1
+        continue
+
     self.log(logging.DEBUG,
              f"Read {block} from register {NAU7802_Scale_Registers['ADCO_B2']}"
              f" at address {self._device_address}")
     value_raw = (block[0] << 16) | (block[1] << 8) | block[2]
 
     # Converting raw data into Volts or Newtons
     if block[0] >> 7:
@@ -306,15 +309,15 @@
       self.log(logging.INFO, "Cleaning up the GPIOs")
       GPIO.cleanup()
 
   def _is_connected(self) -> bool:
     """Tries reading a byte from the device.
 
     Returns:
-      :obj:`bool`: :obj:`True` if reading was successful, else :obj:`False`
+      :obj:`True` if reading was successful, else :obj:`False`
     """
 
     try:
       self._bus.read_byte(self._device_address)
       return True
     except IOError:
       return False
@@ -332,17 +335,17 @@
   def _set_bit(self,
                bit_number: int,
                register_address: int,
                bit: int) -> None:
     """Sets a given bit in the specified register.
 
     Args:
-      bit_number (:obj:`int`): Position of the bit in the register
-      register_address (:obj:`int`): Index of the register
-      bit (:obj:`int`): Value of the bit
+      bit_number: Position of the bit in the register, as an :obj:`int`.
+      register_address: Index of the register, as an :obj:`int`.
+      bit: Value of the bit, as an :obj:`int`.
     """
 
     value = self._bus.read_i2c_block_data(self._device_address,
                                           register_address, 1)[0]
     self.log(logging.DEBUG, f"Read {value} from register {register_address}"
                             f" at address {self._device_address}")
     if bit:
@@ -355,33 +358,33 @@
 
   def _get_bit(self,
                bit_number: int,
                register_address: int) -> bool:
     """Reads a given bit in the specified register.
 
     Args:
-      bit_number (:obj:`int`): Position of the bit in the register
-      register_address (:obj:`int`): Index of the register
+      bit_number: Position of the bit in the register, as an :obj:`int`.
+      register_address: Index of the register, as an :obj:`int`.
 
     Returns:
-      :obj:`bool`: True if the bit value is 1, else False
+      :obj:`True` if the bit value is 1, else :obj:`False`.
     """
 
     value = self._bus.read_i2c_block_data(self._device_address,
                                           register_address, 1)[0]
     self.log(logging.DEBUG, f"Read {value} from register {register_address}"
                             f" at address {self._device_address}")
     value = value >> bit_number & 1
     return bool(value)
 
   def _cal_afe_status(self) -> int:
     """Reads the calibration status bits.
 
     Returns:
-      :obj:`int`: The int value corresponding to the current calibration status
+      The :obj:`int` value corresponding to the current calibration status.
     """
 
     if self._get_bit(NAU7802_CTRL2_Bits['CTRL2_CAL_ERROR'],
                      NAU7802_Scale_Registers['CTRL2']):
       return NAU7802_Cal_Status['CAL_FAILURE']
     elif self._get_bit(NAU7802_CTRL2_Bits['CTRL2_CALS'],
                        NAU7802_Scale_Registers['CTRL2']):
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/ni_daqmx.py` & `crappy-2.0.0.dev2/src/crappy/inout/ni_daqmx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 from time import time
 import numpy as np
-from typing import List, Optional, Dict, Any
+from typing import List, Optional, Dict, Any, Iterable
 from dataclasses import dataclass, field
 from re import fullmatch
 from collections import defaultdict
 from itertools import chain
 import logging
 
 from .meta_inout import InOut
@@ -55,47 +55,51 @@
 
       # All the other keys are put together in the kwargs attribute
       else:
         self.kwargs.update({key: val})
 
 
 class NIDAQmx(InOut):
-  """This class can communicate with NI DAQmx devices using the :mod:`pydaqmx`
-  module.
+  """This class can drive data acquisition hardware from National Instruments.
+
+  It is similar to :class:`~crappy.inout.DAQmx` InOut, except it relies on the
+  :mod:`nidaqmx` module. It was written and tested on a USB 6008 DAQ board, but
+  should work with other instruments as well.
 
   It can read single data points from digital and analog channels, read streams
   of data from analog channels, and set the voltage of analog and digital
   output channels. For analog input channels, several types of acquisition can
   be performed, like voltage, resistance, current, etc.
   """
 
   def __init__(self,
-               channels: List[Dict[str, Any]],
+               channels: Iterable[Dict[str, Any]],
                sample_rate: float = 100,
                n_samples: Optional[int] = None) -> None:
-    """Sets the args and initializes the parent class.
+    """Sets the arguments and initializes the parent class.
 
     Args:
-      channels: A :obj:`list` containing :obj:`dict` holding information on the
-        channels to read data from or write data to. See below for the
-        mandatory and optional keys for the dicts. Note that in streamer mode,
-        the digital input channels are not available for reading. Also, only
-        one type of analog input channel at a time can be read in streamer
-        mode, with no restriction on the number of channels of this type.
+      channels: An iterable (like a :obj:`list` or a :obj:`tuple`) containing
+        :obj:`dict` holding information on the channels to read data from or
+        write data to. See below for the mandatory and optional keys for the
+        dicts. Note that in streamer mode, the digital input channels are not
+        available for reading. Also, only one type of analog input channel at a
+        time can be read in streamer mode, with no restriction on the number of
+        channels of this type.
       sample_rate: The target sample rate for data acquisition in streamer
         mode, given as a :obj:`float`. Default is `100` SPS.
       n_samples: The number of samples to acquire per chunk of data in streamer
         mode. Default is 20% of ``sample_rate``.
 
 
     Note:
       - ``channels`` keys:
 
-        - name: The name of the channel to interface with, given with the
-          following syntax :
+        - name: The name of the channel to drive, given with the following
+          syntax :
           ::
 
             'DevX/[a/d][i/o]Y'
 
           With `X` the index of the device, and `Y` the line on which the
           channel is. `d` stands for digital, `a` for analog, `i` for input and
           `o` for output. For digital channels, `DevX/d[i/o]Y` is internally
@@ -151,24 +155,24 @@
     # Here as well a dict is needed for handling each analog input type
     self._analog_in = defaultdict(list)
 
     for channel in channels:
 
       # Making sure each channel has a 'name' attribute
       if 'name' not in channel:
-        raise AttributeError("[NI DAQmx] The given channels must contain "
-                             "the 'name' key !")
+        raise AttributeError("The given channels must contain the 'name' "
+                             "key !")
 
       # Parsing the channel name to retrieve info from it
       match = fullmatch(r'(.+)/(.+)(\d+)', channel['name'])
       if match is not None:
         dev, type_, num = match.groups()
         num = int(num)
       else:
-        raise AttributeError(f"[NI DAQmx] Invalid format for the channel name "
+        raise AttributeError(f"Invalid format for the channel name "
                              f": {channel['name']} !\nIt should be "
                              f"'Dev<dev num>/[a/d][i/o]<chan num>'")
 
       # Creating a _Channel object holding the information on the channel
       chan = _Channel()
       chan.update(channel)
 
@@ -180,16 +184,16 @@
       elif type_ == 'di':
         chan.name = f"{dev}/port{num // 8}/line{num % 8}"
         self._digital_in.append(chan)
       elif type_ == 'do':
         chan.name = f"{dev}/port{num // 8}/line{num % 8}"
         self._digital_out.append(chan)
       else:
-        raise ValueError(f"[NI DAQmx] Wrong channel type : {type_} !\nIt "
-                         f"should be either 'ai', 'ao', 'di', or 'do'.")
+        raise ValueError(f"Wrong channel type : {type_} !\nIt should be "
+                         f"either 'ai', 'ao', 'di', or 'do'.")
 
   def open(self) -> None:
     """Creates tasks and streams for analog output, digital input, digital
     output, and each type of analog input channels."""
 
     # Creating one task for each type of analog input channel
     self._tasks_ai = {type_: nidaqmx.Task() for type_ in self._analog_in}
@@ -213,15 +217,15 @@
 
         # Adding the channel to the task with the given kwargs
         try:
           func = getattr(self._tasks_ai[type_].ai_channels,
                          f'add_ai_{type_}_chan')
           func(chan.name, **chan.kwargs)
         except AttributeError:
-          raise ValueError(f"[NI DAQmx] Invalid channel type : {type_}")
+          raise ValueError(f"Invalid channel type : {type_}")
 
     # Opening a stream for each analog input task
     self.log(logging.INFO, "Opening the streams for the analog input channels")
     self._stream_ai = {
       type_: stream_readers.AnalogMultiChannelReader(task.in_stream)
       for type_, task in self._tasks_ai.items()}
 
@@ -268,19 +272,17 @@
 
     Data can be acquired via streaming for multiple channels, but only for one
     type of channel.
     """
 
     # Making sure there's only one type of channel to read data from
     if len(self._tasks_ai) > 1:
-      raise IOError("[NI DAQmx] Stream mode can only open one type of "
-                    "channel !")
+      raise IOError("Stream mode can only open one type of channel !")
     elif len(self._tasks_ai) < 1:
-      raise IOError("[NI DAQmx] There's no analog in channel to read data "
-                    "from !")
+      raise IOError("There's no analog in channel to read data from !")
 
     # Starting the streaming task, there should be only one
     for task in self._tasks_ai.values():
       task.timing.cfg_samp_clk_timing(
         self._sample_rate,
         sample_mode=nidaqmx.constants.AcquisitionType.CONTINUOUS)
 
@@ -312,15 +314,15 @@
       self._stream_di.read_one_sample_multi_line(data)
 
       ret.extend(list(data[:, 0]))
 
     return ret
 
   def get_stream(self) -> Optional[List[np.ndarray]]:
-    """Reads data from the NI DAQmx, and returns it in an array along with an
+    """Reads data from the device, and returns it in an array along with an
     array holding the timestamps.
 
     Only data from analog input channels can be read, this method cannot read
     stream data from digital input channels.
     """
 
     if not self._stream_started:
@@ -338,15 +340,15 @@
     return [t, data]
 
   def set_cmd(self, *cmd: float) -> None:
     """Sets the analog and digital output channels according to the given
     command values.
 
     The first command values correspond to the analog channels, the remaining
-    ones correspond the the digital channels. It might be that not all channels
+    ones correspond to the digital channels. It might be that not all channels
     are set if the number of commands doesn't match the number of channels.
     """
 
     # Setting the analog channels
     if self._analog_out:
       self._stream_ao.write_one_sample(np.array(cmd[:len(self._analog_out)],
                                        dtype=np.float64))
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/opsens.py` & `crappy-2.0.0.dev2/src/crappy/modifier/integrate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,59 @@
 # coding: utf-8
 
-from time import time
-from typing import List
+from typing import Optional, Dict, Any
 import logging
 
-from .meta_inout import InOut
-from .._global import OptionalModule
+from .meta_modifier import Modifier
 
-try:
-  import serial
-except (ModuleNotFoundError, ImportError):
-  serial = OptionalModule("pyserial")
-
-
-class OpSens(InOut):
-  """This class allows reading data from an OpSens PicoSens fiber optics signal
-  conditioner.
-
-  It can read data from various fiber optics sensors like temperature,
-  pressure, position or strain.
-  """
+
+class Integrate(Modifier):
+  """This Modifier integrates the data of a label over time and adds the
+  integration value to the returned data."""
 
   def __init__(self,
-               device: str = '/dev/ttyUSB0') -> None:
-    """Sets the arg and initializes the parent class.
+               label: str,
+               time_label: str = 't(s)',
+               out_label: Optional[str] = None) -> None:
+    """Sets the args and initializes the parent class.
 
     Args:
-      device: Address of the serial connection for communicating with the
-        PicoSens.
+      label: The label whose data to integrate over time.
+      time_label: The label carrying the time information.
+      out_label: The label carrying the integration value. If not given,
+        defaults to ``'i_<label>'``.
     """
 
-    self._dev = None
-
     super().__init__()
-
-    self._addr = device
-
-  def open(self) -> None:
-    """Opens the serial connection and configures the PicoSens."""
-
-    self.log(logging.INFO, f"Opening the serial connection on port "
-                           f"{self._addr} with baudrate 57600")
-    self._dev = serial.Serial(port=self._addr, baudrate=57600, timeout=0.1)
-    self._send_cmd("meas:rate min")
-
-  def get_data(self) -> List[float]:
-    """Reads data from the PicoSens and returns it."""
-
-    return [time(), float(self._send_cmd("ch1:data? 1")[:-3])]
-
-  def close(self) -> None:
-    """Closes the serial connection if it was opened."""
-
-    if self._dev is not None:
-      self.log(logging.INFO, f"Closing the serial connection on port "
-                             f"{self._addr}")
-      self._dev.close()
-
-  def _send_cmd(self, cmd: str) -> str:
-    """Sends a command and returns the received answer."""
-
-    self.log(logging.DEBUG, f"Writing b'{cmd}\\n' to port {self._addr}")
-    self._dev.write(cmd + '\n')
-    ret = self._dev.read_until(b'\x04\n').decode()
-    self.log(logging.DEBUG, f"Read {ret} on port {self._addr}")
-    return ret
+    self._label = label
+    self._time_label = time_label
+    self._out_label = out_label if out_label is not None else f'i_{label}'
+
+    self._last_t = None
+    self._last_val = None
+    self._integration = 0
+
+  def __call__(self, data: Dict[str, Any]) -> Dict[str, Any]:
+    """Gets the data from the upstream Block, updates the integration value,
+    adds it to the data and returns the data."""
+
+    self.log(logging.DEBUG, f"Received {data}")
+
+    # For the first received data, storing it and returning 0
+    if self._last_t is None or self._last_val is None:
+      self._last_t = data[self._time_label]
+      self._last_val = data[self._label]
+      data[self._out_label] = self._integration
+      return data
+
+    # Updating the integrated value with the latest received values
+    t = data[self._time_label]
+    val = data[self._label]
+    self._integration += (t - self._last_t) * (val + self._last_val) / 2
+    # Updating the stored data
+    self._last_t = t
+    self._last_val = val
+
+    # Returning the updated data
+    data[self._out_label] = self._integration
+    self.log(logging.DEBUG, f"Sending {data}")
+    return data
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/pijuice_hat.py` & `crappy-2.0.0.dev2/src/crappy/inout/pijuice_hat.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,42 +40,41 @@
                         0x20: 'Weak',
                         0x30: 'Present'}
 
 pijuice_backends = ['Pi4', 'pijuice']
 
 
 class PiJuice(InOut):
-  """Block getting various information about a piJuice power platform,
+  """This class can read various information about a piJuice power platform,
   including the charge level and the power supply status.
 
   Warning:
     Only available on Raspberry Pi !
   """
 
   def __init__(self,
                i2c_port: int = 1,
                address: int = 0x14,
                backend: str = 'Pi4') -> None:
-    """Checks arguments validity.
+    """Checks the validity of the arguments.
 
     Args:
-      backend (:obj:`str`, optional): Should be one of :
+      backend: Should be one of :
         ::
 
           'Pi4', 'pijuice'
 
         The `'Pi4'` backend is based on the :mod:`smbus2` module, while the
-        `'pijuice'` backend is based on the :mod:`pijuice`.
-      i2c_port(:obj:`int`, optional): The I2C port over which the PiJuice
-        should communicate.
-      address(:obj:`int`, optional): The I2C address of the piJuice. The
-        default address is 0x14.
+        `'pijuice'` backend is based on the :mod:`pijuice` module.
+      i2c_port: The I2C port over which the PiJuice should communicate.
+      address: The I2C address of the piJuice. The default address is `0x14`.
     """
 
     self._bus = None
+    self._pijuice = None
 
     super().__init__()
     if not isinstance(i2c_port, int):
       raise TypeError("i2c_port should be an int")
     self._i2c_port = i2c_port
 
     if not isinstance(address, int):
@@ -99,29 +98,28 @@
                              f"port {self._i2c_port} with backend pijuice")
       self._pijuice = PiJuiceModule(self._i2c_port, self._address)
 
   def get_data(self) -> Dict[str, Any]:
     """Reads all the available information on the battery status.
 
     Returns:
-      :obj:`dict`: Returns a dict containing:
-
-        - the timeframe in seconds as a :obj:`float` in label ``t(s)``
-        - the battery status as a :obj:`str` in label ``battery_status``
-        - the USB status as a :obj:`str` in label ``USB_status``
-        - the GPIO status as a :obj:`str` in label ``GPIO_status``
-        - the charge level as an :obj:`int` in label ``charge_level``
-        - the battery temperature in °C as an :obj:`int` in label
+      Returns a :obj:`dict` containing
+        * the timestamp in seconds as a :obj:`float` in label ``t(s)``
+        * the battery status as a :obj:`str` in label ``battery_status``
+        * the USB status as a :obj:`str` in label ``USB_status``
+        * the GPIO status as a :obj:`str` in label ``GPIO_status``
+        * the charge level as an :obj:`int` in label ``charge_level``
+        * the battery temperature in °C as an :obj:`int` in label
           ``battery_temperature``
-        - the battery voltage in mV as an :obj:`int` in label
+        * the battery voltage in mV as an :obj:`int` in label
           ``battery_voltage``
-        - the battery current in mA as an :obj:`int` in label
+        * the battery current in mA as an :obj:`int` in label
           ``battery_current``
-        - the GPIO voltage in mV as an :obj:`int` in label ``GPIO_voltage``
-        - the GPIO current in mA as an :obj:`int` in label ``GPIO_current``
+        * the GPIO voltage in mV as an :obj:`int` in label ``GPIO_voltage``
+        * the GPIO current in mA as an :obj:`int` in label ``GPIO_current``
     """
 
     # Gets the battery status
     status = dict()
 
     if self._backend == 'Pi4':
       data = self._read_i2c(pijuice_commands['status'], 2)
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/spectrum.py` & `crappy-2.0.0.dev2/src/crappy/inout/spectrum_m2i4711.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,73 +1,74 @@
 # coding: utf-8
 
 import numpy as np
 from time import time
-from typing import List, Optional
+from typing import List, Optional, Iterable
 import logging
 
 from .meta_inout import InOut
 from ..tool.bindings import pyspcm as spc
 
 
-class Spectrum(InOut):
+class SpectrumM2I4711(InOut):
   """This class can read data from a Spectrum high speed ADC interfacing over
   PCIe.
 
   It can acquire data over multiple channels, and set for each channel a
   different voltage range. It is possible to tune the sample rate, the chunk
   size and the memory allocated to the data buffer.
 
   This class can only acquire data by streaming, it cannot acquire single data
   points.
   """
 
   def __init__(self,
-               channels: List[int],
+               channels: Iterable[int],
                device: str = '/dev/spcm0',
-               ranges: Optional[List[int]] = None,
+               ranges: Optional[Iterable[int]] = None,
                sample_rate: int = 100000,
                buff_size: int = 2**26,
                notify_size: int = 2**16) -> None:
-    """Sets the args and initializes the parent class.
+    """Sets the arguments and initializes the parent class.
 
     Args:
-      channels: A :obj:`list` of all the channels to read data from, given as
-        :obj:`int`. Refer to the documentation to know which combinations of
+      channels: An iterable (like a :obj:`list` or a :obj:`tuple`) of all the
+        channels to read data from, given as :obj:`int`. Refer to the
+        documentation of the Spectrum board to know which combinations of
         channels are allowed.
       device: The address of the device to read data from, as a :obj:`str`.
-      ranges: A :obj:`list` indicating for each channel the range of the
-        acquisition in mV, as an :obj:`int`. There should be as many values in
-        this list as there are channels. If not given, all ranges default to
-        `10000` mV.
+      ranges: An iterable (like a :obj:`list` or a :obj:`tuple`) indicating for
+        each channel the range of the acquisition in mV, as an :obj:`int`.
+        There should be as many values in this iterable as there are channels.
+        If not given, all ranges default to `10000` mV.
       sample_rate: The sample rate of the acquisition for all channels, in Hz.
         The default is 100KHz.
       buff_size: The size of the memory allocated as a rolling buffer to copy
         the data from the card, in bytes. The default is 67MB.
       notify_size: The size of each chunk of data to copy from the card, in
         bytes. The default is 65kB.
     """
 
     self._spectrum = None
 
     super().__init__()
 
     # Setting the args
-    self._channels = channels
+    self._channels = list(channels)
     self._device = device.encode()
     self._ranges = ranges if ranges is not None else [10000 for _ in channels]
     self._sample_rate = sample_rate
     self._buff_size = buff_size
     self._notify_size = notify_size
-    self._chunk_size = notify_size // (2 * len(channels))
+    self._chunk_size = notify_size // (2 * len(self._channels))
 
     self.log(logging.INFO,
-             f"Will send {2 * sample_rate * len(channels) / notify_size} "
-             f"chunks of {notify_size / 1024} kB per second "
-             f"({sample_rate * len(channels) / 512} kB/s)")
+             f"Will send {2 * sample_rate * len(self._channels) / notify_size}"
+             f" chunks of {notify_size / 1024} kB per second "
+             f"({sample_rate * len(self._channels) / 512} kB/s)")
 
     # These attributes will be set later
     self._dt = None
     self._buff = None
     self._stream_t0 = 0
     self._n_points = 0
     self._stream_started = False
@@ -146,12 +147,12 @@
     """Stops the stream, if it was started."""
 
     if self._stream_started:
       spc.dw_set_param(self._spectrum, spc.SPC_M2CMD, spc.M2CMD_CARD_STOP |
                        spc.M2CMD_DATA_STOPDMA)
 
   def close(self) -> None:
-    """Closes the connection to the Spectrum if it was opened."""
+    """Closes the connection to the Spectrum, if it was opened."""
 
     if self._spectrum is not None:
       self.log(logging.INFO, "closing the connection to the Spectrum")
       spc.vClose(self._spectrum)
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/waveshare_ad_da.py` & `crappy-2.0.0.dev2/src/crappy/inout/waveshare_ad_da.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 import time
 from time import sleep, time
 from re import fullmatch, findall
-from typing import Union, Optional, List
+from typing import Union, Optional, List, Iterable
 import logging
 
 from .meta_inout import InOut
 from .._global import OptionalModule
 
 try:
   import RPi.GPIO as GPIO
@@ -83,99 +83,89 @@
 AD_DA_pins = {'RST_PIN_ADS': 18,
               'CS_PIN_ADS': 22,
               'DRDY_PIN_ADS': 17,
               'CS_PIN_DAC': 23}
 
 
 class WaveshareADDA(InOut):
-  """Class for controlling Waveshare's AD/DA hat.
+  """Class for controlling Waveshare's AD/DA Raspberry Pi hat.
 
-  The WaveshareADDA InOut block is meant for communicating with Waveshare's
-  AD/DA Raspberry Pi hat, using the SPI protocol and the GPIOs. It allows to
-  read values from the 8-channels ADC and/or to set the 2-channels DAC.
-
-  Warning:
-    This class is specifically meant to be used on a Raspberry Pi. See
-    :ref:`Waveshare AD/DA FT232H` for use with FTDI's FT232H.
+  It communicates over the SPI protocol and the GPIOs. It allows to
+  read values from the 8-channels ADC and/or to set the 2-channels DAC. The hat
+  can acquire up to 30000 samples per second, although this data rate is
+  impossible to achieve using Crappy.
+
+  Important:
+    This class is specifically meant to be used on a Raspberry Pi.
   """
 
   def __init__(self,
-               dac_channels: Optional[List[str]] = None,
-               adc_channels: Optional[List[str]] = None,
+               dac_channels: Optional[Iterable[str]] = None,
+               adc_channels: Optional[Iterable[str]] = None,
                gain_hardware: int = 1,
                v_ref: float = 3.3,
                gain: float = 1,
                offset: float = 0,
                sample_rate: Union[int, float] = 100) -> None:
     """Checks the validity of the arguments.
 
     Args:
-      dac_channels (:obj:`list`, optional): A :obj:`list` of :obj:`str`
-        representing the channels to be set. The syntax for each string is
-        'DACi' with i being either `0` or `1`.
-      adc_channels (:obj:`list`, optional): A :obj:`list` of :obj:`str`
-        representing the channels to read. The syntax for all strings is
-        either:
+      dac_channels: An iterable (like a :obj:`list` or a :obj:`tuple`) of
+        :obj:`str` representing the channels to be set. The syntax for each
+        string is 'DACi' with i being either `0` or `1`.
+      adc_channels: An iterable (like a :obj:`list` or a :obj:`tuple`) of
+        :obj:`str` representing the channels to read. The syntax for all the
+        strings is either:
         ::
 
           'ADi' (i in range(8))
 
         or else:
         ::
 
           'ADi - ADj' (i, j in range(8))
 
-      gain_hardware (:obj:`int`, optional): The gain to be used by the
-        programmable gain amplifier. Setting a high gain allows to read small
-        voltages with a better precision, but it might saturate the sensor for
-        higher voltages. The available gain values are:
+      gain_hardware: The gain to be used by the programmable gain amplifier.
+        Setting a high gain allows to read small voltages with a better
+        precision, but it might saturate the sensor for higher voltages. The
+        available gain values are:
         ::
 
           1, 2, 4, 8, 16, 32, 64
 
-      v_ref (:obj:`float`, optional): The voltage reference set by the `VREF`
-        jumper. When reading single inputs, ``v_ref`` is the value the ADC
-        compares the signals with. In a similar way, the maximum output voltage
-        of the DAC is ``v_ref``. `3.3` and `5` are the only possible values for
-        this setting, as the Raspberry Pi can only provide `3.3V` and `5V`.
-      gain (:obj:`float`, optional): Allows to tune the output values of the
-        DAC according to the formula:
-        ::
-
-          output = gain * tension + offset.
-
-        The same gain applies to all the outputs.
-      offset (:obj:`float`, optional): Allows to tune the output values of the
-        ADC according to the formula:
-        ::
-
-          output = gain * tension + offset.
-
-        The same offset applies to all the outputs.
-      sample_rate (optional): The ADC data output rate in SPS. The available
-        values are:
+      v_ref: The voltage reference set by the `VREF` jumper. When reading
+        single inputs, ``v_ref`` is the value the ADC compares the signals
+        with. In a similar way, the maximum output voltage of the DAC is
+        ``v_ref``. `3.3` and `5` are the only possible values for this setting,
+        as the Raspberry Pi can only provide `3.3V` and `5V`.
+      gain: Allows to tune the output values of the ADC according to the
+        formula : :math:`output = gain * tension + offset`. The same gain
+        applies to all the outputs.
+      offset: Allows to tune the output values of the ADC according to the
+        formula : :math:`output = gain * tension + offset`. The same offset
+        applies to all the outputs.
+      sample_rate: The ADC data output rate in SPS. The available values are:
         ::
 
           2.5, 5, 10, 15, 25, 30, 50, 60, 100, 500,
           1000, 2000, 3750, 7500, 15000, 30000
 
     Warning:
       - ``adc_channels``:
         For reading single inputs the `JMP_AGND` jumper should normally be
         connected, whereas it should be disconnected for reading differential
         inputs. It is however possible to set a different reference than `AGND`
         for single input measurements, in which case the `JMP_AGND` jumper
         should not be connected and the voltage reference should be plugged
         in the `AINCOM` pin.
 
-        The AD/DA offers the possibility to read single inputs or
-        differential inputs, but not both at the same time ! This is due to
-        the `JMP_AGND` jumper.
-        For measuring both input types simultaneously, is it necessary to
-        connect `AGND` to one of the channels (for example `AD0`). Then all
+        The AD/DA offers the possibility to read single inputs or differential
+        inputs, but not both at the same time ! This is due to the `JMP_AGND`
+        jumper. For measuring both input types simultaneously, is it necessary
+        to connect `AGND` to one of the channels (for example `AD0`). Then all
         single inputs `'ADi'` should be replaced by `'ADi - AD0'`. They are
         then considered as differential inputs.
 
         The ADC channels voltages should not be lower than `AGND-0.1V`, and not
         be greater than `AGND+5.1V`. This is independent of `VREF` value.
 
     Note:
@@ -288,16 +278,16 @@
   def get_data(self) -> List[float]:
     """Reads data from all the user-specified ADC channels, in a sequential
     way.
 
     Data is returned in Volts, but this can be tuned using gain and offset.
 
     Returns:
-      :obj:`list`: A list containing the timeframe, and then the values for
-      each channel to read
+      A :obj:`list` containing the timestamp, and then the values for each
+      channel to read.
     """
 
     out = [time()]
 
     # The values are read one channel after the other, not simultaneously
     for chan in self._channels_read:
       GPIO.output(AD_DA_pins['CS_PIN_ADS'], GPIO.LOW)
@@ -337,15 +327,15 @@
 
     return out
 
   def set_cmd(self, *cmd: float) -> None:
     """Sets the user-specified DAC channels according to the input values.
 
     Args:
-      cmd (:obj:`float`): The input values, in Volts
+      cmd: The input values as :obj:`float`, in Volts.
     """
 
     # The values are set one channel after the other, not simultaneously
     for val, channel in zip(cmd, self._channels_write):
       if not 0 <= val <= self._v_ref:
         raise ValueError("Desired output voltage should be between 0 and "
                          "v_ref")
```

### Comparing `crappy-2.0.0.dev1/src/crappy/inout/waveshare_high_precision.py` & `crappy-2.0.0.dev2/src/crappy/inout/waveshare_high_precision.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding : utf-8
 
 from time import time, sleep
 from re import fullmatch, findall
-from typing import Union, List, Optional
+from typing import Union, List, Optional, Iterable
 import logging
 
 from .meta_inout import InOut
 from .._global import OptionalModule
 
 try:
   import RPi.GPIO as GPIO
@@ -115,19 +115,19 @@
   and the 3.3 and 5V power are supplied.
   """
 
   def __init__(self,
                spi_port: int = 0,
                gain_hardware: int = 16,
                sample_rate: Union[int, float] = 50,
-               channels: Optional[List[str]] = None,
+               channels: Optional[Iterable[str]] = None,
                digital_filter: int = 4,
                gain: float = 1,
                offset: float = 0) -> None:
-    """Sets the args and initializes the parent class.
+    """Sets the arguments and initializes the parent class.
 
     Args:
       spi_port: The SPI port for communicating with the Waveshare HAT.
       gain_hardware: A programmable gain for the signal. Should be one of :
         ::
 
           1, 2, 4, 8, 16, 32
@@ -143,16 +143,17 @@
           14400, 19200, 38400
 
         The actual achieved sample rate might be lower depending on the
         capability of the PC and the load on the processor. Note that the
         greater the sample rate, the greater the noise. For multiple channels,
         the achieved sample rate is roughly the target sample rate divided by
         the number of channels.
-      channels: A :obj:`list` containing strings representing the channels to
-        acquire. Each channel must follow on of the two syntax :
+      channels: An iterable (like a :obj:`list` or a :obj:`tuple`) containing
+        strings representing the channels to acquire. Each channel must follow
+        one of the two syntax :
         ::
 
           'INi', i in range(10)
 
         or else
         ::
 
@@ -164,27 +165,19 @@
         of the channels `i` and `j`. It is preferable to use the channels in
         pair (0 & 1, 2 & 3, etc.) for differential acquisition. The data from
         the different channels is acquired sequentially, not all at once.
       digital_filter: The Waveshare Hat features a digital filter that can
         accept different settings. Refer to the documentation of the ADS1263
         for more detail.
       gain: Allows to tune the output values of the ADC according to the
-        formula:
-        ::
-
-          output = gain * tension + offset.
-
-        The same gain applies to all the channels.
+        formula : :math:`output = gain * tension + offset`. The same gain
+        applies to all the channels.
       offset: Allows to tune the output values of the ADC according to the
-        formula:
-        ::
-
-          output = gain * tension + offset.
-
-        The same offset applies to all the channels.
+        formula : :math:`output = gain * tension + offset`. The same offset
+        applies to all the channels.
 
     Important:
       When the ``gain_hardware`` is greater than 1, the PGA cannot amplify
       above 4.7V or under 0.3V. For example a 2.8V signal read with a gain of 2
       would be read as 4.7V after the PGA, not 4.8V ! Beware !
     """
 
@@ -209,14 +202,16 @@
     if digital_filter not in range(5):
       raise ValueError(f'digital_filter should be in {list(range(5))}')
     self._filter = digital_filter
 
     # Parsing the channels to check the right syntax was given
     if channels is None:
       channels = ['IN0']
+    else:
+      channels = list(channels)
 
     for channel in channels:
       if fullmatch(r'IN\d', channel) is None and \
             fullmatch(r'IN\d\s?-\s?IN\d', channel) is None:
         raise ValueError("Valid formats for adc_channels values are "
                          "either 'INi' (i in range(10)) or 'INi - INj'")
     self._chan = channels
```

### Comparing `crappy-2.0.0.dev1/src/crappy/links/link.py` & `crappy-2.0.0.dev2/src/crappy/links/link.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,71 +1,79 @@
 # coding: utf-8
 
 from multiprocessing import Pipe
 from time import time
 from copy import deepcopy
-from typing import Callable, Union, Any, Dict, Optional, List
+from typing import Callable, Union, Any, Dict, Optional, List, Iterable
 from collections import defaultdict
 from select import select
+from platform import system
 from multiprocessing import current_process
 import logging
 
-from ..modifier import Modifier
 from .._global import LinkDataError
 
 ModifierType = Callable[[Dict[str, Any]], Dict[str, Any]]
 
 
 class Link:
-  """This class is used for transferring information between the Blocks.
+  """This class is used for transferring information between two instances of
+  :class:`~crappy.blocks.Block`.
 
-  The created link is unidirectional, from the input block to the output block.
-  Under the hood, a link is basically a :class:`multiprocessing.Pipe` with
+  The created Link is unidirectional, from the input Block to the output Block.
+  Under the hood, a Link is basically a :obj:`multiprocessing.Pipe` with
   extra features.
 
   Note:
-    It is possible to add one or multiple :ref:`Modifiers` to modify the
-    transferred value. The modifiers should either be children of
-    :ref:`Modifier` or callables taking a :obj:`dict` as argument and
-    returning a :obj:`dict`.
+    It is possible to add one or multiple :class:`~crappy.modifier.Modifier` to
+    modify the transferred value. The Modifiers should be callables taking a
+    :obj:`dict` as argument and returning a :obj:`dict`. They can be functions,
+    or preferably children of :class:`~crappy.modifier.Modifier`.
   """
 
   _count = 0
 
   def __init__(self,
                input_block,
                output_block,
-               modifiers: Optional[List[Union[ModifierType, Modifier]]] = None,
+               modifiers: Optional[List[ModifierType]] = None,
                name: Optional[str] = None) -> None:
     """Sets the instance attributes.
 
     Args:
-      input_block: The Block sending data through the link.
-      output_block: The Block receiving data through the link.
-      modifiers: A :obj:`list` containing children of :ref:`Modifier` and/or
-        callables. If several objects given ,they will be called in the given
-        order. See :ref:`Modifiers` for more information.
-      name: Name of the link, to differentiate it from the others when
-        debugging. If no specific name is given, the links are anyway numbered
-        in the order in which they are instantiated in the code.
+      input_block: The Block sending data through the Link.
+      output_block: The Block receiving data through the Link.
+      modifiers: A :obj:`list` containing callables. If several objects given,
+        they will be called in the given order. Refer to
+        :class:`~crappy.modifier.Modifier` for more information.
+      name: Name of the Link, to differentiate it from the others when
+        debugging. If no specific name is given, the Links are numbered in the
+        order in which they are instantiated in the script.
     """
 
     if modifiers is None:
       modifiers = list()
 
+    # Checking that all the given modifiers are callable
+    if modifiers and not all(callable(mod) for mod in modifiers):
+      not_callable = [mod for mod in modifiers if not callable(mod)]
+      raise TypeError(f"The following objects passed as modifiers are not "
+                      f"callable : {not_callable} !")
+
     self.name = name if name is not None else f'link{self._get_count()}'
     self._in, self._out = Pipe()
     self._modifiers = modifiers
 
     # Associating the link to the input and output blocks
     input_block.add_output(self)
     output_block.add_input(self)
 
     self._last_warn = time()
     self._logger: Optional[logging.Logger] = None
+    self._system = system()
 
   def __new__(cls, *args, **kwargs):
     """When instantiating a new Link, increments the Link counter."""
 
     cls._count += 1
     return super().__new__(cls)
 
@@ -93,42 +101,42 @@
     """Returns :obj:`True` if there's data available for reading."""
 
     return self._in.poll()
 
   def send(self, value: Dict[str, Any]) -> None:
     """Sends a value from the upstream Block to the downstream Block.
 
-    Before sending, applies the given modifiers and makes sure there's room in
-    the Pipe for sending the data.
+    Before sending, applies the given Modifiers and makes sure there's room in
+    the Pipe for sending the data (Linux only).
     """
 
+    # Applying the modifiers to the value to send
     for mod in self._modifiers:
-      # Case when the modifier is a class
-      if hasattr(mod, 'evaluate'):
-        value = mod.evaluate(deepcopy(value))
-      # Case when the modifier is a method
-      else:
-        value = mod(deepcopy(value))
-
-    if value is None:
-      return
+      value = mod(deepcopy(value))
+      # No need to continue if there's no value to send anymore
+      if value is None:
+        return
 
     if not isinstance(value, dict):
       self.log(logging.ERROR, f"Trying to send object of type {type(value)} "
                               f"instead of dict !")
       raise LinkDataError
 
     # Finally, sending the dict to the link
-    if select([], [self._out], [], 0)[1]:
-      self._out.send(value)
+    if self._system == 'Linux':
+      # Can only check on Linux if a pipe is full
+      if select([], [self._out], [], 0)[1]:
+        self._out.send(value)
+      # Warning in case the pipe is full
+      elif time() - self._last_warn > 1:
+          self._last_warn = time()
+          self.log(logging.WARNING, f"Cannot send the values, the Link is "
+                                    f"full !")
     else:
-      if time() - self._last_warn > 1:
-        self._last_warn = time()
-        self.log(logging.WARNING, f"Cannot send the values, the Link is "
-                                  f"full !")
+      self._out.send(value)
 
   def recv(self) -> Dict[str, Any]:
     """Reads a single value from the Link and returns it.
 
     The read value is the oldest available in the Link, see :meth:`recv_last`
     for reading the newest available value.
 
@@ -179,36 +187,45 @@
         ret[label].append(value)
 
     return dict(ret)
 
 
 def link(in_block,
          out_block,
-         modifier: Optional[Union[List[Union[ModifierType, Modifier]],
-                                  Union[ModifierType, Modifier]]] = None,
+         modifier: Optional[Union[Iterable[ModifierType],
+                                  ModifierType]] = None,
          name: Optional[str] = None) -> None:
-  """Function linking two blocks, allowing to send data from one to the other.
+  """Function linking two Blocks, allowing to send data from one to the other.
+
+  It instantiates a :class:`~crappy.links.Link` between two children of
+  :class:`~crappy.blocks.Block`.
 
-  The created link is unidirectional, from the input block to the output block.
-  Under the hood, a link is basically a :class:`multiprocessing.Pipe` with
+  The created Link is unidirectional, from the input Block to the output Block.
+  Under the hood, a Link is basically a :obj:`multiprocessing.Pipe` with
   extra features.
 
   Args:
-    in_block: The Block sending data through the link.
-    out_block: The Block receiving data through the link.
-    modifier: Either a child class of :ref:`Modifier`, or a callable, or a
-      :obj:`list` containing such objects. If several given (in a list), calls
-      them in the  given order. See :ref:`Modifiers` for more information.
-    name: Name of the link, to differentiate it from the others when debugging.
-      If no specific name is given, the links are anyway numbered in the order
-      in which they are instantiated in the code.
+    in_block: The Block sending data through the Link.
+    out_block: The Block receiving data through the Link.
+    modifier: Either a callable, or an iterable (like a :obj:`list` or a
+      :obj:`tuple`) containing callables. If several given (in an iterable),
+      they are called in the given order. They should preferably be children of
+      :class:`~crappy.modifier.Modifier`. Refer to  the associated
+      documentation for more information.
+    name: Name of the Link, to differentiate it from the others when debugging.
+      If no specific name is given, the Links are numbered in the order in
+      which they are instantiated in the script.
   """
 
   # Forcing the modifiers into lists
-  if modifier is not None and not isinstance(modifier, list):
-    modifier = [modifier]
+  if modifier is not None:
+    try:
+      iter(modifier)
+      modifier = list(modifier)
+    except TypeError:
+      modifier = [modifier]
 
   # Actually creating the Link object
   Link(input_block=in_block,
        output_block=out_block,
        modifiers=modifier,
        name=name)
```

### Comparing `crappy-2.0.0.dev1/src/crappy/modifier/demux.py` & `crappy-2.0.0.dev2/src/crappy/modifier/demux.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,72 @@
 # coding: utf-8
 
 import numpy as np
-from typing import Dict, Any, Union, List, Tuple
+from typing import Dict, Any, Union, Iterable
 import logging
 
 from .meta_modifier import Modifier
 
 
 class Demux(Modifier):
-  """Modifier converting a stream into a regular Crappy :obj:`dict` giving for
-  each label a single value.
+  """Modifier converting a stream into a regular data flow interpretable by
+  most Blocks.
 
-  The single value is either the first value of a column/row, or the average
-  of the row/column values. This Modifier is mainly meant for linking streaming
-  :ref:`IOBlock` blocks to :ref:`Grapher` blocks, as it is otherwise impossible
-  to plot their data.
+  It is meant to be used on a :class:`~crappy.links.Link` taking an
+  :class:`~crappy.blocks.IOBlock` in streamer mode as an input. It converts
+  the stream to make it readable by most Blocks, and also splits the stream in
+  several labels if necessary.
+
+  It takes a stream as an input, i.e. a :obj:`dict` whose values are numpy
+  arrays, and outputs another :obj:`dict` whose values are :obj:`float`. If the
+  numpy arrays contains several columns (corresponding to several acquired
+  channels), it splits them into several labels.
+
+  Important:
+    In the process of converting the stream data to regular labeled data, much
+    information is lost ! This Modifier is intended to format the stream data
+    for low-frequency plotting, or low-frequency decision-making. To save all
+    the stream data, use the :class:`~crappy.blocks.HDFRecorder` Block.
   """
 
   def __init__(self,
-               labels: Union[str, List[str], Tuple[str, ...]],
+               labels: Union[str, Iterable[str]],
                stream_label: str = "stream",
                mean: bool = False,
                time_label: str = "t(s)",
                transpose: bool = False) -> None:
     """Sets the args and initializes the parent class.
 
     Args:
       labels: The labels corresponding to the rows or columns of the stream.
-        It can be either a single label, or a :obj:`list` of labels, or a
-        :obj:`tuple` of labels. They must be given in the same order as they
-        appear in the stream. If fewer labels are given than there are rows or
-        columns in the stream, only the data from the first rows/columns will
-        be retrieved.
+        It can be either a single label, or an iterable of labels (like a
+        :obj:`list` or a :obj:`tuple`). They must be given in the same order as
+        they appear in the stream. If fewer labels are given than there are
+        rows or columns in the stream, only the data from the first rows or
+        columns will be retrieved.
       stream_label: The label carrying the stream.
       mean: If :obj:`True`, the returned value will be the average of the
-        stream data. Otherwise, it will be the first value.
+        row or column. Otherwise, it will be the first value.
       time_label: The label carrying the time information.
       transpose: If :obj:`True`, each label corresponds to a row in the stream.
         Otherwise, a label corresponds to a column in the stream.
     """
 
     super().__init__()
 
-    if isinstance(labels, list) or isinstance(labels, tuple):
-      self._labels = labels
-    else:
-      self._labels = (labels,)
+    if isinstance(labels, str):
+      labels = (labels,)
+    self._labels = labels
+
     self._stream_label = stream_label
     self._mean = mean
     self._time_label = time_label
     self._transpose = transpose
 
-  def evaluate(self, data: Dict[str, np.ndarray]) -> Dict[str, Any]:
+  def __call__(self, data: Dict[str, np.ndarray]) -> Dict[str, Any]:
     """Retrieves for each label its value in the stream, also gets the
     corresponding timestamp, and returns them."""
 
     self.log(logging.DEBUG, f"Received {data}")
 
     # If there are no rows or no column, cannot perform the demux
     if 0 in data[self._stream_label].shape:
```

### Comparing `crappy-2.0.0.dev1/src/crappy/modifier/differentiate.py` & `crappy-2.0.0.dev2/src/crappy/modifier/differentiate.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,41 +3,41 @@
 from typing import Optional, Dict, Any
 import logging
 
 from .meta_modifier import Modifier
 
 
 class Diff(Modifier):
-  """This modifier differentiates the data of a label over time and adds the
-  differentiation value to the returned data."""
+  """This Modifier calculates the time derivative of a given label and adds the
+  derivative to the returned data."""
 
   def __init__(self,
                label: str,
                time_label: str = 't(s)',
                out_label: Optional[str] = None) -> None:
     """Sets the args and initializes the parent class.
 
     Args:
-      label: The label whose data to differentiate over time.
+      label: The label whose time derivative to compute.
       time_label: The label carrying the time information.
-      out_label: The label carrying the differentiation value. If not given,
+      out_label: The label carrying the calculated derivative. If not given,
         defaults to ``'d_<label>'``.
     """
 
     super().__init__()
     self._label = label
     self._time_label = time_label
     self._out_label = out_label if out_label is not None else f'd_{label}'
 
     self._last_t = None
     self._last_val = None
 
-  def evaluate(self, data: Dict[str, Any]) -> Dict[str, Any]:
-    """Gets the data from the upstream block, updates the differentiation value
-    and returns it."""
+  def __call__(self, data: Dict[str, Any]) -> Dict[str, Any]:
+    """Gets the data from the upstream Block, updates the derivative value,
+    appends it to the data and returns the data."""
 
     self.log(logging.DEBUG, f"Received {data}")
 
     # For the first received data, storing it and returning 0
     if self._last_t is None or self._last_val is None:
       self._last_t = data[self._time_label]
       self._last_val = data[self._label]
```

### Comparing `crappy-2.0.0.dev1/src/crappy/modifier/mean.py` & `crappy-2.0.0.dev2/src/crappy/modifier/median.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 import numpy as np
 from typing import Dict, Any, Optional
 import logging
 
 from .meta_modifier import Modifier
 
 
-class Mean(Modifier):
+class Median(Modifier):
   """Modifier waiting for a given number of data points to be received, then
-  returning their average, and starting all over again.
+  returning their median, and starting all over again.
 
-  Unlike :ref:`Moving Average`, it only returns a value once every ``n_points``
-  points.
+  Unlike :class:`~crappy.modifier.MovingMed`, it only returns a value once
+  every ``n_points`` points.
   """
 
   def __init__(self, n_points: int = 100) -> None:
     """Sets the args and initializes the parent class.
 
     Args:
-      n_points: The number of points on which to compute the average.
+      n_points: The number of points on which to compute the median.
     """
 
     super().__init__()
     self._n_points = n_points
     self._buf = None
 
-  def evaluate(self, data: Dict[str, Any]) -> Optional[Dict[str, Any]]:
-    """Receives data from the upstream block, and computes the average of every
+  def __call__(self, data: Dict[str, Any]) -> Optional[Dict[str, Any]]:
+    """Receives data from the upstream Block, and computes the median of every
     label once the right number of points have been received. Then empties the
-    buffer and returns the averages.
+    buffer and returns the medians.
 
     If there are not enough points, doesn't return anything.
     """
 
     self.log(logging.DEBUG, f"Received {data}")
 
     # Initializing the buffer
@@ -41,18 +41,18 @@
       self._buf = {key: [value] for key, value in data.items()}
 
     ret = {}
     for label in data:
       # Updating the buffer with the newest data
       self._buf[label].append(data[label])
 
-      # Once there's enough data in the buffer, calculating the average value
+      # Once there's enough data in the buffer, calculating the median value
       if len(self._buf[label]) == self._n_points:
         try:
-          ret[label] = np.mean(self._buf[label])
+          ret[label] = np.median(self._buf[label])
         except TypeError:
           ret[label] = self._buf[label][-1]
 
         # Resetting the buffer
         self._buf[label].clear()
 
     if ret:
```

### Comparing `crappy-2.0.0.dev1/src/crappy/modifier/median.py` & `crappy-2.0.0.dev2/src/crappy/modifier/mean.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 import numpy as np
 from typing import Dict, Any, Optional
 import logging
 
 from .meta_modifier import Modifier
 
 
-class Median(Modifier):
+class Mean(Modifier):
   """Modifier waiting for a given number of data points to be received, then
-  returning their median, and starting all over again.
+  returning their average, and starting all over again.
 
-  Unlike :ref:`Moving Median`, it only returns a value once every ``n_points``
-  points.
+  Unlike :class:`~crappy.modifier.MovingAvg`, it only returns a value once
+  every ``n_points`` points.
   """
 
   def __init__(self, n_points: int = 100) -> None:
     """Sets the args and initializes the parent class.
 
     Args:
-      n_points: The number of points on which to compute the median.
+      n_points: The number of points on which to compute the average.
     """
 
     super().__init__()
     self._n_points = n_points
     self._buf = None
 
-  def evaluate(self, data: Dict[str, Any]) -> Optional[Dict[str, Any]]:
-    """Receives data from the upstream block, and computes the median of every
+  def __call__(self, data: Dict[str, Any]) -> Optional[Dict[str, Any]]:
+    """Receives data from the upstream Block, and computes the average of every
     label once the right number of points have been received. Then empties the
-    buffer and returns the medians.
+    buffer and returns the averages.
 
     If there are not enough points, doesn't return anything.
     """
 
     self.log(logging.DEBUG, f"Received {data}")
 
     # Initializing the buffer
@@ -41,18 +41,18 @@
       self._buf = {key: [value] for key, value in data.items()}
 
     ret = {}
     for label in data:
       # Updating the buffer with the newest data
       self._buf[label].append(data[label])
 
-      # Once there's enough data in the buffer, calculating the median value
+      # Once there's enough data in the buffer, calculating the average value
       if len(self._buf[label]) == self._n_points:
         try:
-          ret[label] = np.median(self._buf[label])
+          ret[label] = np.mean(self._buf[label])
         except TypeError:
           ret[label] = self._buf[label][-1]
 
         # Resetting the buffer
         self._buf[label].clear()
 
     if ret:
```

### Comparing `crappy-2.0.0.dev1/src/crappy/modifier/moving_avg.py` & `crappy-2.0.0.dev2/src/crappy/modifier/moving_med.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 import numpy as np
 from typing import Dict, Any
 import logging
 
 from .meta_modifier import Modifier
 
 
-class MovingAvg(Modifier):
-  """Modifier replacing the data of each label with its average value over a
+class MovingMed(Modifier):
+  """Modifier replacing the data of each label with its median value over a
   chosen number of points.
 
-  Unlike :ref:`Mean`, it returns a value each time a message is received from
-  the upstream link.
+  Unlike :class:`~crappy.modifier.Median`, it returns a value each time data is
+  received from the upstream Block.
   """
 
   def __init__(self, n_points: int = 100) -> None:
     """Sets the args and initializes the parent class.
 
     Args:
-      n_points: The maximum number of points on which to compute the average.
+      n_points: The maximum number of points on which to compute the median.
     """
 
     super().__init__()
     self._n_points = n_points
     self._buf = None
 
-  def evaluate(self, data: Dict[str, Any]) -> Dict[str, Any]:
-    """Receives data from the upstream block, computes the average of every
+  def __call__(self, data: Dict[str, Any]) -> Dict[str, Any]:
+    """Receives data from the upstream Block, computes the median of every
     label and replaces the original data with it."""
 
     self.log(logging.DEBUG, f"Received {data}")
 
     # Initializing the buffer
     if self._buf is None:
       self._buf = {key: [value] for key, value in data.items()}
@@ -41,15 +41,15 @@
       # Updating the buffer with the newest data
       self._buf[label].append(data[label])
 
       # Trimming the buffer if there's too much data
       if len(self._buf[label]) > self._n_points:
         self._buf[label] = self._buf[label][-self._n_points:]
 
-      # Calculating the average for each label
+      # Calculating the median for each label
       try:
-        ret[label] = np.mean(self._buf[label])
+        ret[label] = np.median(self._buf[label])
       except TypeError:
         ret[label] = self._buf[label][-1]
 
     self.log(logging.DEBUG, f"Sending {ret}")
     return ret
```

### Comparing `crappy-2.0.0.dev1/src/crappy/modifier/moving_med.py` & `crappy-2.0.0.dev2/src/crappy/modifier/moving_avg.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 import numpy as np
 from typing import Dict, Any
 import logging
 
 from .meta_modifier import Modifier
 
 
-class MovingMed(Modifier):
-  """Modifier replacing the data of each label with its median value over a
+class MovingAvg(Modifier):
+  """Modifier replacing the data of each label with its average value over a
   chosen number of points.
 
-  Unlike :ref:`Median`, it returns a value each time a message is received from
-  the upstream link.
+  Unlike :class:`~crappy.modifier.Mean`, it returns a value each time data is
+  received from the upstream Block.
   """
 
   def __init__(self, n_points: int = 100) -> None:
     """Sets the args and initializes the parent class.
 
     Args:
-      n_points: The maximum number of points on which to compute the median.
+      n_points: The maximum number of points on which to compute the average.
     """
 
     super().__init__()
     self._n_points = n_points
     self._buf = None
 
-  def evaluate(self, data: Dict[str, Any]) -> Dict[str, Any]:
-    """Receives data from the upstream block, computes the median of every
+  def __call__(self, data: Dict[str, Any]) -> Dict[str, Any]:
+    """Receives data from the upstream Block, computes the average of every
     label and replaces the original data with it."""
 
     self.log(logging.DEBUG, f"Received {data}")
 
     # Initializing the buffer
     if self._buf is None:
       self._buf = {key: [value] for key, value in data.items()}
@@ -41,15 +41,15 @@
       # Updating the buffer with the newest data
       self._buf[label].append(data[label])
 
       # Trimming the buffer if there's too much data
       if len(self._buf[label]) > self._n_points:
         self._buf[label] = self._buf[label][-self._n_points:]
 
-      # Calculating the median for each label
+      # Calculating the average for each label
       try:
-        ret[label] = np.median(self._buf[label])
+        ret[label] = np.mean(self._buf[label])
       except TypeError:
         ret[label] = self._buf[label][-1]
 
     self.log(logging.DEBUG, f"Sending {ret}")
     return ret
```

### Comparing `crappy-2.0.0.dev1/src/crappy/modifier/offset.py` & `crappy-2.0.0.dev2/src/crappy/modifier/offset.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 
-from typing import Dict, Any, List, Union, Tuple
+from typing import Dict, Any, Union, Iterable
 import logging
 
 from .meta_modifier import Modifier
 
 
 class Offset(Modifier):
   """This Modifier offsets every value of the given labels by a constant. This
@@ -12,54 +12,58 @@
   equal to a user-defined target.
 
   For example if for a given label the target is `6` and the first received
   value is `3`, the Modifier will add `3` to each value received over this
   label.
 
   This Modifier can be used for example when measuring a variable that should
-  start at `0` (like a force) but doesn't because of a sensor offset. It can
-  also just be used to plot nicer figures. It is not very accurate as it is
-  only based on a single data point for the offset calculation. The
-  ``make_zero`` argument of the :ref:`IOBlock` is a better alternative if
-  precision is required when offsetting the data.
+  start at `0` but doesn't because of a sensor offset. It can also just be used
+  to plot nicer figures. It is not very accurate as it is only based on a
+  single data point for the offset calculation. The ``make_zero`` argument of
+  the :class:`~crappy.blocks.IOBlock` is a better alternative if precision is
+  required when offsetting a sensor.
   """
 
   def __init__(self,
-               labels: Union[str, List[str], Tuple[str, ...]],
-               offsets: Union[float, List[float], Tuple[float, ...]]) -> None:
+               labels: Union[str, Iterable[str]],
+               offsets: Union[float, Iterable[float]]) -> None:
     """Sets the args and initializes the parent class.
 
     Args:
       labels: The labels to offset. Can be given as a single label, a
         :obj:`list` of labels or a :obj:`tuple` of labels.
       offsets: For each label, the target for the first received value. Can be
         given as a single value, a :obj:`list` of values or a :obj:`tuple` of
         values.
     """
 
     super().__init__()
 
     # Handling the case when only one label needs to be offset
-    if not isinstance(labels, list) and not isinstance(labels, tuple):
+    if isinstance(labels, str):
       labels = (labels,)
-    if not isinstance(offsets, list) and not isinstance(offsets, tuple):
+    labels = tuple(labels)
+    try:
+      iter(offsets)
+    except TypeError:
       offsets = (offsets,)
+    offsets = tuple(offsets)
 
     # Checking that the number of offsets match the number of labels
     if len(offsets) != len(labels):
       raise ValueError("As many offsets as there are labels should be given.")
 
     # Associating each offset to its label
     self._offsets = {label: offset for label, offset in zip(labels, offsets)}
 
     self._compensations = None
     self._compensated = False
 
-  def evaluate(self, data: Dict[str, Any]) -> Dict[str, Any]:
-    """If the compensations are not set, sets them, anf then offsets the
+  def __call__(self, data: Dict[str, Any]) -> Dict[str, Any]:
+    """If the compensations are not set, sets them, and then offsets the
     required labels."""
 
     self.log(logging.DEBUG, f"Received {data}")
 
     # During the first loop, calculating the compensation values
     if not self._compensated:
       self._compensations = {label: -data[label] + offset for label, offset in
```

### Comparing `crappy-2.0.0.dev1/src/crappy/modifier/trig_on_change.py` & `crappy-2.0.0.dev2/src/crappy/modifier/trig_on_change.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 from typing import Optional, Dict, Any
 import logging
 
 from .meta_modifier import Modifier
 
 
 class TrigOnChange(Modifier):
-  """Modifier passing the data to the downstream block only when the value of
+  """Modifier passing the data to the downstream Block only when the value of
   a given label changes.
 
-  It also transmits the first received data. Can be used to trig a block upon
-  change of a label value.
+  It also transmits the first received data. Can be used to trigger a Block
+  upon change of a label value.
   """
 
   def __init__(self, label: str) -> None:
     """Sets the args and initializes the parent class.
 
     Args:
       label: The name of the label to monitor.
     """
 
     super().__init__()
     self._label = label
     self._last = None
 
-  def evaluate(self, data: Dict[str, Any]) -> Optional[Dict[str, Any]]:
+  def __call__(self, data: Dict[str, Any]) -> Optional[Dict[str, Any]]:
     """Compares the received value with the last sent one, and if they're
     different sends the received data and stores the latest value."""
 
     self.log(logging.DEBUG, f"Received {data}")
 
     # Storing the first received value and returning the data
     if self._last is None:
```

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/bindings/comedi_bind.py` & `crappy-2.0.0.dev2/src/crappy/tool/bindings/comedi_bind.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # coding: utf-8
 
 """This file contains the code for binding the C++ Comedi library in Python.
 
-The bindings haven't been tested for a while.
+It is only used by the :class:`~crappy.inout.Comedi` InOut. The bindings
+haven't been tested for a while.
 """
 
 from ctypes import *
 from ..._global import OptionalModule
 
 try:
   comedi = cdll.LoadLibrary("/usr/lib/libcomedi.so")
```

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/bindings/pyspcm.py` & `crappy-2.0.0.dev2/src/crappy/tool/bindings/pyspcm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # coding: utf-8
 
 """This file contains the code for binding the C++ Spectrum library in Python.
 
-The bindings haven't been tested for a while.
+It is only used by the :class:`~crappy.inout.SpectrumM2I4711` InOut. The
+bindings haven't been tested for a while.
 """
 
 from ctypes import *
 from sys import platform
 from ..._global import OptionalModule
 
 # ======= Constants definition ======
```

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/camera_config/camera_config.py` & `crappy-2.0.0.dev2/src/crappy/tool/camera_config/camera_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,93 @@
 # coding: utf-8
 
 import tkinter as tk
 from tkinter.messagebox import showerror
+from _tkinter import TclError
 from platform import system
 import numpy as np
 from time import time, sleep
 from typing import Optional, Tuple
-from functools import partial
 from pkg_resources import resource_string
 from io import BytesIO
 import logging
-from multiprocessing import current_process
+from multiprocessing import current_process, Event, Pipe
+from multiprocessing.queues import Queue
 
-from .config_tools import Zoom
+from .config_tools import Zoom, HistogramProcess
 from ...camera.meta_camera.camera_setting import CameraBoolSetting, \
   CameraChoiceSetting, CameraScaleSetting
 from ...camera.meta_camera import Camera
 from ..._global import OptionalModule
 
 try:
   from PIL import ImageTk, Image
 except (ModuleNotFoundError, ImportError):
   ImageTk = OptionalModule("pillow")
   Image = OptionalModule("pillow")
 
 
 class CameraConfig(tk.Tk):
   """This class is a GUI allowing the user to visualize the images from a
-  camera before a Crappy test starts, and to tune the settings of the camera.
+  :class:`~crappy.camera.Camera` before a Crappy test starts, and to tune the
+  settings of the Camera.
 
   It is meant to be user-friendly and interactive. It is possible to zoom on
   the image using the mousewheel, and to move on the zoomed image by
-  left-clicking and dragging.
+  right-clicking and dragging.
 
   In addition to the image, the interface also displays a histogram of the
   pixel values, an FPS counter, a detected bits counter, the minimum and
-  maximum pixel values and the value and position of the pixel currently under
+  maximum pixel values, and the value and position of the pixel currently under
   the mouse. A checkbox allows auto-adjusting the pixel range to get a better
   contrast.
+
+  This class is used as is by the :class:`~crappy.blocks.Camera`, but also 
+  subclassed to provide more specific functionalities to other camera-related 
+  Blocks like :class:`~crappy.blocks.VideoExtenso` or 
+  :class:`~crappy.blocks.DICVE`.
+  
+  This class is a child of :obj:`tkinter.Tk`. It relies on the 
+  :class:`~crappy.tool.camera_config.config_tools.Zoom` and 
+  :class:`~crappy.tool.camera_config.config_tools.HistogramProcess` tools. It
+  also interacts with instances of the 
+  :class:`~crappy.camera.meta_camera.camera_setting.CameraSetting` class.
   """
 
-  def __init__(self, camera: Camera) -> None:
-    """Initializes the interface and starts displaying the first image.
+  def __init__(self,
+               camera: Camera,
+               log_queue: Queue,
+               log_level: Optional[int]) -> None:
+    """Initializes the interface and displays it.
 
     Args:
-      camera: The camera object in charge of acquiring the images.
+      camera: The :class:`~crappy.camera.Camera` object in charge of acquiring 
+        the images.
+      log_queue: A :obj:`multiprocessing.Queue` for sending the log messages to 
+        the main :obj:`~logging.Logger`, only used in Windows.
+      log_level: The minimum logging level of the entire Crappy script, as an
+        :obj:`int`.
     """
 
     super().__init__()
     self._camera = camera
     self.shape = None
     self.dtype = None
     self._logger: Optional[logging.Logger] = None
 
+    # Instantiating objects for the process managing the histogram calculation
+    self._stop_event = Event()
+    self._processing_event = Event()
+    self._img_in, img_in_proc = Pipe()
+    img_out_proc, self._img_out = Pipe()
+    self._histogram_process = HistogramProcess(
+        stop_event=self._stop_event, processing_event=self._processing_event,
+        img_in=img_in_proc, img_out=img_out_proc, log_level=log_level,
+        log_queue=log_queue)
+
     # Attributes containing the several images and histograms
     self._img = None
     self._pil_img = None
     self._original_img = None
     self._hist = None
     self._pil_hist = None
 
@@ -71,61 +102,103 @@
     # Settings for adjusting the behavior of the zoom
     self._zoom_ratio = 0.9
     self._zoom_step = 0
     self._max_zoom_step = 15
 
     # Settings of the root window
     self.title(f'Configuration window for the camera: {type(camera).__name__}')
-    self.protocol("WM_DELETE_WINDOW", self._stop)
+    self.protocol("WM_DELETE_WINDOW", self.finish)
     self._zoom_values = Zoom()
 
     # Initializing the interface
     self._set_variables()
     self._set_traces()
     self._set_layout()
     self._set_bindings()
     self._add_settings()
     self.update()
 
-    # Displaying the first image
-    self._update_img(init=True)
-
   def main(self) -> None:
     """Constantly updates the image and the information on the GUI, until asked
     to stop."""
 
+    # Starting the histogram calculation process
+    self._histogram_process.start()
+
     self._n_loops = 0
     start_time = time()
 
     while self._run:
       # Update the image, the histogram and the information
-      self._update_img(init=False)
+      self._update_img()
 
       # Update the FPS counter
       if time() - start_time > 0.5:
         self._fps_var.set(self._n_loops / (time() - start_time))
         self._n_loops = 0
         start_time = time()
 
   def log(self, level: int, msg: str) -> None:
-    """"""
+    """Record log messages for the CameraConfig window.
+
+    Also instantiates the :obj:`~logging.Logger` when logging the first
+    message.
+
+    Args:
+      level: An :obj:`int` indicating the logging level of the message.
+      msg: The message to log, as a :obj:`str`.
+    """
 
     if self._logger is None:
       self._logger = logging.getLogger(
         f"{current_process().name}.{type(self).__name__}")
 
     self._logger.log(level, msg)
 
   def report_callback_exception(self, exc: Exception, val: str, tb) -> None:
-    """"""
+    """Method displaying an error message in case an exception is raised in a
+    :mod:`tkinter` callback."""
 
     self._logger.exception(f"Caught exception in {type(self).__name__}: "
                            f"{exc.__name__}({val})", exc_info=tb)
     showerror("Error !", message=f"{exc.__name__}\n{val}")
 
+  def finish(self) -> None:
+    """Method called when the user tries to close the configuration window.
+
+    Mostly intended for being overwritten.
+    """
+
+    self.stop()
+
+  def stop(self) -> None:
+    """Method called for gracefully stopping the GUI.
+
+    Stops the process calculating the histogram, and destroys the GUI.
+    """
+
+    # Stopping the event loop and the histogram process
+    self._run = False
+    self._stop_event.set()
+    sleep(0.1)
+
+    # Killing the histogram process if it's still alive
+    if self._histogram_process.is_alive():
+      self.log(logging.WARNING, "The histogram process failed to stop, "
+                                "killing it !")
+      self._histogram_process.terminate()
+
+    self.log(logging.DEBUG, "Destroying the configuration window")
+
+    try:
+      self.destroy()
+    except TclError:
+      self.log(logging.WARNING, "Cannot destroy the configuration window, "
+                                "ignoring")
+
   def _set_layout(self) -> None:
     """Creates and places the different elements of the display on the GUI."""
 
     self.log(logging.DEBUG, "Setting the interface layout")
 
     # The main frame of the window
     self._main_frame = tk.Frame()
@@ -576,30 +649,33 @@
     self.log(logging.DEBUG, f"Adding the choice setting {cam_set.name}")
 
     cam_set.tk_var = tk.StringVar(value=cam_set.value)
     label = tk.Label(self._canvas_frame, text=f'{cam_set.name} :')
     label.pack(anchor='w', side='top', expand=False, fill='none',
                padx=12, pady=2)
     for value in cam_set.choices:
-      cam_set.tk_obj = tk.Radiobutton(self._canvas_frame,
-                                      text=value,
-                                      variable=cam_set.tk_var,
-                                      value=value)
-      cam_set.tk_obj.pack(anchor='w', side='top', expand=False,
-                          fill='none', padx=5, pady=2)
+      tk_obj = tk.Radiobutton(self._canvas_frame,
+                              text=value,
+                              variable=cam_set.tk_var,
+                              value=value)
+      tk_obj.pack(anchor='w', side='top', expand=False,
+                  fill='none', padx=5, pady=2)
+      cam_set.tk_obj.append(tk_obj)
 
   def _set_variables(self) -> None:
     """Sets the text and numeric variables holding information about the
     display."""
 
     self.log(logging.DEBUG, "Setting the interface variables")
 
     # The FPS counter
     self._fps_var = tk.DoubleVar(value=0.)
-    self._fps_txt = tk.StringVar(value=f'fps = {self._fps_var.get():.2f}')
+    self._fps_txt = tk.StringVar(
+        value=f'fps = {self._fps_var.get():.2f}\n(might be lower in this GUI '
+              f'than actual)')
 
     # The variable for enabling or disabling the auto range
     self._auto_range = tk.BooleanVar(value=False)
 
     # The minimum and maximum pixel value counters
     self._min_pixel = tk.IntVar(value=0)
     self._max_pixel = tk.IntVar(value=0)
@@ -643,15 +719,16 @@
     self._x_pos.trace_add('write', self._update_reticle)
     self._y_pos.trace_add('write', self._update_reticle)
     self._reticle_val.trace_add('write', self._update_reticle)
 
   def _update_fps(self, _, __, ___) -> None:
     """Auto-update of the FPS display."""
 
-    self._fps_txt.set(f'fps = {self._fps_var.get():.2f}')
+    self._fps_txt.set(f'fps = {self._fps_var.get():.2f}\n'
+                      f'(might be lower in this GUI than actual)')
 
   def _update_min_max(self, _, __, ___) -> None:
     """Auto-update of the minimum and maximum pixel values display."""
 
     self._min_max_pix_txt.set(f'min: {self._min_pixel.get():d}, '
                               f'max: {self._max_pixel.get():d}')
 
@@ -786,44 +863,42 @@
 
   def _calc_hist(self) -> None:
     """Calculates the histogram of the current image."""
 
     if self._original_img is None:
       return
 
-    self.log(logging.DEBUG, "Calculating the histogram of the image")
-
-    # The histogram is calculated on a grey level image
-    if len(self._original_img.shape) == 3:
-      self._original_img = np.mean(self._original_img, axis=2)
-
-    # Building the image containing the histogram
-    hist, _ = np.histogram(self._original_img, bins=np.arange(257))
-    hist = np.repeat(hist / np.max(hist) * 80, 2)
-    hist = np.repeat(hist[np.newaxis, :], 80, axis=0)
-
-    out_img = np.fromfunction(partial(self._hist_func, histo=hist),
-                              shape=(80, 512))
-    out_img = np.flip(out_img, axis=0).astype('uint8')
-
-    # Adding vertical grey bars to indicate the limits of the auto range
-    if self._auto_range.get():
-      out_img[:, round(2 * self._low_thresh)] = 127
-      out_img[:, round(2 * self._high_thresh)] = 127
-
-    self._hist = out_img
-
-  @staticmethod
-  def _hist_func(x: np.ndarray,
-                 _: np.ndarray,
-                 histo: np.ndarray) -> np.ndarray:
-    """Function passed to the :meth:`np.fromfunction` method for building the
-    histogram."""
+    # Don't calculate histogram if a calculation is already running
+    if self._processing_event.is_set():
+      self.log(logging.DEBUG, "A calculation is running for the histogram, "
+                              "not sending image for calculation")
+      return
 
-    return np.where(x <= histo, 0, 255)
+    # If no calculation is running, sending a new image for calculation
+    else:
+      # Reshaping the image before sending to the histogram process
+      self.log(logging.DEBUG, "Preparing image for histogram calculation")
+      hist_img = Image.fromarray(self._original_img)
+      if hist_img.width > 320 or hist_img.height > 240:
+        factor = min(320 / hist_img.width, 240 / hist_img.height)
+        hist_img = hist_img.resize((int(hist_img.width * factor),
+                                    int(hist_img.height * factor)))
+      # The histogram is calculated on a grey level image
+      if len(self._original_img.shape) == 3:
+        hist_img = hist_img.convert('L')
+
+      # Sending the image to the histogram process
+      self.log(logging.DEBUG, "Sending image for histogram calculation")
+      self._img_in.send((hist_img, self._auto_range.get(),
+                         self._low_thresh, self._high_thresh))
+
+    # Checking if a histogram is available for display
+    while self._img_out.poll():
+      self._hist = self._img_out.recv()
+      self.log(logging.DEBUG, "Received histogram from histogram process")
 
   def _resize_hist(self) -> None:
     """Resizes the histogram image to make it fit in the GUI."""
 
     if self._hist is None:
       return
 
@@ -852,32 +927,26 @@
     """Resizes the histogram and updates the display when the GUI has been
     resized."""
 
     self._resize_hist()
     self._display_hist()
     self.update()
 
-  def _update_img(self, init: bool = False) -> None:
+  def _update_img(self) -> None:
     """Acquires an image from the camera, casts and resizes it, calculates its
-    histogram, displays them and updates the image information.
-
-    Args:
-      init: If :obj:`True`, means that the method is called during
-        :meth:`__init__` and if the image cannot be obtained it should be
-        replaced with a dummy one.
-    """
+    histogram, displays them and updates the image information."""
 
     self.log(logging.DEBUG, "Updating the image")
 
     ret = self._camera.get_image()
 
     # If no frame could be grabbed from the camera
     if ret is None:
       # If it's the first call, generate error image to initialize the window
-      if init:
+      if not self._n_loops:
         self.log(logging.WARNING, "Could not get an image from the camera, "
                                   "displaying an error image instead")
         ret = None, np.array(Image.open(BytesIO(resource_string(
           'crappy', 'tool/data/no_image.png'))))
       # Otherwise, just pass
       else:
         self.log(logging.DEBUG, "No image returned by the camera")
@@ -901,15 +970,7 @@
 
     self._display_img()
     self._display_hist()
 
     self._update_pixel_value()
 
     self.update()
-
-  def _stop(self) -> None:
-    """When the window is being destroyed, stop the main loop."""
-
-    self._run = False
-    sleep(0.1)
-    self.log(logging.DEBUG, "Destroying the configuration window")
-    self.destroy()
```

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/camera_config/camera_config_boxes.py` & `crappy-2.0.0.dev2/src/crappy/tool/camera_config/camera_config_boxes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,78 @@
 # coding: utf-8
 
 import numpy as np
 import tkinter as tk
 import logging
+from typing import Optional
+from multiprocessing.queues import Queue
 
 from .camera_config import CameraConfig
 from .config_tools import Box, SpotsBoxes
 from ...camera.meta_camera import Camera
 
 
 class CameraConfigBoxes(CameraConfig):
   """This class is a basis for the configuration GUIs featuring boxes to
   display or to draw.
-
-  It implements useful methods for drawing the boxes. If instantiated, this
-  class behaves the exact same way as its parent class. It is not used as is by
-  any block in Crappy.
+  
+  It is a child of the base :class:`~crappy.tool.camera_config.CameraConfig`,
+  and relies on the :class:`~crappy.tool.camera_config.config_tools.Box` and
+  :class:`~crappy.tool.camera_config.config_tools.SpotsBoxes` tools. It
+  implements useful methods for drawing one or several Boxes. If instantiated,
+  this class behaves the exact same way as its parent class. It is not used as
+  is by any Block in Crappy.
   """
 
-  def __init__(self, camera: Camera) -> None:
-    """Initializes the parent class and sets the spots container."""
+  def __init__(self,
+               camera: Camera,
+               log_queue: Queue,
+               log_level: Optional[int]) -> None:
+    """Initializes the parent class and sets the spots container.
+
+    Args:
+      camera: The :class:`~crappy.camera.Camera` object in charge of acquiring 
+        the images.
+      log_queue: A :obj:`multiprocessing.Queue` for sending the log messages to 
+        the main :obj:`~logging.Logger`, only used in Windows.
+      log_level: The minimum logging level of the entire Crappy script, as an
+        :obj:`int`.
+    """
 
     self._spots = SpotsBoxes()
     self._select_box = Box()
-    super().__init__(camera)
+    super().__init__(camera, log_queue, log_level)
 
   def _draw_box(self, box: Box) -> None:
     """Draws one line of the box after the other, making sure they fit in the
     image."""
 
     if self._img is None or box.no_points():
       return
 
     self.log(logging.DEBUG, f"Drawing the box: {box}")
 
-    # The sides need to be sorted before slicing numpy array
-    y_left, y_right, x_top, x_bottom = box.sorted()
-
-    # Drawing one line after the other
-    for slice_ in ((slice(x_top, x_bottom), y_left),
-                   (slice(x_top, x_bottom), y_right),
-                   (x_top, slice(y_left, y_right)),
-                   (x_bottom, slice(y_left, y_right))):
-      try:
-        # The color of the line is adjusted according to the background
-        # The original image must be used as no lines are already drawn on it
-        if np.size(self._original_img[slice_]) > 0:
-          self._img[slice_] = 255 * np.rint(np.mean(self._img[slice_] < 128))
-      except IndexError:
-        self._handle_box_outside_img(box)
-        return
+    # Determining the number of lines to draw
+    x_top, x_bottom, y_left, y_right = box.sorted()
+    canvas_width = self._img_canvas.winfo_width()
+    canvas_height = self._img_canvas.winfo_height()
+    max_fact = max(self._img.shape[0] // canvas_height,
+                   self._img.shape[1] // canvas_width, 1)
+
+    try:
+      for line in (line for i in range(max_fact) for line in
+                   ((box.y_start + i, slice(x_top, x_bottom)),
+                    (box.y_end - i, slice(x_top, x_bottom)),
+                    (slice(y_left, y_right), x_top + i),
+                    (slice(y_left, y_right), x_bottom - i))):
+        if np.size(self._original_img[line]) > 0:
+          self._img[line] = 255 * int(np.mean(self._img[line]) < 128)
+    except IndexError:
+      self._handle_box_outside_img(box)
+      return
 
   def _handle_box_outside_img(self, _: Box) -> None:
     """This method is meant to simplify the customization of the action to
     perform when a patch is outside the image in subclasses."""
 
     pass
```

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/camera_config/config_tools/box.py` & `crappy-2.0.0.dev2/src/crappy/tool/camera_config/config_tools/box.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from __future__ import annotations
 from dataclasses import dataclass
 from typing import Optional, Tuple
 
 
 @dataclass
 class Box:
-  """This class represents a box to be drawn on the image of a CameraConfig
-  GUI.
+  """This class represents a box to be drawn on top of the image of a
+  :class:`~crappy.tool.camera_config.CameraConfig` window.
 
   It can be either the box drawn when selecting a region, or the bounding box
   of a previously detected area."""
 
   x_start: Optional[int] = None
   x_end: Optional[int] = None
   y_start: Optional[int] = None
@@ -21,15 +21,15 @@
   x_disp: Optional[float] = None
   y_disp: Optional[float] = None
 
   x_centroid: Optional[float] = None
   y_centroid: Optional[float] = None
 
   def update(self, box: Box) -> None:
-    """"""
+    """Changes the coordinates of the box to those of another box."""
 
     self.x_start = box.x_start
     self.y_start = box.y_start
     self.x_end = box.x_end
     self.y_end = box.y_end
 
     self.x_disp = box.x_disp
@@ -51,23 +51,16 @@
     self.x_end = None
     self.y_start = None
     self.y_end = None
 
     self.x_centroid = None
     self.y_centroid = None
 
-  def get_patch(self) -> Tuple[int, int, int, int]:
-    """Returns the information of the box in the patch format, for
-    compatibility with other blocks."""
-
-    return (self.y_start, self.x_start, self.y_end - self.y_start,
-            self.x_end - self.x_start)
-
   def sorted(self) -> Tuple[int, int, int, int]:
-    """Returns the four sides values but sorted in the order : min x, max x,
+    """Returns the four coordinates but sorted in the order : min x, max x,
     min y, max y."""
 
     if self.no_points():
       raise ValueError("Cannot sort, some values are None !")
 
     x_top = min(self.x_start, self.x_end)
     x_bottom = max(self.x_start, self.x_end)
```

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/camera_config/config_tools/spots_boxes.py` & `crappy-2.0.0.dev2/src/crappy/tool/camera_config/config_tools/spots_boxes.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 from typing import Optional, List, Tuple
 
 from .box import Box
 
 
 @dataclass
 class SpotsBoxes:
-  """This class stores up to four instances of :class:`Box`, defining the
-  bounding boxes of the spots for video extensometry or the patches for DICVE.
+  """This class stores up to four instances of
+  :class:`~crappy.tool.camera_config.config_tools.Box`, defining the bounding
+  boxes of the spots for :class:`~crappy.blocks.VideoExtenso` or the patches
+  for :class:`~crappy.blocks.DICVE`.
 
-  It can also instantiate the Box object by parsing a list of tuples containing
-  enough information.
+  It can also instantiate the Box objects by parsing a list of tuples
+  containing enough information.
   """
 
   spot_1: Optional[Box] = None
   spot_2: Optional[Box] = None
   spot_3: Optional[Box] = None
   spot_4: Optional[Box] = None
 
@@ -62,24 +64,29 @@
       raise StopIteration
 
   def __len__(self) -> int:
     return len([spot for spot in self if spot is not None])
 
   def set_spots(self,
                 spots: List[Tuple[int, int, int, int]]) -> None:
-    """Parses a list of tuples and instantiates the corresponding Box
-    objects."""
+    """Parses a list of tuples and instantiates the corresponding
+    :class:`~crappy.tool.camera_config.config_tools.Box` objects."""
 
     for i, spot in enumerate(spots):
       self[i] = Box(x_start=spot[1], x_end=spot[1] + spot[3],
                     y_start=spot[0], y_end=spot[0] + spot[2])
 
   def save_length(self) -> None:
-    """"""
+    """Setting the :attr:`x_l0` and :attr:`y_l0` attributes based on the
+    positions of the centroids.
 
+    If only one spot is detected, setting the initial lengths to 0.
+    """
+
+    # Calculating the centroids of the spots if not already known
     for spot in self:
       if spot is not None and spot.x_centroid is None:
         min_x, max_x, min_y, max_y = spot.sorted()
         spot.x_centroid = min_x + (max_x - min_x) / 2
         spot.y_centroid = min_y + (max_y - min_y) / 2
 
     # Simply taking the distance between the extrema as the initial length
```

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/camera_config/config_tools/zoom.py` & `crappy-2.0.0.dev2/src/crappy/tool/camera_config/config_tools/zoom.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from dataclasses import dataclass
 
 
 @dataclass
 class Zoom:
   """This class stores the upper and lower limits of the image to display in
-  the configuration window.
+  the :class:`~crappy.tool.camera_config.CameraConfig` window.
 
   It also allows updating them when the user changes the zoom ratio or drags
   the image with the mouse.
   """
 
   x_low: float = 0.
   x_high: float = 1.
```

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/camera_config/dic_ve_config.py` & `crappy-2.0.0.dev2/src/crappy/tool/camera_config/dis_correl_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,136 +1,166 @@
 # coding: utf-8
 
-from typing import Optional
-from tkinter.messagebox import showerror
 import tkinter as tk
+from tkinter.messagebox import showerror
+from typing import Optional
 import numpy as np
 from io import BytesIO
 from pkg_resources import resource_string
 from time import sleep
 import logging
+from multiprocessing.queues import Queue
 
 from .camera_config_boxes import CameraConfigBoxes
-from .config_tools import Box, SpotsBoxes
+from .config_tools import Box
 from ...camera.meta_camera import Camera
-from ...camera.meta_camera.camera_setting import CameraScaleSetting
 from ..._global import OptionalModule
 
 try:
   from PIL import Image
 except (ModuleNotFoundError, ImportError):
   Image = OptionalModule("pillow")
 
 
-class DICVEConfig(CameraConfigBoxes):
-  """Class similar to :ref:`Camera Configurator` but also displaying the
-  bounding boxes of the regions defined as patches.
-
-  It is meant to be used for configuring the :ref:`DIS VE` block.
+class DISCorrelConfig(CameraConfigBoxes):
+  """Class similar to :class:`~crappy.tool.camera_config.CameraConfig` but also 
+  allowing to select the area on which the correlation will be performed.
+  
+  It relies on the :class:`~crappy.tool.camera_config.config_tools.Box` tool. 
+  It is meant to be used for configuring the :class:`~crappy.blocks.DISCorrel` 
+  Block.
   """
 
-  def __init__(self, camera: Camera, patches: SpotsBoxes) -> None:
-    """Sets the patches and initializes the parent class.
+  def __init__(self,
+               camera: Camera,
+               log_queue: Queue,
+               log_level: Optional[int],
+               patch: Box) -> None:
+    """Initializes the parent class and sets the correlation Box.
 
     Args:
-      camera: The camera object in charge of acquiring the images.
-      patches: The patches to follow for image correlation.
+      camera: The :class:`~crappy.camera.Camera` object in charge of acquiring 
+        the images.
+      log_queue: A :obj:`multiprocessing.Queue` for sending the log messages to 
+        the main :obj:`~logging.Logger`, only used in Windows.
+      log_level: The minimum logging level of the entire Crappy script, as an
+        :obj:`int`.
+      patch: The :class:`~crappy.tool.camera_config.config_tools.Box` container
+        that will save the information on the patch where to perform image
+        correlation.
     """
 
-    self._patch_size: Optional[CameraScaleSetting] = None
-
-    super().__init__(camera)
+    self._correl_box = patch
+    self._draw_correl_box = True
 
-    # Setting the patches
-    self._spots = patches
+    super().__init__(camera, log_queue, log_level)
 
-  def _add_settings(self) -> None:
-    """"""
+  @property
+  def box(self) -> Box:
+    """Returns the :class:`~crappy.tool.camera_config.config_tools.Box` object
+    containing the region of interest."""
 
-    self._patch_size = CameraScaleSetting("Patch size (px)", 2, 1024,
-                                          default=128)
-    self._add_slider_setting(self._patch_size)
+    return self._correl_box
 
-    super()._add_settings()
+  def finish(self) -> None:
+    """Method called when the user tries to close the configuration window.
 
-  def _update_settings(self) -> None:
-    """"""
+    Checks that a patch was selected on the image. If not, warns the user and
+    prevents him from exiting except with CTRL+C.
+    """
 
-    if self._patch_size.value != self._patch_size.tk_var.get():
-      self._patch_size.value = self._patch_size.tk_var.get()
-    self._patch_size.tk_var.set(self._patch_size.value)
+    if self.box.no_points():
+      self.log(logging.WARNING, "No ROI selected ! Not exiting the "
+                                "configuration window")
+      showerror('Error !',
+                message="Please select a ROI before exiting the config "
+                        "window !\nOr hit CTRL+C to exit Crappy")
+      return
 
-    super()._update_settings()
+    super().stop()
 
   def _set_bindings(self) -> None:
-    """"""
+    """Binds the left mouse button click for drawing the box on which the
+    correlation will be performed."""
 
     super()._set_bindings()
 
     self._img_canvas.bind('<ButtonPress-1>', self._start_box)
     self._img_canvas.bind('<B1-Motion>', self._extend_box)
     self._img_canvas.bind('<ButtonRelease-1>', self._stop_box)
 
-  def _extend_box(self, event: tk.Event) -> None:
-    """"""
+  def _start_box(self, event: tk.Event) -> None:
+    """Simply saves the position of the user click, and disables the display of
+    the current correl box."""
+
+    self.log(logging.DEBUG, "Starting the selection box")
 
-    super()._extend_box(event)
+    # If the mouse is on the canvas but not on the image, do nothing
+    if not self._check_event_pos(event):
+      return
+
+    self._select_box.x_start, \
+        self._select_box.y_start = self._coord_to_pix(event.x, event.y)
 
-    if not self._select_box.no_points() and self._patch_size is not None:
-      min_x, max_x, min_y, max_y = self._select_box.sorted()
-      size = self._patch_size.value
-      if max_x - min_x >= 3 * size and max_y - min_y >= 3 * size:
-        self._spots.spot_1 = Box(min_x, min_x + size,
-                                 (min_y + max_y - size) // 2,
-                                 (min_y + max_y + size) // 2)
-        self._spots.spot_2 = Box(max_x - size, max_x,
-                                 (min_y + max_y - size) // 2,
-                                 (min_y + max_y + size) // 2)
-        self._spots.spot_3 = Box((min_x + max_x - size) // 2,
-                                 (min_x + max_x + size) // 2,
-                                 min_y, min_y + size)
-        self._spots.spot_4 = Box((min_x + max_x - size) // 2,
-                                 (min_x + max_x + size) // 2,
-                                 max_y - size, max_y)
+    self._draw_correl_box = False
 
   def _stop_box(self, _: tk.Event) -> None:
-    """"""
+    """Makes sure that the selected region is valid, sets it as the new correl
+    box, and enables the display of the correl box."""
+
+    self.log(logging.DEBUG, "Ending the selection box")
+
+    # If it's just a regular click with no dragging, do nothing
+    if self._img is None or self._select_box.no_points():
+      self._select_box.reset()
+      self._draw_correl_box = True
+      return
+
+    # The sides need to be sorted before slicing numpy array
+    y_left, y_right, x_top, x_bottom = self._select_box.sorted()
+
+    # If the box is flat, resetting it
+    if y_left == y_right or x_top == x_bottom:
+      self._select_box.reset()
+      self._draw_correl_box = True
+      return
 
-    # This box is not needed anymore
+    # The new correl box is just the copy of the select box
+    self._correl_box.update(self._select_box)
     self._select_box.reset()
 
+    self._draw_correl_box = True
+
   def _on_img_resize(self, _: Optional[tk.Event] = None) -> None:
-    """Same as in the parent class except it also draws the patches on top of
-    the displayed image."""
+    """Same as in the parent class except it also draws the select box on top
+    of the displayed image."""
 
     self.log(logging.DEBUG, "The image canvas was resized")
 
-    self._draw_spots()
+    # Do not draw the correl box if the user is creating the select box
+    if self._draw_correl_box:
+      self._draw_box(self._correl_box)
+    self._draw_box(self._select_box)
+
     self._resize_img()
     self._display_img()
     self.update()
 
-  def _update_img(self, init: bool = False) -> None:
-    """Same as in the parent class except it also draws the patches on top of
-    the displayed image.
-
-    Args:
-      init: If :obj:`True`, means that the method is called during
-        :meth:`__init__` and if the image cannot be obtained it should be
-        replaced with a dummy one.
-    """
+  def _update_img(self) -> None:
+    """Same as in the parent class except it also draws the select box on top
+    of the displayed image."""
 
     self.log(logging.DEBUG, "Updating the image")
 
     ret = self._camera.get_image()
 
     # If no frame could be grabbed from the camera
     if ret is None:
       # If it's the first call, generate error image to initialize the window
-      if init:
+      if not self._n_loops:
         self.log(logging.WARNING, "Could not get an image from the camera, "
                                   "displaying an error image instead")
         ret = None, np.array(Image.open(BytesIO(resource_string(
           'crappy', 'tool/data/no_image.png'))))
       # Otherwise, just pass
       else:
         self.log(logging.DEBUG, "No image returned by the camera")
@@ -143,46 +173,28 @@
 
     if img.dtype != self.dtype:
       self.dtype = img.dtype
     if self.shape != img.shape:
       self.shape = img.shape
 
     self._cast_img(img)
-    self._draw_spots()
+    # Do not draw the correl box if the user is creating the select box
+    if self._draw_correl_box:
+      self._draw_box(self._correl_box)
+    self._draw_box(self._select_box)
     self._resize_img()
 
     self._calc_hist()
     self._resize_hist()
 
     self._display_img()
     self._display_hist()
 
     self._update_pixel_value()
 
     self.update()
 
-  def _handle_box_outside_img(self, box: Box) -> None:
-    """If a patch is outside the image, maybe the user entered a wrong value or
-    the image size has been modified. Raising an exception as the DICVE can't
-    run in this situation."""
-
-    self.log(logging.WARNING, f"The patch {box} is outside the image, "
-                              f"resetting the patches")
-    self._spots.reset()
-
-  def _stop(self) -> None:
-    """"""
-
-    if self._spots.empty():
-      self.log(logging.WARNING, "No patches selected ! Not exiting the "
-                                "configuration window")
-      showerror('Error !',
-                message="Please select patches before exiting the config "
-                        "window !\nOr hit CTRL+C to exit Crappy")
-      return
-
-    self._spots.save_length()
-    self.log(logging.INFO,
-             f"Successfully saved L0 ! L0 x : {self._spots.x_l0}, "
-             f"L0 y : {self._spots.y_l0}")
+  def _handle_box_outside_img(self, _: Box) -> None:
+    """If the correl box is outside the image, it means that the image size has
+    been modified. Simply resetting the correl box then."""
 
-    super()._stop()
+    self._correl_box.reset()
```

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/camera_config/dis_correl_config.py` & `crappy-2.0.0.dev2/src/crappy/tool/camera_config/config_tools/histogram_process.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,182 +1,159 @@
 # coding: utf-8
 
-import tkinter as tk
-from tkinter.messagebox import showerror
-from typing import Optional
 import numpy as np
-from io import BytesIO
-from pkg_resources import resource_string
-from time import sleep
+from multiprocessing import Process, current_process, get_start_method
+from multiprocessing.synchronize import Event
+from multiprocessing.connection import Connection
+from multiprocessing.queues import Queue
 import logging
+import logging.handlers
+from typing import Optional
+from functools import partial
+from time import sleep
 
-from .camera_config_boxes import CameraConfigBoxes
-from .config_tools import Box
-from ...camera.meta_camera import Camera
-from ..._global import OptionalModule
-
-try:
-  from PIL import Image
-except (ModuleNotFoundError, ImportError):
-  Image = OptionalModule("pillow")
-
-
-class DISCorrelConfig(CameraConfigBoxes):
-  """Class similar to :ref:`Camera Configurator` but also allowing to select
-  the area on which the correlation will be performed.
 
-  It is meant to be used for configuring the :ref:`DIS Correl` block.
+class HistogramProcess(Process):
+  """This class is a :obj:`multiprocessing.Process` taking an image as an input 
+  via a :obj:`multiprocessing.Pipe`, and returning the histogram of that image 
+  in another :obj:`~multiprocessing.Pipe`.
+
+  It is used by the :class:`~crappy.tool.camera_config.CameraConfig` window and 
+  its children to delegate and parallelize the calculation of the histogram. It
+  allows to gain a few frames per second on the display in the configuration
+  window.
   """
 
-  def __init__(self, camera: Camera, patch: Box) -> None:
-    """Initializes the parent class and sets the correl box."""
-
-    self._correl_box = patch
-    self._draw_correl_box = True
-
-    super().__init__(camera)
-
-  @property
-  def box(self) -> Box:
-    """Returns the Box object containing the region of interest."""
-
-    return self._correl_box
-
-  def _set_bindings(self) -> None:
-    """Binds the left mouse button click for drawing the box on which the
-    correlation will be performed."""
-
-    super()._set_bindings()
-
-    self._img_canvas.bind('<ButtonPress-1>', self._start_box)
-    self._img_canvas.bind('<B1-Motion>', self._extend_box)
-    self._img_canvas.bind('<ButtonRelease-1>', self._stop_box)
-
-  def _start_box(self, event: tk.Event) -> None:
-    """Simply saves the position of the user click, and disables the display of
-    the current correl box."""
+  def __init__(self,
+               stop_event: Event,
+               processing_event: Event,
+               img_in: Connection,
+               img_out: Connection,
+               log_level: Optional[int],
+               log_queue: Queue) -> None:
+    """Sets the arguments and initializes the parent class.
 
-    self.log(logging.DEBUG, "Starting the selection box")
-
-    # If the mouse is on the canvas but not on the image, do nothing
-    if not self._check_event_pos(event):
-      return
-
-    self._select_box.x_start, \
-        self._select_box.y_start = self._coord_to_pix(event.x, event.y)
-
-    self._draw_correl_box = False
-
-  def _stop_box(self, _: tk.Event) -> None:
-    """Makes sure that the selected region is valid, sets it as the new correl
-    box, and enables the display of the correl box."""
-
-    self.log(logging.DEBUG, "Ending the selection box")
+    Args:
+      stop_event: An :obj:`multiprocessing.Event` signaling the
+        :obj:`~multiprocessing.Process` when to stop running.
+      processing_event: An :obj:`multiprocessing.Event` set by the
+        :obj:`multiprocessing.Process` to indicate that it's currently
+        processing an image. Avoids having images to process piling up.
+      img_in: The :obj:`~multiprocessing.connection.Connection` through which 
+        the images to process are received.
+      img_out: The :obj:`~multiprocessing.connection.Connection` through which 
+        the calculated histograms are sent back.
+      log_level: The minimum logging level of the entire Crappy script, as an
+        :obj:`int`.
+      log_queue: A :obj:`multiprocessing.Queue` for sending the log messages to 
+        the main :obj:`~logging.Logger`, only used in Windows.
+    """
 
-    # If it's just a regular click with no dragging, do nothing
-    if self._img is None or self._select_box.no_points():
-      self._select_box.reset()
-      self._draw_correl_box = True
-      return
+    self._logger: Optional[logging.Logger] = None
+    self._log_level = log_level
+    self._log_queue = log_queue
+
+    super().__init__(name=f"{current_process().name}.{type(self).__name__}")
+
+    self._stop_event: Event = stop_event
+    self._processing_event: Event = processing_event
+    self._img_in: Connection = img_in
+    self._img_out: Connection = img_out
+
+  def run(self) -> None:
+    """The main method being run by the HistogramProcess.
+
+    It continuously receives images from the 
+    :class:`~crappy.tool.camera_config.CameraConfig`, calculates their 
+    histograms and returns them back as a nice image to integrate on the
+    window.
+    """
 
-    # The sides need to be sorted before slicing numpy array
-    y_left, y_right, x_top, x_bottom = self._select_box.sorted()
+    try:
+      self._processing_event.clear()
 
-    # If the box is flat, resetting it
-    if y_left == y_right or x_top == x_bottom:
-      self._select_box.reset()
-      self._draw_correl_box = True
-      return
+      # Looping until told to stop or an exception is raised
+      while not self._stop_event.is_set():
 
-    # The new correl box is just the copy of the select box
-    self._correl_box.update(self._select_box)
-    self._select_box.reset()
+        # Setting the processing event when busy processing an image
+        if self._img_in.poll():
+          self._processing_event.set()
+          # Receiving the image to process as well as additional parameters
+          while self._img_in.poll():
+            img, auto_range, low_thresh, high_thresh = self._img_in.recv()
+
+          self.log(logging.DEBUG, "Received image from CameraConfig")
+
+          # Calculating the histogram
+          hist, _ = np.histogram(img, bins=np.arange(257))
+          hist = np.repeat(hist / np.max(hist) * 80, 2)
+          hist = np.repeat(hist[np.newaxis, :], 80, axis=0)
+
+          # Making a nice image out of the calculated histogram
+          out_img = np.fromfunction(partial(self._hist_func, histo=hist),
+                                    shape=(80, 512))
+          out_img = np.flip(out_img, axis=0).astype('uint8')
+
+          # Adding vertical grey bars to indicate the limits of the auto range
+          if auto_range:
+            self.log(logging.DEBUG, "Drawing the line of the auto-range")
+            out_img[:, round(2 * low_thresh)] = 127
+            out_img[:, round(2 * high_thresh)] = 127
+
+          # Sending back the histogram
+          self._img_out.send(out_img)
+          self._processing_event.clear()
+          self.log(logging.DEBUG, "Sent the histogram back to the "
+                                  "CameraConfig")
+
+        # To avoid spamming the CPU in vain when idle
+        else:
+          sleep(0.001)
+
+      self.log(logging.INFO, "Stop event set, stopping")
+
+    except KeyboardInterrupt:
+      self.log(logging.INFO, "Caught KeyboardInterrupt, stopping")
+
+  @staticmethod
+  def _hist_func(x: np.ndarray,
+                 _: np.ndarray,
+                 histo: np.ndarray) -> np.ndarray:
+    """Function passed to the :meth:`numpy.fromfunction` method for building 
+    the histogram."""
 
-    self._draw_correl_box = True
+    return np.where(x <= histo, 0, 255)
 
-  def _on_img_resize(self, _: Optional[tk.Event] = None) -> None:
-    """Same as in the parent class except it also draws the select box on top
-    of the displayed image."""
+  def log(self, level: int, msg: str) -> None:
+    """Records log messages for the HistogramProcess.
 
-    self.log(logging.DEBUG, "The image canvas was resized")
+    Also instantiates the :obj:`~logging.Logger` when logging the first
+    message.
 
-    # Do not draw the correl box if the user is creating the select box
-    if self._draw_correl_box:
-      self._draw_box(self._correl_box)
-    self._draw_box(self._select_box)
+    Args:
+      level: An :obj:`int` indicating the logging level of the message.
+      msg: The message to log, as a :obj:`str`.
+    """
 
-    self._resize_img()
-    self._display_img()
-    self.update()
+    if self._logger is None:
+      self._set_logger()
 
-  def _update_img(self, init: bool = False) -> None:
-    """Same as in the parent class except it also draws the select box on top
-    of the displayed image.
+    self._logger.log(level, msg)
 
-    Args:
-      init: If :obj:`True`, means that the method is called during
-        :meth:`__init__` and if the image cannot be obtained it should be
-        replaced with a dummy one.
-    """
+  def _set_logger(self) -> None:
+    """Instantiates and sets up the logger for the HistogramProcess."""
 
-    self.log(logging.DEBUG, "Updating the image")
+    logger = logging.getLogger(self.name)
 
-    ret = self._camera.get_image()
+    # Disabling logging if requested
+    if self._log_level is not None:
+      logger.setLevel(self._log_level)
+    else:
+      logging.disable()
 
-    # If no frame could be grabbed from the camera
-    if ret is None:
-      # If it's the first call, generate error image to initialize the window
-      if init:
-        self.log(logging.WARNING, "Could not get an image from the camera, "
-                                  "displaying an error image instead")
-        ret = None, np.array(Image.open(BytesIO(resource_string(
-          'crappy', 'tool/data/no_image.png'))))
-      # Otherwise, just pass
-      else:
-        self.log(logging.DEBUG, "No image returned by the camera")
-        self.update()
-        sleep(0.001)
-        return
-
-    self._n_loops += 1
-    _, img = ret
-
-    if img.dtype != self.dtype:
-      self.dtype = img.dtype
-    if self.shape != img.shape:
-      self.shape = img.shape
-
-    self._cast_img(img)
-    # Do not draw the correl box if the user is creating the select box
-    if self._draw_correl_box:
-      self._draw_box(self._correl_box)
-    self._draw_box(self._select_box)
-    self._resize_img()
-
-    self._calc_hist()
-    self._resize_hist()
-
-    self._display_img()
-    self._display_hist()
-
-    self._update_pixel_value()
-
-    self.update()
-
-  def _handle_box_outside_img(self, _: Box) -> None:
-    """If the correl box is outside the image, it means that the image size has
-    been modified. Simply resetting the correl box then."""
-
-    self._correl_box.reset()
-
-  def _stop(self) -> None:
-    """"""
-
-    if self.box.no_points():
-      self.log(logging.WARNING, "No ROI selected ! Not exiting the "
-                                "configuration window")
-      showerror('Error !',
-                message="Please select a ROI before exiting the config "
-                        "window !\nOr hit CTRL+C to exit Crappy")
-      return
+    # On Windows, the messages need to be sent through a Queue for logging
+    if get_start_method() == "spawn" and self._log_level is not None:
+      queue_handler = logging.handlers.QueueHandler(self._log_queue)
+      queue_handler.setLevel(self._log_level)
+      logger.addHandler(queue_handler)
 
-    super()._stop()
+    self._logger = logger
```

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/camera_config/video_extenso_config.py` & `crappy-2.0.0.dev2/src/crappy/tool/camera_config/dic_ve_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,143 +1,171 @@
 # coding: utf-8
 
-import tkinter as tk
-from tkinter.messagebox import showerror
 from typing import Optional
+from tkinter.messagebox import showerror
+import tkinter as tk
 import numpy as np
 from io import BytesIO
 from pkg_resources import resource_string
 from time import sleep
 import logging
+from multiprocessing.queues import Queue
 
 from .camera_config_boxes import CameraConfigBoxes
-from .config_tools import Box, SpotsDetector
+from .config_tools import Box, SpotsBoxes
 from ...camera.meta_camera import Camera
+from ...camera.meta_camera.camera_setting import CameraScaleSetting
 from ..._global import OptionalModule
 
 try:
   from PIL import Image
 except (ModuleNotFoundError, ImportError):
   Image = OptionalModule("pillow")
 
 
-class VideoExtensoConfig(CameraConfigBoxes):
-  """Class similar to :ref:`Camera Configurator` but also displaying the
-  bounding boxes of the detected spots, and allowing to select the area where
-  to detect the spots by drawing a box with the left mouse button.
-
-  It is meant to be used for configuring the :ref:`Video Extenso` block.
+class DICVEConfig(CameraConfigBoxes):
+  """Class similar to :class:`~crappy.tool.camera_config.CameraConfig` but also 
+  displaying the bounding boxes of the regions defined as patches.
+  
+  It relies on the :class:`~crappy.tool.camera_config.config_tools.Box` and 
+  :class:`~crappy.tool.camera_config.config_tools.SpotsBoxes` tools. It is
+  meant to be used for configuring the :class:`~crappy.blocks.DICVE` Block.
   """
 
-  def __init__(self, camera: Camera, detector: SpotsDetector) -> None:
-    """Sets the args and initializes the parent class.
+  def __init__(self,
+               camera: Camera,
+               log_queue: Queue,
+               log_level: Optional[int],
+               patches: SpotsBoxes) -> None:
+    """Sets the patches and initializes the parent class.
 
     Args:
-      camera: The camera object in charge of acquiring the images.
+      camera: The :class:`~crappy.camera.Camera` object in charge of acquiring 
+        the images.
+      log_queue: A :obj:`multiprocessing.Queue` for sending the log messages to 
+        the main :obj:`~logging.Logger`, only used in Windows.
+      log_level: The minimum logging level of the entire Crappy script, as an
+        :obj:`int`.
+      patches: An instance of
+        :class:`~crappy.tool.camera_config.config_tools.SpotsBoxes` containing
+        the patches to follow for image correlation.
+    """
+
+    self._patch_size: Optional[CameraScaleSetting] = None
+
+    super().__init__(camera, log_queue, log_level)
+
+    # Setting the patches
+    self._spots = patches
+
+  def finish(self) -> None:
+    """Method called when the user tries to close the configuration window.
+
+    Check that patches were selected on the image. If not, warns the user and
+    prevents him from exiting except with CTRL+C. If not already done by the
+    user, also saves the initial length between the patches.
     """
 
-    super().__init__(camera)
-    self._detector = detector
-    self._spots = detector.spots
+    if self._spots.empty():
+      self.log(logging.WARNING, "No patches selected ! Not exiting the "
+                                "configuration window")
+      showerror('Error !',
+                message="Please select patches before exiting the config "
+                        "window !\nOr hit CTRL+C to exit Crappy")
+      return
+
+    self._spots.save_length()
+    self.log(logging.INFO,
+             f"Successfully saved L0 ! L0 x : {self._spots.x_l0}, "
+             f"L0 y : {self._spots.y_l0}")
+
+    super().stop()
+
+  def _add_settings(self) -> None:
+    """Same as in the parent class except it also adds a Path size setting to
+    the list of possible settings."""
+
+    self._patch_size = CameraScaleSetting("Patch size (px)", 2, 1024,
+                                          default=128)
+    self._add_slider_setting(self._patch_size)
+
+    super()._add_settings()
+
+  def _update_settings(self) -> None:
+    """Same as in the parent class except it also updates the Path size setting
+    in addition to all the other settings."""
+
+    if self._patch_size.value != self._patch_size.tk_var.get():
+      self._patch_size.value = self._patch_size.tk_var.get()
+    self._patch_size.tk_var.set(self._patch_size.value)
+
+    super()._update_settings()
 
   def _set_bindings(self) -> None:
-    """Binds the left mouse button click for drawing the box in which the spots
-    will be searched."""
+    """Binds the left mouse button click to drawing the patches on which to
+    perform the image correlation."""
 
     super()._set_bindings()
 
     self._img_canvas.bind('<ButtonPress-1>', self._start_box)
     self._img_canvas.bind('<B1-Motion>', self._extend_box)
     self._img_canvas.bind('<ButtonRelease-1>', self._stop_box)
 
-  def _create_buttons(self) -> None:
-    """Compared with the parent class, creates an extra button for saving the
-    original position of the spots."""
-
-    self._update_button = tk.Button(self._sets_frame, text="Apply Settings",
-                                    command=self._update_settings)
-    self._update_button.pack(expand=False, fill='none', ipadx=5, ipady=5,
-                             padx=5, pady=5, anchor='n', side='top')
-
-    self._update_button = tk.Button(self._sets_frame, text="Save L0",
-                                    command=self._save_l0)
-    self._update_button.pack(expand=False, fill='none', ipadx=5, ipady=5,
-                             padx=5, pady=5, anchor='n', side='top')
+  def _extend_box(self, event: tk.Event) -> None:
+    """When the user drags the selection box, updating the four patches being
+    drawn."""
+
+    super()._extend_box(event)
+
+    if not self._select_box.no_points() and self._patch_size is not None:
+      min_x, max_x, min_y, max_y = self._select_box.sorted()
+      size = self._patch_size.value
+      if max_x - min_x >= 3 * size and max_y - min_y >= 3 * size:
+        self._spots.spot_1 = Box(min_x, min_x + size,
+                                 (min_y + max_y - size) // 2,
+                                 (min_y + max_y + size) // 2)
+        self._spots.spot_2 = Box(max_x - size, max_x,
+                                 (min_y + max_y - size) // 2,
+                                 (min_y + max_y + size) // 2)
+        self._spots.spot_3 = Box((min_x + max_x - size) // 2,
+                                 (min_x + max_x + size) // 2,
+                                 min_y, min_y + size)
+        self._spots.spot_4 = Box((min_x + max_x - size) // 2,
+                                 (min_x + max_x + size) // 2,
+                                 max_y - size, max_y)
 
   def _stop_box(self, _: tk.Event) -> None:
-    """When the user releases the mouse, searches for spots in the selected
-    area and displays them if any were found."""
-
-    # If it's just a regular click with no dragging, do nothing
-    if self._img is None or self._select_box.no_points():
-      self._select_box.reset()
-      return
-
-    # The sides need to be sorted before slicing numpy array
-    y_left, y_right, x_top, x_bottom = self._select_box.sorted()
-
-    # If the box is flat, resetting it
-    if y_left == y_right or x_top == x_bottom:
-      self._select_box.reset()
-      return
-
-    # Now actually trying to detect the spots
-    try:
-      self._detector.detect_spots(self._original_img[x_top: x_bottom,
-                                                     y_left: y_right],
-                                  x_top, y_left)
-    except IndexError:
-      # Highly unlikely but always better to be careful
-      self._detector.spots.reset()
-      return
+    """Simply resets the selection box."""
 
     # This box is not needed anymore
     self._select_box.reset()
 
-  def _save_l0(self) -> None:
-    """Saves the original positions of the spots on the image."""
-
-    if self._detector.spots.empty():
-      self.log(logging.WARNING, "Cannot save L0, there are no spots !")
-    else:
-      self._detector.spots.save_length()
-      self.log(logging.INFO,
-               f"Successfully saved L0 ! L0 x : {self._detector.spots.x_l0}, "
-               f"L0 y : {self._detector.spots.y_l0}")
-
   def _on_img_resize(self, _: Optional[tk.Event] = None) -> None:
-    """Same as in the parent class except it also draws the patches and the
-    select box on top of the displayed image."""
+    """Same as in the parent class except it also draws the patches on top of
+    the displayed image."""
 
     self.log(logging.DEBUG, "The image canvas was resized")
 
-    self._draw_box(self._select_box)
     self._draw_spots()
     self._resize_img()
     self._display_img()
     self.update()
 
-  def _update_img(self, init: bool = False) -> None:
-    """Same as in the parent class except it also draws the patches and the
-    select box on top of the displayed image.
-
-    Args:
-      init: If :obj:`True`, means that the method is called during
-        :meth:`__init__` and if the image cannot be obtained it should be
-        replaced with a dummy one.
-    """
+  def _update_img(self) -> None:
+    """Same as in the parent class except it also draws the patches on top of
+    the displayed image."""
 
     self.log(logging.DEBUG, "Updating the image")
 
     ret = self._camera.get_image()
 
     # If no frame could be grabbed from the camera
     if ret is None:
       # If it's the first call, generate error image to initialize the window
-      if init:
+      if not self._n_loops:
         self.log(logging.WARNING, "Could not get an image from the camera, "
                                   "displaying an error image instead")
         ret = None, np.array(Image.open(BytesIO(resource_string(
           'crappy', 'tool/data/no_image.png'))))
       # Otherwise, just pass
       else:
         self.log(logging.DEBUG, "No image returned by the camera")
@@ -150,45 +178,27 @@
 
     if img.dtype != self.dtype:
       self.dtype = img.dtype
     if self.shape != img.shape:
       self.shape = img.shape
 
     self._cast_img(img)
-    self._draw_box(self._select_box)
     self._draw_spots()
     self._resize_img()
 
     self._calc_hist()
     self._resize_hist()
 
     self._display_img()
     self._display_hist()
 
     self._update_pixel_value()
 
     self.update()
 
-  def _handle_box_outside_img(self, _: Box) -> None:
-    """If a patch is outside the image, it means that the image size has been
-    modified. Simply resetting the spots then."""
+  def _handle_box_outside_img(self, box: Box) -> None:
+    """If a patch is outside the image, warning the user and resetting the
+    patches."""
 
+    self.log(logging.WARNING, f"The patch {box} is outside the image, "
+                              f"resetting the patches")
     self._spots.reset()
-
-  def _stop(self) -> None:
-    """"""
-
-    if self._detector.spots.empty():
-      self.log(logging.WARNING, "No spots were selected ! Not exiting the "
-                                "configuration window")
-      showerror("Error !",
-                message="Please select spots before exiting the config "
-                        "window !\nOr hit CTRL+C to exit Crappy")
-      return
-
-    if self._detector.spots.x_l0 is None or self._detector.spots.y_l0 is None:
-      self._detector.spots.save_length()
-      self.log(logging.INFO,
-               f"Successfully saved L0 ! L0 x : {self._detector.spots.x_l0}, "
-               f"L0 y : {self._detector.spots.y_l0}")
-
-    super()._stop()
```

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/data/no_image.png` & `crappy-2.0.0.dev2/src/crappy/tool/data/no_image.png`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/data/pad.png` & `crappy-2.0.0.dev2/src/crappy/tool/data/pad.png`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/data/speckle.png` & `crappy-2.0.0.dev2/src/crappy/tool/data/speckle.png`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/data/ve_markers.tif` & `crappy-2.0.0.dev2/src/crappy/tool/data/ve_markers.tif`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/ft232h/ft232h.py` & `crappy-2.0.0.dev2/src/crappy/tool/ft232h/ft232h.py`

 * *Files 6% similar despite different names*

```diff
@@ -177,34 +177,33 @@
                serial_nr: Optional[str] = None,
                i2c_speed: float = 100E3,
                spi_turbo: bool = False) -> None:
     """Checks the arguments validity, initializes the device and sets the
     locks.
 
     Args:
-      mode (:obj:`str`): The communication mode, can be :
+      mode: The communication mode as a :obj:`str`, can be :
         ::
 
           'SPI', 'I2C', 'GPIO_only', 'Write_serial_nr'
 
         GPIOs can be driven in any mode, but faster speeds are achievable in
         `GPIO_only` mode.
-      serial_nr (:obj:`str`, optional): The serial number of the FT232H to
-        drive. In `Write_serial_nr` mode, the serial number to be written.
-      i2c_speed (:obj:`str`, optional): In I2C mode, the I2C bus clock
-        frequency in Hz. Available values are :
+      serial_nr: The serial number of the FT232H to drive, as a :obj:`str`. In
+        `Write_serial_nr` mode, the serial number to be written.
+      i2c_speed: In I2C mode, the I2C bus clock frequency in Hz, as an
+        :obj:`int`. Available values are :
         ::
 
           100E3, 400E3, 1E6
 
         or any value between `10kHz` and `100kHz`. Lowering below the default
         value may solve I2C clock stretching issues on some devices.
-
-      spi_turbo (:obj:`str`, optional): Increases the achievable bus speed, but
-        may not work with some devices.
+      spi_turbo: If :obj:`True`, increases the achievable bus speed in SPI
+        mode, but may not work with some devices.
 
     Note:
       - **CS pin**:
         The CS pin for selecting SPI devices is always `D3`. This pin is
         reserved and cannot be used as a GPIO. If you want to drive the CS line
         manually, it is possible not to drive the CS pin by setting the SPI
         parameter :attr:`no_cs` to :obj:`True` and to drive the CS line from a
@@ -448,46 +447,53 @@
 
     # Disable adaptative clock
     self._write_data(bytearray([False and
                                 ft232h_cmds['enable_clk_adaptative'] or
                                 ft232h_cmds['disable_clk_adaptative']]))
 
   def log(self, level: int, msg: str) -> None:
-    """"""
+    """Wrapper for logging messages.
+
+    Also initializes the Logger on the first message.
+
+    Args:
+      level: The logging level of the message, as an :obj:`int`.
+      msg: The message to log, as a :obj:`str`.
+    """
 
     if self._logger is None:
       self._logger = logging.getLogger(f"{current_process().name}."
                                        f"{type(self).__name__}")
 
     self._logger.log(level, msg)
 
   @staticmethod
   def _compute_delay_cycles(value: float) -> int:
     """Approximates the number of clock cycles over a given delay.
 
     Args:
-      value (:obj:`float`): delay (in seconds)
+      value: The delay in seconds, as a :obj:`float`.
 
     Returns:
-      Number of clock cycles
+      The number of clock cycles, as an :obj:`int`.
     """
 
     bit_delay = ft232h_mpsse_bit_delay
     return max(1, int((value + bit_delay) / bit_delay))
 
   def _set_latency_timer(self, latency: int) -> None:
     """Sets the latency timer.
 
     Sets the latency timer, i.e. the delay the chip waits before sending the
     data stored in the buffer to the host. Not applicable when a send
     immediate command is issued, in which case the buffered data is returned
     immediately.
 
     Args:
-      latency (:obj:`int`): latency (in milliseconds)
+      latency: The latency in milliseconds, as an :obj:`int`.
     """
 
     self.log(logging.DEBUG, f"Setting the latency timer to {latency}")
 
     if not ft232h_latency['min'] <= latency <= ft232h_latency['max']:
       raise ValueError("Latency out of range")
     if self._ctrl_transfer_out(ft232h_sio_req['set_latency_timer'], latency):
@@ -497,18 +503,18 @@
     """Sets the bus frequency.
 
     Sets the FT232H clock divisor value, according to the desired bus
     frequency. The actual bus frequency is then as close as possible to the
     desired value, but may still be slightly different.
 
     Args:
-      frequency (:obj:`float`): Desired bus frequency (in Hz)
+      frequency: The desired bus frequency in Hz, as a :obj:`float`.
 
     Returns:
-      Actual bus frequency
+      The actual bus frequency, as a :obj:`float`.
     """
 
     self.log(logging.DEBUG, f"Setting the clock frequency to {frequency}")
 
     # Calculate base speed clock divider
     divcode = ft232h_cmds['enable_clk_div5']
     divisor = int((ft232h_clock['base'] + frequency / 2) / frequency) - 1
@@ -546,16 +552,16 @@
 
     return actual_freq
 
   def _set_bitmode(self, bitmask: int, mode: BitMode) -> None:
     """Sets the bitbang mode.
 
     Args:
-      bitmask (:obj:`int`): Mask for choosing the driven GPIOs.
-      mode (:class:`BitMode`): Bitbang mode to be set.
+      bitmask: Mask for choosing the driven GPIOs.
+      mode: The bitbang mode to be set.
     """
 
     mask = sum(FT232H.BitMode)
     value = (bitmask & 0xff) | ((mode.value & mask) << 8)
     if self._ctrl_transfer_out(ft232h_sio_req['set_bitmode'], value):
       raise IOError('Unable to set bitmode')
 
@@ -586,17 +592,17 @@
   def _ctrl_transfer_out(self,
                          reqtype: int,
                          value: int,
                          data: bytes = b'') -> int:
     """Sends a control message to the device.
 
     Args:
-      reqtype (:obj:`int`): bmRequest
-      value (:obj:`int`): wValue
-      data (:obj:`bytes`): payload
+      reqtype: bmRequest
+      value: wValue
+      data: payload
 
     Returns:
       Number of bytes actually written
     """
 
     try:
       self.log(logging.DEBUG,
@@ -613,15 +619,16 @@
     """(Over)Writes the serial number.
 
     Writes the desired serial number to the EEPROM. It is then accessible to
     USB commands as a string descriptor. Also sets the manufacturer and
     product string descriptors.
 
     Args:
-      serial_number (:obj:`str`): Serial number to be written in the EEPROM
+      serial_number: Serial number to be written in the EEPROM, as a
+        :obj:`str`.
     """
 
     if not isinstance(serial_number, str):
       serial_number = str(serial_number)
     if any(char in serial_number for char in ':/'):
       raise ValueError("Invalid character : or / in serial number")
 
@@ -755,16 +762,16 @@
 
     Reads data from the FTDI interface. The data buffer is rebuilt from
     chunk-sized blocks received over the USB bus. The FTDI device always sends
     internal status bytes, which are stripped out as not part of the data
     payload.
 
     Args:
-      size (:obj:`int`): The number of bytes to receive from the device
-      attempt (:obj:`int`): Attempt cycle count
+      size: The number of bytes to receive from the device, as an :obj:`int`.
+      attempt: Attempt cycle count
       request_gen: A callable that takes the number of bytes read and expects a
         bytes buffer to send back to the remote device. This is only useful to
         perform optimized/continuous transfer from a slave device.
 
     Returns:
       Payload bytes
     """
@@ -925,15 +932,15 @@
         self._clk_hi_data_lo * self._ck_su_sto + \
         self._idle * self._ck_idle
 
   def _do_prolog(self, i2caddress: int) -> None:
     """Sends the MPSSE commands for starting an I2C transaction.
 
     Args:
-      i2caddress (:obj:`int`): I2C address of the slave
+      i2caddress: I2C address of the slave
     """
 
     if i2caddress is None:
       return
     cmd = bytearray(self._idle * self._ck_delay)
     cmd.extend(self._start)
     cmd.extend((ft232h_cmds['write_bytes_NVE_MSB'], 0, 0))
@@ -943,29 +950,28 @@
     except IOError:
       raise
 
   def _do_write(self, out: list) -> None:
     """Sends the MPSSE commands for writing bytes to an I2C slave.
 
     Args:
-      out (:obj:`list`): List of bytes to write
+      out: List of bytes to write
     """
 
     if not isinstance(out, bytearray):
       out = bytearray(out)
     if not out:
       return
     for byte in out:
       cmd = bytearray((ft232h_cmds['write_bytes_NVE_MSB'], 0, 0))
       cmd.append(byte)
       self._send_check_ack(cmd)
 
   def _do_read(self, readlen: int) -> bytearray:
-    """
-    Sends the MPSSE commands for reading bytes from an I2C slave, and then
+    """Sends the MPSSE commands for reading bytes from an I2C slave, and then
     returns these bytes.
 
     Args:
       readlen: Number of bytes to read
 
     Returns: Read bytes as a bytearray
     """
@@ -1029,15 +1035,15 @@
     return bytearray(b''.join(chunks))
 
   def _send_check_ack(self, cmd: bytearray) -> None:
     """Actually sends the MPSSE commands generated by :meth:`_do_prolog` and
     :meth:`_do_write` methods, and checks whether the slave ACKs it.
 
     Args:
-      cmd (:obj:`bytearray`): The MPSSE commands to send
+      cmd: The MPSSE commands to send
     """
 
     # SCL low, SDA high-Z
     cmd.extend(self._clk_lo_data_hi)
     # read SDA (ack from slave)
     cmd.extend((ft232h_cmds['read_bits_PVE_MSB'], 0))
     cmd.extend((ft232h_cmds['send_immediate'],))
@@ -1051,18 +1057,17 @@
   def _write_i2c(self,
                  address: int,
                  out: list,
                  stop: bool = True) -> None:
     """Writes bytes to an I2C slave.
 
     Args:
-      address (:obj:`int`): I2C address of the slave
-      out (:obj:`list`): List of bytes to send
-      stop (:obj:`bool`, optional): Should the stop condition be sent at the
-        end of the message ?
+      address: I2C address of the slave
+      out: List of bytes to send
+      stop: Should the stop condition be sent at the end of the message ?
     """
 
     i2caddress = (address << 1) & 0xFF
     retries = self._retry_count
     while True:
       try:
         self._do_prolog(i2caddress)
@@ -1079,18 +1084,17 @@
   def _read_i2c(self,
                 address: int,
                 length: int,
                 stop: bool = True) -> bytearray:
     """Reads bytes from an I2C slave.
 
     Args:
-      address (:obj:`int`): I2C address of the slave
-      length (:obj:`int`): Number of bytes to read
-      stop (:obj:`bool`, optional): Should the stop condition be sent at the
-        end of the message ?
+      address: I2C address of the slave
+      length: Number of bytes to read
+      stop: Should the stop condition be sent at the end of the message ?
     """
 
     i2caddress = (address << 1) & 0xFF
     retries = self._retry_count
     while True:
       try:
         self._do_prolog(i2caddress | 0x01)
@@ -1110,17 +1114,17 @@
                     address: int,
                     out: list,
                     readlen: int = 0) -> bytearray:
     """Writes bytes to an I2C slave, and then reads a given number of bytes
     from this same slave.
 
     Args:
-      address (:obj:`int`): I2C address of the slave
-      out (:obj:`list`): List of bytes to send
-      readlen (:obj:`int`): Number of bytes to read
+      address: I2C address of the slave
+      out: List of bytes to send
+      readlen: Number of bytes to read
 
     Returns:
       Read bytes as a bytearray
     """
 
     if readlen < 1:
       raise IOError('Nothing to read')
@@ -1147,16 +1151,16 @@
       finally:
         self._write_data(bytearray(self._stop))
 
   def write_byte(self, i2c_addr: int, value: int) -> None:
     """Writes a single byte to an I2C slave, in register 0.
 
     Args:
-      i2c_addr (:obj:`int`): I2C address of the slave
-      value (:obj:`int`): The value to write
+      i2c_addr: The I2C address of the slave, as an :obj:`int`.
+      value: The value to write, as an :obj:`int`.
     """
 
     self.log(logging.DEBUG, f"Requested I2C byte write with value {value} to "
                             f"address {i2c_addr}")
 
     self.write_i2c_block_data(i2c_addr=i2c_addr,
                               register=0x00,
@@ -1165,17 +1169,17 @@
   def write_byte_data(self,
                       i2c_addr: int,
                       register: int,
                       value: int) -> None:
     """Writes a single byte to an I2C slave, in the specified register.
 
     Args:
-      i2c_addr (:obj:`int`): I2C address of the slave
-      register (:obj:`int`): Index of the register to be written
-      value (:obj:`int`): The value to write
+      i2c_addr: The I2C address of the slave, as an :obj:`int`.
+      register: The index of the register to be written, as an :obj:`int`.
+      value: The value to write, as an :obj:`int`.
     """
 
     self.log(logging.DEBUG, f"Requested I2C byte write with value {value} to "
                             f"register {register} at address {i2c_addr}")
 
     self.write_i2c_block_data(i2c_addr=i2c_addr,
                               register=register,
@@ -1188,17 +1192,18 @@
     """Writes 2 bytes to an I2C slave from a single int value, starting at the
     specified register.
 
     Depending on the size of the registers, the next register may be written as
     well.
 
     Args:
-      i2c_addr (:obj:`int`): I2C address of the slave
-      register (:obj:`int`): Index of the first register to be written
-      value (:obj:`int`): The value to write
+      i2c_addr: The I2C address of the slave, as an :obj:`int`.
+      register: The index of the first register to be written, as an
+        :obj:`int`.
+      value: The value to write, as an :obj:`int`.
     """
 
     self.log(logging.DEBUG, f"Requested I2C word write with value {value} to "
                             f"register {register} at address {i2c_addr}")
 
     self.write_i2c_block_data(i2c_addr=i2c_addr,
                               register=register,
@@ -1207,17 +1212,18 @@
   def write_block_data(self,
                        i2c_addr: int,
                        register: int,
                        data: list) -> None:
     """Actually calls :meth:`write_i2c_block_data`.
 
     Args:
-      i2c_addr (:obj:`int`): I2C address of the slave
-      register (:obj:`int`): Index of the first register to be written
-      data (:obj:`list`): List of bytes to write
+      i2c_addr: The I2C address of the slave, as an :obj:`int`.
+      register: The index of the first register to be written, as an
+        :obj:`int`.
+      data: A :obj:`list` of bytes to write.
     """
 
     self.log(logging.DEBUG, f"Requested I2C block write with data {data} to "
                             f"register {register} at address {i2c_addr}")
 
     self.write_i2c_block_data(i2c_addr=i2c_addr,
                               register=register,
@@ -1227,17 +1233,18 @@
                            i2c_addr: int,
                            register: int,
                            data: list) -> None:
     """Writes bytes from a :obj:`list` to an I2C slave, starting at the
     specified register.
 
     Args:
-      i2c_addr (:obj:`int`): I2C address of the slave
-      register (:obj:`int`): Index of the first register to be written
-      data (:obj:`list`): List of bytes to write
+      i2c_addr: The I2C address of the slave, as an :obj:`int`.
+      register: The index of the first register to be written, as an
+        :obj:`int`.
+      data: A :obj:`list` of bytes to write.
     """
 
     self.log(logging.DEBUG, f"Requested I2C block write with data {data} to "
                             f"register {register} at address {i2c_addr}")
 
     if self._ft232h_mode != 'I2C':
       raise ValueError("Method only available in I2C mode")
@@ -1247,15 +1254,15 @@
     self._write_i2c(address=i2c_addr,
                     out=[register] + data)
 
   def read_byte(self, i2c_addr: int) -> int:
     """Reads a single byte from an I2C slave, from the register `0`.
 
     Args:
-      i2c_addr (:obj:`int`): I2C address of the slave
+      i2c_addr: The I2C address of the slave, as an :obj:`int`.
 
     Returns:
       Value of the read register
     """
 
     self.log(logging.DEBUG, f"Requested I2C byte read at address {i2c_addr}")
 
@@ -1267,16 +1274,16 @@
       self.log(logging.ERROR, "No data to read from USB device")
       raise
 
   def read_byte_data(self, i2c_addr: int, register: int) -> int:
     """Reads a single byte from an I2C slave, from the specified register.
 
     Args:
-      i2c_addr (:obj:`int`): I2C address of the slave
-      register (:obj:`int`): Index of the register to be read
+      i2c_addr: The I2C address of the slave, as an :obj:`int`.
+      register: The index of the register to be read, as an :obj:`int`.
 
     Returns:
       Value of the read register
     """
 
     self.log(logging.DEBUG, f"Requested I2C byte read from register {register}"
                             f" at address {i2c_addr}")
@@ -1290,16 +1297,16 @@
       raise
 
   def read_word_data(self, i2c_addr: int, register: int) -> int:
     """Reads 2 bytes from an I2C slave, starting at the specified register, and
     returns them as one single value.
 
     Args:
-      i2c_addr (:obj:`int`): I2C address of the slave
-      register (:obj:`int`): Index of the first register to be read
+      i2c_addr: The I2C address of the slave, as an :obj:`int`.
+      register: The index of the first register to be read, as an :obj:`int`.
 
     Returns:
       Value of the read registers
     """
 
     self.log(logging.DEBUG, f"Requested I2C word read from register {register}"
                             f" at address {i2c_addr}")
@@ -1317,17 +1324,17 @@
                           i2c_addr: int,
                           register: int,
                           length: int) -> List[int]:
     """Reads a given number of bytes from an I2C slave, starting at the
     specified register.
 
     Args:
-      i2c_addr (:obj:`int`): I2C address of the slave
-      register (:obj:`int`): Index of the first register to be read
-      length (:obj:`int`): Number of bytes to read
+      i2c_addr: The I2C address of the slave, as an :obj:`int`.
+      register: The index of the first register to be read, as an :obj:`int`.
+      length: The number of bytes to read, as an :obj:`int`.
 
     Returns:
       Values of read registers as a :obj:`list`
     """
 
     self.log(logging.DEBUG, f"Requested I2C block read of length {length} from"
                             f" register {register} at address {i2c_addr}")
@@ -1356,16 +1363,16 @@
   def i2c_rdwr(self, *i2c_msgs: I2CMessage) -> None:
     """Exchanges messages with a slave that doesn't feature registers.
 
     A start condition is sent at the beginning of each transaction, but only
     one stop condition is sent after the last transaction.
 
     Args:
-      *i2c_msgs: Messages to exchange with the slave. They are either read or
-        write messages.
+      *i2c_msgs: One or several :class:`~crappy.tool.ft232h.I2CMessage` to
+        exchange with the slave. They are either read or write messages.
     """
 
     self.log(logging.DEBUG, "Requested I2C readwrite")
 
     nr = len(i2c_msgs)
     for i, msg in enumerate(i2c_msgs):
       if msg.type == 'w':
@@ -1556,32 +1563,35 @@
       raise TypeError("threewire should be either True or False")
     if value:
       raise ValueError("threewire mode not implemented")
 
     self.log(logging.DEBUG, f"Set SPI threewire to {value}")
     self._threewire = value
 
-  def _exchange_spi(self, readlen: int, out: list, start: bool,
-                    stop: bool, duplex: bool) -> bytes:
+  def _exchange_spi(self,
+                    readlen: int,
+                    out: list,
+                    start: bool,
+                    stop: bool,
+                    duplex: bool) -> bytes:
     """Exchanges bytes with an SPI slave.
 
     Can read and/or write data, in a sequential or simultaneous way. Also
     manages the CS line.
 
     Args:
-      readlen (:obj:`int`): Number of bytes to read. If 0, no reading is
-        performed.
-      out (:obj:`list`): List of bytes to write. If empty, no writing is
-        performed.
-      start (:obj:`bool`): If :obj:`False`, the CS line is not driven before
-        exchanging data, and remains in its previous state.
-      stop (:obj:`bool`): If :obj:`False`, the CS line is not driven after
-        exchanging data, and remains in its previous state.
-      duplex (:obj:`int`): If :obj:`True`, the data is read and written
-        simultaneously. If :obj:`False`, writes then reads in a sequential way.
+      readlen: The umber of bytes to read, as an :obj:`int`. If 0, no reading
+        is performed.
+      out: A :obj:`list` of bytes to write. If empty, no writing is performed.
+      start: If :obj:`False`, the CS line is not driven before exchanging data,
+        and remains in its previous state.
+      stop: If :obj:`False`, the CS line is not driven after exchanging data,
+        and remains in its previous state.
+      duplex: If :obj:`True`, the data is read and written simultaneously. If
+        :obj:`False`, writes then reads in a sequential way.
 
     Returns:
       Read data as bytes
     """
 
     if len(out) > ft232h_max_payload:
       raise IOError("Output payload is too large")
@@ -1732,19 +1742,19 @@
   def readbytes(self,
                 len: int,
                 start: bool = True,
                 stop: bool = True) -> List[int]:
     """Reads the specified number of bytes from an SPI slave.
 
     Args:
-      len (:obj:`int`): Number of bytes to read
-      start (:obj:`bool`): If :obj:`False`, the CS line is not driven before
-        reading data, and remains in its previous state.
-      stop (:obj:`bool`): If :obj:`False`, the CS line is not driven after
-        reading data, and remains in its previous state.
+      len: The number of bytes to read, as an :obj:`int`.
+      start: If :obj:`False`, the CS line is not driven before reading data,
+        and remains in its previous state.
+      stop: If :obj:`False`, the CS line is not driven after reading data, and
+        remains in its previous state.
 
     Returns:
       List of read bytes
     """
 
     self.log(logging.DEBUG, f"Requested SPI bytes read of length {len}")
 
@@ -1759,19 +1769,19 @@
   def writebytes(self,
                  values: list,
                  start: bool = True,
                  stop: bool = True) -> None:
     """Write bytes from a list to an SPI slave.
 
     Args:
-      values (:obj:`list`): List of bytes to write
-      start (:obj:`bool`): If :obj:`False`, the CS line is not driven before
-        reading data, and remains in its previous state.
-      stop (:obj:`bool`): If :obj:`False`, the CS line is not driven after
-        reading data, and remains in its previous state.
+      values: A :obj:list` of bytes to write
+      start: If :obj:`False`, the CS line is not driven before reading data,
+        and remains in its previous state.
+      stop: If :obj:`False`, the CS line is not driven after reading data, and
+        remains in its previous state.
     """
 
     self.log(logging.DEBUG, f"Requested SPI bytes write with values {values}")
 
     if self._ft232h_mode != 'SPI':
       raise ValueError("Method only available in SPI mode")
     self._exchange_spi(readlen=0,
@@ -1801,23 +1811,23 @@
            stop: bool = True) -> List[int]:
     """Simultaneously reads and write bytes to an SPI slave.
 
     The number of bytes to read is equal to the number of bytes in the write
     buffer.
 
     Args:
-      values (:obj:`list`): List of bytes to write
-      speed (:obj:`float`): Sets the bus clock frequency before issuing the
-        command (in Hz)
-      delay (:obj:`float`): Not implemented, should be 0.0
-      bits (:obj:`int`):  Not implemented, should be 8
-      start (:obj:`bool`): If :obj:`False`, the CS line is not driven before
-        reading data, and remains in its previous state.
-      stop (:obj:`bool`): If :obj:`False`, the CS line is not driven after
-        reading data, and remains in its previous state.
+      values: A :obj:list` of bytes to write.
+      speed: Sets the bus clock frequency in Hz before issuing the command, as
+        a :obj:`float`.
+      delay: Not implemented, should be 0.0
+      bits:  Not implemented, should be 8
+      start: If :obj:`False`, the CS line is not driven before reading data,
+        and remains in its previous state.
+      stop: If :obj:`False`, the CS line is not driven after reading data, and
+        remains in its previous state.
 
     Returns:
       List of read bytes
     """
 
     self.log(logging.DEBUG, f"Requested SPI xfer with values {values}")
 
@@ -1931,15 +1941,15 @@
     value, = unpack(fmt, data)
     return value
 
   def get_gpio(self, gpio_str: str) -> bool:
     """Reads the 3.3V-logic voltage value of the specified pin.
 
     Args:
-      gpio_str (:obj:`str`): Name of the GPIO to be read
+      gpio_str: The name of the GPIO to be read, as a :obj:`str`.
 
     Returns:
       3.3V-logic value corresponding to the input voltage
     """
 
     self.log(logging.DEBUG, f"Requested GPIO value reading for {gpio_str}")
 
@@ -1956,16 +1966,16 @@
 
     return bool(self._read_gpio_raw() & gpio_bit)
 
   def set_gpio(self, gpio_str: str, value: int) -> None:
     """Sets the specified GPIO as an output and sets its output value.
 
     Args:
-      gpio_str (:obj:`str`): Name of the GPIO to be set
-      value (:obj:`int`): 1 for setting the GPIO high, 0 for setting it low
+      gpio_str: The name of the GPIO to be set, as a :obj:`str`.
+      value: 1 for setting the GPIO high, 0 for setting it low.
     """
 
     self.log(logging.DEBUG, f"Requested GPIO value writing to {value} "
                             f"for {gpio_str}")
 
     if value not in [0, 1]:
       raise ValueError("value should be either 0 or 1")
```

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/ft232h/ft232h_server.py` & `crappy-2.0.0.dev2/src/crappy/tool/ft232h/ft232h_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,36 +95,50 @@
 
 ft232h_i2c_speed = {100E3: ft232h_i2c_timings(4.0E-6, 4.7E-6, 4.0E-6, 4.7E-6),
                     400E3: ft232h_i2c_timings(0.6E-6, 0.6E-6, 0.6E-6, 1.3E-6),
                     1E6: ft232h_i2c_timings(0.26E-6, 0.26E-6, 0.26E-6, 0.5E-6)}
 
 
 class DelayedKeyboardInterrupt:
-  """"""
+  """This class implements a context manager for temporarily disabling the
+  :exc:`KeyboardInterrupt` and storing any exception received in the meantime.
+
+  It is meant to avoid having a I2C or SPI communication interrupted, which 
+  could cause devices to bug and not be able to properly finish.
+  """
 
   def __enter__(self) -> None:
+    """Enters the context and sets :meth:`_handler` as the new handler for
+    SIGINT signals."""
+
     self._signal_received = None
     self._prev_handler = signal.signal(signal.SIGINT, self._handler)
 
   def __exit__(self, _, __, ___) -> None:
+    """Exits the context, sets the previous handler back, and handles any
+    SIGINT signal received while in the context."""
+
     signal.signal(signal.SIGINT, self._prev_handler)
     if self._signal_received is not None:
       self._prev_handler(*self._signal_received)
 
   def _handler(self, sig, frame) -> None:
+    """Handler that just stores the received SIGINT while in the context."""
+
     self._signal_received = (sig, frame)
 
 
 class FT232HServer(FT232H):
   """A class for controlling FTDI's USB to Serial FT232H.
 
-  This class is very similar to the :class:`ft232h` except it doesn't
-  directly instantiate the USB device nor send commands to it directly.
-  Instead, the commands are sent to a USB server managing communication with
-  the different FT232H devices.
+  This class is very similar to the :class:`~crappy.tool.ft232h.FT232H` except 
+  it doesn't directly instantiate the USB device nor send commands to it 
+  directly. Instead, the commands are sent to a 
+  :class:`~crappy.tool.ft232h.USBServer` managing communication with the FT232H 
+  device(s).
 
   Communication in SPI and I2C are implemented, along with GPIO control. The
   name of the methods for SPI and I2C communication are those of :mod:`smbus`
   and :mod:`spidev` libraries, in order to facilitate the use and the
   integration in a multi-backend environment. This class also allows to write a
   USB serial number in the EEPROM, as there's no default serial number on the
   chip.
@@ -166,45 +180,50 @@
                shared_lock: RLock,
                serial_nr: Optional[str] = None,
                i2c_speed: float = 100E3,
                spi_turbo: bool = False) -> None:
     """Checks the argument validity and initializes the device.
 
     Args:
-      mode: The communication mode, can be :
+      mode: The communication mode as a :obj:`str`, can be :
         ::
 
           'SPI', 'I2C', 'GPIO_only', 'Write_serial_nr'
 
         GPIOs can be driven in any mode, but faster speeds are achievable in
         `GPIO_only` mode.
-      block_index: The index the block driving this ft232h_server instance has
-        been assigned.
-      current_block:
+      block_index: The index the :class:`~crappy.blocks.Block` driving this 
+        FT232HServer instance has been assigned by the 
+        :class:`~crappy.tool.ft232h.USBServer`, as an :obj:`int`.
+      current_block: The handle to a shared :obj:`multiprocessing.Value` 
+        indicating which :class:`~crappy.blocks.Block` can currently
+        communicate with the :class:`~crappy.tool.ft232h.USBServer`.
       command_file: A file in which the current command to be executed by the
         USB server is written.
       answer_file: A file in which the answer to the current command is
         written.
-      block_lock: A lock assigned to this block only, for signaling the USB
-        server when the command has been written in the command_file.
-      shared_lock: A lock common to all the blocks that allows the one block
-        holding it to communicate with the USB server.
-      serial_nr (:obj:`str`, optional): The serial number of the FT232H to
-        drive. In `Write_serial_nr` mode, the serial number to be written.
+      block_lock: A :obj:`multiprocessing.Lock` assigned to this 
+        :class:`~crappy.blocks.Block` only, for signaling the 
+        :class:`~crappy.tool.ft232h.USBServer` when the command has been 
+        written in the command_file.
+      shared_lock: A :obj:`multiprocessing.Lock` common to all the 
+        :class:`~crappy.blocks.Block` that allows the one Block holding it to 
+        communicate with the :class:`~crappy.tool.ft232h.USBServer`.
+      serial_nr: The serial number of the FT232H to drive, as a :obj:`str`. In
+        `Write_serial_nr` mode, the serial number to be written.
       i2c_speed: In I2C mode, the I2C bus clock frequency in Hz. Available
         values are :
         ::
 
           100E3, 400E3, 1E6
 
         or any value between `10kHz` and `100kHz`. Lowering below the default
         value may solve I2C clock stretching issues on some devices.
-
-      spi_turbo: Increases the achievable bus speed, but may not work with some
-        devices.
+      spi_turbo: Increases the achievable bus speed in SPI mode, but may not
+        work with some devices.
 
     Note:
       - **CS pin**:
         The CS pin for selecting SPI devices is always `D3`. This pin is
         reserved and cannot be used as a GPIO. If you want to drive the CS line
         manually, it is possible not to drive the CS pin by setting the SPI
         parameter :attr:`no_cs` to :obj:`True` and to drive the CS line from a
@@ -566,17 +585,17 @@
   def _ctrl_transfer_out(self,
                          reqtype: int,
                          value: int,
                          data: bytes = b'') -> int:
     """Sends a control message to the device.
 
     Args:
-      reqtype (:obj:`int`): bmRequest
-      value (:obj:`int`): wValue
-      data (:obj:`bytes`): payload
+      reqtype: bmRequest
+      value: wValue
+      data: payload
 
     Returns:
       Number of bytes actually written
     """
 
     try:
       self.log(logging.DEBUG,
@@ -592,24 +611,27 @@
   def _read_data_bytes(self,
                        size: int,
                        attempt: int = 2,
                        request_gen: Optional[
                          Callable[[int], Union[bytearray,
                                                bytes]]] = None) -> bytes:
     """Reads data from the FT232H.
+
     Reads data from the FTDI interface. The data buffer is rebuilt from
     chunk-sized blocks received over the USB bus. The FTDI device always sends
     internal status bytes, which are stripped out as not part of the data
     payload.
+
     Args:
-      size (:obj:`int`): The number of bytes to receive from the device
-      attempt (:obj:`int`): Attempt cycle count
+      size: The number of bytes to receive from the device
+      attempt: Attempt cycle count
       request_gen: A callable that takes the number of bytes read and expects a
         bytes buffer to send back to the remote device. This is only useful to
         perform optimized/continuous transfer from a slave device.
+
     Returns:
       Payload bytes
     """
 
     # Packet size sanity check
     if not self._max_packet_size:
       raise ValueError("max_packet_size is bogus")
@@ -709,15 +731,16 @@
     """(Over)Writes the serial number.
 
     Writes the desired serial number to the EEPROM. It is then accessible to
     USB commands as a string descriptor. Also sets the manufacturer and
     product string descriptors.
 
     Args:
-      serial_number (:obj:`str`): Serial number to be written in the EEPROM
+      serial_number: Serial number to be written in the EEPROM, as a
+        :obj:`str`.
     """
 
     if not isinstance(serial_number, str):
       serial_number = str(serial_number)
     if any(char in serial_number for char in ':/'):
       raise ValueError("Invalid character : or / in serial number")
 
@@ -861,15 +884,25 @@
       self._send_server(['dispose_resources'])
 
     self._send_server(['farewell'])
 
   @staticmethod
   @contextmanager
   def acquire_timeout(lock: RLock, timeout: float) -> bool:
-    """"""
+    """Short context manager for acquiring a :obj:`multiprocessing.Lock` with a
+    specified timeout.
+
+    Args:
+      lock: The lock to acquire.
+      timeout: The timeout for acquiring the Lock, as a :obj:`float`.
+
+    Returns:
+      :obj:`True` if the Lock was successfully acquired, :obj:`False`
+      otherwise.
+    """
 
     ret = False
     try:
       ret = lock.acquire(timeout=timeout)
       yield ret
     finally:
       if ret:
```

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/ft232h/i2c_message.py` & `crappy-2.0.0.dev2/src/crappy/tool/ft232h/i2c_message.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 # coding: utf-8
 
 from __future__ import annotations
 from typing import Optional, List
 
 
 class I2CMessage:
-  """Class that mimics the :obj:`i2c_msg` class of the :mod:`smbus2` module."""
+  """Class that mimics the :class:`smbus2.i2c_msg` class.
+
+  It is used for communication with the
+  :class:`~crappy.tool.ft232h.FT232HServer`, only by the
+  :class:`~crappy.inout.MPRLS` InOut.
+  """
 
   def __init__(self,
                type_: str,
                address: int,
                length: Optional[int] = None,
                buf: Optional[list] = None) -> None:
-    """Simply sets the attributes of the class, that characterise the i2c
+    """Simply sets the attributes of the class, that characterizes the I2C
     message.
 
     Args:
-      type_ (:obj:`str`): Either a read (`'r'`) or a write (`'w'`) message
-      address (:obj:`int`): The address of the I2C slave.
-      length (:obj:`int`, optional): For a read message, the number of bytes to
-        read.
-      buf (:obj:`list`, optional): For a write message, the list of bytes to be
-        written.
+      type_: Either a read (`'r'`) or a write (`'w'`) message
+      address: The address of the I2C slave, as an :obj:`int`.
+      length: For a read message, the number of bytes to read as an :obj:`int`.
+      buf: For a write message, the :obj:`list` of :obj:`bytes` to be written.
     """
 
     if type_ not in ['r', 'w']:
       raise ValueError("type_ should be either 'r' or 'w' !")
 
     self.type = type_
     self.addr = address
     self.len = length if length else 0
     self.buf = buf if buf else []
 
   @classmethod
   def read(cls, address: int, length: int) -> I2CMessage:
-    """Instantiates an :class:`i2c_msg_ft232h` object for reading bytes.
+    """Instantiates an :class:`I2CMessage` object for reading bytes.
 
     Args:
-      address (:obj:`int`): The address of the I2C slave.
-      length (:obj:`int`): The number of bytes to read.
+      address: The address of the I2C slave, as an :obj:`int`.
+      length: The number of bytes to read, as an :obj:`int`.
     """
 
     return cls(type_='r', address=address, length=length)
 
   @classmethod
   def write(cls, address: int, buf: list) -> I2CMessage:
-    """Instantiates an :class:`i2c_msg_ft232h` object for writing bytes.
+    """Instantiates an :class:`I2CMessage` object for writing bytes.
 
     Args:
-      address (:obj:`int`): The address of the I2C slave.
-      buf (:obj:`list`): The list of bytes to be written.
+      address: The address of the I2C slave, as an :obj:`int`.
+      buf: The :obj:`list` of :obj:`bytes` to be written.
     """
 
     return cls(type_='w', address=address, buf=buf)
 
   @property
   def addr(self) -> int:
     """The address of the I2C slave."""
```

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/ft232h/usb_server.py` & `crappy-2.0.0.dev2/src/crappy/tool/ft232h/usb_server.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,25 +28,40 @@
                     FileIO, multiprocessing.synchronize.RLock,
                     Synchronized]
 
 
 @dataclass
 class BlockObjects:
   """This class stores all the objects specific to a single Block, in order to
-  easily pass them to the USB server process."""
+  easily pass them to the :class:`USBServer` process.
+
+  Such a class will be created for each :class:`~crappy.blocks.Block`
+  registering with the :class:`USBServer`.
+  """
 
   ser_num: str
   lock: multiprocessing.synchronize.RLock
   device: Device
 
   finished: bool = False
 
 
 class USBServer(Process):
-  """"""
+  """This class is a server managing communication with USB devices through the
+  :mod:`pysub` library.
+
+  As :mod:`pyusb` is not process-safe in Python, running a server is the only
+  option to allow multiple :class:`~crappy.blocks.Block` to use the library in
+  parallel. This server simply sends the USB commands it receives to the USB
+  devices, and returns back the answers. It features a quite complex
+  architecture for managing the requests and properly starting up and shutting
+  down.
+
+  The server is a child of :obj:`multiprocessing.Process`.
+  """
 
   initialized = False
   logger: Optional[logging.Logger] = None
 
   process: Optional[multiprocessing.context.Process] = None
   block_nr: int = 0
   devices: Dict[str, Device] = dict()
@@ -63,22 +78,32 @@
                current_block: Synchronized,
                command_file: FileIO,
                answer_file: FileIO,
                block_dict: Dict[int, BlockObjects],
                stop_event: multiprocessing.synchronize.Event,
                log_queue: multiprocessing.queues.Queue,
                log_level: Optional[int]) -> None:
-    """
+    """Sets the arguments.
 
     Args:
-      current_block:
-      command_file:
-      answer_file:
-      block_dict:
-      stop_event:
+      current_block: A :obj:`multiprocessing.Value` storing the index of
+        the :class:`~crappy.blocks.Block` currently allowed to communicate with
+        the server.
+      command_file: The handle to a file where the USB commands to send will be
+        written.
+      answer_file: The handle to a file where to write the answers from the USB
+        devices.
+      block_dict: A :obj:`dict` indicating for each index which
+        :class:`~crappy.blocks.Block` it corresponds to.
+      stop_event: A :obj:`multiprocessing.Event` indicating the server when it
+        should stop running.
+      log_queue: A :obj:`multiprocessing.Queue` for sending the log messages to
+        the main :obj:`~logging.Logger`, only used in Windows.
+      log_level: The minimum logging level of the entire Crappy script, as an
+        :obj:`int`.
     """
 
     super().__init__(name=f'crappy.{type(self).__name__}')
 
     # Objects for synchronizing with the server
     self._current_block = current_block
     self._command_file = command_file
@@ -95,21 +120,26 @@
     for ser_num in set(block.ser_num for block in self._block_dict.values()):
       self._dev_count[ser_num] = sum(
         1 for _ in (block for block in self._block_dict.values()
                     if block.ser_num == ser_num))
 
   @classmethod
   def register(cls, ser_num: Optional[str] = None) -> USBArgsType:
-    """
+    """Allows a :class:`~crappy.blocks.Block` to register for communicating
+    with the server. This Block is then given the necessary information for
+    communication.
 
     Args:
-      ser_num:
+      ser_num: The serial number of the FT232H to communicate with, as a
+        :obj:`str`.
 
     Returns:
-
+      A :obj:`tuple` containing the necessary information for other objects to
+      communicate with the server. This information is for example given as
+      arguments to :class:`~crappy.tool.ft232h.FT232HServer` objects.
     """
 
     # Initializing the synchronization objects
     if not cls.initialized:
       cls._initialize()
 
     # Assigning an index to the calling Block
@@ -137,20 +167,22 @@
     return (index, lock, cls.command_file, cls.answer_file, cls.shared_lock,
             cls.current_block)
 
   @classmethod
   def start_server(cls,
                    log_queue: multiprocessing.queues.Queue,
                    log_level: int) -> None:
-    """Initializes and starts the USB server process.
+    """Initializes and starts the USB server Process.
 
     Args:
-      log_queue: The queue carrying the log messages from the server process to
-        Crappy's centralized log handler.
-      log_level:
+      log_queue: The :obj:`multiprocessing.Queue` carrying the log messages 
+        from the server Process to Crappy's centralized log handler. Only used 
+        in Windows.
+      log_level: The minimum logging level of the entire Crappy script, as an
+        :obj:`int`.
     """
 
     cls.process = cls(current_block=cls.current_block,
                       command_file=cls.command_file,
                       answer_file=cls.answer_file,
                       block_dict=cls.block_dict,
                       stop_event=cls.stop_event,
@@ -187,49 +219,61 @@
     cls.answer_file = TemporaryFile(buffering=0)
     cls.shared_lock = RLock()
 
     cls.initialized = True
 
   @classmethod
   def log(cls, level: int, msg: str) -> None:
-    """"""
+    """Wrapper for recording log messages.
+
+    Also instantiates the :obj:`~logging.Logger` on the first message.
+
+    Args:
+      level: The logging level of the message, as an :obj:`int`.
+      msg: The message to log, as a :obj:`str`.
+    """
 
     if cls.logger is None:
       cls.logger = logging.getLogger(f'crappy.{cls.__name__}')
 
     cls.logger.log(level, msg)
 
   @staticmethod
   @contextmanager
   def acquire_timeout(lock: multiprocessing.synchronize.RLock,
                       timeout: float) -> bool:
-    """
+    """Short context manager for acquiring a :obj:`multiprocessing.Lock` with a 
+    specified timeout.
 
     Args:
-      lock:
-      timeout:
+      lock: The Lock to acquire.
+      timeout: The timeout for acquiring the Lock, as a :obj:`float`.
 
     Returns:
-
+      :obj:`True` if the Lock was successfully acquired, :obj:`False`
+      otherwise.
     """
 
     ret = False
     try:
       ret = lock.acquire(timeout=timeout)
       yield ret
     finally:
       if ret:
         lock.release()
 
   @staticmethod
   def _get_devices() -> Dict[str, Any]:
-    """
+    """Detects all the connected FT232H devices and returns them as a 
+    :obj:`dict`.
 
     Returns:
-
+      A :obj:`dict` containing as keys the detected serial numbers and as
+      values the handles in the :mod:`pyusb` module to the associated FT232H
+      devices.
     """
 
     # Searching for the FT232H devices
     devices: List[Device] = list(find(find_all=True,
                                       idVendor=0x0403,
                                       idProduct=0x6014))
     if not devices:
@@ -250,15 +294,21 @@
         else:
           raise ValueError('Please set a serial number for each FT232H ! It '
                            'can be done using the dedicated crappy tool')
 
     return dev_dict
 
   def run(self) -> None:
-    """"""
+    """The main loop of the server.
+
+    Waits for a :class:`~crappy.blocks.Block` to acquire control, reads its 
+    command, sends it to the correct USB device, reads the answer from the USB 
+    device and sends it back to the Block in control. Then, does the same with 
+    the next Block getting control over the server.
+    """
 
     self._set_logger()
     self._log(logging.INFO, "Logger configured")
 
     # Disabling the KeyboardInterrupt exceptions, to avoid disruptions
     self._log(logging.WARNING, "Disabling KeyboardInterrupt for the server !")
     signal.signal(signal.SIGINT, signal.SIG_IGN)
@@ -336,15 +386,15 @@
     """Sends commands to a USB device and returns the answer.
 
     Args:
       command: The command to send to the device. The bytes are arranged in a
         specific way for each type of command.
       device: The :mod:`pyusb` Device to which the commands are sent.
       serial_nr: The serial number of the :mod:`pyusb` device.
-      index: The index of the block currently controlling the server.
+      index: The index of the Block currently controlling the server.
 
     Returns:
       The index of the command, followed by the answer from the USB device if
       applicable.
     """
 
     command = command.split(b',')
@@ -424,15 +474,16 @@
     # Registers a block as gone
     # It doesn't actually interact with the device
     elif command[0] == b'13':
       self._block_dict[index].finished = True
       return b'13,'
 
   def _set_logger(self) -> None:
-    """"""
+    """Instantiates and sets up the :obj:`~logging.Logger` for recording log
+    messages."""
 
     logger = logging.getLogger(self.name)
 
     # Disabling logging if requested
     if self._log_level is not None:
       logger.setLevel(self._log_level)
     else:
@@ -443,19 +494,19 @@
       queue_handler = logging.handlers.QueueHandler(self._log_queue)
       queue_handler.setLevel(self._log_level)
       logger.addHandler(queue_handler)
 
     self._logger = logger
 
   def _log(self, level: int, msg: str) -> None:
-    """
+    """Wrapper for recording log messages.
 
     Args:
-      level:
-      msg:
+      level: The logging level of the message, as an :obj:`int`.
+      msg: The message to lof, as a :obj:`str`.
     """
 
     if self._logger is None:
       return
     self._logger.log(level, msg)
 
   @staticmethod
@@ -463,15 +514,15 @@
     """Returns some configuration information from a USB object.
 
     Args:
       device: A :obj:`usb.core.Device`
 
     Returns:
       The index, in endpoint, out endpoint and maximum packet size of a USB
-      device
+      device.
     """
 
     interface = device.get_active_configuration()[(0, 0)]
     index = interface.bInterfaceNumber + 1
     in_ep, out_ep = sorted([ep.bEndpointAddress for ep in interface])[:2]
     max_packet_size = interface[0].wMaxPacketSize
     return index, in_ep, out_ep, max_packet_size
```

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/image_processing/dic_ve.py` & `crappy-2.0.0.dev2/src/crappy/tool/image_processing/dic_ve.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 try:
   import cv2
 except (ModuleNotFoundError, ImportError):
   cv2 = OptionalModule("opencv-python")
 
 
 class DICVETool:
-  """This tool computes the displacement of regions of interest (patches) on an
-  image compared to a reference image.
+  """This class is the core of the :class:`~crappy.blocks.DICVE` Block.
+
+  It tracks patches on images received from a :class:`~crappy.camera.Camera` 
+  object, and computes a strain value at each new image.
 
   It relies on cross-correlation algorithms to calculate the displacement.
-  Different algorithms are available depending on the needs.
-  This tool is mainly used to perform video-extensometry on speckled surfaces,
-  although it can as well be of use for other applications.
+  Different algorithms are available depending on the needs. This tool is
+  mainly used to perform video-extensometry on speckled surfaces, although it
+  could as well be of use for other applications.
   """
 
   def __init__(self,
                patches: SpotsBoxes,
                method: str = 'Disflow',
                alpha: float = 3,
                delta: float = 1,
@@ -31,40 +33,43 @@
                iterations: int = 1,
                gradient_iterations: int = 10,
                patch_size: int = 8,
                patch_stride: int = 3,
                border: float = 0.2,
                safe: bool = True,
                follow: bool = True) -> None:
-    """Sets a few attributes and initializes Disflow if this method was
+    """Sets a few attributes and initializes DISFlow if this method was
     selected.
 
     Args:
-      patches: The regions to track, given as a :class:`Spot_boxes` object.
+      patches: An instance of the
+        :class:`~crappy.tool.camera_config.config_tools.SpotsBoxes` class,
+        containing the coordinates of the patches to track.
       method: The method to use to calculate the displacement. `Disflow` uses
         opencv's DISOpticalFlow and `Lucas Kanade` uses opencv's
         calcOpticalFlowPyrLK, while all other methods are based on a basic
         cross-correlation in the Fourier domain. `Pixel precision` calculates
         the displacement by getting the position of the maximum of the
         cross-correlation, and has thus a 1-pixel resolution. It is mainly
         meant for debugging. `Parabola` refines the result of
         `Pixel precision` by interpolating the neighborhood of the maximum, and
-        have thus sub-pixel resolutions.
-      alpha: Weight of the smoothness term in DisFlow.
-      delta: Weight of the color constancy term in DisFlow.
-      gamma: Weight of the gradient constancy term in DisFlow.
+        has thus a sub-pixel resolution.
+      alpha: Weight of the smoothness term in DISFlow, as a :obj:`float`.
+      delta: Weight of the color constancy term in DISFlow, as a :obj:`float`.
+      gamma: Weight of the gradient constancy term in DISFlow , as a
+        :obj:`float`.
       finest_scale: Finest level of the Gaussian pyramid on which the flow
-        is computed in DisFlow (`0` means full scale).
+        is computed in DISFlow (`0` means full scale), as an :obj:`int`.
       iterations: Maximum number of gradient descent iterations in the
-        patch inverse search stage in DisFlow.
+        patch inverse search stage in DISFlow, as an :obj:`int`.
       gradient_iterations: Maximum number of gradient descent iterations
-        in the patch inverse search stage in DisFlow.
-      patch_size: Size of an image patch for matching in DisFlow
+        in the patch inverse search stage in DISFlow, as an :obj:`int`.
+      patch_size: Size of an image patch for matching in DISFlow
         (in pixels).
-      patch_stride: Stride between neighbor patches in DisFlow. Must be
+      patch_stride: Stride between neighbor patches in DISFlow. Must be
         less than patch size.
       border: Crop the patch on each side according to this value before
         calculating the displacements. 0 means no cropping, 1 means the entire
         patch is cropped.
       safe: If :obj:`True`, checks whether the patches aren't exiting the
         image, and raises an error if that's the case.
       follow: It :obj:`True`, the patches will move to follow the displacement
@@ -81,15 +86,15 @@
     self._safe = safe
     self._follow = follow
 
     # These attributes will be set later
     self._img0 = None
     self._height, self._width = None, None
 
-    # Initialize Disflow if it is the selected method
+    # Initialize DISFlow if it is the selected method
     if self._method == 'Disflow':
       self._dis = cv2.DISOpticalFlow_create(cv2.DISOPTICAL_FLOW_PRESET_FAST)
       self._dis.setVariationalRefinementIterations(iterations)
       self._dis.setVariationalRefinementAlpha(alpha)
       self._dis.setVariationalRefinementDelta(delta)
       self._dis.setVariationalRefinementGamma(gamma)
       self._dis.setFinestScale(finest_scale)
@@ -216,15 +221,15 @@
       return [(y, x)], 0, 0, [(y_disp, x_disp)]
 
   def _calc_disflow(self,
                     patch: Box,
                     img: np.ndarray,
                     offset: Tuple[int, int]) -> List[float]:
     """Returns the displacement between the original and the current image with
-    a sub-pixel precision, using Disflow."""
+    a sub-pixel precision, using DISFlow."""
 
     disp_img = self._dis.calc(self._get_patch(self._img0, patch, offset),
                               self._get_patch(img, patch), None)
     return np.average(self._trim_patch(disp_img), axis=(0, 1)).tolist()
 
   def _calc_pixel_precision(self,
                             patch: Box,
@@ -345,15 +350,15 @@
     y_off, x_off = offset
     x_top, x_bottom, y_left, y_right = patch.sorted()
     return np.array(img[y_left - y_off: y_right - y_off,
                         x_top - x_off: x_bottom - x_off])
 
   def _trim_patch(self, patch: np.ndarray) -> np.ndarray:
     """Trims the border of a patch according to the value set by the user, and
-    returns the tuple corresponding to the trimmed patch."""
+    returns the sub image corresponding to the trimmed patch."""
 
     height, width, *_ = patch.shape
     return patch[int(height * self._border / 2):
                  int(height * (1 - self._border / 2)),
                  int(width * self._border / 2):
                  int(width * (1 - self._border / 2))]
```

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/image_processing/dis_correl.py` & `crappy-2.0.0.dev2/src/crappy/tool/image_processing/dis_correl.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,57 +10,61 @@
   import cv2
 except (ModuleNotFoundError, ImportError):
   cv2 = OptionalModule("opencv-python")
 import numpy as np
 
 
 class DISCorrelTool:
-  """This class simply stores the data needed for performing image correlation
-  using DisFlow, and also performs the correlation.
+  """This class is the core of the :class:`~crappy.blocks.DISCorrel` Block.
 
-  Multiple parameters of DisFlow can be tuned, but not all of them. The class
-  also takes care of projecting the image on the chosen base of fields, and
-  optionally to estimate the residuals of the correlation process.
+  It receives images from a :class:`~crappy.camera.Camera` object, and performs 
+  Dense Inverse Search correlation on each new image to get fields of interest. 
+  It relies on DISFlow for the image correlation, handles the projection of the 
+  image on the chosen fields, and calculates the residuals.
   """
 
   def __init__(self,
                box: Box,
                fields: Optional[List[str]] = None,
                alpha: float = 3,
                delta: float = 1,
                gamma: float = 0,
                finest_scale: int = 1,
                init: bool = True,
                iterations: int = 1,
                gradient_iterations: int = 10,
                patch_size: int = 8,
                patch_stride: int = 3) -> None:
-    """Sets the parameters of DisFlow.
+    """Sets the parameters of DISFlow.
 
     Args:
+      box: An instance of the
+        :class:`~crappy.tool.camera_config.config_tools.Box` object containing
+        the coordinates of the patch on which to perform image correlation.
       fields: The base of fields to use for the projection, given as a
         :obj:`list` of :obj:`str`. The available fields are :
         ::
 
           'x', 'y', 'r', 'exx', 'eyy', 'exy', 'eyx', 'exy2', 'z'
 
-      alpha: Weight of the smoothness term in DisFlow.
-      delta: Weight of the color constancy term in DisFlow.
-      gamma: Weight of the gradient constancy term in DisFlow
+      alpha: Weight of the smoothness term in DISFlow, as a :obj:`float`.
+      delta: Weight of the color constancy term in DISFlow, as a :obj:`float`.
+      gamma: Weight of the gradient constancy term in DISFlow , as a
+        :obj:`float`.
       finest_scale: Finest level of the Gaussian pyramid on which the flow
-        is computed in DisFlow (`0` means full scale).
+        is computed in DISFlow (`0` means full scale), as an :obj:`int`.
       init: If :obj:`True`, the last field is used to initialize the
         calculation for the next one.
       iterations: Maximum number of gradient descent iterations in the
-        patch inverse search stage in DisFlow.
+        patch inverse search stage in DISFlow, as an :obj:`int`.
       gradient_iterations: Maximum number of gradient descent iterations
-        in the patch inverse search stage in DisFlow.
-      patch_size: Size of an image patch for matching in DisFlow
+        in the patch inverse search stage in DISFlow, as an :obj:`int`.
+      patch_size: Size of an image patch for matching in DISFlow
         (in pixels).
-      patch_stride: Stride between neighbor patches in DisFlow. Must be
+      patch_stride: Stride between neighbor patches in DISFlow. Must be
         less than patch size.
     """
 
     if fields is not None and not all((field in allowed_fields
                                        for field in fields)):
       raise ValueError(f"The only allowed values for the fields "
                        f"are {allowed_fields}")
@@ -112,21 +116,21 @@
     # These attributes will be used later
     self._base = [fields[:, :, :, i] for i in range(fields.shape[3])]
     self._norm2 = [np.sum(base_field ** 2) for base_field in self._base]
 
   def get_data(self,
                img: np.ndarray,
                residuals: bool = False) -> List[float]:
-    """Processes the input image and returns the required data in a
+    """Processes the input image and returns the requested data in a
     :obj:`list`.
 
     Args:
       img: The new image to process.
       residuals: Whether the residuals should be calculated or not for the
-        image.
+        image, as a :obj:`bool`.
 
     Returns:
       A :obj:`list` containing the data to calculate, and the residuals at the
       end if requested.
     """
 
     # Making sure the reference image and the base fields were set
```

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/image_processing/fields.py` & `crappy-2.0.0.dev2/src/crappy/tool/image_processing/fields.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,21 +13,25 @@
 allowed_fields = ('x', 'y', 'r', 'exx', 'eyy', 'exy', 'eyx', 'exy2', 'z')
 
 
 def get_field(field_string: str,
               h: int,
               w: int) -> Tuple[np.ndarray, np.ndarray]:
   """Creates and returns the two fields on which the image will be projected,
-  as numpy arrays.
+  as :mod:`numpy` arrays.
+  
+  This function is used by the
+  :class:`~crappy.tool.image_processing.DISCorrelTool` and
+  :class:`~crappy.tool.image_processing.GPUCorrelTool` tools.
 
   Args:
-    field_string: The string describing the field on which to project the image
-      for correlation.
-    h: The height of the image.
-    w: The width of the image.
+    field_string: The :obj:`str` describing the field on which to project the
+      image for correlation.
+    h: The height of the image, as an :obj:`int`.
+    w: The width of the image, as an :obj:`int`.
   """
 
   if field_string == 'x':
     return (np.ones((h, w), dtype=np.float32),
             np.zeros((h, w), dtype=np.float32))
 
   elif field_string == 'y':
@@ -67,24 +71,27 @@
 
   elif field_string == 'z':
     u, v = np.meshgrid(np.linspace(-w, w, w, dtype=np.float32),
                        np.linspace(-h, h, h, dtype=np.float32))
     return u / 200, v / 200
 
   else:
-    raise NameError(f"[DICVE Field parser] Unknown field {field_string}")
+    raise NameError(f"Unknown field {field_string}")
 
 
 def get_res(ref: np.ndarray, img: np.ndarray, flow: np.ndarray) -> np.ndarray:
   """Calculates the difference between the original image and the one
-    reconstructed from the current image and the calculated flow.
+  reconstructed from the current image and the calculated flow.
+
+  This function is used by the
+  :class:`~crappy.tool.image_processing.DISCorrelTool` tool.
 
   Args:
-    ref: The reference image for calculating the optical flow
-    img: The current image for calculating the optical flow
+    ref: The reference image for calculating the optical flow.
+    img: The current image for calculating the optical flow.
     flow: The calculated optical flow
   """
 
   x, y = np.meshgrid(np.arange(img.shape[1]), np.arange(img.shape[0]))
   return ref - cv2.remap(img.astype(np.float32),
                          (x + flow[:, :, 0]).astype(np.float32),
                          (y + flow[:, :, 1]).astype(np.float32), 1)
```

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/image_processing/gpu_correl.py` & `crappy-2.0.0.dev2/src/crappy/tool/image_processing/gpu_correl.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     for i in range(nx):
       out[j, i] = arr[int(ry * j + .5), int(rx * i + .5)]
 
   return out
 
 
 class CorrelStage:
-  """Represents a stage of the pyramid used by the :ref:`GPUCorrel` tool for
+  """Represents a stage of the pyramid used by the :class:`GPUCorrelTool` for
   performing GPU correlation.
 
   This class actually performs the GPU computation, while the calling classes
   only manage the data.
   """
 
   def __init__(self,
@@ -71,14 +71,15 @@
                n_fields: Optional[int] = None,
                kernel_file: Optional[Union[Path, str]] = None) -> None:
     """Sets the args and instantiates the :mod:`pycuda` objects.
 
     Args:
       img_size: The shape of the images to process. It is given beforehand so
         that the memory can be allocated before the test starts.
+      logger_name: The name of the parent logger, as a :obj:`str`.
       verbose: The verbose level as an integer, between `0` and `3`. At level
         `0` no information is displayed, and at level `3` so much information
         is displayed that is slows the code down.
       iterations: The maximum number of iterations to run before returning the
         results. The results may be returned before if the residuals start
         increasing.
       mul: The scalar by which the direction will be multiplied before being
@@ -473,27 +474,31 @@
 
     self._gradient_krnl.prepared_call(self._grid, self._block,
                                       self._dev_grad_x.gpudata,
                                       self._dev_grad_y.gpudata)
 
 
 class GPUCorrelTool:
-  """This tool performs GPU correlation between two images in order to identify
-  fields of rigid body displacements.
+  """This class is the core of the :class:`~crappy.blocks.GPUCorrel` and 
+  :class:`~crappy.blocks.GPUVE` Blocks.
+
+  It receives images from a :class:`~crappy.camera.Camera`, and performs 
+  GPU-accelerated image correlation on each received image. From this 
+  correlation, rigid body displacements or other fields are identified.
 
   This class  is meant to be efficient enough to run in real-time. It relies on
-  :class:`CorrelStage` to perform correlation on different scales. It mainly
-  takes a list of base fields and a reference image as inputs, and project the
-  displacement between the current image and the reference one on the base of
-  fields. The optimal fit is achieved by lowering the residuals with a
-  least-squares method.
+  the :class:`CorrelStage` class (not documented) to perform correlation on
+  different scales. It mainly takes a list of base fields and a reference image
+  as inputs, and project the displacement between the current image and the
+  reference one on the base of fields. The optimal fit is achieved by lowering
+  the residuals with a least-squares method.
 
   The projection on the base is performed sequentially, using the results
   obtained at stages with low resolution to initialize the computation on
-  on stages with higher resolution. A newton method is used to converge towards
+  stages with higher resolution. A Newton method is used to converge towards
   an optimal solution.
   """
 
   context = None
 
   def __init__(self,
                logger_name: str,
@@ -506,50 +511,53 @@
                fields: Optional[List[str]] = None,
                ref_img: Optional[np.ndarray] = None,
                mask: Optional[np.ndarray] = None,
                mul: float = 3) -> None:
     """Sets the args and a few parameters of :mod:`pycuda`.
 
     Args:
+      logger_name: The name of the parent :obj:`~logging.Logger`, to be used
+        for setting the Logger of the class.
       context: Optionally, the :mod:`pycuda` context to use. If not specified,
         a new context is instantiated.
       verbose: The verbose level as an integer, between `0` and `3`. At level
         `0` no information is displayed, and at level `3` so much information
         is displayed that is slows the code down.
       levels: Number of levels of the pyramid. More levels may help converging
         on images with large strain, but may fail on images that don't contain
         low spatial frequency. Fewer levels mean that the program runs faster.
-      resampling_factor: the factor by which the resolution is divided between
+      resampling_factor: The factor by which the resolution is divided between
         each stage of the pyramid. A low factor ensures coherence between the
         stages, but is more computationally intensive. A high factor allows
         reaching a finer detail level, but may lead to a coherence loss between
         the stages.
       kernel_file: The path to the file containing the kernels to use for the
-        correlation. Can be a :obj:`pathlib.Path` object or a :obj:`str`.
+        correlation. Can be a :obj:`pathlib.Path` object or a :obj:`str`. If
+        not provided, the default :ref:`GPU Kernels` are used.
       iterations: The maximum number of iterations to run before returning the
         results. The results may be returned before if the residuals start
         increasing.
       fields: A :obj:`list` of :obj:`str` representing the base of fields on
         which the image will be projected during correlation. The possible
         fields are :
         ::
 
           'x', 'y', 'r', 'exx', 'eyy', 'exy', 'eyx', 'exy2', 'z'
 
-      ref_img: the reference image, as a 2D :mod:`numpy` array with `dtype`
-        `float32`. It can either be given at ``__init__``, or set later with
-        :meth:`set_orig`.
+      ref_img: The reference image, as a 2D :obj:`numpy.array` with `dtype`
+        `float32`. It can either be given at :meth:`__init__`, or set later
+        with :meth:`set_orig`.
       mask: The mask used for weighting the region of interest on the image. It
         is generally used to prevent unexpected behavior on the border of the
         image.
       mul: The scalar by which the direction will be multiplied before being
         added to the solution. If it's too high, the convergence will be fast
-        but there's a risk that to go past the solution and to diverge. If it's
-        too low, the convergence will be slower and require more iterations.
-        `3` was found to be an acceptable value in most cases, but it is
+        but there's a risk to go past the solution and to diverge. If it's too
+        low, the convergence will be slower and require more iterations. `3`
+        was found to be an acceptable value in most cases, but it is
         recommended to tune this value for each application so that the
         convergence is neither too slow nor too fast.
     """
 
     self._context = context
     self._logger: Optional[logging.Logger] = None
     self._logger_name = logger_name
@@ -747,15 +755,15 @@
     properly."""
 
     GPUCorrelTool.context.pop()
 
   def _get_fields(self,
                   y: Optional[int] = None,
                   x: Optional[int] = None) -> (Any, Any):
-    """Returns the fields, resampled to size `(y,x)`."""
+    """Returns the fields, resampled to size `(y, x)`."""
 
     if x is None or y is None:
       y, x = self._heights[0], self._widths[0]
 
     out_x = gpuarray.empty((self._n_fields, y, x), np.float32)
     out_y = gpuarray.empty((self._n_fields, y, x), np.float32)
     grid = (int(ceil(x / 32)), int(ceil(y / 32)))
```

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/image_processing/kernels.cu` & `crappy-2.0.0.dev2/src/crappy/tool/image_processing/kernels.cu`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/image_processing/video_extenso/tracker.py` & `crappy-2.0.0.dev2/src/crappy/camera/opencv_camera.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,251 +1,261 @@
 # coding: utf-8
 
-from multiprocessing import Process, get_start_method
-from multiprocessing.connection import Connection
-from multiprocessing.queues import Queue
-import numpy as np
-from typing import Optional, Union
-from time import time
-from select import select
+from time import time, sleep
+from typing import Tuple, List, Optional
+from numpy import ndarray
+from platform import system
+from subprocess import run
+from re import findall, split, search
 import logging
-import logging.handlers
 
-from ...camera_config import Box
-from ...._global import OptionalModule
+from .meta_camera import Camera
+from .._global import OptionalModule
 
 try:
   import cv2
 except (ModuleNotFoundError, ImportError):
   cv2 = OptionalModule("opencv-python")
-try:
-  from skimage.filters import threshold_otsu
-except (ModuleNotFoundError, ImportError):
-  threshold_otsu = OptionalModule("skimage", "Please install scikit-image to "
-                                             "use Video-extenso")
 
 
-class LostSpotError(Exception):
-  """Exception raised when a spot is lost, or when there's too much
-  overlapping."""
+class CameraOpencv(Camera):
+  """A class for reading images from any camera able to interface with OpenCv.
 
+  The number of the video device to read images from can be specified. It is
+  then also possible to tune the encoding format and the size.
 
-class Tracker(Process):
-  """Process whose task is to track a spot on an image.
-
-  It receives a subframe centered on the last known position of the spot, and
-  returns the updated position of the detected spot.
+  This camera class is less performant than the
+  :class:`~crappy.camera.CameraGstreamer` one that relies on GStreamer, but the
+  installation of OpenCv is way easier than the one of GStreamer.
+
+  Note:
+    For a better performance of this class in Linux, it is recommended to have
+    `v4l-utils` installed.
   """
 
-  names = list()
+  def __init__(self) -> None:
+    """Sets variables and adds the channels setting."""
 
-  def __init__(self,
-               pipe: Connection,
-               logger_name: str,
-               log_level: Optional[int],
-               log_queue: Queue,
-               white_spots: bool = False,
-               thresh: Optional[int] = None,
-               blur: Optional[float] = 5) -> None:
-    """Sets the args.
+    super().__init__()
+
+    self._cap = None
+    self._device_num: Optional[int] = None
+    self._formats: List[str] = list()
+
+    self.add_choice_setting(name="channels",
+                            choices=('1', '3'),
+                            default='1')
+
+  def open(self, device_num: int = 0, **kwargs) -> None:
+    """Opens the video stream and sets any user-specified settings.
 
     Args:
-      pipe: The :obj:`multiprocessing.connection.Connection` object through
-        which the image is received and the updated coordinates of the spot
-        are sent back.
-      white_spots: If :obj:`True`, detects white objects on a black background,
-        else black objects on a white background.
-      thresh: If given, this threshold value will always be used for isolating
-        the spot from the background. If not given (:obj:`None`), a new
-        threshold is recalculated for each new subframe. Spots are less likely
-        to be lost with an adaptive threshold, but it takes a bit more time.
-      blur: If not :obj:`None`, the subframe is first blurred before trying to
-        detect the spot. This argument gives the size of the kernel to use for
-        blurring. Better results are obtained with blurring, but it takes a bit
-        more time.
-      logger_name:
+      device_num: The index of the device to open, as an :obj:`int`.
+      **kwargs: Any additional setting to set before opening the configuration
+        window.
     """
 
-    super().__init__()
-    self.name = self.get_name(logger_name, type(self).__name__)
+    if not isinstance(device_num, int) or device_num < 0:
+      raise ValueError("device_num should be an integer !")
 
-    self._pipe = pipe
-    self._white_spots = white_spots
-    self._thresh = thresh
-    self._blur = blur
+    # Opening the videocapture device
+    self.log(logging.INFO, "Opening the image stream from the camera")
+    self._cap = cv2.VideoCapture(device_num)
+    self._device_num = device_num
+    fourcc = self._get_fourcc()
+
+    if system() == 'Linux':
+      self._formats = []
+
+      # Trying to run v4l2-ctl to get the available formats
+      command = ['v4l2-ctl', '-d', str(device_num), '--list-formats-ext']
+      try:
+        self.log(logging.INFO, f"Getting the available image formats with "
+                               f"command {command}")
+        check = run(command, capture_output=True, text=True)
+      except FileNotFoundError:
+        self.log(logging.WARNING, "The performance of the CameraOpencv class "
+                                  "could be improved if v4l-utils was "
+                                  "installed !")
+        check = None
+      check = check.stdout if check is not None else ''
+
+      # Splitting the returned string to isolate each encoding
+      if findall(r'\[\d+]', check):
+        check = split(r'\[\d+]', check)[1:]
+      elif findall(r'Pixel\sFormat', check):
+        check = split(r'Pixel\sFormat', check)[1:]
+      else:
+        check = []
 
-    self._logger: Optional[logging.Logger] = None
-    self._log_level = log_level
-    self._log_queue = log_queue
+      if check:
+        for img_format in check:
+          # For each encoding, finding its name
+          name, *_ = search(r"'(\w+)'", img_format).groups()
+          sizes = findall(r'\d+x\d+', img_format)
+          fps_sections = split(r'\d+x\d+', img_format)[1:]
+
+          # For each name, finding the available sizes
+          for size, fps_section in zip(sizes, fps_sections):
+            fps_list = findall(r'\((\d+\.\d+)\sfps\)', fps_section)
+            for fps in fps_list:
+              self._formats.append(f'{name} {size} ({fps} fps)')
 
-    self._n = 0
-    self._last_warn = time()
+      else:
+        # If v4l-utils is not installed, proposing two encodings without
+        # further detail
+        self._formats = [fourcc, 'MJPG']
+
+        # Still letting the user choose the size
+        self.add_scale_setting(name='width', lowest=1, highest=1920,
+                               getter=self._get_width, setter=self._set_width)
+        self.add_scale_setting(name='height', lowest=1, highest=1080,
+                               getter=self._get_height,
+                               setter=self._set_height)
 
-  @classmethod
-  def get_name(cls, logger_name: str, self_name: str) -> str:
-    """"""
+    else:
+      # On Windows the fourcc management is even messier than on Linux
+      self._formats = []
 
-    i = 1
-    while f"{logger_name}.{self_name}-{i}" in cls.names:
-      i += 1
+      # Still letting the user choose the size
+      self.add_scale_setting(name='width', lowest=1, highest=1920,
+                             getter=self._get_width, setter=self._set_width)
+      self.add_scale_setting(name='height', lowest=1, highest=1080,
+                             getter=self._get_height, setter=self._set_height)
+
+    if self._formats:
+      # The format integrates the size selection
+      if ' ' in self._formats[0]:
+        self.add_choice_setting(name='format',
+                                choices=tuple(self._formats),
+                                getter=self._get_format_size,
+                                setter=self._set_format)
+      # The size is independent of the format
+      else:
+        self.add_choice_setting(name='format',
+                                choices=tuple(self._formats),
+                                getter=self._get_fourcc,
+                                setter=self._set_format)
+
+    # Adding the software ROI selection settings
+    if 'width' in self.settings and 'height' in self.settings:
+      width, height = self._get_width(), self._get_height()
+      self.add_software_roi(width, height)
+    elif 'format' in self.settings:
+      width, height = search(r'(\d+)x(\d+)', self._get_format_size()).groups()
+      self.add_software_roi(int(width), int(height))
+
+    # Setting the kwargs if any
+    self.set_all(**kwargs)
+
+  def get_image(self) -> Tuple[float, ndarray]:
+    """Grabs a frame from the videocapture object and returns it along with a
+    timestamp."""
+
+    # Grabbing the frame and the timestamp
+    t = time()
+    ret, frame = self._cap.read()
+
+    # Checking the integrity of the frame
+    if not ret:
+      raise IOError("Error reading the camera")
+
+    # Returning the image in the right format, and its timestamp
+    if self.channels == '1':
+      return t, self.apply_soft_roi(cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY))
+    else:
+      return t, self.apply_soft_roi(frame)
 
-    cls.names.append(f"{logger_name}.{self_name}-{i}")
-    return f"{logger_name}.{self_name}-{i}"
+  def close(self) -> None:
+    """Releases the videocapture object."""
 
-  def run(self) -> None:
-    """Continuously reads incoming subframes, tries to detect a spot and sends
-    back the coordinates of the detected spot.
+    if self._cap is not None:
+      self.log(logging.INFO, "Closing the image stream from the camera")
+      self._cap.release()
 
-    Can only be stopped either with a :exc:`KeyboardInterrupt` or when
-    receiving a text message from the parent VideoExtenso class.
-    """
+  def _get_fourcc(self) -> str:
+    """Returns the current fourcc string of the video encoding."""
 
-    # Looping forever for receiving data
-    try:
-      self._set_logger()
-
-      while True:
-        # Making sure the call to recv is not blocking
-        if self._pipe.poll(0.5):
-          y_start, x_start, img = self._pipe.recv()
-          self._log(logging.DEBUG, "Received data from pipe")
-          self._n += 1
-
-          # If a string is received, always means the process has to stop
-          if isinstance(img, str):
-            break
-
-          # Simply sending back the new Box containing the spot
-          try:
-            self._log(logging.DEBUG, "Sending back data through pipe")
-            self._send(self._evaluate(x_start, y_start, img))
-
-          # If the caught exception is a KeyboardInterrupt, simply stopping
-          except KeyboardInterrupt:
-            self._log(logging.INFO, "Caught KeyboardInterrupt, stopping the "
-                                    "process")
-            break
-          # Sending back the exception if anything else unexpected happened
-          except (Exception,) as exc:
-            self._logger.exception("Caught exception while tracking spot",
-                                   exc_info=exc)
-            self._send('stop')
-            break
-
-    # In case the user presses CTRL+C, simply stopping the process
-    except KeyboardInterrupt:
-      self._log(logging.INFO, "Caught KeyboardInterrupt, stopping the process")
-
-  def _evaluate(self, x_start: int, y_start: int, img: np.ndarray) -> Box:
-    """Takes a sub-image, applies a threshold on it and tries to detect the new
-    position of the spot.
+    fcc = int(self._cap.get(cv2.CAP_PROP_FOURCC))
+    return f"{fcc & 0xFF:c}{(fcc >> 8) & 0xFF:c}" \
+           f"{(fcc >> 16) & 0xFF:c}{(fcc >> 24) & 0xFF:c}"
 
-    Args:
-      x_start: The x position of the top left pixel of the subframe on the
-        entire image.
-      y_start: The y position of the top left pixel of the subframe on the
-        entire image.
-      img: The subframe on which to search for a spot.
-
-    Returns:
-      A Box object containing the x and y start and end positions of the
-      detected spot, as well as the coordinates of the centroid.
-    """
+  def _get_width(self) -> int:
+    """Returns the current image width."""
 
-    # First, blurring the image if asked to
-    if self._blur is not None and self._blur > 1:
-      img = cv2.medianBlur(img, self._blur)
-
-    # Determining the best threshold for the image if required
-    thresh = self._thresh if self._thresh is not None else threshold_otsu(img)
-
-    # Getting all pixels superior or inferior to threshold
-    if self._white_spots:
-      black_white = (img > thresh).astype('uint8')
-    else:
-      black_white = (img <= thresh).astype('uint8')
+    return self._cap.get(cv2.CAP_PROP_FRAME_WIDTH)
 
-    # Checking that the detected spot is large enough
-    if np.count_nonzero(black_white) < 0.1 * img.size:
+  def _get_height(self) -> int:
+    """Returns the current image height."""
 
-      # If the threshold is pre-defined, trying again with an updated one
-      if self._thresh is not None:
-        self._log(logging.WARNING,
-                  "Detected spot too small compared with overall box size, "
-                  "recalculating threshold")
-        thresh = threshold_otsu(img)
-        if self._white_spots:
-          black_white = (img > thresh).astype('uint8')
-        else:
-          black_white = (img <= thresh).astype('uint8')
-
-        # If the spot still cannot be detected, aborting
-        if np.count_nonzero(black_white) < 0.1 * img.size:
-          self._log(logging.ERROR,
-                    "Couldn't detect spot with adaptive threshold, aborting !")
-          raise LostSpotError
+    return self._cap.get(cv2.CAP_PROP_FRAME_HEIGHT)
 
-      # If an adaptive threshold is already used, nothing more can be done
-      else:
-        self._log(logging.ERROR,
-                  "Couldn't detect spot with adaptive threshold, aborting !")
-        raise LostSpotError
+  def _set_width(self, width: int) -> None:
+    """Tries to set the image width."""
 
-    # Calculating the coordinates of the centroid using the image moments
-    moments = cv2.moments(black_white)
-    try:
-      x = moments['m10'] / moments['m00']
-      y = moments['m01'] / moments['m00']
-    except ZeroDivisionError:
-      raise ZeroDivisionError("Couldn't compute the centroid because the "
-                              "moment of order 0, 0 is zero !")
-
-    # Getting the updated centroid and coordinates of the spot
-    x_min, y_min, width, height = cv2.boundingRect(black_white)
-    return Box(x_start=x_start + x_min,
-               y_start=y_start + y_min,
-               x_end=x_start + x_min + width,
-               y_end=y_start + y_min + height,
-               x_centroid=x_start + x,
-               y_centroid=y_start + y)
+    self._cap.set(cv2.CAP_PROP_FRAME_WIDTH, width)
 
-  def _send(self, val: Union[Box, str]) -> None:
-    """"""
+    # Reloading the software ROI selection settings
+    if self._soft_roi_set:
+      sleep(0.1)
+      width, height = self._get_width(), self._get_height()
+      self.reload_software_roi(width, height)
 
-    if select([], [self._pipe], [], 0)[1]:
-      self._pipe.send(val)
-    else:
-      if time() - self._last_warn > 1:
-        self._last_warn = time()
-        self._log(logging.WARNING, f"Cannot send the detected spot to the "
-                                   f"VideoExtenso tool, the Pipe is full !")
-
-  def _set_logger(self) -> None:
-    """"""
-
-    logger = logging.getLogger(self.name)
-
-    # Disabling logging if requested
-    if self._log_level is not None:
-      logger.setLevel(self._log_level)
-    else:
-      logging.disable()
+  def _set_height(self, height: int) -> None:
+    """Tries to set the image height."""
 
-    # On Windows, the messages need to be sent through a Queue for logging
-    if get_start_method() == "spawn" and self._log_level is not None:
-      queue_handler = logging.handlers.QueueHandler(self._log_queue)
-      queue_handler.setLevel(self._log_level)
-      logger.addHandler(queue_handler)
+    self._cap.set(cv2.CAP_PROP_FRAME_HEIGHT, height)
 
-    self._logger = logger
+    # Reloading the software ROI selection settings
+    if self._soft_roi_set:
+      sleep(0.1)
+      width, height = self._get_width(), self._get_height()
+      self.reload_software_roi(width, height)
 
-  def _log(self, level: int, msg: str) -> None:
-    """Sends a log message to the logger.
+  def _set_format(self, img_format: str) -> None:
+    """Sets the format of the image according to the user's choice."""
 
-    Args:
-      level: The logging level, as an :obj:`int`.
-      msg: The message to log, as a :obj:`str`.
-    """
+    # The format might be made of a name and a dimension, or just a name
+    try:
+      format_name, img_size, fps = findall(r"(\w+)\s(\w+)\s\((\d+.\d+) fps\)",
+                                           img_format)[0]
+    except ValueError:
+      format_name, img_size, fps = img_format, None, None
+
+    # Setting the format
+    self._cap.set(cv2.CAP_PROP_FOURCC, cv2.VideoWriter_fourcc(*format_name))
+
+    if img_size is not None:
+      # Getting the width and height from the second half of the string
+      width, height = map(int, img_size.split('x'))
+
+      # Setting the size
+      self._set_width(width)
+      self._set_height(height)
+
+    if fps is not None:
+      self._cap.set(cv2.CAP_PROP_FPS, float(fps))
+
+    # Reloading the software ROI selection settings
+    if self._soft_roi_set:
+      sleep(0.1)
+      width, height = search(r'(\d+)x(\d+)', self._get_format_size()).groups()
+      self.reload_software_roi(int(width), int(height))
+
+  def _get_format_size(self) -> str:
+    """Parses the ``v4l2-ctl -V`` command to get the current image format as a
+    :obj:`str`."""
+
+    # Sending the v4l2-ctl command
+    command = ['v4l2-ctl', '-d', str(self._device_num), '--all']
+    check = run(command, capture_output=True, text=True).stdout
+
+    # Parsing the answer
+    format_ = width = height = fps = ''
+    if search(r"Pixel Format\s*:\s*'(\w+)'", check) is not None:
+      format_, *_ = search(r"Pixel Format\s*:\s*'(\w+)'", check).groups()
+    if search(r"Width/Height\s*:\s*(\d+)/(\d+)", check) is not None:
+      width, height = search(r"Width/Height\s*:\s*(\d+)/(\d+)", check).groups()
+    if search(r"Frames per second\s*:\s*(\d+.\d+)", check) is not None:
+      fps, *_ = search(r"Frames per second\s*:\s*(\d+.\d+)", check).groups()
 
-    if self._logger is None:
-      return
-    self._logger.log(level, msg)
+    return f'{format_} {width}x{height} ({fps} fps)'
```

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/image_processing/video_extenso/video_extenso.py` & `crappy-2.0.0.dev2/src/crappy/tool/image_processing/video_extenso/video_extenso.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,115 +6,128 @@
 from typing import Optional, Tuple, List, Union
 import numpy as np
 from itertools import combinations
 from time import sleep, time
 import logging
 import logging.handlers
 from select import select
+from platform import system
 
 from ...camera_config import SpotsBoxes, Box
 from .tracker import Tracker, LostSpotError
 
 
 class VideoExtensoTool:
-  """This class tracks up to 4 spots on successive images, and computes the
-  strain on the material based on the displacement of the spots from their
-  original position.
-
-  The first step is to detect the spots to track. Once this is done, the
-  initial distances in x and y between the spots is saved. For each spot, a
-  Process in charge of tracking it is started. When a new image is received,
-  subframes based on the last known positions of the spots are sent to the
-  tracker processes, and they return the new positions of the detected spots.
-  Based on these new positions, updated strain values are returned.
+  """This class is the core of the :class:`~crappy.blocks.VideoExtenso` Block.
+
+  It performs spot tracking on up to `4` spots on the images acquired by the
+  :class:`~crappy.camera.Camera`, and computes the strain values at each new 
+  image. For each spot, the tracking is performed by an independent
+  :class:`~crappy.tool.image_processing.video_extenso.tracker.tracker.Tracker`
+  Process.
 
   It is possible to track only one spot, in which case only the position of its
-  center is returned and the strain values are left to 0.
+  center is returned and the strain values are left to `0`.
   """
 
   def __init__(self,
                spots: SpotsBoxes,
                thresh: int,
                log_level: Optional[int],
                log_queue: Queue,
                white_spots: bool = False,
                update_thresh: bool = False,
-               num_spots: Optional[int] = None,
                safe_mode: bool = False,
                border: int = 5,
                blur: Optional[int] = 5) -> None:
-    """Sets the args and the other instance attributes.
+    """Sets the arguments and the other instance attributes.
 
     Args:
-      white_spots: If :obj:`True`, detects white objects on a black background,
-        else black objects on a white background.
-      update_thresh: If :obj:`True`, the threshold for detecting the spots is
-        re-calculated for each new image. Otherwise, the first calculated
-        threshold is kept for the entire test. The spots are less likely to be
-        lost with adaptive threshold, but the measurement will be more noisy.
-        Adaptive threshold may also yield inconsistent results when spots are
-        lost.
-      num_spots: The number of spots to detect, between 1 and 4. The class will
-        then try to detect this exact number of spots, and won't work if not
-        enough spots can be found. If this argument is not given, at most 4
-        spots can be detected but the class will work with any number of
-        detected spots between 1 and 4.
+      spots: An instance of the 
+        :class:`~crappy.tool.camera_config.config_tools.SpotsBoxes` tool 
+        containing the coordinates of the spots to track.
+      thresh: The grey level value of the threshold to use for discriminating
+        spots from the background, as an :obj:int`. Passed to the
+        :class:`~crappy.tool.image_processing.video_extenso.tracker.Tracker`
+        and not used in this class.
+      log_level: The minimum logging level of the entire Crappy script, as an
+        :obj:`int`.
+      log_queue: A :obj:`multiprocessing.Queue` for sending the log messages to 
+        the main :obj:`~logging.Logger`, only used in Windows.
+      white_spots: If :obj:`True`, detects white objects over a black
+        background, else black objects over a white background. Passed to the
+        :class:`~crappy.tool.image_processing.video_extenso.tracker.Tracker`
+        and not used in this class.
+      update_thresh: If :obj:`True`, the grey level threshold for detecting the
+        spots is re-calculated at each new image. Otherwise, the first
+        calculated threshold is kept for the entire test. The spots are less
+        likely to be lost with adaptive threshold, but the measurement will be
+        more noisy. Adaptive threshold may also yield inconsistent results when
+        spots are lost. Passed to the 
+        :class:`~crappy.tool.image_processing.video_extenso.tracker.Tracker`
+        and not used in this class.
       safe_mode: If :obj:`True`, the class will stop and raise an exception as
-        soon as overlapping is detected. Otherwise, it will first try to reduce
-        the detection window to get rid of overlapping. This argument should be
-        used when inconsistency in the results may have critical consequences.
+        soon as overlapping spots are detected. Otherwise, it will first try to
+        reduce the detection window to get rid of overlapping. This argument
+        should be used when inconsistency in the results may have critical
+        consequences.
       border: When searching for the new position of a spot, the class will
         search in the last known bounding box of this spot plus a few
         additional pixels in each direction. This argument sets the number of
         additional pixels to use. It should be greater than the expected
-        "speed" of the spots, in pixels / frame. But if it's too big, noise or
-        other spots might hinder the detection.
-      blur: The size in pixels of the kernel to use for applying a median blur
-        to the image before the spot detection. If not given, no blurring is
-        performed. A slight blur improves the spot detection by smoothening the
-        noise, but also takes a bit more time compared to no blurring.
+        "speed" of the spots, in pixels / frame. But if it's set too high,
+        noise or other spots might hinder the detection. Passed to the
+        :class:`~crappy.tool.image_processing.video_extenso.tracker.Tracker`
+        and not used in this class.
+      blur: The size in pixels (as an odd :obj:`int` greater than `1`) of the
+        kernel to use when applying a median blur filter to the image before
+        the spot detection. If not given, no blurring is performed. A slight 
+        blur improves the spot detection by smoothening the noise, but also 
+        takes a bit more time compared to no blurring. Passed to the 
+        :class:`~crappy.tool.image_processing.video_extenso.tracker.Tracker`
+        and not used in this class.
     """
 
     # These attributes will be used later
     self._consecutive_overlaps = 0
     self._trackers = list()
     self._pipes = list()
 
-    if num_spots is not None and num_spots not in range(1, 5):
-      raise ValueError("num_spots should be either None, 1, 2, 3 or 4 !")
-    self._num_spots = num_spots
-
     # Setting the args
     self._white_spots = white_spots
     self._update_thresh = update_thresh
     self._safe_mode = safe_mode
     self._border = border
     self._blur = blur
     self.spots = spots
     self._thresh = thresh
 
     self._logger: Optional[logging.Logger] = None
     self._log_level = log_level
     self._log_queue = log_queue
 
     self._last_warn = time()
+    self._system = system()
 
   def __del__(self) -> None:
     """Security to ensure there are no zombie processes left when exiting."""
 
     self.stop_tracking()
 
   def start_tracking(self) -> None:
-    """Creates a Tracker process for each detected spot, and starts it.
+    """Creates a
+    :class:`~crappy.tool.image_processing.video_extenso.tracker.Tracker`
+    Process for each detected spot, and starts it.
 
-    Also creates a Pipe for each spot to communicate with the Tracker process.
+    Also creates a :obj:`multiprocessing.Pipe` for each spot to communicate 
+    with the Tracker process.
     """
 
     if self.spots.empty():
-      raise AttributeError("[VideoExtenso] No spots selected, aborting !")
+      raise AttributeError("No spots selected, aborting !")
 
     for spot in self.spots:
       if spot is None:
         continue
 
       inlet, outlet = Pipe()
       tracker = Tracker(pipe=outlet,
@@ -126,16 +139,18 @@
                         thresh=None if self._update_thresh else self._thresh,
                         blur=self._blur)
       self._pipes.append(inlet)
       self._trackers.append(tracker)
       tracker.start()
 
   def stop_tracking(self) -> None:
-    """Stops all the active Tracker processes, either gently or by terminating
-    them if they don't stop by themselves."""
+    """Stops all the active 
+    :class:`~crappy.tool.image_processing.video_extenso.tracker.Tracker`
+    Processes, either gently or by terminating them if they don't stop by
+    themselves."""
 
     if any((tracker.is_alive() for tracker in self._trackers)):
       # First, gently asking the trackers to stop
       for pipe, tracker in zip(self._pipes, self._trackers):
         if tracker.is_alive():
           pipe.send(('stop', 'stop', 'stop'))
       sleep(0.1)
@@ -144,26 +159,26 @@
       for tracker in self._trackers:
         if tracker.is_alive():
           self._log(logging.WARNING, "Tracker process did not stop properly, "
                                      "terminating it")
           tracker.terminate()
 
   def get_data(self,
-               img: np.ndarray) -> Optional[Tuple[List[Tuple[float, ...]],
-                                                  float, float]]:
+               img: np.ndarray
+               ) -> Optional[Tuple[List[Tuple[float, ...]], float, float]]:
     """Takes an image as an input, performs spot detection on it, computes the
     strain from the newly detected spots, and returns the spot positions and
     strain values.
 
     Args:
       img: The image on which the spots should be detected.
 
     Returns:
-      A :obj:`list` containing tuples with the coordinates of the centers of
-      the detected spots, and the calculated x and y strain values.
+      A :obj:`list` containing :obj:`tuple` with the coordinates of the centers 
+      of the detected spots, and the calculated x and y strain values.
     """
 
     # Sending the latest sub-image containing the spot to track
     # Also sending the coordinates of the top left pixel
     for pipe, spot in zip(self._pipes, self.spots):
       x_top, x_bottom, y_left, y_right = spot.sorted()
       slice_y = slice(max(0, y_left - self._border),
@@ -250,34 +265,50 @@
     # If only one spot was detected, the strain isn't computed
     else:
       x = self.spots[0].x_centroid
       y = self.spots[0].y_centroid
       return [(y, x)], 0, 0
 
   def _log(self, level: int, msg: str) -> None:
-    """"""
+    """Wrapper for recording log messages.
+
+    Also instantiates the :obj:`~logging.Logger` on the first message.
+
+    Args:
+      level: The logging level of the message, as an :obj:`int`.
+      msg: The message to lof, as a :obj:`str`.
+    """
 
     if self._logger is None:
       self._logger = logging.getLogger(
         f"{current_process().name}.{type(self).__name__}")
 
     self._logger.log(level, msg)
 
   def _send(self,
             conn: Connection,
             val: Union[str, Tuple[int, int, np.ndarray]]) -> None:
-    """"""
+    """Wrapper for sending messages to the Tracker processes.
 
-    if select([], [conn], [], 0)[1]:
-      conn.send(val)
+    In Linux, checks that the Pipe is not full before sending the message.
+
+    Args:
+      conn: The Connection to use for sending the message.
+      val: The message to send to the Tracker process.
+    """
+
+    if self._system == 'Linux':
+      if select([], [conn], [], 0)[1]:
+        conn.send(val)
+      elif time() - self._last_warn > 1:
+          self._last_warn = time()
+          self._log(logging.WARNING, f"Cannot send the image to process to the"
+                                     f" Tracker process, the Pipe is full !")
     else:
-      if time() - self._last_warn > 1:
-        self._last_warn = time()
-        self._log(logging.WARNING, f"Cannot send the image to process to the "
-                                   f"Tracker process, the Pipe is full !")
+      conn.send(val)
 
   @staticmethod
   def _overlap_box(box_1: Box, box_2: Box) -> bool:
     """Determines whether two boxes are overlapping or not."""
 
     x_min_1, x_max_1, y_min_1, y_max_1 = box_1.sorted()
     x_min_2, x_max_2, y_min_2, y_max_2 = box_2.sorted()
```

### Comparing `crappy-2.0.0.dev1/src/crappy/tool/microcontroller.py` & `crappy-2.0.0.dev2/src/crappy/tool/microcontroller.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/src/crappy.egg-info/PKG-INFO` & `crappy-2.0.0.dev2/src/crappy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 Metadata-Version: 2.1
 Name: crappy
-Version: 2.0.0.dev1
-Summary: Command and Real-time Acquisition Parallelized in Python
+Version: 2.0.0.dev2
+Summary: Command and Real-time Acquisition in Parallelized Python
 Home-page: https://github.com/LaboratoireMecaniqueLille/crappy
+Download-URL: https://pypi.org/project/crappy/#files
 Author: LaMcube
 Author-email: antoine.weisrock1@centralelille.fr
+Maintainer: Antoine Weisrock
+Maintainer-email: antoine.weisrock@gmail.com
 License: GPL V2
 Project-URL: Documentation, https://crappy.readthedocs.io/en/latest/index.html
-Keywords: control command acquisition multiprocessing
+Keywords: control,command,acquisition,multiprocessing
 Classifier: Development Status :: 4 - Beta 
 Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Embedded Systems
+Requires-Python: >=3.7
 Provides-Extra: SBC
 Provides-Extra: image
 Provides-Extra: hardware
 Provides-Extra: main
 License-File: LICENSE
 
 =================
```

### Comparing `crappy-2.0.0.dev1/src/crappy.egg-info/SOURCES.txt` & `crappy-2.0.0.dev2/src/crappy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 examples/ready_to_run/custom_out.py
 examples/ready_to_run/dic_ve_fake_test.py
 examples/ready_to_run/dic_ve_simple.py
 examples/ready_to_run/dis_correl_basic.py
 examples/ready_to_run/dis_correl_fake_test.py
 examples/ready_to_run/dis_correl_fake_test_strain_controlled.py
 examples/ready_to_run/displayer.py
-examples/ready_to_run/drawing.py
 examples/ready_to_run/fake_test.py
 examples/ready_to_run/furnace_simulation.py
 examples/ready_to_run/generator.py
 examples/ready_to_run/generator_steps.py
 examples/ready_to_run/mean.py
 examples/ready_to_run/modifiers.py
 examples/ready_to_run/multiplexer.py
@@ -74,49 +73,48 @@
 src/crappy.egg-info/PKG-INFO
 src/crappy.egg-info/SOURCES.txt
 src/crappy.egg-info/dependency_links.txt
 src/crappy.egg-info/not-zip-safe
 src/crappy.egg-info/requires.txt
 src/crappy.egg-info/top_level.txt
 src/crappy/actuator/__init__.py
-src/crappy/actuator/biaxe.py
-src/crappy/actuator/biotens.py
-src/crappy/actuator/cm_drive.py
+src/crappy/actuator/adafruit_dc_motor_hat.py
 src/crappy/actuator/fake_motor.py
-src/crappy/actuator/motor_kit_pump.py
-src/crappy/actuator/oriental.py
+src/crappy/actuator/jvl_mac_140.py
+src/crappy/actuator/kollmorgen_servostar_300.py
+src/crappy/actuator/newport_tra6ppd.py
+src/crappy/actuator/oriental_ard_k.py
 src/crappy/actuator/pololu_tic.py
-src/crappy/actuator/servostar.py
-src/crappy/actuator/tra6ppd.py
+src/crappy/actuator/schneider_mdrive_23.py
 src/crappy/actuator/ft232h/__init__.py
-src/crappy/actuator/ft232h/motor_kit_pump_ft232h.py
+src/crappy/actuator/ft232h/adafruit_dc_motor_hat.py
 src/crappy/actuator/meta_actuator/__init__.py
 src/crappy/actuator/meta_actuator/actuator.py
 src/crappy/actuator/meta_actuator/meta_actuator.py
 src/crappy/blocks/__init__.py
-src/crappy/blocks/auto_drive.py
+src/crappy/blocks/auto_drive_video_extenso.py
+src/crappy/blocks/button.py
 src/crappy/blocks/camera.py
+src/crappy/blocks/canvas.py
 src/crappy/blocks/client_server.py
 src/crappy/blocks/dashboard.py
 src/crappy/blocks/dic_ve.py
 src/crappy/blocks/dis_correl.py
-src/crappy/blocks/drawing.py
 src/crappy/blocks/fake_machine.py
 src/crappy/blocks/generator.py
 src/crappy/blocks/gpu_correl.py
 src/crappy/blocks/gpu_ve.py
 src/crappy/blocks/grapher.py
-src/crappy/blocks/gui.py
 src/crappy/blocks/hdf_recorder.py
 src/crappy/blocks/ioblock.py
+src/crappy/blocks/link_reader.py
 src/crappy/blocks/machine.py
 src/crappy/blocks/mean.py
-src/crappy/blocks/multiplex.py
+src/crappy/blocks/multiplexer.py
 src/crappy/blocks/pid.py
-src/crappy/blocks/reader.py
 src/crappy/blocks/recorder.py
 src/crappy/blocks/sink.py
 src/crappy/blocks/ucontroller.py
 src/crappy/blocks/video_extenso.py
 src/crappy/blocks/camera_processes/__init__.py
 src/crappy/blocks/camera_processes/camera_process.py
 src/crappy/blocks/camera_processes/dic_ve.py
@@ -140,24 +138,23 @@
 src/crappy/blocks/generator_path/meta_path/path.py
 src/crappy/blocks/meta_block/__init__.py
 src/crappy/blocks/meta_block/block.py
 src/crappy/blocks/meta_block/meta_block.py
 src/crappy/camera/__init__.py
 src/crappy/camera/fake_camera.py
 src/crappy/camera/file_reader.py
-src/crappy/camera/gstreamer.py
-src/crappy/camera/opencv.py
-src/crappy/camera/pi_camera.py
+src/crappy/camera/gstreamer_camera.py
+src/crappy/camera/opencv_camera.py
+src/crappy/camera/opencv_camera_basic.py
+src/crappy/camera/raspberry_pi_camera.py
 src/crappy/camera/seek_thermal_pro.py
-src/crappy/camera/webcam.py
-src/crappy/camera/xiapi.py
+src/crappy/camera/ximea_xiapi.py
 src/crappy/camera/cameralink/__init__.py
-src/crappy/camera/cameralink/bispectral.py
-src/crappy/camera/cameralink/cameralink.py
-src/crappy/camera/cameralink/jai.py
+src/crappy/camera/cameralink/basler_ironman_cameralink.py
+src/crappy/camera/cameralink/jai_go_5000c_pmcl.py
 src/crappy/camera/meta_camera/__init__.py
 src/crappy/camera/meta_camera/camera.py
 src/crappy/camera/meta_camera/meta_camera.py
 src/crappy/camera/meta_camera/camera_setting/__init__.py
 src/crappy/camera/meta_camera/camera_setting/camera_bool_setting.py
 src/crappy/camera/meta_camera/camera_setting/camera_choice_setting.py
 src/crappy/camera/meta_camera/camera_setting/camera_scale_setting.py
@@ -166,38 +163,42 @@
 src/crappy/inout/ads1115.py
 src/crappy/inout/agilent_34420A.py
 src/crappy/inout/comedi.py
 src/crappy/inout/daqmx.py
 src/crappy/inout/fake_inout.py
 src/crappy/inout/gpio_pwm.py
 src/crappy/inout/gpio_switch.py
-src/crappy/inout/gsm.py
-src/crappy/inout/kollmorgen.py
+src/crappy/inout/kollmorgen_akd_pdmm.py
 src/crappy/inout/labjack_t7.py
 src/crappy/inout/labjack_t7_streamer.py
 src/crappy/inout/labjack_ue9.py
 src/crappy/inout/mcp9600.py
 src/crappy/inout/mprls.py
 src/crappy/inout/nau7802.py
 src/crappy/inout/ni_daqmx.py
-src/crappy/inout/opsens.py
+src/crappy/inout/opsens_handysens.py
 src/crappy/inout/pijuice_hat.py
-src/crappy/inout/spectrum.py
+src/crappy/inout/sim868.py
+src/crappy/inout/spectrum_m2i4711.py
 src/crappy/inout/waveshare_ad_da.py
 src/crappy/inout/waveshare_high_precision.py
 src/crappy/inout/ft232h/__init__.py
-src/crappy/inout/ft232h/ads1115_ft232h.py
-src/crappy/inout/ft232h/gpio_switch_ft232h.py
-src/crappy/inout/ft232h/mcp9600_ft232h.py
-src/crappy/inout/ft232h/mprls_ft232h.py
-src/crappy/inout/ft232h/nau7802_ft232h.py
-src/crappy/inout/ft232h/waveshare_ad_da_ft232h.py
+src/crappy/inout/ft232h/ads1115.py
+src/crappy/inout/ft232h/gpio_switch.py
+src/crappy/inout/ft232h/mcp9600.py
+src/crappy/inout/ft232h/mprls.py
+src/crappy/inout/ft232h/nau7802.py
+src/crappy/inout/ft232h/waveshare_ad_da.py
 src/crappy/inout/meta_inout/__init__.py
 src/crappy/inout/meta_inout/inout.py
 src/crappy/inout/meta_inout/meta_inout.py
+src/crappy/lamcube/__init__.py
+src/crappy/lamcube/biaxe.py
+src/crappy/lamcube/biotens.py
+src/crappy/lamcube/bispectral.py
 src/crappy/links/__init__.py
 src/crappy/links/link.py
 src/crappy/modifier/__init__.py
 src/crappy/modifier/demux.py
 src/crappy/modifier/differentiate.py
 src/crappy/modifier/integrate.py
 src/crappy/modifier/mean.py
@@ -219,14 +220,15 @@
 src/crappy/tool/camera_config/camera_config.py
 src/crappy/tool/camera_config/camera_config_boxes.py
 src/crappy/tool/camera_config/dic_ve_config.py
 src/crappy/tool/camera_config/dis_correl_config.py
 src/crappy/tool/camera_config/video_extenso_config.py
 src/crappy/tool/camera_config/config_tools/__init__.py
 src/crappy/tool/camera_config/config_tools/box.py
+src/crappy/tool/camera_config/config_tools/histogram_process.py
 src/crappy/tool/camera_config/config_tools/spots_boxes.py
 src/crappy/tool/camera_config/config_tools/spots_detector.py
 src/crappy/tool/camera_config/config_tools/zoom.py
 src/crappy/tool/data/no_image.png
 src/crappy/tool/data/pad.png
 src/crappy/tool/data/speckle.png
 src/crappy/tool/data/ve_markers.tif
```

### Comparing `crappy-2.0.0.dev1/util/set_ft232h_serial_nr.py` & `crappy-2.0.0.dev2/util/set_ft232h_serial_nr.py`

 * *Files identical despite different names*

### Comparing `crappy-2.0.0.dev1/util/udev_rule_setter.sh` & `crappy-2.0.0.dev2/util/udev_rule_setter.sh`

 * *Files identical despite different names*

