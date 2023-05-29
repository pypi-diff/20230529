# Comparing `tmp/pyhalo-0.2.3.tar.gz` & `tmp/pyhalo-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhalo-0.2.3.tar", last modified: Sun May 28 05:03:51 2023, max compression
+gzip compressed data, was "pyhalo-0.2.4.tar", last modified: Mon May 29 07:28:09 2023, max compression
```

## Comparing `pyhalo-0.2.3.tar` & `pyhalo-0.2.4.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 05:03:51.678465 pyhalo-0.2.3/
--rw-r--r--   0 danielgilman   (501) staff       (20)      156 2018-08-15 00:45:59.000000 pyhalo-0.2.3/AUTHORS.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     3515 2018-08-15 00:45:59.000000 pyhalo-0.2.3/CONTRIBUTING.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       89 2018-08-15 00:45:59.000000 pyhalo-0.2.3/HISTORY.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     1072 2018-08-15 00:45:59.000000 pyhalo-0.2.3/LICENSE
--rw-r--r--   0 danielgilman   (501) staff       (20)      262 2018-08-15 00:45:59.000000 pyhalo-0.2.3/MANIFEST.in
--rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-05-28 05:03:51.677672 pyhalo-0.2.3/PKG-INFO
--rw-r--r--   0 danielgilman   (501) staff       (20)     2041 2023-05-26 19:45:13.000000 pyhalo-0.2.3/README.rst
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 05:03:51.594957 pyhalo-0.2.3/docs/
--rw-r--r--   0 danielgilman   (501) staff       (20)      607 2018-08-15 00:45:59.000000 pyhalo-0.2.3/docs/Makefile
--rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.3/docs/authors.rst
--rwxr-xr-x   0 danielgilman   (501) staff       (20)     4799 2018-10-06 19:25:46.000000 pyhalo-0.2.3/docs/conf.py
--rw-r--r--   0 danielgilman   (501) staff       (20)       33 2018-08-15 00:45:59.000000 pyhalo-0.2.3/docs/contributing.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.3/docs/history.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)      303 2018-08-15 00:45:59.000000 pyhalo-0.2.3/docs/index.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     1110 2018-08-15 00:45:59.000000 pyhalo-0.2.3/docs/installation.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)      768 2018-08-15 00:45:59.000000 pyhalo-0.2.3/docs/make.bat
--rw-r--r--   0 danielgilman   (501) staff       (20)       27 2018-08-15 00:45:59.000000 pyhalo-0.2.3/docs/readme.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       67 2018-08-15 00:45:59.000000 pyhalo-0.2.3/docs/usage.rst
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 05:03:51.605070 pyhalo-0.2.3/pyHalo/
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 05:03:51.610191 pyhalo-0.2.3/pyHalo/Cosmology/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-08-15 00:50:13.000000 pyhalo-0.2.3/pyHalo/Cosmology/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4768 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Cosmology/cosmology.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     9394 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Cosmology/geometry.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 05:03:51.614239 pyhalo-0.2.3/pyHalo/Halos/
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 05:03:51.619075 pyhalo-0.2.3/pyHalo/Halos/HaloModels/
--rw-r--r--   0 danielgilman   (501) staff       (20)     2920 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Halos/HaloModels/NFW.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1515 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Halos/HaloModels/PTMass.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4967 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Halos/HaloModels/PsuedoJaffe.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3967 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Halos/HaloModels/TNFW.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5544 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Halos/HaloModels/TNFWemulator.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     9969 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Halos/HaloModels/ULDM.py
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-11-11 08:37:06.000000 pyhalo-0.2.3/pyHalo/Halos/HaloModels/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1575 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Halos/HaloModels/gaussian.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4561 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Halos/HaloModels/generalized_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5615 2023-05-18 16:09:33.000000 pyhalo-0.2.3/pyHalo/Halos/HaloModels/powerlaw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-02-20 20:53:15.000000 pyhalo-0.2.3/pyHalo/Halos/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8628 2023-05-26 19:44:32.000000 pyhalo-0.2.3/pyHalo/Halos/concentration.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5423 2023-05-28 04:22:20.000000 pyhalo-0.2.3/pyHalo/Halos/halo_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    16076 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Halos/lens_cosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8469 2023-05-28 04:43:27.000000 pyhalo-0.2.3/pyHalo/Halos/tidal_truncation.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2142 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Halos/util.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 05:03:51.623904 pyhalo-0.2.3/pyHalo/Rendering/
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 05:03:51.628727 pyhalo-0.2.3/pyHalo/Rendering/MassFunctions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.3/pyHalo/Rendering/MassFunctions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1873 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Rendering/MassFunctions/delta_function.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     7019 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Rendering/MassFunctions/density_peaks.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    10149 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Rendering/MassFunctions/mass_function_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      883 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Rendering/MassFunctions/util.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 05:03:51.634075 pyhalo-0.2.3/pyHalo/Rendering/SpatialDistributions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.3/pyHalo/Rendering/SpatialDistributions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      361 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Rendering/SpatialDistributions/base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2440 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Rendering/SpatialDistributions/correlated.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3156 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Rendering/SpatialDistributions/nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4384 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Rendering/SpatialDistributions/uniform.py
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.3/pyHalo/Rendering/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8837 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Rendering/correlated_structure.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5268 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Rendering/halo_population.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4621 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Rendering/line_of_sight.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3205 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Rendering/rendering_class_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5972 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Rendering/subhalos.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3487 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/Rendering/two_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      149 2018-08-15 00:45:59.000000 pyhalo-0.2.3/pyHalo/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2570 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/concentration_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3846 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/defaults.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2447 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/mass_function_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    46841 2023-05-26 19:51:20.000000 pyhalo-0.2.3/pyHalo/preset_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5617 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/pyhalo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    26366 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/realization_extensions.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    36187 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/single_realization.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1176 2023-05-18 15:44:57.000000 pyhalo-0.2.3/pyHalo/truncation_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    14271 2023-05-28 04:22:20.000000 pyhalo-0.2.3/pyHalo/utilities.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 05:03:51.608980 pyhalo-0.2.3/pyHalo.egg-info/
--rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-05-28 05:03:51.000000 pyhalo-0.2.3/pyHalo.egg-info/PKG-INFO
--rw-r--r--   0 danielgilman   (501) staff       (20)     3893 2023-05-28 05:03:51.000000 pyhalo-0.2.3/pyHalo.egg-info/SOURCES.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)        1 2023-05-28 05:03:51.000000 pyhalo-0.2.3/pyHalo.egg-info/dependency_links.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)       43 2023-05-28 05:03:51.000000 pyhalo-0.2.3/pyHalo.egg-info/entry_points.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)        1 2018-08-23 21:07:23.000000 pyhalo-0.2.3/pyHalo.egg-info/not-zip-safe
--rw-r--r--   0 danielgilman   (501) staff       (20)       11 2023-05-28 05:03:51.000000 pyhalo-0.2.3/pyHalo.egg-info/requires.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)       13 2023-05-28 05:03:51.000000 pyhalo-0.2.3/pyHalo.egg-info/top_level.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)      526 2023-05-28 05:03:42.000000 pyhalo-0.2.3/pyproject.toml
--rw-r--r--   0 danielgilman   (501) staff       (20)       38 2023-05-28 05:03:51.678786 pyhalo-0.2.3/setup.cfg
--rw-r--r--   0 danielgilman   (501) staff       (20)     1639 2023-05-24 16:05:34.000000 pyhalo-0.2.3/setup.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 05:03:51.649429 pyhalo-0.2.3/tests/
--rw-r--r--   0 danielgilman   (501) staff       (20)       61 2018-10-06 19:25:46.000000 pyhalo-0.2.3/tests/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1688 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_concentration_models.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 05:03:51.654507 pyhalo-0.2.3/tests/test_cosmology/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-10-18 06:20:01.000000 pyhalo-0.2.3/tests/test_cosmology/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5023 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_cosmology/test_cone_geometry.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3841 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_cosmology/test_cosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3969 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_cosmology/test_cylinder_geometry.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 05:03:51.667124 pyhalo-0.2.3/tests/test_halos/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-12-04 22:13:12.000000 pyhalo-0.2.3/tests/test_halos/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2832 2023-05-28 04:43:27.000000 pyhalo-0.2.3/tests/test_halos/test_adiabatic_tides.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4220 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_halos/test_concentrations.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1334 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_halos/test_gaussian.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     6011 2023-05-18 16:13:37.000000 pyhalo-0.2.3/tests/test_halos/test_general_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3407 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_halos/test_lenscosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2682 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_halos/test_nfw_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3343 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_halos/test_pjaffe.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1665 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_halos/test_point_mass.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4304 2023-05-18 16:13:19.000000 pyhalo-0.2.3/tests/test_halos/test_powerlaw_profile.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2719 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_halos/test_tnfw_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2401 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_halos/test_truncation.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5002 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_halos/test_uldm.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1068 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_halos/test_util.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      874 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_mass_function_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3224 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_preset_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8793 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_pyhalo_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    16257 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_realization_extensions.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 05:03:51.670723 pyhalo-0.2.3/tests/test_rendering/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.3/tests/test_rendering/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2584 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_rendering/test_2halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3422 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_rendering/test_los.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 05:03:51.673689 pyhalo-0.2.3/tests/test_rendering/test_mass_functions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_rendering/test_mass_functions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5915 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_rendering/test_mass_functions/test_base_functions.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2173 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_rendering/test_mass_functions/test_delta_function.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    11175 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_rendering/test_mass_functions/test_sheth_tormen.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2936 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_rendering/test_population.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 05:03:51.676485 pyhalo-0.2.3/tests/test_rendering/test_spatial_distribution/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_rendering/test_spatial_distribution/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2096 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_rendering/test_spatial_distribution/test_correlated.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2191 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_rendering/test_spatial_distribution/test_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2153 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_rendering/test_spatial_distribution/test_uniform.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3491 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_rendering/test_subhalos.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    23809 2023-05-18 15:44:57.000000 pyhalo-0.2.3/tests/test_single_realization.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3437 2023-05-28 05:02:49.000000 pyhalo-0.2.3/tests/test_utilities.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:09.034663 pyhalo-0.2.4/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      156 2018-08-15 00:45:59.000000 pyhalo-0.2.4/AUTHORS.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3515 2018-08-15 00:45:59.000000 pyhalo-0.2.4/CONTRIBUTING.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       89 2018-08-15 00:45:59.000000 pyhalo-0.2.4/HISTORY.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1072 2018-08-15 00:45:59.000000 pyhalo-0.2.4/LICENSE
+-rw-r--r--   0 danielgilman   (501) staff       (20)      262 2018-08-15 00:45:59.000000 pyhalo-0.2.4/MANIFEST.in
+-rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-05-29 07:28:09.033773 pyhalo-0.2.4/PKG-INFO
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2034 2023-05-29 07:26:56.000000 pyhalo-0.2.4/README.rst
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:08.874652 pyhalo-0.2.4/docs/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      607 2018-08-15 00:45:59.000000 pyhalo-0.2.4/docs/Makefile
+-rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.4/docs/authors.rst
+-rwxr-xr-x   0 danielgilman   (501) staff       (20)     4799 2018-10-06 19:25:46.000000 pyhalo-0.2.4/docs/conf.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)       33 2018-08-15 00:45:59.000000 pyhalo-0.2.4/docs/contributing.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.4/docs/history.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)      303 2018-08-15 00:45:59.000000 pyhalo-0.2.4/docs/index.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1110 2018-08-15 00:45:59.000000 pyhalo-0.2.4/docs/installation.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)      768 2018-08-15 00:45:59.000000 pyhalo-0.2.4/docs/make.bat
+-rw-r--r--   0 danielgilman   (501) staff       (20)       27 2018-08-15 00:45:59.000000 pyhalo-0.2.4/docs/readme.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       67 2018-08-15 00:45:59.000000 pyhalo-0.2.4/docs/usage.rst
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:08.894116 pyhalo-0.2.4/pyHalo/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:08.907939 pyhalo-0.2.4/pyHalo/Cosmology/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-08-15 00:50:13.000000 pyhalo-0.2.4/pyHalo/Cosmology/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4768 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Cosmology/cosmology.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     9394 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Cosmology/geometry.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:08.923470 pyhalo-0.2.4/pyHalo/Halos/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:08.946585 pyhalo-0.2.4/pyHalo/Halos/HaloModels/
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2920 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Halos/HaloModels/NFW.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1515 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Halos/HaloModels/PTMass.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4967 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Halos/HaloModels/PsuedoJaffe.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3967 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Halos/HaloModels/TNFW.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5544 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Halos/HaloModels/TNFWemulator.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     9969 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Halos/HaloModels/ULDM.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-11-11 08:37:06.000000 pyhalo-0.2.4/pyHalo/Halos/HaloModels/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1575 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Halos/HaloModels/gaussian.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4561 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Halos/HaloModels/generalized_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5615 2023-05-18 16:09:33.000000 pyhalo-0.2.4/pyHalo/Halos/HaloModels/powerlaw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-02-20 20:53:15.000000 pyhalo-0.2.4/pyHalo/Halos/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8462 2023-05-29 07:26:42.000000 pyhalo-0.2.4/pyHalo/Halos/concentration.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5423 2023-05-28 04:22:20.000000 pyhalo-0.2.4/pyHalo/Halos/halo_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    16076 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Halos/lens_cosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     9940 2023-05-29 07:26:42.000000 pyhalo-0.2.4/pyHalo/Halos/tidal_truncation.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2142 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Halos/util.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:08.958773 pyhalo-0.2.4/pyHalo/Rendering/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:08.967941 pyhalo-0.2.4/pyHalo/Rendering/MassFunctions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.4/pyHalo/Rendering/MassFunctions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1873 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Rendering/MassFunctions/delta_function.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     7019 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Rendering/MassFunctions/density_peaks.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    10149 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Rendering/MassFunctions/mass_function_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      883 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Rendering/MassFunctions/util.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:08.976021 pyhalo-0.2.4/pyHalo/Rendering/SpatialDistributions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.4/pyHalo/Rendering/SpatialDistributions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      361 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Rendering/SpatialDistributions/base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2440 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Rendering/SpatialDistributions/correlated.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4339 2023-05-29 07:26:42.000000 pyhalo-0.2.4/pyHalo/Rendering/SpatialDistributions/nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4696 2023-05-29 07:26:42.000000 pyhalo-0.2.4/pyHalo/Rendering/SpatialDistributions/uniform.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.4/pyHalo/Rendering/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8837 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Rendering/correlated_structure.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5268 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Rendering/halo_population.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4605 2023-05-29 07:26:42.000000 pyhalo-0.2.4/pyHalo/Rendering/line_of_sight.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3205 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Rendering/rendering_class_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5991 2023-05-29 07:26:42.000000 pyhalo-0.2.4/pyHalo/Rendering/subhalos.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3487 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/Rendering/two_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      149 2018-08-15 00:45:59.000000 pyhalo-0.2.4/pyHalo/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2570 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/concentration_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3846 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/defaults.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2447 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/mass_function_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    46841 2023-05-29 07:14:39.000000 pyhalo-0.2.4/pyHalo/preset_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5617 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/pyhalo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    26366 2023-05-18 15:44:57.000000 pyhalo-0.2.4/pyHalo/realization_extensions.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    36339 2023-05-29 07:26:42.000000 pyhalo-0.2.4/pyHalo/single_realization.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1302 2023-05-29 07:26:42.000000 pyhalo-0.2.4/pyHalo/truncation_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    14271 2023-05-28 04:22:20.000000 pyhalo-0.2.4/pyHalo/utilities.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:08.902976 pyhalo-0.2.4/pyHalo.egg-info/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-05-29 07:28:08.000000 pyhalo-0.2.4/pyHalo.egg-info/PKG-INFO
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3893 2023-05-29 07:28:08.000000 pyhalo-0.2.4/pyHalo.egg-info/SOURCES.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)        1 2023-05-29 07:28:08.000000 pyhalo-0.2.4/pyHalo.egg-info/dependency_links.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)       43 2023-05-29 07:28:08.000000 pyhalo-0.2.4/pyHalo.egg-info/entry_points.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)        1 2018-08-23 21:07:23.000000 pyhalo-0.2.4/pyHalo.egg-info/not-zip-safe
+-rw-r--r--   0 danielgilman   (501) staff       (20)       11 2023-05-29 07:28:08.000000 pyhalo-0.2.4/pyHalo.egg-info/requires.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)       13 2023-05-29 07:28:08.000000 pyhalo-0.2.4/pyHalo.egg-info/top_level.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)      526 2023-05-29 07:27:28.000000 pyhalo-0.2.4/pyproject.toml
+-rw-r--r--   0 danielgilman   (501) staff       (20)       38 2023-05-29 07:28:09.034908 pyhalo-0.2.4/setup.cfg
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1639 2023-05-24 16:05:34.000000 pyhalo-0.2.4/setup.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:08.996563 pyhalo-0.2.4/tests/
+-rw-r--r--   0 danielgilman   (501) staff       (20)       61 2018-10-06 19:25:46.000000 pyhalo-0.2.4/tests/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1688 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_concentration_models.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:09.000406 pyhalo-0.2.4/tests/test_cosmology/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-10-18 06:20:01.000000 pyhalo-0.2.4/tests/test_cosmology/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5023 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_cosmology/test_cone_geometry.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3841 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_cosmology/test_cosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3969 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_cosmology/test_cylinder_geometry.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:09.014871 pyhalo-0.2.4/tests/test_halos/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-12-04 22:13:12.000000 pyhalo-0.2.4/tests/test_halos/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2832 2023-05-28 04:43:27.000000 pyhalo-0.2.4/tests/test_halos/test_adiabatic_tides.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4220 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_halos/test_concentrations.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1334 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_halos/test_gaussian.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     6011 2023-05-18 16:13:37.000000 pyhalo-0.2.4/tests/test_halos/test_general_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3407 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_halos/test_lenscosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2682 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_halos/test_nfw_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3343 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_halos/test_pjaffe.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1665 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_halos/test_point_mass.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4304 2023-05-18 16:13:19.000000 pyhalo-0.2.4/tests/test_halos/test_powerlaw_profile.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2719 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_halos/test_tnfw_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3517 2023-05-29 07:26:42.000000 pyhalo-0.2.4/tests/test_halos/test_truncation.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5002 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_halos/test_uldm.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1068 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_halos/test_util.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      874 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_mass_function_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3224 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_preset_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8793 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_pyhalo_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    16257 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_realization_extensions.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:09.022096 pyhalo-0.2.4/tests/test_rendering/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.4/tests/test_rendering/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2584 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_rendering/test_2halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3422 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_rendering/test_los.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:09.026253 pyhalo-0.2.4/tests/test_rendering/test_mass_functions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_rendering/test_mass_functions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5915 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_rendering/test_mass_functions/test_base_functions.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2173 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_rendering/test_mass_functions/test_delta_function.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    11175 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_rendering/test_mass_functions/test_sheth_tormen.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2936 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_rendering/test_population.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-29 07:28:09.032304 pyhalo-0.2.4/tests/test_rendering/test_spatial_distribution/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_rendering/test_spatial_distribution/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2096 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_rendering/test_spatial_distribution/test_correlated.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2484 2023-05-29 07:26:42.000000 pyhalo-0.2.4/tests/test_rendering/test_spatial_distribution/test_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2153 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_rendering/test_spatial_distribution/test_uniform.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3491 2023-05-29 07:23:17.000000 pyhalo-0.2.4/tests/test_rendering/test_subhalos.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    23809 2023-05-18 15:44:57.000000 pyhalo-0.2.4/tests/test_single_realization.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3429 2023-05-29 07:26:42.000000 pyhalo-0.2.4/tests/test_utilities.py
```

### Comparing `pyhalo-0.2.3/CONTRIBUTING.rst` & `pyhalo-0.2.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/LICENSE` & `pyhalo-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/PKG-INFO` & `pyhalo-0.2.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhalo
-Version: 0.2.3
+Version: 0.2.4
 Summary: A python package for generating populations of dark matter halos
 Home-page: https://github.com/dangilman/pyHalo
 Author: Daniel Gilman
 Author-email: Daniel Gilman <daniel.gilman@utoronto.ca>
 License: MIT license
 Project-URL: Homepage, https://github.com/dangilman/pyHalo
 Project-URL: Bug Tracker, https://github.com/dangilman/pyHalo/issues
```

### Comparing `pyhalo-0.2.3/README.rst` & `pyhalo-0.2.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 pyHalo renders full mass distributions for substructure lensing simulations with the open source gravitational lensing software package lenstronomy (https://github.com/sibirrer/lenstronomy). The example notebooks illustrate the core functionality of this package. 
 
 If you would like to use this package and have questions, please get in touch with me at daniel.gilman@utoronto.ca - I am happy to help! 
 
 Installation
 ------------
-"python3 -m pip install pyhalo==0.2.1"
+"python3 -m pip install pyhalo"
 
 Or clone the repository, navigate into the directory that contains the setup.py file and run "python setup.py install"
 
 The first code release, before majoring refactoring, is 8302393. 
 
 In order to use this package when not installing via pip, you'll need to install colossus http://www.benediktdiemer.com/code/colossus/
```

### Comparing `pyhalo-0.2.3/docs/Makefile` & `pyhalo-0.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/docs/conf.py` & `pyhalo-0.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/docs/installation.rst` & `pyhalo-0.2.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/docs/make.bat` & `pyhalo-0.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Cosmology/cosmology.py` & `pyhalo-0.2.4/pyHalo/Cosmology/cosmology.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Cosmology/geometry.py` & `pyhalo-0.2.4/pyHalo/Cosmology/geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Halos/HaloModels/NFW.py` & `pyhalo-0.2.4/pyHalo/Halos/HaloModels/NFW.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Halos/HaloModels/PTMass.py` & `pyhalo-0.2.4/pyHalo/Halos/HaloModels/PTMass.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Halos/HaloModels/PsuedoJaffe.py` & `pyhalo-0.2.4/pyHalo/Halos/HaloModels/PsuedoJaffe.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Halos/HaloModels/TNFW.py` & `pyhalo-0.2.4/pyHalo/Halos/HaloModels/TNFW.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Halos/HaloModels/TNFWemulator.py` & `pyhalo-0.2.4/pyHalo/Halos/HaloModels/TNFWemulator.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Halos/HaloModels/ULDM.py` & `pyhalo-0.2.4/pyHalo/Halos/HaloModels/ULDM.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Halos/HaloModels/gaussian.py` & `pyhalo-0.2.4/pyHalo/Halos/HaloModels/gaussian.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Halos/HaloModels/generalized_nfw.py` & `pyhalo-0.2.4/pyHalo/Halos/HaloModels/generalized_nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Halos/HaloModels/powerlaw.py` & `pyhalo-0.2.4/pyHalo/Halos/HaloModels/powerlaw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Halos/concentration.py` & `pyhalo-0.2.4/pyHalo/Halos/concentration.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,14 @@
         self._scatter_dex = scatter_dex
 
     def nfw_concentration(self, m, z):
         """
         Evaluates the concentration of a halo of mass 'm' at redshift z
         :param M: halo mass [M_sun]
         :param z: halo redshift
-        :param scatter: bool; add log-normal scatter to concentration
-        :param scatter_amplitude: the amount of scatter in dex, assumes log-normal distribution
         :return:
         """
         c = self._evaluate_concentration(m, z)
         if self._scatter:
             log_c = numpy.log(c)
             c = numpy.random.lognormal(log_c, self._scatter_dex)
         return c
```

### Comparing `pyhalo-0.2.3/pyHalo/Halos/halo_base.py` & `pyhalo-0.2.4/pyHalo/Halos/halo_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Halos/lens_cosmo.py` & `pyhalo-0.2.4/pyHalo/Halos/lens_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Halos/tidal_truncation.py` & `pyhalo-0.2.4/pyHalo/Halos/tidal_truncation.py`

 * *Files 10% similar despite different names*

```diff
@@ -195,7 +195,48 @@
         """
         (log10c, log10mass_loss_fraction) = point
         log10c = max(self._min_c, log10c)
         log10c = min(self._max_c, log10c)
         log10mass_loss_fraction = max(-1.5, log10mass_loss_fraction)
         log10mass_loss_fraction = min(-0.01, log10mass_loss_fraction)
         return (log10c, log10mass_loss_fraction)
+
+class TruncateMeanDensity(object):
+
+    def __init__(self, lens_cosmo, median_rt_over_rs=1.0, c_power=3.0):
+        """
+
+        :param lens_cosmo:
+        :param median_rt_over_rs:
+        :param c_power:
+        """
+        self._norm = median_rt_over_rs
+        self._cpower = c_power
+        self.lens_cosmo = lens_cosmo
+        self._concentration_cdm = ConcentrationDiemerJoyce(lens_cosmo.cosmo,
+                                                           scatter=False)
+
+    def truncation_radius_halo(self, halo):
+
+        """
+        Thiis method computess the truncation radius using the class attributes of an instance of Halo
+        :param halo: an instance of halo
+        :return: the truncation radius in physical kpc
+        """
+        c_median = self._concentration_cdm.nfw_concentration(halo.mass, halo.z_eval)
+        c_actual = halo.c
+        halo_rpericenter = halo.rperi_units_r200
+        return self.truncation_radius(halo.mass, halo.z, c_median, c_actual, halo_rpericenter)
+
+    def truncation_radius(self, halo_mass, halo_redshift, c_median, c_actual, r_peri):
+        """
+
+        :param halo_mass:
+        :param halo_redshift:
+        :param c_median:
+        :param c_actual:
+        :param r_peri:
+        :return:
+        """
+        rt_over_rs = self._norm * (c_actual / c_median) ** self._cpower * (r_peri / 0.5)
+        _, rs, _ = self.lens_cosmo.NFW_params_physical(halo_mass, c_actual, halo_redshift)
+        return rs * rt_over_rs
```

### Comparing `pyhalo-0.2.3/pyHalo/Halos/util.py` & `pyhalo-0.2.4/pyHalo/Halos/util.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Rendering/MassFunctions/delta_function.py` & `pyhalo-0.2.4/pyHalo/Rendering/MassFunctions/delta_function.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Rendering/MassFunctions/density_peaks.py` & `pyhalo-0.2.4/pyHalo/Rendering/MassFunctions/density_peaks.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Rendering/MassFunctions/mass_function_base.py` & `pyhalo-0.2.4/pyHalo/Rendering/MassFunctions/mass_function_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Rendering/MassFunctions/util.py` & `pyhalo-0.2.4/pyHalo/Rendering/MassFunctions/util.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Rendering/SpatialDistributions/correlated.py` & `pyhalo-0.2.4/pyHalo/Rendering/SpatialDistributions/correlated.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Rendering/SpatialDistributions/uniform.py` & `pyhalo-0.2.4/pyHalo/Rendering/SpatialDistributions/uniform.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,24 @@
 
         :param geometry: an instance of Geometry (Cosmology.geometry)
         """
         self._cosmo_geometry = geometry
         self._uni = Uniform(0.5 * cone_opening_angle, geometry)
         super(LensConeUniform, self).__init__()
 
+    @classmethod
+    def from_Mhost(cls, *args, **kwargs):
+        """
+
+        :param rmax2d_arcsec:
+        :param geometry:
+        :return:
+        """
+        raise Exception('Spatial distribution class LensConeUniform not currently implemented for subhalos')
+
     def draw(self, N, z_plane, center_x=0, center_y=0):
 
         """
         Generates samples in two dimensions out to a maximum radius r = 0.5 * cone_opening_angle * f(z)
         where f(z) = geometry.rendering_scale(z)
         :param N: number of objects to generate
         :param z_plane: the redshift where the objects are being placed (used to compute the conversion to physical kpc)
@@ -66,22 +76,22 @@
         :param geometry: an instance of Geometry (Cosmology.geometry)
         """
         self.rmax2d_arcsec = rmax2d_arcsec
         self._geo = geometry
         super(Uniform, self).__init__()
 
     @classmethod
-    def from_Mhost(cls, rmax2d_arcsec, geometry):
+    def from_Mhost(cls, *args, **kwargs):
         """
 
         :param rmax2d_arcsec:
         :param geometry:
         :return:
         """
-        return Uniform(rmax2d_arcsec, geometry)
+        raise Exception('Spatial distribution class Uniform not currently implemented for subhalos')
 
     def draw(self, N, z_plane, rescale=1.0, center_x=0, center_y=0):
 
         """
         Generate samples distributed uniformly in two dimensions
         :param N: number of objects to generate
         :param z_plane: the redshift where the objects are being placed (used to compute the conversion to physical kpc)
@@ -100,11 +110,12 @@
         r = np.random.uniform(0, rmax ** 2, int(N))
 
         x_arcsec = r ** .5 * np.cos(angle)
         y_arcsec = r ** .5 * np.sin(angle)
 
         x_arcsec += center_x
         y_arcsec += center_y
+
         kpc_per_asec = self._geo.kpc_per_arcsec(z_plane)
         x_kpc, y_kpc = x_arcsec * kpc_per_asec, y_arcsec * kpc_per_asec
 
         return np.array(x_kpc), np.array(y_kpc)
```

### Comparing `pyhalo-0.2.3/pyHalo/Rendering/correlated_structure.py` & `pyhalo-0.2.4/pyHalo/Rendering/correlated_structure.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Rendering/halo_population.py` & `pyhalo-0.2.4/pyHalo/Rendering/halo_population.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Rendering/line_of_sight.py` & `pyhalo-0.2.4/pyHalo/Rendering/line_of_sight.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,16 +70,16 @@
         """
         this routine applies the negative convergence sheet correction for lens planes along the line of sight
         :param kwargs_mass_sheets: keyword arguments that overwrite whatever the default settings for the mass sheet
         sheet are - leave it as None for most applications
         :return:
         """
 
-        lens_plane_redshifts = self._lens_plane_redshifts[0::2]
-        delta_zs = 2 * self._delta_z_list[0::2]
+        lens_plane_redshifts = self._lens_plane_redshifts
+        delta_zs = self._delta_z_list
         kwargs_out = []
         profile_names_out = []
         redshifts = []
 
         if zmin is None:
             zmin = 0.0
         if zmax is None:
```

### Comparing `pyhalo-0.2.3/pyHalo/Rendering/rendering_class_base.py` & `pyhalo-0.2.4/pyHalo/Rendering/rendering_class_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/Rendering/subhalos.py` & `pyhalo-0.2.4/pyHalo/Rendering/subhalos.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         """
         :param nhalos: number of halos or objects to generate
         :return: the x, y coordinate of objects in arcsec, and a 3 dimensional coordinate in kpc
         The 3d coordinate only has a clear physical interpretation for subhalos, and is used to compute truncation raddi.
         For line of sight halos it is set to None.
         """
 
-        x_kpc, y_kpc, r3d_kpc = self._spatial_distribution_model.draw(nhalos, None)
+        x_kpc, y_kpc, r3d_kpc = self._spatial_distribution_model.draw(nhalos, self._lens_cosmo.z_lens)
         if len(x_kpc) > 0:
             kpc_per_asec = self._geometry.kpc_per_arcsec(self._lens_cosmo.z_lens)
             x_arcsec = x_kpc * kpc_per_asec ** -1
             y_arcsec = y_kpc * kpc_per_asec ** -1
             return x_arcsec, y_arcsec, r3d_kpc
         else:
             return np.array([]), np.array([]), np.array([])
```

### Comparing `pyhalo-0.2.3/pyHalo/Rendering/two_halo.py` & `pyhalo-0.2.4/pyHalo/Rendering/two_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/concentration_models.py` & `pyhalo-0.2.4/pyHalo/concentration_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/defaults.py` & `pyhalo-0.2.4/pyHalo/defaults.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/mass_function_models.py` & `pyhalo-0.2.4/pyHalo/mass_function_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/preset_models.py` & `pyhalo-0.2.4/pyHalo/preset_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/pyhalo.py` & `pyhalo-0.2.4/pyHalo/pyhalo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/realization_extensions.py` & `pyhalo-0.2.4/pyHalo/realization_extensions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo/single_realization.py` & `pyhalo-0.2.4/pyHalo/single_realization.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,19 +40,20 @@
                 indexes.append(_indexes[i])
     else:
         halos = _halos
         indexes = _indexes
 
     centerx, centery = realization.rendering_center
     kwargs_halo_model = realization.kwargs_halo_model
+    geometry = realization.geometry
     return Realization.from_halos(halos, realization.lens_cosmo,
                                   kwargs_halo_model,
                                   mass_sheet_correction,
                                   realization.rendering_classes,
-                                  centerx, centery), indexes
+                                  centerx, centery, geometry), indexes
 
 class Realization(object):
 
     """
     This is the main class for storing a population of dark matter halos, both in the main lens plane and along the
     line of sight. This class is created by the main pyhalo module.
     """
@@ -550,19 +551,21 @@
         """
 
         kwargs_mass_sheets_out = []
         redshifts_out = []
         profiles_out = []
 
         if subtract_exact_sheets:
-
+            redshifts_out = []
             for zi in self.unique_redshifts:
+                redshifts_out.append(zi)
                 area = self.geometry.angle_to_physical_area(0.5 * self.geometry.cone_opening_angle, zi)
-                kwargs_mass_sheets_out += [{'kappa_ext': -self.mass_at_z_exact(zi) / self.lens_cosmo.sigma_crit_mass(zi, area)}]
-            redshifts_out = self.unique_redshifts
+                kappa_ext = -self.mass_at_z_exact(zi) / self.lens_cosmo.sigma_crit_mass(zi, area)
+                kwargs_sheet = {'kappa_ext': kappa_ext}
+                kwargs_mass_sheets_out.append(kwargs_sheet)
             profiles_out = ['CONVERGENCE'] * len(kwargs_mass_sheets_out)
 
         else:
 
             for rendering_class in rendering_classes:
 
                 if rendering_class is None:
```

### Comparing `pyhalo-0.2.3/pyHalo/truncation_models.py` & `pyhalo-0.2.4/pyHalo/truncation_models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from pyHalo.Halos.tidal_truncation import TruncationRN, TruncationRoche, AdiabaticTidesTruncation, TruncationSplashBack
+from pyHalo.Halos.tidal_truncation import TruncationRN, TruncationRoche, \
+    AdiabaticTidesTruncation, TruncationSplashBack, TruncateMeanDensity
 
 
 def truncation_models(model_name):
     """
     Loads and returns methods to set the tidal truncation radius (or equivalent parameter) of halos
     """
     kwargs_model = {}
@@ -19,10 +20,12 @@
         kwargs_model['m_power'] = 1./3
         kwargs_model['RocheNu'] = 2./3
         return TruncationRoche, kwargs_model
     elif model_name == 'ADIABATIC_TIDES':
         return AdiabaticTidesTruncation, kwargs_model
     elif model_name == 'SPLASHBACK':
         return TruncationSplashBack, kwargs_model
+    elif model_name == 'TRUNCATION_MEAN_DENSITY':
+        return TruncateMeanDensity, kwargs_model
     else:
         raise Exception('model '+str(model_name)+' not recognized')
```

### Comparing `pyhalo-0.2.3/pyHalo/utilities.py` & `pyhalo-0.2.4/pyHalo/utilities.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyHalo.egg-info/PKG-INFO` & `pyhalo-0.2.4/pyHalo.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhalo
-Version: 0.2.3
+Version: 0.2.4
 Summary: A python package for generating populations of dark matter halos
 Home-page: https://github.com/dangilman/pyHalo
 Author: Daniel Gilman
 Author-email: Daniel Gilman <daniel.gilman@utoronto.ca>
 License: MIT license
 Project-URL: Homepage, https://github.com/dangilman/pyHalo
 Project-URL: Bug Tracker, https://github.com/dangilman/pyHalo/issues
```

### Comparing `pyhalo-0.2.3/pyHalo.egg-info/SOURCES.txt` & `pyhalo-0.2.4/pyHalo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/pyproject.toml` & `pyhalo-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyhalo"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="Daniel Gilman", email="daniel.gilman@utoronto.ca" },
 ]
 description = "A python package for generating populations of dark matter halos"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pyhalo-0.2.3/setup.py` & `pyhalo-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_concentration_models.py` & `pyhalo-0.2.4/tests/test_concentration_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_cosmology/test_cone_geometry.py` & `pyhalo-0.2.4/tests/test_cosmology/test_cone_geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_cosmology/test_cosmo.py` & `pyhalo-0.2.4/tests/test_cosmology/test_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_cosmology/test_cylinder_geometry.py` & `pyhalo-0.2.4/tests/test_cosmology/test_cylinder_geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_halos/test_adiabatic_tides.py` & `pyhalo-0.2.4/tests/test_halos/test_adiabatic_tides.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_halos/test_concentrations.py` & `pyhalo-0.2.4/tests/test_halos/test_concentrations.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_halos/test_gaussian.py` & `pyhalo-0.2.4/tests/test_halos/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_halos/test_general_nfw.py` & `pyhalo-0.2.4/tests/test_halos/test_general_nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_halos/test_lenscosmo.py` & `pyhalo-0.2.4/tests/test_halos/test_lenscosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_halos/test_nfw_halo.py` & `pyhalo-0.2.4/tests/test_halos/test_nfw_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_halos/test_pjaffe.py` & `pyhalo-0.2.4/tests/test_halos/test_pjaffe.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_halos/test_point_mass.py` & `pyhalo-0.2.4/tests/test_halos/test_point_mass.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_halos/test_powerlaw_profile.py` & `pyhalo-0.2.4/tests/test_halos/test_powerlaw_profile.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_halos/test_tnfw_halo.py` & `pyhalo-0.2.4/tests/test_halos/test_tnfw_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_halos/test_truncation.py` & `pyhalo-0.2.4/tests/test_halos/test_truncation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import pytest
 from pyHalo.Halos.lens_cosmo import LensCosmo
 from pyHalo.Cosmology.cosmology import Cosmology
 import numpy.testing as npt
-from pyHalo.Halos.tidal_truncation import TruncationRN, TruncationRoche, TruncationSplashBack
+from pyHalo.Halos.tidal_truncation import TruncationRN, TruncationRoche, TruncationSplashBack, TruncateMeanDensity
 from pyHalo.truncation_models import truncation_models
 from astropy.cosmology import FlatLambdaCDM
+from pyHalo.Halos.concentration import ConcentrationDiemerJoyce
 import os
 
 
 class TestTruncation(object):
 
     def setup_method(self):
 
         astropy = FlatLambdaCDM(70.0, 0.3)
         cosmo = Cosmology(astropy)
         self.lenscosmo = LensCosmo(0.5, 1.5, cosmo)
 
     def test_load_models(self):
 
         model_name_list = ['TRUNCATION_R50', 'TRUNCATION_RN', 'TRUNCATION_ROCHE', 'TRUNCATION_ROCHE_GILMAN2020',
-                           'SPLASHBACK']
+                           'SPLASHBACK', 'TRUNCATION_MEAN_DENSITY']
         kwargs_model_list = [{}, {'LOS_truncation_factor': 50.}, {'RocheNorm': 1.0, 'm_power': 1./3, 'RocheNu': 2.0/3.0}, {},
-                             {}]
+                             {}, {}]
         for model,kwargs in zip(model_name_list, kwargs_model_list):
             mod, kw = truncation_models(model)
             kwargs.update(kw)
             kwargs['lens_cosmo'] = self.lenscosmo
             _ = mod(**kwargs)
 
     def test_truncation_RN(self):
@@ -57,10 +58,34 @@
                 self.z = z
         truncation_splashback = TruncationSplashBack(self.lenscosmo)
         rt = truncation_splashback.truncation_radius(10**8, 0.4)
         halo = DummyHalo(10**8, 0.4)
         rt_halo = truncation_splashback.truncation_radius_halo(halo)
         npt.assert_almost_equal(rt, rt_halo)
 
+    def test_truncation_mean_density(self):
+
+        class DummyHalo(object):
+            def __init__(self, m, z):
+                self.mass = m
+                self.z = z
+                self.z_eval = z
+                self.rperi_units_r200 = 0.7
+                self.c = 16.0
+
+        halo = DummyHalo(10 ** 8, 0.4)
+        median_rt_over_rs = 2.0
+        c_power = 4.0
+        cmodel = ConcentrationDiemerJoyce(self.lenscosmo.cosmo, scatter=False)
+        c_theory = cmodel.nfw_concentration(10 ** 8, 0.4)
+        truncation = TruncateMeanDensity(self.lenscosmo, median_rt_over_rs, c_power)
+        r_t = truncation.truncation_radius(10**8, 0.4, c_theory, 16.0, 0.7)
+        r_t_halo = truncation.truncation_radius_halo(halo)
+        npt.assert_almost_equal(r_t, r_t_halo)
+
+        rt_over_rs_theory = median_rt_over_rs * (16.0 / c_theory) ** c_power * (0.7 / 0.5)
+        rs = self.lenscosmo.NFW_params_physical(10**8, 16.0, 0.4)[1]
+        npt.assert_almost_equal(rs * rt_over_rs_theory, r_t)
+
 
 if __name__ == '__main__':
     pytest.main()
```

### Comparing `pyhalo-0.2.3/tests/test_halos/test_uldm.py` & `pyhalo-0.2.4/tests/test_halos/test_uldm.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_halos/test_util.py` & `pyhalo-0.2.4/tests/test_halos/test_util.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_mass_function_models.py` & `pyhalo-0.2.4/tests/test_mass_function_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_preset_models.py` & `pyhalo-0.2.4/tests/test_preset_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_pyhalo_base.py` & `pyhalo-0.2.4/tests/test_pyhalo_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_realization_extensions.py` & `pyhalo-0.2.4/tests/test_realization_extensions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_rendering/test_2halo.py` & `pyhalo-0.2.4/tests/test_rendering/test_2halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_rendering/test_los.py` & `pyhalo-0.2.4/tests/test_rendering/test_los.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_rendering/test_mass_functions/test_base_functions.py` & `pyhalo-0.2.4/tests/test_rendering/test_mass_functions/test_base_functions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_rendering/test_mass_functions/test_delta_function.py` & `pyhalo-0.2.4/tests/test_rendering/test_mass_functions/test_delta_function.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_rendering/test_mass_functions/test_sheth_tormen.py` & `pyhalo-0.2.4/tests/test_rendering/test_mass_functions/test_sheth_tormen.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_rendering/test_population.py` & `pyhalo-0.2.4/tests/test_rendering/test_population.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_rendering/test_spatial_distribution/test_correlated.py` & `pyhalo-0.2.4/tests/test_rendering/test_spatial_distribution/test_correlated.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_rendering/test_spatial_distribution/test_nfw.py` & `pyhalo-0.2.4/tests/test_rendering/test_spatial_distribution/test_nfw.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,67 @@
 import numpy as np
 import numpy.testing as npt
 import pytest
 from pyHalo.Rendering.SpatialDistributions.nfw import ProjectedNFW, CNFW
+from lenstronomy.Util.analysis_util import azimuthalAverage
 import matplotlib.pyplot as plt
 
 
 class TestProjectedNFW(object):
 
     def setup_method(self):
 
-        rmax2d_arcsec = 20.0
+        rmax2d_arcsec = 10.0
         rs_kpc = 60
         r200_kpc = 550
 
         self.arcsec_to_kpc = 6.2
         self.rs_arcsec = rs_kpc / self.arcsec_to_kpc
         self.rmax2d_arcsec = rmax2d_arcsec
         self.r200_arcsec = r200_kpc / self.arcsec_to_kpc
-        self.rcore_arcsec = 0.2 * self.rs_arcsec
+        self.rcore_arcsec = 0.5 * self.rs_arcsec
         self.nfw = ProjectedNFW(self.rmax2d_arcsec, self.rs_arcsec, self.rcore_arcsec,
                                 self.r200_arcsec, self.arcsec_to_kpc)
 
     def test_limit(self):
 
         x, y, r3 = self.nfw.draw(50000)
         r2_kpc = np.hypot(x, y)
         rmax_kpc = self.rmax2d_arcsec * self.arcsec_to_kpc
         npt.assert_almost_equal(max(r2_kpc)/rmax_kpc, 1, 2)
         rmax_3d_kpc = self.r200_arcsec * self.arcsec_to_kpc
         npt.assert_almost_equal(max(r3)/rmax_3d_kpc,1,1)
 
     def test_profile(self):
 
-        rbins = np.linspace(0.001*self.rmax2d_arcsec, self.rmax2d_arcsec, 200)
+        rbins = np.linspace(0.005*self.rmax2d_arcsec, self.rmax2d_arcsec, 100)
 
-        x_kpc, y_kpc, r3d_kpc = self.nfw.draw(500000)
+        x_kpc, y_kpc, r3d_kpc = self.nfw.draw(3000000)
         x_arcsec, y_arcsec = x_kpc / self.arcsec_to_kpc, y_kpc / self.arcsec_to_kpc
         r_arcsec = np.hypot(x_arcsec, y_arcsec)
         number_density = []
         for i in range(0, len(rbins)-1):
             cond1 = r_arcsec >= rbins[i]
             cond2 = r_arcsec < rbins[i+1]
             cond = np.logical_and(cond1, cond2)
-            number_density.append(np.sum(cond)/1.0)
+            area = rbins[i+1]**2 - rbins[i] ** 2
+            number_density.append(np.sum(cond)/area)
         number_density = np.array(number_density)
-        plt.loglog(rbins[0:-1], number_density)
+
+        #plt.loglog(rbins[0:-1], number_density, color='k')
 
         cnfw_profile = CNFW()
         number_density_true = cnfw_profile.density_2d(rbins, 0.0, self.rs_arcsec, 1.0, self.rcore_arcsec)
-        rescale = number_density[0]/number_density_true[0]
+        rescale = np.mean(number_density[0:10])/number_density_true[0]
         number_density_true *= rescale
         ratio = []
         for i in range(0, len(rbins[0:-1])):
             ratio.append(number_density_true[i]/number_density[i])
         ratio = np.array(ratio)
         npt.assert_array_less(abs(1-np.sum(ratio)/len(ratio)), 0.05)
+        # plt.loglog(rbins, number_density_true, color='b')
+        # plt.gca().axvline(self.rcore_arcsec)
+        # plt.xlim(0.01, 20)
+        # plt.show()
 
 if __name__ == '__main__':
      pytest.main()
```

### Comparing `pyhalo-0.2.3/tests/test_rendering/test_spatial_distribution/test_uniform.py` & `pyhalo-0.2.4/tests/test_rendering/test_spatial_distribution/test_uniform.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_rendering/test_subhalos.py` & `pyhalo-0.2.4/tests/test_rendering/test_subhalos.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_single_realization.py` & `pyhalo-0.2.4/tests/test_single_realization.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.3/tests/test_utilities.py` & `pyhalo-0.2.4/tests/test_utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         mu = 2.0
         sigma = 1.5
         func = lambda x: np.exp(-0.5 * (x - mu) ** 2 / sigma**2)
         x = np.linspace(mu - 5*sigma, mu + 5*sigma, 1000)
         x_samples = inverse_transform_sampling(x, func, (), 100000)
         npt.assert_almost_equal(np.mean(x_samples)/mu, 1.0, 2)
         npt.assert_almost_equal(np.std(x_samples)/sigma, 1.0, 2)
-        
+
     def test_ITSampling(self):
 
         mu = 2.14
         sigma = 0.35
         x = np.random.normal(mu, sigma, 250000)
         sampler = ITSampling.from_samples(x)
         x_samples = sampler(100000)
```

