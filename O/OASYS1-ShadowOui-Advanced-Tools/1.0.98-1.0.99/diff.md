# Comparing `tmp/OASYS1-ShadowOui-Advanced-Tools-1.0.98.tar.gz` & `tmp/OASYS1-ShadowOui-Advanced-Tools-1.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/OASYS1-ShadowOui-Advanced-Tools-1.0.98.tar", last modified: Sat Feb 26 15:57:00 2022, max compression
+gzip compressed data, was "dist/OASYS1-ShadowOui-Advanced-Tools-1.0.99.tar", last modified: Sat Feb 26 16:18:52 2022, max compression
```

## Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98.tar` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/
--rw-rw-rw-   0 bishop    (1601)      907    29803 2020-06-09 15:58:27.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/LICENSE.pdf
--rwxrwxrwx   0 bishop    (1601)      907      292 2020-08-18 21:57:44.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/MANIFEST.in
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/OASYS1_ShadowOui_Advanced_Tools.egg-info/
--rw-r--r--   0 bishop    (1601)      907     4198 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/OASYS1_ShadowOui_Advanced_Tools.egg-info/PKG-INFO
--rw-r--r--   0 bishop    (1601)      907     3935 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/OASYS1_ShadowOui_Advanced_Tools.egg-info/SOURCES.txt
--rw-r--r--   0 bishop    (1601)      907        1 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/OASYS1_ShadowOui_Advanced_Tools.egg-info/dependency_links.txt
--rw-r--r--   0 bishop    (1601)      907      429 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/OASYS1_ShadowOui_Advanced_Tools.egg-info/entry_points.txt
--rw-r--r--   0 bishop    (1601)      907       94 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/OASYS1_ShadowOui_Advanced_Tools.egg-info/namespace_packages.txt
--rw-r--r--   0 bishop    (1601)      907        1 2020-06-10 19:46:55.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/OASYS1_ShadowOui_Advanced_Tools.egg-info/not-zip-safe
--rw-r--r--   0 bishop    (1601)      907       84 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/OASYS1_ShadowOui_Advanced_Tools.egg-info/requires.txt
--rw-r--r--   0 bishop    (1601)      907       14 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/OASYS1_ShadowOui_Advanced_Tools.egg-info/top_level.txt
--rw-r--r--   0 bishop    (1601)      907     4198 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/PKG-INFO
--rw-rw-rw-   0 bishop    (1601)      907     3165 2020-06-09 15:51:59.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/README.md
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/
--rw-rw-rw-   0 bishop    (1601)      907     3448 2021-02-23 22:43:19.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/
--rw-rw-rw-   0 bishop    (1601)      907     3447 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/menu/
--rw-rw-rw-   0 bishop    (1601)      907     3453 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/menu/__init__.py
--rwxrwxrwx   0 bishop    (1601)      907     7347 2021-07-14 23:09:46.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/menu/ow_shadow_advanced_tools_menu.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/util/
--rw-rw-rw-   0 bishop    (1601)      907     3391 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/util/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/util/fresnel_zone_plates/
--rw-rw-rw-   0 bishop    (1601)      907     3345 2020-09-11 15:28:15.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/util/fresnel_zone_plates/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907    33933 2022-02-03 15:17:05.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/util/fresnel_zone_plates/fresnel_zone_plate_simulator.py
--rw-rw-rw-   0 bishop    (1601)      907     6557 2020-09-14 22:43:17.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/util/fresnel_zone_plates/hankel_transform.py
--rw-rw-rw-   0 bishop    (1601)      907   225474 2020-10-07 17:54:40.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/util/fresnel_zone_plates/refractive_index.py
--rw-rw-rw-   0 bishop    (1601)      907    28380 2021-07-12 20:17:39.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/util/gui.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/
--rw-rw-rw-   0 bishop    (1601)      907     3447 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/optical_elements/
--rw-rw-rw-   0 bishop    (1601)      907      157 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/optical_elements/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/optical_elements/bl/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2021-09-29 23:43:32.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/optical_elements/bl/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907    14607 2021-09-30 22:21:54.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/optical_elements/bl/bendable_ellipsoid_mirror_bl.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/optical_elements/icons/
--rw-rw-rw-   0 bishop    (1601)      907    40399 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/optical_elements/icons/bendable_ellipsoid_mirror.png
--rw-rw-rw-   0 bishop    (1601)      907    51797 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/optical_elements/icons/oe.png
--rw-rw-rw-   0 bishop    (1601)      907    81869 2020-08-13 22:38:44.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/optical_elements/icons/zone_plate.png
--rwxrwxrwx   0 bishop    (1601)      907    16556 2022-02-03 15:17:05.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/optical_elements/ow_bendable_ellipsoid_mirror.py
--rw-rw-rw-   0 bishop    (1601)      907    44567 2022-02-08 01:10:41.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/optical_elements/ow_fresnel_zone_plate.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/sources/
--rw-rw-rw-   0 bishop    (1601)      907      173 2020-06-15 20:50:49.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/sources/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/sources/attributes/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2021-10-01 20:12:24.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/sources/attributes/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907     8259 2021-10-01 20:16:33.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/sources/attributes/hybrid_undulator_attributes.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/sources/bl/
--rw-rw-rw-   0 bishop    (1601)      907        0 2021-09-09 16:14:58.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/sources/bl/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907    50813 2022-02-08 01:10:41.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/sources/bl/hybrid_undulator_bl.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/sources/icons/
--rw-rw-rw-   0 bishop    (1601)      907    28443 2020-06-15 20:59:26.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/sources/icons/source.png
--rw-rw-rw-   0 bishop    (1601)      907    51237 2020-06-11 19:05:36.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/sources/icons/undulator.png
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/sources/misc/
--rw-rw-rw-   0 bishop    (1601)      907    13486 2020-07-23 22:14:39.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/sources/misc/symmetry.png
--rw-rw-rw-   0 bishop    (1601)      907    57691 2022-02-06 21:50:50.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/sources/ow_hybrid_undulator.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/
--rw-rw-rw-   0 bishop    (1601)      907      161 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/
--rw-rw-rw-   0 bishop    (1601)      907    69777 2021-01-29 18:05:21.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/bm_plot_xy_power.png
--rwxrwxrwx   0 bishop    (1601)      907   302350 2020-06-11 23:23:25.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/cycle_power.png
--rw-rw-rw-   0 bishop    (1601)      907    83396 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/flux.png
--rw-rw-rw-   0 bishop    (1601)      907    20332 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/footprint_reader.png
--rw-rw-rw-   0 bishop    (1601)      907    81273 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/plot_xy_power.png
--rw-rw-rw-   0 bishop    (1601)      907     4642 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/thermal.png
--rw-rw-rw-   0 bishop    (1601)      907     5413 2020-06-14 03:57:11.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/total_filter.png
--rw-rw-rw-   0 bishop    (1601)      907    24109 2020-06-14 03:51:53.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/total_reflectivity.png
-drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/misc/
--rw-rw-rw-   0 bishop    (1601)      907   107751 2021-07-09 17:31:33.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/misc/fit_formulas.png
--rw-rw-rw-   0 bishop    (1601)      907    73917 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/misc/flux_calculator.png
--rw-r--r--   0 bishop    (1601)      907    11840 2022-02-26 15:20:34.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/misc/gauss_formula.png
--rw-r--r--   0 bishop    (1601)      907    30670 2022-02-26 15:21:07.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/misc/pv_formula.png
--rw-rw-rw-   0 bishop    (1601)      907    11895 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_flux_calculator.py
--rwxrwxrwx   0 bishop    (1601)      907    12409 2021-11-30 03:47:40.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_footprint_file_reader.py
--rwxrwxrwx   0 bishop    (1601)      907    49512 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_power_node_point.py
--rwxrwxrwx   0 bishop    (1601)      907   104606 2022-02-26 15:53:39.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_power_plot_xy.py
--rwxrwxrwx   0 bishop    (1601)      907    42092 2021-02-02 03:22:48.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_power_plot_xy_BM.py
--rw-rw-rw-   0 bishop    (1601)      907    16637 2020-09-01 22:43:02.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_total_reflectivity.py
--rw-r--r--   0 bishop    (1601)      907       38 2022-02-26 15:57:00.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/setup.cfg
--rw-rw-rw-   0 bishop    (1601)      907     6778 2022-02-26 15:56:34.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.98/setup.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/
+-rw-rw-rw-   0 bishop    (1601)      907    29803 2020-06-09 15:58:27.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/LICENSE.pdf
+-rwxrwxrwx   0 bishop    (1601)      907      292 2020-08-18 21:57:44.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/MANIFEST.in
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/OASYS1_ShadowOui_Advanced_Tools.egg-info/
+-rw-r--r--   0 bishop    (1601)      907     4198 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/OASYS1_ShadowOui_Advanced_Tools.egg-info/PKG-INFO
+-rw-r--r--   0 bishop    (1601)      907     4009 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/OASYS1_ShadowOui_Advanced_Tools.egg-info/SOURCES.txt
+-rw-r--r--   0 bishop    (1601)      907        1 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/OASYS1_ShadowOui_Advanced_Tools.egg-info/dependency_links.txt
+-rw-r--r--   0 bishop    (1601)      907      429 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/OASYS1_ShadowOui_Advanced_Tools.egg-info/entry_points.txt
+-rw-r--r--   0 bishop    (1601)      907       94 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/OASYS1_ShadowOui_Advanced_Tools.egg-info/namespace_packages.txt
+-rw-r--r--   0 bishop    (1601)      907        1 2020-06-10 19:46:55.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/OASYS1_ShadowOui_Advanced_Tools.egg-info/not-zip-safe
+-rw-r--r--   0 bishop    (1601)      907       84 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/OASYS1_ShadowOui_Advanced_Tools.egg-info/requires.txt
+-rw-r--r--   0 bishop    (1601)      907       14 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/OASYS1_ShadowOui_Advanced_Tools.egg-info/top_level.txt
+-rw-r--r--   0 bishop    (1601)      907     4198 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/PKG-INFO
+-rw-rw-rw-   0 bishop    (1601)      907     3165 2020-06-09 15:51:59.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/README.md
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/
+-rw-rw-rw-   0 bishop    (1601)      907     3448 2021-02-23 22:43:19.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/
+-rw-rw-rw-   0 bishop    (1601)      907     3447 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/menu/
+-rw-rw-rw-   0 bishop    (1601)      907     3453 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/menu/__init__.py
+-rwxrwxrwx   0 bishop    (1601)      907     7347 2021-07-14 23:09:46.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/menu/ow_shadow_advanced_tools_menu.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/util/
+-rw-rw-rw-   0 bishop    (1601)      907     3391 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/util/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/util/fresnel_zone_plates/
+-rw-rw-rw-   0 bishop    (1601)      907     3345 2020-09-11 15:28:15.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/util/fresnel_zone_plates/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907    33933 2022-02-03 15:17:05.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/util/fresnel_zone_plates/fresnel_zone_plate_simulator.py
+-rw-rw-rw-   0 bishop    (1601)      907     6557 2020-09-14 22:43:17.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/util/fresnel_zone_plates/hankel_transform.py
+-rw-rw-rw-   0 bishop    (1601)      907   225474 2020-10-07 17:54:40.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/util/fresnel_zone_plates/refractive_index.py
+-rw-rw-rw-   0 bishop    (1601)      907    28380 2021-07-12 20:17:39.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/util/gui.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/
+-rw-rw-rw-   0 bishop    (1601)      907     3447 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/optical_elements/
+-rw-rw-rw-   0 bishop    (1601)      907      157 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/optical_elements/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/optical_elements/bl/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2021-09-29 23:43:32.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/optical_elements/bl/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907    14607 2021-09-30 22:21:54.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/optical_elements/bl/bendable_ellipsoid_mirror_bl.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/optical_elements/icons/
+-rw-rw-rw-   0 bishop    (1601)      907    40399 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/optical_elements/icons/bendable_ellipsoid_mirror.png
+-rw-rw-rw-   0 bishop    (1601)      907    51797 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/optical_elements/icons/oe.png
+-rw-rw-rw-   0 bishop    (1601)      907    81869 2020-08-13 22:38:44.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/optical_elements/icons/zone_plate.png
+-rwxrwxrwx   0 bishop    (1601)      907    16556 2022-02-03 15:17:05.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/optical_elements/ow_bendable_ellipsoid_mirror.py
+-rw-rw-rw-   0 bishop    (1601)      907    44567 2022-02-08 01:10:41.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/optical_elements/ow_fresnel_zone_plate.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/sources/
+-rw-rw-rw-   0 bishop    (1601)      907      173 2020-06-15 20:50:49.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/sources/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/sources/attributes/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2021-10-01 20:12:24.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/sources/attributes/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907     8259 2021-10-01 20:16:33.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/sources/attributes/hybrid_undulator_attributes.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/sources/bl/
+-rw-rw-rw-   0 bishop    (1601)      907        0 2021-09-09 16:14:58.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/sources/bl/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907    50813 2022-02-08 01:10:41.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/sources/bl/hybrid_undulator_bl.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/sources/icons/
+-rw-rw-rw-   0 bishop    (1601)      907    28443 2020-06-15 20:59:26.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/sources/icons/source.png
+-rw-rw-rw-   0 bishop    (1601)      907    51237 2020-06-11 19:05:36.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/sources/icons/undulator.png
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/sources/misc/
+-rw-rw-rw-   0 bishop    (1601)      907    13486 2020-07-23 22:14:39.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/sources/misc/symmetry.png
+-rw-rw-rw-   0 bishop    (1601)      907    57691 2022-02-06 21:50:50.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/sources/ow_hybrid_undulator.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/
+-rw-rw-rw-   0 bishop    (1601)      907      161 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/
+-rw-rw-rw-   0 bishop    (1601)      907    69777 2021-01-29 18:05:21.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/bm_plot_xy_power.png
+-rwxrwxrwx   0 bishop    (1601)      907   302350 2020-06-11 23:23:25.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/cycle_power.png
+-rw-rw-rw-   0 bishop    (1601)      907    83396 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/flux.png
+-rw-rw-rw-   0 bishop    (1601)      907    20332 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/footprint_reader.png
+-rw-rw-rw-   0 bishop    (1601)      907    81273 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/plot_xy_power.png
+-rw-rw-rw-   0 bishop    (1601)      907     4642 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/thermal.png
+-rw-rw-rw-   0 bishop    (1601)      907     5413 2020-06-14 03:57:11.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/total_filter.png
+-rw-rw-rw-   0 bishop    (1601)      907    24109 2020-06-14 03:51:53.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/total_reflectivity.png
+drwxr-xr-x   0 bishop    (1601)      907        0 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/misc/
+-rw-rw-rw-   0 bishop    (1601)      907   107751 2021-07-09 17:31:33.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/misc/fit_formulas.png
+-rw-rw-rw-   0 bishop    (1601)      907    73917 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/misc/flux_calculator.png
+-rw-r--r--   0 bishop    (1601)      907    11840 2022-02-26 15:20:34.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/misc/gauss_formula.png
+-rw-r--r--   0 bishop    (1601)      907     7583 2022-02-26 16:11:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/misc/poly_formula.png
+-rw-r--r--   0 bishop    (1601)      907    30670 2022-02-26 15:21:07.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/misc/pv_formula.png
+-rw-rw-rw-   0 bishop    (1601)      907    11895 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_flux_calculator.py
+-rwxrwxrwx   0 bishop    (1601)      907    12409 2021-11-30 03:47:40.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_footprint_file_reader.py
+-rwxrwxrwx   0 bishop    (1601)      907    49512 2021-02-22 18:06:12.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_power_node_point.py
+-rwxrwxrwx   0 bishop    (1601)      907   105029 2022-02-26 16:16:57.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_power_plot_xy.py
+-rwxrwxrwx   0 bishop    (1601)      907    42092 2021-02-02 03:22:48.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_power_plot_xy_BM.py
+-rw-rw-rw-   0 bishop    (1601)      907    16637 2020-09-01 22:43:02.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_total_reflectivity.py
+-rw-r--r--   0 bishop    (1601)      907       38 2022-02-26 16:18:52.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/setup.cfg
+-rw-rw-rw-   0 bishop    (1601)      907     6778 2022-02-26 16:07:50.000000 OASYS1-ShadowOui-Advanced-Tools-1.0.99/setup.py
```

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/LICENSE.pdf` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/LICENSE.pdf`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/OASYS1_ShadowOui_Advanced_Tools.egg-info/PKG-INFO` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/OASYS1_ShadowOui_Advanced_Tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: OASYS1-ShadowOui-Advanced-Tools
-Version: 1.0.98
+Version: 1.0.99
 Summary: ShadowOui advanced simulation tools
 Home-page: https://github.com/oasys-kit/ShadowOui-Advanced-Tools
 Author: Luca Rebuffi
 Author-email: lrebuffi@anl.gov
 License: GPLv3
 Download-URL: https://github.com/oasys-kit/ShadowOui-Advanced-Tools
 Description: # ShadowOui-Advanced-Tools
```

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/OASYS1_ShadowOui_Advanced_Tools.egg-info/SOURCES.txt` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/OASYS1_ShadowOui_Advanced_Tools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -52,8 +52,9 @@
 orangecontrib/shadow_advanced_tools/widgets/thermal/icons/plot_xy_power.png
 orangecontrib/shadow_advanced_tools/widgets/thermal/icons/thermal.png
 orangecontrib/shadow_advanced_tools/widgets/thermal/icons/total_filter.png
 orangecontrib/shadow_advanced_tools/widgets/thermal/icons/total_reflectivity.png
 orangecontrib/shadow_advanced_tools/widgets/thermal/misc/fit_formulas.png
 orangecontrib/shadow_advanced_tools/widgets/thermal/misc/flux_calculator.png
 orangecontrib/shadow_advanced_tools/widgets/thermal/misc/gauss_formula.png
+orangecontrib/shadow_advanced_tools/widgets/thermal/misc/poly_formula.png
 orangecontrib/shadow_advanced_tools/widgets/thermal/misc/pv_formula.png
```

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/PKG-INFO` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: OASYS1-ShadowOui-Advanced-Tools
-Version: 1.0.98
+Version: 1.0.99
 Summary: ShadowOui advanced simulation tools
 Home-page: https://github.com/oasys-kit/ShadowOui-Advanced-Tools
 Author: Luca Rebuffi
 Author-email: lrebuffi@anl.gov
 License: GPLv3
 Download-URL: https://github.com/oasys-kit/ShadowOui-Advanced-Tools
 Description: # ShadowOui-Advanced-Tools
```

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/README.md` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/README.md`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/__init__.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/__init__.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/__init__.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/menu/__init__.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/menu/__init__.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/menu/ow_shadow_advanced_tools_menu.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/menu/ow_shadow_advanced_tools_menu.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/util/__init__.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/util/fresnel_zone_plates/__init__.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/util/fresnel_zone_plates/__init__.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/util/fresnel_zone_plates/fresnel_zone_plate_simulator.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/util/fresnel_zone_plates/fresnel_zone_plate_simulator.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/util/fresnel_zone_plates/hankel_transform.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/util/fresnel_zone_plates/hankel_transform.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/util/fresnel_zone_plates/refractive_index.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/util/fresnel_zone_plates/refractive_index.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/util/gui.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/util/gui.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/__init__.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/optical_elements/bl/__init__.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/optical_elements/bl/__init__.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/optical_elements/bl/bendable_ellipsoid_mirror_bl.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/optical_elements/bl/bendable_ellipsoid_mirror_bl.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/optical_elements/icons/bendable_ellipsoid_mirror.png` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/optical_elements/icons/bendable_ellipsoid_mirror.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/optical_elements/icons/oe.png` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/optical_elements/icons/oe.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/optical_elements/icons/zone_plate.png` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/optical_elements/icons/zone_plate.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/optical_elements/ow_bendable_ellipsoid_mirror.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/optical_elements/ow_bendable_ellipsoid_mirror.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/optical_elements/ow_fresnel_zone_plate.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/optical_elements/ow_fresnel_zone_plate.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/sources/attributes/__init__.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/sources/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/sources/attributes/hybrid_undulator_attributes.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/sources/attributes/hybrid_undulator_attributes.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/sources/bl/hybrid_undulator_bl.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/sources/bl/hybrid_undulator_bl.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/sources/icons/source.png` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/sources/icons/source.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/sources/icons/undulator.png` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/sources/icons/undulator.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/sources/misc/symmetry.png` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/sources/misc/symmetry.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/sources/ow_hybrid_undulator.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/sources/ow_hybrid_undulator.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/bm_plot_xy_power.png` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/bm_plot_xy_power.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/cycle_power.png` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/cycle_power.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/flux.png` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/flux.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/footprint_reader.png` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/footprint_reader.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/plot_xy_power.png` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/plot_xy_power.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/thermal.png` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/thermal.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/total_filter.png` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/total_filter.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/total_reflectivity.png` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/icons/total_reflectivity.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/misc/fit_formulas.png` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/misc/fit_formulas.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/misc/flux_calculator.png` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/misc/flux_calculator.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/misc/gauss_formula.png` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/misc/gauss_formula.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/misc/pv_formula.png` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/misc/pv_formula.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_flux_calculator.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_flux_calculator.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_footprint_file_reader.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_footprint_file_reader.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_power_node_point.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_power_node_point.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_power_plot_xy.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_power_plot_xy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1633,15 +1633,15 @@
                         r'$A=%.4f$' %   (self.gauss_A,),
                         r'$x_0=%.4f$' % (self.gauss_x0,),
                         r'$y_0=%.4f$' % (self.gauss_y0,),
                         r'$f_x=%.6f$' % (self.gauss_fx,),
                         r'$f_y=%.6f$' % (self.gauss_fy,),
                     ))
 
-                    if show: self.plot_fit(h_coord, v_coord, histogram, pd_fit_g, "Gaussian", self.gauss_chisquare, params_string,
+                    if show: self.plot_fit(h_coord, v_coord, histogram, pd_fit_g, "Gaussian", "gauss", self.gauss_chisquare, params_string,
                                            formula_img_file=gauss_formula_path, zoom=0.5, xybox=(85, -20))
 
                 elif self.fit_algorithm == 1:
                     if self.pv_c_fixed == 1: bounds = bounds_pv(c=[-1e-12, 1e-12])
                     else:                    bounds = None
 
                     pd_fit_pv, params_pv = get_fitted_data_pv(h_coord, v_coord, histogram, bounds=bounds)
@@ -1663,47 +1663,50 @@
                         r'$y_0=%.4f$' % (self.pv_y0,),
                         r'$f_x=%.6f$' % (self.pv_fx,),
                         r'$f_y=%.6f$' % (self.pv_fy,),
                         r'$m_x=%.4f$' % (self.pv_mx,),
                         r'$m_y=%.4f$' % (self.pv_my,),
                     ))
 
-                    if show: self.plot_fit(h_coord, v_coord, histogram, pd_fit_pv, "Pseudo-Voigt", self.pv_chisquare, params_string,
+                    if show: self.plot_fit(h_coord, v_coord, histogram, pd_fit_pv, "Pseudo-Voigt", "p-v", self.pv_chisquare, params_string,
                                            formula_img_file=pv_formula_path, zoom=0.42, xybox=(215, -15))
 
                 elif self.fit_algorithm == 2:
                     congruence.checkStrictlyPositiveNumber(self.poly_degree, "Degree")
 
                     pd_fit_poly, params_poly = get_fitted_data_poly(h_coord, v_coord, histogram, self.poly_degree)
 
                     params_poly = numpy.reshape(params_poly, (self.poly_degree + 1, self.poly_degree + 1))
                     params_string     = []
                     params_string_mpl = []
                     for i in range(params_poly.shape[0]):
                         for j in range(params_poly.shape[1]):
                             param = params_poly[i, j]
-                            params_string.append(r'c%d,%d=%.4f$' %   (i, j, param,))
-                            params_string_mpl.append(r'$c_{%d,%d}=%.4f$' %   (i, j, param,))
+                            params_string.append(r'c%d,%d=%.4f' % (i, j, param,))
+                            params_string_mpl.append(r'c_{%d,%d}=%.4f' % (i, j, param,))
 
-                    params_string = '\n'.join(params_string)
+                    params_string     = '\n'.join(params_string)
                     params_string_mpl = '\n'.join(params_string_mpl)
 
                     self.poly_coefficients_text.setText(params_string)
                     self.poly_chisquare = round(chisquare(histogram, pd_fit_poly, len(params_poly)), 4)
 
-                    if show: self.plot_fit(h_coord, v_coord, histogram, pd_fit_poly, "Polynomial", self.poly_chisquare, params_string_mpl, fontsize=10)
+                    if show: self.plot_fit(h_coord, v_coord, histogram, pd_fit_poly, "Polynomial", "poly", self.poly_chisquare, params_string_mpl, fontsize=10,
+                                           formula_img_file=poly_formula_path, zoom=0.5, xybox=(25, -20))
 
             except Exception as e:
                 QMessageBox.critical(self, "Error", str(e), QMessageBox.Ok)
 
                 if self.IS_DEVELOP: raise e
 
-    def plot_fit(self, xx, yy, pd, pd_fit, algorithm, chisquare, params, fontsize=14, formula_img_file=None, zoom=0.5, xybox=(85, -20)):
+    def plot_fit(self, xx, yy, pd, pd_fit, algorithm, suffix, chisquare, params, fontsize=14,
+                 formula_img_file=None, zoom=0.5, xybox=(85, -20)):
         dialog = ShowFitResultDialog(xx, yy, pd, pd_fit, algorithm, chisquare, params,
                                      file_name=None if self.autosave==0 else self.autosave_file_name,
+                                     suffix=suffix,
                                      fontsize=fontsize,
                                      formula_img_file=formula_img_file,
                                      zoom=zoom,
                                      xybox=xybox,
                                      parent=self)
         dialog.show()
 
@@ -1984,25 +1987,26 @@
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
 from matplotlib.figure import Figure
 
 from matplotlib import gridspec
 
 gauss_formula_path = os.path.join(resources.package_dirname("orangecontrib.shadow_advanced_tools.widgets.thermal"), "misc", "gauss_formula.png")
 pv_formula_path = os.path.join(resources.package_dirname("orangecontrib.shadow_advanced_tools.widgets.thermal"), "misc", "pv_formula.png")
-
+poly_formula_path = os.path.join(resources.package_dirname("orangecontrib.shadow_advanced_tools.widgets.thermal"), "misc", "poly_formula.png")
 
 class ShowFitResultDialog(QDialog):
 
-    def __init__(self, xx, yy, pd, pd_fit, algorithm, chisquare, params_string, file_name=None,
+    def __init__(self, xx, yy, pd, pd_fit, algorithm, chisquare, params_string, file_name=None, suffix=None,
                  fontsize=14, formula_img_file=None, zoom=0.5, xybox=(85, -20), parent=None):
         QDialog.__init__(self, parent)
         self.setWindowTitle('Fit Result')
         layout = QVBoxLayout(self)
 
-        self.file_name = None if file_name is None else congruence.checkDir(os.path.splitext(file_name)[0] + "_fit.png")
+        self.file_name = None if file_name is None else \
+            congruence.checkDir(os.path.splitext(file_name)[0] + "_fit" + ("" if suffix is None else ("_" + suffix)) + ".png")
 
         figure = Figure(figsize=(4, 8))
         figure.patch.set_facecolor('white')
 
         gs = gridspec.GridSpec(1, 2, width_ratios=[1, 3])
         ax = [None, None]
         ax[0] = figure.add_subplot(gs[0])
```

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_power_plot_xy_BM.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_power_plot_xy_BM.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_total_reflectivity.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/orangecontrib/shadow_advanced_tools/widgets/thermal/ow_total_reflectivity.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ShadowOui-Advanced-Tools-1.0.98/setup.py` & `OASYS1-ShadowOui-Advanced-Tools-1.0.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 try:
     from setuptools import find_packages, setup
 except AttributeError:
     from setuptools import find_packages, setup
 
 NAME = 'OASYS1-ShadowOui-Advanced-Tools'
-VERSION = '1.0.98'
+VERSION = '1.0.99'
 ISRELEASED = True
 
 DESCRIPTION = 'ShadowOui advanced simulation tools'
 README_FILE = os.path.join(os.path.dirname(__file__), 'README.md')
 LONG_DESCRIPTION = open(README_FILE).read()
 AUTHOR = 'Luca Rebuffi'
 AUTHOR_EMAIL = 'lrebuffi@anl.gov'
```

