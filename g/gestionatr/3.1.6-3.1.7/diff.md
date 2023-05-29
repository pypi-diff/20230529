# Comparing `tmp/gestionatr-3.1.6.tar.gz` & `tmp/gestionatr-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gestionatr-3.1.6.tar", last modified: Fri Apr 21 08:36:28 2023, max compression
+gzip compressed data, was "dist/gestionatr-3.1.7.tar", last modified: Mon May 29 07:35:07 2023, max compression
```

## Comparing `gestionatr-3.1.6.tar` & `gestionatr-3.1.7.tar`

### file list

```diff
@@ -1,298 +1,299 @@
-drwxrwxr-x   0 emili     (1000) emili     (1000)        0 2023-04-21 08:36:28.000000 gestionatr-3.1.6/
--rw-rw-r--   0 emili     (1000) emili     (1000)       54 2022-06-08 07:47:15.000000 gestionatr-3.1.6/MANIFEST.in
-drwxrwxr-x   0 emili     (1000) emili     (1000)        0 2023-04-21 08:36:28.000000 gestionatr-3.1.6/gestionatr/
--rw-rw-r--   0 emili     (1000) emili     (1000)     1235 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/parser_xml_defs_gas.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     4820 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/utils.py
--rw-rw-r--   0 emili     (1000) emili     (1000)   104061 2023-04-21 08:23:28.000000 gestionatr-3.1.6/gestionatr/defs.py
-drwxrwxr-x   0 emili     (1000) emili     (1000)        0 2023-04-21 08:36:28.000000 gestionatr-3.1.6/gestionatr/helpers/
--rw-rw-r--   0 emili     (1000) emili     (1000)     4366 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/helpers/funcions.py
--rw-rw-r--   0 emili     (1000) emili     (1000)       87 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/helpers/__init__.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     6998 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/cli.py
--rw-rw-r--   0 emili     (1000) emili     (1000)       46 2023-04-21 08:35:13.000000 gestionatr-3.1.6/gestionatr/__init__.py
-drwxrwxr-x   0 emili     (1000) emili     (1000)        0 2023-04-21 08:36:28.000000 gestionatr-3.1.6/gestionatr/output/
-drwxrwxr-x   0 emili     (1000) emili     (1000)        0 2023-04-21 08:36:28.000000 gestionatr-3.1.6/gestionatr/output/messages/
--rw-rw-r--   0 emili     (1000) emili     (1000)    25200 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_r1.py
--rw-rw-r--   0 emili     (1000) emili     (1000)      916 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/base_gas.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     1556 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_a1_46.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     3811 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_a1_05.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     6976 2023-01-19 15:12:26.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_t1.py
--rw-rw-r--   0 emili     (1000) emili     (1000)    22975 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_c1.py
--rw-rw-r--   0 emili     (1000) emili     (1000)    12407 2023-04-21 08:23:28.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_d1.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     4153 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_a1_41.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     1425 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_b2.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     1405 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_a20_36.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     1457 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_a1_49.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     1795 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_a1_43.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     2457 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_a25_42.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     3914 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_m1.py
--rw-rw-r--   0 emili     (1000) emili     (1000)    15493 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_c2.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     2970 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_a3.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     6302 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_a1_42.py
--rw-rw-r--   0 emili     (1000) emili     (1000)    12204 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_a1_48.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     1865 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_a1_04.py
--rw-rw-r--   0 emili     (1000) emili     (1000)    15170 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_p0.py
--rw-rw-r--   0 emili     (1000) emili     (1000)       24 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/output/messages/__init__.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     2085 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_a1_44.py
--rw-rw-r--   0 emili     (1000) emili     (1000)    34989 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_f1.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     5093 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/base.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     1514 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_a1_03.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     2737 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_a1.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     1770 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_a1_02.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     2638 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_w1.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     4593 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_a1_38.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     4054 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_q1.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     5049 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_b1.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     6718 2023-01-19 15:12:26.000000 gestionatr-3.1.6/gestionatr/output/messages/sw_e1.py
--rw-rw-r--   0 emili     (1000) emili     (1000)       24 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/output/__init__.py
-drwxrwxr-x   0 emili     (1000) emili     (1000)        0 2023-04-21 08:36:28.000000 gestionatr-3.1.6/gestionatr/input/
-drwxrwxr-x   0 emili     (1000) emili     (1000)        0 2023-04-21 08:36:28.000000 gestionatr-3.1.6/gestionatr/input/messages/
--rw-rw-r--   0 emili     (1000) emili     (1000)    31504 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/R1.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     8489 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/A12_26.py
--rw-rw-r--   0 emili     (1000) emili     (1000)    10247 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/A1.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     5864 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/Q1.py
--rw-rw-r--   0 emili     (1000) emili     (1000)      929 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/A1_02.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     4050 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/A1_46.py
--rw-rw-r--   0 emili     (1000) emili     (1000)      414 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/A1_03.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     1216 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/A1_49.py
--rw-rw-r--   0 emili     (1000) emili     (1000)      431 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/input/messages/A13_50.py
--rw-rw-r--   0 emili     (1000) emili     (1000)    25263 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/P0.py
--rw-rw-r--   0 emili     (1000) emili     (1000)    10092 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/A1_44.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     2018 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/defs.py
--rw-rw-r--   0 emili     (1000) emili     (1000)    52068 2023-04-21 08:23:38.000000 gestionatr-3.1.6/gestionatr/input/messages/B70.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     3297 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/T1.py
--rw-rw-r--   0 emili     (1000) emili     (1000)      459 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/A3.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     3591 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/B1.py
--rw-rw-r--   0 emili     (1000) emili     (1000)    27844 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/A1_48.py
--rw-rw-r--   0 emili     (1000) emili     (1000)    16369 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/message.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     1883 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/A1_43.py
--rw-rw-r--   0 emili     (1000) emili     (1000)      797 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/A1_42.py
--rw-rw-r--   0 emili     (1000) emili     (1000)      765 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/B2.py
--rw-rw-r--   0 emili     (1000) emili     (1000)    17800 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/C2.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     4659 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/A1_38.py
--rw-rw-r--   0 emili     (1000) emili     (1000)    26696 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/A1_41.py
--rw-rw-r--   0 emili     (1000) emili     (1000)    15986 2023-04-21 08:23:28.000000 gestionatr-3.1.6/gestionatr/input/messages/D1.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     2590 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/W1.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     1353 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/A1_05.py
--rw-rw-r--   0 emili     (1000) emili     (1000)    93514 2023-04-21 08:34:56.000000 gestionatr-3.1.6/gestionatr/input/messages/F1.py
--rw-rw-r--   0 emili     (1000) emili     (1000)      749 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/A1_04.py
--rw-rw-r--   0 emili     (1000) emili     (1000)      893 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/__init__.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     1915 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/A19_45.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     1266 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/M1.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     4157 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/A20_36.py
--rw-rw-r--   0 emili     (1000) emili     (1000)      718 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/input/messages/A12_24.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     1114 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/Deadlines.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     9406 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/message_gas.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     4004 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/E1.py
--rw-rw-r--   0 emili     (1000) emili     (1000)    19377 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/gestionatr_maker.py
--rw-rw-r--   0 emili     (1000) emili     (1000)    24815 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/input/messages/C1.py
--rw-rw-r--   0 emili     (1000) emili     (1000)       24 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/input/__init__.py
-drwxrwxr-x   0 emili     (1000) emili     (1000)        0 2023-04-21 08:36:28.000000 gestionatr-3.1.6/gestionatr/data/
--rw-rw-r--   0 emili     (1000) emili     (1000)     3469 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2S42.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3937 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A103.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     2961 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A529.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     5691 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/B7033.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     8884 2023-01-19 15:12:26.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeP002.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      696 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/ActivacionBajaSuspension.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     6109 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A441.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     1218 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeB201.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4685 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2541.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)   141040 2023-01-19 15:12:26.000000 gestionatr-3.1.6/gestionatr/data/TiposSencillos.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)    54319 2023-01-19 15:12:26.000000 gestionatr-3.1.6/gestionatr/data/TiposComplejos.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     1257 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeA101.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)    11518 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/TiposComplejosCCAA.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4311 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A104.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3044 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2643.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3043 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2644.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4650 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A102.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     2860 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeT101.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)    70346 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/CommonTagsATCOM.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     1840 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/SolicitudAportacionLectura.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     6339 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A144.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     5593 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A1350.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4306 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A3S02.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      717 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/AceptacionReclamacion.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     5303 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A142.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3366 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A8609.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3872 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A219.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     8279 2022-11-21 11:16:12.000000 gestionatr-3.1.6/gestionatr/data/B7031.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     7901 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A349.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3044 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2641.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     9740 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A1550.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      653 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/ContestacionIncidencia.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      695 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/AceptacionTraspasoCOR.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      676 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/BajaSuspension.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      620 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/Rechazo.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      599 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/Alta.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      665 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/IncidenciasATRDistribuidor.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      745 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/ActivacionTraspasoCORSaliente.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     7290 2022-11-21 11:16:12.000000 gestionatr-3.1.6/gestionatr/data/B7032.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4385 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A8409.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)    13726 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A341.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      654 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/AceptacionModificacionDeATR.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)    13496 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A138.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      650 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/ActivacionTraspasoCOR.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)    10137 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A1945.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      703 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/AceptacionBajaSuspension.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      664 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/SolicitudInformacionAlRegistroDePS.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     1837 2023-01-19 15:12:26.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeM105.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      642 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/RechazoTraspasoCOR.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     5460 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A205.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     1019 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/AceptacionCambiodeComercializadorSaliente.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     5943 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A304.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      822 2023-01-19 15:12:26.000000 gestionatr-3.1.6/gestionatr/data/SaldoLecturasFacturacion.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4685 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2505.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      638 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/RechazoPeticion.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      746 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/NotificacionActivacionPorDesistimiento.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     9982 2022-11-21 11:16:12.000000 gestionatr-3.1.6/gestionatr/data/A105.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4344 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A4S41.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     5131 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A8509.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     2359 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeSaliente.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4678 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2538.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     5038 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A204.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3044 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2642.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      738 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/EnvioInformacionReclamacion.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     7416 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A302.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4238 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A15S50.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     9415 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A305.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      692 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/RechazoDesistimiento.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      691 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/SolicitudDesistimiento.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)    34602 2023-01-19 15:12:26.000000 gestionatr-3.1.6/gestionatr/data/Facturacion.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3044 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2604.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     9633 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A444.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      813 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/AceptacionAnulacionReclamacion.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      693 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/EnvioInformacionPS.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      784 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/AceptacionAportacionLectura.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     5523 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A438.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3859 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2S03.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3469 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2S41.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     9219 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A141.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)    17413 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A629.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      653 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/RechazoReclamacion.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     6973 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A21.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      699 2023-04-21 08:23:28.000000 gestionatr-3.1.6/gestionatr/data/NotificacionCambiosATRDesdeDistribuidor.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     1264 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/WebserviceSync.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)    11459 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A338.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3044 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2649.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4276 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A143.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     2355 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeC101.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4679 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2504.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      717 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/ActivacionModificacionDeATR.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     5820 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A348.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     1939 2023-01-19 15:12:26.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeC205.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      813 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/RechazoCambiodeComercializadorSaliente.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     6846 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeAceptacion.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     1773 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeT105.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      693 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/AceptacionDesistimiento.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4858 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A248.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     6346 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A242.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     1651 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeB101.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     7417 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A8009.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      684 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/PeticionInformacionAdicionalReclamacion.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     9128 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/xml.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      768 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/ActivacionCambiodeComercializadorConCambios.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     6487 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2544.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     9764 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A344.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     7281 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A342.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)    13772 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A1226.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     1945 2023-01-19 15:12:26.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeC105.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     1046 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/WebserviceRPS.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4672 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A246.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4001 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A449.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     5663 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A442.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     6496 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A202.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4533 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A243.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     6598 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A238.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     5034 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A404.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3044 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2638.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      738 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/CambiodeComercializadorSinCambios.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     7878 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/CommonTagsPETS.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3951 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A146.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)    80962 2022-11-21 11:16:12.000000 gestionatr-3.1.6/gestionatr/data/CommonTagsCONT.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3278 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A20.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      738 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/CambiodeComercializadorConCambios.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      780 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/AceptacionAnulacion.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     7530 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2548.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3984 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A405.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     5730 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A443.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      629 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/ActivacionAlta.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)    18240 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/TiposSencillosCCAA.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      768 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/ActivacionCambiodeComercializadorSinCambios.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3962 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A4S42.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      728 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/AceptacionAlta.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)    10626 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A6161.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      708 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/CierreReclamacion.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      700 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/ActivacionBaja.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4579 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A148.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     1545 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeRechazoCCAA.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3753 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A149.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4489 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A203.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     2628 2023-01-19 15:12:26.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeM101.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     2821 2023-01-19 15:12:26.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeA301.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      612 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/RechazoD1.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4303 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A3S41.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4026 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A3S42.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      690 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/ModificacionDeATR.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4551 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A1224.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     1026 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeA102.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     1166 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeB105.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4338 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2648.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4152 2023-01-19 15:12:26.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeE.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      739 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/AceptacionCambiodeComercializadorSinCambios.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4573 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A244.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     1562 2023-01-19 15:12:26.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeA305.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4475 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A402.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3535 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A343.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)    14321 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeR105.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     6556 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeRechazo.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     7660 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A241.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      724 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/ActivacionDesistimiento.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3950 2023-01-19 15:12:26.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeC201.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      739 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/AceptacionCambiodeComercializadorConCambios.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)    11577 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A3S49.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4685 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2543.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      699 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/AceptacionD1.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4685 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2542.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)    37855 2022-11-21 11:16:12.000000 gestionatr-3.1.6/gestionatr/data/CommonTagsFACT.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3469 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2S02.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      647 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/SolicitudTraspasoCOR.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      964 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A101.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4344 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A4S49.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3044 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2605.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     1063 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A102e.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      598 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/AnulacionSolicitudReclamacion.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3653 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A1450.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      741 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/ActivacionComercializadorSaliente.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4751 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A249.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     9516 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A708.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4685 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2549.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      716 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/ReclamacionPeticion.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     4344 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A4S02.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     1051 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/AceptacionNotificacionCambiosATRDesdeDistribuidor.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      857 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/AceptacionAnulacionBaja.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     5848 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/TipoMensajeR101.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     3390 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A2S49.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)      565 2021-06-28 17:31:48.000000 gestionatr-3.1.6/gestionatr/data/AnulacionSolicitud.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)     5337 2022-06-08 07:47:15.000000 gestionatr-3.1.6/gestionatr/data/A8109.xsd
--rw-rw-r--   0 emili     (1000) emili     (1000)       40 2022-10-13 14:33:14.000000 gestionatr-3.1.6/gestionatr/exceptions.py
--rw-rw-r--   0 emili     (1000) emili     (1000)   133884 2023-04-04 13:09:21.000000 gestionatr-3.1.6/gestionatr/defs_gas.py
--rw-rw-r--   0 emili     (1000) emili     (1000)       54 2023-04-04 13:09:21.000000 gestionatr-3.1.6/requirements.txt
--rw-rw-r--   0 emili     (1000) emili     (1000)       38 2023-04-21 08:36:28.000000 gestionatr-3.1.6/setup.cfg
--rw-rw-r--   0 emili     (1000) emili     (1000)      279 2023-04-04 13:09:21.000000 gestionatr-3.1.6/README.md
--rw-rw-r--   0 emili     (1000) emili     (1000)     1391 2022-06-08 07:47:15.000000 gestionatr-3.1.6/setup.py
--rw-rw-r--   0 emili     (1000) emili     (1000)        7 2022-06-08 07:47:15.000000 gestionatr-3.1.6/requirements-dev.txt
-drwxrwxr-x   0 emili     (1000) emili     (1000)        0 2023-04-21 08:36:28.000000 gestionatr-3.1.6/gestionatr.egg-info/
--rw-rw-r--   0 emili     (1000) emili     (1000)       58 2023-04-21 08:36:28.000000 gestionatr-3.1.6/gestionatr.egg-info/entry_points.txt
--rw-rw-r--   0 emili     (1000) emili     (1000)       54 2023-04-21 08:36:28.000000 gestionatr-3.1.6/gestionatr.egg-info/requires.txt
--rw-rw-r--   0 emili     (1000) emili     (1000)     9453 2023-04-21 08:36:28.000000 gestionatr-3.1.6/gestionatr.egg-info/SOURCES.txt
--rw-rw-r--   0 emili     (1000) emili     (1000)        1 2023-04-21 08:36:28.000000 gestionatr-3.1.6/gestionatr.egg-info/dependency_links.txt
--rw-rw-r--   0 emili     (1000) emili     (1000)       17 2023-04-21 08:36:28.000000 gestionatr-3.1.6/gestionatr.egg-info/top_level.txt
--rw-rw-r--   0 emili     (1000) emili     (1000)      278 2023-04-21 08:36:28.000000 gestionatr-3.1.6/gestionatr.egg-info/PKG-INFO
-drwxrwxr-x   0 emili     (1000) emili     (1000)        0 2023-04-21 08:36:28.000000 gestionatr-3.1.6/tests/
--rw-rw-r--   0 emili     (1000) emili     (1000)     5605 2023-04-04 13:09:21.000000 gestionatr-3.1.6/tests/utils.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     2047 2023-04-04 13:09:21.000000 gestionatr-3.1.6/tests/test_cli.py
--rw-rw-r--   0 emili     (1000) emili     (1000)   231034 2023-04-21 08:23:28.000000 gestionatr-3.1.6/tests/test_output.py
--rw-rw-r--   0 emili     (1000) emili     (1000)   299786 2023-04-21 08:23:28.000000 gestionatr-3.1.6/tests/test_input.py
--rw-rw-r--   0 emili     (1000) emili     (1000)      640 2022-06-08 07:47:15.000000 gestionatr-3.1.6/tests/test_table_description.py
--rw-rw-r--   0 emili     (1000) emili     (1000)       99 2022-06-08 07:47:15.000000 gestionatr-3.1.6/tests/__init__.py
--rw-rw-r--   0 emili     (1000) emili     (1000)     1262 2023-04-04 13:09:21.000000 gestionatr-3.1.6/tests/test_helpers.py
--rw-rw-r--   0 emili     (1000) emili     (1000)      278 2023-04-21 08:36:28.000000 gestionatr-3.1.6/PKG-INFO
+drwxrwxr-x   0 eberloso  (1000) eberloso  (1000)        0 2023-05-29 07:35:07.000000 gestionatr-3.1.7/
+drwxrwxr-x   0 eberloso  (1000) eberloso  (1000)        0 2023-05-29 07:35:07.000000 gestionatr-3.1.7/gestionatr.egg-info/
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)       58 2023-05-29 07:35:07.000000 gestionatr-3.1.7/gestionatr.egg-info/entry_points.txt
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)       17 2023-05-29 07:35:07.000000 gestionatr-3.1.7/gestionatr.egg-info/top_level.txt
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)       54 2023-05-29 07:35:07.000000 gestionatr-3.1.7/gestionatr.egg-info/requires.txt
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     9478 2023-05-29 07:35:07.000000 gestionatr-3.1.7/gestionatr.egg-info/SOURCES.txt
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)        1 2023-05-29 07:35:07.000000 gestionatr-3.1.7/gestionatr.egg-info/dependency_links.txt
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      278 2023-05-29 07:35:07.000000 gestionatr-3.1.7/gestionatr.egg-info/PKG-INFO
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1391 2021-06-15 06:26:33.000000 gestionatr-3.1.7/setup.py
+drwxrwxr-x   0 eberloso  (1000) eberloso  (1000)        0 2023-05-29 07:35:07.000000 gestionatr-3.1.7/tests/
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)   299786 2023-03-30 16:38:37.000000 gestionatr-3.1.7/tests/test_input.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      640 2021-06-15 06:26:33.000000 gestionatr-3.1.7/tests/test_table_description.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     5605 2023-03-30 16:38:37.000000 gestionatr-3.1.7/tests/utils.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)       99 2021-06-15 06:26:33.000000 gestionatr-3.1.7/tests/__init__.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4654 2023-04-03 10:31:46.000000 gestionatr-3.1.7/tests/test_request_p0.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)   231034 2023-03-30 16:38:37.000000 gestionatr-3.1.7/tests/test_output.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1262 2023-03-30 16:38:37.000000 gestionatr-3.1.7/tests/test_helpers.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     2047 2023-03-30 16:38:37.000000 gestionatr-3.1.7/tests/test_cli.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      279 2023-03-30 16:38:37.000000 gestionatr-3.1.7/README.md
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)        7 2021-06-15 06:26:33.000000 gestionatr-3.1.7/requirements-dev.txt
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      278 2023-05-29 07:35:07.000000 gestionatr-3.1.7/PKG-INFO
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)       38 2023-05-29 07:35:07.000000 gestionatr-3.1.7/setup.cfg
+drwxrwxr-x   0 eberloso  (1000) eberloso  (1000)        0 2023-05-29 07:35:07.000000 gestionatr-3.1.7/gestionatr/
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)   133900 2023-05-29 07:30:29.000000 gestionatr-3.1.7/gestionatr/defs_gas.py
+drwxrwxr-x   0 eberloso  (1000) eberloso  (1000)        0 2023-05-29 07:35:07.000000 gestionatr-3.1.7/gestionatr/input/
+drwxrwxr-x   0 eberloso  (1000) eberloso  (1000)        0 2023-05-29 07:35:07.000000 gestionatr-3.1.7/gestionatr/input/messages/
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    27844 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/A1_48.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     2590 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/W1.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    10092 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/A1_44.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     8489 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/A12_26.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     9406 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/message_gas.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      718 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/input/messages/A12_24.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      797 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/A1_42.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    52068 2023-04-05 06:29:49.000000 gestionatr-3.1.7/gestionatr/input/messages/B70.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1216 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/A1_49.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     2018 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/defs.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      765 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/B2.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      414 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/A1_03.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4157 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/A20_36.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     5864 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/Q1.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3591 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/B1.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      929 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/A1_02.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    19377 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/gestionatr_maker.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4659 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/A1_38.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    17800 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/C2.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3297 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/T1.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1114 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/Deadlines.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1266 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/M1.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      893 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/__init__.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    31504 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/R1.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    16369 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/message.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    24815 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/C1.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      749 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/A1_04.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    25263 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/P0.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1883 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/A1_43.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    15986 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/D1.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1353 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/A1_05.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      459 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/A3.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    93514 2023-05-08 06:58:19.000000 gestionatr-3.1.7/gestionatr/input/messages/F1.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4004 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/E1.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    10247 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/A1.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    26696 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/A1_41.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4050 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/A1_46.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      431 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/input/messages/A13_50.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1915 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/input/messages/A19_45.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)       24 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/input/__init__.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)   104061 2023-05-09 12:44:32.000000 gestionatr-3.1.7/gestionatr/defs.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4820 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/utils.py
+drwxrwxr-x   0 eberloso  (1000) eberloso  (1000)        0 2023-05-29 07:35:07.000000 gestionatr-3.1.7/gestionatr/data/
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      857 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/AceptacionAnulacionBaja.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     5034 2020-08-06 12:55:00.000000 gestionatr-3.1.7/gestionatr/data/A404.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     6339 2021-07-06 06:22:24.000000 gestionatr-3.1.7/gestionatr/data/A144.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1945 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeC105.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     7660 2020-08-06 12:50:16.000000 gestionatr-3.1.7/gestionatr/data/A241.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1063 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/A102e.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     5691 2021-11-10 10:16:12.000000 gestionatr-3.1.7/gestionatr/data/B7033.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3366 2021-05-10 13:10:36.000000 gestionatr-3.1.7/gestionatr/data/A8609.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    54319 2022-11-17 11:45:11.000000 gestionatr-3.1.7/gestionatr/data/TiposComplejos.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    11459 2021-06-09 09:22:42.000000 gestionatr-3.1.7/gestionatr/data/A338.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     7290 2022-11-18 07:42:03.000000 gestionatr-3.1.7/gestionatr/data/B7032.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     8884 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeP002.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3043 2020-08-06 12:56:32.000000 gestionatr-3.1.7/gestionatr/data/A2644.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     5460 2021-05-10 09:27:42.000000 gestionatr-3.1.7/gestionatr/data/A205.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3469 2020-08-06 12:36:44.000000 gestionatr-3.1.7/gestionatr/data/A2S02.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    34602 2022-11-17 11:45:11.000000 gestionatr-3.1.7/gestionatr/data/Facturacion.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3044 2020-09-15 08:48:18.000000 gestionatr-3.1.7/gestionatr/data/A2642.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      738 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/CambiodeComercializadorSinCambios.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    37855 2022-11-18 07:42:03.000000 gestionatr-3.1.7/gestionatr/data/CommonTagsFACT.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     2860 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeT101.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      728 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/AceptacionAlta.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      696 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/ActivacionBajaSuspension.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      738 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/EnvioInformacionReclamacion.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     6109 2020-08-06 12:53:34.000000 gestionatr-3.1.7/gestionatr/data/A441.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      724 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/ActivacionDesistimiento.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1218 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeB201.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      695 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/AceptacionTraspasoCOR.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3872 2020-08-06 12:50:26.000000 gestionatr-3.1.7/gestionatr/data/A219.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     5730 2020-08-06 12:53:20.000000 gestionatr-3.1.7/gestionatr/data/A443.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      784 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/AceptacionAportacionLectura.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4685 2020-08-06 12:57:26.000000 gestionatr-3.1.7/gestionatr/data/A2543.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3044 2020-08-06 12:56:46.000000 gestionatr-3.1.7/gestionatr/data/A2641.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1562 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeA305.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4026 2020-08-06 12:43:46.000000 gestionatr-3.1.7/gestionatr/data/A3S42.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      598 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/AnulacionSolicitudReclamacion.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1019 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/AceptacionCambiodeComercializadorSaliente.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3044 2020-09-15 08:48:08.000000 gestionatr-3.1.7/gestionatr/data/A2643.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      612 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/RechazoD1.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    11577 2021-05-10 10:47:02.000000 gestionatr-3.1.7/gestionatr/data/A3S49.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      699 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/NotificacionCambiosATRDesdeDistribuidor.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      780 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/AceptacionAnulacion.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     6846 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeAceptacion.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4306 2020-08-06 12:44:00.000000 gestionatr-3.1.7/gestionatr/data/A3S02.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1046 2021-06-16 05:55:26.000000 gestionatr-3.1.7/gestionatr/data/WebserviceRPS.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     7878 2020-08-06 12:59:06.000000 gestionatr-3.1.7/gestionatr/data/CommonTagsPETS.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    80962 2022-11-18 07:42:03.000000 gestionatr-3.1.7/gestionatr/data/CommonTagsCONT.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      822 2021-09-06 06:23:29.000000 gestionatr-3.1.7/gestionatr/data/SaldoLecturasFacturacion.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4344 2020-08-06 12:43:32.000000 gestionatr-3.1.7/gestionatr/data/A4S02.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1837 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeM105.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4001 2020-08-06 12:53:10.000000 gestionatr-3.1.7/gestionatr/data/A449.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      703 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/AceptacionBajaSuspension.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      690 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/ModificacionDeATR.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4152 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeE.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4685 2020-08-06 12:57:32.000000 gestionatr-3.1.7/gestionatr/data/A2541.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     2961 2020-08-06 12:53:06.000000 gestionatr-3.1.7/gestionatr/data/A529.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1939 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeC205.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1840 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/SolicitudAportacionLectura.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3951 2020-08-06 12:46:34.000000 gestionatr-3.1.7/gestionatr/data/A146.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4573 2020-08-06 12:49:52.000000 gestionatr-3.1.7/gestionatr/data/A244.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      664 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/SolicitudInformacionAlRegistroDePS.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      768 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/ActivacionCambiodeComercializadorConCambios.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1545 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeRechazoCCAA.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      699 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/AceptacionD1.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3469 2020-08-06 12:42:10.000000 gestionatr-3.1.7/gestionatr/data/A2S41.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1051 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/AceptacionNotificacionCambiosATRDesdeDistribuidor.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     5820 2020-08-06 12:51:08.000000 gestionatr-3.1.7/gestionatr/data/A348.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4679 2020-08-06 12:57:44.000000 gestionatr-3.1.7/gestionatr/data/A2504.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4276 2022-02-18 09:02:26.000000 gestionatr-3.1.7/gestionatr/data/A143.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    18240 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TiposSencillosCCAA.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     2821 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeA301.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     7901 2021-05-10 10:46:16.000000 gestionatr-3.1.7/gestionatr/data/A349.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     9764 2020-08-06 12:48:56.000000 gestionatr-3.1.7/gestionatr/data/A344.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4385 2021-05-10 13:09:52.000000 gestionatr-3.1.7/gestionatr/data/A8409.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     6598 2022-02-18 09:02:27.000000 gestionatr-3.1.7/gestionatr/data/A238.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      684 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/PeticionInformacionAdicionalReclamacion.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      565 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/AnulacionSolicitud.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      964 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/A101.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1773 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeT105.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1651 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeB101.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      708 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/CierreReclamacion.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      692 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/RechazoDesistimiento.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3535 2022-02-18 09:02:28.000000 gestionatr-3.1.7/gestionatr/data/A343.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     2359 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeSaliente.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      745 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/ActivacionTraspasoCORSaliente.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      653 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/RechazoReclamacion.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1257 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeA101.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     9128 2020-08-06 12:59:22.000000 gestionatr-3.1.7/gestionatr/data/xml.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4311 2020-08-06 12:45:50.000000 gestionatr-3.1.7/gestionatr/data/A104.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3984 2020-08-06 12:54:42.000000 gestionatr-3.1.7/gestionatr/data/A405.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     5523 2020-08-06 12:53:38.000000 gestionatr-3.1.7/gestionatr/data/A438.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      813 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/AceptacionAnulacionReclamacion.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     7281 2021-06-17 14:10:42.000000 gestionatr-3.1.7/gestionatr/data/A342.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3962 2020-08-06 12:46:56.000000 gestionatr-3.1.7/gestionatr/data/A4S42.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     2628 2022-11-16 15:23:36.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeM101.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     5848 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeR101.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      647 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/SolicitudTraspasoCOR.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    13772 2020-08-06 12:52:46.000000 gestionatr-3.1.7/gestionatr/data/A1226.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4751 2020-08-06 12:49:38.000000 gestionatr-3.1.7/gestionatr/data/A249.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3278 2020-08-06 12:46:10.000000 gestionatr-3.1.7/gestionatr/data/A20.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     9415 2021-06-11 05:42:58.000000 gestionatr-3.1.7/gestionatr/data/A305.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1026 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeA102.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3937 2020-08-06 12:45:54.000000 gestionatr-3.1.7/gestionatr/data/A103.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      665 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/IncidenciasATRDistribuidor.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3044 2020-08-06 12:56:50.000000 gestionatr-3.1.7/gestionatr/data/A2638.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     6556 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeRechazo.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      768 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/ActivacionCambiodeComercializadorSinCambios.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4685 2020-08-06 12:57:10.000000 gestionatr-3.1.7/gestionatr/data/A2549.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3753 2020-08-06 12:46:14.000000 gestionatr-3.1.7/gestionatr/data/A149.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    13496 2021-05-10 10:08:46.000000 gestionatr-3.1.7/gestionatr/data/A138.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4685 2020-08-06 12:57:30.000000 gestionatr-3.1.7/gestionatr/data/A2542.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      741 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/ActivacionComercializadorSaliente.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4338 2020-08-06 12:56:28.000000 gestionatr-3.1.7/gestionatr/data/A2648.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      650 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/ActivacionTraspasoCOR.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      738 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/CambiodeComercializadorConCambios.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      739 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/AceptacionCambiodeComercializadorSinCambios.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      693 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/EnvioInformacionPS.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      676 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/BajaSuspension.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      739 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/AceptacionCambiodeComercializadorConCambios.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4344 2020-08-06 12:44:28.000000 gestionatr-3.1.7/gestionatr/data/A4S49.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     8279 2022-11-18 07:42:03.000000 gestionatr-3.1.7/gestionatr/data/B7031.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      746 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/NotificacionActivacionPorDesistimiento.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4475 2020-08-06 12:55:04.000000 gestionatr-3.1.7/gestionatr/data/A402.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     9516 2020-08-06 12:52:56.000000 gestionatr-3.1.7/gestionatr/data/A708.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    70346 2021-07-06 06:27:52.000000 gestionatr-3.1.7/gestionatr/data/CommonTagsATCOM.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    10626 2020-08-06 12:56:20.000000 gestionatr-3.1.7/gestionatr/data/A6161.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1166 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeB105.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4489 2020-08-06 12:50:58.000000 gestionatr-3.1.7/gestionatr/data/A203.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3044 2020-08-06 12:57:06.000000 gestionatr-3.1.7/gestionatr/data/A2604.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      813 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/RechazoCambiodeComercializadorSaliente.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4238 2020-08-06 12:44:20.000000 gestionatr-3.1.7/gestionatr/data/A15S50.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    14321 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeR105.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    13726 2021-06-17 14:34:54.000000 gestionatr-3.1.7/gestionatr/data/A341.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     9219 2020-08-06 12:45:36.000000 gestionatr-3.1.7/gestionatr/data/A141.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     5593 2020-08-06 12:52:42.000000 gestionatr-3.1.7/gestionatr/data/A1350.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     9982 2022-11-18 07:42:03.000000 gestionatr-3.1.7/gestionatr/data/A105.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      691 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/SolicitudDesistimiento.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      700 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/ActivacionBaja.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4672 2020-08-06 12:49:46.000000 gestionatr-3.1.7/gestionatr/data/A246.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     6346 2020-08-06 12:50:12.000000 gestionatr-3.1.7/gestionatr/data/A242.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3859 2020-08-06 12:42:02.000000 gestionatr-3.1.7/gestionatr/data/A2S03.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     5131 2021-06-09 13:38:46.000000 gestionatr-3.1.7/gestionatr/data/A8509.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      654 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/AceptacionModificacionDeATR.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     5303 2020-08-06 12:45:30.000000 gestionatr-3.1.7/gestionatr/data/A142.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     6973 2020-08-06 12:46:04.000000 gestionatr-3.1.7/gestionatr/data/A21.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     6487 2020-08-06 12:57:22.000000 gestionatr-3.1.7/gestionatr/data/A2544.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     5337 2021-06-09 13:37:06.000000 gestionatr-3.1.7/gestionatr/data/A8109.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     7416 2021-06-17 14:34:54.000000 gestionatr-3.1.7/gestionatr/data/A302.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3653 2020-08-06 12:52:36.000000 gestionatr-3.1.7/gestionatr/data/A1450.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      642 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/RechazoTraspasoCOR.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     6496 2020-08-06 12:51:12.000000 gestionatr-3.1.7/gestionatr/data/A202.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      599 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/Alta.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      717 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/ActivacionModificacionDeATR.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     9740 2021-05-10 10:50:02.000000 gestionatr-3.1.7/gestionatr/data/A1550.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4650 2020-08-06 12:45:58.000000 gestionatr-3.1.7/gestionatr/data/A102.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1264 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/WebserviceSync.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3950 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeC201.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3044 2020-08-06 12:56:54.000000 gestionatr-3.1.7/gestionatr/data/A2605.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      653 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/ContestacionIncidencia.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4533 2022-02-18 09:02:27.000000 gestionatr-3.1.7/gestionatr/data/A243.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4303 2020-08-06 12:43:54.000000 gestionatr-3.1.7/gestionatr/data/A3S41.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      693 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/AceptacionDesistimiento.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3390 2020-08-06 12:44:10.000000 gestionatr-3.1.7/gestionatr/data/A2S49.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    11518 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TiposComplejosCCAA.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     5038 2020-08-06 12:50:42.000000 gestionatr-3.1.7/gestionatr/data/A204.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      716 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/ReclamacionPeticion.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     9633 2020-08-06 12:53:14.000000 gestionatr-3.1.7/gestionatr/data/A444.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    10137 2020-08-06 12:55:10.000000 gestionatr-3.1.7/gestionatr/data/A1945.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      620 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/Rechazo.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4579 2020-08-06 12:46:28.000000 gestionatr-3.1.7/gestionatr/data/A148.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     7417 2021-05-10 13:09:20.000000 gestionatr-3.1.7/gestionatr/data/A8009.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     5943 2020-08-06 12:49:28.000000 gestionatr-3.1.7/gestionatr/data/A304.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3469 2020-08-06 12:42:16.000000 gestionatr-3.1.7/gestionatr/data/A2S42.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     7530 2020-08-06 12:57:16.000000 gestionatr-3.1.7/gestionatr/data/A2548.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      638 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/RechazoPeticion.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)   141040 2022-11-17 11:45:48.000000 gestionatr-3.1.7/gestionatr/data/TiposSencillos.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3044 2020-08-06 12:56:24.000000 gestionatr-3.1.7/gestionatr/data/A2649.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4858 2020-08-06 12:49:42.000000 gestionatr-3.1.7/gestionatr/data/A248.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4678 2020-08-06 12:57:36.000000 gestionatr-3.1.7/gestionatr/data/A2538.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4344 2020-08-06 12:43:24.000000 gestionatr-3.1.7/gestionatr/data/A4S41.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     2355 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/TipoMensajeC101.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4685 2020-08-06 12:57:40.000000 gestionatr-3.1.7/gestionatr/data/A2505.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      717 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/AceptacionReclamacion.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      629 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/data/ActivacionAlta.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    17413 2021-06-17 14:46:24.000000 gestionatr-3.1.7/gestionatr/data/A629.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     5663 2020-08-06 12:53:24.000000 gestionatr-3.1.7/gestionatr/data/A442.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4551 2020-08-06 12:52:52.000000 gestionatr-3.1.7/gestionatr/data/A1224.xsd
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)       46 2023-05-29 07:34:25.000000 gestionatr-3.1.7/gestionatr/__init__.py
+drwxrwxr-x   0 eberloso  (1000) eberloso  (1000)        0 2023-05-29 07:35:07.000000 gestionatr-3.1.7/gestionatr/output/
+drwxrwxr-x   0 eberloso  (1000) eberloso  (1000)        0 2023-05-29 07:35:07.000000 gestionatr-3.1.7/gestionatr/output/messages/
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    15493 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_c2.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1514 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_a1_03.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     2085 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_a1_44.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     5049 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_b1.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     6302 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_a1_42.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1457 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_a1_49.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    12204 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_a1_48.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4054 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_q1.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     2638 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_w1.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     6718 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_e1.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    25200 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_r1.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    34989 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_f1.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3914 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_m1.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)      916 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/base_gas.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4153 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_a1_41.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4593 2021-09-30 11:27:34.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_a1_38.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1865 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_a1_04.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1770 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_a1_02.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)       24 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/output/messages/__init__.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1405 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_a20_36.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     3811 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_a1_05.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    12407 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_d1.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     5093 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/base.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    22975 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_c1.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1795 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_a1_43.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1425 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_b2.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     2737 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_a1.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     6976 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_t1.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)    15170 2023-04-03 11:01:43.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_p0.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1556 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_a1_46.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     2970 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_a3.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     2457 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/output/messages/sw_a25_42.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)       24 2021-06-15 06:26:33.000000 gestionatr-3.1.7/gestionatr/output/__init__.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     6998 2023-04-03 10:30:13.000000 gestionatr-3.1.7/gestionatr/cli.py
+drwxrwxr-x   0 eberloso  (1000) eberloso  (1000)        0 2023-05-29 07:35:07.000000 gestionatr-3.1.7/gestionatr/helpers/
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     4366 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/helpers/funcions.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)       87 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/helpers/__init__.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)       40 2022-10-27 10:36:10.000000 gestionatr-3.1.7/gestionatr/exceptions.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)     1235 2023-03-30 16:38:37.000000 gestionatr-3.1.7/gestionatr/parser_xml_defs_gas.py
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)       54 2023-03-30 16:38:37.000000 gestionatr-3.1.7/requirements.txt
+-rw-rw-r--   0 eberloso  (1000) eberloso  (1000)       54 2021-06-15 06:26:33.000000 gestionatr-3.1.7/MANIFEST.in
```

### Comparing `gestionatr-3.1.6/gestionatr/parser_xml_defs_gas.py` & `gestionatr-3.1.7/gestionatr/parser_xml_defs_gas.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/utils.py` & `gestionatr-3.1.7/gestionatr/utils.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/defs.py` & `gestionatr-3.1.7/gestionatr/defs.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/helpers/funcions.py` & `gestionatr-3.1.7/gestionatr/helpers/funcions.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/cli.py` & `gestionatr-3.1.7/gestionatr/cli.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_r1.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_r1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/base_gas.py` & `gestionatr-3.1.7/gestionatr/output/messages/base_gas.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_a1_46.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_a1_46.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_a1_05.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_a1_05.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_t1.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_t1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_c1.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_c1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_d1.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_d1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_a1_41.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_a1_41.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_b2.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_b2.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_a20_36.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_a20_36.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_a1_49.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_a1_49.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_a1_43.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_a1_43.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_a25_42.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_a25_42.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_m1.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_m1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_c2.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_c2.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_a3.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_a3.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_a1_42.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_a1_42.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_a1_48.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_a1_48.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_a1_04.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_a1_04.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_p0.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_p0.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_a1_44.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_a1_44.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_f1.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_f1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/base.py` & `gestionatr-3.1.7/gestionatr/output/messages/base.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_a1_03.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_a1_03.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_a1.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_a1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_a1_02.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_a1_02.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_w1.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_w1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_a1_38.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_a1_38.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_q1.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_q1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_b1.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_b1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/output/messages/sw_e1.py` & `gestionatr-3.1.7/gestionatr/output/messages/sw_e1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/R1.py` & `gestionatr-3.1.7/gestionatr/input/messages/R1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/A12_26.py` & `gestionatr-3.1.7/gestionatr/input/messages/A12_26.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/A1.py` & `gestionatr-3.1.7/gestionatr/input/messages/A1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/Q1.py` & `gestionatr-3.1.7/gestionatr/input/messages/Q1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/A1_02.py` & `gestionatr-3.1.7/gestionatr/input/messages/A1_02.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/A1_46.py` & `gestionatr-3.1.7/gestionatr/input/messages/A1_46.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/A1_49.py` & `gestionatr-3.1.7/gestionatr/input/messages/A1_49.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/P0.py` & `gestionatr-3.1.7/gestionatr/input/messages/P0.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/A1_44.py` & `gestionatr-3.1.7/gestionatr/input/messages/A1_44.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/defs.py` & `gestionatr-3.1.7/gestionatr/input/messages/defs.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/B70.py` & `gestionatr-3.1.7/gestionatr/input/messages/B70.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/T1.py` & `gestionatr-3.1.7/gestionatr/input/messages/T1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/B1.py` & `gestionatr-3.1.7/gestionatr/input/messages/B1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/A1_48.py` & `gestionatr-3.1.7/gestionatr/input/messages/A1_48.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/message.py` & `gestionatr-3.1.7/gestionatr/input/messages/message.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/A1_43.py` & `gestionatr-3.1.7/gestionatr/input/messages/A1_43.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/A1_42.py` & `gestionatr-3.1.7/gestionatr/input/messages/A1_42.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/B2.py` & `gestionatr-3.1.7/gestionatr/input/messages/B2.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/C2.py` & `gestionatr-3.1.7/gestionatr/input/messages/C2.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/A1_38.py` & `gestionatr-3.1.7/gestionatr/input/messages/A1_38.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/A1_41.py` & `gestionatr-3.1.7/gestionatr/input/messages/A1_41.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/D1.py` & `gestionatr-3.1.7/gestionatr/input/messages/D1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/W1.py` & `gestionatr-3.1.7/gestionatr/input/messages/W1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/A1_05.py` & `gestionatr-3.1.7/gestionatr/input/messages/A1_05.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/F1.py` & `gestionatr-3.1.7/gestionatr/input/messages/F1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/A1_04.py` & `gestionatr-3.1.7/gestionatr/input/messages/A1_04.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/__init__.py` & `gestionatr-3.1.7/gestionatr/input/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/A19_45.py` & `gestionatr-3.1.7/gestionatr/input/messages/A19_45.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/M1.py` & `gestionatr-3.1.7/gestionatr/input/messages/M1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/A20_36.py` & `gestionatr-3.1.7/gestionatr/input/messages/A20_36.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/A12_24.py` & `gestionatr-3.1.7/gestionatr/input/messages/A12_24.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/Deadlines.py` & `gestionatr-3.1.7/gestionatr/input/messages/Deadlines.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/message_gas.py` & `gestionatr-3.1.7/gestionatr/input/messages/message_gas.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/E1.py` & `gestionatr-3.1.7/gestionatr/input/messages/E1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/gestionatr_maker.py` & `gestionatr-3.1.7/gestionatr/input/messages/gestionatr_maker.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/input/messages/C1.py` & `gestionatr-3.1.7/gestionatr/input/messages/C1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2S42.xsd` & `gestionatr-3.1.7/gestionatr/data/A2S42.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A103.xsd` & `gestionatr-3.1.7/gestionatr/data/A103.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A529.xsd` & `gestionatr-3.1.7/gestionatr/data/A529.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/B7033.xsd` & `gestionatr-3.1.7/gestionatr/data/B7033.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeP002.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeP002.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/ActivacionBajaSuspension.xsd` & `gestionatr-3.1.7/gestionatr/data/ActivacionBajaSuspension.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A441.xsd` & `gestionatr-3.1.7/gestionatr/data/A441.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeB201.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeB201.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2541.xsd` & `gestionatr-3.1.7/gestionatr/data/A2541.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TiposSencillos.xsd` & `gestionatr-3.1.7/gestionatr/data/TiposSencillos.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TiposComplejos.xsd` & `gestionatr-3.1.7/gestionatr/data/TiposComplejos.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeA101.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeA101.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TiposComplejosCCAA.xsd` & `gestionatr-3.1.7/gestionatr/data/TiposComplejosCCAA.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A104.xsd` & `gestionatr-3.1.7/gestionatr/data/A104.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2643.xsd` & `gestionatr-3.1.7/gestionatr/data/A2643.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2644.xsd` & `gestionatr-3.1.7/gestionatr/data/A2644.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A102.xsd` & `gestionatr-3.1.7/gestionatr/data/A102.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeT101.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeT101.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/CommonTagsATCOM.xsd` & `gestionatr-3.1.7/gestionatr/data/CommonTagsATCOM.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/SolicitudAportacionLectura.xsd` & `gestionatr-3.1.7/gestionatr/data/SolicitudAportacionLectura.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A144.xsd` & `gestionatr-3.1.7/gestionatr/data/A144.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A1350.xsd` & `gestionatr-3.1.7/gestionatr/data/A1350.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A3S02.xsd` & `gestionatr-3.1.7/gestionatr/data/A3S02.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/AceptacionReclamacion.xsd` & `gestionatr-3.1.7/gestionatr/data/AceptacionReclamacion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A142.xsd` & `gestionatr-3.1.7/gestionatr/data/A142.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A8609.xsd` & `gestionatr-3.1.7/gestionatr/data/A8609.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A219.xsd` & `gestionatr-3.1.7/gestionatr/data/A219.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/B7031.xsd` & `gestionatr-3.1.7/gestionatr/data/B7031.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A349.xsd` & `gestionatr-3.1.7/gestionatr/data/A349.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2641.xsd` & `gestionatr-3.1.7/gestionatr/data/A2641.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A1550.xsd` & `gestionatr-3.1.7/gestionatr/data/A1550.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/ContestacionIncidencia.xsd` & `gestionatr-3.1.7/gestionatr/data/ContestacionIncidencia.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/AceptacionTraspasoCOR.xsd` & `gestionatr-3.1.7/gestionatr/data/AceptacionTraspasoCOR.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/BajaSuspension.xsd` & `gestionatr-3.1.7/gestionatr/data/BajaSuspension.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/Rechazo.xsd` & `gestionatr-3.1.7/gestionatr/data/Rechazo.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/Alta.xsd` & `gestionatr-3.1.7/gestionatr/data/Alta.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/IncidenciasATRDistribuidor.xsd` & `gestionatr-3.1.7/gestionatr/data/IncidenciasATRDistribuidor.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/ActivacionTraspasoCORSaliente.xsd` & `gestionatr-3.1.7/gestionatr/data/ActivacionTraspasoCORSaliente.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/B7032.xsd` & `gestionatr-3.1.7/gestionatr/data/B7032.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A8409.xsd` & `gestionatr-3.1.7/gestionatr/data/A8409.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A341.xsd` & `gestionatr-3.1.7/gestionatr/data/A341.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/AceptacionModificacionDeATR.xsd` & `gestionatr-3.1.7/gestionatr/data/AceptacionModificacionDeATR.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A138.xsd` & `gestionatr-3.1.7/gestionatr/data/A138.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/ActivacionTraspasoCOR.xsd` & `gestionatr-3.1.7/gestionatr/data/ActivacionTraspasoCOR.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A1945.xsd` & `gestionatr-3.1.7/gestionatr/data/A1945.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/AceptacionBajaSuspension.xsd` & `gestionatr-3.1.7/gestionatr/data/AceptacionBajaSuspension.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/SolicitudInformacionAlRegistroDePS.xsd` & `gestionatr-3.1.7/gestionatr/data/SolicitudInformacionAlRegistroDePS.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeM105.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeM105.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/RechazoTraspasoCOR.xsd` & `gestionatr-3.1.7/gestionatr/data/RechazoTraspasoCOR.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A205.xsd` & `gestionatr-3.1.7/gestionatr/data/A205.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/AceptacionCambiodeComercializadorSaliente.xsd` & `gestionatr-3.1.7/gestionatr/data/AceptacionCambiodeComercializadorSaliente.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A304.xsd` & `gestionatr-3.1.7/gestionatr/data/A304.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/SaldoLecturasFacturacion.xsd` & `gestionatr-3.1.7/gestionatr/data/SaldoLecturasFacturacion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2505.xsd` & `gestionatr-3.1.7/gestionatr/data/A2505.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/RechazoPeticion.xsd` & `gestionatr-3.1.7/gestionatr/data/RechazoPeticion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/NotificacionActivacionPorDesistimiento.xsd` & `gestionatr-3.1.7/gestionatr/data/NotificacionActivacionPorDesistimiento.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A105.xsd` & `gestionatr-3.1.7/gestionatr/data/A105.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A4S41.xsd` & `gestionatr-3.1.7/gestionatr/data/A4S41.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A8509.xsd` & `gestionatr-3.1.7/gestionatr/data/A8509.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeSaliente.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeSaliente.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2538.xsd` & `gestionatr-3.1.7/gestionatr/data/A2538.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A204.xsd` & `gestionatr-3.1.7/gestionatr/data/A204.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2642.xsd` & `gestionatr-3.1.7/gestionatr/data/A2642.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/EnvioInformacionReclamacion.xsd` & `gestionatr-3.1.7/gestionatr/data/EnvioInformacionReclamacion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A302.xsd` & `gestionatr-3.1.7/gestionatr/data/A302.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A15S50.xsd` & `gestionatr-3.1.7/gestionatr/data/A15S50.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A305.xsd` & `gestionatr-3.1.7/gestionatr/data/A305.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/RechazoDesistimiento.xsd` & `gestionatr-3.1.7/gestionatr/data/RechazoDesistimiento.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/SolicitudDesistimiento.xsd` & `gestionatr-3.1.7/gestionatr/data/SolicitudDesistimiento.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/Facturacion.xsd` & `gestionatr-3.1.7/gestionatr/data/Facturacion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2604.xsd` & `gestionatr-3.1.7/gestionatr/data/A2604.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A444.xsd` & `gestionatr-3.1.7/gestionatr/data/A444.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/AceptacionAnulacionReclamacion.xsd` & `gestionatr-3.1.7/gestionatr/data/AceptacionAnulacionReclamacion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/EnvioInformacionPS.xsd` & `gestionatr-3.1.7/gestionatr/data/EnvioInformacionPS.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/AceptacionAportacionLectura.xsd` & `gestionatr-3.1.7/gestionatr/data/AceptacionAportacionLectura.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A438.xsd` & `gestionatr-3.1.7/gestionatr/data/A438.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2S03.xsd` & `gestionatr-3.1.7/gestionatr/data/A2S03.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2S41.xsd` & `gestionatr-3.1.7/gestionatr/data/A2S41.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A141.xsd` & `gestionatr-3.1.7/gestionatr/data/A141.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A629.xsd` & `gestionatr-3.1.7/gestionatr/data/A629.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/RechazoReclamacion.xsd` & `gestionatr-3.1.7/gestionatr/data/RechazoReclamacion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A21.xsd` & `gestionatr-3.1.7/gestionatr/data/A21.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/NotificacionCambiosATRDesdeDistribuidor.xsd` & `gestionatr-3.1.7/gestionatr/data/NotificacionCambiosATRDesdeDistribuidor.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/WebserviceSync.xsd` & `gestionatr-3.1.7/gestionatr/data/WebserviceSync.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A338.xsd` & `gestionatr-3.1.7/gestionatr/data/A338.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2649.xsd` & `gestionatr-3.1.7/gestionatr/data/A2649.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A143.xsd` & `gestionatr-3.1.7/gestionatr/data/A143.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeC101.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeC101.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2504.xsd` & `gestionatr-3.1.7/gestionatr/data/A2504.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/ActivacionModificacionDeATR.xsd` & `gestionatr-3.1.7/gestionatr/data/ActivacionModificacionDeATR.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A348.xsd` & `gestionatr-3.1.7/gestionatr/data/A348.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeC205.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeC205.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/RechazoCambiodeComercializadorSaliente.xsd` & `gestionatr-3.1.7/gestionatr/data/RechazoCambiodeComercializadorSaliente.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeAceptacion.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeAceptacion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeT105.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeT105.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/AceptacionDesistimiento.xsd` & `gestionatr-3.1.7/gestionatr/data/AceptacionDesistimiento.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A248.xsd` & `gestionatr-3.1.7/gestionatr/data/A248.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A242.xsd` & `gestionatr-3.1.7/gestionatr/data/A242.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeB101.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeB101.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A8009.xsd` & `gestionatr-3.1.7/gestionatr/data/A8009.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/PeticionInformacionAdicionalReclamacion.xsd` & `gestionatr-3.1.7/gestionatr/data/PeticionInformacionAdicionalReclamacion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/xml.xsd` & `gestionatr-3.1.7/gestionatr/data/xml.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/ActivacionCambiodeComercializadorConCambios.xsd` & `gestionatr-3.1.7/gestionatr/data/ActivacionCambiodeComercializadorConCambios.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2544.xsd` & `gestionatr-3.1.7/gestionatr/data/A2544.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A344.xsd` & `gestionatr-3.1.7/gestionatr/data/A344.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A342.xsd` & `gestionatr-3.1.7/gestionatr/data/A342.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A1226.xsd` & `gestionatr-3.1.7/gestionatr/data/A1226.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeC105.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeC105.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/WebserviceRPS.xsd` & `gestionatr-3.1.7/gestionatr/data/WebserviceRPS.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A246.xsd` & `gestionatr-3.1.7/gestionatr/data/A246.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A449.xsd` & `gestionatr-3.1.7/gestionatr/data/A449.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A442.xsd` & `gestionatr-3.1.7/gestionatr/data/A442.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A202.xsd` & `gestionatr-3.1.7/gestionatr/data/A202.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A243.xsd` & `gestionatr-3.1.7/gestionatr/data/A243.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A238.xsd` & `gestionatr-3.1.7/gestionatr/data/A238.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A404.xsd` & `gestionatr-3.1.7/gestionatr/data/A404.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2638.xsd` & `gestionatr-3.1.7/gestionatr/data/A2638.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/CambiodeComercializadorSinCambios.xsd` & `gestionatr-3.1.7/gestionatr/data/CambiodeComercializadorSinCambios.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/CommonTagsPETS.xsd` & `gestionatr-3.1.7/gestionatr/data/CommonTagsPETS.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A146.xsd` & `gestionatr-3.1.7/gestionatr/data/A146.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/CommonTagsCONT.xsd` & `gestionatr-3.1.7/gestionatr/data/CommonTagsCONT.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A20.xsd` & `gestionatr-3.1.7/gestionatr/data/A20.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/CambiodeComercializadorConCambios.xsd` & `gestionatr-3.1.7/gestionatr/data/CambiodeComercializadorConCambios.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/AceptacionAnulacion.xsd` & `gestionatr-3.1.7/gestionatr/data/AceptacionAnulacion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2548.xsd` & `gestionatr-3.1.7/gestionatr/data/A2548.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A405.xsd` & `gestionatr-3.1.7/gestionatr/data/A405.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A443.xsd` & `gestionatr-3.1.7/gestionatr/data/A443.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/ActivacionAlta.xsd` & `gestionatr-3.1.7/gestionatr/data/ActivacionAlta.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TiposSencillosCCAA.xsd` & `gestionatr-3.1.7/gestionatr/data/TiposSencillosCCAA.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/ActivacionCambiodeComercializadorSinCambios.xsd` & `gestionatr-3.1.7/gestionatr/data/ActivacionCambiodeComercializadorSinCambios.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A4S42.xsd` & `gestionatr-3.1.7/gestionatr/data/A4S42.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/AceptacionAlta.xsd` & `gestionatr-3.1.7/gestionatr/data/AceptacionAlta.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A6161.xsd` & `gestionatr-3.1.7/gestionatr/data/A6161.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/CierreReclamacion.xsd` & `gestionatr-3.1.7/gestionatr/data/CierreReclamacion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/ActivacionBaja.xsd` & `gestionatr-3.1.7/gestionatr/data/ActivacionBaja.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A148.xsd` & `gestionatr-3.1.7/gestionatr/data/A148.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeRechazoCCAA.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeRechazoCCAA.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A149.xsd` & `gestionatr-3.1.7/gestionatr/data/A149.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A203.xsd` & `gestionatr-3.1.7/gestionatr/data/A203.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeM101.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeM101.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeA301.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeA301.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/RechazoD1.xsd` & `gestionatr-3.1.7/gestionatr/data/RechazoD1.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A3S41.xsd` & `gestionatr-3.1.7/gestionatr/data/A3S41.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A3S42.xsd` & `gestionatr-3.1.7/gestionatr/data/A3S42.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/ModificacionDeATR.xsd` & `gestionatr-3.1.7/gestionatr/data/ModificacionDeATR.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A1224.xsd` & `gestionatr-3.1.7/gestionatr/data/A1224.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeA102.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeA102.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeB105.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeB105.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2648.xsd` & `gestionatr-3.1.7/gestionatr/data/A2648.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeE.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeE.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/AceptacionCambiodeComercializadorSinCambios.xsd` & `gestionatr-3.1.7/gestionatr/data/AceptacionCambiodeComercializadorSinCambios.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A244.xsd` & `gestionatr-3.1.7/gestionatr/data/A244.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeA305.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeA305.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A402.xsd` & `gestionatr-3.1.7/gestionatr/data/A402.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A343.xsd` & `gestionatr-3.1.7/gestionatr/data/A343.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeR105.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeR105.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeRechazo.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeRechazo.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A241.xsd` & `gestionatr-3.1.7/gestionatr/data/A241.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/ActivacionDesistimiento.xsd` & `gestionatr-3.1.7/gestionatr/data/ActivacionDesistimiento.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeC201.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeC201.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/AceptacionCambiodeComercializadorConCambios.xsd` & `gestionatr-3.1.7/gestionatr/data/AceptacionCambiodeComercializadorConCambios.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A3S49.xsd` & `gestionatr-3.1.7/gestionatr/data/A3S49.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2543.xsd` & `gestionatr-3.1.7/gestionatr/data/A2543.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/AceptacionD1.xsd` & `gestionatr-3.1.7/gestionatr/data/AceptacionD1.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2542.xsd` & `gestionatr-3.1.7/gestionatr/data/A2542.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/CommonTagsFACT.xsd` & `gestionatr-3.1.7/gestionatr/data/CommonTagsFACT.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2S02.xsd` & `gestionatr-3.1.7/gestionatr/data/A2S02.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/SolicitudTraspasoCOR.xsd` & `gestionatr-3.1.7/gestionatr/data/SolicitudTraspasoCOR.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A101.xsd` & `gestionatr-3.1.7/gestionatr/data/A101.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A4S49.xsd` & `gestionatr-3.1.7/gestionatr/data/A4S49.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2605.xsd` & `gestionatr-3.1.7/gestionatr/data/A2605.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A102e.xsd` & `gestionatr-3.1.7/gestionatr/data/A102e.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/AnulacionSolicitudReclamacion.xsd` & `gestionatr-3.1.7/gestionatr/data/AnulacionSolicitudReclamacion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A1450.xsd` & `gestionatr-3.1.7/gestionatr/data/A1450.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/ActivacionComercializadorSaliente.xsd` & `gestionatr-3.1.7/gestionatr/data/ActivacionComercializadorSaliente.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A249.xsd` & `gestionatr-3.1.7/gestionatr/data/A249.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A708.xsd` & `gestionatr-3.1.7/gestionatr/data/A708.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2549.xsd` & `gestionatr-3.1.7/gestionatr/data/A2549.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/ReclamacionPeticion.xsd` & `gestionatr-3.1.7/gestionatr/data/ReclamacionPeticion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A4S02.xsd` & `gestionatr-3.1.7/gestionatr/data/A4S02.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/AceptacionNotificacionCambiosATRDesdeDistribuidor.xsd` & `gestionatr-3.1.7/gestionatr/data/AceptacionNotificacionCambiosATRDesdeDistribuidor.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/AceptacionAnulacionBaja.xsd` & `gestionatr-3.1.7/gestionatr/data/AceptacionAnulacionBaja.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/TipoMensajeR101.xsd` & `gestionatr-3.1.7/gestionatr/data/TipoMensajeR101.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A2S49.xsd` & `gestionatr-3.1.7/gestionatr/data/A2S49.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/AnulacionSolicitud.xsd` & `gestionatr-3.1.7/gestionatr/data/AnulacionSolicitud.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/data/A8109.xsd` & `gestionatr-3.1.7/gestionatr/data/A8109.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr/defs_gas.py` & `gestionatr-3.1.7/gestionatr/defs_gas.py`

 * *Files 0% similar despite different names*

```diff
@@ -3089,14 +3089,15 @@
     'PRAJE':'PJ',
     'PRAZA':'OV',
     'PROL':'PR',
     'PSAJE':'PS',
     'PSAXE':'PS',
     'PTDA':'PD',
     'PTGE':'PS',
+    'PGE':'PS',
     'PTLLO':'OV',
     'PZO':'OV',
     'PZTA':'PT',
     'RABAL':'OV',
     'RACDA':'OV',
     'RACO':'OV',
     'RAMAL':'OV',
```

### Comparing `gestionatr-3.1.6/setup.py` & `gestionatr-3.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/gestionatr.egg-info/SOURCES.txt` & `gestionatr-3.1.7/gestionatr.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -278,9 +278,10 @@
 gestionatr/output/messages/sw_t1.py
 gestionatr/output/messages/sw_w1.py
 tests/__init__.py
 tests/test_cli.py
 tests/test_helpers.py
 tests/test_input.py
 tests/test_output.py
+tests/test_request_p0.py
 tests/test_table_description.py
 tests/utils.py
```

### Comparing `gestionatr-3.1.6/tests/utils.py` & `gestionatr-3.1.7/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/tests/test_cli.py` & `gestionatr-3.1.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/tests/test_output.py` & `gestionatr-3.1.7/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/tests/test_input.py` & `gestionatr-3.1.7/tests/test_input.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/tests/test_table_description.py` & `gestionatr-3.1.7/tests/test_table_description.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.1.6/tests/test_helpers.py` & `gestionatr-3.1.7/tests/test_helpers.py`

 * *Files identical despite different names*

