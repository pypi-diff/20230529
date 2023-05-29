# Comparing `tmp/musif-1.1.1.tar.gz` & `tmp/musif-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musif-1.1.1.tar", last modified: Thu Apr 27 15:37:01 2023, max compression
+gzip compressed data, was "musif-1.1.2.tar", last modified: Mon May 29 09:38:51 2023, max compression
```

## Comparing `musif-1.1.1.tar` & `musif-1.1.2.tar`

### file list

```diff
@@ -1,103 +1,99 @@
--rw-r--r--   0        0        0      971 2023-04-27 15:28:52.916781 musif-1.1.1/README.md
--rw-r--r--   0        0        0      258 2023-04-20 14:52:06.385051 musif-1.1.1/musif/__init__.py
--rw-r--r--   0        0        0     7344 2023-04-27 15:28:46.353448 musif-1.1.1/musif/__main__.py
--rw-r--r--   0        0        0      232 2023-04-20 14:52:06.385051 musif-1.1.1/musif/cache/__init__.py
--rw-r--r--   0        0        0    17854 2023-04-27 15:28:46.353448 musif-1.1.1/musif/cache/cache.py
--rw-r--r--   0        0        0     7606 2023-04-27 15:28:46.353448 musif-1.1.1/musif/cache/utils.py
--rw-r--r--   0        0        0        1 2023-04-20 14:52:06.388385 musif-1.1.1/musif/common/__init__.py
--rw-r--r--   0        0        0      202 2023-04-20 14:52:06.388385 musif-1.1.1/musif/common/_constants.py
--rw-r--r--   0        0        0     2402 2023-04-20 14:52:06.388385 musif-1.1.1/musif/common/_logs.py
--rw-r--r--   0        0        0     3067 2023-04-20 14:52:06.388385 musif-1.1.1/musif/common/_utils.py
--rw-r--r--   0        0        0      826 2023-04-20 14:52:06.388385 musif-1.1.1/musif/common/constants.py
--rw-r--r--   0        0        0     1700 2023-04-20 14:52:06.388385 musif-1.1.1/musif/common/didone_utils.py
--rw-r--r--   0        0        0     1175 2023-04-20 14:52:06.388385 musif-1.1.1/musif/common/exceptions.py
--rw-r--r--   0        0        0     4102 2023-04-20 14:52:06.388385 musif-1.1.1/musif/common/sort.py
--rw-r--r--   0        0        0     2103 2023-04-20 14:52:06.388385 musif-1.1.1/musif/common/translate.py
--rw-r--r--   0        0        0     7287 2023-04-27 15:28:52.916781 musif-1.1.1/musif/config.py
--rw-r--r--   0        0        0     7225 2023-04-21 13:30:56.223307 musif-1.1.1/musif/config.py~
--rw-r--r--   0        0        0       52 2023-04-20 14:52:06.388385 musif-1.1.1/musif/extract/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 14:52:06.388385 musif-1.1.1/musif/extract/basic_modules/file_name_generic/__init__.py
--rw-r--r--   0        0        0       34 2023-04-20 14:52:06.388385 musif-1.1.1/musif/extract/basic_modules/file_name_generic/constants.py
--rw-r--r--   0        0        0      999 2023-04-20 14:52:06.388385 musif-1.1.1/musif/extract/basic_modules/file_name_generic/handler.py
--rw-r--r--   0        0        0        0 2023-04-20 14:52:06.388385 musif-1.1.1/musif/extract/basic_modules/scoring/__init__.py
--rw-r--r--   0        0        0      646 2023-04-20 14:52:06.388385 musif-1.1.1/musif/extract/basic_modules/scoring/constants.py
--rw-r--r--   0        0        0     5686 2023-04-20 14:52:06.388385 musif-1.1.1/musif/extract/basic_modules/scoring/handler.py
--rw-r--r--   0        0        0     1600 2023-04-20 14:52:06.388385 musif-1.1.1/musif/extract/common.py
--rw-r--r--   0        0        0     1178 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/constants.py
--rw-r--r--   0        0        0    28678 2023-04-27 15:28:52.916781 musif-1.1.1/musif/extract/extract.py
--rw-r--r--   0        0        0    28696 2023-04-21 14:59:05.660981 musif-1.1.1/musif/extract/extract.py~
--rw-r--r--   0        0        0        0 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/__init__.py
--rw-r--r--   0        0        0       25 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/ambitus/__init__.py
--rw-r--r--   0        0        0      270 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/ambitus/constants.py
--rw-r--r--   0        0        0     2705 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/ambitus/handler.py
--rw-r--r--   0        0        0        0 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/core/__init__.py
--rw-r--r--   0        0        0      465 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/core/constants.py
--rw-r--r--   0        0        0     7246 2023-04-27 15:28:46.353448 musif-1.1.1/musif/extract/features/core/handler.py
--rw-r--r--   0        0        0       55 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/density/__init__.py
--rw-r--r--   0        0        0       57 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/density/constants.py
--rw-r--r--   0        0        0     7668 2023-04-27 15:28:46.353448 musif-1.1.1/musif/extract/features/density/handler.py
--rw-r--r--   0        0        0       25 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/dynamics/__init__.py
--rw-r--r--   0        0        0      821 2023-04-27 15:28:46.353448 musif-1.1.1/musif/extract/features/dynamics/constants.py
--rw-r--r--   0        0        0     9029 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/dynamics/handler.py
--rw-r--r--   0        0        0        0 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/harmony/__init__.py
--rw-r--r--   0        0        0      815 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/harmony/constants.py
--rw-r--r--   0        0        0     2741 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/harmony/handler.py
--rw-r--r--   0        0        0    26047 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/harmony/utils.py
--rw-r--r--   0        0        0       29 2023-04-27 15:28:52.916781 musif-1.1.1/musif/extract/features/jsymbolic/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 15:03:56.233060 musif-1.1.1/musif/extract/features/jsymbolic/__init__.py~
--rw-r--r--   0        0        0      282 2023-04-27 15:28:52.916781 musif-1.1.1/musif/extract/features/jsymbolic/__main__.py
--rw-r--r--   0        0        0      282 2023-04-20 15:03:56.233060 musif-1.1.1/musif/extract/features/jsymbolic/__main__.py~
--rw-r--r--   0        0        0     2827 2023-04-27 15:36:24.763452 musif-1.1.1/musif/extract/features/jsymbolic/handler.py
--rw-r--r--   0        0        0     2827 2023-04-27 15:35:28.226785 musif-1.1.1/musif/extract/features/jsymbolic/handler.py~
--rw-r--r--   0        0        0     3381 2023-04-27 15:28:52.920114 musif-1.1.1/musif/extract/features/jsymbolic/utils.py
--rw-r--r--   0        0        0     3379 2023-04-21 13:22:20.964657 musif-1.1.1/musif/extract/features/jsymbolic/utils.py~
--rw-r--r--   0        0        0        0 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/key/__init__.py
--rw-r--r--   0        0        0      165 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/key/constants.py
--rw-r--r--   0        0        0     1044 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/key/handler.py
--rw-r--r--   0        0        0       25 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/lyrics/__init__.py
--rw-r--r--   0        0        0      113 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/lyrics/constants.py
--rw-r--r--   0        0        0     3669 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/lyrics/handler.py
--rw-r--r--   0        0        0       25 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/melody/__init__.py
--rw-r--r--   0        0        0    10534 2023-04-27 15:28:46.353448 musif-1.1.1/musif/extract/features/melody/constants.py
--rw-r--r--   0        0        0    30504 2023-04-27 15:28:46.353448 musif-1.1.1/musif/extract/features/melody/handler.py
--rw-r--r--   0        0        0       80 2023-04-27 15:28:46.353448 musif-1.1.1/musif/extract/features/music21/__init__.py
--rw-r--r--   0        0        0      173 2023-04-27 15:28:52.920114 musif-1.1.1/musif/extract/features/music21/constants.py
--rw-r--r--   0        0        0      174 2023-04-21 14:21:18.728272 musif-1.1.1/musif/extract/features/music21/constants.py~
--rw-r--r--   0        0        0     2182 2023-04-27 15:28:52.920114 musif-1.1.1/musif/extract/features/music21/handler.py
--rw-r--r--   0        0        0     2109 2023-04-21 14:26:52.742891 musif-1.1.1/musif/extract/features/music21/handler.py~
--rw-r--r--   0        0        0     3554 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/prefix.py
--rw-r--r--   0        0        0        0 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/rhythm/__init__.py
--rw-r--r--   0        0        0      273 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/rhythm/constants.py
--rw-r--r--   0        0        0     5925 2023-04-27 15:28:46.353448 musif-1.1.1/musif/extract/features/rhythm/handler.py
--rw-r--r--   0        0        0        0 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/scale/__init__.py
--rw-r--r--   0        0        0      269 2023-04-27 15:28:46.356781 musif-1.1.1/musif/extract/features/scale/constants.py
--rw-r--r--   0        0        0     3627 2023-04-20 14:52:06.398385 musif-1.1.1/musif/extract/features/scale/handler.py
--rw-r--r--   0        0        0        0 2023-04-20 14:52:06.398385 musif-1.1.1/musif/extract/features/scale_relative/__init__.py
--rw-r--r--   0        0        0      102 2023-04-20 14:52:06.398385 musif-1.1.1/musif/extract/features/scale_relative/constants.py
--rw-r--r--   0        0        0     2842 2023-04-20 14:52:06.398385 musif-1.1.1/musif/extract/features/scale_relative/handler.py
--rw-r--r--   0        0        0     7321 2023-04-20 14:52:06.398385 musif-1.1.1/musif/extract/features/scale_relative/utils.py
--rw-r--r--   0        0        0        0 2023-04-20 14:52:06.398385 musif-1.1.1/musif/extract/features/tempo/__init__.py
--rw-r--r--   0        0        0      306 2023-04-20 14:52:06.398385 musif-1.1.1/musif/extract/features/tempo/constants.py
--rw-r--r--   0        0        0     5145 2023-04-27 15:28:46.356781 musif-1.1.1/musif/extract/features/tempo/handler.py
--rw-r--r--   0        0        0        0 2023-04-20 14:52:06.398385 musif-1.1.1/musif/extract/features/texture/__init__.py
--rw-r--r--   0        0        0       45 2023-04-20 14:52:06.398385 musif-1.1.1/musif/extract/features/texture/constants.py
--rw-r--r--   0        0        0     3077 2023-04-20 14:52:06.398385 musif-1.1.1/musif/extract/features/texture/handler.py
--rw-r--r--   0        0        0    21081 2023-04-27 15:28:46.356781 musif-1.1.1/musif/extract/utils.py
--rw-r--r--   0        0        0    21081 2023-04-20 15:03:44.999752 musif-1.1.1/musif/extract/utils.py~
--rw-r--r--   0        0        0     2011 2023-04-20 14:52:06.398385 musif-1.1.1/musif/logs.py
--rw-r--r--   0        0        0       61 2023-04-20 14:52:06.398385 musif-1.1.1/musif/musescore/__init__.py
--rw-r--r--   0        0        0      948 2023-04-20 14:52:06.398385 musif-1.1.1/musif/musescore/common.py
--rw-r--r--   0        0        0       95 2023-04-20 14:52:06.398385 musif-1.1.1/musif/musescore/constants.py
--rw-r--r--   0        0        0       91 2023-04-20 14:52:06.398385 musif-1.1.1/musif/musicxml/__init__.py
--rw-r--r--   0        0        0     7532 2023-04-27 15:28:46.356781 musif-1.1.1/musif/musicxml/common.py
--rw-r--r--   0        0        0    15310 2023-04-27 15:28:46.356781 musif-1.1.1/musif/musicxml/constants.py
--rw-r--r--   0        0        0     2092 2023-04-20 14:52:06.401718 musif-1.1.1/musif/musicxml/key.py
--rw-r--r--   0        0        0    17541 2023-04-20 14:52:06.401718 musif-1.1.1/musif/musicxml/repeat.py
--rw-r--r--   0        0        0     4513 2023-04-27 15:28:46.356781 musif-1.1.1/musif/musicxml/scoring.py
--rw-r--r--   0        0        0     8151 2023-04-27 15:28:46.356781 musif-1.1.1/musif/musicxml/tempo.py
--rw-r--r--   0        0        0        0 2023-04-20 14:52:06.401718 musif-1.1.1/musif/process/__init__.py
--rw-r--r--   0        0        0      410 2023-04-20 14:52:06.401718 musif-1.1.1/musif/process/constants.py
--rw-r--r--   0        0        0    11327 2023-04-27 15:28:46.356781 musif-1.1.1/musif/process/processor.py
--rw-r--r--   0        0        0     7824 2023-04-27 15:28:46.356781 musif-1.1.1/musif/process/utils.py
--rw-r--r--   0        0        0      650 2023-04-27 15:36:49.866786 musif-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 musif-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2143 2023-05-29 09:31:41.363076 musif-1.1.2/README.md
+-rw-r--r--   0        0        0      258 2023-04-19 09:15:49.949723 musif-1.1.2/musif/__init__.py
+-rw-r--r--   0        0        0     7344 2023-04-26 14:35:45.753205 musif-1.1.2/musif/__main__.py
+-rw-r--r--   0        0        0      232 2023-04-19 09:14:37.169723 musif-1.1.2/musif/cache/__init__.py
+-rw-r--r--   0        0        0    17854 2023-04-26 14:35:45.753205 musif-1.1.2/musif/cache/cache.py
+-rw-r--r--   0        0        0     7606 2023-04-26 14:35:45.753205 musif-1.1.2/musif/cache/utils.py
+-rw-r--r--   0        0        0        1 2023-04-19 09:14:37.169723 musif-1.1.2/musif/common/__init__.py
+-rw-r--r--   0        0        0      202 2023-04-19 09:14:37.169723 musif-1.1.2/musif/common/_constants.py
+-rw-r--r--   0        0        0     2402 2023-04-19 09:14:37.169723 musif-1.1.2/musif/common/_logs.py
+-rw-r--r--   0        0        0     3067 2023-04-19 09:14:37.169723 musif-1.1.2/musif/common/_utils.py
+-rw-r--r--   0        0        0      826 2023-04-19 09:14:37.169723 musif-1.1.2/musif/common/constants.py
+-rw-r--r--   0        0        0     1700 2023-04-19 09:14:37.169723 musif-1.1.2/musif/common/didone_utils.py
+-rw-r--r--   0        0        0     1175 2023-04-19 09:14:37.169723 musif-1.1.2/musif/common/exceptions.py
+-rw-r--r--   0        0        0     4102 2023-04-19 09:14:37.169723 musif-1.1.2/musif/common/sort.py
+-rw-r--r--   0        0        0     2103 2023-04-19 09:14:37.169723 musif-1.1.2/musif/common/translate.py
+-rw-r--r--   0        0        0     7287 2023-04-26 14:35:45.753205 musif-1.1.2/musif/config.py
+-rw-r--r--   0        0        0       52 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:15:49.949723 musif-1.1.2/musif/extract/basic_modules/file_name_generic/__init__.py
+-rw-r--r--   0        0        0       34 2023-04-19 09:15:49.949723 musif-1.1.2/musif/extract/basic_modules/file_name_generic/constants.py
+-rw-r--r--   0        0        0      999 2023-04-19 09:15:49.949723 musif-1.1.2/musif/extract/basic_modules/file_name_generic/handler.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/basic_modules/scoring/__init__.py
+-rw-r--r--   0        0        0      646 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/basic_modules/scoring/constants.py
+-rw-r--r--   0        0        0     5686 2023-05-29 08:41:47.409829 musif-1.1.2/musif/extract/basic_modules/scoring/handler.py
+-rw-r--r--   0        0        0     1600 2023-04-19 09:15:49.949723 musif-1.1.2/musif/extract/common.py
+-rw-r--r--   0        0        0     1178 2023-04-19 09:15:49.949723 musif-1.1.2/musif/extract/constants.py
+-rw-r--r--   0        0        0    28678 2023-05-29 08:47:17.936486 musif-1.1.2/musif/extract/extract.py
+-rw-r--r--   0        0        0    28677 2023-04-19 11:27:49.216307 musif-1.1.2/musif/extract/extract.py~
+-rw-r--r--   0        0        0        0 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/features/__init__.py
+-rw-r--r--   0        0        0       25 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/features/ambitus/__init__.py
+-rw-r--r--   0        0        0      270 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/features/ambitus/constants.py
+-rw-r--r--   0        0        0     2705 2023-04-19 09:15:49.949723 musif-1.1.2/musif/extract/features/ambitus/handler.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/features/core/__init__.py
+-rw-r--r--   0        0        0      465 2023-04-19 09:15:49.949723 musif-1.1.2/musif/extract/features/core/constants.py
+-rw-r--r--   0        0        0     7246 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/core/handler.py
+-rw-r--r--   0        0        0       55 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/features/density/__init__.py
+-rw-r--r--   0        0        0       57 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/features/density/constants.py
+-rw-r--r--   0        0        0     7668 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/density/handler.py
+-rw-r--r--   0        0        0       25 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/features/dynamics/__init__.py
+-rw-r--r--   0        0        0      821 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/dynamics/constants.py
+-rw-r--r--   0        0        0     9029 2023-04-19 09:15:49.949723 musif-1.1.2/musif/extract/features/dynamics/handler.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/features/harmony/__init__.py
+-rw-r--r--   0        0        0      815 2023-04-19 09:14:37.173057 musif-1.1.2/musif/extract/features/harmony/constants.py
+-rw-r--r--   0        0        0     2741 2023-04-19 09:15:49.949723 musif-1.1.2/musif/extract/features/harmony/handler.py
+-rw-r--r--   0        0        0    26047 2023-04-19 09:15:49.949723 musif-1.1.2/musif/extract/features/harmony/utils.py
+-rw-r--r--   0        0        0       29 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/jsymbolic/__init__.py
+-rw-r--r--   0        0        0      282 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/jsymbolic/__main__.py
+-rw-r--r--   0        0        0      234 2023-04-19 11:25:57.299641 musif-1.1.2/musif/extract/features/jsymbolic/__main__.py~
+-rw-r--r--   0        0        0     2827 2023-05-29 08:39:41.526500 musif-1.1.2/musif/extract/features/jsymbolic/handler.py
+-rw-r--r--   0        0        0     1809 2023-04-19 11:32:59.902970 musif-1.1.2/musif/extract/features/jsymbolic/handler.py~
+-rw-r--r--   0        0        0     3381 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/jsymbolic/utils.py
+-rw-r--r--   0        0        0     2315 2023-04-19 11:25:00.146309 musif-1.1.2/musif/extract/features/jsymbolic/utils.py~
+-rw-r--r--   0        0        0        0 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/key/__init__.py
+-rw-r--r--   0        0        0      165 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/key/constants.py
+-rw-r--r--   0        0        0     1044 2023-04-19 09:15:49.949723 musif-1.1.2/musif/extract/features/key/handler.py
+-rw-r--r--   0        0        0       25 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/lyrics/__init__.py
+-rw-r--r--   0        0        0      113 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/lyrics/constants.py
+-rw-r--r--   0        0        0     3669 2023-04-19 09:15:49.953056 musif-1.1.2/musif/extract/features/lyrics/handler.py
+-rw-r--r--   0        0        0       25 2023-04-19 09:15:49.953056 musif-1.1.2/musif/extract/features/melody/__init__.py
+-rw-r--r--   0        0        0    10534 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/melody/constants.py
+-rw-r--r--   0        0        0    30504 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/melody/handler.py
+-rw-r--r--   0        0        0       80 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/music21/__init__.py
+-rw-r--r--   0        0        0      173 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/music21/constants.py
+-rw-r--r--   0        0        0     2182 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/music21/handler.py
+-rw-r--r--   0        0        0     1919 2023-04-19 11:30:50.492972 musif-1.1.2/musif/extract/features/music21/handler.py~
+-rw-r--r--   0        0        0     3554 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/prefix.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/rhythm/__init__.py
+-rw-r--r--   0        0        0      273 2023-04-19 09:15:49.953056 musif-1.1.2/musif/extract/features/rhythm/constants.py
+-rw-r--r--   0        0        0     5925 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/rhythm/handler.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/scale/__init__.py
+-rw-r--r--   0        0        0      269 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/scale/constants.py
+-rw-r--r--   0        0        0     3627 2023-04-19 09:15:49.953056 musif-1.1.2/musif/extract/features/scale/handler.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/scale_relative/__init__.py
+-rw-r--r--   0        0        0      102 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/scale_relative/constants.py
+-rw-r--r--   0        0        0     2842 2023-04-19 09:15:49.953056 musif-1.1.2/musif/extract/features/scale_relative/handler.py
+-rw-r--r--   0        0        0     7321 2023-04-19 09:15:49.953056 musif-1.1.2/musif/extract/features/scale_relative/utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/tempo/__init__.py
+-rw-r--r--   0        0        0      306 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/tempo/constants.py
+-rw-r--r--   0        0        0     5145 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/features/tempo/handler.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/texture/__init__.py
+-rw-r--r--   0        0        0       45 2023-04-19 09:14:37.176390 musif-1.1.2/musif/extract/features/texture/constants.py
+-rw-r--r--   0        0        0     3077 2023-04-19 09:15:49.953056 musif-1.1.2/musif/extract/features/texture/handler.py
+-rw-r--r--   0        0        0    21081 2023-04-26 14:35:45.753205 musif-1.1.2/musif/extract/utils.py
+-rw-r--r--   0        0        0     2011 2023-04-19 09:14:37.176390 musif-1.1.2/musif/logs.py
+-rw-r--r--   0        0        0       61 2023-04-19 09:15:49.953056 musif-1.1.2/musif/musescore/__init__.py
+-rw-r--r--   0        0        0      948 2023-04-19 09:14:37.176390 musif-1.1.2/musif/musescore/common.py
+-rw-r--r--   0        0        0       95 2023-04-19 09:15:49.953056 musif-1.1.2/musif/musescore/constants.py
+-rw-r--r--   0        0        0       91 2023-04-19 09:15:49.953056 musif-1.1.2/musif/musicxml/__init__.py
+-rw-r--r--   0        0        0     7670 2023-05-29 09:27:28.939750 musif-1.1.2/musif/musicxml/common.py
+-rw-r--r--   0        0        0    15310 2023-04-26 14:35:45.753205 musif-1.1.2/musif/musicxml/constants.py
+-rw-r--r--   0        0        0     2092 2023-04-19 09:15:49.953056 musif-1.1.2/musif/musicxml/key.py
+-rw-r--r--   0        0        0    17541 2023-04-19 09:14:37.179723 musif-1.1.2/musif/musicxml/repeat.py
+-rw-r--r--   0        0        0     4513 2023-04-26 14:35:45.753205 musif-1.1.2/musif/musicxml/scoring.py
+-rw-r--r--   0        0        0     8151 2023-04-26 14:35:45.753205 musif-1.1.2/musif/musicxml/tempo.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:14:37.179723 musif-1.1.2/musif/process/__init__.py
+-rw-r--r--   0        0        0      410 2023-04-19 09:15:49.953056 musif-1.1.2/musif/process/constants.py
+-rw-r--r--   0        0        0    11327 2023-04-26 14:35:45.756538 musif-1.1.2/musif/process/processor.py
+-rw-r--r--   0        0        0     7824 2023-04-26 14:35:45.756538 musif-1.1.2/musif/process/utils.py
+-rw-r--r--   0        0        0      650 2023-05-29 09:27:28.939750 musif-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2384 1970-01-01 00:00:00.000000 musif-1.1.2/PKG-INFO
```

### Comparing `musif-1.1.1/musif/__main__.py` & `musif-1.1.2/musif/__main__.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/cache/cache.py` & `musif-1.1.2/musif/cache/cache.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/cache/utils.py` & `musif-1.1.2/musif/cache/utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/common/_logs.py` & `musif-1.1.2/musif/common/_logs.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/common/_utils.py` & `musif-1.1.2/musif/common/_utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/common/constants.py` & `musif-1.1.2/musif/common/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/common/didone_utils.py` & `musif-1.1.2/musif/common/didone_utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/common/exceptions.py` & `musif-1.1.2/musif/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/common/sort.py` & `musif-1.1.2/musif/common/sort.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/common/translate.py` & `musif-1.1.2/musif/common/translate.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/config.py` & `musif-1.1.2/musif/config.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/basic_modules/file_name_generic/handler.py` & `musif-1.1.2/musif/extract/basic_modules/file_name_generic/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/basic_modules/scoring/constants.py` & `musif-1.1.2/musif/extract/basic_modules/scoring/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/basic_modules/scoring/handler.py` & `musif-1.1.2/musif/extract/basic_modules/scoring/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/common.py` & `musif-1.1.2/musif/extract/common.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/constants.py` & `musif-1.1.2/musif/extract/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/extract.py` & `musif-1.1.2/musif/extract/extract.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/extract.py~` & `musif-1.1.2/musif/extract/extract.py~`

 * *Files 1% similar despite different names*

```diff
@@ -250,20 +250,20 @@
         )
         # self.regex = re.compile("from {FEATURES_MODULES}.([\w\.]+) import")
         # creates the directory for the cache
         if self._cfg.cache_dir is not None:
             pinfo("Cache activated!")
             Path(self._cfg.cache_dir).mkdir(exist_ok=True)
 
-        if "jsymbolic" in self._cfg.features:
+        if 'jsymbolic' in self._cfg.features:
             from musif.extract.features import jsymbolic
-
             jsymbolic.utils.download_jsymbolic()
             jsymbolic.utils.get_java_path()
 
+
     def extract(self) -> DataFrame:
         """
         Extracts features given in the configuration data getting a file, directory or several file paths,
         returning a DataFrame containing musical features.
 
         Returns
         ------
@@ -344,21 +344,21 @@
         )
 
         if self._cfg.window_size is not None:
             all_dfs = []
             for score in scores_features:
                 df_score = DataFrame(score)
                 df_score = df_score.reindex(sorted(df_score.columns), axis=1)
-                df_score.replace(["NA", "NaN"], pd.NA, inplace=True)
+                df_score.replace("NA", pd.NA, inplace=True)
                 all_dfs.append(df_score)
             all_dfs = pd.concat(all_dfs, axis=0, keys=range(len(all_dfs)))
         else:
             all_dfs = DataFrame(scores_features)
             all_dfs = all_dfs.reindex(sorted(all_dfs.columns), axis=1)
-            all_dfs = all_dfs.replace(["NA", "NaN"], pd.NA)
+            all_dfs = all_dfs.replace(pd.NA, "NA").replace("NA", pd.NA)
         return all_dfs
 
     def _init_score_processing(self, idx: int, filename: PurePath):
         if self._cfg.cache_dir is not None:
             cache_name = (
                 Path(self._cfg.cache_dir)
                 / filename.parent
@@ -450,18 +450,16 @@
 
     def _select_window_data(
         self, score_data: dict, parts_data: list, first_measure: int, last_measure: int
     ):
         window_score = score_data[C.DATA_SCORE].measures(
             first_measure, last_measure, indicesNotNumbers=True
         )
-        filtered_partNames = [i.partName for i in score_data["parts"]]
-        window_parts = [
-            i for i in window_score.parts if i.partName in filtered_partNames
-        ]
+        filtered_partNames = [i.partName for i in score_data['parts']]
+        window_parts = [i for i in window_score.parts if i.partName in filtered_partNames]
         if (
             self._cfg.is_requested_musescore_file()
             and score_data[C.DATA_MUSESCORE_SCORE] is not None
         ):
             window_mscore = score_data[C.DATA_MUSESCORE_SCORE].loc[
                 (score_data[C.DATA_MUSESCORE_SCORE]["mn"] <= last_measure)
                 & (score_data[C.DATA_MUSESCORE_SCORE]["mn"] >= first_measure)
```

### Comparing `musif-1.1.1/musif/extract/features/ambitus/handler.py` & `musif-1.1.2/musif/extract/features/ambitus/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/features/core/handler.py` & `musif-1.1.2/musif/extract/features/core/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/features/density/handler.py` & `musif-1.1.2/musif/extract/features/density/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/features/dynamics/constants.py` & `musif-1.1.2/musif/extract/features/dynamics/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/features/dynamics/handler.py` & `musif-1.1.2/musif/extract/features/dynamics/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/features/harmony/constants.py` & `musif-1.1.2/musif/extract/features/harmony/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/features/harmony/handler.py` & `musif-1.1.2/musif/extract/features/harmony/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/features/harmony/utils.py` & `musif-1.1.2/musif/extract/features/harmony/utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/features/jsymbolic/handler.py` & `musif-1.1.2/musif/extract/features/jsymbolic/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/features/jsymbolic/handler.py~` & `musif-1.1.2/musif/extract/features/jsymbolic/handler.py~`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from typing import List
 from musif.config import ExtractConfiguration
 
-import contextlib
 import os
 import tempfile
 import subprocess
 import pandas as pd
 
-import musif.extract.constants as C
-from musif.logs import pwarn
 from musif.extract.features.jsymbolic.utils import get_java_path, _jsymbolic_path
 
-JSYMBOLIC_JAR = str(_jsymbolic_path())
+JSYMBOLIC_JAR = _jsymbolic_path()
 JAVA_PATH = get_java_path()
 
 
 def get_tmpdir():
     if os.path.exists("/dev/shm"):
         return tempfile.TemporaryDirectory(dir="/dev/shm")
     else:
@@ -28,56 +25,37 @@
     cfg: ExtractConfiguration,
     parts_features: List[dict],
     score_features: dict,
 ):
     # 1. create a temporary directory (if Linux, force RAM usig /dev/shm)
     with get_tmpdir() as tmpdirname:
         # 2. convert the score to MEI usiing music21
-        # TODO: if music21 implements export to MEI, use it
-        midi_path = os.path.abspath(os.path.join(tmpdirname, "score.midi"))
-        try:
-            with open(os.devnull, 'w') as devnull:
-                with contextlib.redirect_stdout(devnull):
-                    score_data['score'].write("MIDI", midi_path)
-        except Exception as e:
-            filename = score_data[C.DATA_FILE]
-            pwarn(f"jSymbolic: could not convert {filename} to MIDI: {e}")
-            return
-
+        mei_path = os.path.join(tmpdirname, "score.mei")
+        score_data.write("MEI", mei_path)
         # 3. run the MEI file through the jSymbolic jar savign csv into the temporary
         # directory in RAM
-        out_path = os.path.abspath(os.path.join(tmpdirname, "features"))
-        cmd = [JAVA_PATH,
-               f"-Xmx{cfg.jsymbolic_max_ram}",
-               "-jar",
-               JSYMBOLIC_JAR,
-               "-csv",
-               ]
-        if cfg.jsymbolic_config_file is not None:
-            cmd += ["-configrun", cfg.jsymbolic_config_file]
-        try:
-            subprocess.run(
-                cmd + [
-                    midi_path,
-                    out_path + ".xml",
-                    out_path + "_def.xml",
-                ],
-                check=True,
-                stdout=subprocess.DEVNULL,
-            )
-        except Exception as e:
-            filename = score_data[C.DATA_FILE]
-            pwarn(f"jSymbolic: cannot run jSymbolic on {filename}: {e}")
-            return
+        out_path = os.path.join(tmpdirname, "features")
+        subprocess.run(
+            [
+                JAVA_PATH,
+                "-Xmx25g",
+                "-jar",
+                JSYMBOLIC_JAR,
+                "-csv",
+                mei_path,
+                out_path + ".xml",
+                out_path + "_def.xml",
+            ],
+            check=True,
+        )
         # 4. read the csv file into a pandas dataframe
-        df = pd.read_csv(out_path + ".csv", na_values=["NaN", " NaN", "NaN ", " NaN "])
-        df = df.drop(columns=df.columns[0])
+        df = pd.read_csv(out_path + ".csv")
         # 5. add `js_` prefix to the column names
         df.columns = ["js_" + c for c in df.columns]
         # 6. load the features into the score_features dictionary
-        score_features.update(df.to_dict(orient='records')[0])
+        score_features.update(df.to_dict())
 
 
 def update_part_objects(
     score_data: dict, part_data: dict, cfg: ExtractConfiguration, part_features: dict
 ):
     pass
```

### Comparing `musif-1.1.1/musif/extract/features/jsymbolic/utils.py` & `musif-1.1.2/musif/extract/features/jsymbolic/utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/features/key/handler.py` & `musif-1.1.2/musif/extract/features/key/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/features/lyrics/handler.py` & `musif-1.1.2/musif/extract/features/lyrics/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/features/melody/constants.py` & `musif-1.1.2/musif/extract/features/melody/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/features/melody/handler.py` & `musif-1.1.2/musif/extract/features/melody/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/features/music21/handler.py` & `musif-1.1.2/musif/extract/features/music21/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/features/music21/handler.py~` & `musif-1.1.2/musif/extract/features/music21/handler.py~`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from typing import List
 
 import music21 as m21
 from music21.features import jSymbolic, native
-from music21.features.base import extractorsById
 
 from musif import cache
 from musif.config import ExtractConfiguration
 from musif.extract.constants import DATA_SCORE
-from .constants import ERRORED_NAMES
+from .constants import COLUMNS, ERRORED_NAMES
 
 
 def allFeaturesAsList(streamInput, includeJSymbolic=True):
     """
     only a little change around m21.features.base.allFeaturesAsList: no Parallel
     processing
     """
@@ -44,21 +43,18 @@
     score = score_data[DATA_SCORE]
     # override the isinstance and hasattr definitions for the caching system
     m21.features.base.isinstance = cache.isinstance
     m21.features.base.hasattr = cache.hasattr
     # avoid extracting jsymbolic features twice
     includeJSymbolic = 'jsymbolic' in cfg.features
     features = allFeaturesAsList(score, includeJSymbolic=includeJSymbolic)
-    if includeJSymbolic:
-        all_columns = [x.id for x in extractorsById("all")]
-    columns = [c for c in all_columns if c not in ERRORED_NAMES]
     score_features.update(
         {
-            'm21_' + columns[outer] + f"_{i}": f
-            for outer in range(len(columns))
+            'm21_' + COLUMNS[outer] + f"_{i}": f
+            for outer in range(len(COLUMNS))
             for i, f in enumerate(features[outer])
         }
     )
 
 
 def update_part_objects(
     score_data: dict, part_data: dict, cfg: ExtractConfiguration, part_features: dict
```

### Comparing `musif-1.1.1/musif/extract/features/prefix.py` & `musif-1.1.2/musif/extract/features/prefix.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/features/rhythm/handler.py` & `musif-1.1.2/musif/extract/features/rhythm/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/features/scale/handler.py` & `musif-1.1.2/musif/extract/features/scale/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/features/scale_relative/handler.py` & `musif-1.1.2/musif/extract/features/scale_relative/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/features/scale_relative/utils.py` & `musif-1.1.2/musif/extract/features/scale_relative/utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/features/tempo/handler.py` & `musif-1.1.2/musif/extract/features/tempo/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/features/texture/handler.py` & `musif-1.1.2/musif/extract/features/texture/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/utils.py` & `musif-1.1.2/musif/extract/utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/extract/utils.py~` & `musif-1.1.2/musif/musicxml/repeat.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,126 +1,63 @@
 import itertools
-from typing import Union
+from typing import List
 
-import ms3
-import music21 as m21
-import pandas as pd
-from music21.stream.base import Measure
-from pandas import DataFrame
-
-import musif.extract.constants as C
-from musif.cache import isinstance
-from musif.extract.constants import PLAYTHROUGH
-from musif.logs import pwarn
-from musif.musicxml.tempo import get_number_of_beats
-
-file_names = []
-repeat_bracket = False
-
-
-def process_musescore_file(file_path: str, expand_repeats: bool = False) -> DataFrame:
-    """
-    Given a mscx file name, parses the file using ms3 library and returns a dataframe containing all harmonic information.
-    Adds Playthrough column that contains number of every measure in the cronological order
-    Parameters
-    ----------
-    file_path: str
-        Path to mscx file
-    expand_repeats: bool
-        Directory path to musescore file
-    Returns
-    -------
-    harmonic_analysis: str
-        Dataframe containing harmonic information
-    """
-
-    msc3_score = ms3.score.Score(file_path, logger_cfg={"level": "ERROR"})
-    harmonic_analysis = msc3_score.mscx.expanded()
-    harmonic_analysis.reset_index(inplace=True)
-    if expand_repeats:
-        harmonic_analysis = msc3_score.mscx.expanded(unfold=True)
-        harmonic_analysis.reset_index(inplace=True)
-        # unfolded_mc=msc3_score.mscx.measures().set_index("mc").next
-        # mn = next2sequence(unfolded_mc)
-        # mn = ms3.utils.next2sequence(unfolded_mc)
-        # mn = pd.Series(mn, name="mc_playthrough")
-        # harmonic_analysis = ms3.utils.unfold_repeats(harmonic_analysis, mn)
-        harmonic_analysis.rename(columns={"mc_playthrough": PLAYTHROUGH}, inplace=True)
-    else:
-        harmonic_analysis = msc3_score.mscx.expanded()
-        harmonic_analysis.reset_index(inplace=True)
-        if harmonic_analysis.mn[0] == 0:
-            harmonic_analysis[PLAYTHROUGH] = harmonic_analysis["mc"]
-        else:
-            harmonic_analysis[PLAYTHROUGH] = harmonic_analysis["mn"]
-    _include_beats_column(harmonic_analysis)
-    return harmonic_analysis
-
-
-def expand_score_repetitions(score, repeat_elements: list):
-    """
-    Given a music21 Score object and a list containing repetition elements, expands the score object and
-    places all measures in their correspondent cronological order
-    Parameters
-    ----------
-    score: music21 Score
-        Score object parsed by music21
-    expand_repeats: list
-        List containing all repetition elements
-    Returns
-    -------
-    final_score: music21 Score
-        Score object with expanded repetitions
-    """
-
-    score = _expand_repeat_bars(score)
-    final_score = m21.stream.Score()
-    final_score.metadata = score.metadata
-
-    if len(repeat_elements) > 0:
-        for part in score.parts:
-            p = _expand_part(part, repeat_elements)
-
-            final_score.insert(0, p)
-    else:
-        final_score = score
-    return final_score
-
-
-def _measure_ranges(
-    instrument_measures: int,
-    init: int,
-    end: int,
-    iteration: int = None,
-    offset: int = None,
-    twocompasses_flag: bool = False,
-    remove_repetition_marks_flag: bool = False,
-) -> list:
+from music21.bar import Repeat
+from music21.chord import Chord
+from music21.meter import TimeSignature
+from music21.note import Note, Rest
+from music21.repeat import RepeatMark
+from music21.spanner import RepeatBracket, Slur
+from music21.stream import Measure, Part, Score
+
+from musif.logs import ldebug
+
+# TODO: document this module
+
+
+def measure_ranges(
+    instrument_measures,
+    init,
+    end,
+    iteration=None,
+    offset=None,
+    twoCompasses=False,
+    remove_repetition_marks=False,
+):
     measures = []
     o = offset
     last_offset = (
         0.0 if int(init) - 6 < 0 else instrument_measures[int(init) - 6].offset
     )
 
-    init_index, end_index = _find_init_and_end_indexes(instrument_measures, init, end)
+    # Find index where measureNumber init and end is stored
+    init_index = instrument_measures.index(
+        [m for m in instrument_measures if m.measureNumber == init][0]
+    )
+    end_compass = [m for m in instrument_measures if m.measureNumber == end]
+    end_index = (
+        instrument_measures.index(end_compass[0])
+        if len(end_compass) > 0
+        else len(instrument_measures) - 1
+    )
     for i in range(init_index, end_index + 1):
         if (
             not i < 0
             and i < len(instrument_measures)
             and instrument_measures[i].measureNumber >= int(init)
             and instrument_measures[i].measureNumber <= int(end)
         ):
-            if not twocompasses_flag:
+            if not twoCompasses:
                 compass = instrument_measures[i].quarterLength
-                m = m21.stream.Measure(number=instrument_measures[i].measureNumber)
-                if remove_repetition_marks_flag:
+                m = Measure(number=instrument_measures[i].measureNumber)
+                if remove_repetition_marks:
                     m.elements = [
                         e
                         for e in instrument_measures[i].elements
-                        if not isinstance(e, m21.repeat.RepeatMark)
+                        if not isinstance(e, RepeatMark)
                     ]
                 else:
                     m.elements = instrument_measures[i].elements
                 m.quarterLength = compass
                 if offset is None:
                     m.offset = last_offset
                 else:
@@ -129,477 +66,385 @@
 
                 measures.append(m)
                 if (
                     instrument_measures[i].measureNumber != 0.0
                     and instrument_measures[i].offset != 0
                 ):
                     last_offset = instrument_measures[i].offset + compass
-            twocompasses_flag = False
+            twoCompasses = False
 
+    """if iteration is 1:
+        measures = measures[:-1]
+    elif iteration is 2:
+        measures = measures[:-2] + [measures[-1]]"""
     if iteration == 2:
         last_measure = instrument_measures[i + 1]
         last_measure.offset = measures[-1].offset
         measures = measures[:-1] + [last_measure]
     return measures
 
 
-def _find_init_and_end_indexes(
-    instrument_measures: list, init: int, end: int
-) -> Union[int, int]:
-    init_index = instrument_measures.index(
-        [m for m in instrument_measures if m.measureNumber == init][0]
-    )
-    end_compass = [m for m in instrument_measures if m.measureNumber == end]
-    end_index = (
-        instrument_measures.index(end_compass[0])
-        if len(end_compass) > 0
-        else len(instrument_measures) - 1
-    )
-    return init_index, end_index
-
-
-def _get_instrument_elements(part):
-    measures = []
-    for elem in part:
-        if isinstance(elem, m21.stream.Measure):
-            measures.append(elem)
-            # Change the note offsets to avoid problems due to the slurs
-            last_offset = 0
-            last_duration = 0
-            for note in elem:
-                if (
-                    isinstance(note, m21.note.Note)
-                    or isinstance(note, m21.note.Rest)
-                    or isinstance(note, m21.chord.Chord)
-                ):
-                    note.offset = last_offset + last_duration
-                    last_offset = note.offset
-                    last_duration = note.duration.quarterLength
-    return measures
-
-
-def get_repetition_elements(score, v=True):
-    global repeat_bracket
-    repeat_bracket = False
-    repeat_elements = set()
-
-    for instruments in score.parts:
-        instr_repeat_elements = []
-        for elem in instruments.elements:
-            if isinstance(elem, m21.stream.Measure):
-                for e in elem:
-                    if isinstance(e, m21.repeat.RepeatMark) and not isinstance(
-                        e, m21.bar.Repeat
-                    ):
-                        measure = e.measureNumber
-                        if elem.numberSuffix in ["X1", "X2"]:  # Exception
-                            measure += 1
-                        instr_repeat_elements.append((measure, e.name))
-            elif isinstance(elem, m21.spanner.RepeatBracket):
-                repeat_bracket = True
-                string_e = str(elem)
-                index = string_e.find("music21.stream.Measure")
-                string_e = string_e[index:].replace("music21.stream.Measure ", "")
-                measure = (
-                    string_e.split(" ")[0].strip().replace("X1", "").replace("X2", "")
-                )
-                instr_repeat_elements.append(
-                    (int(measure), "repeat bracket" + elem.number)
-                )
-        repeat_elements.update(instr_repeat_elements)
-
-    repeat_elements = sorted(list(repeat_elements), key=lambda tup: tup[0])
-    if v:
-        print("The repeat elements found in this score are: " + str(repeat_elements))
-    return repeat_elements
-
-
-def _include_beats_column(harmonic_analysis: DataFrame) -> None:
-    harmonic_analysis["beats"] = 0
-    for index, measure in enumerate(harmonic_analysis[PLAYTHROUGH].values):
-        if measure <= 1:
-            beat = int(
-                measure
-                + float(harmonic_analysis.mc_onset[index])
-                * get_number_of_beats(harmonic_analysis.timesig[index])
-            )
-        else:
-            time_sig = get_number_of_beats(harmonic_analysis.timesig[index - 1])
-            beat = int(
-                (measure - 1) * time_sig
-                + 1
-                + harmonic_analysis.mc_onset[index]
-                * get_number_of_beats(harmonic_analysis.timesig[index])
-            )
-
-        harmonic_analysis.at[index, "beats"] = beat
-
-
-def _get_beat_position(
-    beats_timesignature: int, number_of_beats: int, pos: int
-) -> float:
-    if number_of_beats == beats_timesignature:
-        return pos
-    else:
-        return (pos / beats_timesignature) + 1
-
-
-def _expand_repeat_bars(score):
-    final_score = m21.stream.Score()
+# TODO: This function is too long
+def expand_repeat_bars(score):
+    final_score = Score()
     final_score.metadata = score.metadata
     exist_repetition_bars = False
-
     # find repeat bars and expand
     for instr in score.parts:
-        part_measures = _get_instrument_elements(
+        part_measures = get_measures_with_repetitions(
             instr.elements
         )  # returns the measures with repetitions
         last_measure = part_measures[-1].measureNumber
         part_measures_expanded = []
         startsin0 = part_measures[0].measureNumber == 0  # Everything should be -1
         repetition_bars = []
 
         # Find all repetitions in that instrument
         for elem in instr.elements:
-            if isinstance(elem, m21.stream.Measure):
-                exist_repetition_bars = _examine_measure(repetition_bars, elem)
-            elif isinstance(elem, m21.spanner.RepeatBracket):
-                _examine_repeat_bracket(instr, repetition_bars, elem)
+            if isinstance(elem, Measure):
+                for e in elem:
+                    if isinstance(e, Repeat):
+                        exist_repetition_bars = True
+                        if e.direction == "start":
+                            repetition_bars.append((e.measureNumber, "start"))
+                        elif e.direction == "end":
+                            repetition_bars.append((e.measureNumber, "end"))
+                        index = elem.elements.index(e)
+                        elem.elements = (
+                            elem.elements[:index] + elem.elements[index + 1 :]
+                        )
+            elif isinstance(elem, RepeatBracket):
+                string_e = str(elem)
+                index = string_e.find("music21.stream.Measure")
+                measure = (
+                    string_e[index:].replace("music21.stream.Measure", "")[1:3].strip()
+                )
+                repetition_bars.append((int(measure), elem.number))
+                index = instr.elements.index(elem)
+                elem.elements = instr.elements[:index] + instr.elements[index + 1 :]
         repetition_bars = sorted(list(repetition_bars), key=lambda tup: tup[0])
 
         start = 0 if startsin0 else 1
-        _append_repetitions(
-            final_score,
-            exist_repetition_bars,
-            instr,
-            part_measures,
-            last_measure,
-            part_measures_expanded,
-            repetition_bars,
-            start,
-        )
+        if exist_repetition_bars:
+            p = Part()
+            p.id = instr.id
+            p.partName = instr.partName
+            for rb in repetition_bars:
+                compass = measure_ranges(part_measures, rb[0], rb[0])[0].quarterLength
+                if rb[1] == "start":
+                    if len(part_measures_expanded) > 0:
+                        offset = part_measures_expanded[-1][-1].offset
+                    else:
+                        offset = 0
+                    start_measures = measure_ranges(
+                        part_measures, start, rb[0] - 1, offset=offset + compass
+                    )
+                    if len(start_measures) > 0:
+                        part_measures_expanded.append(start_measures)
+                    start = rb[0]
+                elif rb[1] == "end":
+                    if len(part_measures_expanded) > 0:
+                        offset = part_measures_expanded[-1][-1].offset
+                    else:
+                        offset = 0
+                    casilla_1 = (
+                        True
+                        if any(
+                            re[1] == "1" and re[0] <= rb[0] for re in repetition_bars
+                        )
+                        else False
+                    )
+                    casilla_2 = None
+                    if casilla_1:
+                        casilla_2 = [
+                            re
+                            for re in repetition_bars
+                            if re[1] == "2" and re[0] > rb[0]
+                        ]
+                        casilla_2 = None if len(casilla_2) == 0 else casilla_2[0]
+                    part_measures_expanded.append(
+                        measure_ranges(
+                            part_measures,
+                            init=start,
+                            end=rb[0],
+                            offset=offset + compass,
+                            remove_repetition_marks=True,
+                        )
+                    )  # This should erase the repetition marks
+                    if casilla_2 is not None:
+                        part_measures_expanded.append(
+                            measure_ranges(
+                                part_measures,
+                                start,
+                                casilla_2[0],
+                                iteration=2,
+                                offset=part_measures_expanded[-1][-1].offset + compass,
+                            )
+                        )
+                        start = casilla_2[0] + 1
+                    else:
+                        part_measures_expanded.append(
+                            measure_ranges(
+                                part_measures,
+                                init=start,
+                                end=rb[0],
+                                offset=part_measures_expanded[-1][-1].offset + compass,
+                            )
+                        )
+                        start = rb[0] + 1
+            if start < last_measure:
+                compass = measure_ranges(part_measures, start, start + 1)[
+                    0
+                ].quarterLength
+                offset = part_measures_expanded[-1][-1].offset
+                part_measures_expanded.append(
+                    measure_ranges(
+                        part_measures, start, last_measure + 1, offset=offset + compass
+                    )
+                )
+            p.elements = list(itertools.chain(*tuple(part_measures_expanded)))
+            final_score.insert(0, p)
 
     return final_score if exist_repetition_bars else score
 
 
-def _append_repetitions(
-    final_score,
-    exist_repetition_bars,
-    instr,
-    part_measures,
-    last_measure,
-    part_measures_expanded,
-    repetition_bars,
-    start,
-):
-    if exist_repetition_bars:
-        p = m21.stream.Part()
-        p.id = instr.id
-        p.partName = instr.partName
-        for repetition_bar in repetition_bars:
-            measure = _measure_ranges(
-                part_measures, repetition_bar[0], repetition_bar[0]
-            )[0].quarterLength
-            if repetition_bar[1] == "start":
-                start = _add_start(
-                    part_measures,
-                    part_measures_expanded,
-                    start,
-                    repetition_bar,
-                    measure,
-                )
-            elif repetition_bar[1] == "end":
-                start = _add_end(
-                    part_measures,
-                    part_measures_expanded,
-                    repetition_bars,
-                    start,
-                    repetition_bar,
-                    measure,
-                )
-        if start < last_measure:
-            measure = _measure_ranges(part_measures, start, start + 1)[0].quarterLength
-            offset = part_measures_expanded[-1][-1].offset
-            part_measures_expanded.append(
-                _measure_ranges(
-                    part_measures, start, last_measure + 1, offset=offset + measure
-                )
-            )
-
-        p.elements = list(itertools.chain(*tuple(part_measures_expanded)))
-        final_score.insert(0, p)
-
+def slur_processing(part):
+    slurs = [s for s in part.elements if isinstance(s, Slur)]
+    part_measures = get_measures_with_repetitions(
+        part.elements
+    )  # returns the measures with repetitions
 
-def _add_end(
-    part_measures,
-    part_measures_expanded,
-    repetition_bars,
-    start,
-    repetition_bar,
-    measure,
-):
-    if len(part_measures_expanded) > 0:
-        offset = part_measures_expanded[-1][-1].offset
-    else:
-        offset = 0
-    casilla_1 = (
-        True
-        if any(re[1] == "1" and re[0] <= repetition_bar[0] for re in repetition_bars)
-        else False
-    )
-    casilla_2 = None
-    if casilla_1:
-        casilla_2 = [
-            re for re in repetition_bars if re[1] == "2" and re[0] > repetition_bar[0]
-        ]
-        casilla_2 = None if len(casilla_2) == 0 else casilla_2[0]
-    part_measures_expanded.append(
-        _measure_ranges(
-            part_measures,
-            init=start,
-            end=repetition_bar[0],
-            offset=offset + measure,
-            remove_repetition_marks_flag=True,
+    for slur in slurs:
+        slur_notes = slur.getSpannedElements()
+        first_note_measure = slur_notes[0].measureNumber
+        first_note_offset = slur_notes[0].offset
+        last_note_measure = slur_notes[-1].measureNumber
+        last_note_offset = slur_notes[-1].offset
+        # Buscar ese compas y offset y recorrer desde esa nota hasta la siguiente
+        implied_measures = measure_ranges(
+            part_measures, first_note_measure, last_note_measure
         )
-    )  # This should erase the repetition marks
-    if casilla_2 != None:
-        part_measures_expanded.append(
-            _measure_ranges(
-                part_measures,
-                start,
-                casilla_2[0],
-                iteration=2,
-                offset=part_measures_expanded[-1][-1].offset + measure,
-            )
-        )
-        start = casilla_2[0] + 1
-    else:
-        part_measures_expanded.append(
-            _measure_ranges(
-                part_measures,
-                init=start,
-                end=repetition_bar[0],
-                offset=part_measures_expanded[-1][-1].offset + measure,
-            )
-        )
-        start = repetition_bar[0] + 1
-    return start
+        first_found = False
+        last_found = False
+        for measure in implied_measures:
+            notes = measure.elements
+            i = 0
+            while i < len(notes) and not last_found:
+                if isinstance(notes[i], Note):
+                    if notes[i].offset == first_note_offset:
+                        first_found = True
+                    elif notes[i].offset == last_note_offset:
+                        last_found = True
+                    elif first_found and not last_found:
+                        slur.addSpannedElements(notes[i])
+                i += 1
+
+
+def expand_score_repetitions(score, repeat_elements):
+    score = expand_repeat_bars(score)  # FIRST EXPAND REPEAT BARS
+    final_score = Score()
+    final_score.metadata = score.metadata
 
+    if len(repeat_elements) > 0:
+        for part in score.parts:
+            p = expand_part(part, repeat_elements)
 
-def _add_start(part_measures, part_measures_expanded, start, repetition_bar, measure):
-    if len(part_measures_expanded) > 0:
-        offset = part_measures_expanded[-1][-1].offset
+            final_score.insert(0, p)
     else:
-        offset = 0
-    start_measures = _measure_ranges(
-        part_measures, start, repetition_bar[0] - 1, offset=offset + measure
-    )
-    if len(start_measures) > 0:
-        part_measures_expanded.append(start_measures)
-    start = repetition_bar[0]
-    return start
-
-
-def _examine_repeat_bracket(instr, repetition_bars, elem):
-    string_e = str(elem)
-    index = string_e.find("music21.stream.Measure")
-    measure = string_e[index:].replace("music21.stream.Measure", "")[1:3].strip()
-    repetition_bars.append((int(measure), elem.number))
-    index = instr.elements.index(elem)
-    elem.elements = instr.elements[:index] + instr.elements[index + 1 :]
-
-
-def _examine_measure(repetition_bars, elem):
-    for e in elem:
-        if isinstance(e, m21.bar.Repeat):
-            exist_repetition_bars = True
-            if e.direction == "start":
-                repetition_bars.append((e.measureNumber, "start"))
-            elif e.direction == "end":
-                repetition_bars.append((e.measureNumber, "end"))
-            index = elem.elements.index(e)
-            elem.elements = elem.elements[:index] + elem.elements[index + 1 :]
-    return exist_repetition_bars
+        final_score = score
+    return final_score
 
 
-def _get_measures_list(part_measures: list, repeat_elements: list):
+# TODO: this function seems alittle long as well
+def get_expanded_measures(part_measures, repeat_elements):
+    repeat_bracket = (
+        sum([1 if "repeat bracket" in item[1] else 0 for item in repeat_elements]) > 0
+    )
     measures_list = []
     startsin0 = part_measures[0].measureNumber == 0  # Everything should be -1
 
     there_is_fine = False
     there_is_segno = False
     # 1. find the fine and segno
     if any([r[1] == "fine" for r in repeat_elements]):
         f = [x[0] for x in repeat_elements if x[1] == "fine"][0]
         there_is_fine = True
     if any([r[1] == "segno" for r in repeat_elements]):
         s = [x[0] for x in repeat_elements if x[1] == "segno"][0]
         there_is_segno = True
 
-    # Having all the repetition elements, get the measures
-    if there_is_segno:
-        before_segno = _measure_ranges(part_measures, 1 if not startsin0 else 0, s - 1)
+    # 2. Having all the repetition elements, get the measures
+    if there_is_segno:  # Introduction
+        before_segno = measure_ranges(part_measures, 1 if not startsin0 else 0, s - 1)
         measures_list.append(
             before_segno
         )  # S -1 OR S-> when segno in compass 1, s, else s-1?
         dc_time_signature = [
-            y
-            for x in before_segno
-            for y in x.elements
-            if isinstance(y, m21.meter.TimeSignature)
+            y for x in before_segno for y in x.elements if isinstance(y, TimeSignature)
         ]
     elif there_is_fine:
         measures_list.append(
-            _measure_ranges(
+            measure_ranges(
                 part_measures,
                 1 if not startsin0 else 0,
                 f - 1,
                 iteration=1 if repeat_bracket else None,
             )
         )
     else:
         measures_list.append(
-            _measure_ranges(
+            measure_ranges(
                 part_measures,
                 1 if not startsin0 else 0,
                 len(part_measures),
                 iteration=1 if repeat_bracket else None,
             )
         )
 
     for repeat in repeat_elements:
-        repeat_measure = _measure_ranges(part_measures, repeat[0], repeat[0])
+        repeat_measure = measure_ranges(part_measures, repeat[0], repeat[0])
         compass = repeat_measure[0].quarterLength
 
         if repeat[1] == "segno":
             offset = measures_list[-1][-1].offset
-            segno_part = _measure_ranges(
+            segno_part = measure_ranges(
                 part_measures,
                 s,
                 f - 1 if there_is_fine else len(part_measures),
                 iteration=1 if repeat_bracket else None,
                 offset=offset + compass,
-                remove_repetition_marks_flag=True,
+                remove_repetition_marks=True,
             )
             measures_list.append(segno_part)  # Segno to Fine
         elif repeat[1] == "fine":
             twoCompasses = False
             """if len(repeat_measure) > 0:
                 twoCompasses = True"""
             offset = measures_list[-1][-1].offset
-            fine_part = _measure_ranges(
+            fine_part = measure_ranges(
                 part_measures,
                 f,
                 len(part_measures),
                 offset=offset + compass,
-                twocompasses_flag=twoCompasses,
-                remove_repetition_marks_flag=True,
+                twoCompasses=twoCompasses,
+                remove_repetition_marks=True,
             )
             measures_list.append(fine_part)  # Fine to end
         elif repeat[1] == "al segno" or repeat[1] == "dal segno":
             offset = measures_list[-1][-1].offset
             # segnos' compass time signature
             segno_time_measure = [
-                x
-                for x in segno_part[0].elements
-                if isinstance(x, m21.meter.TimeSignature)
+                x for x in segno_part[0].elements if isinstance(x, TimeSignature)
             ]
             segno_time_measure = (
                 segno_time_measure
                 if len(segno_time_measure) != 0
                 else dc_time_signature[-1]
             )
-            alsegno_list = _measure_ranges(
+            alsegno_list = measure_ranges(
                 part_measures,
                 s,
                 f - 1 if there_is_fine else len(part_measures),
                 iteration=2 if repeat_bracket else None,
                 offset=offset + compass,
-                remove_repetition_marks_flag=True,
+                remove_repetition_marks=True,
             )
-            if not any(
-                isinstance(x, m21.meter.TimeSignature) for x in alsegno_list[0].elements
-            ):
+            if not any(isinstance(x, TimeSignature) for x in alsegno_list[0].elements):
                 # we reset the time signature that was on the dacapo
                 alsegno_list[0].elements = tuple(
                     [segno_time_measure] + list(alsegno_list[0].elements)
                 )
 
             measures_list.append(alsegno_list)  # Segno to fine
         elif repeat[1] == "da capo":
             offset = measures_list[-1][-1].offset
             if startsin0 and there_is_fine and not repeat_bracket:
                 f += 1
-            dacapo_list = _measure_ranges(
+            dacapo_list = measure_ranges(
                 part_measures,
                 0 if startsin0 else 1,
                 f - 1 if there_is_fine else len(part_measures),
                 iteration=2 if repeat_bracket else None,
                 offset=offset + compass,
-                remove_repetition_marks_flag=True,
+                remove_repetition_marks=True,
             )
             measures_list.append(dacapo_list)
 
     return measures_list
 
 
-def _expand_part(part, repeat_elements: list):
-    part_measures = _get_instrument_elements(
+def get_measures_with_repetitions(obj) -> List[Measure]:
+    measures = []
+    for elem in obj:
+        if isinstance(elem, Measure):
+            measures.append(elem)
+            # Change the note offsets to avoid problems due to slurs
+            last_offset = 0
+            last_duration = 0
+            for note in elem:
+                if (
+                    isinstance(note, Note)
+                    or isinstance(note, Rest)
+                    or isinstance(note, Chord)
+                ):
+                    note.offset = last_offset + last_duration
+                    last_offset = note.offset
+                    last_duration = note.duration.quarterLength
+    return measures
+
+
+def expand_part(part: Part, repeat_elements):
+    part_measures = get_measures_with_repetitions(
         part.elements
-    )  # returns the measures with repetitions
-    p = m21.stream.Part()
+    )  # returns measures with repetitions
+    p = Part()
     p.id = part.id
     p.partName = part.partName
 
-    part_measures_expanded = _get_measures_list(
+    part_measures_expanded = get_expanded_measures(
         part_measures, repeat_elements
     )  # returns the measures expanded
     part_measures_expanded = list(itertools.chain(*part_measures_expanded))
-    # Assign a new continuous measure number to every measure
+    # part_measures_expanded = sorted(tuple(part_measures_expanded), key =lambda x: x.offset)
+    # Assign a new continuous compass number to every measure
     measure_number = 0 if part_measures_expanded[0].measureNumber == 0 else 1
     for i, e in enumerate(part_measures_expanded):
-        m = m21.stream.Measure(number=measure_number)
+        m = Measure(number=measure_number)
         m.elements = e.elements
         m.offset = e.offset
         m.quarterLength = e.quarterLength
         part_measures_expanded[i] = m
         measure_number += 1
     p.elements = part_measures_expanded
     return p
 
 
-def _calculate_total_number_of_beats(time_signatures: list) -> int:
-    """
-    Given a list of time signatures, sums the beats of each time signature
-    """
-    # periods = _get_timesignature_periods(time_signatures)
-    return sum(get_number_of_beats(ts) for ts in time_signatures)
-
-
-def cast_mixed_dtypes(col):
-    if "mixed" in pd.api.types.infer_dtype(col):
-        notna = col.notna()
-        newtype = col[notna].map(type).mode()[0]
-        if issubclass(newtype, float):
-            #  convert fractions like '1/3' to float
-            col[notna] = col[notna].apply(pd.eval)
-            col = col.convert_dtypes()
-        elif issubclass(newtype, int):
-            # convert to string
-            col = col.astype("string")
-    return col
-
-
-def extract_global_time_signature(score_data):
-    """
-    Extracts a global time signature for the score for cases where is not possibel to get measure-by-measure TS
-    """
-    global_ts = (
-        score_data[C.DATA_FILTERED_PARTS][0]
-        .getElementsByClass(Measure)[0]
-        .timeSignature
-    )
-    if global_ts is None:
-        pwarn("Couldn't extract Global Time Sigature!")
-        global_ts = "NA"
-    score_data[C.GLOBAL_TIME_SIGNATURE] = global_ts
-    return global_ts
+def get_repetition_elements(score: Score, verbose=True) -> List[tuple]:
+    # 1. Get the repeat elements
+    repeat_elements = set()
+
+    for part in score.parts:
+        instr_repeat_elements = []
+        for elem in part.elements:
+            if isinstance(elem, Measure):
+                for e in elem:
+                    if isinstance(e, RepeatMark) and not isinstance(e, Repeat):
+                        measure = e.measureNumber
+                        if elem.numberSuffix in ["X1", "X2"]:  # Exception
+                            measure += 1
+                        instr_repeat_elements.append((measure, e.name))
+            elif isinstance(elem, RepeatBracket):
+                string_e = str(elem)
+                index = string_e.find("music21.stream.Measure")
+                string_e = string_e[index:].replace("music21.stream.Measure ", "")
+                measure = (
+                    string_e.split(" ")[0].strip().replace("X1", "").replace("X2", "")
+                )
+                instr_repeat_elements.append(
+                    (int(measure), "repeat bracket" + elem.number)
+                )
+        repeat_elements.update(instr_repeat_elements)
+
+    repeat_elements = sorted(list(repeat_elements), key=lambda tup: tup[0])
+    if verbose:
+        ldebug(f"The repeat elements found in this score are: {str(repeat_elements)}")
+    return repeat_elements
```

### Comparing `musif-1.1.1/musif/logs.py` & `musif-1.1.2/musif/logs.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/musescore/common.py` & `musif-1.1.2/musif/musescore/common.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/musicxml/common.py` & `musif-1.1.2/musif/musicxml/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from copy import deepcopy
 from typing import List, Tuple
 
 from music21.interval import Interval
 from music21.note import Note
+from music21.repeat import RepeatMark
 from music21.scale import MajorScale, MinorScale
 from music21.stream.base import Measure, Part, Score, Voice
 from music21.text import assembleLyrics
 from roman import toRoman
 
 from musif.cache import isinstance
 
@@ -130,31 +132,33 @@
     for measure in part.elements:
         # add missing information to both parts (dynamics, text annotations, etc are
         # missing)
         if isinstance(measure, Measure):
             num_measure += 1
             if any(not isinstance(e, Voice) for e in measure.elements):
                 not_voices_elements = [
-                    e for e in measure.elements if not isinstance(e, Voice)
+                    e
+                    for e in measure.elements
+                    if not isinstance(e, (RepeatMark, Voice))
                 ]  # elements such as clefs, dynamics, text annotations...
                 for p in parts_splitted:
                     if measure.measureNumber == 0 and isinstance(measure, Measure):
                         # number = measure.measureNumber+1
                         # only add elements if we are in am measure
                         if isinstance(p.elements[num_measure], Measure):
                             p.elements[num_measure].elements += tuple(
-                                e
+                                deepcopy(e)
                                 for e in not_voices_elements
                                 if e not in p.elements[num_measure].elements
                             )
                     if measure.measureNumber > 0:
                         if not isinstance(p.elements[num_measure], Measure):
                             continue
                         p.elements[num_measure].elements += tuple(
-                            e
+                            deepcopy(e)
                             for e in not_voices_elements
                             if e not in p.elements[num_measure].elements
                         )
     for num, p in enumerate(parts_splitted, 1):
         p.id = part.id + " " + toRoman(num)  # only I or II
         p.partName = part.partName + " " + toRoman(num)  # only I or II
         # p.elements = p.elements
```

### Comparing `musif-1.1.1/musif/musicxml/constants.py` & `musif-1.1.2/musif/musicxml/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/musicxml/key.py` & `musif-1.1.2/musif/musicxml/key.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/musicxml/scoring.py` & `musif-1.1.2/musif/musicxml/scoring.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/musicxml/tempo.py` & `musif-1.1.2/musif/musicxml/tempo.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/process/processor.py` & `musif-1.1.2/musif/process/processor.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/musif/process/utils.py` & `musif-1.1.2/musif/process/utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.1/pyproject.toml` & `musif-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "roman>=3.3",
     "joblib>=1.0.0",
     "scipy>=1.6.0",
     "music21>=8,<9",
     "deepdiff>=6.2.1",
 ]
 name = "musif"
-version = "1.1.1"
+version = "1.1.2"
 description = "Music feature extraction library from the DIDONE project"
 authors = [
     { name = "Didone Project", email = "didone@iccmu.es" },
 ]
 requires-python = ">=3.10"
 readme = "README.md"
```

### Comparing `musif-1.1.1/PKG-INFO` & `musif-1.1.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,44 @@
 Metadata-Version: 2.1
 Name: musif
-Version: 1.1.1
+Version: 1.1.2
 Summary: Music feature extraction library from the DIDONE project
 License: MIT
 Author-email: Didone Project <didone@iccmu.es>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # musif
 
 Python library for **Music Feature Extraction and Analysis**, developed by [Didone Project](https://didone.eu/). 
 
 For more info, see the documentation website at: https://musif.didone.eu
 
+### Instalation
+To install the latest version of musif, just run
+`pip install musif`
+which will download musif and all its necessary dependencies.
+
+# jSymbolic and music21 features
+Currently, musif is able to process and integrate jsymbolic as well as basic music21 features. If jsymbolic features are selected, Java JRE >= 8 must be installed in your OS and the `JAVA_HOME` environment variable correctly set. `jSymbolic` will be downloaded automatically at the first run. You can force the download of `jSymbolic` and the check of Java installation by running `python -m musif.extract.features.jsymbolic`.
+
+*Important*: right now jSymbolic features are NOT guaranteed to be compatible with musif's cache system, unlike the other stock features and music21 ones. 
+ 
+In case of problems when installing Java or getting it to work as a command, these sites might be helpful:
+https://www.theserverside.com/blog/Coffee-Talk-Java-News-Stories-and-Opinions/How-do-I-install-Java-on-Ubuntu
+https://www.wikihow.com/Set-Java-Home
+
 ## Changelog
 
+#### v1.1.2
+* fixed major bug with music21 automatic onversion to MIDI for jSymbolic features
+
+#### v1.1.1
+* added exception handling for jSymbolic
+
 #### v1.1.0
 * bug fixing
 * improved musif parsing abilities for non-well formatted files
 * added option `ignore_errors` for ignoring errors while parsing large datasets
 * better file naming for cache
 * automatically removing unpitched objects (e.g. percussion symbols)
 * added `max_nan_rows` and `max_nan_columns` for better NaN handling
```

