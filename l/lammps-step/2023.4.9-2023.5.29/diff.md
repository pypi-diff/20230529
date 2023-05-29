# Comparing `tmp/lammps_step-2023.4.9.tar.gz` & `tmp/lammps_step-2023.5.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lammps_step-2023.4.9.tar", last modified: Thu Mar  9 15:50:18 2023, max compression
+gzip compressed data, was "lammps_step-2023.5.29.tar", last modified: Mon May 29 19:08:16 2023, max compression
```

## Comparing `lammps_step-2023.4.9.tar` & `lammps_step-2023.5.29.tar`

### file list

```diff
@@ -1,106 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.394036 lammps_step-2023.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-03-09 15:50:18.394036 lammps_step-2023.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.378035 lammps_step-2023.4.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.378035 lammps_step-2023.4.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.378035 lammps_step-2023.4.9/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9562 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.378035 lammps_step-2023.4.9/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.386036 lammps_step-2023.4.9/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)  2437613 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/getting_started/density.png
--rw-r--r--   0 runner    (1001) docker     (123)   175972 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/getting_started/edit_forcefield.png
--rw-r--r--   0 runner    (1001) docker     (123)   312162 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/getting_started/edit_initialization.png
--rw-r--r--   0 runner    (1001) docker     (123)   877297 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/getting_started/edit_npt.png
--rw-r--r--   0 runner    (1001) docker     (123)   575423 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/getting_started/edit_packmol.png
--rw-r--r--   0 runner    (1001) docker     (123)   408930 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/getting_started/flowchart.png
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)   220257 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/getting_started/lammps_flowchart.png
--rw-r--r--   0 runner    (1001) docker     (123)   148973 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/getting_started/nist.png
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.386036 lammps_step-2023.4.9/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.394036 lammps_step-2023.4.9/lammps_step/
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      492 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-09 15:50:18.394036 lammps_step-2023.4.9/lammps_step/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/custom_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/custom_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.394036 lammps_step-2023.4.9/lammps_step/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/data/configuration.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/data/properties.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/data/seamm-lammps.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/energy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/energy_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    21595 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/initialization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/initialization_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    23619 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)    81558 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/lammps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/lammps_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/lammps_units.py
--rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/minimization.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/minimization_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    22034 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/npt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/npt_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/npt_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/nve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/nve_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/nve_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    13457 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/nvt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/nvt_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/nvt_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/tk_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/tk_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/tk_initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/tk_lammps.py
--rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/tk_minimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    30803 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/tk_npt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/tk_nve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/tk_nvt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/tk_velocities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/velocities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/velocities_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/velocities_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.394036 lammps_step-2023.4.9/lammps_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-03-09 15:50:18.000000 lammps_step-2023.4.9/lammps_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-03-09 15:50:18.000000 lammps_step-2023.4.9/lammps_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 15:50:18.000000 lammps_step-2023.4.9/lammps_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-09 15:50:18.000000 lammps_step-2023.4.9/lammps_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-09 15:50:18.000000 lammps_step-2023.4.9/lammps_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-09 15:50:18.000000 lammps_step-2023.4.9/lammps_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 15:50:05.000000 lammps_step-2023.4.9/lammps_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-09 15:50:18.394036 lammps_step-2023.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.394036 lammps_step-2023.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.394036 lammps_step-2023.4.9/tests/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14459 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/tests/data/Ar_xtal_energy.flow
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/tests/test_lammps_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/tests/test_lammps_units.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.969673 lammps_step-2023.5.29/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-05-29 19:08:16.969673 lammps_step-2023.5.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.941673 lammps_step-2023.5.29/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.945673 lammps_step-2023.5.29/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.945673 lammps_step-2023.5.29/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9562 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.945673 lammps_step-2023.5.29/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.953673 lammps_step-2023.5.29/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)  2437613 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/getting_started/density.png
+-rw-r--r--   0 runner    (1001) docker     (123)   175972 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/getting_started/edit_forcefield.png
+-rw-r--r--   0 runner    (1001) docker     (123)   312162 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/getting_started/edit_initialization.png
+-rw-r--r--   0 runner    (1001) docker     (123)   877297 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/getting_started/edit_npt.png
+-rw-r--r--   0 runner    (1001) docker     (123)   575423 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/getting_started/edit_packmol.png
+-rw-r--r--   0 runner    (1001) docker     (123)   408930 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/getting_started/flowchart.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   220257 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/getting_started/lammps_flowchart.png
+-rw-r--r--   0 runner    (1001) docker     (123)   148973 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/getting_started/nist.png
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.953673 lammps_step-2023.5.29/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.969673 lammps_step-2023.5.29/lammps_step/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      492 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-29 19:08:16.969673 lammps_step-2023.5.29/lammps_step/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/custom_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/custom_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.969673 lammps_step-2023.5.29/lammps_step/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/data/configuration.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/data/properties.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/data/seamm-lammps.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/energy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/energy_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/heat_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/heat_flux_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/heat_flux_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22441 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/initialization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/initialization_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24239 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91984 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/lammps_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/lammps_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11638 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/minimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/minimization_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23933 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/npt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/npt_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/npt_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16217 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/nve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/nve_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/nve_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/nvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/nvt_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/nvt_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/tk_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/tk_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/tk_heat_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/tk_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/tk_lammps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/tk_minimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30919 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/tk_npt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/tk_nve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/tk_nvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/tk_velocities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/velocities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/velocities_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/lammps_step/velocities_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.965673 lammps_step-2023.5.29/lammps_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-05-29 19:08:16.000000 lammps_step-2023.5.29/lammps_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-29 19:08:16.000000 lammps_step-2023.5.29/lammps_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 19:08:16.000000 lammps_step-2023.5.29/lammps_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-29 19:08:16.000000 lammps_step-2023.5.29/lammps_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-29 19:08:16.000000 lammps_step-2023.5.29/lammps_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 19:08:16.000000 lammps_step-2023.5.29/lammps_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 19:07:59.000000 lammps_step-2023.5.29/lammps_step.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-29 19:08:16.969673 lammps_step-2023.5.29/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.969673 lammps_step-2023.5.29/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:08:16.969673 lammps_step-2023.5.29/tests/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14459 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/tests/data/Ar_xtal_energy.flow
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/tests/test_lammps_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/tests/test_lammps_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-05-29 19:07:55.000000 lammps_step-2023.5.29/versioneer.py
```

### Comparing `lammps_step-2023.4.9/CONTRIBUTING.rst` & `lammps_step-2023.5.29/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/HISTORY.rst` & `lammps_step-2023.5.29/HISTORY.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,27 @@
 =======
 History
 =======
+2023.5.29 -- Self diffusion and other improvements
+   * Added trajectory panel to support diffusion, viscosity and simple thermal
+     conductivity.
+   * Added support for separate GPU versions of LAMMPS.
+   * Added support for command-line arguments to LAMMPS, mainly used for accelerators.
+   * Added support for using modules.
+
+2023.4.24 -- Support for thermal conductivity
+   * Internal changes to support thermal conductivity with its embedded flowchart.
+   * Added the heat flux substep.
+   * Now delete output and reference files when rerunning, so the output is clean.
+   * Internal changes to support running LAMMPS from a Python driver.
+   * Corrected units of properties returned from LAMMPS when e.g. metal units used.
+   * Added support for Buckingham potentials
+   * Fixed issues with and cleaned up the use of hybrid types for bonds, angles, ....
+   * Fixed issues with the alignment of some of the widgets in the GUI.
+     
 2023.4.9 -- Hid the warning from pymbar
    * Importing pymbar timeseries writes a warning to the terminal about its proper
      usage. SEAMM already handles the warned case, so the message is simply confusing to
      users and hence this release hides it.
      
 2023.4.6 -- Better forcefield handling.
    * Added correct molecule numbers for valence forcefields.
```

### Comparing `lammps_step-2023.4.9/LICENSE` & `lammps_step-2023.5.29/LICENSE`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/PKG-INFO` & `lammps_step-2023.5.29/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lammps_step
-Version: 2023.4.9
+Version: 2023.5.29
 Summary: A SEAMM plug-in for LAMMPS, a forcefield-based molecular dynamics code.
 Home-page: https://github.com/molssi-seamm/lammps_step
 Author: MolSSI @ Virginia Tech
 Author-email: seamm@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,forcefield,EAM,OpenKIM,molecular dynamics,atomistic,MD
 Platform: Linux
@@ -109,14 +109,31 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2023.5.29 -- Self diffusion and other improvements
+   * Added trajectory panel to support diffusion, viscosity and simple thermal
+     conductivity.
+   * Added support for separate GPU versions of LAMMPS.
+   * Added support for command-line arguments to LAMMPS, mainly used for accelerators.
+   * Added support for using modules.
+
+2023.4.24 -- Support for thermal conductivity
+   * Internal changes to support thermal conductivity with its embedded flowchart.
+   * Added the heat flux substep.
+   * Now delete output and reference files when rerunning, so the output is clean.
+   * Internal changes to support running LAMMPS from a Python driver.
+   * Corrected units of properties returned from LAMMPS when e.g. metal units used.
+   * Added support for Buckingham potentials
+   * Fixed issues with and cleaned up the use of hybrid types for bonds, angles, ....
+   * Fixed issues with the alignment of some of the widgets in the GUI.
+     
 2023.4.9 -- Hid the warning from pymbar
    * Importing pymbar timeseries writes a warning to the terminal about its proper
      usage. SEAMM already handles the warned case, so the message is simply confusing to
      users and hence this release hides it.
      
 2023.4.6 -- Better forcefield handling.
    * Added correct molecule numbers for valence forcefields.
```

### Comparing `lammps_step-2023.4.9/README.rst` & `lammps_step-2023.5.29/README.rst`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/docs/Makefile` & `lammps_step-2023.5.29/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/docs/_static/SEAMM inverted.png` & `lammps_step-2023.5.29/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/docs/_static/SEAMM logo.png` & `lammps_step-2023.5.29/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/docs/_static/molssi_main_logo.png` & `lammps_step-2023.5.29/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/docs/_static/molssi_main_logo_inverted_white.png` & `lammps_step-2023.5.29/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/docs/_static/molssi_square.png` & `lammps_step-2023.5.29/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/docs/_static/nsf.png` & `lammps_step-2023.5.29/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/docs/conf.py` & `lammps_step-2023.5.29/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/docs/developer_guide/installation.rst` & `lammps_step-2023.5.29/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/docs/getting_started/density.png` & `lammps_step-2023.5.29/docs/getting_started/density.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/docs/getting_started/edit_forcefield.png` & `lammps_step-2023.5.29/docs/getting_started/edit_forcefield.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/docs/getting_started/edit_initialization.png` & `lammps_step-2023.5.29/docs/getting_started/edit_initialization.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/docs/getting_started/edit_npt.png` & `lammps_step-2023.5.29/docs/getting_started/edit_npt.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/docs/getting_started/edit_packmol.png` & `lammps_step-2023.5.29/docs/getting_started/edit_packmol.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/docs/getting_started/flowchart.png` & `lammps_step-2023.5.29/docs/getting_started/flowchart.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/docs/getting_started/index.rst` & `lammps_step-2023.5.29/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/docs/getting_started/lammps_flowchart.png` & `lammps_step-2023.5.29/docs/getting_started/lammps_flowchart.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/docs/getting_started/nist.png` & `lammps_step-2023.5.29/docs/getting_started/nist.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/docs/index.rst` & `lammps_step-2023.5.29/docs/index.rst`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/docs/make.bat` & `lammps_step-2023.5.29/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/lammps_step/custom.py` & `lammps_step-2023.5.29/lammps_step/custom.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,8 +66,12 @@
         lines = []
 
         lines.append("")
         lines.append("#     custom scripting")
         lines.append("")
         lines.append(P["script"])
 
-        return lines
+        return {
+            "script": lines,
+            "postscript": None,
+            "use python": False,
+        }
```

### Comparing `lammps_step-2023.4.9/lammps_step/custom_parameters.py` & `lammps_step-2023.5.29/lammps_step/custom_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/lammps_step/custom_step.py` & `lammps_step-2023.5.29/lammps_step/custom_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/lammps_step/data/configuration.txt` & `lammps_step-2023.5.29/lammps_step/data/configuration.txt`

 * *Files 16% similar despite different names*

```diff
@@ -19,21 +19,22 @@
 
 # Whether to write local HTML files for the graphs, etc. generated so
 # they can be viewed without the SEAMM Dashboard.
 
 # html = False
 
 # Information about where/how the executables are installed
-# installation may be 'user', 'conda' or 'module'. If a module is
+# installation may be 'path', 'conda' or 'modules'. If a module is
 # specified it will be loaded and those executables used.  In this
 # case, any path specified using lammps-path will be ignored.
 
 installation = not installed
 conda-environment =
 modules = 
+gpu-modules =
 
 # The path to the executables. Can be empty or not present, in which
 # case the default PATH is used.  If a path is given, lmp_serial and
 # lmp_mpi from this location will be used. If mpiexec is also present
 # it will be used; otherwise mpiexec from the normal PATH will be
 # used. If mpiexec or lmp_mpi is not found, only the serial version of
 # LAMMPS will be used. Conversely, if lmp_serial is not present,
@@ -45,14 +46,34 @@
 
 lammps-path =
 
 # The various LAMMPS executables. You should leave these as their default
 # values unless you have a special need. These values are combined with
 # lammps-path to get the location of the executables.
 #
+# If you are running from a queueing system such as SLURM, if MPI was compiled
+# to know about the batch system, you should be able to use something like
+# 'srun' or 'mpirun' with no further arguments to run parallel tasks. If
+# you are not lucky, and need the parameters, you can add them to the command
+# line like this:
+#
+# mpiexec = mpirun -n {NTASKS} -H {NODELIST} -npernode {NTASKS_PER_NODE}
+#
+# SEAMM picks up the environment variables such as SLURM_NTASKS, strips the
+# prefix from them and replaces any instances in the command line that are
+# enclosed in braces. Hopefully this lets you construct the correct command
+# line.
+#
 # The LAMMPS installer does not handle these variables! They are here
 # just in case!
 
 # lammps-serial = lmp_serial
 # lammps-mpi = lmp_mpi
 # mpiexec = mpiexec
 
+# Optional command-line arguments for LAMMPS. These are usually used with accelerators
+# such as Kokkos or GPU to automatically apply the accelerator. Again there is a normal
+# and GPU version
+
+# cmd-args = -k on -sf kk
+# gpu-cmd-args = -k on g {ngpus} -sf kk -pk kokkos gpu/aware on newton on neigh full neigh/thread on neigh/transpose off comm device
+
```

### Comparing `lammps_step-2023.4.9/lammps_step/data/properties.csv` & `lammps_step-2023.5.29/lammps_step/data/properties.csv`

 * *Files 4% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 "pressure, inefficiency#LAMMPS#{model}",float,,"The statistical inefficiency of the pressure sampling.",https://en.wikipedia.org/wiki/Efficiency_(statistics)
 "temperature#LAMMPS#{model}",float,K,"The temperature.",https://en.wikipedia.org/wiki/Temperature
 "temperature, stderr#LAMMPS#{model}",float,K,"The standard error of the temperature.",https://en.wikipedia.org/wiki/Standard_error
 "temperature, tau#LAMMPS#{model}",float,fs,"The autocorrelation time of the temperature.",https://en.wikipedia.org/wiki/Autocorrelation
 "temperature, inefficiency#LAMMPS#{model}",float,,"The statistical inefficiency of the temperature sampling.",https://en.wikipedia.org/wiki/Efficiency_(statistics)
 "total energy#LAMMPS#{model}",float,kJ/mol,"The {model} total energy.",
 "total energy, stderr#LAMMPS#{model}",float,kJ/mol,"The standard error of the {model} total energy.",https://en.wikipedia.org/wiki/Standard_error
-"total energy, tau#LAMMPS#{model}",float,kJ/mol,"The autocorellation time of the {model} total energy.",https://en.wikipedia.org/wiki/Autocorrelation
-"total energy, inefficiency#LAMMPS#{model}",float,kJ/mol,"The statistical inefficiency of the {model} total energy.",https://en.wikipedia.org/wiki/Efficiency_(statistics)
+"total energy, tau#LAMMPS#{model}",float,fs,"The autocorellation time of the {model} total energy.",https://en.wikipedia.org/wiki/Autocorrelation
+"total energy, inefficiency#LAMMPS#{model}",float,,"The statistical inefficiency of the {model} total energy.",https://en.wikipedia.org/wiki/Efficiency_(statistics)
 "kinetic energy#LAMMPS#{model}",float,kJ/mol,"The {model} kinetic energy.",https://en.wikipedia.org/wiki/Kinetic_energy
 "kinetic energy, stderr#LAMMPS#{model}",float,kJ/mol,"The standard error of the {model} kinetic energy.",https://en.wikipedia.org/wiki/Standard_error
-"kinetic energy, tau#LAMMPS#{model}",float,kJ/mol,"The autocorellation time of the {model} kinetic energy.",https://en.wikipedia.org/wiki/Autocorrelation
-"kinetic energy, inefficiency#LAMMPS#{model}",float,kJ/mol,"The statistical inefficiency of the {model} kinetic energy.",https://en.wikipedia.org/wiki/Efficiency_(statistics)
+"kinetic energy, tau#LAMMPS#{model}",float,fs,"The autocorellation time of the {model} kinetic energy.",https://en.wikipedia.org/wiki/Autocorrelation
+"kinetic energy, inefficiency#LAMMPS#{model}",float,,"The statistical inefficiency of the {model} kinetic energy.",https://en.wikipedia.org/wiki/Efficiency_(statistics)
 "potential energy#LAMMPS#{model}",float,kJ/mol,"The {model} potential energy.",https://en.wikipedia.org/wiki/Potential_energy
 "potential energy, stderr#LAMMPS#{model}",float,kJ/mol,"The standard error of the {model} potential energy.",https://en.wikipedia.org/wiki/Standard_error
-"potential energy, tau#LAMMPS#{model}",float,kJ/mol,"The autocorellation time of the {model} potential energy.",https://en.wikipedia.org/wiki/Autocorrelation
-"potential energy, inefficiency#LAMMPS#{model}",float,kJ/mol,"The statistical inefficiency of the {model} potential energy.",https://en.wikipedia.org/wiki/Efficiency_(statistics)
+"potential energy, tau#LAMMPS#{model}",float,fs,"The autocorellation time of the {model} potential energy.",https://en.wikipedia.org/wiki/Autocorrelation
+"potential energy, inefficiency#LAMMPS#{model}",float,,"The statistical inefficiency of the {model} potential energy.",https://en.wikipedia.org/wiki/Efficiency_(statistics)
```

### Comparing `lammps_step-2023.4.9/lammps_step/data/references.bib` & `lammps_step-2023.5.29/lammps_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/lammps_step/energy_parameters.py` & `lammps_step-2023.5.29/lammps_step/energy_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/lammps_step/energy_step.py` & `lammps_step-2023.5.29/lammps_step/energy_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/lammps_step/initialization.py` & `lammps_step-2023.5.29/lammps_step/initialization.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,15 +127,15 @@
                 or final values. If None, then the parameters values will
                 be used as is.
         """
 
         if not P:
             P = self.parameters.values_to_dict()
 
-        text = "Initialize the calculation with a cutoff of {cutoff} Å"
+        text = "Initialize the calculation with a cutoff of {cutoff}"
         if P["shift_nonbond"]:
             text += ", shifting the nonbond energies to 0 at the cutoff"
         text += ". If the system is periodic"
         if P["kspace_method"][0] == "$":
             text += " use the variable '{method}' to determine whether "
             text += "and how to accelerate the k-space summations."
         elif P["kspace_method"] == "none":
@@ -198,14 +198,16 @@
             for charge in charges:
                 if abs(charge) > smallq:
                     n_charged_atoms += 1
             fraction_charged_atoms = n_charged_atoms / n_atoms
         else:
             n_charged_atoms = 0
 
+        kspace_style = ""
+
         lines = []
         lines.append("")
         lines.append("#     initialization of LAMMPS")
         lines.append("")
         lines.append("units               real")
 
         periodicity = configuration.periodicity
@@ -226,14 +228,18 @@
 
         lines.append("atom_style          full")
         lines.append("newton              on")
         if n_atoms < 20:
             # LAMMPS has problems with bins for small systems
             lines.append("neighbor            2.0 nsq")
         lines.append("")
+        if periodicity == 3:
+            a, b, c, alpha, beta, gamma = configuration.cell.parameters
+            if alpha != 90 or beta != 90 or gamma != 90:
+                lines.append("box                 tilt large")
         lines.append("#    define the style of forcefield")
         lines.append("")
 
         terms = ff.ff["terms"]
 
         logging.debug("LAMMPS initialization, terms = \n" + pprint.pformat(terms))
 
@@ -264,21 +270,23 @@
                         if mixing != item.split()[1]:
                             raise RuntimeError(
                                 "Conflicting combination rules in "
                                 "nonbond(12-6) section '" + section + "'"
                             )
             if mixing == "":
                 mixing = "geometric"
+        elif nonbond_term == "buckingham":
+            pair_style_base = "buck"
+            mixing = None
         else:
             raise RuntimeError("Can't handle nonbond term {} yet!".format(nonbond_term))
 
         shift = "yes" if P["shift_nonbond"] else "no"
         if P["kspace_method"] == "automatic":
             if periodicity == 3:
-                kspace_style = ""
                 if n_charged_atoms == 0:
                     pair_style = pair_style_base
                     string += (
                         " The nonbonded interactions will be evaluated using "
                         "a cutoff of {cutoff} Å. Since there are no charges "
                         "on the atoms, no long-range coulomb method will be "
                         "used."
@@ -309,19 +317,24 @@
                         string += (
                             "using the PPPM method with "
                             "an accuracy of {kspace_accuracy}."
                         )
                 lines.append(
                     "pair_style          {} {}".format(pair_style, P["cutoff"])
                 )
-                lines.append(
-                    "pair_modify         mix "
-                    + mixing
-                    + " tail {} shift {}".format(tail_correction, shift)
-                )
+                if mixing is None:
+                    lines.append(
+                        f"pair_modify         tail {tail_correction} shift {shift}"
+                    )
+                else:
+                    lines.append(
+                        "pair_modify         mix "
+                        + mixing
+                        + " tail {} shift {}".format(tail_correction, shift)
+                    )
                 if shift:
                     string += (
                         " The van der Waals terms will be shifted "
                         "to zero energy at the cutoff distance."
                     )
                 if tail_correction:
                     string += (
@@ -374,17 +387,18 @@
                     string += (
                         " The van der Waals terms will be shifted "
                         "to zero energy at the cutoff distance."
                     )
                 lines.append(
                     "pair_style          {} {}".format(pair_style, P["cutoff"])
                 )
-                lines.append(
-                    "pair_modify         mix " + mixing + " shift {}".format(shift)
-                )
+                if mixing is None:
+                    lines.append(f"pair_modify         shift {shift}")
+                else:
+                    lines.append(f"pair_modify         mix {mixing} shift {shift}")
                 if kspace_style != "":
                     lines.append("kspace_style        " + kspace_style.format(**P))
             self.description.append(__(string, indent=7 * " ", **P))
         else:
             if periodicity == 3:
                 kspace_style = ""
                 if n_charged_atoms == 0 or P["kspace_style"] == "none":
@@ -393,89 +407,95 @@
                     pair_style = pair_style_base + "/coul/long"
                     kspace_style = lammps_step.kspace_methods[
                         P["kspace_method"]
                     ].format(**P)
                 lines.append(
                     "pair_style          {} {}".format(pair_style, P["cutoff"])
                 )
-                lines.append(
-                    "pair_modify         mix "
-                    + mixing
-                    + " tail {} shift {}".format(tail_correction, shift)
-                )
-                if kspace_style != "":
-                    lines.append("kspace_style        " + kspace_style)
+                if mixing is None:
+                    lines.append(
+                        f"pair_modify         tail {tail_correction} shift {shift}"
+                    )
+                else:
+                    lines.append(
+                        "pair_modify         mix "
+                        + mixing
+                        + " tail {} shift {}".format(tail_correction, shift)
+                    )
             else:
                 if n_charged_atoms == 0:
                     pair_style = pair_style_base
                 else:
                     pair_style = pair_style_base + "/coul/cut"
                 lines.append(
                     "pair_style          {} {}".format(pair_style, P["cutoff"])
                 )
-                lines.append(
-                    "pair_modify         mix " + mixing + " shift {}".format(shift)
-                )
+                if mixing is None:
+                    lines.append(f"pair_modify         shift {shift}")
+                else:
+                    lines.append(f"pair_modify         mix {mixing} shift {shift}")
                 if "msm" in lammps_step.kspace_methods[P["kspace_method"]]:
                     kspace_style = lammps_step.kspace_methods[
                         P["kspace_method"]
                     ].format(**P)
-                    lines.append("kspace_style        " + kspace_style)
 
         if "bond" in terms and eex["n_bonds"] > 0:
-            if len(terms["bond"]) == 1:
-                bond_style = lammps_step.bond_style[terms["bond"][0]]
+            forms = set([v[0] for v in eex["bond parameters"]])
+            if len(forms) == 1:
+                bond_style = lammps_step.bond_style[[*forms][0]]
                 lines.append("bond_style          " + bond_style)
             else:
                 line = "bond_style          hybrid"
-                for term in terms["bond"]:
+                for term in forms:
                     line += " " + lammps_step.bond_style[term]
                 lines.append(line)
         if "angle" in terms and eex["n_angles"] > 0:
-            if len(terms["angle"]) == 1:
-                angle_style = lammps_step.angle_style[terms["angle"][0]]
+            forms = set([v[0] for v in eex["angle parameters"]])
+            if len(forms) == 1:
+                angle_style = lammps_step.angle_style[[*forms][0]]
                 lines.append("angle_style         " + angle_style)
             else:
                 line = "angle_style         hybrid"
-                for term in terms["angle"]:
+                for term in forms:
                     line += " " + lammps_step.angle_style[term]
                 lines.append(line)
         if "torsion" in terms and eex["n_torsions"] > 0:
-            if len(terms["torsion"]) == 1:
-                #  yapf: disable
-                dihedral_style = lammps_step.dihedral_style[
-                    terms["torsion"][0]
-                ]  # noqa: E501
-                #  yapf: enable
+            forms = set([v[0] for v in eex["torsion parameters"]])
+            if len(forms) == 1:
+                dihedral_style = lammps_step.dihedral_style[[*forms][0]]
                 lines.append("dihedral_style      " + dihedral_style)
             else:
                 line = "dihedral_style      hybrid"
-                for term in terms["torsion"]:
+                for term in forms:
                     line += " " + lammps_step.dihedral_style[term]
                 lines.append(line)
         if "out-of-plane" in terms and eex["n_oops"] > 0:
-            if len(terms["out-of-plane"]) == 1:
-                improper_style = lammps_step.improper_style[terms["out-of-plane"][0]]
+            forms = set([v[0] for v in eex["oop parameters"]])
+            if len(forms) == 1:
+                improper_style = lammps_step.improper_style[[*forms][0]]
                 lines.append("improper_style      " + improper_style)
             else:
                 line = "improper_style      hybrid"
-                for term in terms["out-of-plane"]:
+                for term in forms:
                     line += " " + lammps_step.improper_style[term]
                 lines.append(line)
 
         lines.append("")
 
         # Handle 1-4s in nonbonds
         if "opls" in ffname:
             lines.append("special_bonds       lj/coul 0.0 0.0 0.5")
             lines.append("")
 
         if extras is not None and "read_data" in extras and extras["read_data"] is True:
             lines.append("read_data           structure.dat")
 
+        if kspace_style != "":
+            lines.append("kspace_style        " + kspace_style)
+
         # Set up standard variables
         for variable in thermo_variables:
             lines.append("variable            {var} equal {var}".format(var=variable))
 
         return (lines, eex)
 
     def OpenKIM_input(self):
```

### Comparing `lammps_step-2023.4.9/lammps_step/initialization_parameters.py` & `lammps_step-2023.5.29/lammps_step/initialization_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/lammps_step/initialization_step.py` & `lammps_step-2023.5.29/lammps_step/initialization_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/lammps_step/installer.py` & `lammps_step-2023.5.29/lammps_step/installer.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,23 +85,23 @@
         If the option `yes` is present and True, this method will attempt to
         correct any errors in the configuration file. Use `--yes` on the
         command line to enable this.
 
         The information in the configuration file is:
 
             installation
-                How LAMMPS is installed. One of `user`, `modules` or `conda`
+                How LAMMPS is installed. One of `path`, `modules` or `conda`
             conda-environment
                 The Conda environment if and only if `installation` = `conda`
             modules
                 The environment modules if `installation` = `modules`
             lammps-path
                 The path where the LAMMPS executables are. Automatically
                 defined if `installation` is `conda` or `modules`, but given
-                by the user is it is `user`.
+                by the user is it is `path`.
 
         Returns
         -------
         bool
             True if everything is OK, False otherwise. If `yes` is given as an
             option, the return value is after fixing the configuration.
         """
@@ -150,15 +150,15 @@
         ):
             lammps_path = None
         else:
             lammps_path = initial_lammps_path
         self.logger.debug(f"initial-lammps-path = {initial_lammps_path}.")
 
         # Is there an installation indicated?
-        if initial_installation in ("user", "conda", "modules"):
+        if initial_installation in ("path", "conda", "modules"):
             installation = initial_installation
         else:
             installation = None
         self.logger.debug(f"initial-installation = {initial_installation}.")
 
         if installation == "conda":
             # Is there a conda environment?
@@ -292,28 +292,26 @@
                     if self.options.yes or self.ask_yes_no(
                         "Found LAMMPS executables in the PATH at "
                         f"{lammps_path}\n"
                         "Use them?",
                         default="yes",
                     ):
                         self.configuration.set_value(
-                            self.section, "installation", "user"
+                            self.section, "installation", "path"
                         )
                         self.configuration.set_value(
                             self.section, "conda-environment", ""
                         )
                         self.configuration.set_value(self.section, "modules", "")
                         self.configuration.save()
                         print("Using the LAMMPS executables at {lammps_path}")
 
             if lammps_path is None:
                 # Can't find LAMMPS
-                print(
-                    "Cannot find LAMMPS executables. You will need to install " "them."
-                )
+                print("Cannot find LAMMPS executables. You will need to install them.")
                 if (
                     initial_installation is not None
                     and initial_installation != "not installed"
                 ):
                     if self.options.yes or self.ask_yes_no(
                         "The configuration file indicates that LAMMPS "
                         "is installed, but it can't be found.\n"
@@ -383,21 +381,34 @@
             if path is not None:
                 path = Path(path).expanduser().resolve()
                 break
         return path
 
     def install(self):
         """Install LAMMPS using a Conda environment."""
+        if self.configuration.section_exists(self.section):
+            # Get the values from the configuration
+            data = self.configuration.get_values(self.section)
+            if "installation" in data:
+                initial_installation = data["installation"]
+                if initial_installation == "path":
+                    print("Using LAMMPS for the path given by the user.")
+                    return
+                elif initial_installation == "modules":
+                    print("Using LAMMPS from the modules given by the user.")
+                    return
+        else:
+            # Update the configuration file.
+            self.check_configuration_file()
+
         print(
             f"Installing Conda environment '{self.environment}'. This "
             "may take a minute or two."
         )
         self.conda.create_environment(self.environment_file, name=self.environment)
-        # Update the configuration file.
-        self.check_configuration_file()
         path = self.conda.path(self.environment) / "bin"
         self.configuration.set_value(self.section, "lammps-path", str(path))
         self.configuration.set_value(self.section, "installation", "conda")
         self.configuration.set_value(
             self.section, "conda-environment", self.environment
         )
         self.configuration.set_value(self.section, "modules", "")
@@ -446,19 +457,21 @@
                         extra = (
                             "from Conda environment " f"{data['conda-environment']}."
                         )
                     else:
                         extra = "from an unknown Conda environment."
                 elif installation == "modules":
                     if "modules" in data and data["modules"] != "":
-                        extra = f"from module(s) {data['modules']}."
+                        print(f"from module(s) {data['modules']}.")
                     else:
-                        extra = "from unknown modules."
-                elif installation == "user":
-                    extra = f"from user-defined path {conf_path}."
+                        print("from unknown modules.")
+                    return
+                elif installation == "path":
+                    print(f"from user-defined path {conf_path}.")
+                    return
 
             if serial is not None:
                 if mpi is not None:
                     if serial_version == mpi_version:
                         print(
                             "LAMMPS serial and mpi executables, version "
                             f"'{serial_version}'"
```

### Comparing `lammps_step-2023.4.9/lammps_step/lammps.py` & `lammps_step-2023.5.29/lammps_step/lammps.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 # -*- coding: utf-8 -*-
 
 """A node or step for LAMMPS in a flowchart"""
 
 from contextlib import contextmanager
 import copy
-import glob
+import json
 import logging
 from math import sqrt, exp, degrees, radians, cos, acos
 from pathlib import Path
 import os
 import os.path
 import pkg_resources
 import pprint
-import re
 import shutil
 import string
 import sys
 import traceback
+import warnings
 
 import bibtexparser
-import numpy
+import numpy as np
 import pandas
 import psutil
-from scipy.stats import t as t_student
+from scipy import stats
 import statsmodels.tsa.stattools as stattools
 
 import lammps_step
 import molsystem
 import seamm
 import seamm_util
 import seamm_util.printing as printing
+from seamm_util import CompactJSONEncoder
 from seamm_util.printing import FormattedText as __
 
 # from pymbar import timeseries
 
 logger = logging.getLogger("lammps")
 job = printing.getPrinter()
 printer = printing.getPrinter("lammps")
@@ -66,14 +67,15 @@
     finally:
         logging.disable(previous_level)
 
 
 with logging_disabled(highest_level=logging.WARNING):
     from pymbar import timeseries
 
+
 # Add LAMMPS's properties to the standard properties
 path = Path(pkg_resources.resource_filename(__name__, "data/"))
 csv_file = path / "properties.csv"
 molsystem.add_properties_from_file(csv_file)
 
 bond_style = {
     "quadratic_bond": "harmonic",
@@ -101,37 +103,55 @@
 
 
 class LAMMPS(seamm.Node):
     display_units = {
         "T": "K",
         "P": "atm",
         "t": "fs",
+        "V": "Å^3",
         "density": "g/mL",
         "a": "Å",
         "b": "Å",
         "c": "Å",
         "Etot": "kcal/mol",
         "Eke": "kcal/mol",
         "Epe": "kcal/mol",
         "Emol": "kcal/mol",
         "Epair": "kcal/mol",
+        "Jx": "W/m^2",
+        "Jy": "W/m^2",
+        "Jz": "W/m^2",
+        "Kappa_x": "W/K/m",
+        "Kappa_y": "W/K/m",
+        "Kappa_z": "W/K/m",
+        "Kappa": "W/K/m",
+        "u": "kcal/mol",
     }
     display_title = {
         "T": "Temperature",
         "P": "Pressure",
         "t": "Time",
+        "V": "Volume",
         "density": "Density",
         "a": "a lattice parameter",
         "b": "b lattice parameter",
         "c": "c lattice parameter",
         "Etot": "Total Energy",
         "Eke": "Kinetic Energy",
         "Epe": "Potential Energy",
         "Emol": "Molecular Energy, Valence Terms",
         "Epair": "Pair (Nonbond) Energy",
+        "Jx": "heat flux in x",
+        "Jy": "heat flux in y",
+        "Jz": "heat flux in z",
+        "Kappa_x": "thermal conductivity in x",
+        "Kappa_y": "thermal conductivity in y",
+        "Kappa_z": "thermal conductivity in z",
+        "Kappa": "thermal conductivity",
+        "u": "atom PE",
     }
 
     def __init__(
         self, flowchart=None, namespace="org.molssi.seamm.lammps", extension=None
     ):
         """Setup the main LAMMPS step
 
@@ -186,15 +206,15 @@
         """Convert cell parameters to the LAMMPS box."""
         if alpha == 90 and beta == 90 and gamma == 90:
             lx = a
             ly = b
             lz = c
             xy = xz = yz = 0.0
         else:
-            lx = 0
+            lx = a
             xy = b * cos(radians(gamma))
             xz = c * cos(radians(beta))
             ly = sqrt(b**2 - xy**2)
             yz = (b * c * cos(radians(alpha)) - xy * xz) / ly
             lz = sqrt(c**2 - xz**2 - yz**2)
 
         return (lx, ly, lz, xy, xz, yz)
@@ -242,14 +262,21 @@
             "--modules",
             nargs="*",
             default=None,
             help="the environment modules to load for LAMMPS",
         )
         parser.add_argument(
             parser_name,
+            "--gpu-modules",
+            nargs="*",
+            default=None,
+            help="the environment modules to load for the GPU version of LAMMPS",
+        )
+        parser.add_argument(
+            parser_name,
             "--lammps-path",
             default=None,
             help="the path to the LAMMPS executables",
         )
         parser.add_argument(
             parser_name,
             "--lammps-serial",
@@ -259,14 +286,26 @@
         parser.add_argument(
             parser_name,
             "--lammps-mpi",
             default="lmp_mpi",
             help="the mpi version of LAMMPS",
         )
         parser.add_argument(
+            parser_name,
+            "--cmd-args",
+            default="",
+            help="the command-line arguments for LAMMPS, e.g. '-k on'",
+        )
+        parser.add_argument(
+            parser_name,
+            "--gpu-cmd-args",
+            default="",
+            help="the command-line arguments for GPU version of LAMMPS, e.g. '-k on'",
+        )
+        parser.add_argument(
             parser_name, "--mpiexec", default="mpiexec", help="the mpi executable"
         )
 
         return result
 
     def set_id(self, node_id):
         """Set the id for node to a given tuple"""
@@ -369,18 +408,14 @@
             else:
                 np = int(np)
         else:
             np = 1
 
         # Print headers and get to work
         printer.important(self.header)
-        if np > 1:
-            printer.important("    LAMMPS using MPI with {} processes.\n".format(np))
-        else:
-            printer.important("   LAMMPS using the serial version.\n")
 
         self.subflowchart.root_directory = self.flowchart.root_directory
 
         files = {}
 
         # Get the first real node
         node = self.subflowchart.get_node("1").next()
@@ -480,17 +515,15 @@
                         node_id = node._id[1]
                         for prp, v in analysis[node_id].items():
                             if v["short_production"] is False:
                                 if v["few_neff"] is False:
                                     accuracy = control_properties[prp]["accuracy"] / 100
                                     dof = v["n_sample"]
                                     mean = v["mean"]
-                                    ci = t_student.interval(
-                                        0.95, dof - 1, loc=0, scale=1
-                                    )
+                                    ci = stats.t.interval(0.95, dof - 1, loc=0, scale=1)
                                     interval = (ci[1] - ci[0]) * v["sem"]
                                     print(abs(interval / mean))
                                     if abs(interval / mean) < accuracy:
                                         control_properties[prp][
                                             "enough_accuracy"
                                         ] = True
                         enough_acc = [
@@ -537,19 +570,22 @@
             base = "lammps"
 
             restart = base + ".restart.*"
             dump = base + ".dump.*"
             input_file = base + ".dat"
             new_input_data = []
             new_input_data.append("run          0")
-            new_input_data.append(f"write_restart          {restart}")
+            new_input_data.append(f"write_restart      {restart}")
 
             new_input_data.append(
-                f"write_dump all custom  {dump} id " "xu yu zu modify flush yes sort id"
+                f"write_dump          all custom  {dump} id "
+                "xu yu zu modify flush yes sort id"
             )
+            new_input_data.append("")
+            new_input_data.append("info               computes fixes dumps log out")
 
             files["input"]["filename"] = input_file
             files["input"]["data"] += new_input_data
             files["input"]["data"] = "\n".join(files["input"]["data"])
 
             self.logger.debug(
                 files["input"]["filename"] + ":\n" + files["input"]["data"]
@@ -568,15 +604,23 @@
 
             files = self._execute_single_sim(files, np=np)
 
             self.analyze(nodes=history_nodes)
 
             self._trajectory = []
 
-        self.read_dump(os.path.join(self.directory, files["dump"]["filename"]))
+        if "dump" in files:
+            try:
+                self.read_dump(os.path.join(self.directory, files["dump"]["filename"]))
+            except Exception as e:
+                printer.normal("Warning: unable to read the LAMMPS dumpfile")
+                logger.warning(f"The was a problem reading the LAMMPS dumpfile: {e}")
+                logger.warning(traceback.format_exc())
+        else:
+            printer.normal("Warning: there is no 'dump' file from LAMMPS")
 
         printer.normal("")
 
         return next_node
 
     def _execute_single_sim(self, files, np=1, return_files=None):
         """
@@ -596,185 +640,317 @@
                 fd.write(v["data"])
 
             tmpdict[v["filename"]] = v["data"]
 
         return_files = [
             "summary_*.txt",
             "trajectory_*.seamm_trj",
+            "*.trj",
             "*.restart.*",
             "*.dump.*",
             "*.log",
             "*.dat",
+            "log.lammps",
             "log.cite",
-        ]  # yapf: disable
+            "run_lammps",
+        ]
 
-        local = seamm.ExecLocal()
-
-        # Find the executables and if they exist.
-        lammps_path = Path(self.options["lammps_path"]).expanduser().resolve()
-        lmp_serial = lammps_path / self.options["lammps_serial"]
-        lmp_serial = lmp_serial.expanduser().resolve()
-        if not lmp_serial.exists():
-            lmp_serial = None
-
-        lmp_mpi = lammps_path / self.options["lammps_mpi"]
-        lmp_mpi = lmp_mpi.expanduser().resolve()
-        if lmp_mpi.exists():
-            mpiexec = lammps_path / self.options["mpiexec"]
-            mpiexec = mpiexec.expanduser().resolve()
-            if not mpiexec.exists():
-                # See if it is in the path
-                mpiexec = shutil.which(self.options["mpiexec"])
-                if mpiexec is None:
+        # Check for already having run
+        path = Path(self.directory) / "success.dat"
+        if path.exists():
+            result = {}
+            path = Path(self.directory) / "log.cite"
+            if path.exists():
+                result["log.cite"] = {
+                    "data": path.read_text(),
+                }
+            path = Path(self.directory) / "stdout.txt"
+            if path.exists():
+                result["stdout"] = path.read_text()
+            result["stderr"] = ""
+        else:
+            # See if we are running in a batch job: SLURM, etc...
+            batch = {}
+            if "SLURM_JOBID" in os.environ:
+                batch["type"] = "slurm"
+                for item, value in os.environ.items():
+                    if item[0:6] == "SLURM_":
+                        batch[item[6:]] = value
+
+                if np > int(batch["NTASKS"]):
+                    np = int(batch["NTASKS"])
+                batch["NTASKS"] = np
+
+                if "NTASKS_PER_NODE" not in batch:
+                    batch["NTASKS_PER_NODE"] = int(batch["NTASKS"]) // int(
+                        batch["NNODES"]
+                    )
+
+                # Expand `[i-k]` naming in nodelist
+                nodes = batch["NODELIST"].split(",")
+                nodelist = []
+                npernode = batch["NTASKS_PER_NODE"]
+                for node in nodes:
+                    if "[" in node:
+                        node, count = node.split("[")
+                        first, last = count[0:-1].split("-")
+                        for i in range(int(first), int(last) + 1):
+                            nodelist.append(f"{node}{i}:{npernode}")
+                    else:
+                        nodelist.append(f"{node}:{npernode}")
+                nodelist = ",".join(nodelist)
+                batch["NODELIST"] = nodelist
+
+                if "JOB_GPUS" in batch:
+                    batch["ngpus"] = len(batch["JOB_GPUS"].split(","))
+
+            local = seamm.ExecLocal()
+
+            # Find the executables and if they exist.
+            if "ngpus" not in batch:
+                modules = self.options["modules"]
+            else:
+                modules = self.options["gpu_modules"]
+            serial = True
+            if len(modules) > 0:
+                # Use a module for LAMMPS
+                shell = True
+                cmd = []
+                cmd.append(f"module load {modules}")
+                lmp_serial = self.options["lammps_serial"]
+                lmp_mpi = self.options["lammps_mpi"]
+                mpiexec = self.options["mpiexec"]
+                if "python script" in files:
+                    python = "python"
+                    if lmp_mpi != "" and (np > 1 or lmp_serial == ""):
+                        serial = False
+                        text = mpiexec.format(**batch) + " python run_lammps"
+                    else:
+                        text = "python run_lammps"
+                    if "ngpus" not in batch and self.options["cmd_args"] != "":
+                        text += " --cmd-args '"
+                        text += self.options["cmd_args"].format(**batch)
+                        text += "'"
+                    if "ngpus" in batch and self.options["gpu_cmd_args"] != "":
+                        text += " --cmd-args '"
+                        text += self.options["gpu_cmd_args"].format(**batch)
+                        text += "'"
+                else:
+                    if lmp_mpi != "" and (np > 1 or lmp_serial == ""):
+                        serial = False
+                        text = mpiexec.format(**batch) + " " + lmp_mpi
+                    else:
+                        text = lmp_serial
+                    if "ngpus" not in batch and self.options["cmd_args"] != "":
+                        text += " " + self.options["cmd_args"].format(**batch)
+                    if "ngpus" in batch and self.options["gpu_cmd_args"] != "":
+                        text += " " + self.options["gpu_cmd_args"].format(**batch)
+                    text += " -in lammps.dat"
+                cmd.append(text)
+                cmd = "\n".join(cmd)
+            else:
+                shell = False
+                lammps_path = Path(self.options["lammps_path"]).expanduser().resolve()
+                lmp_serial = lammps_path / self.options["lammps_serial"]
+                lmp_serial = lmp_serial.expanduser().resolve()
+                if not lmp_serial.exists():
+                    lmp_serial = None
+
+                lmp_mpi = lammps_path / self.options["lammps_mpi"]
+                lmp_mpi = lmp_mpi.expanduser().resolve()
+                if lmp_mpi.exists():
+                    tmp = self.options["mpiexec"].format(**batch).split()
+                    mpiexec = lammps_path / tmp[0]
+                    mpi_options = tmp[1:]
+                    mpiexec = mpiexec.expanduser().resolve()
+                    if not mpiexec.exists():
+                        # See if it is in the path
+                        mpiexec = shutil.which(tmp[0])
+                        if mpiexec is None:
+                            lmp_mpi = None
+                        else:
+                            mpiexec = Path(mpiexec).expanduser().resolve()
+                else:
                     lmp_mpi = None
+
+                # Use the parallel executable if the serial does not exist, and vice
+                # versa
+                if "python script" in files:
+                    python = lammps_path / "python"
+                    if lmp_mpi is not None and (np > 1 or lmp_serial is None):
+                        serial = False
+                        cmd = [str(mpiexec)]
+                        cmd.extend(mpi_options)
+                        cmd.append(str(python))
+                        cmd.append("run_lammps")
+                    else:
+                        cmd = [str(python), "run_lammps"]
+                    if "ngpus" not in batch and self.options["cmd_args"] != "":
+                        cmd_args = self.options["cmd_args"].format(**batch)
+                        cmd.extend(["--cmd-args", cmd_args])
+                    if "ngpus" in batch and self.options["gpu_cmd_args"] != "":
+                        cmd_args = self.options["gpu_cmd_args"].format(**batch)
+                        cmd.extend(["--cmd-args", cmd_args])
                 else:
-                    mpiexec = Path(mpiexec).expanduser().resolve()
-        else:
-            lmp_mpi = None
+                    if lmp_mpi is not None and (np > 1 or lmp_serial is None):
+                        serial = False
+                        cmd = [str(mpiexec)]
+                        cmd.extend(mpi_options)
+                        cmd.append(str(lmp_mpi))
+                    else:
+                        cmd = [str(lmp_serial)]
+                    if "ngpus" not in batch and self.options["cmd_args"] != "":
+                        cmd.extend(self.options["cmd_args"].format(**batch).split())
+                    if "ngpus" in batch and self.options["gpu_cmd_args"] != "":
+                        cmd.extend(self.options["gpu_cmd_args"].format(**batch).split())
+                    cmd.extend(["-in", files["input"]["filename"]])
 
-        # Use the parallel executable if the serial does not exist, and vice
-        # versa
-        if lmp_mpi is not None and (np > 1 or lmp_serial is None):
-            cmd = [str(mpiexec), "-np", str(np), str(lmp_mpi)]
-        else:
-            cmd = [str(lmp_serial)]
-        cmd.extend(["-in", files["input"]["filename"]])
+            if serial:
+                printer.important("   LAMMPS using the serial version.\n")
+            else:
+                if "ngpus" in batch:
+                    printer.important(
+                        f"    LAMMPS using MPI with {np} processes and "
+                        f"{batch['ngpus']} gpus.\n"
+                    )
+                else:
+                    printer.important(f"    LAMMPS using MPI with {np} processes")
 
-        result = local.run(
-            cmd=cmd,
-            files=tmpdict,
-            return_files=return_files,
-            in_situ=True,
-            directory=self.directory,
-        )
+            result = local.run(
+                cmd=cmd,
+                files=tmpdict,
+                return_files=return_files,
+                in_situ=True,
+                directory=self.directory,
+                shell=shell,
+            )
 
-        if result is None:
-            self.logger.error("There was an error running LAMMPS")
-            return None
+            if result is None:
+                self.logger.error("There was an error running LAMMPS")
+                return None
 
-        self.logger.debug("\n" + pprint.pformat(result))
+            self.logger.debug("\n" + pprint.pformat(result))
 
-        self.logger.debug("stdout:\n" + result["stdout"])
+            self.logger.debug("stdout:\n" + result["stdout"])
 
-        f = os.path.join(self.directory, "stdout.txt")
-        with open(f, mode="w") as fd:
-            fd.write(result["stdout"])
+            f = os.path.join(self.directory, "stdout.txt")
+            with open(f, mode="w") as fd:
+                fd.write(result["stdout"])
 
         # Add the citations, getting the version from stdout and any citations
         if "log.cite" in result:
             self._add_lammps_citations(
                 result["stdout"], cite=result["log.cite"]["data"]
             )
         else:
             self._add_lammps_citations(result["stdout"])
 
-        if result["stderr"] != "":
-            self.logger.warning("stderr:\n" + result["stderr"])
-            f = os.path.join(self.directory, "stderr.txt")
-            with open(f, mode="w") as fd:
-                fd.write(result["stderr"])
-
-        for filename in result["files"]:
-            f = os.path.join(self.directory, filename)
-            mode = "wb" if type(result[filename]["data"]) is bytes else "w"
-            with open(f, mode=mode) as fd:
-                if result[filename]["data"] is not None:
-                    fd.write(result[filename]["data"])
-                else:
-                    fd.write(result[filename]["exception"])
-
         base = os.path.basename(files["input"]["filename"][0:-4])
-        restart_file = base + ".restart.*"
-        dump_file = base + ".dump.*"
-        filename = os.path.join(self.directory, restart_file)
-        restart_filenames = glob.glob(filename)
-
-        # Probably the step didn't run
-        if len(restart_filenames) == 0:
-            raise FileNotFoundError(
-                "Lammps_step: could not find any file with the pattern %s" % (filename)
-            )
-
-        run_lengths = []
+        dump_file = base + ".dump.0"
 
-        for f in restart_filenames:
-            try:
-                pre, ext = os.path.splitext(f)
-                ext = int(ext.strip("."))
-            except ValueError:
-                raise Exception("Lammps_step: could not extract run length from %s" % f)
-            run_lengths.append(ext)
-
-            last_snapshot = str(max(run_lengths))
-
-        restart_file = restart_file.replace("*", last_snapshot)
-        dump_file = dump_file.replace("*", last_snapshot)
-        files["restart"] = {}
-        files["restart"]["filename"] = restart_file
         files["dump"] = {}
         files["dump"]["filename"] = dump_file
         files["dump"]["data"] = None
 
-        filename = os.path.join(self.directory, restart_file)
-        with open(filename, mode="rb") as fd:
-            files["restart"]["data"] = fd.read()
-
         files["input"] = {}
         files["input"]["filename"] = None
         initialization_header, eex = self._get_node_input(
             node=self._initialization_node, extras={"read_data": False}
         )
         files["input"]["data"] = copy.deepcopy(initialization_header)
 
+        # Write a small file to say that LAMMPS ran successfully, so cancel
+        # skip if rerunning.
+        path = Path(self.directory) / "success.dat"
+        path.write_text("success")
+
         return files
 
     def _prepare_input(
         self,
         files,
         nodes=None,
         iteration=0,
         read_restart=False,
         write_restart=False,
         extras=None,
     ):
+        python_script = None
+        postscript = None
         if isinstance(nodes, list) is False:
             node_ids = [nodes._id[1]]
-            new_input_data = self._get_node_input(node=nodes, extras=extras)
+            todo = self._get_node_input(node=nodes, extras=extras)
+            new_input_data = todo["script"]
+            if todo["postscript"] is not None:
+                postscript = todo["postscript"]
+            if todo["use python"] and "python script" in todo:
+                python_script = todo["python script"]
         else:
             node_ids = []
             new_input_data = []
             for n in nodes:
                 node_ids.append(n._id[1])
-                new_input_data += self._get_node_input(node=n, extras=extras)
+                todo = self._get_node_input(node=n, extras=extras)
+                new_input_data += todo["script"]
+                if todo["postscript"] is not None:
+                    postscript = todo["postscript"]
+                if todo["use python"] and "python script" in todo:
+                    python_script = todo["python script"]
 
         # base = "lammps_substep_%s_iter_%d" % ("_".join(node_ids), iteration)
         base = "lammps"
 
         input_file = base + ".dat"
-        restart = base + ".restart.*"
+        # restart = base + ".restart.*"
         dump = base + ".dump.*"
 
-        if read_restart:
-            new_input_data.insert(
-                0, "read_restart          %s" % (files["restart"]["filename"])
+        # if read_restart:
+        #     new_input_data.insert(
+        #         0, "read_restart          %s" % (files["restart"]["filename"])
+        #     )
+
+        # if write_restart:
+        #     new_input_data.append(f"write_restart          {restart}")
+
+        if postscript is None:
+            new_input_data.append("reset_timestep      0")
+            new_input_data.append("run                 0")
+            new_input_data.append(
+                f"write_dump         all custom  {dump} id xu yu zu "
+                "modify flush yes sort id"
             )
-
-        if write_restart:
-            new_input_data.append(f"write_restart          {restart}")
-
-        new_input_data.append(
-            f"write_dump all custom  {dump} id " "xu yu zu modify flush yes sort id"
-        )
+            new_input_data.append("")
+            new_input_data.append("")
+            new_input_data.append("info               computes fixes dumps log out")
 
         files["input"]["data"] += new_input_data
 
         files["input"]["filename"] = input_file
         files["input"]["data"] = "\n".join(files["input"]["data"])
         self.logger.debug(files["input"]["filename"] + ":\n" + files["input"]["data"])
 
+        if postscript is not None:
+            postscript.append("reset_timestep      0")
+            postscript.append("run                 0")
+            postscript.append(
+                f"write_dump          all custom  {dump} id xu yu zu "
+                "modify flush yes sort id"
+            )
+            postscript.append("")
+            postscript.append("info               computes fixes dumps log out")
+            files["postscript"] = {
+                "data": "\n".join(postscript),
+                "filename": "lammps_post.dat",
+            }
+        if python_script is not None:
+            files["python script"] = {
+                "data": python_script,
+                "filename": "run_lammps",
+            }
+
         return files
 
     def _get_node_input(self, node=None, extras=None):
         try:
             ret = node.get_input(extras=extras)
         except Exception as e:
             print("Error running LAMMPS flowchart: {} in {}".format(str(e), str(node)))
@@ -796,17 +972,14 @@
             raise
         return ret
 
     def structure_data(self, eex, triclinic=False):
         """Create the LAMMPS structure file from the energy expression"""
         lines = []
 
-        # The terms in the forcefield, and for each a list of forms
-        terms = eex["terms"]
-
         lines.append("Structure file for LAMMPS generated by a MolSSI flowchart")
         lines.append("{:10d} atoms".format(eex["n_atoms"]))
         lines.append("{:10d} atom types".format(eex["n_atom_types"]))
         if "n_bonds" in eex and eex["n_bonds"] > 0:
             lines.append("{:10d} bonds".format(eex["n_bonds"]))
             lines.append("{:10d} bond types".format(eex["n_bond_types"]))
         if "n_angles" in eex and eex["n_angles"] > 0:
@@ -886,60 +1059,78 @@
                     lines.append(
                         f"{i:6d} {index:6d} {q:6.3f} {x:12.7f} {y:12.7f} {z:12.7f}"
                     )
         else:
             for i, xyz_index in enumerate(eex["atoms"]):
                 x, y, z, index = xyz_index
                 lines.append(f"{i+1:6d} {index:6d} {x:12.7f} {y:12.7f} {z:12.7f}")
-        lines.append("")
 
+        lines.append("")
         lines.append("Masses")
         lines.append("")
         self._data["masses"] = []
         for i, parameters in zip(range(1, eex["n_atom_types"] + 1), eex["masses"]):
             mass, itype = parameters
             lines.append("{:6d} {} # {}".format(i, mass, itype))
             self._data["masses"].append(float(mass))
 
         # nonbonds
         if "nonbond parameters" in eex:
             lines.append("")
-            lines.append("Pair Coeffs")
+            if len(eex["nonbond parameters"]) > eex["n_atom_types"]:
+                lines.append("PairIJ Coeffs")
+            else:
+                lines.append("Pair Coeffs")
             lines.append("")
-            for i, parameters in zip(
-                range(1, eex["n_atom_types"] + 1), eex["nonbond parameters"]
-            ):
+            i = 1
+            j = 1
+            for parameters in eex["nonbond parameters"]:
                 form, values, types, parameters_type, real_types = parameters
                 if form == "nonbond(9-6)":
                     lines.append(
                         "{:6d} {} {} # {} --> {}".format(
                             i, values["eps"], values["rmin"], types[0], real_types[0]
                         )
                     )
-                else:
+                    i += 1
+                elif form == "nonbond(12-6)":
                     lines.append(
                         "{:6d} {} {} # {} --> {}".format(
                             i, values["eps"], values["sigma"], types[0], real_types[0]
                         )
                     )
-
+                    i += 1
+                elif form == "buckingham":
+                    line = "{:6d} {} {} {} {}".format(
+                        j, i, values["A"], values["rho"], values["C"]
+                    )
+                    line += (
+                        f" # {types[1]}-{types[0]} --> {real_types[1]}_{real_types[0]}"
+                    )
+                    lines.append(line)
+                    if j == i:
+                        i += 1
+                        j = 1
+                    else:
+                        j += 1
         # bonds
         if "n_bonds" in eex and eex["n_bonds"] > 0:
             lines.append("")
             lines.append("Bonds")
             lines.append("")
             for counter, tmp in zip(range(1, eex["n_bonds"] + 1), eex["bonds"]):
                 i, j, index = tmp
                 lines.append("{:6d} {:6d} {:6d} {:6d}".format(counter, index, i, j))
 
             lines.append("")
             lines.append("Bond Coeffs")
             lines.append("")
 
-            use_hybrid = len(terms["bond"]) > 1
+            forms = set([v[0] for v in eex["bond parameters"]])
+            use_hybrid = len(forms) > 1
 
             for counter, parameters in zip(
                 range(1, eex["n_bond_types"] + 1), eex["bond parameters"]
             ):
                 form, values, types, parameters_type, real_types = parameters
                 if form == "quadratic_bond":
                     function = "harmonic" if use_hybrid else ""
@@ -966,16 +1157,17 @@
                     "{:6d} {:6d} {:6d} {:6d} {:6d}".format(counter, index, i, j, k)
                 )
 
             lines.append("")
             lines.append("Angle Coeffs")
             lines.append("")
 
-            use_hybrid = len(terms["angle"]) > 1
             quartic_function = "class2" if "n_bond-bond_types" in eex else "quartic"
+            forms = set([v[0] for v in eex["angle parameters"]])
+            use_hybrid = len(forms) > 1
 
             for counter, parameters in zip(
                 range(1, eex["n_angle_types"] + 1), eex["angle parameters"]
             ):
                 form, values, types, parameters_type, real_types = parameters
                 if form == "quadratic_angle":
                     function = "harmonic" if use_hybrid else ""
@@ -1006,17 +1198,22 @@
                     range(1, eex["n_bond-bond_types"] + 1),
                     eex["bond-bond parameters"],
                     eex["angle parameters"],
                 ):
                     form, values, types, parameters_type, real_types = parameters
                     angle_form = angles[0]
                     if angle_form == "quartic_angle":
+                        function = "class2" if use_hybrid else ""
                         lines.append(
-                            "{:6d} class2 {} {} {}".format(
-                                counter, values["K"], values["R10"], values["R20"]
+                            "{:6d} {} {} {} {}".format(
+                                counter,
+                                function,
+                                values["K"],
+                                values["R10"],
+                                values["R20"],
                             )
                             + " # {}-{}-{} --> {}-{}-{}".format(
                                 types[0],
                                 types[1],
                                 types[2],
                                 real_types[0],
                                 real_types[1],
@@ -1045,17 +1242,19 @@
                     range(1, eex["n_bond-angle_types"] + 1),
                     eex["bond-angle parameters"],
                     eex["angle parameters"],
                 ):
                     form, values, types, parameters_type, real_types = parameters
                     angle_form = angles[0]
                     if angle_form == "quartic_angle":
+                        function = "class2" if use_hybrid else ""
                         lines.append(
-                            "{:6d} class2 {} {} {} {}".format(
+                            "{:6d} {} {} {} {} {}".format(
                                 counter,
+                                function,
                                 values["K12"],
                                 values["K23"],
                                 values["R10"],
                                 values["R20"],
                             )
                             + " # {}-{}-{} --> {}-{}-{}".format(
                                 types[0],
@@ -1092,15 +1291,16 @@
                     )
                 )
 
             lines.append("")
             lines.append("Dihedral Coeffs")
             lines.append("")
 
-            use_hybrid = len(terms["torsion"]) > 1
+            forms = set([v[0] for v in eex["torsion parameters"]])
+            use_hybrid = len(forms) > 1
 
             for counter, parameters in zip(
                 range(1, eex["n_torsion_types"] + 1), eex["torsion parameters"]
             ):
                 form, values, types, parameters_type, real_types = parameters
                 if form == "torsion_1":
                     KPhi = values["KPhi"]
@@ -1166,17 +1366,19 @@
                     range(1, eex["n_middle_bond-torsion_3_types"] + 1),
                     eex["middle_bond-torsion_3 parameters"],
                     eex["torsion parameters"],
                 ):
                     form, values, types, parameters_type, real_types = parameters
                     torsion_form = torsions[0]
                     if torsion_form == "torsion_3":
+                        function = "class2" if use_hybrid else ""
                         lines.append(
-                            "{:6d} class2 {} {} {} {}".format(
+                            "{:6d} {} {} {} {} {}".format(
                                 counter,
+                                function,
                                 values["V1"],
                                 values["V2"],
                                 values["V3"],
                                 values["R0"],
                             )
                             + " # {}-{}-{}-{} --> {}-{}-{}-{}".format(
                                 types[0],
@@ -1213,17 +1415,19 @@
                     range(1, eex["n_end_bond-torsion_3_types"] + 1),
                     eex["end_bond-torsion_3 parameters"],
                     eex["torsion parameters"],
                 ):
                     form, values, types, parameters_type, real_types = parameters
                     torsion_form = torsions[0]
                     if torsion_form == "torsion_3":
+                        function = "class2" if use_hybrid else ""
                         lines.append(
-                            "{:6d} class2 {} {} {} {} {} {} {} {}".format(
+                            "{:6d} {} {} {} {} {} {} {} {} {}".format(
                                 counter,
+                                function,
                                 values["V1_L"],
                                 values["V2_L"],
                                 values["V3_L"],
                                 values["V1_R"],
                                 values["V2_R"],
                                 values["V3_R"],
                                 values["R0_L"],
@@ -1264,17 +1468,19 @@
                     range(1, eex["n_angle-torsion_3_types"] + 1),
                     eex["angle-torsion_3 parameters"],
                     eex["torsion parameters"],
                 ):
                     form, values, types, parameters_type, real_types = parameters
                     torsion_form = torsions[0]
                     if torsion_form == "torsion_3":
+                        function = "class2" if use_hybrid else ""
                         lines.append(
-                            "{:6d} class2 {} {} {} {} {} {} {} {}".format(
+                            "{:6d} {} {} {} {} {} {} {} {} {}".format(
                                 counter,
+                                function,
                                 values["V1_L"],
                                 values["V2_L"],
                                 values["V3_L"],
                                 values["V1_R"],
                                 values["V2_R"],
                                 values["V3_R"],
                                 values["Theta0_L"],
@@ -1315,17 +1521,19 @@
                     range(1, eex["n_angle-angle-torsion_1_types"] + 1),
                     eex["angle-angle-torsion_1 parameters"],
                     eex["torsion parameters"],
                 ):
                     form, values, types, parameters_type, real_types = parameters
                     torsion_form = torsions[0]
                     if torsion_form == "torsion_3":
+                        function = "class2" if use_hybrid else ""
                         lines.append(
-                            "{:6d} class2 {} {} {}".format(
+                            "{:6d} {} {} {} {}".format(
                                 counter,
+                                function,
                                 values["K"],
                                 values["Theta0_L"],
                                 values["Theta0_R"],
                             )
                             + " # {}-{}-{}-{} --> {}-{}-{}-{}".format(
                                 types[0],
                                 types[1],
@@ -1361,17 +1569,22 @@
                     range(1, eex["n_bond-bond_1_3_types"] + 1),
                     eex["bond-bond_1_3 parameters"],
                     eex["torsion parameters"],
                 ):
                     form, values, types, parameters_type, real_types = parameters
                     torsion_form = torsions[0]
                     if torsion_form == "torsion_3":
+                        function = "class2" if use_hybrid else ""
                         lines.append(
-                            "{:6d} class2 {} {} {}".format(
-                                counter, values["K"], values["R10"], values["R30"]
+                            "{:6d} {} {} {} {}".format(
+                                counter,
+                                function,
+                                values["K"],
+                                values["R10"],
+                                values["R30"],
                             )
                             + " # {}-{}-{}-{} --> {}-{}-{}-{}".format(
                                 types[0],
                                 types[1],
                                 types[2],
                                 types[3],
                                 real_types[0],
@@ -1480,163 +1693,192 @@
                             real_types[1],
                             real_types[2],
                             real_types[3],
                         )
                     )
 
         lines.append("")
+        lines.append("")
         return lines
 
     def analyze(self, indent="", nodes=None, **kwargs):
         """Analyze the output of the calculation"""
         if isinstance(nodes, list) is False:
             nodes = [nodes]
 
         ret = {node._id[1]: None for node in nodes}
 
+        run_dir = Path(self.directory)
+
         for node in nodes:
             for value in node.description:
                 printer.important(value)
                 printer.important(" ")
 
-            id_str = "_".join(str(e) for e in node._id)
-
-            filenames = glob.glob(
-                os.path.join(self.directory, "*trajectory*" + id_str + "*.seamm_trj")
-            )
+            subdir = run_dir / str(node._id[-1])
 
-            if len(filenames) > 1:
-                filenames.sort(
-                    key=lambda x: int(re.search(r"iter_\d+", x).group().split("_")[1])
-                )
-
-            if len(filenames) > 0:
-                filename = filenames[-1]
-
-            P = node.parameters.current_values_to_dict(
-                context=seamm.flowchart_variables._data
-            )
-
-            node_data = None
-
-            if "run_control" in P:
-                if P["run_control"] == "For a fixed length of simulated time.":
-                    control_properties = lambda x: x not in ["tstep"]  # noqa: E731
-                    # Reset the trajectory data so doesn't carry over
-                    self._trajectory = []
-                else:
-                    if len(P["control_properties"]) == 0:
-                        raise KeyError(
-                            "No physical property selected for automatic",
-                            "equilibration detection",
-                        )
-
-                    control_properties = [prp[0] for prp in P["control_properties"]]
+            # Move any old style files
+            id_str = "_".join(str(e) for e in node._id)
+            paths = sorted(run_dir.glob(f"*trajectory*{id_str}*.seamm_trj"))
+            for path in paths:
+                ensemble = str(path).split("_")[1]
+                path.rename(subdir / f"{ensemble}_state.trj")
+
+            paths = sorted(run_dir.glob(f"*summary*{id_str}*.seamm_trj"))
+            for path in paths:
+                ensemble = str(path).split("_")[1]
+                path.rename(subdir / f"{ensemble}_summary.trj")
+
+            # Find the state trajectory, if any
+            paths = sorted(subdir.glob("*state.trj"))
+            if len(paths) > 1:
+                raise RuntimeError(f"More than one state.trj file for {id_str}.")
+            elif len(paths) == 1:
+                control_properties = lambda x: x not in ["tstep"]  # noqa: E731
+                node_data, table = self.analyze_trajectory(
+                    paths[0], control_properties=control_properties, node=node
+                )
+                # Save the state data as JSON
+                data_file = subdir / "state.json"
+                with data_file.open("w") as fd:
+                    json.dump(
+                        node_data, fd, indent=4, cls=CompactJSONEncoder, sort_keys=True
+                    )
 
-                node_data = self.analyze_trajectory(
-                    filename, control_properties=control_properties
-                )
                 # Get just the values from the node data
                 values = {k: v["mean"] for k, v in node_data.items()}
-                node.analyze(data=values)
+                # And the other key values
+                for k, v in node_data.items():
+                    for key in ("stderr", "tau", "inefficiency", "n_samples"):
+                        if key in v:
+                            values[f"{k},{key}"] = v[key]
+            else:
+                node_data = None
+                values = {}
+                table = None
+
+            node.analyze(data=values, properties=node_data, table=table)
 
             ret[node._id[1]] = node_data
 
         return ret
 
-    def analyze_trajectory(self, filename, sampling_rate=20, control_properties=None):
+    def analyze_trajectory(
+        self,
+        path,
+        sampling_rate=20,
+        control_properties=None,
+        node=None,
+    ):
         """Read a trajectory file and do the statistical analysis"""
 
         write_html = "html" in self.options and self.options["html"]
 
-        rootname = os.path.splitext(filename)[0]
-
         results = {}
 
-        if isinstance(control_properties, list) and "t" not in control_properties:
-            control_properties.append("t")
+        table = {
+            "Property": [],
+            "Value": [],
+            " ": [],
+            "StdErr": [],
+            "Units": [],
+            "convergence": [],
+            "tau": [],
+            "inefficiency": [],
+        }
 
         # Process the trajectory data
-
-        with open(filename, "r") as fd:
+        with path.open() as fd:
             file_data = pandas.read_csv(
                 fd,
                 sep=" ",
                 header=0,
                 comment="!",
                 usecols=control_properties,
                 index_col="t",
             )
             self._trajectory.append(file_data.iloc[:-1])
 
-        dt_fs = file_data.index[1] - file_data.index[0]
-        dt = dt_fs
+        dt = lammps_step.from_lammps_units(
+            file_data.index[1] - file_data.index[0], "fs"
+        )
+        dt_fs = dt.m_as("fs")
         data = pandas.concat(self._trajectory)
         data = data.reset_index(drop=True)
-        data.index *= dt
+        data.index *= dt_fs
 
         self.logger.debug("Columns: {}".format(data.columns))
         self.logger.debug("  Types:\n{}".format(data.dtypes))
 
-        printer.normal("       Analysis of " + os.path.basename(filename) + "\n")
-
-        printer.normal(
-            "                                             Std Error  "
-            "Time to\n"
-            "               Property           Value       of mean   "
-            "convergence     tau    inefficiency\n"
-            "          --------------------   ---------  ---------   "
-            "-----------  --------  ------------"
-        )
+        printer.normal(f"       Analysis of {path.name}\n")
 
         # Work out the time step, rather than give the whole vector
         t = data.index
         t_units = "fs"
         len_trj = (len(t) - 1) * dt_fs
         divisor = 1
         if len_trj >= 4000000000:
             t_units = "ms"
-            divisor = 1000000000
         elif len_trj >= 4000000:
             t_units = "ns"
-            divisor = 1000000
         elif len_trj >= 4000:
             t_units = "ps"
-            divisor = 1000
-        dt /= divisor
-        t_max = float((len(t) - 1) * dt)
+        t_max = float((len(t) - 1) * dt.m_as(t_units))
 
         for column in data.columns:
+            if "Unnamed:" in column:
+                continue
+            meta_column = column.rstrip("0123456789")
+
+            if meta_column in LAMMPS.display_title:
+                meta_title = LAMMPS.display_title[meta_column]
+            elif column in LAMMPS.display_title:
+                meta_title = LAMMPS.display_title[column]
+            else:
+                meta_title = f"unknown: {column}"
+            if meta_column in LAMMPS.display_units:
+                meta_units = LAMMPS.display_units[meta_column]
+            elif column in LAMMPS.display_units:
+                meta_units = LAMMPS.display_units[column]
+            else:
+                meta_units = "???"
+
             have_warning = False
             have_acf_warning = False
-            y = data[column]
+            # Ignore first point, t=0, cause it might not be right.
+            y = data[column][1:]
 
             self.logger.info("Analyzing {}, nsamples = {}".format(column, len(y)))
 
             # compute indices of uncorrelated timeseries using pymbar
+            # Their algorithm is quadratic in length of Y unless you
+            # use 'nskip'. I set it so there are about 100 time origins, so
+            # the convergence time is accurate to about 1%.
             yy = y.to_numpy()
-            conv, inefficiency, Neff_max = timeseries.detect_equilibration(yy)
+            nskip = yy.size // 100 + 1
+            conv, inefficiency, Neff_max = timeseries.detect_equilibration(
+                yy, nskip=nskip
+            )
 
             self.logger.info(
                 "  converged in {} steps, inefficiency = {}, Neff_max = {}".format(
                     conv, inefficiency, Neff_max
                 )
             )
 
-            if numpy.isnan(inefficiency) or numpy.isnan(Neff_max):
+            if np.isnan(inefficiency) or np.isnan(Neff_max):
                 # Apparently didn't converge!
-                printer.normal(
-                    __(
-                        "{column:>23s} did not converge to a stationary state",
-                        column=column,
-                        indent=7 * " ",
-                        wrap=False,
-                        dedent=False,
-                    )
-                )
+                table["Property"].append(column)
+                table["Value"].append("")
+                table[" "].append("")
+                table["StdErr"].append("")
+                table["Units"].append("")
+                table["convergence"].append("unconverged")
+                table["tau"].append("")
+                table["inefficiency"].append("")
 
                 have_acf = False
                 is_converged = False
             else:
                 is_converged = True
                 tau = dt_fs * (inefficiency - 1) / 2
                 if tau < dt_fs / 2:
@@ -1655,42 +1897,56 @@
                     print(y_t_equil)
                     print("indices")
                     print(indices)
                     continue
 
                 y_n = y_t_equil[indices]
                 n_samples = len(y_n)
-                mean = y_n.mean()
-                std = y_n.std()
+                mean = float(y_n.mean())
+                std = float(y_n.std())
                 sem = std / sqrt(n_samples)
 
                 # Get the autocorrelation function
                 if len(y_t_equil) < 8:
                     have_acf = False
                     have_acf_warning = True
                     acf_warning = "^"
                 else:
                     have_acf = True
-                    acf_warning = " "
+                    acf_warning = ""
                     nlags = 4 * int(round(inefficiency + 0.5))
+
                     if nlags > int(len(y_t_equil) / 2):
                         nlags = int(len(y_t_equil) / 2)
-                    acf, confidence = stattools.acf(
-                        y_t_equil,
-                        nlags=nlags,
-                        alpha=0.05,
-                        fft=nlags > 16,
-                        adjusted=False,
-                    )
+                    with warnings.catch_warnings():
+                        warnings.simplefilter("ignore", RuntimeWarning)
+                        acf, confidence = stattools.acf(
+                            y_t_equil,
+                            nlags=nlags,
+                            alpha=0.05,
+                            fft=True,
+                            adjusted=False,
+                        )
 
                 results[column] = {}
                 results[column]["mean"] = mean
-                results[column]["sem"] = sem
+                results[column]["stderr"] = sem
                 results[column]["n_sample"] = n_samples
                 results[column]["short_production"] = have_acf_warning
+                results[column]["tau"] = float(tau)
+                results[column]["inefficiency"] = float(inefficiency)
+                results[column]["timestep"] = float(dt_fs)
+                results[column]["rootname"] = path.stem
+                if have_acf:
+                    results[column]["acf"] = acf.tolist()
+                    results[column]["acf_confidence"] = confidence.tolist()
+
+                # Don't print or graph some properties, like heat flux
+                if column in ("Jx", "Jy", "Jz"):
+                    results[column]["values"] = data[column].to_numpy()
 
                 # Work out units on convergence time
                 conv_units = "fs"
                 t_conv = t0
                 if t0 >= 1000000000:
                     conv_units = "ms"
                     t_conv = t0 / 1000000000
@@ -1718,58 +1974,42 @@
                     have_warning = True
                     warn = "*"
                 else:
                     warn = " "
 
                 results[column]["few_neff"] = have_warning
 
-                printer.normal(
-                    __(
-                        "{column:>23s} = {value:9.3f} ± {stderr:7.3f}{warn}"
-                        " {t0:8.2f} {conv_units} {tau:8.1f} {tau_units}{acf} "
-                        "{inefficiency:9.1f}",
-                        column=column,
-                        value=mean,
-                        stderr=sem,
-                        warn=warn,
-                        t0=t_conv,
-                        conv_units=conv_units,
-                        tau=t_tau,
-                        tau_units=tau_units,
-                        acf=acf_warning,
-                        inefficiency=inefficiency,
-                        indent=7 * " ",
-                        wrap=False,
-                        dedent=False,
-                    )
-                )
+                table["Property"].append(f"{column}{warn}")
+                table["Value"].append(f"{mean:.3f}")
+                table[" "].append("±")
+                table["StdErr"].append(f"{sem:.3f}")
+                table["Units"].append(meta_units)
+                table["convergence"].append(f"{t_conv:.2f} {conv_units}")
+                table["tau"].append(f"{t_tau:.1f} {tau_units}{acf_warning}")
+                table["inefficiency"].append(f"{inefficiency:.1f}")
 
             # Create graphs of the property
             figure = self.create_figure(
                 module_path=(self.__module__.split(".")[0], "seamm"),
                 template="line.graph_template",
-                title=LAMMPS.display_title[column],
+                title=meta_title,
             )
 
             # The autocorrelation function
             if have_acf:
                 plot_acf = figure.add_plot("acf")
 
-                dt_acf = float(dt_fs)
                 t_acf_units = "fs"
                 len_acf = (len(acf) - 1) * dt_fs
                 if len_acf >= 2000000000:
                     t_acf_units = "ms"
-                    dt_acf /= 1000000000
                 elif len_acf >= 2000000:
                     t_acf_units = "ns"
-                    dt_acf /= 1000000
                 elif len_acf >= 2000:
                     t_acf_units = "ps"
-                    dt_acf /= 1000
 
                 x_acf_axis = plot_acf.add_axis(
                     "x", label="Time ({})".format(t_acf_units)
                 )
                 y_acf_axis = plot_acf.add_axis("y", label="acf", anchor=x_acf_axis)
                 x_acf_axis.anchor = y_acf_axis
 
@@ -1782,15 +2022,15 @@
                     fit.append(exp(-ts / tau))
 
                 plot_acf.add_trace(
                     x_axis=x_acf_axis,
                     y_axis=y_acf_axis,
                     name="fit",
                     x0=0,
-                    dx=dt_acf,
+                    dx=dt.m_as(t_acf_units),
                     xlabel="t",
                     xunits=t_acf_units,
                     y=fit,
                     ylabel="fit",
                     yunits="",
                     color="gray",
                 )
@@ -1800,74 +2040,73 @@
                 yminus = []
                 t_acf = []
                 tmp = 0.0
                 for lower, upper in confidence:
                     t_acf.append(tmp)
                     yplus.append(upper)
                     yminus.append(lower)
-                    tmp += dt_acf
+                    tmp += dt.m_as(t_acf_units)
 
                 plot_acf.add_trace(
                     x_axis=x_acf_axis,
                     y_axis=y_acf_axis,
                     name="stderr",
                     x=t_acf + t_acf[::-1],
                     xlabel="t",
                     xunits=t_acf_units,
                     y=yplus + yminus[::-1],
                     ylabel="stderr",
-                    yunits=LAMMPS.display_units[column],
-                    showlegend="false",
+                    yunits=meta_units,
                     color="rgba(211,211,211,0.5)",
                     fill="toself",
                 )
 
                 # And the acf plot last
                 plot_acf.add_trace(
                     x_axis=x_acf_axis,
                     y_axis=y_acf_axis,
                     name="acf",
                     x0=0,
-                    dx=dt_acf,
+                    dx=dt.m_as(t_acf_units),
                     xlabel="t",
                     xunits=t_acf_units,
                     y=list(acf),
                     ylabel="acf",
                     yunits="",
                     color="red",
                 )
 
             # The property data over the trajectory
             y = list(data[column])
 
             plot = figure.add_plot("trj")
 
-            ylabel = LAMMPS.display_title[column]
-            if LAMMPS.display_units[column] != "":
-                ylabel += " ({})".format(LAMMPS.display_units[column])
+            ylabel = meta_title
+            if meta_units != "":
+                ylabel += f" ({meta_units})"
 
             x_axis = plot.add_axis("x", label="Time ({})".format(t_units))
             y_axis = plot.add_axis("y", label=ylabel, anchor=x_axis)
             x_axis.anchor = y_axis
 
             # Add the trajectory, error band and median value in that order so
             # stack in a nice order.
 
             # Add the trajectory
             plot.add_trace(
                 x_axis=x_axis,
                 y_axis=y_axis,
                 name=column,
                 x0=0,
-                dx=dt,
+                dx=dt.m_as(t_units),
                 xlabel="t",
                 xunits=t_units,
                 y=list(y),
                 ylabel=column,
-                yunits=LAMMPS.display_units[column],
+                yunits=meta_units,
                 color="#4dbd74",
             )
 
             if is_converged:
                 # the partly transparent error band
                 t_min = t0 / divisor
                 plot.add_trace(
@@ -1875,65 +2114,49 @@
                     y_axis=y_axis,
                     name="sem",
                     x=[t_min, t_max, t_max, t_min],
                     xlabel="t",
                     xunits=t_units,
                     y=[mean + sem, mean + sem, mean - sem, mean - sem],
                     ylabel="sem",
-                    yunits=LAMMPS.display_units[column],
-                    showlegend="false",
+                    yunits=meta_units,
                     color="rgba(211,211,211,0.5)",
                     fill="toself",
                 )
 
                 # and finally the median value so it is on top
                 plot.add_trace(
                     x_axis=x_axis,
                     y_axis=y_axis,
                     name="average",
                     x=[t_min, t_max],
                     xlabel="t",
                     xunits=t_units,
                     y=[mean, mean],
                     ylabel="average",
-                    yunits=LAMMPS.display_units[column],
+                    yunits=meta_units,
                     color="black",
                 )
 
             if have_acf:
                 figure.grid_plots("trj - acf")
             else:
                 figure.grid_plots("trj")
-            figure.dump("{}_{}.graph".format(rootname, column))
+            if node is None:
+                path = Path(f"{path.stem}_{column}.graph")
+            else:
+                node_path = Path(node.directory)
+                node_path.mkdir(parents=True, exist_ok=True)
+                path = node_path / f"{column}.graph"
+
+            figure.dump(path)
 
             if write_html:
                 figure.template = "line.html_template"
-                figure.dump("{}_{}.html".format(rootname, column))
-
-        if have_warning or have_acf_warning:
-            printer.normal("\n")
-        if have_warning:
-            printer.normal(
-                __(
-                    "          * this property has less than 100 independent "
-                    "samples, so may not be accurate.",
-                    wrap=False,
-                    dedent=False,
-                )
-            )
-
-        if have_acf_warning:
-            printer.normal(
-                __(
-                    "          ^ there are not enough samples after "
-                    "equilibration to plot the ACF.",
-                    wrap=False,
-                    dedent=False,
-                )
-            )
+                figure.dump(path.with_suffix(".html"))
 
         # Add citations for pymbar
         self.references.cite(
             raw=self._bibliography["mbar"],
             alias="pymbar-1",
             module="lammps_step",
             level=1,
@@ -1950,15 +2173,15 @@
             raw=self._bibliography["convergence"],
             alias="pymbar-3",
             module="lammps_step",
             level=2,
             note="The third citation for pymbar",
         )
 
-        return results
+        return results, table
 
     def shake_fix(self, P, eex):
         """Create the 'fix shake' line needed for handling waters and X-H.
 
         Parameters
         ----------
         P : dict
```

### Comparing `lammps_step-2023.4.9/lammps_step/lammps_step.py` & `lammps_step-2023.5.29/lammps_step/lammps_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/lammps_step/lammps_units.py` & `lammps_step-2023.5.29/lammps_step/lammps_units.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
     """Set the default unit system for LAMMPS."""
     global lammps_unit_system
     if value not in unit_systems:
         raise ValueError(f"unit system '{value}' not recognized!")
     lammps_unit_system = value
 
 
-def get_lammps_unit_system(value):
+def get_lammps_unit_system():
     """Get the default unit system for LAMMPS."""
     global lammps_unit_system
     return lammps_unit_system
 
 
 def to_lammps_units(value, units=None, quantity=None, unit_system=None):
     """Convert the value with units to the current LAMMPS units."""
```

### Comparing `lammps_step-2023.4.9/lammps_step/metadata.py` & `lammps_step-2023.5.29/lammps_step/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     },
     "density,stderr": {
         "calculation": ["npt"],
         "description": "stderr of density",
         "dimensionality": "scalar",
         "property": "density, stderr#LAMMPS#{model}",
         "type": "float",
-        "units": "K",
+        "units": "g/ml",
     },
     "density,tau": {
         "calculation": ["npt"],
         "description": "autocorrelation time of density",
         "dimensionality": "scalar",
         "property": "density, tau#LAMMPS#{model}",
         "type": "float",
@@ -146,15 +146,15 @@
     },
     "a,stderr": {
         "calculation": ["npt"],
         "description": "stderr of cell 'a'",
         "dimensionality": "scalar",
         "property": "cell_a, stderr#LAMMPS#{model}",
         "type": "float",
-        "units": "K",
+        "units": "Å",
     },
     "a,tau": {
         "calculation": ["npt"],
         "description": "autocorrelation time of cell 'a'",
         "dimensionality": "scalar",
         "property": "cell_a, tau#LAMMPS#{model}",
         "type": "float",
@@ -178,15 +178,15 @@
     },
     "b,stderr": {
         "calculation": ["npt"],
         "description": "stderr of cell 'b'",
         "dimensionality": "scalar",
         "property": "cell_b, stderr#LAMMPS#{model}",
         "type": "float",
-        "units": "K",
+        "units": "Å",
     },
     "b,tau": {
         "calculation": ["npt"],
         "description": "autocorrelation time of cell 'b'",
         "dimensionality": "scalar",
         "property": "cell_b, tau#LAMMPS#{model}",
         "type": "float",
@@ -210,15 +210,15 @@
     },
     "c,stderr": {
         "calculation": ["npt"],
         "description": "stderr of cell 'c'",
         "dimensionality": "scalar",
         "property": "cell_c, stderr#LAMMPS#{model}",
         "type": "float",
-        "units": "K",
+        "units": "Å",
     },
     "c,tau": {
         "calculation": ["npt"],
         "description": "autocorrelation time of cell 'c'",
         "dimensionality": "scalar",
         "property": "cell_c, tau#LAMMPS#{model}",
         "type": "float",
@@ -250,15 +250,15 @@
             "nvt",
             "npt",
         ],
         "description": "stderr of total energy",
         "dimensionality": "scalar",
         "property": "total energy, stderr#LAMMPS#{model}",
         "type": "float",
-        "units": "K",
+        "units": "kcal/mol",
     },
     "Etot,tau": {
         "calculation": [
             "nve",
             "nvt",
             "npt",
         ],
@@ -298,15 +298,15 @@
             "nvt",
             "npt",
         ],
         "description": "stderr of kinetic energy",
         "dimensionality": "scalar",
         "property": "kinetic energy, stderr#LAMMPS#{model}",
         "type": "float",
-        "units": "K",
+        "units": "kcal/mol",
     },
     "Eke,tau": {
         "calculation": [
             "nve",
             "nvt",
             "npt",
         ],
@@ -346,15 +346,15 @@
             "nvt",
             "npt",
         ],
         "description": "stderr of potential energy",
         "dimensionality": "scalar",
         "property": "potential energy, stderr#LAMMPS#{model}",
         "type": "float",
-        "units": "K",
+        "units": "kcal/mol",
     },
     "Epe,tau": {
         "calculation": [
             "nve",
             "nvt",
             "npt",
         ],
@@ -392,15 +392,15 @@
             "nve",
             "nvt",
             "npt",
         ],
         "description": "stderr of nonbond energy",
         "dimensionality": "scalar",
         "type": "float",
-        "units": "K",
+        "units": "kcal/mol",
     },
     "Epair,tau": {
         "calculation": [
             "nve",
             "nvt",
             "npt",
         ],
```

### Comparing `lammps_step-2023.4.9/lammps_step/minimization.py` & `lammps_step-2023.5.29/lammps_step/minimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,8 +136,12 @@
         lines.append("")
         lines.append("thermo_style        custom {}".format(thermo_properties))
         lines.append("thermo              {}".format(100))
         lines.append(
             "minimize            {} {} {} {}".format(etol, ftol, maxiters, maxevals)
         )
 
-        return lines
+        return {
+            "script": lines,
+            "postscript": None,
+            "use python": False,
+        }
```

### Comparing `lammps_step-2023.4.9/lammps_step/minimization_step.py` & `lammps_step-2023.5.29/lammps_step/minimization_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/lammps_step/npt.py` & `lammps_step-2023.5.29/lammps_step/npt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # -*- coding: utf-8 -*-
 
 """NPT (canonical) dynamics in LAMMPS"""
 
+import json
+
 import lammps_step
 import logging
 import seamm
-from seamm_util import units_class
+from seamm_util import units_class, Q_
 import seamm_util.printing as printing
 from seamm_util.printing import FormattedText as __
 import random
 
 logger = logging.getLogger(__name__)
 job = printing.getPrinter()
 printer = printing.getPrinter("lammps")
@@ -178,29 +180,31 @@
         ptext = self.get_pressure_text(P, keep_orthorhombic)
 
         thermo_properties = (
             "time temp press etotal ke pe ebond "
             "eangle edihed eimp evdwl etail ecoul elong"
         )
         properties = (
-            "v_time v_temp v_press v_density v_cella v_cellb "
+            "v_time v_temp v_press v_vol v_density v_cella v_cellb "
             "v_cellc v_etotal v_ke v_pe v_epair"
         )
-        title2 = "tstep t T P density a b c Etot Eke Epe Epair"
+        title2 = "tstep t T P V density a b c Etot Eke Epe Epair"
 
         # and build the LAMMPS script
         lines = []
         lines.append("")
         lines.append("#     NPT dynamics")
         lines.append("")
         lines.append("reset_timestep      0")
         lines.append("timestep            {}".format(timestep))
         lines.append("thermo_style        custom {}".format(thermo_properties))
         lines.append("thermo              {}".format(int(nsteps / 100)))
 
+        ncomputes = 0
+        ndumps = 0
         nfixes = 0
         if P["thermostat"] == "Nose-Hoover":
             Tchain = P["Tchain"]
             Tloop = P["Tloop"]
             drag = P["drag"]
             if barostat == "Nose-Hoover":
                 nfixes += 1
@@ -273,15 +277,15 @@
                 + "all temp/csld "
                 + " {} {} {} {}".format(T0, T1, Tdamp, seed)
             )
             nfixes += 1
             lines.append("fix                 {} ".format(nfixes) + "all nve")
         elif P["thermostat"] == "velocity rescaling":
             frequency = P["frequency"]
-            nevery = round(nsteps / (frequency / timestep))
+            nevery = max(1, round(nsteps / (frequency / timestep)))
             window = lammps_step.to_lammps_units(P["window"], quantity="temperature")
             fraction = P["fraction"]
             nfixes += 1
             lines.append(
                 "fix                 {} ".format(nfixes)
                 + "all temp/rescale "
                 + "{} {} {} {} {}".format(nevery, T0, T1, window, fraction)
@@ -310,96 +314,141 @@
                 raw=self._bibliography[citation],
                 alias=citation,
                 module="lammps_step",
                 level=1,
                 note="Citation for thermostat.",
             )
 
+        # For the heat flux, if requested, we need extra input
+        if P["heat flux"] != "never":
+            # Unit conversion factor
+            if lammps_step.get_lammps_unit_system() == "metal":
+                factor = Q_("eV/Å^2/ps")
+            else:
+                factor = (
+                    Q_("kcal/Å^2/fs/mol") / Q_("kcal/mol") * Q_("kcal/mol").to("kJ")
+                )
+            factor = factor.m_as("W/m^2")
+            lines.append(
+                f"""
+compute             KE all ke/atom
+compute             PE all pe/atom
+
+#          centroid doesn't work with kspace, so split into pair and non-pair parts
+
+compute             S_p all stress/atom NULL pair kspace
+compute             S_b all centroid/stress/atom NULL bond angle dihedral improper
+compute             flux_p all heat/flux KE PE S_p
+compute             flux_b all heat/flux KE PE S_b
+
+#          Conversion from kcal/Å^2/fs/mol to W/m^2")
+
+variable            factor equal {factor}
+variable            Jx equal v_factor*(c_flux_p[1]+c_flux_b[1])/vol
+variable            Jy equal v_factor*(c_flux_p[2]+c_flux_b[2])/vol
+variable            Jz equal v_factor*(c_flux_p[3]+c_flux_b[3])/vol
+"""
+            )
+
         # summary output written 10 times during run so we can see progress
         nevery = 10
         nfreq = int(nsteps / 10)
         nrepeat = int(nfreq / nevery)
         nfreq = nevery * nrepeat
         nfixes += 1
+        filename = f"@{self._id[-1]}+npt_summary.trj"
         lines.append(
-            "fix                 {} ".format(nfixes)
-            + "all ave/time "
-            + "{} {} {} {} off 2 title2 '{}' file summary_npt_{}.txt".format(
-                nevery,
-                nrepeat,
-                nfreq,
-                properties,
-                title2,
-                "_".join(str(e) for e in self._id),
-            )
+            f"fix                 {nfixes} all ave/time {nevery} 1 {nfreq} &\n"
+            f"                       {properties} &\n"
+            "                       off 2 &\n"
+            f"                       file {filename}"
         )
         # instantaneous output written for averaging
         if P["sampling"] == "none":
             self.description.append(
                 __(
                     "The run will be {nsteps:n} steps of dynamics.",
                     nsteps=nsteps,
                     indent=3 * " ",
                 )
             )
         else:
             sampling = lammps_step.to_lammps_units(P["sampling"], quantity="time")
-            nevery = round(sampling / timestep)
+            nevery = max(1, round(sampling / timestep))
             nfreq = int(nsteps / nevery)
             nrepeat = 1
             nfreq = nevery * nrepeat
             nfixes += 1
+            dt = (nevery * P["timestep"]).to_compact()
+            P0tmp = P["Pinitial"].to_compact()
+            P1tmp = P["Pfinal"].to(P0tmp.units)
+            tmp = {
+                "code": "LAMMPS",
+                "type": "NPT",
+                "dt": dt.magnitude,
+                "tunits": str(dt.u),
+                "nsteps": nsteps // nevery,
+                "Tunits": "K",
+                "Punits": str(P0tmp.u),
+            }
+            if P0tmp == P1tmp:
+                tmp["P"] = P0tmp.magnitude
+            else:
+                tmp["P0"] = P0tmp.magnitude
+                tmp["T1"] = P1tmp.magnitude
             if T0 == T1:
-                title1 = (
-                    "!MolSSI trajectory 1.0 LAMMPS, NPT {} steps of {} fs, " "T={} K"
-                ).format(int(nsteps / nevery), timestep * nevery, T0)
+                tmp["T"] = T0
             else:
-                title1 = (
-                    "!MolSSI trajectory 1.0 LAMMPS, NPT {} steps of {} fs, " "T={}-{} K"
-                ).format(int(nsteps / nevery), timestep * nevery, T0, T1)
+                tmp["T0"] = T0
+                tmp["T1"] = T1
+            title1 = "!MolSSI trajectory 2.0 " + json.dumps(tmp, separators=(",", ":"))
+            filename = f"@{self._id[-1]}+npt_state.trj"
             lines.append(
-                (
-                    "fix                 {} all ave/time {} {} {} {} off 2 "
-                    "title1 '{}' title2 '{}' file trajectory_npt_{}.seamm_trj"
-                ).format(
-                    nfixes,
-                    nevery,
-                    nrepeat,
-                    nfreq,
-                    properties,
-                    title1,
-                    title2,
-                    "_".join(str(e) for e in self._id),
-                )
+                f"fix                 {nfixes} all ave/time {nevery} 1 {nfreq} &\n"
+                f"                       {properties} &\n"
+                "                       off 2 &\n"
+                f"                       title1 '{title1}' &\n"
+                f"                       title2 '{title2}' &\n"
+                f"                       file {filename}"
             )
             self.description.append(
                 __(
                     (
                         "The run will be {nsteps:,d} steps of dynamics "
                         "sampled every {nevery:n} steps."
                     ),
                     nsteps=nsteps,
                     nevery=nevery,
                     indent=7 * " ",
                 )
             )
 
+        # Handle trajectories
+        tmp, ncomputes, ndumps, nfixes = self.trajectory_input(
+            P, timestep, nsteps, ncomputes, ndumps, nfixes
+        )
+        lines.extend(tmp)
+
         if extras is not None and "shake" in extras:
             nfixes += 1
             lines.append(extras["shake"].format(nfixes))
 
         lines.append("")
         lines.append("run                 {}".format(nsteps))
         lines.append("")
 
         for fix in range(1, nfixes + 1):
             lines.append("unfix               {}".format(fix))
         lines.append("")
 
-        return lines
+        return {
+            "script": lines,
+            "postscript": None,
+            "use python": False,
+        }
 
     def get_pressure_text(self, P, keep_orthorhombic):
         """Work out and return the pressure/stress part of the
         'fix npt' or 'fix berendsen' in LAMMPS
         """
         system_type = P["system type"]
         Panneal = P["Panneal"]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lammps_step-2023.4.9/lammps_step/npt_parameters.py` & `lammps_step-2023.5.29/lammps_step/npt_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/lammps_step/npt_step.py` & `lammps_step-2023.5.29/lammps_step/npt_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/lammps_step/nve_parameters.py` & `lammps_step-2023.5.29/lammps_step/nvt_parameters.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,104 +1,137 @@
 # -*- coding: utf-8 -*-
-"""Control parameters for NVE (microcanonical) dynamics"""
+
+"""Control parameters for NVT (canonical) dynamics"""
 
 import lammps_step
 import logging
 
 logger = logging.getLogger(__name__)
 
 
-class NVE_Parameters(lammps_step.EnergyParameters):
-    """The control parameters for NVE dynamics in LAMMPS"""
+class NVT_Parameters(lammps_step.NVE_Parameters):
+    """The control parameters for NVT dynamics in LAMMPS"""
 
     parameters = {
-        "run_control": {
-            "default": "For a fixed length of simulated time.",
-            "kind": "enumeration",
-            "default_units": None,
-            "format_string": "",
+        "thermostat": {
+            "default": "Nose-Hoover",
+            "kind": "string",
+            "format_string": "s",
             "enumeration": (
-                "Until properties converge to the requested accuracy.",
-                "For a fixed length of simulated time.",
+                "Nose-Hoover",
+                "Berendsen",
+                "canonical sampling, velocity rescaling (csvr)",
+                "canonical sampling, langevin dynamics (csld)",
+                "velocity rescaling",
+                "Langevin",
             ),
-            "description": "How long to run? ",
+            "description": "Thermostat:",
+            "help_text": ("The thermostat used to control the " "temperature."),
+        },
+        "T0": {
+            "default": 298.15,
+            "kind": "float",
+            "default_units": "K",
+            "format_string": ".2f",
+            "description": "Temperature:",
             "help_text": (
-                "How to determine when to stop the simulation. "
-                "You can give a fixed length of simulation time, "
-                "e.g. 15 ps, or you can ask to run long enough to "
-                "determine one or more properties to a given "
-                "accuracy."
+                "The temperature, or initial temperature for " "simulated annealing."
             ),
         },
-        "time": {
-            "default": 100.0,
+        "T1": {
+            "default": 298.15,
             "kind": "float",
-            "default_units": "ps",
-            "format_string": ".1f",
-            "description": "Simulation time:",
-            "help_text": ("The time to simulate in the dynamics run."),
+            "default_units": "K",
+            "format_string": ".2f",
+            "description": "Final temperature:",
+            "help_text": "The final temperature for simulated annealing.",
         },
-        "maximum_time": {
-            "default": 1.0,
+        "Tdamp": {
+            "default": 100.0,
             "kind": "float",
-            "default_units": "ns",
+            "default_units": "fs",
             "format_string": ".1f",
-            "description": "Maximum simulation time:",
-            "help_text": ("The maximum time to simulate when converging properties."),
+            "description": "Damping time:",
+            "help_text": "The damping time constant for thermostat",
         },
-        "timestep": {
-            "default": "normal",
+        "Tchain": {
+            "default": 3,
+            "kind": "integer",
+            "default_units": None,
+            "format_string": "d",
+            "description": "Thermostat chain:",
+            "help_text": "The number of thermostats in the chain.",
+        },
+        "Tloop": {
+            "default": 1,
+            "kind": "integer",
+            "default_units": None,
+            "format_string": "d",
+            "description": "Thermostat iterations:",
+            "help_text": ("The number of sub-iterations for the thermostat."),
+        },
+        "drag": {
+            "default": 0.0,
             "kind": "float",
-            "default_units": "fs",
-            "enumeration": ("normal", "accurate but slow", "coarse but fast"),
+            "default_units": None,
             "format_string": ".1f",
-            "description": "Timestep:",
+            "description": "Drag:",
             "help_text": (
-                "The time step for the numerical integration in "
-                "the dynamics. 1 fs is safe for most systems, "
-                "except perhaps at high temperatures. For systems "
-                "without hydrogen, helium, lithium or other light "
-                "elements, 2-4 fs steps are reasonable. The "
-                "timestep needs to be less than 1/10 the highest "
-                "frequency. 10^14 Hz is a period if 10 fs, and "
-                "corresponds to a frequency of 3,300 wavenumbers or "
-                "a wavelength of 3 micrometers.\n"
-                "You can enter a value or use the choices, which pick a "
-                "reasonable timestep based on the calculation."
-            ),
-        },
-        "control_properties": {
-            "default": {},
-            "kind": "special",
-            "widget": "seamm_widgets.PropertyTable",
+                "The amount of drag to apply on the thermostat "
+                "and barostat if the pressure is controlled. "
+                "Typically a value of 0.2 - 2.0 is appropriate."
+            ),
+        },
+        "seed": {
+            "default": "random",
+            "kind": "integer",
             "default_units": None,
-            "enumeration": tuple(),
             "format_string": "",
-            "description": "Convergence properties",
+            "enumeration": ("random",),
+            "description": "Random seed:",
             "help_text": (
-                "The properties to converge when controlling the run " "automatically."
+                "The seed for the random number generator."
+                "'random' means to generate a random integer "
+                "as the seed."
             ),
         },
-        "sampling": {
-            "default": "50",
+        "frequency": {
+            "default": 100.0,
             "kind": "float",
             "default_units": "fs",
-            "enumeration": ("none",),
             "format_string": ".1f",
-            "description": "Sampling frequency:",
+            "description": "Rescaling frequency:",
+            "help_text": (
+                "The frequency (in time units) for the thermostat " "to operate."
+            ),
+        },
+        "window": {
+            "default": 20.0,
+            "kind": "float",
+            "default_units": "K",
+            "format_string": ".1f",
+            "description": "Temperature window:",
+            "help_text": (
+                "The temperature window to use when rescaling."
+                "When the instantaneous temperature is outside "
+                "the temperature window, the velocities will be "
+                "rescaled."
+            ),
+        },
+        "fraction": {
+            "default": 1.0,
+            "kind": "float",
+            "default_units": None,
+            "format_string": ".1f",
+            "description": "Fraction to scale:",
             "help_text": (
-                "How often to sample the energy, temperature, "
-                "etc. during the dynamics run. This controls "
-                "writing to the trajectory files. Faster gives "
-                "more fidelity to a point, but increases the "
-                "file size and slows the calculation down."
-                "\nYou can ask for no sampling, give a specific interval, "
-                "or allow the system the choose for you."
+                "The fraction of the temperature difference "
+                "to correct by scaling the velocities."
             ),
         },
     }
 
     def __init__(self, defaults={}, data=None):
         """Initialize the instance, by default from the default
         parameters given in the class"""
 
-        super().__init__(defaults={**NVE_Parameters.parameters, **defaults}, data=data)
+        super().__init__(defaults={**NVT_Parameters.parameters, **defaults}, data=data)
```

### Comparing `lammps_step-2023.4.9/lammps_step/nve_step.py` & `lammps_step-2023.5.29/lammps_step/nve_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/lammps_step/nvt_step.py` & `lammps_step-2023.5.29/lammps_step/nvt_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/lammps_step/tk_custom.py` & `lammps_step-2023.5.29/lammps_step/tk_custom.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/lammps_step/tk_energy.py` & `lammps_step-2023.5.29/lammps_step/tk_energy.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,19 @@
         self.popup_menu.add_command(label="Edit..", command=self.edit)
 
         self.popup_menu.tk_popup(event.x_root, event.y_root, 0)
 
     def create_dialog(self, title="Edit LAMMPS Energy Step"):
         """Create the dialog!"""
 
-        super().create_dialog(title=title)
+        frame = super().create_dialog(title=title)
 
         self["message"] = ttk.Label(
             self["frame"],
             text="The LAMMPS energy step has no parameters\n"
             "All relevant parameters are set in the initialization step.",
         )
         self["message"].grid()
 
         self.setup_results()
+
+        return frame
```

### Comparing `lammps_step-2023.4.9/lammps_step/tk_initialization.py` & `lammps_step-2023.5.29/lammps_step/tk_initialization.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/lammps_step/tk_lammps.py` & `lammps_step-2023.5.29/lammps_step/tk_lammps.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/lammps_step/tk_minimization.py` & `lammps_step-2023.5.29/lammps_step/tk_minimization.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/lammps_step/tk_npt.py` & `lammps_step-2023.5.29/lammps_step/tk_npt.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,40 +151,44 @@
         self["barostat"].grid(row=row, column=0, sticky=tk.W)
         row += 1
 
         self["Panneal"].grid(row=row, column=0, sticky=tk.W)
         row += 1
 
         if system_type == "fluid":
-            sw.align_labels((self["system type"], self["barostat"], self["Panneal"]))
+            sw.align_labels(
+                (self["system type"], self["barostat"], self["Panneal"]),
+                sticky=tk.E,
+            )
         else:
             self["use_stress"].grid(row=row, column=0, sticky=tk.W)
             row += 1
 
             self["couple"].grid(row=row, column=0, sticky=tk.W)
             row += 1
 
             sw.align_labels(
                 (
                     self["system type"],
                     self["barostat"],
                     self["Panneal"],
                     self["use_stress"],
                     self["couple"],
-                )
+                ),
+                sticky=tk.E,
             )
 
         self["stress_frame"].grid(row=row, column=0, sticky=tk.W)
         row += 1
 
         if barostat == "Nose-Hoover":
             self["nreset"].grid(row=row, column=0, sticky=tk.W)
             row += 1
             self["mtk"].grid(row=row, column=0, sticky=tk.W)
-            sw.align_labels((self["nreset"], self["mtk"]))
+            sw.align_labels((self["nreset"], self["mtk"]), sticky=tk.E)
         else:
             self["modulus"].grid(row=row, column=0, sticky=tk.W)
 
         # and lay out the pressure or stress terms
         self.reset_stress_frame()
 
     def reset_stress_frame(self, widget=None):
@@ -718,15 +722,15 @@
                 widgets.append(self["Pfinal"])
                 row += 1
 
             if barostat == "Nose-Hoover":
                 self["Pdamp"].grid(row=row, column=0, sticky=tk.W)
                 widgets.append(self["Pdamp"])
                 row += 1
-            sw.align_labels(widgets)
+            sw.align_labels(widgets, sticky=tk.E)
 
     def handle_dialog(self, result):
         """Handle when the user clicks a button on the dialog,
         which can either be 'Cancel', 'Help' or 'OK', or they can
         close the dialog with the 'x' button == 'Cancel'"""
 
         if result == "OK":
```

### Comparing `lammps_step-2023.4.9/lammps_step/tk_nve.py` & `lammps_step-2023.5.29/lammps_step/tk_nve.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,19 +42,41 @@
             my_logger=my_logger,
         )
 
     def create_dialog(self, title="Edit NVE dynamics parameters"):
         """Create the dialog!"""
 
         # Let parent classes do their thing.
-        super().create_dialog(title=title)
+        frame = super().create_dialog(title=title)
 
         # Shortcut for parameters
         P = self.node.parameters
 
+        # Add a tab for the trajectory setup
+        notebook = self["notebook"]
+        tframe = ttk.Frame(notebook)
+        self["trajectory frame"] = tframe
+        notebook.insert(
+            self["results frame"], tframe, text="Trajectories", sticky=tk.NSEW
+        )
+
+        row = 0
+        widgets = []
+        for key in lammps_step.NVE_Parameters.trajectories:
+            if title == "Heat Flux" and key == "heat flux":
+                continue
+            self[key] = P[key].widget(tframe)
+            self[key].grid(row=row, column=0)
+            row += 1
+            widgets.append(self[key])
+        sw.align_labels(widgets, sticky=tk.E)
+
+        if title == "Heat Flux":
+            return frame
+
         # Frame to isolate widgets
         c_frame = self["control_frame"] = ttk.LabelFrame(
             self["frame"],
             borderwidth=4,
             relief="sunken",
             text="General Parameters",
             labelanchor="n",
@@ -71,14 +93,16 @@
         self["run_control"].combobox.configure(width=40)
 
         # and binding to change as needed
         self["run_control"].combobox.bind(
             "<<ComboboxSelected>>", self.reset_control_frame
         )
 
+        return frame
+
     def reset_dialog(self, widget=None):
         """Layout the widgets as needed for the current state"""
 
         frame = self["frame"]
         # Clear the dialog
         for slave in frame.grid_slaves():
             slave.grid_forget()
@@ -124,15 +148,15 @@
             widgets.append(self["sampling"])
             self["sampling"].grid(row=row, column=0, sticky=tk.W)
             row += 1
         else:
             self["control_properties"].grid(row=row, column=0, sticky=tk.NSEW)
             row += 1
 
-        sw.align_labels(widgets)
+        sw.align_labels(widgets, sticky=tk.E)
 
     def handle_dialog(self, result):
         if result == "OK":
             # Shortcut for parameters
             P = self.node.parameters
 
             value, units = self["time"].get()
```

### Comparing `lammps_step-2023.4.9/lammps_step/tk_nvt.py` & `lammps_step-2023.5.29/lammps_step/tk_nvt.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
         self["T1"].grid(row=row, column=0, columnspan=2, sticky=tk.W)
         row += 1
 
         self["thermostat"].grid(row=row, column=0, columnspan=2, sticky=tk.W)
         row += 1
 
-        sw.align_labels((self["T0"], self["T1"], self["thermostat"]))
+        sw.align_labels((self["T0"], self["T1"], self["thermostat"]), sticky=tk.E)
 
         # and controls for specific thermostats
         if thermostat != "velocity rescaling":
             self["Tdamp"].grid(row=row, column=1, sticky=tk.W)
             row += 1
 
         if thermostat == "Nose-Hoover":
@@ -144,15 +144,16 @@
             self["Tchain"].grid(row=row, column=1, sticky=tk.W)
             row += 1
 
             self["Tloop"].grid(row=row, column=1, sticky=tk.W)
             row += 1
 
             sw.align_labels(
-                (self["Tdamp"], self["Tchain"], self["Tloop"], self["drag"])
+                (self["Tdamp"], self["Tchain"], self["Tloop"], self["drag"]),
+                sticky=tk.E,
             )
         elif thermostat == "Berendsen":
             pass
         elif "csvr" in thermostat or "csld" in thermostat:
             self["seed"].grid(row=row, column=1, sticky=tk.W)
             row += 1
         elif thermostat == "velocity rescaling":
@@ -161,19 +162,21 @@
 
             self["window"].grid(row=row, column=1, sticky=tk.W)
             row += 1
 
             self["fraction"].grid(row=row, column=1, sticky=tk.W)
             row += 1
 
-            sw.align_labels((self["frequency"], self["window"], self["fraction"]))
+            sw.align_labels(
+                (self["frequency"], self["window"], self["fraction"]), sticky=tk.E
+            )
         elif thermostat == "Langevin":
             self["seed"].grid(row=row, column=1, sticky=tk.W)
             row += 1
-            sw.align_labels((self["Tdamp"], self["seed"]))
+            sw.align_labels((self["Tdamp"], self["seed"]), sticky=tk.E)
         else:
             raise RuntimeError(
                 "Don't recognize thermostat " + "'{}'".format(thermostat)
             )
 
         t_frame.columnconfigure(0, minsize=50)
```

### Comparing `lammps_step-2023.4.9/lammps_step/tk_velocities.py` & `lammps_step-2023.5.29/lammps_step/tk_velocities.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,8 +60,8 @@
             row += 1
 
         if "scaling" in method:
             self["seed"].grid(row=row, column=0, sticky=tk.EW)
             widgets.append(self["seed"])
             row += 1
 
-            sw.align_labels(widgets)
+            sw.align_labels(widgets, sticky=tk.E)
```

### Comparing `lammps_step-2023.4.9/lammps_step/velocities.py` & `lammps_step-2023.5.29/lammps_step/velocities.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,19 +67,19 @@
         if P["remove_momentum"][0] == "$":
             text += (
                 " Whether to remove translational or rotational "
                 "momentum will be determined at runtime by "
                 "'{remove_momentum}'"
             )
         else:
-            text += " LAMMPS will {remove_momentum}."
+            text += " LAMMPS will {remove_momentum}"
 
         if P["method"] != "scaling current velocities":
             if P["seed"] == "random":
-                text += " The random number generator will be initialized " "randomly."
+                text += " The random number generator will be initialized randomly."
             else:
                 text += (
                     " The random number generator will be initialized "
                     "with the seed '{seed}'."
                 )
 
         return self.header + "\n" + __(text, **P, indent=4 * " ").__str__()
@@ -114,31 +114,27 @@
 
         # Get the input lines
         lines = []
         lines.append("")
         lines.append("#     velocities")
         lines.append("")
 
-        if P["remove_momentum"] == (
-            "remove translational but not " "rotational momentum"
-        ):
+        if P["remove_momentum"] == "remove translational but not rotational momentum":
             remove_translations = "yes"
             remove_rotations = "no"
-        elif P["remove_momentum"] == (
-            "remove rotational but not " "translational momentum"
-        ):
+        elif P["remove_momentum"] == "remove rotational but not translational momentum":
             remove_translations = "no"
             remove_rotations = "yes"
         elif P["remove_momentum"] == (
-            "remove both translational and " "rotational momentum"
+            "remove both translational and rotational momentum"
         ):
             remove_translations = "yes"
             remove_rotations = "yes"
         elif P["remove_momentum"] == (
-            "remove neither translational nor " "rotational momentum"
+            "remove neither translational nor rotational momentum"
         ):
             remove_translations = "no"
             remove_rotations = "no"
         else:
             raise RuntimeError(
                 "Don't recognize 'remove_momentum' of '{}'".format(P["remove_momentum"])
             )
@@ -158,8 +154,12 @@
                 )
             )
         else:
             raise RuntimeError(
                 "Velocity method '{}' not supported yet".format(P["method"])
             )
 
-        return lines
+        return {
+            "script": lines,
+            "postscript": None,
+            "use python": False,
+        }
```

### Comparing `lammps_step-2023.4.9/lammps_step/velocities_parameters.py` & `lammps_step-2023.5.29/lammps_step/velocities_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/lammps_step/velocities_step.py` & `lammps_step-2023.5.29/lammps_step/velocities_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/lammps_step.egg-info/PKG-INFO` & `lammps_step-2023.5.29/lammps_step.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lammps-step
-Version: 2023.4.9
+Version: 2023.5.29
 Summary: A SEAMM plug-in for LAMMPS, a forcefield-based molecular dynamics code.
 Home-page: https://github.com/molssi-seamm/lammps_step
 Author: MolSSI @ Virginia Tech
 Author-email: seamm@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,forcefield,EAM,OpenKIM,molecular dynamics,atomistic,MD
 Platform: Linux
@@ -109,14 +109,31 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2023.5.29 -- Self diffusion and other improvements
+   * Added trajectory panel to support diffusion, viscosity and simple thermal
+     conductivity.
+   * Added support for separate GPU versions of LAMMPS.
+   * Added support for command-line arguments to LAMMPS, mainly used for accelerators.
+   * Added support for using modules.
+
+2023.4.24 -- Support for thermal conductivity
+   * Internal changes to support thermal conductivity with its embedded flowchart.
+   * Added the heat flux substep.
+   * Now delete output and reference files when rerunning, so the output is clean.
+   * Internal changes to support running LAMMPS from a Python driver.
+   * Corrected units of properties returned from LAMMPS when e.g. metal units used.
+   * Added support for Buckingham potentials
+   * Fixed issues with and cleaned up the use of hybrid types for bonds, angles, ....
+   * Fixed issues with the alignment of some of the widgets in the GUI.
+     
 2023.4.9 -- Hid the warning from pymbar
    * Importing pymbar timeseries writes a warning to the terminal about its proper
      usage. SEAMM already handles the warned case, so the message is simply confusing to
      users and hence this release hides it.
      
 2023.4.6 -- Better forcefield handling.
    * Added correct molecule numbers for valence forcefields.
```

### Comparing `lammps_step-2023.4.9/lammps_step.egg-info/SOURCES.txt` & `lammps_step-2023.5.29/lammps_step.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 lammps_step/_version.py
 lammps_step/custom.py
 lammps_step/custom_parameters.py
 lammps_step/custom_step.py
 lammps_step/energy.py
 lammps_step/energy_parameters.py
 lammps_step/energy_step.py
+lammps_step/heat_flux.py
+lammps_step/heat_flux_parameters.py
+lammps_step/heat_flux_step.py
 lammps_step/initialization.py
 lammps_step/initialization_parameters.py
 lammps_step/initialization_step.py
 lammps_step/installer.py
 lammps_step/lammps.py
 lammps_step/lammps_step.py
 lammps_step/lammps_units.py
@@ -62,14 +65,15 @@
 lammps_step/nve_parameters.py
 lammps_step/nve_step.py
 lammps_step/nvt.py
 lammps_step/nvt_parameters.py
 lammps_step/nvt_step.py
 lammps_step/tk_custom.py
 lammps_step/tk_energy.py
+lammps_step/tk_heat_flux.py
 lammps_step/tk_initialization.py
 lammps_step/tk_lammps.py
 lammps_step/tk_minimization.py
 lammps_step/tk_npt.py
 lammps_step/tk_nve.py
 lammps_step/tk_nvt.py
 lammps_step/tk_velocities.py
```

### Comparing `lammps_step-2023.4.9/lammps_step.egg-info/entry_points.txt` & `lammps_step-2023.5.29/lammps_step.egg-info/entry_points.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 
 [org.molssi.seamm]
 LAMMPS = lammps_step:LAMMPSStep
 
 [org.molssi.seamm.lammps]
 Custom = lammps_step:CustomStep
 Energy = lammps_step:EnergyStep
+HeatFlux = lammps_step:HeatFluxStep
 Initialization = lammps_step:InitializationStep
 Minimization = lammps_step:MinimizationStep
 NPT = lammps_step:NPTStep
 NVE = lammps_step:NVEStep
 NVT = lammps_step:NVTStep
 Velocities = lammps_step:VelocitiesStep
 
 [org.molssi.seamm.lammps.tk]
 Custom = lammps_step:CustomStep
 Energy = lammps_step:EnergyStep
+HeatFlux = lammps_step:HeatFluxStep
 Initialization = lammps_step:InitializationStep
 Minimization = lammps_step:MinimizationStep
 NPT = lammps_step:NPTStep
 NVE = lammps_step:NVEStep
 NVT = lammps_step:NVTStep
 Velocities = lammps_step:VelocitiesStep
```

### Comparing `lammps_step-2023.4.9/setup.py` & `lammps_step-2023.5.29/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,24 +85,26 @@
         'org.molssi.seamm': [
             'LAMMPS = lammps_step:LAMMPSStep',
         ],
         'org.molssi.seamm.tk': [
             'LAMMPS = lammps_step:LAMMPSStep',
         ],
         'org.molssi.seamm.lammps': [
+            'HeatFlux = lammps_step:HeatFluxStep',
             'Custom = lammps_step:CustomStep',
             'Energy = lammps_step:EnergyStep',
             'Initialization = lammps_step:InitializationStep',
             'Minimization = lammps_step:MinimizationStep',
             'NVE = lammps_step:NVEStep',
             'NVT = lammps_step:NVTStep',
             'NPT = lammps_step:NPTStep',
             'Velocities = lammps_step:VelocitiesStep',
         ],
         'org.molssi.seamm.lammps.tk': [
+            'HeatFlux = lammps_step:HeatFluxStep',
             'Custom = lammps_step:CustomStep',
             'Energy = lammps_step:EnergyStep',
             'Initialization = lammps_step:InitializationStep',
             'Minimization = lammps_step:MinimizationStep',
             'NVE = lammps_step:NVEStep',
             'NVT = lammps_step:NVTStep',
             'NPT = lammps_step:NPTStep',
```

### Comparing `lammps_step-2023.4.9/tests/data/Ar_xtal_energy.flow` & `lammps_step-2023.5.29/tests/data/Ar_xtal_energy.flow`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/tests/test_lammps_step.py` & `lammps_step-2023.5.29/tests/test_lammps_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/tests/test_lammps_units.py` & `lammps_step-2023.5.29/tests/test_lammps_units.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.9/versioneer.py` & `lammps_step-2023.5.29/versioneer.py`

 * *Files identical despite different names*

