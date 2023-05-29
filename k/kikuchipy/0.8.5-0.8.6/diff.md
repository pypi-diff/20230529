# Comparing `tmp/kikuchipy-0.8.5.tar.gz` & `tmp/kikuchipy-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kikuchipy-0.8.5.tar", last modified: Sun May 21 11:44:59 2023, max compression
+gzip compressed data, was "kikuchipy-0.8.6.tar", last modified: Mon May 29 08:45:04 2023, max compression
```

## Comparing `kikuchipy-0.8.5.tar` & `kikuchipy-0.8.6.tar`

### file list

```diff
@@ -1,261 +1,261 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.369459 kikuchipy-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)    52350 2023-05-21 11:44:47.000000 kikuchipy-0.8.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-05-21 11:44:47.000000 kikuchipy-0.8.5/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-21 11:44:47.000000 kikuchipy-0.8.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-21 11:44:47.000000 kikuchipy-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-21 11:44:47.000000 kikuchipy-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-05-21 11:44:59.369459 kikuchipy-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-05-21 11:44:47.000000 kikuchipy-0.8.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-21 11:44:47.000000 kikuchipy-0.8.5/RELEASE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.341459 kikuchipy-0.8.5/kikuchipy/
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.341459 kikuchipy-0.8.5/kikuchipy/_rotation/
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/_rotation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.341459 kikuchipy-0.8.5/kikuchipy/_rotation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/_rotation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/_rotation/tests/test_rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.341459 kikuchipy-0.8.5/kikuchipy/_util/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/_util/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/_util/_transfer_axes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.345459 kikuchipy-0.8.5/kikuchipy/_util/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/_util/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/_util/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/_util/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/_util/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    14809 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.345459 kikuchipy-0.8.5/kikuchipy/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27984 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.345459 kikuchipy-0.8.5/kikuchipy/data/bruker_h5ebsd/
--rw-r--r--   0 runner    (1001) docker     (123)    16614 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/bruker_h5ebsd/create_bruker_h5ebsd_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    73176 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/bruker_h5ebsd/patterns.h5
--rw-r--r--   0 runner    (1001) docker     (123)    59696 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/bruker_h5ebsd/patterns_roi.h5
--rw-r--r--   0 runner    (1001) docker     (123)    55824 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/bruker_h5ebsd/patterns_roi_nonrectangular.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.345459 kikuchipy-0.8.5/kikuchipy/data/edax_binary/
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/edax_binary/create_dummy_edax_binary_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    32416 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/edax_binary/edax_binary.up1
--rw-r--r--   0 runner    (1001) docker     (123)    72042 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/edax_binary/edax_binary.up2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.345459 kikuchipy-0.8.5/kikuchipy/data/edax_h5ebsd/
--rw-r--r--   0 runner    (1001) docker     (123)   938661 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/edax_h5ebsd/patterns.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.345459 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd/
--rw-r--r--   0 runner    (1001) docker     (123)   351168 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd/EBSD_TEST_Ni.h5
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd/create_dummy_emsoft_ebsd_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    35624 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd/simulated_ebsd.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.349459 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/BetheParameters.nml
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/convert_emsoft_ebsd_masterpattern_file_uint8_gzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/create_dummy_emsoft_ebsd_master_pattern_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    61872 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/master_patterns.h5
--rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni.xtal
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni_ebsdmaster.nml
--rw-r--r--   0 runner    (1001) docker     (123)    19638 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc.out
--rw-r--r--   0 runner    (1001) docker     (123)   908492 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc_mp_20kv_uint8_gzip_opts9.h5
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mcopencl.nml
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mp.out
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.349459 kikuchipy-0.8.5/kikuchipy/data/emsoft_ecp_master_pattern/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ecp_master_pattern/create_dummy_emsoft_ecp_master_pattern_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    62296 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ecp_master_pattern/ecp_master_pattern.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.349459 kikuchipy-0.8.5/kikuchipy/data/emsoft_tkd_master_pattern/
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_tkd_master_pattern/create_dummy_emsoft_tkd_master_pattern_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    61600 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_tkd_master_pattern/tkd_master_pattern.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.349459 kikuchipy-0.8.5/kikuchipy/data/kikuchipy_h5ebsd/
--rw-r--r--   0 runner    (1001) docker     (123)   149400 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/kikuchipy_h5ebsd/patterns.h5
--rw-r--r--   0 runner    (1001) docker     (123)    46480 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/kikuchipy_h5ebsd/patterns_nochunks.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.349459 kikuchipy-0.8.5/kikuchipy/data/nordif/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4678 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/nordif/Background acquisition pattern.bmp
--rwxr-xr-x   0 runner    (1001) docker     (123)     4678 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/nordif/Background calibration pattern.bmp
--rwxr-xr-x   0 runner    (1001) docker     (123)     4678 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/nordif/Calibration (294,532).bmp
--rwxr-xr-x   0 runner    (1001) docker     (123)     4678 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/nordif/Calibration (425,447).bmp
--rw-r--r--   0 runner    (1001) docker     (123)    32400 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/nordif/Pattern.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/nordif/Setting.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/nordif/Setting_bad1.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/nordif/Setting_bad2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/nordif/Setting_bad3.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.349459 kikuchipy-0.8.5/kikuchipy/data/oxford_binary/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/oxford_binary/create_dummy_oxford_binary_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    32786 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/oxford_binary/patterns.ebsp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/data/oxford_h5ebsd/
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/oxford_h5ebsd/create_oxford_h5ebsd_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    59152 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/oxford_h5ebsd/patterns.h5oina
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/tests/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/detectors/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14225 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/detectors/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    67124 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/detectors/ebsd_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/detectors/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/detectors/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/detectors/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    39863 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/detectors/tests/test_ebsd_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/draw/
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/draw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/draw/_navigators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/draw/_plot_pattern_positions_in_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/draw/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/draw/markers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/draw/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/draw/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/draw/tests/test_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/draw/tests/test_markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/draw/tests/test_navigators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/draw/tests/test_plot_pattern_positions_in_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/filters/fft_barnes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/filters/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/filters/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/filters/tests/test_fft_barnes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15640 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/filters/tests/test_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/filters/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/generators/
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/generators/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/generators/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10012 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/generators/tests/test_virtual_bse_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/generators/virtual_bse_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/hyperspy_extension.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/imaging/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/imaging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/imaging/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/imaging/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/imaging/tests/test_virtual_bse_imager.py
--rw-r--r--   0 runner    (1001) docker     (123)    16325 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/imaging/vbse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.357459 kikuchipy-0.8.5/kikuchipy/indexing/
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/_dictionary_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12343 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/_hough_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    14530 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/_merge_crystal_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/_orientation_similarity_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.357459 kikuchipy-0.8.5/kikuchipy/indexing/_refinement/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/_refinement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/_refinement/_objective_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    44415 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/_refinement/_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/_refinement/_solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.357459 kikuchipy-0.8.5/kikuchipy/indexing/similarity_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/similarity_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/similarity_metrics/_normalized_cross_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/similarity_metrics/_normalized_dot_product.py
--rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/similarity_metrics/_similarity_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.357459 kikuchipy-0.8.5/kikuchipy/indexing/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/tests/test_dictionary_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    47403 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/tests/test_ebsd_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)    23728 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/tests/test_merge_crystal_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/tests/test_orientation_similarity_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/tests/test_similarity_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.357459 kikuchipy-0.8.5/kikuchipy/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.361459 kikuchipy-0.8.5/kikuchipy/io/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/_emsoft_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    16167 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/bruker_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/ebsd_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/edax_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/edax_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/emsoft_ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/emsoft_ebsd_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/emsoft_ecp_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/emsoft_tkd_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    17736 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/kikuchipy_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    14826 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/nordif.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/nordif_calibration_patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)    19627 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/oxford_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/oxford_h5ebsd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.361459 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_bruker_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_ebsd_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_edax_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_edax_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_emsoft_ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_emsoft_ebsd_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_emsoft_ecp_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_emsoft_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_emsoft_tkd_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_kikuchipy_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_nordif.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_nordif_calibration_patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_oxford_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_oxford_h5ebsd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.361459 kikuchipy-0.8.5/kikuchipy/io/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.361459 kikuchipy-0.8.5/kikuchipy/pattern/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/pattern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25808 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/pattern/_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/pattern/chunk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.361459 kikuchipy-0.8.5/kikuchipy/pattern/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/pattern/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/pattern/tests/test_chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)    18739 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/pattern/tests/test_pattern.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.361459 kikuchipy-0.8.5/kikuchipy/projections/
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/projections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/projections/gnomonic_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/projections/hesse_normal_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/projections/lambert_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/projections/spherical_projection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.365459 kikuchipy-0.8.5/kikuchipy/projections/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/projections/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/projections/tests/test_gnomonic_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/projections/tests/test_hesse_normal_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/projections/tests/test_lambert_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/projections/tests/test_spherical_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.365459 kikuchipy-0.8.5/kikuchipy/signals/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13111 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/_kikuchi_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    22408 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/_kikuchipy_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)   131373 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    18279 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/ebsd_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/ecp_master_pattern.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.365459 kikuchipy-0.8.5/kikuchipy/signals/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    88067 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/tests/test_ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/tests/test_ebsd_hough_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    27376 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/tests/test_ebsd_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/tests/test_ecp_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/tests/test_kikuchi_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/tests/test_virtual_bse_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.365459 kikuchipy-0.8.5/kikuchipy/signals/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/_crystal_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/_map_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    22702 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/_overwrite_hyperspy_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/array_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.365459 kikuchipy-0.8.5/kikuchipy/signals/util/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/tests/test_array_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/tests/test_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/tests/test_overwrite_hyperspy_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/virtual_bse_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.369459 kikuchipy-0.8.5/kikuchipy/simulations/
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/simulations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/simulations/_kikuchi_pattern_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    26644 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/simulations/_kikuchi_pattern_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    27443 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/simulations/kikuchi_pattern_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.369459 kikuchipy-0.8.5/kikuchipy/simulations/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/simulations/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/simulations/tests/test_kikuchi_pattern_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14664 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/simulations/tests/test_kikuchi_pattern_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.341459 kikuchipy-0.8.5/kikuchipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-05-21 11:44:59.000000 kikuchipy-0.8.5/kikuchipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-05-21 11:44:59.000000 kikuchipy-0.8.5/kikuchipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 11:44:59.000000 kikuchipy-0.8.5/kikuchipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-21 11:44:59.000000 kikuchipy-0.8.5/kikuchipy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-21 11:44:59.000000 kikuchipy-0.8.5/kikuchipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-21 11:44:59.000000 kikuchipy-0.8.5/kikuchipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 11:44:59.000000 kikuchipy-0.8.5/kikuchipy.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-21 11:44:59.369459 kikuchipy-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.205722 kikuchipy-0.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    53040 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-05-29 08:45:04.205722 kikuchipy-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/RELEASE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.157722 kikuchipy-0.8.6/kikuchipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.157722 kikuchipy-0.8.6/kikuchipy/_rotation/
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/_rotation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.157722 kikuchipy-0.8.6/kikuchipy/_rotation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/_rotation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/_rotation/tests/test_rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.161722 kikuchipy-0.8.6/kikuchipy/_util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/_util/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/_util/_transfer_axes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.161722 kikuchipy-0.8.6/kikuchipy/_util/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/_util/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/_util/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/_util/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/_util/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14809 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.161722 kikuchipy-0.8.6/kikuchipy/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27981 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.161722 kikuchipy-0.8.6/kikuchipy/data/bruker_h5ebsd/
+-rw-r--r--   0 runner    (1001) docker     (123)    16614 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/bruker_h5ebsd/create_bruker_h5ebsd_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73176 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/bruker_h5ebsd/patterns.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    59696 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/bruker_h5ebsd/patterns_roi.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    55824 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/bruker_h5ebsd/patterns_roi_nonrectangular.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.161722 kikuchipy-0.8.6/kikuchipy/data/edax_binary/
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/edax_binary/create_dummy_edax_binary_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32416 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/edax_binary/edax_binary.up1
+-rw-r--r--   0 runner    (1001) docker     (123)    72042 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/edax_binary/edax_binary.up2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.165722 kikuchipy-0.8.6/kikuchipy/data/edax_h5ebsd/
+-rw-r--r--   0 runner    (1001) docker     (123)   938661 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/edax_h5ebsd/patterns.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.165722 kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd/
+-rw-r--r--   0 runner    (1001) docker     (123)   351168 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd/EBSD_TEST_Ni.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd/create_dummy_emsoft_ebsd_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35624 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd/simulated_ebsd.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.169722 kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd_master_pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd_master_pattern/BetheParameters.nml
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd_master_pattern/convert_emsoft_ebsd_masterpattern_file_uint8_gzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd_master_pattern/create_dummy_emsoft_ebsd_master_pattern_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61872 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd_master_pattern/master_patterns.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd_master_pattern/ni.xtal
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd_master_pattern/ni_ebsdmaster.nml
+-rw-r--r--   0 runner    (1001) docker     (123)    19638 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc.out
+-rw-r--r--   0 runner    (1001) docker     (123)   908492 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc_mp_20kv_uint8_gzip_opts9.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mcopencl.nml
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mp.out
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.169722 kikuchipy-0.8.6/kikuchipy/data/emsoft_ecp_master_pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/emsoft_ecp_master_pattern/create_dummy_emsoft_ecp_master_pattern_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62296 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/emsoft_ecp_master_pattern/ecp_master_pattern.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.169722 kikuchipy-0.8.6/kikuchipy/data/emsoft_tkd_master_pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/emsoft_tkd_master_pattern/create_dummy_emsoft_tkd_master_pattern_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61600 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/emsoft_tkd_master_pattern/tkd_master_pattern.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.169722 kikuchipy-0.8.6/kikuchipy/data/kikuchipy_h5ebsd/
+-rw-r--r--   0 runner    (1001) docker     (123)   149400 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/kikuchipy_h5ebsd/patterns.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    46480 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/kikuchipy_h5ebsd/patterns_nochunks.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.173722 kikuchipy-0.8.6/kikuchipy/data/nordif/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4678 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/nordif/Background acquisition pattern.bmp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4678 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/nordif/Background calibration pattern.bmp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4678 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/nordif/Calibration (294,532).bmp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4678 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/nordif/Calibration (425,447).bmp
+-rw-r--r--   0 runner    (1001) docker     (123)    32400 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/nordif/Pattern.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/nordif/Setting.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/nordif/Setting_bad1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/nordif/Setting_bad2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/nordif/Setting_bad3.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.173722 kikuchipy-0.8.6/kikuchipy/data/oxford_binary/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/oxford_binary/create_dummy_oxford_binary_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32786 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/oxford_binary/patterns.ebsp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.173722 kikuchipy-0.8.6/kikuchipy/data/oxford_h5ebsd/
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/oxford_h5ebsd/create_oxford_h5ebsd_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59152 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/oxford_h5ebsd/patterns.h5oina
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.173722 kikuchipy-0.8.6/kikuchipy/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/data/tests/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.177722 kikuchipy-0.8.6/kikuchipy/detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14225 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/detectors/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67124 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/detectors/ebsd_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.177722 kikuchipy-0.8.6/kikuchipy/detectors/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/detectors/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/detectors/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39863 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/detectors/tests/test_ebsd_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.177722 kikuchipy-0.8.6/kikuchipy/draw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/draw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/draw/_navigators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/draw/_plot_pattern_positions_in_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/draw/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/draw/markers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.177722 kikuchipy-0.8.6/kikuchipy/draw/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/draw/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/draw/tests/test_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/draw/tests/test_markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/draw/tests/test_navigators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/draw/tests/test_plot_pattern_positions_in_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.177722 kikuchipy-0.8.6/kikuchipy/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/filters/fft_barnes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.181722 kikuchipy-0.8.6/kikuchipy/filters/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/filters/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/filters/tests/test_fft_barnes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15640 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/filters/tests/test_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/filters/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.181722 kikuchipy-0.8.6/kikuchipy/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.181722 kikuchipy-0.8.6/kikuchipy/generators/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/generators/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10012 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/generators/tests/test_virtual_bse_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/generators/virtual_bse_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/hyperspy_extension.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.181722 kikuchipy-0.8.6/kikuchipy/imaging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/imaging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.181722 kikuchipy-0.8.6/kikuchipy/imaging/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/imaging/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/imaging/tests/test_virtual_bse_imager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16325 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/imaging/vbse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.181722 kikuchipy-0.8.6/kikuchipy/indexing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/indexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/indexing/_dictionary_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12343 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/indexing/_hough_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14530 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/indexing/_merge_crystal_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/indexing/_orientation_similarity_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.185722 kikuchipy-0.8.6/kikuchipy/indexing/_refinement/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/indexing/_refinement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/indexing/_refinement/_objective_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44415 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/indexing/_refinement/_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/indexing/_refinement/_solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.185722 kikuchipy-0.8.6/kikuchipy/indexing/similarity_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/indexing/similarity_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/indexing/similarity_metrics/_normalized_cross_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/indexing/similarity_metrics/_normalized_dot_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/indexing/similarity_metrics/_similarity_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.185722 kikuchipy-0.8.6/kikuchipy/indexing/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/indexing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/indexing/tests/test_dictionary_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47403 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/indexing/tests/test_ebsd_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23728 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/indexing/tests/test_merge_crystal_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/indexing/tests/test_orientation_similarity_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/indexing/tests/test_similarity_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.185722 kikuchipy-0.8.6/kikuchipy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.189722 kikuchipy-0.8.6/kikuchipy/io/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/_emsoft_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16041 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/bruker_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/ebsd_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/edax_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/edax_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/emsoft_ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/emsoft_ebsd_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/emsoft_ecp_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/emsoft_tkd_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17736 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/kikuchipy_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14826 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/nordif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/nordif_calibration_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19627 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/oxford_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/oxford_h5ebsd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.193722 kikuchipy-0.8.6/kikuchipy/io/plugins/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_bruker_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_ebsd_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_edax_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_edax_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_emsoft_ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_emsoft_ebsd_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_emsoft_ecp_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_emsoft_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_emsoft_tkd_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_kikuchipy_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_nordif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_nordif_calibration_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_oxford_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_oxford_h5ebsd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.193722 kikuchipy-0.8.6/kikuchipy/io/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/io/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.193722 kikuchipy-0.8.6/kikuchipy/pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/pattern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25808 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/pattern/_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/pattern/chunk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.197722 kikuchipy-0.8.6/kikuchipy/pattern/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/pattern/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/pattern/tests/test_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18739 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/pattern/tests/test_pattern.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.197722 kikuchipy-0.8.6/kikuchipy/projections/
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/projections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/projections/gnomonic_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/projections/hesse_normal_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/projections/lambert_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/projections/spherical_projection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.197722 kikuchipy-0.8.6/kikuchipy/projections/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/projections/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/projections/tests/test_gnomonic_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/projections/tests/test_hesse_normal_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/projections/tests/test_lambert_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/projections/tests/test_spherical_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.197722 kikuchipy-0.8.6/kikuchipy/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13111 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/_kikuchi_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22408 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/_kikuchipy_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131373 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18279 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/ebsd_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/ecp_master_pattern.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.201722 kikuchipy-0.8.6/kikuchipy/signals/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88067 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/tests/test_ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/tests/test_ebsd_hough_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27376 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/tests/test_ebsd_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/tests/test_ecp_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/tests/test_kikuchi_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/tests/test_virtual_bse_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.201722 kikuchipy-0.8.6/kikuchipy/signals/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/util/_crystal_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/util/_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/util/_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/util/_map_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22702 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/util/_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/util/_overwrite_hyperspy_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/util/array_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.205722 kikuchipy-0.8.6/kikuchipy/signals/util/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/util/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/util/tests/test_array_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/util/tests/test_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/util/tests/test_overwrite_hyperspy_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/signals/virtual_bse_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.205722 kikuchipy-0.8.6/kikuchipy/simulations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/simulations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/simulations/_kikuchi_pattern_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26644 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/simulations/_kikuchi_pattern_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27443 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/simulations/kikuchi_pattern_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.205722 kikuchipy-0.8.6/kikuchipy/simulations/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/simulations/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/simulations/tests/test_kikuchi_pattern_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14664 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/kikuchipy/simulations/tests/test_kikuchi_pattern_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:45:04.157722 kikuchipy-0.8.6/kikuchipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-05-29 08:45:04.000000 kikuchipy-0.8.6/kikuchipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-05-29 08:45:04.000000 kikuchipy-0.8.6/kikuchipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 08:45:04.000000 kikuchipy-0.8.6/kikuchipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-29 08:45:04.000000 kikuchipy-0.8.6/kikuchipy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-29 08:45:04.000000 kikuchipy-0.8.6/kikuchipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-29 08:45:04.000000 kikuchipy-0.8.6/kikuchipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 08:45:03.000000 kikuchipy-0.8.6/kikuchipy.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-29 08:45:04.205722 kikuchipy-0.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-05-29 08:44:50.000000 kikuchipy-0.8.6/setup.py
```

### Comparing `kikuchipy-0.8.5/CHANGELOG.rst` & `kikuchipy-0.8.6/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,32 @@
 All user facing changes to this project are documented in this file. The format is based
 on `Keep a Changelog <https://keepachangelog.com/en/1.1.0>`__, and this project tries
 its best to adhere to `Semantic Versioning <https://semver.org/spec/v2.0.0.html>`__.
 
 List entries are sorted in descending chronological order. Contributors to each release
 were listed in alphabetical order by first name until version 0.7.0.
 
+0.8.6 (2023-05-29)
+==================
+
+Changed
+-------
+- Use memory mapping (``numpy.memmap()``) instead of reading into memory
+  (``numpy.fromfile()``) for non-lazy reading of EBSD patterns from EDAX binary .up1/2
+  files. (`#641 <https://github.com/pyxem/kikuchipy/pull/641>`_)
+
+Fixed
+-----
+- EBSD patterns from some EDAX binary .up1/2 files were incorrectly read due to an
+  incorrect file offset, making the patterns appear shifted horizontally.
+  (`#641 <https://github.com/pyxem/kikuchipy/pull/641>`_)
+- Reading of EBSD patterns from H5OINA files with the "Camera Binning Mode" dataset not
+  containing the detector binning.
+  (`#641 <https://github.com/pyxem/kikuchipy/pull/641>`_)
+
 0.8.5 (2023-05-21)
 ==================
 
 Fixed
 -----
 - Not-indexed points in crystal maps are handled correctly when merging.
   (`#639 <https://github.com/pyxem/kikuchipy/pull/639>`_)
```

### Comparing `kikuchipy-0.8.5/CODE_OF_CONDUCT.rst` & `kikuchipy-0.8.6/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/LICENSE` & `kikuchipy-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/PKG-INFO` & `kikuchipy-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kikuchipy
-Version: 0.8.5
+Version: 0.8.6
 Summary: Processing, simulating and indexing of electron backscatter diffraction (EBSD) patterns.
 Home-page: https://kikuchipy.org
 Download-URL: https://pypi.python.org/pypi/kikuchipy
 Author: kikuchipy developers
 Author-email: hakon.w.anes@ntnu.no
 Maintainer: Håkon Wiik Ånes
 Maintainer-email: hakon.w.anes@ntnu.no
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kikuchipy Version: 0.8.5 Summary: Processing,
+Metadata-Version: 2.1 Name: kikuchipy Version: 0.8.6 Summary: Processing,
 simulating and indexing of electron backscatter diffraction (EBSD) patterns.
 Home-page: https://kikuchipy.org Download-URL: https://pypi.python.org/pypi/
 kikuchipy Author: kikuchipy developers Author-email: hakon.w.anes@ntnu.no
 Maintainer: HÃ¥kon Wiik Ãnes Maintainer-email: hakon.w.anes@ntnu.no License:
 GPLv3+ Project-URL: Bug Tracker, https://github.com/pyxem/kikuchipy/issues
 Project-URL: Documentation, https://kikuchipy.org Project-URL: Source Code,
 https://github.com/pyxem/kikuchipy Keywords: EBSD,electron backscatter
```

### Comparing `kikuchipy-0.8.5/README.md` & `kikuchipy-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/RELEASE.rst` & `kikuchipy-0.8.6/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/__init__.py` & `kikuchipy-0.8.6/kikuchipy/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/_rotation/__init__.py` & `kikuchipy-0.8.6/kikuchipy/_rotation/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/_rotation/tests/__init__.py` & `kikuchipy-0.8.6/kikuchipy/_rotation/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/_rotation/tests/test_rotation.py` & `kikuchipy-0.8.6/kikuchipy/_rotation/tests/test_rotation.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/_util/__init__.py` & `kikuchipy-0.8.6/kikuchipy/_util/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/_util/_deprecated.py` & `kikuchipy-0.8.6/kikuchipy/_util/_deprecated.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/_util/_transfer_axes.py` & `kikuchipy-0.8.6/kikuchipy/_util/_transfer_axes.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/_util/tests/__init__.py` & `kikuchipy-0.8.6/kikuchipy/_util/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/_util/tests/test_deprecated.py` & `kikuchipy-0.8.6/kikuchipy/_util/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/_util/tests/test_import.py` & `kikuchipy-0.8.6/kikuchipy/_util/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/_util/tests/test_logging.py` & `kikuchipy-0.8.6/kikuchipy/_util/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/conftest.py` & `kikuchipy-0.8.6/kikuchipy/conftest.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/__init__.py` & `kikuchipy-0.8.6/kikuchipy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/_data.py` & `kikuchipy-0.8.6/kikuchipy/data/_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -640,15 +640,15 @@
     Returns
     -------
     ebsd_master_pattern_signal
         EBSD master pattern signal.
 
     See Also
     --------
-    nickel_ebsd_master_pattern_small, si_ebsd_master_pattern
+    nickel_ebsd_master_pattern_small, ebsd_master_pattern
 
     Notes
     -----
     The master patterns are downloaded in HDF5 files (carrying a CC BY
     4.0 license) from Zenodo.
 
     ===========  =========  =================  ============  ==============  ======================
```

### Comparing `kikuchipy-0.8.5/kikuchipy/data/_registry.py` & `kikuchipy-0.8.6/kikuchipy/data/_registry.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/bruker_h5ebsd/create_bruker_h5ebsd_file.py` & `kikuchipy-0.8.6/kikuchipy/data/bruker_h5ebsd/create_bruker_h5ebsd_file.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/bruker_h5ebsd/patterns.h5` & `kikuchipy-0.8.6/kikuchipy/data/bruker_h5ebsd/patterns.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/bruker_h5ebsd/patterns_roi.h5` & `kikuchipy-0.8.6/kikuchipy/data/bruker_h5ebsd/patterns_roi.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/bruker_h5ebsd/patterns_roi_nonrectangular.h5` & `kikuchipy-0.8.6/kikuchipy/data/bruker_h5ebsd/patterns_roi_nonrectangular.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/edax_binary/create_dummy_edax_binary_file.py` & `kikuchipy-0.8.6/kikuchipy/data/edax_binary/create_dummy_edax_binary_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 # You should have received a copy of the GNU General Public License
 # along with kikuchipy. If not, see <http://www.gnu.org/licenses/>.
 
 """Script to create dummy EDAX binary UP1/UP2 files for testing and use
 in the documentation.
 """
 
-import os
 from pathlib import Path
 
 import numpy as np
 
 import kikuchipy as kp
 
 
@@ -31,19 +30,19 @@
 
 sx, sy = s.axes_manager.signal_shape
 n_pixels = sy * sx
 nx, ny = s.axes_manager.navigation_shape
 n_patterns = ny * nx
 step_size = s.axes_manager["x"].scale
 
-dir_data = Path(os.path.dirname(__file__))
+DIR_DATA = Path(__file__).parent
 
 # UP1, version 1
 # --------------
-with open(dir_data / "edax_binary.up1", mode="w") as file1:
+with open(DIR_DATA / "edax_binary.up1", mode="w") as file1:
     # File header: 16 bytes
     # 4 bytes with the file version
     np.array([1], "uint32").tofile(file1)
     # 12 bytes with the pattern width, height and file offset position
     np.array([sx, sy, 16], "uint32").tofile(file1)
 
     # Patterns
@@ -53,15 +52,15 @@
 # --------------
 # With hexagonal grid, assuming this grid (patterns as "x"):
 # ------- #
 #  x x x  #
 # x x x x #
 #  x x x  #
 # ------- #
-with open(dir_data / "edax_binary.up2", mode="w") as file2:
+with open(DIR_DATA / "edax_binary.up2", mode="w") as file2:
     # File header: 42 bytes
     # 4 bytes with the file version
     np.array([3], "uint32").tofile(file2)
     # 12 bytes with the pattern width, height and file offset position
     np.array([sx, sy, 42], "uint32").tofile(file2)
     # 1 byte with any "extra patterns" (?)
     np.array([1], "uint8").tofile(file2)
```

### Comparing `kikuchipy-0.8.5/kikuchipy/data/edax_binary/edax_binary.up1` & `kikuchipy-0.8.6/kikuchipy/data/edax_binary/edax_binary.up1`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/edax_binary/edax_binary.up2` & `kikuchipy-0.8.6/kikuchipy/data/edax_binary/edax_binary.up2`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/edax_h5ebsd/patterns.h5` & `kikuchipy-0.8.6/kikuchipy/data/edax_h5ebsd/patterns.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd/EBSD_TEST_Ni.h5` & `kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd/EBSD_TEST_Ni.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd/create_dummy_emsoft_ebsd_file.py` & `kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd/create_dummy_emsoft_ebsd_file.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd/simulated_ebsd.h5` & `kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd/simulated_ebsd.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/convert_emsoft_ebsd_masterpattern_file_uint8_gzip.py` & `kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd_master_pattern/convert_emsoft_ebsd_masterpattern_file_uint8_gzip.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/create_dummy_emsoft_ebsd_master_pattern_file.py` & `kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd_master_pattern/create_dummy_emsoft_ebsd_master_pattern_file.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/master_patterns.h5` & `kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd_master_pattern/master_patterns.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni.xtal` & `kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd_master_pattern/ni.xtal`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni_ebsdmaster.nml` & `kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd_master_pattern/ni_ebsdmaster.nml`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc.out` & `kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc.out`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc_mp_20kv_uint8_gzip_opts9.h5` & `kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc_mp_20kv_uint8_gzip_opts9.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mcopencl.nml` & `kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mcopencl.nml`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mp.out` & `kikuchipy-0.8.6/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mp.out`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/emsoft_ecp_master_pattern/create_dummy_emsoft_ecp_master_pattern_file.py` & `kikuchipy-0.8.6/kikuchipy/data/emsoft_ecp_master_pattern/create_dummy_emsoft_ecp_master_pattern_file.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/emsoft_ecp_master_pattern/ecp_master_pattern.h5` & `kikuchipy-0.8.6/kikuchipy/data/emsoft_ecp_master_pattern/ecp_master_pattern.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/emsoft_tkd_master_pattern/create_dummy_emsoft_tkd_master_pattern_file.py` & `kikuchipy-0.8.6/kikuchipy/data/emsoft_tkd_master_pattern/create_dummy_emsoft_tkd_master_pattern_file.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/emsoft_tkd_master_pattern/tkd_master_pattern.h5` & `kikuchipy-0.8.6/kikuchipy/data/emsoft_tkd_master_pattern/tkd_master_pattern.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/kikuchipy_h5ebsd/patterns.h5` & `kikuchipy-0.8.6/kikuchipy/data/kikuchipy_h5ebsd/patterns.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/kikuchipy_h5ebsd/patterns_nochunks.h5` & `kikuchipy-0.8.6/kikuchipy/data/kikuchipy_h5ebsd/patterns_nochunks.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/nordif/Background acquisition pattern.bmp` & `kikuchipy-0.8.6/kikuchipy/data/nordif/Background acquisition pattern.bmp`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/nordif/Background calibration pattern.bmp` & `kikuchipy-0.8.6/kikuchipy/data/nordif/Background calibration pattern.bmp`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/nordif/Calibration (294,532).bmp` & `kikuchipy-0.8.6/kikuchipy/data/nordif/Calibration (294,532).bmp`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/nordif/Calibration (425,447).bmp` & `kikuchipy-0.8.6/kikuchipy/data/nordif/Calibration (425,447).bmp`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/nordif/Pattern.dat` & `kikuchipy-0.8.6/kikuchipy/data/nordif/Pattern.dat`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/nordif/Setting.txt` & `kikuchipy-0.8.6/kikuchipy/data/nordif/Setting.txt`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/nordif/Setting_bad1.txt` & `kikuchipy-0.8.6/kikuchipy/data/nordif/Setting_bad1.txt`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/nordif/Setting_bad2.txt` & `kikuchipy-0.8.6/kikuchipy/data/nordif/Setting_bad2.txt`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/nordif/Setting_bad3.txt` & `kikuchipy-0.8.6/kikuchipy/data/nordif/Setting_bad3.txt`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/oxford_binary/create_dummy_oxford_binary_file.py` & `kikuchipy-0.8.6/kikuchipy/data/oxford_binary/create_dummy_oxford_binary_file.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/oxford_binary/patterns.ebsp` & `kikuchipy-0.8.6/kikuchipy/data/oxford_binary/patterns.ebsp`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/oxford_h5ebsd/create_oxford_h5ebsd_file.py` & `kikuchipy-0.8.6/kikuchipy/data/oxford_h5ebsd/create_oxford_h5ebsd_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 """Creation of a dummy Oxford Instruments h5ebsd file (H5OINA) used when
 testing the Oxford h5ebsd reader.
 
 Only the groups and datasets read in the reader are included.
 """
 
-import os
+from pathlib import Path
 
 from h5py import File
 import numpy as np
 from orix.quaternion import Rotation
 
 import kikuchipy as kp
 
@@ -38,18 +38,18 @@
 
 s = kp.data.nickel_ebsd_small()
 ny, nx = s._navigation_shape_rc
 n = ny * nx
 sy, sx = s._signal_shape_rc
 dx = s.axes_manager["x"].scale
 
-dir_data = os.path.abspath(os.path.dirname(__file__))
+dir_data = Path(__file__).parent
 
 
-f = File(os.path.join(dir_data, "patterns.h5oina"), mode="w")
+f = File(dir_data / "patterns.h5oina", mode="w")
 
 # Top group
 f.create_dataset("Format Version", data=b"5.0")
 f.create_dataset("Index", data=b"1")
 f.create_dataset("Manufacturer", data=b"Oxford Instruments")
 f.create_dataset("Software Version", data=b"6.0.8014.1")
 scan = f.create_group("1")
```

### Comparing `kikuchipy-0.8.5/kikuchipy/data/oxford_h5ebsd/patterns.h5oina` & `kikuchipy-0.8.6/kikuchipy/data/oxford_h5ebsd/patterns.h5oina`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/tests/__init__.py` & `kikuchipy-0.8.6/kikuchipy/data/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/data/tests/test_data.py` & `kikuchipy-0.8.6/kikuchipy/data/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/detectors/__init__.py` & `kikuchipy-0.8.6/kikuchipy/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/detectors/calibration.py` & `kikuchipy-0.8.6/kikuchipy/detectors/calibration.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/detectors/ebsd_detector.py` & `kikuchipy-0.8.6/kikuchipy/detectors/ebsd_detector.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/detectors/tests/__init__.py` & `kikuchipy-0.8.6/kikuchipy/detectors/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/detectors/tests/test_calibration.py` & `kikuchipy-0.8.6/kikuchipy/detectors/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/detectors/tests/test_ebsd_detector.py` & `kikuchipy-0.8.6/kikuchipy/detectors/tests/test_ebsd_detector.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/draw/__init__.py` & `kikuchipy-0.8.6/kikuchipy/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/draw/_navigators.py` & `kikuchipy-0.8.6/kikuchipy/draw/_navigators.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/draw/_plot_pattern_positions_in_map.py` & `kikuchipy-0.8.6/kikuchipy/draw/_plot_pattern_positions_in_map.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/draw/colors.py` & `kikuchipy-0.8.6/kikuchipy/draw/colors.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/draw/markers.py` & `kikuchipy-0.8.6/kikuchipy/draw/markers.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/draw/tests/__init__.py` & `kikuchipy-0.8.6/kikuchipy/draw/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/draw/tests/test_colors.py` & `kikuchipy-0.8.6/kikuchipy/draw/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/draw/tests/test_markers.py` & `kikuchipy-0.8.6/kikuchipy/draw/tests/test_markers.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/draw/tests/test_navigators.py` & `kikuchipy-0.8.6/kikuchipy/draw/tests/test_navigators.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/draw/tests/test_plot_pattern_positions_in_map.py` & `kikuchipy-0.8.6/kikuchipy/draw/tests/test_plot_pattern_positions_in_map.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/filters/__init__.py` & `kikuchipy-0.8.6/kikuchipy/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/filters/fft_barnes.py` & `kikuchipy-0.8.6/kikuchipy/filters/fft_barnes.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/filters/tests/__init__.py` & `kikuchipy-0.8.6/kikuchipy/filters/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/filters/tests/test_fft_barnes.py` & `kikuchipy-0.8.6/kikuchipy/filters/tests/test_fft_barnes.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/filters/tests/test_window.py` & `kikuchipy-0.8.6/kikuchipy/filters/tests/test_window.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/filters/window.py` & `kikuchipy-0.8.6/kikuchipy/filters/window.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/generators/__init__.py` & `kikuchipy-0.8.6/kikuchipy/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/generators/tests/__init__.py` & `kikuchipy-0.8.6/kikuchipy/generators/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/generators/tests/test_virtual_bse_generator.py` & `kikuchipy-0.8.6/kikuchipy/generators/tests/test_virtual_bse_generator.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/generators/virtual_bse_generator.py` & `kikuchipy-0.8.6/kikuchipy/generators/virtual_bse_generator.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/hyperspy_extension.yaml` & `kikuchipy-0.8.6/kikuchipy/hyperspy_extension.yaml`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/imaging/__init__.py` & `kikuchipy-0.8.6/kikuchipy/imaging/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/imaging/tests/__init__.py` & `kikuchipy-0.8.6/kikuchipy/imaging/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/imaging/tests/test_virtual_bse_imager.py` & `kikuchipy-0.8.6/kikuchipy/imaging/tests/test_virtual_bse_imager.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/imaging/vbse.py` & `kikuchipy-0.8.6/kikuchipy/imaging/vbse.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/indexing/__init__.py` & `kikuchipy-0.8.6/kikuchipy/indexing/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/indexing/_dictionary_indexing.py` & `kikuchipy-0.8.6/kikuchipy/indexing/_dictionary_indexing.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/indexing/_hough_indexing.py` & `kikuchipy-0.8.6/kikuchipy/indexing/_hough_indexing.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/indexing/_merge_crystal_maps.py` & `kikuchipy-0.8.6/kikuchipy/indexing/_merge_crystal_maps.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/indexing/_orientation_similarity_map.py` & `kikuchipy-0.8.6/kikuchipy/indexing/_orientation_similarity_map.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/indexing/_refinement/__init__.py` & `kikuchipy-0.8.6/kikuchipy/indexing/_refinement/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/indexing/_refinement/_objective_functions.py` & `kikuchipy-0.8.6/kikuchipy/indexing/_refinement/_objective_functions.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/indexing/_refinement/_refinement.py` & `kikuchipy-0.8.6/kikuchipy/indexing/_refinement/_refinement.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/indexing/_refinement/_solvers.py` & `kikuchipy-0.8.6/kikuchipy/indexing/_refinement/_solvers.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/indexing/similarity_metrics/__init__.py` & `kikuchipy-0.8.6/kikuchipy/indexing/similarity_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/indexing/similarity_metrics/_normalized_cross_correlation.py` & `kikuchipy-0.8.6/kikuchipy/indexing/similarity_metrics/_normalized_cross_correlation.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/indexing/similarity_metrics/_normalized_dot_product.py` & `kikuchipy-0.8.6/kikuchipy/indexing/similarity_metrics/_normalized_dot_product.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/indexing/similarity_metrics/_similarity_metric.py` & `kikuchipy-0.8.6/kikuchipy/indexing/similarity_metrics/_similarity_metric.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/indexing/tests/__init__.py` & `kikuchipy-0.8.6/kikuchipy/indexing/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/indexing/tests/test_dictionary_indexing.py` & `kikuchipy-0.8.6/kikuchipy/indexing/tests/test_dictionary_indexing.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/indexing/tests/test_ebsd_refinement.py` & `kikuchipy-0.8.6/kikuchipy/indexing/tests/test_ebsd_refinement.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/indexing/tests/test_merge_crystal_maps.py` & `kikuchipy-0.8.6/kikuchipy/indexing/tests/test_merge_crystal_maps.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/indexing/tests/test_orientation_similarity_map.py` & `kikuchipy-0.8.6/kikuchipy/indexing/tests/test_orientation_similarity_map.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/indexing/tests/test_similarity_metrics.py` & `kikuchipy-0.8.6/kikuchipy/indexing/tests/test_similarity_metrics.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/__init__.py` & `kikuchipy-0.8.6/kikuchipy/io/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/_io.py` & `kikuchipy-0.8.6/kikuchipy/io/_io.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/_util.py` & `kikuchipy-0.8.6/kikuchipy/io/_util.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/__init__.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/_emsoft_master_pattern.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/_emsoft_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/_h5ebsd.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/_h5ebsd.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,16 +41,15 @@
     Parameters
     ----------
     group
         HDF5 group object.
     dictionary
         To fill dataset values into.
     recursive
-        Whether to add subgroups to ``dictionary`` (default is
-        ``False``).
+        Whether to add subgroups to ``dictionary`` (default is False).
     data_dset_names
         List of names of HDF5 data sets with data to not read.
 
     Returns
     -------
     dictionary
         Dataset values in group (and subgroups if ``recursive=True``).
@@ -167,18 +166,18 @@
         datasets containing manufacturer, version and scans in the top
         group.
 
         Raises
         ------
         IOError
             If there are no datasets in the top group named
-            ``"manufacturer"`` and ``"version"``, or if there are no
-            groups in the top group containing the datasets
-            ``"EBSD/Data"`` and ``"EBSD/Header"``, or if there is no
-            reader for the file ``"manufacturer"``.
+            "manufacturer" and "version", or if there are no groups in
+            the top group containing the datasets
+            "EBSD/Data" and "EBSD/Header", or if there is no reader for
+            the file "manufacturer".
         """
         error = None
         if self.manufacturer is None or self.version is None:
             error = "manufacturer and/or version could not be read from its top group"
         elif not any(
             "EBSD/Data" in group and "EBSD/Header" in group
             for group in self.scan_groups
@@ -287,15 +286,15 @@
         ----------
         group
             Group with patterns.
         data_shape
             Output shape of pattern array, (ny, nx, sy, sx) = (
             map rows, map columns, pattern rows, pattern columns).
         lazy
-            Whether to read dataset lazily (default is ``False``).
+            Whether to read dataset lazily (default is False).
         indices
             Mapping from pattern entry in the file to the 2D map, only
             used in the Bruker Nano reader.
 
         Returns
         -------
         data
@@ -357,18 +356,18 @@
     @staticmethod
     def get_axes_list(data_shape: tuple, data_scale: tuple) -> List[dict]:
         """Return a description of each data axis.
 
         Parameters
         ----------
         data_shape
-            4D shape of pattern array, ``(ny, nx, sy, sx)`` = (
-            map rows, map columns, pattern rows, pattern columns).
+            4D shape of pattern array, (ny, nx, sy, sx) = ( map rows,
+            map columns, pattern rows, pattern columns).
         data_scale
-            Map scale and detector pixel size, ``(dy, dx, px_size)``.
+            Map scale and detector pixel size, (dy, dx, px_size).
 
         Returns
         -------
         axes_list
             Description of each data axis as a list of dictionaries.
         """
         ny, nx, sy, sx = data_shape
@@ -450,23 +449,23 @@
 
         Parameters
         ----------
         group_names
             Name or a list of names of the desired top HDF5 group(s). If
             not given, the first scan group is returned.
         lazy
-            Read dataset lazily (default is ``False``). If ``False``,
-            the file is closed after reading.
+            Read dataset lazily (default is False). If False, the file
+            is closed after reading.
 
         Returns
         -------
         scan_list
-            List of dictionaries with keys ``"axes"``, ``"data"``,
-            ``"metadata"``, ``"original_metadata"``, ``"detector"``,
-            (possibly) ``"static_background"``, and ``"xmap"``.
+            List of dictionaries with keys "axes", "data", "metadata",
+            "original_metadata", "detector", (possibly)
+            "static_background", and "xmap".
         """
         scan_dict_list = []
         for scan in self.get_desired_scan_groups(group_names):
             scan_dict_list.append(self.scan2dict(scan, lazy))
 
         if not lazy:
             self.file.close()
@@ -478,19 +477,18 @@
         """Read (possibly lazily) patterns from group.
 
         Parameters
         ----------
         group
             HDF5 group with patterns.
         lazy
-            Read dataset lazily (default is ``False``).
+            Read dataset lazily (default is False).
 
         Returns
         -------
         scan_dict
-            Dictionary with keys ``"axes"``, ``"data"``, ``"metadata"``,
-            ``"original_metadata"``, ``"detector"``,
-            ``"static_background"``, and ``"xmap"``. This dictionary can
-             be passed as keyword arguments to create an
-             :class:`~kikuchipy.signals.EBSD` signal.
+            Dictionary with keys "axes", "data", "metadata",
+            "original_metadata", "detector", "static_background", and
+            "xmap". This dictionary can be passed as keyword arguments
+            to create an :class:`~kikuchipy.signals.EBSD` signal.
         """
         return NotImplemented  # pragma: no cover
```

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/bruker_h5ebsd.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/bruker_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/ebsd_directory.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/ebsd_directory.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/edax_binary.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/edax_binary.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # along with kikuchipy. If not, see <http://www.gnu.org/licenses/>.
 
 """Reader of EBSD data from EDAX TSL UP1/2 files.
 
 The reader is adapted from the EDAX UP1/2 reader in PyEBSDIndex.
 """
 
-import os
 from pathlib import Path
 from typing import BinaryIO, Dict, List, Optional, Tuple, Union
 import warnings
 
 import dask.array as da
 import numpy as np
 
@@ -35,17 +34,16 @@
 
 
 # Plugin characteristics
 # ----------------------
 format_name = "EDAX binary"
 description = (
     "Read support for electron backscatter diffraction patterns stored "
-    "in a binary file formatted in EDAX TSL's UP1/UP2 format with file "
-    "extension '.up1' or '.up2'. The reader is adapted from the EDAX "
-    "UP1/2 reader in PyEBSDIndex."
+    "in a binary EDAX TSL's UP1/UP2 file extension '.up1' or '.up2'. "
+    "The reader is adapted from the EDAX UP1/2 reader in PyEBSDIndex."
 )
 full_support = False
 # Recognised file extension
 file_extensions = ["up1", "up2"]
 default_extension = 0
 # Writing capabilities (signal dimensions, navigation dimensions)
 writes = False
@@ -71,15 +69,15 @@
         be attempted to be determined from the file. If it could not be,
         the returned signal will have only one navigation dimension. If
         patterns were acquired in an hexagonal grid, the returned signal
         will have only one navigation dimension irrespective of this
         parameter's value.
     lazy
         Read the data lazily without actually reading the data from disk
-        until required. Default is ``False``.
+        until required. Default is False.
 
     Returns
     -------
     scan
         Data, axes, metadata and original metadata.
 
     Raises
@@ -99,32 +97,32 @@
 
     Notes
     -----
     Reader adapted from the EDAX UP1/2 reader in PyEBSDIndex.
     """
     with open(filename, mode="rb") as f:
         reader = EDAXBinaryFileReader(f)
-        scan = reader.read_scan(nav_shape=nav_shape, lazy=lazy)
+        scan = reader.read_scan(nav_shape, lazy)
     return [scan]
 
 
 class EDAXBinaryFileReader:
     """EDAX TSL's binary UP1/2 file reader.
 
     Parameters
     ----------
     file
         Open EDAX binary UP1/2 file with uncompressed patterns.
     """
 
     def __init__(self, file: BinaryIO):
         """Prepare to read EBSD patterns from an open EDAX UP1/2 file."""
-        self.file = file  # Already open file
+        self.file = file
 
-        ext = os.path.splitext(file.name)[1][1:].lower()
+        ext = Path(file.name).suffix[1:].lower()
         self.dtype = {"up1": np.uint8, "up2": np.uint16}[ext]
 
         file.seek(0)
         self.version = np.fromfile(self.file, "uint32", 1)[0]
         if self.version == 2:
             raise ValueError("Only files with version 1 or >= 3, not 2, can be read")
 
@@ -136,35 +134,36 @@
         dictionary
         """
         self.file.seek(4)
         sx, sy, pattern_offset = np.fromfile(self.file, "uint32", count=3)
         file_size = Path(self.file.name).stat().st_size
 
         if self.version == 1:
-            n_patterns = int(
-                (file_size - pattern_offset) / (sx * sy * self.dtype(0).nbytes)
-            )
+            n_patterns = (file_size - pattern_offset) / (sx * sy * self.dtype(0).nbytes)
+            n_patterns = int(n_patterns)
             nx, ny = n_patterns, 1
             dx, dy = 1, 1
             is_hex = False
         else:  # Version >= 3
             nx, ny = np.fromfile(self.file, "uint32", 2, offset=1)
 
-            is_hex = bool(np.fromfile(self.file, "uint8", 1)[0])
+            is_hex = np.fromfile(self.file, "uint8", 1)[0]
+            is_hex = bool(is_hex)
             if is_hex:
                 warnings.warn(
                     "Returned signal has one navigation dimension since an hexagonal "
                     "grid is not supported"
                 )
-                n_patterns = int(
-                    (file_size - pattern_offset) / (sx * sy * self.dtype(0).nbytes)
+                n_patterns = (file_size - pattern_offset) / (
+                    sx * sy * self.dtype(0).nbytes
                 )
+                n_patterns = int(n_patterns)
                 nx, ny = n_patterns, 1
             else:
-                n_patterns = int(nx * ny)
+                n_patterns = nx * ny
 
             dx, dy = np.fromfile(self.file, "float64", 2)
 
         return {
             "sx": sx,
             "sy": sy,
             "pattern_offset": pattern_offset,
@@ -181,17 +180,17 @@
     ) -> dict:
         """Return a dictionary with scan information and patterns.
 
         Parameters
         ----------
         nav_shape
             Navigation shape, as (n map rows, n map columns). Default is
-            ``None``.
+            None.
         lazy
-            Whether to reader patterns lazily. Default is ``False``.
+            Whether to reader patterns lazily. Default is False.
 
         Returns
         -------
         dictionary
             Dictionary of scan information.
         """
         header = self.read_header()
@@ -202,39 +201,36 @@
             if n_patterns != header["n_patterns"]:
                 raise ValueError(
                     f"Given `nav_shape` {nav_shape} does not match the number of "
                     f"patterns in the file, {header['n_patterns']}."
                 )
         else:
             ny, nx = header["ny"], header["nx"]
-            n_patterns = header["n_patterns"]
 
         sy, sx = header["sy"], header["sx"]
         data_shape = (ny, nx, sy, sx)
         if ny == 1:
             data_shape = data_shape[1:]
         ndim = len(data_shape)
         nav_dim = ndim - 2
 
+        data = np.memmap(
+            self.file.name,
+            dtype=self.dtype,
+            shape=data_shape,
+            mode="c",
+            offset=header["pattern_offset"],
+        )
+
         if lazy:
-            data = np.memmap(
-                self.file,
-                dtype=self.dtype,
-                shape=data_shape,
-                mode="r",
-                offset=header["pattern_offset"],
-            )
             data = da.from_array(data)
             chunks = get_chunking(
                 data_shape=data_shape, nav_dim=nav_dim, sig_dim=2, dtype=self.dtype
             )
             data = data.rechunk(chunks)
-        else:
-            data = np.fromfile(self.file, self.dtype, n_patterns * sy * sx)
-            data = data.reshape(data_shape)
 
         units = ["um"] * ndim
         scales = [header["dy"], header["dx"]] + [1, 1][:nav_dim]
         axes_names = ["y", "x"][-nav_dim:] + ["dy", "dx"]
         axes = [
             {
                 "size": data.shape[i],
@@ -243,22 +239,18 @@
                 "scale": scales[i],
                 "offset": 0.0,
                 "units": units[i],
             }
             for i in range(ndim)
         ]
         fname = self.file.name
-        metadata = dict(
-            General=dict(
-                original_filename=fname,
-                title=os.path.splitext(os.path.split(fname)[1])[0],
-            ),
-            Signal=dict(signal_type="EBSD", record_by="image"),
-        )
+        metadata = {
+            "General": {
+                "original_filename": fname,
+                "title": Path(fname).stem,
+            },
+            "Signal": {"signal_type": "EBSD", "record_by": "image"},
+        }
 
-        scan = dict(
-            axes=axes,
-            data=data,
-            metadata=metadata,
-        )
+        scan = {"axes": axes, "data": data, "metadata": metadata}
 
         return scan
```

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/edax_h5ebsd.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/edax_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/emsoft_ebsd.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/emsoft_ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/emsoft_ebsd_master_pattern.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/emsoft_ebsd_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/emsoft_ecp_master_pattern.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/emsoft_ecp_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/emsoft_tkd_master_pattern.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/emsoft_tkd_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/kikuchipy_h5ebsd.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/kikuchipy_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/nordif.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/nordif.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/nordif_calibration_patterns.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/nordif_calibration_patterns.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/oxford_binary.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/oxford_binary.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/oxford_h5ebsd.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/oxford_h5ebsd.py`

 * *Files 18% similar despite different names*

```diff
@@ -76,24 +76,23 @@
         """Read (possibly lazily) patterns from group.
 
         Parameters
         ----------
         group
             Group with patterns.
         lazy
-            Whether to read dataset lazily (default is ``False``).
+            Whether to read dataset lazily (default is False).
 
         Returns
         -------
         scan_dict
-            Dictionary with keys ``"axes"``, ``"data"``, ``"metadata"``,
-            ``"original_metadata"``, ``"detector"``,
-            ``"static_background"``, and ``"xmap"``. This dictionary can
-             be passed as keyword arguments to create an
-             :class:`~kikuchipy.signals.EBSD` signal.
+            Dictionary with keys "axes", "data", "metadata",
+            "original_metadata", "detector", "static_background", and
+            "xmap". This dictionary can be passed as keyword arguments
+            to create an :class:`~kikuchipy.signals.EBSD` signal.
 
         Raises
         ------
         IOError
             If patterns are not acquired in a square grid.
         """
         hd = _hdf5group2dict(group["EBSD/Header"], recursive=True)
@@ -156,22 +155,22 @@
         detector_kw = dict(
             shape=(sy, sx),
             pc=pc,
             sample_tilt=np.rad2deg(hd.get("Tilt Angle", np.deg2rad(70))),
             convention="oxford",
         )
         detector_tilt_euler = hd.get("Detector Orientation Euler")
-        binning_str = hd.get("Camera Binning Mode")
         try:
             detector_kw["tilt"] = np.rad2deg(detector_tilt_euler[1]) - 90
         except (IndexError, TypeError):  # pragma: no cover
             _logger.debug("Could not read detector tilt")
+        binning_str = hd.get("Camera Binning Mode")
         try:
             detector_kw["binning"] = int(binning_str.split("x")[0])
-        except IndexError:  # pragma: no cover
+        except (IndexError, ValueError):  # pragma: no cover
             _logger.debug("Could not read detector binning")
         scan_dict["detector"] = EBSDDetector(**detector_kw)
 
         return scan_dict
 
 
 def file_reader(
@@ -193,22 +192,21 @@
     scan_group_names
         Name or a list of names of HDF5 top group(s) containing the
         scan(s) to return. If not given (default), the first scan in the
         file is returned.
     lazy
         Open the data lazily without actually reading the data from disk
         until required. Allows opening arbitrary sized datasets. Default
-        is ``False``.
+        is False.
     **kwargs
         Keyword arguments passed to :class:`h5py.File`.
 
     Returns
     -------
     scan_dict_list
-        List of one or more dictionaries with the keys ``"axes"``,
-        ``"data"``, ``"metadata"``, ``"original_metadata"``,
-        ``"detector"``, and ``"xmap"``. This
+        List of one or more dictionaries with the keys "axes", "data",
+        "metadata", "original_metadata", "detector", and "xmap". This
         dictionary can be passed as keyword arguments to create an
         :class:`~kikuchipy.signals.EBSD` signal.
     """
     reader = OxfordH5EBSDReader(filename, **kwargs)
     return reader.read(scan_group_names, lazy)
```

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/__init__.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_bruker_h5ebsd.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_bruker_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_ebsd_directory.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_ebsd_directory.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_edax_binary.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_edax_binary.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,27 +11,26 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with kikuchipy. If not, see <http://www.gnu.org/licenses/>.
 
-import os
+from pathlib import Path
 
 import dask.array as da
 import numpy as np
 import pytest
 
 import kikuchipy as kp
 
 
-DIR_PATH = os.path.dirname(__file__)
-EDAX_PATH = os.path.join(DIR_PATH, "../../../data/edax_binary")
-FILE_UP1 = os.path.join(EDAX_PATH, "edax_binary.up1")
-FILE_UP2 = os.path.join(EDAX_PATH, "edax_binary.up2")
+EDAX_PATH = Path(__file__).parent / "../../../data/edax_binary"
+FILE_UP1 = EDAX_PATH / "edax_binary.up1"
+FILE_UP2 = EDAX_PATH / "edax_binary.up2"
 
 
 class TestEDAXBinaryReader:
     def test_load_up1(self):
         """Load UP1 file into memory."""
         s = kp.data.nickel_ebsd_small()
         s1 = kp.load(FILE_UP1)
```

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_edax_h5ebsd.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_edax_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_emsoft_ebsd.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_emsoft_ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_emsoft_ebsd_master_pattern.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_emsoft_ebsd_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_emsoft_ecp_master_pattern.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_emsoft_ecp_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_emsoft_master_pattern.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_emsoft_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_emsoft_tkd_master_pattern.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_emsoft_tkd_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_kikuchipy_h5ebsd.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_kikuchipy_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_nordif.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_nordif.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_nordif_calibration_patterns.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_nordif_calibration_patterns.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_oxford_binary.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_oxford_binary.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_oxford_h5ebsd.py` & `kikuchipy-0.8.6/kikuchipy/io/plugins/tests/test_oxford_h5ebsd.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,25 +11,23 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with kikuchipy. If not, see <http://www.gnu.org/licenses/>.
 
-import os
+from pathlib import Path
 
 import numpy as np
 
 import kikuchipy as kp
 from kikuchipy.conftest import assert_dictionary
 
 
-DIR_PATH = os.path.dirname(__file__)
-DATA_PATH = os.path.join(DIR_PATH, "../../../data")
-OXFORD_FILE = os.path.join(DATA_PATH, "oxford_h5ebsd/patterns.h5oina")
+OXFORD_FILE = Path(__file__).parent / "../../../data/oxford_h5ebsd/patterns.h5oina"
 
 
 class TestOxfordH5EBSD:
     def test_load(self, tmp_path, ni_small_axes_manager):
         s = kp.load(OXFORD_FILE)
         assert s.data.shape == (3, 3, 60, 60)
         assert_dictionary(s.axes_manager.as_dictionary(), ni_small_axes_manager)
```

### Comparing `kikuchipy-0.8.5/kikuchipy/io/tests/__init__.py` & `kikuchipy-0.8.6/kikuchipy/io/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/tests/test_io.py` & `kikuchipy-0.8.6/kikuchipy/io/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/io/tests/test_util.py` & `kikuchipy-0.8.6/kikuchipy/io/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/pattern/__init__.py` & `kikuchipy-0.8.6/kikuchipy/pattern/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/pattern/_pattern.py` & `kikuchipy-0.8.6/kikuchipy/pattern/_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/pattern/chunk.py` & `kikuchipy-0.8.6/kikuchipy/pattern/chunk.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/pattern/tests/__init__.py` & `kikuchipy-0.8.6/kikuchipy/pattern/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/pattern/tests/test_chunk.py` & `kikuchipy-0.8.6/kikuchipy/pattern/tests/test_chunk.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/pattern/tests/test_pattern.py` & `kikuchipy-0.8.6/kikuchipy/pattern/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/projections/__init__.py` & `kikuchipy-0.8.6/kikuchipy/projections/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/projections/gnomonic_projection.py` & `kikuchipy-0.8.6/kikuchipy/projections/gnomonic_projection.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/projections/hesse_normal_form.py` & `kikuchipy-0.8.6/kikuchipy/projections/hesse_normal_form.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/projections/lambert_projection.py` & `kikuchipy-0.8.6/kikuchipy/projections/lambert_projection.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/projections/spherical_projection.py` & `kikuchipy-0.8.6/kikuchipy/projections/spherical_projection.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/projections/tests/__init__.py` & `kikuchipy-0.8.6/kikuchipy/projections/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/projections/tests/test_gnomonic_projection.py` & `kikuchipy-0.8.6/kikuchipy/projections/tests/test_gnomonic_projection.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/projections/tests/test_hesse_normal_form.py` & `kikuchipy-0.8.6/kikuchipy/projections/tests/test_hesse_normal_form.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/projections/tests/test_lambert_projection.py` & `kikuchipy-0.8.6/kikuchipy/projections/tests/test_lambert_projection.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/projections/tests/test_spherical_projection.py` & `kikuchipy-0.8.6/kikuchipy/projections/tests/test_spherical_projection.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/release.py` & `kikuchipy-0.8.6/kikuchipy/release.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 ]
 license = "GPLv3+"
 maintainer = "Håkon Wiik Ånes"
 maintainer_email = "hakon.w.anes@ntnu.no"
 name = "kikuchipy"
 platforms = ["Linux", "MacOS X", "Windows"]
 status = "Development"
-version = "0.8.5"
+version = "0.8.6"
```

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/__init__.py` & `kikuchipy-0.8.6/kikuchipy/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/_kikuchi_master_pattern.py` & `kikuchipy-0.8.6/kikuchipy/signals/_kikuchi_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/_kikuchipy_signal.py` & `kikuchipy-0.8.6/kikuchipy/signals/_kikuchipy_signal.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/ebsd.py` & `kikuchipy-0.8.6/kikuchipy/signals/ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/ebsd_master_pattern.py` & `kikuchipy-0.8.6/kikuchipy/signals/ebsd_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/ecp_master_pattern.py` & `kikuchipy-0.8.6/kikuchipy/signals/ecp_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/tests/__init__.py` & `kikuchipy-0.8.6/kikuchipy/signals/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/tests/test_ebsd.py` & `kikuchipy-0.8.6/kikuchipy/signals/tests/test_ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/tests/test_ebsd_hough_indexing.py` & `kikuchipy-0.8.6/kikuchipy/signals/tests/test_ebsd_hough_indexing.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/tests/test_ebsd_master_pattern.py` & `kikuchipy-0.8.6/kikuchipy/signals/tests/test_ebsd_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/tests/test_ecp_master_pattern.py` & `kikuchipy-0.8.6/kikuchipy/signals/tests/test_ecp_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/tests/test_kikuchi_master_pattern.py` & `kikuchipy-0.8.6/kikuchipy/signals/tests/test_kikuchi_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/tests/test_virtual_bse_image.py` & `kikuchipy-0.8.6/kikuchipy/signals/tests/test_virtual_bse_image.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/util/__init__.py` & `kikuchipy-0.8.6/kikuchipy/signals/util/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/util/_crystal_map.py` & `kikuchipy-0.8.6/kikuchipy/signals/util/_crystal_map.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/util/_dask.py` & `kikuchipy-0.8.6/kikuchipy/signals/util/_dask.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/util/_detector.py` & `kikuchipy-0.8.6/kikuchipy/signals/util/_detector.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/util/_map_helper.py` & `kikuchipy-0.8.6/kikuchipy/signals/util/_map_helper.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/util/_master_pattern.py` & `kikuchipy-0.8.6/kikuchipy/signals/util/_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/util/_overwrite_hyperspy_methods.py` & `kikuchipy-0.8.6/kikuchipy/signals/util/_overwrite_hyperspy_methods.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/util/array_tools.py` & `kikuchipy-0.8.6/kikuchipy/signals/util/array_tools.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/util/tests/__init__.py` & `kikuchipy-0.8.6/kikuchipy/signals/util/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/util/tests/test_array_tools.py` & `kikuchipy-0.8.6/kikuchipy/signals/util/tests/test_array_tools.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/util/tests/test_dask.py` & `kikuchipy-0.8.6/kikuchipy/signals/util/tests/test_dask.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/util/tests/test_overwrite_hyperspy_methods.py` & `kikuchipy-0.8.6/kikuchipy/signals/util/tests/test_overwrite_hyperspy_methods.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/signals/virtual_bse_image.py` & `kikuchipy-0.8.6/kikuchipy/signals/virtual_bse_image.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/simulations/__init__.py` & `kikuchipy-0.8.6/kikuchipy/simulations/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/simulations/_kikuchi_pattern_features.py` & `kikuchipy-0.8.6/kikuchipy/simulations/_kikuchi_pattern_features.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/simulations/_kikuchi_pattern_simulation.py` & `kikuchipy-0.8.6/kikuchipy/simulations/_kikuchi_pattern_simulation.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/simulations/kikuchi_pattern_simulator.py` & `kikuchipy-0.8.6/kikuchipy/simulations/kikuchi_pattern_simulator.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/simulations/tests/__init__.py` & `kikuchipy-0.8.6/kikuchipy/simulations/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/simulations/tests/test_kikuchi_pattern_simulation.py` & `kikuchipy-0.8.6/kikuchipy/simulations/tests/test_kikuchi_pattern_simulation.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy/simulations/tests/test_kikuchi_pattern_simulator.py` & `kikuchipy-0.8.6/kikuchipy/simulations/tests/test_kikuchi_pattern_simulator.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy.egg-info/PKG-INFO` & `kikuchipy-0.8.6/kikuchipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kikuchipy
-Version: 0.8.5
+Version: 0.8.6
 Summary: Processing, simulating and indexing of electron backscatter diffraction (EBSD) patterns.
 Home-page: https://kikuchipy.org
 Download-URL: https://pypi.python.org/pypi/kikuchipy
 Author: kikuchipy developers
 Author-email: hakon.w.anes@ntnu.no
 Maintainer: Håkon Wiik Ånes
 Maintainer-email: hakon.w.anes@ntnu.no
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kikuchipy Version: 0.8.5 Summary: Processing,
+Metadata-Version: 2.1 Name: kikuchipy Version: 0.8.6 Summary: Processing,
 simulating and indexing of electron backscatter diffraction (EBSD) patterns.
 Home-page: https://kikuchipy.org Download-URL: https://pypi.python.org/pypi/
 kikuchipy Author: kikuchipy developers Author-email: hakon.w.anes@ntnu.no
 Maintainer: HÃ¥kon Wiik Ãnes Maintainer-email: hakon.w.anes@ntnu.no License:
 GPLv3+ Project-URL: Bug Tracker, https://github.com/pyxem/kikuchipy/issues
 Project-URL: Documentation, https://kikuchipy.org Project-URL: Source Code,
 https://github.com/pyxem/kikuchipy Keywords: EBSD,electron backscatter
```

### Comparing `kikuchipy-0.8.5/kikuchipy.egg-info/SOURCES.txt` & `kikuchipy-0.8.6/kikuchipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/kikuchipy.egg-info/requires.txt` & `kikuchipy-0.8.6/kikuchipy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/readthedocs.yaml` & `kikuchipy-0.8.6/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/setup.cfg` & `kikuchipy-0.8.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.5/setup.py` & `kikuchipy-0.8.6/setup.py`

 * *Files identical despite different names*

