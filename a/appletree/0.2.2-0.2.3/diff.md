# Comparing `tmp/appletree-0.2.2.tar.gz` & `tmp/appletree-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appletree-0.2.2.tar", last modified: Thu May 25 08:20:07 2023, max compression
+gzip compressed data, was "appletree-0.2.3.tar", last modified: Mon May 29 04:41:34 2023, max compression
```

## Comparing `appletree-0.2.2.tar` & `appletree-0.2.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:07.429190 appletree-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-25 08:19:59.000000 appletree-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-05-25 08:20:07.429190 appletree-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-25 08:19:59.000000 appletree-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:07.425190 appletree-0.2.2/appletree/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20163 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:07.425190 appletree-0.2.2/appletree/components/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/components/ac.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/components/er.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/components/nr.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/components/yields.py
--rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13775 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:07.425190 appletree-0.2.2/appletree/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/contexts/er_only.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:07.425190 appletree-0.2.2/appletree/data/
--rw-r--r--   0 runner    (1001) docker     (123)   160762 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/data/AC_Rn220.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    20522 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/data/data_Ar37.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/data/data_Neutron.csv
--rw-r--r--   0 runner    (1001) docker     (123)    47270 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/data/data_Rn220.csv
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/hist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:07.425190 appletree-0.2.2/appletree/instructs/
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/instructs/literature_lyqy.json
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/instructs/neutron_low.json
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/instructs/rn220.json
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/instructs/rn220_ar37.json
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16017 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:07.429190 appletree-0.2.2/appletree/maps/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/maps/3fold_recon_eff.json
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/maps/elife.json
--rw-r--r--   0 runner    (1001) docker     (123)    15745 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/maps/nr_ly_median.json
--rw-r--r--   0 runner    (1001) docker     (123)    15789 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/maps/nr_qy_median.json
--rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/maps/nr_spectrum.json
--rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/maps/posrec_reso.json
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/maps/s1_bias_3f.json
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/maps/s1_correction_map_regbin.json
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/maps/s1_cut_acc.json
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/maps/s1_smearing_3f.json
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/maps/s2_bias.json
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/maps/s2_correction_map_regbin.json
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/maps/s2_cut_acc.json
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/maps/s2_smearing.json
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:07.429190 appletree-0.2.2/appletree/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/parameters/er.json
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/parameters/nestv2.json
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/parameters/nr_low.json
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:07.429190 appletree-0.2.2/appletree/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/plugins/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/plugins/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/plugins/efficiency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/plugins/er_microphys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/plugins/lyqy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/plugins/nestv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/plugins/reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/randgen.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/share.py
--rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-05-25 08:19:59.000000 appletree-0.2.2/appletree/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:07.425190 appletree-0.2.2/appletree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-05-25 08:20:07.000000 appletree-0.2.2/appletree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-25 08:20:07.000000 appletree-0.2.2/appletree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 08:20:07.000000 appletree-0.2.2/appletree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 08:20:07.000000 appletree-0.2.2/appletree.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-25 08:20:07.000000 appletree-0.2.2/appletree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 08:20:07.000000 appletree-0.2.2/appletree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-25 08:20:07.429190 appletree-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-25 08:19:59.000000 appletree-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:41:34.014093 appletree-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-29 04:41:25.000000 appletree-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-05-29 04:41:34.014093 appletree-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-29 04:41:25.000000 appletree-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:41:34.010093 appletree-0.2.3/appletree/
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20163 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:41:34.010093 appletree-0.2.3/appletree/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/components/ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/components/er.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/components/nr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/components/yields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13775 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:41:34.010093 appletree-0.2.3/appletree/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/contexts/er_only.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:41:34.010093 appletree-0.2.3/appletree/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   160762 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/data/AC_Rn220.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    20522 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/data/data_Ar37.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/data/data_Neutron.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    47270 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/data/data_Rn220.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/hist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:41:34.010093 appletree-0.2.3/appletree/instructs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/instructs/literature_lyqy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/instructs/neutron_low.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/instructs/rn220.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/instructs/rn220_ar37.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16017 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:41:34.010093 appletree-0.2.3/appletree/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/maps/3fold_recon_eff.json
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/maps/elife.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15745 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/maps/nr_ly_median.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15789 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/maps/nr_qy_median.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/maps/nr_spectrum.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/maps/posrec_reso.json
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/maps/s1_bias_3f.json
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/maps/s1_correction_map_regbin.json
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/maps/s1_cut_acc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/maps/s1_smearing_3f.json
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/maps/s2_bias.json
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/maps/s2_correction_map_regbin.json
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/maps/s2_cut_acc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/maps/s2_smearing.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:41:34.010093 appletree-0.2.3/appletree/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/parameters/er.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/parameters/nestv2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/parameters/nr_low.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:41:34.014093 appletree-0.2.3/appletree/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/plugins/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/plugins/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/plugins/efficiency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/plugins/er_microphys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/plugins/lyqy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/plugins/nestv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/plugins/reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/randgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/share.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-05-29 04:41:25.000000 appletree-0.2.3/appletree/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:41:34.010093 appletree-0.2.3/appletree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-05-29 04:41:33.000000 appletree-0.2.3/appletree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-29 04:41:33.000000 appletree-0.2.3/appletree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 04:41:33.000000 appletree-0.2.3/appletree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 04:41:33.000000 appletree-0.2.3/appletree.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-29 04:41:33.000000 appletree-0.2.3/appletree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-29 04:41:33.000000 appletree-0.2.3/appletree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-29 04:41:34.014093 appletree-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-29 04:41:25.000000 appletree-0.2.3/setup.py
```

### Comparing `appletree-0.2.2/LICENSE` & `appletree-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/PKG-INFO` & `appletree-0.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,87 @@
 Metadata-Version: 2.1
 Name: appletree
-Version: 0.2.2
+Version: 0.2.3
 Summary: A high-Performance Program simuLatEs and fiTs REsponse of xEnon.
 Home-page: https://github.com/XENONnT/appletree
 Author: Appletree contributors, the XENON collaboration
 License: UNKNOWN
 Description: # Appletree
+        
         A high-Performance Program simuLatEs and fiTs REsponse of xEnon.
         
         [![DOI](https://zenodo.org/badge/534803881.svg)](https://zenodo.org/badge/latestdoi/534803881)
         [![Test package](https://github.com/XENONnT/appletree/actions/workflows/pytest.yml/badge.svg?branch=master)](https://github.com/XENONnT/appletree/actions/workflows/pytest.yml)
         [![Coverage Status](https://coveralls.io/repos/github/XENONnT/appletree/badge.svg)](https://coveralls.io/github/XENONnT/appletree)
         [![PyPI version shields.io](https://img.shields.io/pypi/v/appletree.svg)](https://pypi.python.org/pypi/appletree/)
         [![Readthedocs Badge](https://readthedocs.org/projects/appletree/badge/?version=latest)](https://appletree.readthedocs.io/en/latest/?badge=latest)
         [![CodeFactor](https://www.codefactor.io/repository/github/xenonnt/appletree/badge)](https://www.codefactor.io/repository/github/xenonnt/appletree)
         
         ## Installation and Set-Up
         
         ### Regular installation:
+        
+        With cpu support:
+        
+        ```
+        pip install appletree[cpu]
+        ```
+        
+        With CUDA Toolkit 11.2 support:
+        
+        ```
+        pip install appletree[cuda112] -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+        ```
+        
+        With CUDA Toolkit 12.1 support:
+        
         ```
-        pip install appletree -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+        pip install appletree[cuda121] -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
         ```
         
         ### Developer setup:
+        
         Clone the repository:
         
         ```
         git clone https://github.com/XENONnT/appletree
         cd appletree
         ```
         
-        Install the package and requirements in your environment:
+        To install the package and requirements in your environment, replace `pip install appletree[*]` to `python3 -m pip install .[*] --user` in the above `pip` commands.
         
-        ```
-        pip install -r requirements.txt
-        python3 -m pip install ./ --user
-        ```
+        To install appletree in editable mode, insert `--editable` argument after `install` in the above `pip install` or `python3 -m pip install` commands.
         
-        If you wanna install appletree in editable mode, replace the last line with
+        For example, to install in your environment and in editable mode with CUDA Toolkit 12.1 support:
         
         ```
-        python3 -m pip install --editable ./ --user
+        python3 -m pip install --editable .[cuda121] --user -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
         ```
         
-        You are now good to go!
+        Then you are now good to go!
         
         ## Usage
+        
         The best way to start with the `appletree` package is to have a look at the tutorial `notebooks`. 
         
         ## Contributing
+        
         Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
         
         Please make sure to update tests as appropriate.
         
         
+        v0.2.3 / 2023-05-29
+        -------------------
+        * Add pip install user by @dachengx in https://github.com/XENONnT/appletree/pull/96
+        * Installation with various `extras_require`s for different CUDA support by @dachengx in https://github.com/XENONnT/appletree/pull/97
+        
+        **Full Changelog**: https://github.com/XENONnT/appletree/compare/v0.2.2...v0.2.3
+        
+        
         v0.2.2 / 2023-05-25
         -------------------
         * Stop using MANIFEST.in, move to a modern way of file system configuration by @dachengx in https://github.com/XENONnT/appletree/pull/94
         
         **Full Changelog**: https://github.com/XENONnT/appletree/compare/v0.2.1...v0.2.2
         
         
@@ -115,9 +139,10 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: doc
-Provides-Extra: test
+Provides-Extra: cpu
+Provides-Extra: cuda112
+Provides-Extra: cuda121
```

### Comparing `appletree-0.2.2/README.md` & `appletree-0.2.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,63 @@
 # Appletree
+
 A high-Performance Program simuLatEs and fiTs REsponse of xEnon.
 
 [![DOI](https://zenodo.org/badge/534803881.svg)](https://zenodo.org/badge/latestdoi/534803881)
 [![Test package](https://github.com/XENONnT/appletree/actions/workflows/pytest.yml/badge.svg?branch=master)](https://github.com/XENONnT/appletree/actions/workflows/pytest.yml)
 [![Coverage Status](https://coveralls.io/repos/github/XENONnT/appletree/badge.svg)](https://coveralls.io/github/XENONnT/appletree)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/appletree.svg)](https://pypi.python.org/pypi/appletree/)
 [![Readthedocs Badge](https://readthedocs.org/projects/appletree/badge/?version=latest)](https://appletree.readthedocs.io/en/latest/?badge=latest)
 [![CodeFactor](https://www.codefactor.io/repository/github/xenonnt/appletree/badge)](https://www.codefactor.io/repository/github/xenonnt/appletree)
 
 ## Installation and Set-Up
 
 ### Regular installation:
+
+With cpu support:
+
+```
+pip install appletree[cpu]
+```
+
+With CUDA Toolkit 11.2 support:
+
+```
+pip install appletree[cuda112] -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
-pip install appletree -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+
+With CUDA Toolkit 12.1 support:
+
+```
+pip install appletree[cuda121] -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
 
 ### Developer setup:
+
 Clone the repository:
 
 ```
 git clone https://github.com/XENONnT/appletree
 cd appletree
 ```
 
-Install the package and requirements in your environment:
+To install the package and requirements in your environment, replace `pip install appletree[*]` to `python3 -m pip install .[*] --user` in the above `pip` commands.
 
-```
-pip install -r requirements.txt
-python3 -m pip install ./ --user
-```
+To install appletree in editable mode, insert `--editable` argument after `install` in the above `pip install` or `python3 -m pip install` commands.
 
-If you wanna install appletree in editable mode, replace the last line with
+For example, to install in your environment and in editable mode with CUDA Toolkit 12.1 support:
 
 ```
-python3 -m pip install --editable ./ --user
+python3 -m pip install --editable .[cuda121] --user -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
 
-You are now good to go!
+Then you are now good to go!
 
 ## Usage
+
 The best way to start with the `appletree` package is to have a look at the tutorial `notebooks`. 
 
 ## Contributing
+
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
```

### Comparing `appletree-0.2.2/appletree/__init__.py` & `appletree-0.2.3/appletree/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.2'
+__version__ = '0.2.3'
 
 from . import utils
 from .utils import *
 
 from . import hist
 from .hist import *
 
@@ -37,14 +37,29 @@
 
 from . import contexts
 from .contexts import *
 
 from . import context
 from .context import *
 
+# check CUDA support setup
+from warnings import warn
+platform = utils.get_platform()
+if platform == 'cpu':
+    warning = 'You are running appletree on CPU, which usually results in low performance.'
+    warn(warning)
+try:
+    import jax
+    # try allocate something
+    jax.numpy.ones(1)
+except BaseException:
+    if platform == 'gpu':
+        print('Can not allocate memory on GPU, please check your CUDA version.')
+    raise ImportError(f'Appletree is not correctly setup to be used on {platform.upper()}.')
+
 try:
     import aptext
     HAVE_APTEXT = True
     print('Using aptext package from https://github.com/XENONnT/applefiles')
 except ImportError:
     HAVE_APTEXT = False
     print('Can not find aptext')
```

### Comparing `appletree-0.2.2/appletree/component.py` & `appletree-0.2.3/appletree/component.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/components/er.py` & `appletree-0.2.3/appletree/components/er.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/components/nr.py` & `appletree-0.2.3/appletree/components/nr.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/components/yields.py` & `appletree-0.2.3/appletree/components/yields.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/config.py` & `appletree-0.2.3/appletree/config.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/context.py` & `appletree-0.2.3/appletree/context.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/contexts/er_only.py` & `appletree-0.2.3/appletree/contexts/er_only.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/data/AC_Rn220.pkl` & `appletree-0.2.3/appletree/data/AC_Rn220.pkl`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/data/data_Ar37.csv` & `appletree-0.2.3/appletree/data/data_Ar37.csv`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/data/data_Neutron.csv` & `appletree-0.2.3/appletree/data/data_Neutron.csv`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/data/data_Rn220.csv` & `appletree-0.2.3/appletree/data/data_Rn220.csv`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/hist.py` & `appletree-0.2.3/appletree/hist.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/instructs/literature_lyqy.json` & `appletree-0.2.3/appletree/instructs/literature_lyqy.json`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/instructs/neutron_low.json` & `appletree-0.2.3/appletree/instructs/neutron_low.json`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/instructs/rn220.json` & `appletree-0.2.3/appletree/instructs/rn220.json`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/instructs/rn220_ar37.json` & `appletree-0.2.3/appletree/instructs/rn220_ar37.json`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/interpolation.py` & `appletree-0.2.3/appletree/interpolation.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/likelihood.py` & `appletree-0.2.3/appletree/likelihood.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/maps/nr_ly_median.json` & `appletree-0.2.3/appletree/maps/nr_ly_median.json`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/maps/nr_qy_median.json` & `appletree-0.2.3/appletree/maps/nr_qy_median.json`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/maps/nr_spectrum.json` & `appletree-0.2.3/appletree/maps/nr_spectrum.json`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/maps/posrec_reso.json` & `appletree-0.2.3/appletree/maps/posrec_reso.json`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/maps/s1_correction_map_regbin.json` & `appletree-0.2.3/appletree/maps/s1_correction_map_regbin.json`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/maps/s1_smearing_3f.json` & `appletree-0.2.3/appletree/maps/s1_smearing_3f.json`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/maps/s2_smearing.json` & `appletree-0.2.3/appletree/maps/s2_smearing.json`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/parameter.py` & `appletree-0.2.3/appletree/parameter.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/parameters/er.json` & `appletree-0.2.3/appletree/parameters/er.json`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/parameters/nestv2.json` & `appletree-0.2.3/appletree/parameters/nestv2.json`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/parameters/nr_low.json` & `appletree-0.2.3/appletree/parameters/nr_low.json`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/plugin.py` & `appletree-0.2.3/appletree/plugin.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/plugins/common.py` & `appletree-0.2.3/appletree/plugins/common.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/plugins/detector.py` & `appletree-0.2.3/appletree/plugins/detector.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/plugins/efficiency.py` & `appletree-0.2.3/appletree/plugins/efficiency.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/plugins/er_microphys.py` & `appletree-0.2.3/appletree/plugins/er_microphys.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/plugins/lyqy.py` & `appletree-0.2.3/appletree/plugins/lyqy.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/plugins/nestv2.py` & `appletree-0.2.3/appletree/plugins/nestv2.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/plugins/reconstruction.py` & `appletree-0.2.3/appletree/plugins/reconstruction.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/randgen.py` & `appletree-0.2.3/appletree/randgen.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/share.py` & `appletree-0.2.3/appletree/share.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree/utils.py` & `appletree-0.2.3/appletree/utils.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/appletree.egg-info/PKG-INFO` & `appletree-0.2.3/appletree.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,87 @@
 Metadata-Version: 2.1
 Name: appletree
-Version: 0.2.2
+Version: 0.2.3
 Summary: A high-Performance Program simuLatEs and fiTs REsponse of xEnon.
 Home-page: https://github.com/XENONnT/appletree
 Author: Appletree contributors, the XENON collaboration
 License: UNKNOWN
 Description: # Appletree
+        
         A high-Performance Program simuLatEs and fiTs REsponse of xEnon.
         
         [![DOI](https://zenodo.org/badge/534803881.svg)](https://zenodo.org/badge/latestdoi/534803881)
         [![Test package](https://github.com/XENONnT/appletree/actions/workflows/pytest.yml/badge.svg?branch=master)](https://github.com/XENONnT/appletree/actions/workflows/pytest.yml)
         [![Coverage Status](https://coveralls.io/repos/github/XENONnT/appletree/badge.svg)](https://coveralls.io/github/XENONnT/appletree)
         [![PyPI version shields.io](https://img.shields.io/pypi/v/appletree.svg)](https://pypi.python.org/pypi/appletree/)
         [![Readthedocs Badge](https://readthedocs.org/projects/appletree/badge/?version=latest)](https://appletree.readthedocs.io/en/latest/?badge=latest)
         [![CodeFactor](https://www.codefactor.io/repository/github/xenonnt/appletree/badge)](https://www.codefactor.io/repository/github/xenonnt/appletree)
         
         ## Installation and Set-Up
         
         ### Regular installation:
+        
+        With cpu support:
+        
+        ```
+        pip install appletree[cpu]
+        ```
+        
+        With CUDA Toolkit 11.2 support:
+        
+        ```
+        pip install appletree[cuda112] -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+        ```
+        
+        With CUDA Toolkit 12.1 support:
+        
         ```
-        pip install appletree -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+        pip install appletree[cuda121] -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
         ```
         
         ### Developer setup:
+        
         Clone the repository:
         
         ```
         git clone https://github.com/XENONnT/appletree
         cd appletree
         ```
         
-        Install the package and requirements in your environment:
+        To install the package and requirements in your environment, replace `pip install appletree[*]` to `python3 -m pip install .[*] --user` in the above `pip` commands.
         
-        ```
-        pip install -r requirements.txt
-        python3 -m pip install ./ --user
-        ```
+        To install appletree in editable mode, insert `--editable` argument after `install` in the above `pip install` or `python3 -m pip install` commands.
         
-        If you wanna install appletree in editable mode, replace the last line with
+        For example, to install in your environment and in editable mode with CUDA Toolkit 12.1 support:
         
         ```
-        python3 -m pip install --editable ./ --user
+        python3 -m pip install --editable .[cuda121] --user -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
         ```
         
-        You are now good to go!
+        Then you are now good to go!
         
         ## Usage
+        
         The best way to start with the `appletree` package is to have a look at the tutorial `notebooks`. 
         
         ## Contributing
+        
         Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
         
         Please make sure to update tests as appropriate.
         
         
+        v0.2.3 / 2023-05-29
+        -------------------
+        * Add pip install user by @dachengx in https://github.com/XENONnT/appletree/pull/96
+        * Installation with various `extras_require`s for different CUDA support by @dachengx in https://github.com/XENONnT/appletree/pull/97
+        
+        **Full Changelog**: https://github.com/XENONnT/appletree/compare/v0.2.2...v0.2.3
+        
+        
         v0.2.2 / 2023-05-25
         -------------------
         * Stop using MANIFEST.in, move to a modern way of file system configuration by @dachengx in https://github.com/XENONnT/appletree/pull/94
         
         **Full Changelog**: https://github.com/XENONnT/appletree/compare/v0.2.1...v0.2.2
         
         
@@ -115,9 +139,10 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: doc
-Provides-Extra: test
+Provides-Extra: cpu
+Provides-Extra: cuda112
+Provides-Extra: cuda121
```

### Comparing `appletree-0.2.2/appletree.egg-info/SOURCES.txt` & `appletree-0.2.3/appletree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/setup.cfg` & `appletree-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `appletree-0.2.2/setup.py` & `appletree-0.2.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,27 +15,35 @@
     readme = file.read()
 
 with open('HISTORY.md') as file:
     history = file.read()
 
 setuptools.setup(
     name='appletree',
-    version='0.2.2',
+    version='0.2.3',
     description='A high-Performance Program simuLatEs and fiTs REsponse of xEnon.',
     author='Appletree contributors, the XENON collaboration',
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     setup_requires=['pytest-runner'],
     install_requires=requires,
     python_requires='>=3.8',
     extras_require={
-        'doc': [],
-        'test': [
-            'pytest',
-            'flake8',
+        'cpu': [
+            # pip install appletree[cpu]
+            'jax[cpu]',
+        ],
+        'cuda112': [
+            # pip install appletree[cuda112] -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+            'jax[cuda]==0.3.15',
+        ],
+        'cuda121': [
+            # pip install appletree[cuda121] -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+            # according to this commit, jax[cuda12_pip]==0.4.10 is valid for CUDA Toolkit 12.1
+            'jax[cuda12_pip]',
         ],
     },
     packages=setuptools.find_packages(),
     package_data={
         'appletree': [
             'instructs/*',
             'parameters/*',
```

