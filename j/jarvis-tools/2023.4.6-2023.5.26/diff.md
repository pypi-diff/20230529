# Comparing `tmp/jarvis-tools-2023.4.6.tar.gz` & `tmp/jarvis-tools-2023.5.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jarvis-tools-2023.4.6.tar", last modified: Fri Apr  7 04:53:25 2023, max compression
+gzip compressed data, was "dist/jarvis-tools-2023.5.26.tar", last modified: Mon May 29 12:53:07 2023, max compression
```

## Comparing `jarvis-tools-2023.4.6.tar` & `jarvis-tools-2023.5.26.tar`

### file list

```diff
@@ -1,279 +1,279 @@
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:25.000000 jarvis-tools-2023.4.6/
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:12.000000 jarvis-tools-2023.4.6/jarvis/
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:12.000000 jarvis-tools-2023.4.6/jarvis/ai/
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:12.000000 jarvis-tools-2023.4.6/jarvis/ai/descriptors/
--rw-r--r--   0 knc6     (54782) users      (100)       48 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/ai/descriptors/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)    48400 2023-03-24 19:10:21.000000 jarvis-tools-2023.4.6/jarvis/ai/descriptors/cfid.py
--rw-r--r--   0 knc6     (54782) users      (100)     1370 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/ai/descriptors/coulomb.py
--rw-r--r--   0 knc6     (54782) users      (100)      511 2022-05-21 15:06:08.000000 jarvis-tools-2023.4.6/jarvis/ai/descriptors/elemental.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:12.000000 jarvis-tools-2023.4.6/jarvis/ai/gcn/
--rw-r--r--   0 knc6     (54782) users      (100)       47 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/ai/gcn/__init__.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:12.000000 jarvis-tools-2023.4.6/jarvis/ai/pkgs/
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:12.000000 jarvis-tools-2023.4.6/jarvis/ai/pkgs/lgbm/
--rw-r--r--   0 knc6     (54782) users      (100)       28 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/ai/pkgs/lgbm/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     1148 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/ai/pkgs/lgbm/classification.py
--rw-r--r--   0 knc6     (54782) users      (100)     9541 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/ai/pkgs/lgbm/regression.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:13.000000 jarvis-tools-2023.4.6/jarvis/ai/pkgs/sklearn/
--rw-r--r--   0 knc6     (54782) users      (100)       44 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/ai/pkgs/sklearn/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     5144 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/ai/pkgs/sklearn/classification.py
--rw-r--r--   0 knc6     (54782) users      (100)    11368 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/ai/pkgs/sklearn/hyper_params.py
--rw-r--r--   0 knc6     (54782) users      (100)     2969 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/ai/pkgs/sklearn/regression.py
--rw-r--r--   0 knc6     (54782) users      (100)       35 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/ai/pkgs/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     3585 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/ai/pkgs/utils.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:13.000000 jarvis-tools-2023.4.6/jarvis/ai/uncertainty/
--rw-r--r--   0 knc6     (54782) users      (100)       34 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/ai/uncertainty/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     7487 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/ai/uncertainty/lgbm_quantile_uncertainty.py
--rw-r--r--   0 knc6     (54782) users      (100)       35 2021-06-19 18:54:48.000000 jarvis-tools-2023.4.6/jarvis/ai/__init__.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:13.000000 jarvis-tools-2023.4.6/jarvis/analysis/
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:13.000000 jarvis-tools-2023.4.6/jarvis/analysis/darkmatter/
--rw-r--r--   0 knc6     (54782) users      (100)       51 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/analysis/darkmatter/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)      786 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/analysis/darkmatter/metrics.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:13.000000 jarvis-tools-2023.4.6/jarvis/analysis/defects/
--rw-r--r--   0 knc6     (54782) users      (100)       47 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/analysis/defects/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     2328 2021-08-18 22:05:59.000000 jarvis-tools-2023.4.6/jarvis/analysis/defects/substitutions.py
--rw-r--r--   0 knc6     (54782) users      (100)     9305 2021-07-23 21:33:58.000000 jarvis-tools-2023.4.6/jarvis/analysis/defects/surface.py
--rw-r--r--   0 knc6     (54782) users      (100)     5048 2022-05-21 15:07:48.000000 jarvis-tools-2023.4.6/jarvis/analysis/defects/vacancy.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:13.000000 jarvis-tools-2023.4.6/jarvis/analysis/diffraction/
--rw-r--r--   0 knc6     (54782) users      (100)       49 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/analysis/diffraction/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     6825 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/analysis/diffraction/atomic_scattering_params.json
--rw-r--r--   0 knc6     (54782) users      (100)     7327 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/analysis/diffraction/xrd.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:13.000000 jarvis-tools-2023.4.6/jarvis/analysis/elastic/
--rw-r--r--   0 knc6     (54782) users      (100)       43 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/analysis/elastic/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     6602 2022-05-06 22:27:09.000000 jarvis-tools-2023.4.6/jarvis/analysis/elastic/tensor.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:14.000000 jarvis-tools-2023.4.6/jarvis/analysis/interface/
--rw-r--r--   0 knc6     (54782) users      (100)       53 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/analysis/interface/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)    14764 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/analysis/interface/zur.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:14.000000 jarvis-tools-2023.4.6/jarvis/analysis/magnetism/
--rw-r--r--   0 knc6     (54782) users      (100)       46 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/analysis/magnetism/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     8101 2021-06-19 18:54:50.000000 jarvis-tools-2023.4.6/jarvis/analysis/magnetism/magmom_setup.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:14.000000 jarvis-tools-2023.4.6/jarvis/analysis/periodic/
--rw-r--r--   0 knc6     (54782) users      (100)       49 2021-06-19 18:54:50.000000 jarvis-tools-2023.4.6/jarvis/analysis/periodic/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     5907 2021-06-19 18:54:50.000000 jarvis-tools-2023.4.6/jarvis/analysis/periodic/ptable.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:14.000000 jarvis-tools-2023.4.6/jarvis/analysis/phonon/
--rw-r--r--   0 knc6     (54782) users      (100)       49 2021-06-19 18:54:50.000000 jarvis-tools-2023.4.6/jarvis/analysis/phonon/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     3934 2022-12-06 20:07:55.000000 jarvis-tools-2023.4.6/jarvis/analysis/phonon/dos.py
--rw-r--r--   0 knc6     (54782) users      (100)     1189 2021-06-19 18:54:50.000000 jarvis-tools-2023.4.6/jarvis/analysis/phonon/force_constants.py
--rw-r--r--   0 knc6     (54782) users      (100)     6473 2023-01-09 20:58:01.000000 jarvis-tools-2023.4.6/jarvis/analysis/phonon/ir.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:15.000000 jarvis-tools-2023.4.6/jarvis/analysis/solarefficiency/
--rw-r--r--   0 knc6     (54782) users      (100)       59 2021-06-19 18:54:50.000000 jarvis-tools-2023.4.6/jarvis/analysis/solarefficiency/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)    35436 2021-06-19 18:54:50.000000 jarvis-tools-2023.4.6/jarvis/analysis/solarefficiency/am1.5G.dat
--rw-r--r--   0 knc6     (54782) users      (100)    14217 2021-06-19 18:54:50.000000 jarvis-tools-2023.4.6/jarvis/analysis/solarefficiency/solar.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:15.000000 jarvis-tools-2023.4.6/jarvis/analysis/stem/
--rw-r--r--   0 knc6     (54782) users      (100)       38 2021-06-19 18:54:50.000000 jarvis-tools-2023.4.6/jarvis/analysis/stem/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     7315 2022-05-21 15:11:22.000000 jarvis-tools-2023.4.6/jarvis/analysis/stem/convolution_apprx.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:15.000000 jarvis-tools-2023.4.6/jarvis/analysis/stm/
--rw-r--r--   0 knc6     (54782) users      (100)       67 2021-06-19 18:54:50.000000 jarvis-tools-2023.4.6/jarvis/analysis/stm/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)    10094 2021-07-01 05:40:25.000000 jarvis-tools-2023.4.6/jarvis/analysis/stm/tersoff_hamann.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:15.000000 jarvis-tools-2023.4.6/jarvis/analysis/structure/
--rw-r--r--   0 knc6     (54782) users      (100)       46 2021-06-19 18:54:50.000000 jarvis-tools-2023.4.6/jarvis/analysis/structure/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)    21798 2021-06-19 18:54:50.000000 jarvis-tools-2023.4.6/jarvis/analysis/structure/neighbors.py
--rw-r--r--   0 knc6     (54782) users      (100)    25663 2021-12-17 15:03:20.000000 jarvis-tools-2023.4.6/jarvis/analysis/structure/spacegroup.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:16.000000 jarvis-tools-2023.4.6/jarvis/analysis/thermodynamics/
--rw-r--r--   0 knc6     (54782) users      (100)       42 2021-06-19 18:54:50.000000 jarvis-tools-2023.4.6/jarvis/analysis/thermodynamics/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)    14613 2023-04-07 04:22:25.000000 jarvis-tools-2023.4.6/jarvis/analysis/thermodynamics/energetics.py
--rw-r--r--   0 knc6     (54782) users      (100)     4527 2021-06-19 18:54:50.000000 jarvis-tools-2023.4.6/jarvis/analysis/thermodynamics/unary.json
--rw-r--r--   0 knc6     (54782) users      (100)     4781 2021-06-21 21:20:14.000000 jarvis-tools-2023.4.6/jarvis/analysis/thermodynamics/unary_qe_tb.json
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:16.000000 jarvis-tools-2023.4.6/jarvis/analysis/topological/
--rw-r--r--   0 knc6     (54782) users      (100)       50 2021-06-19 18:54:50.000000 jarvis-tools-2023.4.6/jarvis/analysis/topological/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)    11892 2021-06-19 18:54:50.000000 jarvis-tools-2023.4.6/jarvis/analysis/topological/spillage.py
--rw-r--r--   0 knc6     (54782) users      (100)       35 2021-06-19 18:54:49.000000 jarvis-tools-2023.4.6/jarvis/analysis/__init__.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:17.000000 jarvis-tools-2023.4.6/jarvis/core/
--rw-r--r--   0 knc6     (54782) users      (100)  1421253 2021-06-19 18:54:50.000000 jarvis-tools-2023.4.6/jarvis/core/Elements.json
--rw-r--r--   0 knc6     (54782) users      (100)       49 2021-06-19 18:54:51.000000 jarvis-tools-2023.4.6/jarvis/core/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)    28393 2021-06-19 18:54:51.000000 jarvis-tools-2023.4.6/jarvis/core/atom_init.json
--rw-r--r--   0 knc6     (54782) users      (100)    66720 2022-08-28 18:59:14.000000 jarvis-tools-2023.4.6/jarvis/core/atoms.py
--rw-r--r--   0 knc6     (54782) users      (100)     4313 2022-05-21 15:13:20.000000 jarvis-tools-2023.4.6/jarvis/core/circuits.py
--rw-r--r--   0 knc6     (54782) users      (100)     5258 2021-07-06 06:09:50.000000 jarvis-tools-2023.4.6/jarvis/core/composition.py
--rw-r--r--   0 knc6     (54782) users      (100)  1162701 2021-06-19 18:54:51.000000 jarvis-tools-2023.4.6/jarvis/core/element_charge.json
--rw-r--r--   0 knc6     (54782) users      (100)    22721 2022-07-18 17:09:48.000000 jarvis-tools-2023.4.6/jarvis/core/graphs.py
--rw-r--r--   0 knc6     (54782) users      (100)    10693 2022-08-28 18:10:43.000000 jarvis-tools-2023.4.6/jarvis/core/image.py
--rw-r--r--   0 knc6     (54782) users      (100)    37783 2021-10-05 17:33:43.000000 jarvis-tools-2023.4.6/jarvis/core/kpoints.py
--rw-r--r--   0 knc6     (54782) users      (100)    17427 2023-01-09 20:58:01.000000 jarvis-tools-2023.4.6/jarvis/core/lattice.py
--rw-r--r--   0 knc6     (54782) users      (100)    47766 2021-07-23 21:33:59.000000 jarvis-tools-2023.4.6/jarvis/core/magpie.json
--rw-r--r--   0 knc6     (54782) users      (100)    11981 2021-07-23 21:33:59.000000 jarvis-tools-2023.4.6/jarvis/core/specie.py
--rw-r--r--   0 knc6     (54782) users      (100)     2891 2023-01-09 20:58:01.000000 jarvis-tools-2023.4.6/jarvis/core/spectrum.py
--rw-r--r--   0 knc6     (54782) users      (100)     8933 2022-02-24 23:02:40.000000 jarvis-tools-2023.4.6/jarvis/core/utils.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:18.000000 jarvis-tools-2023.4.6/jarvis/db/
--rw-r--r--   0 knc6     (54782) users      (100)       53 2021-06-19 18:54:52.000000 jarvis-tools-2023.4.6/jarvis/db/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)    19682 2023-03-24 19:10:21.000000 jarvis-tools-2023.4.6/jarvis/db/figshare.py
--rw-r--r--   0 knc6     (54782) users      (100)      378 2021-06-19 18:54:52.000000 jarvis-tools-2023.4.6/jarvis/db/jsonutils.py
--rw-r--r--   0 knc6     (54782) users      (100)     7761 2021-06-20 06:25:45.000000 jarvis-tools-2023.4.6/jarvis/db/lammps_to_xml.py
--rw-r--r--   0 knc6     (54782) users      (100)    10649 2021-06-19 18:54:52.000000 jarvis-tools-2023.4.6/jarvis/db/qe_to_xml.py
--rw-r--r--   0 knc6     (54782) users      (100)    16857 2021-06-19 18:54:52.000000 jarvis-tools-2023.4.6/jarvis/db/restapi.py
--rw-r--r--   0 knc6     (54782) users      (100)    75218 2021-06-19 18:54:52.000000 jarvis-tools-2023.4.6/jarvis/db/vasp_to_xml.py
--rw-r--r--   0 knc6     (54782) users      (100)     9586 2021-06-19 18:54:52.000000 jarvis-tools-2023.4.6/jarvis/db/webpages.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:18.000000 jarvis-tools-2023.4.6/jarvis/io/
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:18.000000 jarvis-tools-2023.4.6/jarvis/io/boltztrap/
--rw-r--r--   0 knc6     (54782) users      (100)       67 2021-06-19 18:54:55.000000 jarvis-tools-2023.4.6/jarvis/io/boltztrap/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     6511 2021-06-19 18:54:55.000000 jarvis-tools-2023.4.6/jarvis/io/boltztrap/inputs.py
--rw-r--r--   0 knc6     (54782) users      (100)     6767 2021-06-19 18:54:55.000000 jarvis-tools-2023.4.6/jarvis/io/boltztrap/outputs.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:18.000000 jarvis-tools-2023.4.6/jarvis/io/calphad/
--rw-r--r--   0 knc6     (54782) users      (100)       61 2021-06-19 18:54:55.000000 jarvis-tools-2023.4.6/jarvis/io/calphad/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     4228 2021-06-19 18:54:56.000000 jarvis-tools-2023.4.6/jarvis/io/calphad/write_decorated_poscar.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:18.000000 jarvis-tools-2023.4.6/jarvis/io/lammps/
--rw-r--r--   0 knc6     (54782) users      (100)       52 2021-06-19 18:54:56.000000 jarvis-tools-2023.4.6/jarvis/io/lammps/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)    14622 2021-08-06 21:54:48.000000 jarvis-tools-2023.4.6/jarvis/io/lammps/inputs.py
--rw-r--r--   0 knc6     (54782) users      (100)    20748 2021-08-06 21:54:48.000000 jarvis-tools-2023.4.6/jarvis/io/lammps/outputs.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:18.000000 jarvis-tools-2023.4.6/jarvis/io/nexus/
--rw-r--r--   0 knc6     (54782) users      (100)       47 2021-09-28 18:06:38.000000 jarvis-tools-2023.4.6/jarvis/io/nexus/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     4519 2022-12-07 19:52:37.000000 jarvis-tools-2023.4.6/jarvis/io/nexus/inputs.py
--rw-r--r--   0 knc6     (54782) users      (100)       36 2021-09-28 18:06:38.000000 jarvis-tools-2023.4.6/jarvis/io/nexus/outputs.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:19.000000 jarvis-tools-2023.4.6/jarvis/io/pennylane/
--rw-r--r--   0 knc6     (54782) users      (100)       61 2021-06-19 18:54:56.000000 jarvis-tools-2023.4.6/jarvis/io/pennylane/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     2196 2021-06-19 18:54:56.000000 jarvis-tools-2023.4.6/jarvis/io/pennylane/inputs.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:19.000000 jarvis-tools-2023.4.6/jarvis/io/phonopy/
--rw-r--r--   0 knc6     (54782) users      (100)       43 2021-06-19 18:54:56.000000 jarvis-tools-2023.4.6/jarvis/io/phonopy/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     4501 2023-01-09 20:58:01.000000 jarvis-tools-2023.4.6/jarvis/io/phonopy/fcmat2hr.py
--rw-r--r--   0 knc6     (54782) users      (100)     6844 2023-01-09 20:58:01.000000 jarvis-tools-2023.4.6/jarvis/io/phonopy/inputs.py
--rw-r--r--   0 knc6     (54782) users      (100)     5696 2021-06-19 18:55:19.000000 jarvis-tools-2023.4.6/jarvis/io/phonopy/outputs.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:19.000000 jarvis-tools-2023.4.6/jarvis/io/prismatic/
--rw-r--r--   0 knc6     (54782) users      (100)       50 2021-06-19 18:54:56.000000 jarvis-tools-2023.4.6/jarvis/io/prismatic/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)      674 2021-06-19 18:54:56.000000 jarvis-tools-2023.4.6/jarvis/io/prismatic/inputs.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:19.000000 jarvis-tools-2023.4.6/jarvis/io/qe/
--rw-r--r--   0 knc6     (54782) users      (100)       57 2021-06-19 18:54:56.000000 jarvis-tools-2023.4.6/jarvis/io/qe/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)    15328 2023-03-24 17:09:02.000000 jarvis-tools-2023.4.6/jarvis/io/qe/inputs.py
--rwxr-xr-x   0 knc6     (54782) users      (100)    26674 2022-05-21 15:16:55.000000 jarvis-tools-2023.4.6/jarvis/io/qe/outputs.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:19.000000 jarvis-tools-2023.4.6/jarvis/io/qiskit/
--rw-r--r--   0 knc6     (54782) users      (100)       56 2021-06-19 18:54:56.000000 jarvis-tools-2023.4.6/jarvis/io/qiskit/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)    12100 2022-09-17 18:37:16.000000 jarvis-tools-2023.4.6/jarvis/io/qiskit/inputs.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:20.000000 jarvis-tools-2023.4.6/jarvis/io/tequila/
--rw-r--r--   0 knc6     (54782) users      (100)       60 2021-06-19 18:54:56.000000 jarvis-tools-2023.4.6/jarvis/io/tequila/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     2702 2021-06-19 18:54:56.000000 jarvis-tools-2023.4.6/jarvis/io/tequila/inputs.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:20.000000 jarvis-tools-2023.4.6/jarvis/io/vasp/
--rw-r--r--   0 knc6     (54782) users      (100)       56 2021-06-19 18:54:56.000000 jarvis-tools-2023.4.6/jarvis/io/vasp/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     1522 2021-06-19 18:54:56.000000 jarvis-tools-2023.4.6/jarvis/io/vasp/default_potcars.json
--rw-r--r--   0 knc6     (54782) users      (100)    21148 2022-07-18 17:07:16.000000 jarvis-tools-2023.4.6/jarvis/io/vasp/inputs.py
--rw-r--r--   0 knc6     (54782) users      (100)    77837 2022-07-18 17:08:30.000000 jarvis-tools-2023.4.6/jarvis/io/vasp/outputs.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:20.000000 jarvis-tools-2023.4.6/jarvis/io/wannier/
--rw-r--r--   0 knc6     (54782) users      (100)       61 2021-06-19 18:54:56.000000 jarvis-tools-2023.4.6/jarvis/io/wannier/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     4550 2021-06-19 18:55:19.000000 jarvis-tools-2023.4.6/jarvis/io/wannier/default_semicore.json
--rw-r--r--   0 knc6     (54782) users      (100)     6929 2021-06-19 18:55:19.000000 jarvis-tools-2023.4.6/jarvis/io/wannier/inputs.py
--rw-r--r--   0 knc6     (54782) users      (100)    34195 2021-06-19 18:54:56.000000 jarvis-tools-2023.4.6/jarvis/io/wannier/outputs.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:20.000000 jarvis-tools-2023.4.6/jarvis/io/wanniertools/
--rw-r--r--   0 knc6     (54782) users      (100)       60 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/io/wanniertools/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)    10376 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/io/wanniertools/inputs.py
--rw-r--r--   0 knc6     (54782) users      (100)     3818 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/io/wanniertools/outputs.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:20.000000 jarvis-tools-2023.4.6/jarvis/io/wien2k/
--rw-r--r--   0 knc6     (54782) users      (100)       55 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/io/wien2k/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     3192 2021-12-17 15:03:19.000000 jarvis-tools-2023.4.6/jarvis/io/wien2k/inputs.py
--rw-r--r--   0 knc6     (54782) users      (100)     3254 2021-07-23 21:33:59.000000 jarvis-tools-2023.4.6/jarvis/io/wien2k/outputs.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:21.000000 jarvis-tools-2023.4.6/jarvis/io/zeopp/
--rw-r--r--   0 knc6     (54782) users      (100)       35 2021-07-01 05:40:26.000000 jarvis-tools-2023.4.6/jarvis/io/zeopp/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     2184 2021-10-14 00:41:09.000000 jarvis-tools-2023.4.6/jarvis/io/zeopp/inputs.py
--rw-r--r--   0 knc6     (54782) users      (100)       76 2021-06-19 18:54:55.000000 jarvis-tools-2023.4.6/jarvis/io/__init__.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:21.000000 jarvis-tools-2023.4.6/jarvis/tasks/
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:21.000000 jarvis-tools-2023.4.6/jarvis/tasks/boltztrap/
--rw-r--r--   0 knc6     (54782) users      (100)       56 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tasks/boltztrap/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)      608 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tasks/boltztrap/run.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:21.000000 jarvis-tools-2023.4.6/jarvis/tasks/lammps/
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:21.000000 jarvis-tools-2023.4.6/jarvis/tasks/lammps/templates/
--rw-r--r--   0 knc6     (54782) users      (100)       47 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tasks/lammps/templates/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     3463 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tasks/lammps/templates/displace.mod
--rw-r--r--   0 knc6     (54782) users      (100)     6416 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tasks/lammps/templates/inelast.mod
--rw-r--r--   0 knc6     (54782) users      (100)     6449 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tasks/lammps/templates/inelast_min.mod
--rw-r--r--   0 knc6     (54782) users      (100)     6418 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tasks/lammps/templates/inelast_nobox.mod
--rw-r--r--   0 knc6     (54782) users      (100)     6415 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tasks/lammps/templates/inelastcomb.mod
--rw-r--r--   0 knc6     (54782) users      (100)     6389 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tasks/lammps/templates/inelastreax.mod
--rw-r--r--   0 knc6     (54782) users      (100)     2653 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tasks/lammps/templates/relax.mod
--rw-r--r--   0 knc6     (54782) users      (100)      145 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tasks/lammps/templates/run0.mod
--rw-r--r--   0 knc6     (54782) users      (100)      917 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tasks/lammps/templates/templates.py
--rw-r--r--   0 knc6     (54782) users      (100)       55 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tasks/lammps/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)    13948 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tasks/lammps/lammps.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:21.000000 jarvis-tools-2023.4.6/jarvis/tasks/nexus/
--rw-r--r--   0 knc6     (54782) users      (100)       34 2022-12-07 20:41:49.000000 jarvis-tools-2023.4.6/jarvis/tasks/nexus/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     3243 2022-12-12 23:19:44.000000 jarvis-tools-2023.4.6/jarvis/tasks/nexus/qmc.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:22.000000 jarvis-tools-2023.4.6/jarvis/tasks/phonopy/
--rw-r--r--   0 knc6     (54782) users      (100)       54 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tasks/phonopy/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)      765 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tasks/phonopy/run.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:22.000000 jarvis-tools-2023.4.6/jarvis/tasks/qe/
--rw-r--r--   0 knc6     (54782) users      (100)       29 2022-01-11 17:34:47.000000 jarvis-tools-2023.4.6/jarvis/tasks/qe/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)    19582 2023-03-24 17:09:02.000000 jarvis-tools-2023.4.6/jarvis/tasks/qe/converg.py
--rw-r--r--   0 knc6     (54782) users      (100)     3665 2022-12-12 23:02:08.000000 jarvis-tools-2023.4.6/jarvis/tasks/qe/master_super.py
--rw-r--r--   0 knc6     (54782) users      (100)     3505 2023-03-24 17:09:02.000000 jarvis-tools-2023.4.6/jarvis/tasks/qe/qe.py
--rw-r--r--   0 knc6     (54782) users      (100)    10588 2023-03-24 17:09:02.000000 jarvis-tools-2023.4.6/jarvis/tasks/qe/super.py
--rw-r--r--   0 knc6     (54782) users      (100)     7387 2022-05-06 22:27:09.000000 jarvis-tools-2023.4.6/jarvis/tasks/qe/super_tetra.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:22.000000 jarvis-tools-2023.4.6/jarvis/tasks/vasp/
--rw-r--r--   0 knc6     (54782) users      (100)       61 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tasks/vasp/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)    66478 2022-08-23 21:07:21.000000 jarvis-tools-2023.4.6/jarvis/tasks/vasp/vasp.py
--rw-r--r--   0 knc6     (54782) users      (100)       47 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tasks/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     5873 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tasks/queue_jobs.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:22.000000 jarvis-tools-2023.4.6/jarvis/tests/
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:22.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:23.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/ai/
--rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/ai/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)      943 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/ai/test_ai_uncertainty.py
--rw-r--r--   0 knc6     (54782) users      (100)    67390 2021-07-23 21:33:59.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/ai/test_desc.py
--rw-r--r--   0 knc6     (54782) users      (100)     2206 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/ai/test_pkgs.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:23.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:23.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/darkmatter/
--rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/darkmatter/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)      464 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/darkmatter/test_metrics.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:23.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/defects/
--rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/defects/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)      444 2021-08-18 22:06:00.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/defects/test_subs.py
--rw-r--r--   0 knc6     (54782) users      (100)     3252 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/defects/test_surface.py
--rw-r--r--   0 knc6     (54782) users      (100)     1216 2021-07-01 05:40:26.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/defects/test_vacancy.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:23.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/elastic/
--rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/elastic/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     2577 2022-03-10 17:24:29.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/elastic/test_tensor.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:23.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/interface/
--rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:58.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/interface/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     8683 2021-07-23 21:33:59.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/interface/test_zur.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:23.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/magnetism/
--rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:58.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/magnetism/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)      589 2021-07-23 21:33:59.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/magnetism/test_magnetism.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:23.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/phonon/
--rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:58.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/phonon/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     5121 2022-08-23 21:40:41.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/phonon/test_dos.py
--rw-r--r--   0 knc6     (54782) users      (100)      326 2021-06-19 18:54:58.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/phonon/test_fc.py
--rw-r--r--   0 knc6     (54782) users      (100)     1279 2021-06-19 18:54:58.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/phonon/test_ir.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:23.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/solar/
--rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:58.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/solar/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     1397 2021-06-19 18:54:58.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/solar/test_solar.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:24.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/stm/
--rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:58.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/stm/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     1660 2022-08-28 17:53:45.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/stm/test_stm.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:24.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/structure/
--rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:58.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/structure/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)      390 2021-06-19 18:54:58.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/structure/test_energetics.py
--rw-r--r--   0 knc6     (54782) users      (100)     1301 2021-06-19 18:54:58.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/structure/test_neighbors.py
--rw-r--r--   0 knc6     (54782) users      (100)     3585 2021-06-19 18:54:58.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/structure/test_spacegroup.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:24.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/thermodynamics/
--rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:59.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/thermodynamics/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     1554 2022-08-28 17:29:20.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/thermodynamics/test_energetics.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:24.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/topological/
--rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:55:00.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/topological/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)      424 2021-06-19 18:55:00.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/topological/test_spillage.py
--rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/__init__.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:24.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/core/
--rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:55:00.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/core/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     5666 2021-07-23 21:34:05.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/core/p.py
--rw-r--r--   0 knc6     (54782) users      (100)     5483 2022-08-28 19:00:04.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/core/test_atoms.py
--rw-r--r--   0 knc6     (54782) users      (100)      262 2021-06-20 06:25:45.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/core/test_circuits.py
--rw-r--r--   0 knc6     (54782) users      (100)      481 2021-06-19 18:55:00.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/core/test_composition.py
--rw-r--r--   0 knc6     (54782) users      (100)     2844 2021-06-19 18:55:00.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/core/test_graph.py
--rw-r--r--   0 knc6     (54782) users      (100)    11116 2021-07-23 21:34:05.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/core/test_kpoints.py
--rw-r--r--   0 knc6     (54782) users      (100)     1507 2021-07-23 21:34:05.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/core/test_latice.py
--rw-r--r--   0 knc6     (54782) users      (100)      339 2021-07-13 15:03:29.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/core/test_pdb.py
--rw-r--r--   0 knc6     (54782) users      (100)      551 2021-07-01 05:40:26.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/core/test_specie.py
--rw-r--r--   0 knc6     (54782) users      (100)      541 2021-06-19 18:55:00.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/core/test_utils.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:25.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/db/
--rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:55:00.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/db/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)     1496 2021-07-23 21:34:05.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/db/test_figshare.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:25.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/tasks/
--rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:55:05.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/tasks/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)      804 2021-06-19 18:55:05.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/tasks/test_lammps.py
--rw-r--r--   0 knc6     (54782) users      (100)      696 2021-06-19 18:55:05.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/tasks/test_vasp.py
--rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tests/testfiles/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)       35 2021-06-19 18:54:57.000000 jarvis-tools-2023.4.6/jarvis/tests/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)      245 2023-04-07 04:26:33.000000 jarvis-tools-2023.4.6/jarvis/__init__.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-07 04:53:25.000000 jarvis-tools-2023.4.6/jarvis_tools.egg-info/
--rw-r--r--   0 knc6     (54782) users      (100)    18166 2023-04-07 04:53:08.000000 jarvis-tools-2023.4.6/jarvis_tools.egg-info/PKG-INFO
--rw-r--r--   0 knc6     (54782) users      (100)     7499 2023-04-07 04:53:09.000000 jarvis-tools-2023.4.6/jarvis_tools.egg-info/SOURCES.txt
--rw-r--r--   0 knc6     (54782) users      (100)        1 2023-04-07 04:53:08.000000 jarvis-tools-2023.4.6/jarvis_tools.egg-info/dependency_links.txt
--rw-r--r--   0 knc6     (54782) users      (100)      265 2023-04-07 04:53:08.000000 jarvis-tools-2023.4.6/jarvis_tools.egg-info/requires.txt
--rw-r--r--   0 knc6     (54782) users      (100)        7 2023-04-07 04:53:08.000000 jarvis-tools-2023.4.6/jarvis_tools.egg-info/top_level.txt
--rw-r--r--   0 knc6     (54782) users      (100)    14481 2023-04-07 04:25:58.000000 jarvis-tools-2023.4.6/README.rst
--rw-r--r--   0 knc6     (54782) users      (100)      195 2023-04-07 04:53:25.000000 jarvis-tools-2023.4.6/setup.cfg
--rw-r--r--   0 knc6     (54782) users      (100)     2502 2023-04-07 04:26:18.000000 jarvis-tools-2023.4.6/setup.py
--rw-r--r--   0 knc6     (54782) users      (100)    18166 2023-04-07 04:53:25.000000 jarvis-tools-2023.4.6/PKG-INFO
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:07.000000 jarvis-tools-2023.5.26/
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:51.000000 jarvis-tools-2023.5.26/jarvis/
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:51.000000 jarvis-tools-2023.5.26/jarvis/ai/
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:52.000000 jarvis-tools-2023.5.26/jarvis/ai/descriptors/
+-rw-r--r--   0 knc6     (54782) users      (100)       48 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/ai/descriptors/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)    48400 2023-03-24 19:10:21.000000 jarvis-tools-2023.5.26/jarvis/ai/descriptors/cfid.py
+-rw-r--r--   0 knc6     (54782) users      (100)     1370 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/ai/descriptors/coulomb.py
+-rw-r--r--   0 knc6     (54782) users      (100)      511 2022-05-21 15:06:08.000000 jarvis-tools-2023.5.26/jarvis/ai/descriptors/elemental.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:52.000000 jarvis-tools-2023.5.26/jarvis/ai/gcn/
+-rw-r--r--   0 knc6     (54782) users      (100)       47 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/ai/gcn/__init__.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:52.000000 jarvis-tools-2023.5.26/jarvis/ai/pkgs/
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:52.000000 jarvis-tools-2023.5.26/jarvis/ai/pkgs/lgbm/
+-rw-r--r--   0 knc6     (54782) users      (100)       28 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/ai/pkgs/lgbm/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     1148 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/ai/pkgs/lgbm/classification.py
+-rw-r--r--   0 knc6     (54782) users      (100)     9541 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/ai/pkgs/lgbm/regression.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:52.000000 jarvis-tools-2023.5.26/jarvis/ai/pkgs/sklearn/
+-rw-r--r--   0 knc6     (54782) users      (100)       44 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/ai/pkgs/sklearn/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     5144 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/ai/pkgs/sklearn/classification.py
+-rw-r--r--   0 knc6     (54782) users      (100)    11368 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/ai/pkgs/sklearn/hyper_params.py
+-rw-r--r--   0 knc6     (54782) users      (100)     2969 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/ai/pkgs/sklearn/regression.py
+-rw-r--r--   0 knc6     (54782) users      (100)       35 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/ai/pkgs/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     3585 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/ai/pkgs/utils.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:52.000000 jarvis-tools-2023.5.26/jarvis/ai/uncertainty/
+-rw-r--r--   0 knc6     (54782) users      (100)       34 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/ai/uncertainty/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     7487 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/ai/uncertainty/lgbm_quantile_uncertainty.py
+-rw-r--r--   0 knc6     (54782) users      (100)       35 2021-06-19 18:54:48.000000 jarvis-tools-2023.5.26/jarvis/ai/__init__.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:52.000000 jarvis-tools-2023.5.26/jarvis/analysis/
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:52.000000 jarvis-tools-2023.5.26/jarvis/analysis/darkmatter/
+-rw-r--r--   0 knc6     (54782) users      (100)       51 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/analysis/darkmatter/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)      786 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/analysis/darkmatter/metrics.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:53.000000 jarvis-tools-2023.5.26/jarvis/analysis/defects/
+-rw-r--r--   0 knc6     (54782) users      (100)       47 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/analysis/defects/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     2328 2021-08-18 22:05:59.000000 jarvis-tools-2023.5.26/jarvis/analysis/defects/substitutions.py
+-rw-r--r--   0 knc6     (54782) users      (100)     9305 2021-07-23 21:33:58.000000 jarvis-tools-2023.5.26/jarvis/analysis/defects/surface.py
+-rw-r--r--   0 knc6     (54782) users      (100)     5048 2022-05-21 15:07:48.000000 jarvis-tools-2023.5.26/jarvis/analysis/defects/vacancy.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:53.000000 jarvis-tools-2023.5.26/jarvis/analysis/diffraction/
+-rw-r--r--   0 knc6     (54782) users      (100)       49 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/analysis/diffraction/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     6825 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/analysis/diffraction/atomic_scattering_params.json
+-rw-r--r--   0 knc6     (54782) users      (100)     7327 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/analysis/diffraction/xrd.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:53.000000 jarvis-tools-2023.5.26/jarvis/analysis/elastic/
+-rw-r--r--   0 knc6     (54782) users      (100)       43 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/analysis/elastic/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     6602 2022-05-06 22:27:09.000000 jarvis-tools-2023.5.26/jarvis/analysis/elastic/tensor.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:53.000000 jarvis-tools-2023.5.26/jarvis/analysis/interface/
+-rw-r--r--   0 knc6     (54782) users      (100)       53 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/analysis/interface/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)    14764 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/analysis/interface/zur.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:53.000000 jarvis-tools-2023.5.26/jarvis/analysis/magnetism/
+-rw-r--r--   0 knc6     (54782) users      (100)       46 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/analysis/magnetism/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     8101 2021-06-19 18:54:50.000000 jarvis-tools-2023.5.26/jarvis/analysis/magnetism/magmom_setup.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:54.000000 jarvis-tools-2023.5.26/jarvis/analysis/periodic/
+-rw-r--r--   0 knc6     (54782) users      (100)       49 2021-06-19 18:54:50.000000 jarvis-tools-2023.5.26/jarvis/analysis/periodic/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     5907 2021-06-19 18:54:50.000000 jarvis-tools-2023.5.26/jarvis/analysis/periodic/ptable.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:54.000000 jarvis-tools-2023.5.26/jarvis/analysis/phonon/
+-rw-r--r--   0 knc6     (54782) users      (100)       49 2021-06-19 18:54:50.000000 jarvis-tools-2023.5.26/jarvis/analysis/phonon/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     3934 2022-12-06 20:07:55.000000 jarvis-tools-2023.5.26/jarvis/analysis/phonon/dos.py
+-rw-r--r--   0 knc6     (54782) users      (100)     1189 2021-06-19 18:54:50.000000 jarvis-tools-2023.5.26/jarvis/analysis/phonon/force_constants.py
+-rw-r--r--   0 knc6     (54782) users      (100)     6473 2023-01-09 20:58:01.000000 jarvis-tools-2023.5.26/jarvis/analysis/phonon/ir.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:54.000000 jarvis-tools-2023.5.26/jarvis/analysis/solarefficiency/
+-rw-r--r--   0 knc6     (54782) users      (100)       59 2021-06-19 18:54:50.000000 jarvis-tools-2023.5.26/jarvis/analysis/solarefficiency/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)    35436 2021-06-19 18:54:50.000000 jarvis-tools-2023.5.26/jarvis/analysis/solarefficiency/am1.5G.dat
+-rw-r--r--   0 knc6     (54782) users      (100)    14217 2021-06-19 18:54:50.000000 jarvis-tools-2023.5.26/jarvis/analysis/solarefficiency/solar.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:54.000000 jarvis-tools-2023.5.26/jarvis/analysis/stem/
+-rw-r--r--   0 knc6     (54782) users      (100)       38 2021-06-19 18:54:50.000000 jarvis-tools-2023.5.26/jarvis/analysis/stem/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     7315 2022-05-21 15:11:22.000000 jarvis-tools-2023.5.26/jarvis/analysis/stem/convolution_apprx.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:54.000000 jarvis-tools-2023.5.26/jarvis/analysis/stm/
+-rw-r--r--   0 knc6     (54782) users      (100)       67 2021-06-19 18:54:50.000000 jarvis-tools-2023.5.26/jarvis/analysis/stm/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)    10094 2021-07-01 05:40:25.000000 jarvis-tools-2023.5.26/jarvis/analysis/stm/tersoff_hamann.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:57.000000 jarvis-tools-2023.5.26/jarvis/analysis/structure/
+-rw-r--r--   0 knc6     (54782) users      (100)       46 2021-06-19 18:54:50.000000 jarvis-tools-2023.5.26/jarvis/analysis/structure/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)    21798 2021-06-19 18:54:50.000000 jarvis-tools-2023.5.26/jarvis/analysis/structure/neighbors.py
+-rw-r--r--   0 knc6     (54782) users      (100)    25663 2021-12-17 15:03:20.000000 jarvis-tools-2023.5.26/jarvis/analysis/structure/spacegroup.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:57.000000 jarvis-tools-2023.5.26/jarvis/analysis/thermodynamics/
+-rw-r--r--   0 knc6     (54782) users      (100)       42 2021-06-19 18:54:50.000000 jarvis-tools-2023.5.26/jarvis/analysis/thermodynamics/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)    14613 2023-04-07 04:22:25.000000 jarvis-tools-2023.5.26/jarvis/analysis/thermodynamics/energetics.py
+-rw-r--r--   0 knc6     (54782) users      (100)     4527 2021-06-19 18:54:50.000000 jarvis-tools-2023.5.26/jarvis/analysis/thermodynamics/unary.json
+-rw-r--r--   0 knc6     (54782) users      (100)     4781 2021-06-21 21:20:14.000000 jarvis-tools-2023.5.26/jarvis/analysis/thermodynamics/unary_qe_tb.json
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:57.000000 jarvis-tools-2023.5.26/jarvis/analysis/topological/
+-rw-r--r--   0 knc6     (54782) users      (100)       50 2021-06-19 18:54:50.000000 jarvis-tools-2023.5.26/jarvis/analysis/topological/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)    11892 2021-06-19 18:54:50.000000 jarvis-tools-2023.5.26/jarvis/analysis/topological/spillage.py
+-rw-r--r--   0 knc6     (54782) users      (100)       35 2021-06-19 18:54:49.000000 jarvis-tools-2023.5.26/jarvis/analysis/__init__.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:59.000000 jarvis-tools-2023.5.26/jarvis/core/
+-rw-r--r--   0 knc6     (54782) users      (100)  1421253 2021-06-19 18:54:50.000000 jarvis-tools-2023.5.26/jarvis/core/Elements.json
+-rw-r--r--   0 knc6     (54782) users      (100)       49 2021-06-19 18:54:51.000000 jarvis-tools-2023.5.26/jarvis/core/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)    28393 2021-06-19 18:54:51.000000 jarvis-tools-2023.5.26/jarvis/core/atom_init.json
+-rw-r--r--   0 knc6     (54782) users      (100)    66720 2022-08-28 18:59:14.000000 jarvis-tools-2023.5.26/jarvis/core/atoms.py
+-rw-r--r--   0 knc6     (54782) users      (100)     4313 2022-05-21 15:13:20.000000 jarvis-tools-2023.5.26/jarvis/core/circuits.py
+-rw-r--r--   0 knc6     (54782) users      (100)     5258 2021-07-06 06:09:50.000000 jarvis-tools-2023.5.26/jarvis/core/composition.py
+-rw-r--r--   0 knc6     (54782) users      (100)  1162701 2021-06-19 18:54:51.000000 jarvis-tools-2023.5.26/jarvis/core/element_charge.json
+-rw-r--r--   0 knc6     (54782) users      (100)    22721 2022-07-18 17:09:48.000000 jarvis-tools-2023.5.26/jarvis/core/graphs.py
+-rw-r--r--   0 knc6     (54782) users      (100)    10693 2022-08-28 18:10:43.000000 jarvis-tools-2023.5.26/jarvis/core/image.py
+-rw-r--r--   0 knc6     (54782) users      (100)    37783 2021-10-05 17:33:43.000000 jarvis-tools-2023.5.26/jarvis/core/kpoints.py
+-rw-r--r--   0 knc6     (54782) users      (100)    17427 2023-01-09 20:58:01.000000 jarvis-tools-2023.5.26/jarvis/core/lattice.py
+-rw-r--r--   0 knc6     (54782) users      (100)    47766 2021-07-23 21:33:59.000000 jarvis-tools-2023.5.26/jarvis/core/magpie.json
+-rw-r--r--   0 knc6     (54782) users      (100)    11981 2021-07-23 21:33:59.000000 jarvis-tools-2023.5.26/jarvis/core/specie.py
+-rw-r--r--   0 knc6     (54782) users      (100)     2891 2023-01-09 20:58:01.000000 jarvis-tools-2023.5.26/jarvis/core/spectrum.py
+-rw-r--r--   0 knc6     (54782) users      (100)     8933 2022-02-24 23:02:40.000000 jarvis-tools-2023.5.26/jarvis/core/utils.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:59.000000 jarvis-tools-2023.5.26/jarvis/db/
+-rw-r--r--   0 knc6     (54782) users      (100)       53 2021-06-19 18:54:52.000000 jarvis-tools-2023.5.26/jarvis/db/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)    24550 2023-05-29 02:42:07.000000 jarvis-tools-2023.5.26/jarvis/db/figshare.py
+-rw-r--r--   0 knc6     (54782) users      (100)      378 2021-06-19 18:54:52.000000 jarvis-tools-2023.5.26/jarvis/db/jsonutils.py
+-rw-r--r--   0 knc6     (54782) users      (100)     7761 2021-06-20 06:25:45.000000 jarvis-tools-2023.5.26/jarvis/db/lammps_to_xml.py
+-rw-r--r--   0 knc6     (54782) users      (100)    10649 2021-06-19 18:54:52.000000 jarvis-tools-2023.5.26/jarvis/db/qe_to_xml.py
+-rw-r--r--   0 knc6     (54782) users      (100)    16857 2021-06-19 18:54:52.000000 jarvis-tools-2023.5.26/jarvis/db/restapi.py
+-rw-r--r--   0 knc6     (54782) users      (100)    75218 2021-06-19 18:54:52.000000 jarvis-tools-2023.5.26/jarvis/db/vasp_to_xml.py
+-rw-r--r--   0 knc6     (54782) users      (100)     9586 2021-06-19 18:54:52.000000 jarvis-tools-2023.5.26/jarvis/db/webpages.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:59.000000 jarvis-tools-2023.5.26/jarvis/io/
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:52:59.000000 jarvis-tools-2023.5.26/jarvis/io/boltztrap/
+-rw-r--r--   0 knc6     (54782) users      (100)       67 2021-06-19 18:54:55.000000 jarvis-tools-2023.5.26/jarvis/io/boltztrap/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     6511 2021-06-19 18:54:55.000000 jarvis-tools-2023.5.26/jarvis/io/boltztrap/inputs.py
+-rw-r--r--   0 knc6     (54782) users      (100)     6767 2021-06-19 18:54:55.000000 jarvis-tools-2023.5.26/jarvis/io/boltztrap/outputs.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:01.000000 jarvis-tools-2023.5.26/jarvis/io/calphad/
+-rw-r--r--   0 knc6     (54782) users      (100)       61 2021-06-19 18:54:55.000000 jarvis-tools-2023.5.26/jarvis/io/calphad/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     4228 2021-06-19 18:54:56.000000 jarvis-tools-2023.5.26/jarvis/io/calphad/write_decorated_poscar.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:01.000000 jarvis-tools-2023.5.26/jarvis/io/lammps/
+-rw-r--r--   0 knc6     (54782) users      (100)       52 2021-06-19 18:54:56.000000 jarvis-tools-2023.5.26/jarvis/io/lammps/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)    14622 2021-08-06 21:54:48.000000 jarvis-tools-2023.5.26/jarvis/io/lammps/inputs.py
+-rw-r--r--   0 knc6     (54782) users      (100)    20748 2021-08-06 21:54:48.000000 jarvis-tools-2023.5.26/jarvis/io/lammps/outputs.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:01.000000 jarvis-tools-2023.5.26/jarvis/io/nexus/
+-rw-r--r--   0 knc6     (54782) users      (100)       47 2021-09-28 18:06:38.000000 jarvis-tools-2023.5.26/jarvis/io/nexus/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     4519 2022-12-07 19:52:37.000000 jarvis-tools-2023.5.26/jarvis/io/nexus/inputs.py
+-rw-r--r--   0 knc6     (54782) users      (100)       36 2021-09-28 18:06:38.000000 jarvis-tools-2023.5.26/jarvis/io/nexus/outputs.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:01.000000 jarvis-tools-2023.5.26/jarvis/io/pennylane/
+-rw-r--r--   0 knc6     (54782) users      (100)       61 2021-06-19 18:54:56.000000 jarvis-tools-2023.5.26/jarvis/io/pennylane/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     2196 2021-06-19 18:54:56.000000 jarvis-tools-2023.5.26/jarvis/io/pennylane/inputs.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:01.000000 jarvis-tools-2023.5.26/jarvis/io/phonopy/
+-rw-r--r--   0 knc6     (54782) users      (100)       43 2021-06-19 18:54:56.000000 jarvis-tools-2023.5.26/jarvis/io/phonopy/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     4501 2023-01-09 20:58:01.000000 jarvis-tools-2023.5.26/jarvis/io/phonopy/fcmat2hr.py
+-rw-r--r--   0 knc6     (54782) users      (100)     6844 2023-01-09 20:58:01.000000 jarvis-tools-2023.5.26/jarvis/io/phonopy/inputs.py
+-rw-r--r--   0 knc6     (54782) users      (100)     5696 2021-06-19 18:55:19.000000 jarvis-tools-2023.5.26/jarvis/io/phonopy/outputs.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:02.000000 jarvis-tools-2023.5.26/jarvis/io/prismatic/
+-rw-r--r--   0 knc6     (54782) users      (100)       50 2021-06-19 18:54:56.000000 jarvis-tools-2023.5.26/jarvis/io/prismatic/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)      674 2021-06-19 18:54:56.000000 jarvis-tools-2023.5.26/jarvis/io/prismatic/inputs.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:02.000000 jarvis-tools-2023.5.26/jarvis/io/qe/
+-rw-r--r--   0 knc6     (54782) users      (100)       57 2021-06-19 18:54:56.000000 jarvis-tools-2023.5.26/jarvis/io/qe/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)    15328 2023-03-24 17:09:02.000000 jarvis-tools-2023.5.26/jarvis/io/qe/inputs.py
+-rwxr-xr-x   0 knc6     (54782) users      (100)    26674 2022-05-21 15:16:55.000000 jarvis-tools-2023.5.26/jarvis/io/qe/outputs.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:02.000000 jarvis-tools-2023.5.26/jarvis/io/qiskit/
+-rw-r--r--   0 knc6     (54782) users      (100)       56 2021-06-19 18:54:56.000000 jarvis-tools-2023.5.26/jarvis/io/qiskit/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)    12100 2022-09-17 18:37:16.000000 jarvis-tools-2023.5.26/jarvis/io/qiskit/inputs.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:02.000000 jarvis-tools-2023.5.26/jarvis/io/tequila/
+-rw-r--r--   0 knc6     (54782) users      (100)       60 2021-06-19 18:54:56.000000 jarvis-tools-2023.5.26/jarvis/io/tequila/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     2702 2021-06-19 18:54:56.000000 jarvis-tools-2023.5.26/jarvis/io/tequila/inputs.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:03.000000 jarvis-tools-2023.5.26/jarvis/io/vasp/
+-rw-r--r--   0 knc6     (54782) users      (100)       56 2021-06-19 18:54:56.000000 jarvis-tools-2023.5.26/jarvis/io/vasp/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     1522 2021-06-19 18:54:56.000000 jarvis-tools-2023.5.26/jarvis/io/vasp/default_potcars.json
+-rw-r--r--   0 knc6     (54782) users      (100)    21148 2022-07-18 17:07:16.000000 jarvis-tools-2023.5.26/jarvis/io/vasp/inputs.py
+-rw-r--r--   0 knc6     (54782) users      (100)    77837 2022-07-18 17:08:30.000000 jarvis-tools-2023.5.26/jarvis/io/vasp/outputs.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:03.000000 jarvis-tools-2023.5.26/jarvis/io/wannier/
+-rw-r--r--   0 knc6     (54782) users      (100)       61 2021-06-19 18:54:56.000000 jarvis-tools-2023.5.26/jarvis/io/wannier/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     4550 2021-06-19 18:55:19.000000 jarvis-tools-2023.5.26/jarvis/io/wannier/default_semicore.json
+-rw-r--r--   0 knc6     (54782) users      (100)     6929 2021-06-19 18:55:19.000000 jarvis-tools-2023.5.26/jarvis/io/wannier/inputs.py
+-rw-r--r--   0 knc6     (54782) users      (100)    34195 2021-06-19 18:54:56.000000 jarvis-tools-2023.5.26/jarvis/io/wannier/outputs.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:03.000000 jarvis-tools-2023.5.26/jarvis/io/wanniertools/
+-rw-r--r--   0 knc6     (54782) users      (100)       60 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/io/wanniertools/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)    10376 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/io/wanniertools/inputs.py
+-rw-r--r--   0 knc6     (54782) users      (100)     3818 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/io/wanniertools/outputs.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:03.000000 jarvis-tools-2023.5.26/jarvis/io/wien2k/
+-rw-r--r--   0 knc6     (54782) users      (100)       55 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/io/wien2k/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     3192 2021-12-17 15:03:19.000000 jarvis-tools-2023.5.26/jarvis/io/wien2k/inputs.py
+-rw-r--r--   0 knc6     (54782) users      (100)     3254 2021-07-23 21:33:59.000000 jarvis-tools-2023.5.26/jarvis/io/wien2k/outputs.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:03.000000 jarvis-tools-2023.5.26/jarvis/io/zeopp/
+-rw-r--r--   0 knc6     (54782) users      (100)       35 2021-07-01 05:40:26.000000 jarvis-tools-2023.5.26/jarvis/io/zeopp/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     2184 2021-10-14 00:41:09.000000 jarvis-tools-2023.5.26/jarvis/io/zeopp/inputs.py
+-rw-r--r--   0 knc6     (54782) users      (100)       76 2021-06-19 18:54:55.000000 jarvis-tools-2023.5.26/jarvis/io/__init__.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:04.000000 jarvis-tools-2023.5.26/jarvis/tasks/
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:04.000000 jarvis-tools-2023.5.26/jarvis/tasks/boltztrap/
+-rw-r--r--   0 knc6     (54782) users      (100)       56 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tasks/boltztrap/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)      608 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tasks/boltztrap/run.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:04.000000 jarvis-tools-2023.5.26/jarvis/tasks/lammps/
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:04.000000 jarvis-tools-2023.5.26/jarvis/tasks/lammps/templates/
+-rw-r--r--   0 knc6     (54782) users      (100)       47 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tasks/lammps/templates/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     3463 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tasks/lammps/templates/displace.mod
+-rw-r--r--   0 knc6     (54782) users      (100)     6416 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tasks/lammps/templates/inelast.mod
+-rw-r--r--   0 knc6     (54782) users      (100)     6449 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tasks/lammps/templates/inelast_min.mod
+-rw-r--r--   0 knc6     (54782) users      (100)     6418 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tasks/lammps/templates/inelast_nobox.mod
+-rw-r--r--   0 knc6     (54782) users      (100)     6415 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tasks/lammps/templates/inelastcomb.mod
+-rw-r--r--   0 knc6     (54782) users      (100)     6389 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tasks/lammps/templates/inelastreax.mod
+-rw-r--r--   0 knc6     (54782) users      (100)     2653 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tasks/lammps/templates/relax.mod
+-rw-r--r--   0 knc6     (54782) users      (100)      145 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tasks/lammps/templates/run0.mod
+-rw-r--r--   0 knc6     (54782) users      (100)      917 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tasks/lammps/templates/templates.py
+-rw-r--r--   0 knc6     (54782) users      (100)       55 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tasks/lammps/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)    13948 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tasks/lammps/lammps.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:04.000000 jarvis-tools-2023.5.26/jarvis/tasks/nexus/
+-rw-r--r--   0 knc6     (54782) users      (100)       34 2022-12-07 20:41:49.000000 jarvis-tools-2023.5.26/jarvis/tasks/nexus/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     3243 2022-12-12 23:19:44.000000 jarvis-tools-2023.5.26/jarvis/tasks/nexus/qmc.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:04.000000 jarvis-tools-2023.5.26/jarvis/tasks/phonopy/
+-rw-r--r--   0 knc6     (54782) users      (100)       54 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tasks/phonopy/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)      765 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tasks/phonopy/run.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:04.000000 jarvis-tools-2023.5.26/jarvis/tasks/qe/
+-rw-r--r--   0 knc6     (54782) users      (100)       29 2022-01-11 17:34:47.000000 jarvis-tools-2023.5.26/jarvis/tasks/qe/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)    19582 2023-03-24 17:09:02.000000 jarvis-tools-2023.5.26/jarvis/tasks/qe/converg.py
+-rw-r--r--   0 knc6     (54782) users      (100)     3665 2022-12-12 23:02:08.000000 jarvis-tools-2023.5.26/jarvis/tasks/qe/master_super.py
+-rw-r--r--   0 knc6     (54782) users      (100)     3505 2023-03-24 17:09:02.000000 jarvis-tools-2023.5.26/jarvis/tasks/qe/qe.py
+-rw-r--r--   0 knc6     (54782) users      (100)    10588 2023-03-24 17:09:02.000000 jarvis-tools-2023.5.26/jarvis/tasks/qe/super.py
+-rw-r--r--   0 knc6     (54782) users      (100)     7387 2022-05-06 22:27:09.000000 jarvis-tools-2023.5.26/jarvis/tasks/qe/super_tetra.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:05.000000 jarvis-tools-2023.5.26/jarvis/tasks/vasp/
+-rw-r--r--   0 knc6     (54782) users      (100)       61 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tasks/vasp/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)    66478 2022-08-23 21:07:21.000000 jarvis-tools-2023.5.26/jarvis/tasks/vasp/vasp.py
+-rw-r--r--   0 knc6     (54782) users      (100)       47 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tasks/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     5873 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tasks/queue_jobs.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:05.000000 jarvis-tools-2023.5.26/jarvis/tests/
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:05.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:05.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/ai/
+-rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/ai/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)      943 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/ai/test_ai_uncertainty.py
+-rw-r--r--   0 knc6     (54782) users      (100)    67390 2021-07-23 21:33:59.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/ai/test_desc.py
+-rw-r--r--   0 knc6     (54782) users      (100)     2206 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/ai/test_pkgs.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:05.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:05.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/darkmatter/
+-rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/darkmatter/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)      464 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/darkmatter/test_metrics.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:05.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/defects/
+-rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/defects/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)      444 2021-08-18 22:06:00.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/defects/test_subs.py
+-rw-r--r--   0 knc6     (54782) users      (100)     3252 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/defects/test_surface.py
+-rw-r--r--   0 knc6     (54782) users      (100)     1216 2021-07-01 05:40:26.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/defects/test_vacancy.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:05.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/elastic/
+-rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/elastic/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     2577 2022-03-10 17:24:29.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/elastic/test_tensor.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:05.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/interface/
+-rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:58.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/interface/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     8683 2021-07-23 21:33:59.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/interface/test_zur.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:05.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/magnetism/
+-rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:58.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/magnetism/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)      589 2021-07-23 21:33:59.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/magnetism/test_magnetism.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:06.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/phonon/
+-rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:58.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/phonon/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     5121 2022-08-23 21:40:41.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/phonon/test_dos.py
+-rw-r--r--   0 knc6     (54782) users      (100)      326 2021-06-19 18:54:58.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/phonon/test_fc.py
+-rw-r--r--   0 knc6     (54782) users      (100)     1279 2021-06-19 18:54:58.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/phonon/test_ir.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:06.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/solar/
+-rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:58.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/solar/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     1397 2021-06-19 18:54:58.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/solar/test_solar.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:06.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/stm/
+-rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:58.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/stm/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     1660 2022-08-28 17:53:45.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/stm/test_stm.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:06.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/structure/
+-rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:58.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/structure/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)      390 2021-06-19 18:54:58.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/structure/test_energetics.py
+-rw-r--r--   0 knc6     (54782) users      (100)     1301 2021-06-19 18:54:58.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/structure/test_neighbors.py
+-rw-r--r--   0 knc6     (54782) users      (100)     3585 2021-06-19 18:54:58.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/structure/test_spacegroup.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:06.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/thermodynamics/
+-rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:59.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/thermodynamics/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     1554 2022-08-28 17:29:20.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/thermodynamics/test_energetics.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:06.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/topological/
+-rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:55:00.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/topological/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)      424 2021-06-19 18:55:00.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/topological/test_spillage.py
+-rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/__init__.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:07.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/core/
+-rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:55:00.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/core/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     5666 2021-07-23 21:34:05.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/core/p.py
+-rw-r--r--   0 knc6     (54782) users      (100)     5483 2022-08-28 19:00:04.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/core/test_atoms.py
+-rw-r--r--   0 knc6     (54782) users      (100)      262 2021-06-20 06:25:45.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/core/test_circuits.py
+-rw-r--r--   0 knc6     (54782) users      (100)      481 2021-06-19 18:55:00.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/core/test_composition.py
+-rw-r--r--   0 knc6     (54782) users      (100)     2844 2021-06-19 18:55:00.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/core/test_graph.py
+-rw-r--r--   0 knc6     (54782) users      (100)    11116 2021-07-23 21:34:05.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/core/test_kpoints.py
+-rw-r--r--   0 knc6     (54782) users      (100)     1507 2021-07-23 21:34:05.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/core/test_latice.py
+-rw-r--r--   0 knc6     (54782) users      (100)      339 2021-07-13 15:03:29.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/core/test_pdb.py
+-rw-r--r--   0 knc6     (54782) users      (100)      551 2021-07-01 05:40:26.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/core/test_specie.py
+-rw-r--r--   0 knc6     (54782) users      (100)      541 2021-06-19 18:55:00.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/core/test_utils.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:07.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/db/
+-rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:55:00.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/db/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)     1496 2021-07-23 21:34:05.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/db/test_figshare.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:07.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/tasks/
+-rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:55:05.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/tasks/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)      804 2021-06-19 18:55:05.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/tasks/test_lammps.py
+-rw-r--r--   0 knc6     (54782) users      (100)      696 2021-06-19 18:55:05.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/tasks/test_vasp.py
+-rw-r--r--   0 knc6     (54782) users      (100)        0 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tests/testfiles/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)       35 2021-06-19 18:54:57.000000 jarvis-tools-2023.5.26/jarvis/tests/__init__.py
+-rw-r--r--   0 knc6     (54782) users      (100)      245 2023-05-29 03:53:38.000000 jarvis-tools-2023.5.26/jarvis/__init__.py
+drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-05-29 12:53:07.000000 jarvis-tools-2023.5.26/jarvis_tools.egg-info/
+-rw-r--r--   0 knc6     (54782) users      (100)    18167 2023-05-29 12:52:47.000000 jarvis-tools-2023.5.26/jarvis_tools.egg-info/PKG-INFO
+-rw-r--r--   0 knc6     (54782) users      (100)     7499 2023-05-29 12:52:48.000000 jarvis-tools-2023.5.26/jarvis_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 knc6     (54782) users      (100)        1 2023-05-29 12:52:47.000000 jarvis-tools-2023.5.26/jarvis_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 knc6     (54782) users      (100)      265 2023-05-29 12:52:47.000000 jarvis-tools-2023.5.26/jarvis_tools.egg-info/requires.txt
+-rw-r--r--   0 knc6     (54782) users      (100)        7 2023-05-29 12:52:47.000000 jarvis-tools-2023.5.26/jarvis_tools.egg-info/top_level.txt
+-rw-r--r--   0 knc6     (54782) users      (100)    14481 2023-04-07 04:25:58.000000 jarvis-tools-2023.5.26/README.rst
+-rw-r--r--   0 knc6     (54782) users      (100)      195 2023-05-29 12:53:07.000000 jarvis-tools-2023.5.26/setup.cfg
+-rw-r--r--   0 knc6     (54782) users      (100)     2502 2023-05-29 03:53:22.000000 jarvis-tools-2023.5.26/setup.py
+-rw-r--r--   0 knc6     (54782) users      (100)    18167 2023-05-29 12:53:07.000000 jarvis-tools-2023.5.26/PKG-INFO
```

### Comparing `jarvis-tools-2023.4.6/jarvis/ai/descriptors/cfid.py` & `jarvis-tools-2023.5.26/jarvis/ai/descriptors/cfid.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/ai/descriptors/coulomb.py` & `jarvis-tools-2023.5.26/jarvis/ai/descriptors/coulomb.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/ai/pkgs/lgbm/classification.py` & `jarvis-tools-2023.5.26/jarvis/ai/pkgs/lgbm/classification.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/ai/pkgs/lgbm/regression.py` & `jarvis-tools-2023.5.26/jarvis/ai/pkgs/lgbm/regression.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/ai/pkgs/sklearn/classification.py` & `jarvis-tools-2023.5.26/jarvis/ai/pkgs/sklearn/classification.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/ai/pkgs/sklearn/hyper_params.py` & `jarvis-tools-2023.5.26/jarvis/ai/pkgs/sklearn/hyper_params.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/ai/pkgs/sklearn/regression.py` & `jarvis-tools-2023.5.26/jarvis/ai/pkgs/sklearn/regression.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/ai/pkgs/utils.py` & `jarvis-tools-2023.5.26/jarvis/ai/pkgs/utils.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/ai/uncertainty/lgbm_quantile_uncertainty.py` & `jarvis-tools-2023.5.26/jarvis/ai/uncertainty/lgbm_quantile_uncertainty.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/darkmatter/metrics.py` & `jarvis-tools-2023.5.26/jarvis/analysis/darkmatter/metrics.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/defects/substitutions.py` & `jarvis-tools-2023.5.26/jarvis/analysis/defects/substitutions.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/defects/surface.py` & `jarvis-tools-2023.5.26/jarvis/analysis/defects/surface.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/defects/vacancy.py` & `jarvis-tools-2023.5.26/jarvis/analysis/defects/vacancy.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/diffraction/atomic_scattering_params.json` & `jarvis-tools-2023.5.26/jarvis/analysis/diffraction/atomic_scattering_params.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/diffraction/xrd.py` & `jarvis-tools-2023.5.26/jarvis/analysis/diffraction/xrd.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/elastic/tensor.py` & `jarvis-tools-2023.5.26/jarvis/analysis/elastic/tensor.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/interface/zur.py` & `jarvis-tools-2023.5.26/jarvis/analysis/interface/zur.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/magnetism/magmom_setup.py` & `jarvis-tools-2023.5.26/jarvis/analysis/magnetism/magmom_setup.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/periodic/ptable.py` & `jarvis-tools-2023.5.26/jarvis/analysis/periodic/ptable.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/phonon/dos.py` & `jarvis-tools-2023.5.26/jarvis/analysis/phonon/dos.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/phonon/force_constants.py` & `jarvis-tools-2023.5.26/jarvis/analysis/phonon/force_constants.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/phonon/ir.py` & `jarvis-tools-2023.5.26/jarvis/analysis/phonon/ir.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/solarefficiency/am1.5G.dat` & `jarvis-tools-2023.5.26/jarvis/analysis/solarefficiency/am1.5G.dat`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/solarefficiency/solar.py` & `jarvis-tools-2023.5.26/jarvis/analysis/solarefficiency/solar.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/stem/convolution_apprx.py` & `jarvis-tools-2023.5.26/jarvis/analysis/stem/convolution_apprx.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/stm/tersoff_hamann.py` & `jarvis-tools-2023.5.26/jarvis/analysis/stm/tersoff_hamann.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/structure/neighbors.py` & `jarvis-tools-2023.5.26/jarvis/analysis/structure/neighbors.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/structure/spacegroup.py` & `jarvis-tools-2023.5.26/jarvis/analysis/structure/spacegroup.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/thermodynamics/energetics.py` & `jarvis-tools-2023.5.26/jarvis/analysis/thermodynamics/energetics.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/thermodynamics/unary.json` & `jarvis-tools-2023.5.26/jarvis/analysis/thermodynamics/unary.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/thermodynamics/unary_qe_tb.json` & `jarvis-tools-2023.5.26/jarvis/analysis/thermodynamics/unary_qe_tb.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/analysis/topological/spillage.py` & `jarvis-tools-2023.5.26/jarvis/analysis/topological/spillage.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/core/Elements.json` & `jarvis-tools-2023.5.26/jarvis/core/Elements.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/core/atom_init.json` & `jarvis-tools-2023.5.26/jarvis/core/atom_init.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/core/atoms.py` & `jarvis-tools-2023.5.26/jarvis/core/atoms.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/core/circuits.py` & `jarvis-tools-2023.5.26/jarvis/core/circuits.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/core/composition.py` & `jarvis-tools-2023.5.26/jarvis/core/composition.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/core/element_charge.json` & `jarvis-tools-2023.5.26/jarvis/core/element_charge.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/core/graphs.py` & `jarvis-tools-2023.5.26/jarvis/core/graphs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/core/image.py` & `jarvis-tools-2023.5.26/jarvis/core/image.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/core/kpoints.py` & `jarvis-tools-2023.5.26/jarvis/core/kpoints.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/core/lattice.py` & `jarvis-tools-2023.5.26/jarvis/core/lattice.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/core/magpie.json` & `jarvis-tools-2023.5.26/jarvis/core/magpie.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/core/specie.py` & `jarvis-tools-2023.5.26/jarvis/core/specie.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/core/spectrum.py` & `jarvis-tools-2023.5.26/jarvis/core/spectrum.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/core/utils.py` & `jarvis-tools-2023.5.26/jarvis/core/utils.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/db/figshare.py` & `jarvis-tools-2023.5.26/jarvis/db/figshare.py`

 * *Files 13% similar despite different names*

```diff
@@ -252,14 +252,129 @@
         # https://doi.org/10.6084/m9.figshare.14211857
         "cord19": [
             "https://ndownloader.figshare.com/files/26804798",
             "cord19.json",
             "Obtaining CORD19 dataset 223k...",
             "https://github.com/usnistgov/cord19-cdcs-nist",
         ],
+        # https://doi.org/10.6084/m9.figshare.22583677
+        "ssub": [
+            "https://figshare.com/ndownloader/files/40084921",
+            "ssub.json",
+            "Obtaining SSUB dataset 1726...",
+            "https://github.com/wolverton-research-group/qmpy",
+        ],
+        # https://doi.org/10.6084/m9.figshare.22721047
+        "mlearn": [
+            "https://figshare.com/ndownloader/files/40424156",
+            "mlearn.json",
+            "Obtaining mlearn dataset 1730...",
+            "https://github.com/materialsvirtuallab/mlearn",
+        ],
+        # https://doi.org/10.6084/m9.figshare.22814318
+        "foundry_ml_exp_bandgaps": [
+            "https://figshare.com/ndownloader/files/40557743",
+            "foundry_ml_exp_bandgaps.json",
+            "Obtaining foundry_ml_exp_bandgaps dataset 2069...",
+            "https://foundry-ml.org/#/datasets/10.18126/wg3u-g8vu",
+        ],
+        # ToFix# https://doi.org/10.6084/m9.figshare.22815926
+        # "mat_scholar_ner": [
+        #    "https://figshare.com/ndownloader/files/40563593",
+        #    "mat_scholar_ner.json",
+        #    "Obtaining mat_scholar_ner dataset XYZ...",
+        #    "https://pubs.acs.org/doi/10.1021/acs.jcim.9b00470",
+        # ],
+        # https://doi.org/10.6084/m9.figshare.22817633
+        # Contains repeats
+        "ocp10k": [
+            "https://figshare.com/ndownloader/files/40566122",
+            "ocp10k.json",
+            "Obtaining OCP 10k train dataset, 59886...",
+            "https://github.com/Open-Catalyst-Project/ocp",
+        ],
+        # https://doi.org/10.6084/m9.figshare.22817651
+        "arxiv_summary": [
+            "https://figshare.com/ndownloader/files/40566137",
+            "arxiv_summary.json",
+            "Obtaining arxiv summary cond.mat dataset 137927...",
+            "https://github.com/usnistgov/chemnlp",
+        ],
+        # TODO:PubChem
+        # https://doi.org/10.6084/m9.figshare.22975787
+        "supercon_chem": [
+            "https://figshare.com/ndownloader/files/40719260",
+            "supercon_chem.json",
+            "Obtaining supercon chem dataset 16414...",
+            "https://www.nature.com/articles/s41524-018-0085-8",
+        ],
+        # https://doi.org/10.6084/m9.figshare.22976285
+        "mag2d_chem": [
+            "https://figshare.com/ndownloader/files/40720004",
+            "mag2d_chem.json",
+            "Obtaining magnetic 2D chem dataset 226...",
+            "https://doi.org/10.24435/materialscloud:2019.0020/v1",
+        ],
+        # https://doi.org/10.6084/m9.figshare.23000573
+        "vacancydb": [
+            "https://figshare.com/ndownloader/files/40750811",
+            "vacancydb.json",
+            "Obtaining vacancy dataset 464...",
+            "https://arxiv.org/abs/2205.08366",
+        ],
+        # Contains repeats
+        # https://doi.org/10.6084/m9.figshare.23206193
+        "ocp100k": [
+            "https://figshare.com/ndownloader/files/40902845",
+            "ocp100k.json",
+            "Obtaining OCP100k dataset 149886...",
+            "https://github.com/Open-Catalyst-Project/ocp",
+        ],
+        # https://doi.org/10.6084/m9.figshare.23250629
+        "ocp_all": [
+            "https://figshare.com/ndownloader/files/40974599",
+            "ocp_all.json",
+            "Obtaining OCPall dataset 510214...",
+            "https://github.com/Open-Catalyst-Project/ocp",
+        ],
+        # https://doi.org/10.6084/m9.figshare.23225687
+        "tinnet_N": [
+            "https://figshare.com/ndownloader/files/40934285",
+            "tinnet_N.json",
+            "Obtaining TinNet Nitrogen dataset 329...",
+            "https://github.com/hlxin/tinnet",
+        ],
+        # https://doi.org/10.6084/m9.figshare.23254151
+        "tinnet_O": [
+            "https://figshare.com/ndownloader/files/40978943",
+            "tinnet_O.json",
+            "Obtaining TinNet Oxygen dataset 747...",
+            "https://github.com/hlxin/tinnet",
+        ],
+        # https://doi.org/10.6084/m9.figshare.23254154
+        "tinnet_OH": [
+            "https://figshare.com/ndownloader/files/40978949",
+            "tinnet_OH.json",
+            "Obtaining TinNet OH dataset 748...",
+            "https://github.com/hlxin/tinnet",
+        ],
+        # https://doi.org/10.6084/m9.figshare.21370572
+        "supercon_3d": [
+            "https://figshare.com/ndownloader/files/38307921",
+            "jarvis_epc_data_figshare_1058.json",
+            "Obtaining supercond. Tc dataset 1058...",
+            "https://www.nature.com/articles/s41524-022-00933-1",
+        ],
+        # https://doi.org/10.6084/m9.figshare.21370572
+        "supercon_2d": [
+            "https://figshare.com/ndownloader/files/38950433",
+            "jarvis_epc_data_2d.json",
+            "Obtaining supercond. Tc dataset 161...",
+            "https://doi.org/10.1021/acs.nanolett.2c04420",
+        ],
         # https://doi.org/10.6084/m9.figshare.13154159
         "raw_files": [
             "https://ndownloader.figshare.com/files/25295732",
             "figshare_data-10-28-2020.json",
             "Obtaining raw io files 145k...",
             "https://www.nature.com/articles/s41524-020-00440-1",
         ],
```

### Comparing `jarvis-tools-2023.4.6/jarvis/db/lammps_to_xml.py` & `jarvis-tools-2023.5.26/jarvis/db/lammps_to_xml.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/db/qe_to_xml.py` & `jarvis-tools-2023.5.26/jarvis/db/qe_to_xml.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/db/restapi.py` & `jarvis-tools-2023.5.26/jarvis/db/restapi.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/db/vasp_to_xml.py` & `jarvis-tools-2023.5.26/jarvis/db/vasp_to_xml.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/db/webpages.py` & `jarvis-tools-2023.5.26/jarvis/db/webpages.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/boltztrap/inputs.py` & `jarvis-tools-2023.5.26/jarvis/io/boltztrap/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/boltztrap/outputs.py` & `jarvis-tools-2023.5.26/jarvis/io/boltztrap/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/calphad/write_decorated_poscar.py` & `jarvis-tools-2023.5.26/jarvis/io/calphad/write_decorated_poscar.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/lammps/inputs.py` & `jarvis-tools-2023.5.26/jarvis/io/lammps/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/lammps/outputs.py` & `jarvis-tools-2023.5.26/jarvis/io/lammps/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/nexus/inputs.py` & `jarvis-tools-2023.5.26/jarvis/io/nexus/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/pennylane/inputs.py` & `jarvis-tools-2023.5.26/jarvis/io/pennylane/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/phonopy/fcmat2hr.py` & `jarvis-tools-2023.5.26/jarvis/io/phonopy/fcmat2hr.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/phonopy/inputs.py` & `jarvis-tools-2023.5.26/jarvis/io/phonopy/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/phonopy/outputs.py` & `jarvis-tools-2023.5.26/jarvis/io/phonopy/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/prismatic/inputs.py` & `jarvis-tools-2023.5.26/jarvis/io/prismatic/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/qe/inputs.py` & `jarvis-tools-2023.5.26/jarvis/io/qe/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/qe/outputs.py` & `jarvis-tools-2023.5.26/jarvis/io/qe/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/qiskit/inputs.py` & `jarvis-tools-2023.5.26/jarvis/io/qiskit/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/tequila/inputs.py` & `jarvis-tools-2023.5.26/jarvis/io/tequila/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/vasp/default_potcars.json` & `jarvis-tools-2023.5.26/jarvis/io/vasp/default_potcars.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/vasp/inputs.py` & `jarvis-tools-2023.5.26/jarvis/io/vasp/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/vasp/outputs.py` & `jarvis-tools-2023.5.26/jarvis/io/vasp/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/wannier/default_semicore.json` & `jarvis-tools-2023.5.26/jarvis/io/wannier/default_semicore.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/wannier/inputs.py` & `jarvis-tools-2023.5.26/jarvis/io/wannier/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/wannier/outputs.py` & `jarvis-tools-2023.5.26/jarvis/io/wannier/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/wanniertools/inputs.py` & `jarvis-tools-2023.5.26/jarvis/io/wanniertools/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/wanniertools/outputs.py` & `jarvis-tools-2023.5.26/jarvis/io/wanniertools/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/wien2k/inputs.py` & `jarvis-tools-2023.5.26/jarvis/io/wien2k/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/wien2k/outputs.py` & `jarvis-tools-2023.5.26/jarvis/io/wien2k/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/io/zeopp/inputs.py` & `jarvis-tools-2023.5.26/jarvis/io/zeopp/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tasks/boltztrap/run.py` & `jarvis-tools-2023.5.26/jarvis/tasks/boltztrap/run.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tasks/lammps/templates/displace.mod` & `jarvis-tools-2023.5.26/jarvis/tasks/lammps/templates/displace.mod`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tasks/lammps/templates/inelast.mod` & `jarvis-tools-2023.5.26/jarvis/tasks/lammps/templates/inelast.mod`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tasks/lammps/templates/inelast_min.mod` & `jarvis-tools-2023.5.26/jarvis/tasks/lammps/templates/inelast_min.mod`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tasks/lammps/templates/inelast_nobox.mod` & `jarvis-tools-2023.5.26/jarvis/tasks/lammps/templates/inelast_nobox.mod`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tasks/lammps/templates/inelastcomb.mod` & `jarvis-tools-2023.5.26/jarvis/tasks/lammps/templates/inelastcomb.mod`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tasks/lammps/templates/inelastreax.mod` & `jarvis-tools-2023.5.26/jarvis/tasks/lammps/templates/inelastreax.mod`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tasks/lammps/templates/relax.mod` & `jarvis-tools-2023.5.26/jarvis/tasks/lammps/templates/relax.mod`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tasks/lammps/templates/templates.py` & `jarvis-tools-2023.5.26/jarvis/tasks/lammps/templates/templates.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tasks/lammps/lammps.py` & `jarvis-tools-2023.5.26/jarvis/tasks/lammps/lammps.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tasks/nexus/qmc.py` & `jarvis-tools-2023.5.26/jarvis/tasks/nexus/qmc.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tasks/phonopy/run.py` & `jarvis-tools-2023.5.26/jarvis/tasks/phonopy/run.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tasks/qe/converg.py` & `jarvis-tools-2023.5.26/jarvis/tasks/qe/converg.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tasks/qe/master_super.py` & `jarvis-tools-2023.5.26/jarvis/tasks/qe/master_super.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tasks/qe/qe.py` & `jarvis-tools-2023.5.26/jarvis/tasks/qe/qe.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tasks/qe/super.py` & `jarvis-tools-2023.5.26/jarvis/tasks/qe/super.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tasks/qe/super_tetra.py` & `jarvis-tools-2023.5.26/jarvis/tasks/qe/super_tetra.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tasks/vasp/vasp.py` & `jarvis-tools-2023.5.26/jarvis/tasks/vasp/vasp.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tasks/queue_jobs.py` & `jarvis-tools-2023.5.26/jarvis/tasks/queue_jobs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/ai/test_ai_uncertainty.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/ai/test_ai_uncertainty.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/ai/test_desc.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/ai/test_desc.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/ai/test_pkgs.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/ai/test_pkgs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/defects/test_surface.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/defects/test_surface.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/defects/test_vacancy.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/defects/test_vacancy.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/elastic/test_tensor.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/elastic/test_tensor.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/interface/test_zur.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/interface/test_zur.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/magnetism/test_magnetism.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/magnetism/test_magnetism.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/phonon/test_dos.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/phonon/test_dos.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/phonon/test_ir.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/phonon/test_ir.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/solar/test_solar.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/solar/test_solar.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/stm/test_stm.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/stm/test_stm.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/structure/test_neighbors.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/structure/test_neighbors.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/structure/test_spacegroup.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/structure/test_spacegroup.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/analysis/thermodynamics/test_energetics.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/analysis/thermodynamics/test_energetics.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/core/p.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/core/p.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/core/test_atoms.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/core/test_atoms.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/core/test_graph.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/core/test_graph.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/core/test_kpoints.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/core/test_kpoints.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/core/test_latice.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/core/test_latice.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/core/test_specie.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/core/test_specie.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/core/test_utils.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/db/test_figshare.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/db/test_figshare.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/tasks/test_lammps.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/tasks/test_lammps.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis/tests/testfiles/tasks/test_vasp.py` & `jarvis-tools-2023.5.26/jarvis/tests/testfiles/tasks/test_vasp.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/jarvis_tools.egg-info/PKG-INFO` & `jarvis-tools-2023.5.26/jarvis_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarvis-tools
-Version: 2023.4.6
+Version: 2023.5.26
 Summary: jarvis-tools: an open-source software package for data-driven atomistic materials design. https://jarvis.nist.gov/
 Home-page: https://github.com/usnistgov/jarvis
 Author: Kamal Choudhary
 Author-email: kamal.choudhary@nist.gov
 License: NIST
 Description: .. class:: center
```

### Comparing `jarvis-tools-2023.4.6/jarvis_tools.egg-info/SOURCES.txt` & `jarvis-tools-2023.5.26/jarvis_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/README.rst` & `jarvis-tools-2023.5.26/README.rst`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2023.4.6/setup.py` & `jarvis-tools-2023.5.26/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 base_dir = os.path.dirname(__file__)
 with open(os.path.join(base_dir, "README.rst")) as f:
     long_d = f.read()
 
 setup(
     name="jarvis-tools",
-    version="2023.04.06",
+    version="2023.05.26",
     long_description=long_d,
     install_requires=[
         "numpy>=1.19.5",
         "scipy>=1.4.1",
         "matplotlib>=3.0.0",
         "spglib>=1.14.1",
         "joblib>=0.14.1",
```

### Comparing `jarvis-tools-2023.4.6/PKG-INFO` & `jarvis-tools-2023.5.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarvis-tools
-Version: 2023.4.6
+Version: 2023.5.26
 Summary: jarvis-tools: an open-source software package for data-driven atomistic materials design. https://jarvis.nist.gov/
 Home-page: https://github.com/usnistgov/jarvis
 Author: Kamal Choudhary
 Author-email: kamal.choudhary@nist.gov
 License: NIST
 Description: .. class:: center
```

