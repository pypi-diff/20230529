# Comparing `tmp/mafese-0.1.1.tar.gz` & `tmp/mafese-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mafese-0.1.1.tar", last modified: Thu May 25 09:22:39 2023, max compression
+gzip compressed data, was "mafese-0.1.2.tar", last modified: Mon May 29 09:38:05 2023, max compression
```

## Comparing `mafese-0.1.1.tar` & `mafese-0.1.2.tar`

### file list

```diff
@@ -1,64 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:22:39.994101 mafese-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-25 09:21:52.000000 mafese-0.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-25 09:21:52.000000 mafese-0.1.1/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-25 09:21:52.000000 mafese-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-25 09:21:52.000000 mafese-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-05-25 09:22:39.994101 mafese-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-05-25 09:21:52.000000 mafese-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:22:39.974101 mafese-0.1.1/mafese/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:22:39.990101 mafese-0.1.1/mafese/data/
--rw-r--r--   0 runner    (1001) docker     (123)   369879 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/Arrhythmia.csv
--rw-r--r--   0 runner    (1001) docker     (123)    22145 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/BreastCancer.csv
--rw-r--r--   0 runner    (1001) docker     (123)   119681 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/BreastEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/CongressEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)   498322 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/Digits.csv
--rw-r--r--   0 runner    (1001) docker     (123)    28000 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/Exactly.csv
--rw-r--r--   0 runner    (1001) docker     (123)    28000 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/Exactly2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/Glass.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/HeartEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)   438254 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/Hill-valley.csv
--rw-r--r--   0 runner    (1001) docker     (123)    37338 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/Horse.csv
--rw-r--r--   0 runner    (1001) docker     (123)    75329 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/Ionosphere.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/Iris.csv
--rw-r--r--   0 runner    (1001) docker     (123)   236504 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/KrVsKpEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/Lymphography.csv
--rw-r--r--   0 runner    (1001) docker     (123)    28000 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/M-of-n.csv
--rw-r--r--   0 runner    (1001) docker     (123)  5205194 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/Madelon.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/Monk1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/Monk2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/Monk3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    47596 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/PenglungEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)    85876 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/Sonar.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/Soybean-small.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/SpectEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19160 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/Tic-tac-toe.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/Vote.csv
--rw-r--r--   0 runner    (1001) docker     (123)    65346 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/Vowel.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1053755 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/WaveformEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/Wine.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/data/Zoo.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:22:39.994101 mafese-0.1.1/mafese/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/utils/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/utils/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/utils/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/utils/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:22:39.994101 mafese-0.1.1/mafese/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/wrapper/recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-25 09:21:52.000000 mafese-0.1.1/mafese/wrapper/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:22:39.974101 mafese-0.1.1/mafese.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-05-25 09:22:39.000000 mafese-0.1.1/mafese.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-25 09:22:39.000000 mafese-0.1.1/mafese.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:22:39.000000 mafese-0.1.1/mafese.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 09:22:39.000000 mafese-0.1.1/mafese.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 09:22:39.000000 mafese-0.1.1/mafese.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 09:22:39.994101 mafese-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-25 09:21:52.000000 mafese-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:22:39.994101 mafese-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-25 09:21:52.000000 mafese-0.1.1/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-25 09:21:52.000000 mafese-0.1.1/tests/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:38:05.337797 mafese-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-29 09:37:18.000000 mafese-0.1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-29 09:37:18.000000 mafese-0.1.2/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 09:37:18.000000 mafese-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-29 09:37:18.000000 mafese-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-05-29 09:38:05.333797 mafese-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-05-29 09:37:18.000000 mafese-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:38:05.309796 mafese-0.1.2/mafese/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:38:05.329797 mafese-0.1.2/mafese/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   369879 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Arrhythmia.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    22145 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/BreastCancer.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   119681 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/BreastEW.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/CongressEW.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   498322 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Digits.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    28000 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Exactly.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    28000 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Exactly2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Glass.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/HeartEW.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   438254 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Hill-valley.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    37338 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Horse.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    75329 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Ionosphere.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Iris.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   236504 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/KrVsKpEW.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Lymphography.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    28000 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/M-of-n.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  5205194 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Madelon.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Monk1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Monk2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Monk3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    47596 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/PenglungEW.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    85876 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Sonar.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Soybean-small.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/SpectEW.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19160 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Tic-tac-toe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Vote.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    65346 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Vowel.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1053755 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/WaveformEW.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Wine.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/data/Zoo.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:38:05.333797 mafese-0.1.2/mafese/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/utils/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/utils/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/utils/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/utils/mealpy_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/utils/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:38:05.333797 mafese-0.1.2/mafese/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11582 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/wrapper/mha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/wrapper/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-29 09:37:18.000000 mafese-0.1.2/mafese/wrapper/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:38:05.309796 mafese-0.1.2/mafese.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-05-29 09:38:05.000000 mafese-0.1.2/mafese.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-29 09:38:05.000000 mafese-0.1.2/mafese.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 09:38:05.000000 mafese-0.1.2/mafese.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-29 09:38:05.000000 mafese-0.1.2/mafese.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 09:38:05.000000 mafese-0.1.2/mafese.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 09:38:05.337797 mafese-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-29 09:37:18.000000 mafese-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:38:05.333797 mafese-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-29 09:37:18.000000 mafese-0.1.2/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-29 09:37:18.000000 mafese-0.1.2/tests/test_wrapper.py
```

### Comparing `mafese-0.1.1/CODE_OF_CONDUCT.md` & `mafese-0.1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/LICENSE` & `mafese-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/PKG-INFO` & `mafese-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mafese
-Version: 0.1.1
+Version: 0.1.2
 Summary: MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library
 Home-page: https://github.com/thieu1995/mafese
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mafese.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/mafese
@@ -43,15 +43,15 @@
 
 
 <p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MAFESE" title="MAFESE"/></p>
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.1-yellow.svg)](https://github.com/thieu1995/mafese/releases)
+[![GitHub release](https://img.shields.io/badge/release-0.1.2-yellow.svg)](https://github.com/thieu1995/mafese/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mafese) 
 [![PyPI version](https://badge.fury.io/py/mafese.svg)](https://badge.fury.io/py/mafese)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mafese.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mafese.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mafese.svg)
 [![Downloads](https://pepy.tech/badge/mafese)](https://pepy.tech/project/mafese)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml)
@@ -83,15 +83,15 @@
 
 # Installation
 
 ### Install with pip
 
 Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
 ```sh 
-$ pip install mafese==0.1.1
+$ pip install mafese==0.1.2
 ```
 
 ### Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/mafese.git
 $ cd mafese
 $ python setup.py install
@@ -100,25 +100,34 @@
 
 ### Lib's structure
 
 ```code 
 docs
 examples
 mafese
-    wrapper
+    data/
+        Arrhythmia.csv
+        BreastCancer.csv
+        ...
+    wrapper/
+        mha.py
         recursive.py
         sequential.py
     filter.py
-    utils
+    utils/
         correlation.py
+        data_loader.py
         encoder.py
         estimator.py
+        mealpy_util.py
+        transfer.py
         validator.py
     __init__.py
     selector.py
+    evaluator.py
 README.md
 setup.py
 ```
 
 
 # Usage
 
@@ -239,23 +248,60 @@
 
 # call transform() on X to filter it down to selected features
 X_train_selected = feat_selector.transform(data.X_train)
 X_test_selected = feat_selector.transform(data.X_test)
 ```
 
 
+Or, use Metaheuristic-based feature selection with different metaheuristic algorithms:
+
+```python
+from mafese.wrapper.mha import MhaSelector
+from mafese import get_dataset
+from mafese import evaluator
+from sklearn.svm import SVC
+
+data = get_dataset("Arrhythmia")
+data.split_train_test(test_size=0.2)
+print(data.X_train.shape, data.X_test.shape)            # (361, 279) (91, 279)
+
+# define mafese feature selection method
+feat_selector = MhaSelector(problem="classification", estimator="knn",
+                            optimizer="BaseGA", optimizer_paras=None,
+                            transfer_func="vstf_01", obj_name="AS")
+# find all relevant features
+feat_selector.fit(data.X_train, data.y_train, fit_weights=(0.9, 0.1), verbose=True)
+
+# check selected features - True (or 1) is selected, False (or 0) is not selected
+print(feat_selector.selected_feature_masks)
+print(feat_selector.selected_feature_solution)
+
+# check the index of selected features
+print(feat_selector.selected_feature_indexes)
+
+# call transform() on X to filter it down to selected features
+X_train_selected = feat_selector.transform(data.X_train)
+X_test_selected = feat_selector.transform(data.X_test)
+
+# Evaluate final dataset with different estimator with multiple performance metrics
+results = evaluator.evaluate(feat_selector, estimator=SVC(), data=data, metrics=["AS", "PS", "RS"])
+print(results)
+# {'AS_train': 0.77176, 'PS_train': 0.54177, 'RS_train': 0.6205, 'AS_test': 0.72636, 'PS_test': 0.34628, 'RS_test': 0.52747}
+```
+
+
 
 For more usage examples please look at [examples](/examples) folder.
 
 ### Shortcut 
 To call the class
 
 ```code 
 from mafese import Data, get_dataset
-from mafese import SequentialSelector, RecursiveSelector, FilterSelector
+from mafese import SequentialSelector, RecursiveSelector, FilterSelector, MhaSelector
 ```
 
 
 # Get helps (questions, problems)
 
 * Official source code repo: https://github.com/thieu1995/mafese
 * Official document: https://mafese.readthedocs.io/
```

### Comparing `mafese-0.1.1/README.md` & `mafese-0.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 <p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MAFESE" title="MAFESE"/></p>
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.1-yellow.svg)](https://github.com/thieu1995/mafese/releases)
+[![GitHub release](https://img.shields.io/badge/release-0.1.2-yellow.svg)](https://github.com/thieu1995/mafese/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mafese) 
 [![PyPI version](https://badge.fury.io/py/mafese.svg)](https://badge.fury.io/py/mafese)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mafese.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mafese.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mafese.svg)
 [![Downloads](https://pepy.tech/badge/mafese)](https://pepy.tech/project/mafese)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml)
@@ -40,15 +40,15 @@
 
 # Installation
 
 ### Install with pip
 
 Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
 ```sh 
-$ pip install mafese==0.1.1
+$ pip install mafese==0.1.2
 ```
 
 ### Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/mafese.git
 $ cd mafese
 $ python setup.py install
@@ -57,25 +57,34 @@
 
 ### Lib's structure
 
 ```code 
 docs
 examples
 mafese
-    wrapper
+    data/
+        Arrhythmia.csv
+        BreastCancer.csv
+        ...
+    wrapper/
+        mha.py
         recursive.py
         sequential.py
     filter.py
-    utils
+    utils/
         correlation.py
+        data_loader.py
         encoder.py
         estimator.py
+        mealpy_util.py
+        transfer.py
         validator.py
     __init__.py
     selector.py
+    evaluator.py
 README.md
 setup.py
 ```
 
 
 # Usage
 
@@ -196,23 +205,60 @@
 
 # call transform() on X to filter it down to selected features
 X_train_selected = feat_selector.transform(data.X_train)
 X_test_selected = feat_selector.transform(data.X_test)
 ```
 
 
+Or, use Metaheuristic-based feature selection with different metaheuristic algorithms:
+
+```python
+from mafese.wrapper.mha import MhaSelector
+from mafese import get_dataset
+from mafese import evaluator
+from sklearn.svm import SVC
+
+data = get_dataset("Arrhythmia")
+data.split_train_test(test_size=0.2)
+print(data.X_train.shape, data.X_test.shape)            # (361, 279) (91, 279)
+
+# define mafese feature selection method
+feat_selector = MhaSelector(problem="classification", estimator="knn",
+                            optimizer="BaseGA", optimizer_paras=None,
+                            transfer_func="vstf_01", obj_name="AS")
+# find all relevant features
+feat_selector.fit(data.X_train, data.y_train, fit_weights=(0.9, 0.1), verbose=True)
+
+# check selected features - True (or 1) is selected, False (or 0) is not selected
+print(feat_selector.selected_feature_masks)
+print(feat_selector.selected_feature_solution)
+
+# check the index of selected features
+print(feat_selector.selected_feature_indexes)
+
+# call transform() on X to filter it down to selected features
+X_train_selected = feat_selector.transform(data.X_train)
+X_test_selected = feat_selector.transform(data.X_test)
+
+# Evaluate final dataset with different estimator with multiple performance metrics
+results = evaluator.evaluate(feat_selector, estimator=SVC(), data=data, metrics=["AS", "PS", "RS"])
+print(results)
+# {'AS_train': 0.77176, 'PS_train': 0.54177, 'RS_train': 0.6205, 'AS_test': 0.72636, 'PS_test': 0.34628, 'RS_test': 0.52747}
+```
+
+
 
 For more usage examples please look at [examples](/examples) folder.
 
 ### Shortcut 
 To call the class
 
 ```code 
 from mafese import Data, get_dataset
-from mafese import SequentialSelector, RecursiveSelector, FilterSelector
+from mafese import SequentialSelector, RecursiveSelector, FilterSelector, MhaSelector
 ```
 
 
 # Get helps (questions, problems)
 
 * Official source code repo: https://github.com/thieu1995/mafese
 * Official document: https://mafese.readthedocs.io/
```

### Comparing `mafese-0.1.1/mafese/__init__.py` & `mafese-0.1.2/mafese/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 15:23, 06/03/2022 ----------%                                                                               
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 from mafese.utils.data_loader import Data, get_dataset
 from mafese.filter import FilterSelector
 from mafese.wrapper.recursive import RecursiveSelector
 from mafese.wrapper.sequential import SequentialSelector
+from mafese.wrapper.mha import MhaSelector
```

### Comparing `mafese-0.1.1/mafese/data/Arrhythmia.csv` & `mafese-0.1.2/mafese/data/Arrhythmia.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/data/BreastCancer.csv` & `mafese-0.1.2/mafese/data/BreastCancer.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/data/BreastEW.csv` & `mafese-0.1.2/mafese/data/BreastEW.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/data/Digits.csv` & `mafese-0.1.2/mafese/data/Digits.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/data/Glass.csv` & `mafese-0.1.2/mafese/data/Glass.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/data/HeartEW.csv` & `mafese-0.1.2/mafese/data/HeartEW.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/data/Hill-valley.csv` & `mafese-0.1.2/mafese/data/Hill-valley.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/data/Horse.csv` & `mafese-0.1.2/mafese/data/Horse.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/data/Ionosphere.csv` & `mafese-0.1.2/mafese/data/Ionosphere.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/data/Iris.csv` & `mafese-0.1.2/mafese/data/Iris.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/data/Lymphography.csv` & `mafese-0.1.2/mafese/data/Lymphography.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/data/Madelon.csv` & `mafese-0.1.2/mafese/data/Madelon.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/data/Monk1.csv` & `mafese-0.1.2/mafese/data/Monk1.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/data/Monk2.csv` & `mafese-0.1.2/mafese/data/Monk2.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/data/Monk3.csv` & `mafese-0.1.2/mafese/data/Monk3.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/data/PenglungEW.csv` & `mafese-0.1.2/mafese/data/PenglungEW.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/data/Sonar.csv` & `mafese-0.1.2/mafese/data/Sonar.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/data/Soybean-small.csv` & `mafese-0.1.2/mafese/data/Soybean-small.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/data/Vowel.csv` & `mafese-0.1.2/mafese/data/Vowel.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/data/WaveformEW.csv` & `mafese-0.1.2/mafese/data/WaveformEW.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/data/Wine.csv` & `mafese-0.1.2/mafese/data/Wine.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/data/Zoo.csv` & `mafese-0.1.2/mafese/data/Zoo.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/filter.py` & `mafese-0.1.2/mafese/filter.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/selector.py` & `mafese-0.1.2/mafese/selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     """
     name = "Feature Selector"
     SUPPORTED_PROBLEMS = ["classification", "regression"]
 
     def __init__(self, problem="classification"):
         self.problem = self.set_problem(problem)
         self.selector = None
+        self.estimator = None
         self.paras = {}
         self.selected_feature_indexes = []
         self.selected_feature_masks = []
         self.selected_feature_solution = []
         self.epsilon = 1e-8
         self.w = 1e8
```

### Comparing `mafese-0.1.1/mafese/utils/correlation.py` & `mafese-0.1.2/mafese/utils/correlation.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/utils/data_loader.py` & `mafese-0.1.2/mafese/utils/data_loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,20 @@
     def split_train_test(self, test_size=0.2, train_size=None,
                          random_state=41, shuffle=True, stratify=None, inplace=True):
         self.X_train, self.X_test, self.y_train, self.y_test = train_test_split(self.X, self.y, test_size=test_size,
                         train_size=train_size, random_state=random_state, shuffle=shuffle, stratify=stratify)
         if not inplace:
             return self.X_train, self.X_test, self.y_train, self.y_test
 
+    def set_train_test(self, X_train=None, y_train=None, X_test=None, y_test=None):
+        self.X_train = X_train
+        self.y_train = y_train
+        self.X_test = X_test
+        self.y_test = y_test
+
 
 def get_dataset(dataset_name):
     # function to retrieve the data
     dir_root = f"{Path(__file__).parent.parent.__str__()}/data"
     list_paths = Path(dir_root).glob("*.csv")
     list_datasets = [pathfile.name[:-4] for pathfile in list_paths]
```

### Comparing `mafese-0.1.1/mafese/utils/encoder.py` & `mafese-0.1.2/mafese/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/utils/estimator.py` & `mafese-0.1.2/mafese/utils/estimator.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/utils/validator.py` & `mafese-0.1.2/mafese/utils/validator.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/wrapper/recursive.py` & `mafese-0.1.2/mafese/wrapper/recursive.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese/wrapper/sequential.py` & `mafese-0.1.2/mafese/wrapper/sequential.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/mafese.egg-info/PKG-INFO` & `mafese-0.1.2/mafese.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mafese
-Version: 0.1.1
+Version: 0.1.2
 Summary: MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library
 Home-page: https://github.com/thieu1995/mafese
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mafese.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/mafese
@@ -43,15 +43,15 @@
 
 
 <p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MAFESE" title="MAFESE"/></p>
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.1-yellow.svg)](https://github.com/thieu1995/mafese/releases)
+[![GitHub release](https://img.shields.io/badge/release-0.1.2-yellow.svg)](https://github.com/thieu1995/mafese/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mafese) 
 [![PyPI version](https://badge.fury.io/py/mafese.svg)](https://badge.fury.io/py/mafese)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mafese.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mafese.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mafese.svg)
 [![Downloads](https://pepy.tech/badge/mafese)](https://pepy.tech/project/mafese)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml)
@@ -83,15 +83,15 @@
 
 # Installation
 
 ### Install with pip
 
 Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
 ```sh 
-$ pip install mafese==0.1.1
+$ pip install mafese==0.1.2
 ```
 
 ### Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/mafese.git
 $ cd mafese
 $ python setup.py install
@@ -100,25 +100,34 @@
 
 ### Lib's structure
 
 ```code 
 docs
 examples
 mafese
-    wrapper
+    data/
+        Arrhythmia.csv
+        BreastCancer.csv
+        ...
+    wrapper/
+        mha.py
         recursive.py
         sequential.py
     filter.py
-    utils
+    utils/
         correlation.py
+        data_loader.py
         encoder.py
         estimator.py
+        mealpy_util.py
+        transfer.py
         validator.py
     __init__.py
     selector.py
+    evaluator.py
 README.md
 setup.py
 ```
 
 
 # Usage
 
@@ -239,23 +248,60 @@
 
 # call transform() on X to filter it down to selected features
 X_train_selected = feat_selector.transform(data.X_train)
 X_test_selected = feat_selector.transform(data.X_test)
 ```
 
 
+Or, use Metaheuristic-based feature selection with different metaheuristic algorithms:
+
+```python
+from mafese.wrapper.mha import MhaSelector
+from mafese import get_dataset
+from mafese import evaluator
+from sklearn.svm import SVC
+
+data = get_dataset("Arrhythmia")
+data.split_train_test(test_size=0.2)
+print(data.X_train.shape, data.X_test.shape)            # (361, 279) (91, 279)
+
+# define mafese feature selection method
+feat_selector = MhaSelector(problem="classification", estimator="knn",
+                            optimizer="BaseGA", optimizer_paras=None,
+                            transfer_func="vstf_01", obj_name="AS")
+# find all relevant features
+feat_selector.fit(data.X_train, data.y_train, fit_weights=(0.9, 0.1), verbose=True)
+
+# check selected features - True (or 1) is selected, False (or 0) is not selected
+print(feat_selector.selected_feature_masks)
+print(feat_selector.selected_feature_solution)
+
+# check the index of selected features
+print(feat_selector.selected_feature_indexes)
+
+# call transform() on X to filter it down to selected features
+X_train_selected = feat_selector.transform(data.X_train)
+X_test_selected = feat_selector.transform(data.X_test)
+
+# Evaluate final dataset with different estimator with multiple performance metrics
+results = evaluator.evaluate(feat_selector, estimator=SVC(), data=data, metrics=["AS", "PS", "RS"])
+print(results)
+# {'AS_train': 0.77176, 'PS_train': 0.54177, 'RS_train': 0.6205, 'AS_test': 0.72636, 'PS_test': 0.34628, 'RS_test': 0.52747}
+```
+
+
 
 For more usage examples please look at [examples](/examples) folder.
 
 ### Shortcut 
 To call the class
 
 ```code 
 from mafese import Data, get_dataset
-from mafese import SequentialSelector, RecursiveSelector, FilterSelector
+from mafese import SequentialSelector, RecursiveSelector, FilterSelector, MhaSelector
 ```
 
 
 # Get helps (questions, problems)
 
 * Official source code repo: https://github.com/thieu1995/mafese
 * Official document: https://mafese.readthedocs.io/
```

### Comparing `mafese-0.1.1/mafese.egg-info/SOURCES.txt` & `mafese-0.1.2/mafese.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 CODE_OF_CONDUCT.md
 ChangeLog.md
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 mafese/__init__.py
+mafese/evaluator.py
 mafese/filter.py
 mafese/selector.py
 mafese.egg-info/PKG-INFO
 mafese.egg-info/SOURCES.txt
 mafese.egg-info/dependency_links.txt
 mafese.egg-info/requires.txt
 mafese.egg-info/top_level.txt
@@ -43,13 +44,16 @@
 mafese/data/Wine.csv
 mafese/data/Zoo.csv
 mafese/utils/__init__.py
 mafese/utils/correlation.py
 mafese/utils/data_loader.py
 mafese/utils/encoder.py
 mafese/utils/estimator.py
+mafese/utils/mealpy_util.py
+mafese/utils/transfer.py
 mafese/utils/validator.py
 mafese/wrapper/__init__.py
+mafese/wrapper/mha.py
 mafese/wrapper/recursive.py
 mafese/wrapper/sequential.py
 tests/test_filter.py
 tests/test_wrapper.py
```

### Comparing `mafese-0.1.1/setup.py` & `mafese-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with open('README.md', encoding='utf-8') as f:
         README = f.read()
     return README
 
 
 setup(
     name="mafese",
-    version="0.1.1",
+    version="0.1.2",
     author="Thieu",
     author_email="nguyenthieu2102@gmail.com",
     description="MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords=["engineering optimization problems", "mathematical optimization",
               "feature selection", "classification problem",
```

### Comparing `mafese-0.1.1/tests/test_filter.py` & `mafese-0.1.2/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.1/tests/test_wrapper.py` & `mafese-0.1.2/tests/test_wrapper.py`

 * *Files identical despite different names*

