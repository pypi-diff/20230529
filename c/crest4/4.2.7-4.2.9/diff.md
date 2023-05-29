# Comparing `tmp/crest4-4.2.7.tar.gz` & `tmp/crest4-4.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crest4-4.2.7.tar", last modified: Thu Jan 19 16:15:21 2023, max compression
+gzip compressed data, was "crest4-4.2.9.tar", last modified: Mon May 29 14:31:53 2023, max compression
```

## Comparing `crest4-4.2.7.tar` & `crest4-4.2.9.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-01-19 16:15:21.263153 crest4-4.2.7/
--rw-r--r--   0 sinclair   (501) staff       (20)    35149 2021-04-19 16:21:09.000000 crest4-4.2.7/LICENSE.txt
--rw-r--r--   0 sinclair   (501) staff       (20)      623 2022-05-20 08:41:00.000000 crest4-4.2.7/MANIFEST.in
--rw-r--r--   0 sinclair   (501) staff       (20)    18895 2023-01-19 16:15:21.263015 crest4-4.2.7/PKG-INFO
--rw-r--r--   0 sinclair   (501) staff       (20)    18418 2023-01-19 16:15:06.000000 crest4-4.2.7/README.md
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-01-19 16:15:21.255152 crest4-4.2.7/crest4/
--rw-r--r--   0 sinclair   (501) staff       (20)      507 2023-01-19 16:15:06.000000 crest4-4.2.7/crest4/__init__.py
--rw-r--r--   0 sinclair   (501) staff       (20)      499 2022-04-06 16:04:26.000000 crest4-4.2.7/crest4/__main__.py
--rw-r--r--   0 sinclair   (501) staff       (20)    16252 2023-01-19 15:49:41.000000 crest4-4.2.7/crest4/classify.py
--rw-r--r--   0 sinclair   (501) staff       (20)    11454 2023-01-19 15:55:40.000000 crest4-4.2.7/crest4/databases.py
--rw-r--r--   0 sinclair   (501) staff       (20)     4633 2022-05-29 11:33:56.000000 crest4-4.2.7/crest4/otu_tables.py
--rw-r--r--   0 sinclair   (501) staff       (20)     6360 2022-05-28 19:47:22.000000 crest4-4.2.7/crest4/query.py
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-01-19 16:15:21.256204 crest4-4.2.7/crest4/tests/
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-01-19 16:15:21.256690 crest4-4.2.7/crest4/tests/actualize_database/
--rw-r--r--   0 sinclair   (501) staff       (20)      207 2021-07-13 09:13:43.000000 crest4-4.2.7/crest4/tests/actualize_database/README.md
--rw-r--r--   0 sinclair   (501) staff       (20)     1262 2021-10-17 14:02:01.000000 crest4-4.2.7/crest4/tests/actualize_database/run_test.py
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-01-19 16:15:21.257273 crest4-4.2.7/crest4/tests/cmd_line_tool/
--rw-r--r--   0 sinclair   (501) staff       (20)       84 2021-07-13 09:13:43.000000 crest4-4.2.7/crest4/tests/cmd_line_tool/README.md
--rw-r--r--   0 sinclair   (501) staff       (20)     1343 2022-05-28 21:46:13.000000 crest4-4.2.7/crest4/tests/cmd_line_tool/run_test.py
--rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-07-13 09:13:43.000000 crest4-4.2.7/crest4/tests/cmd_line_tool/two_seqs.fasta
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-01-19 16:15:21.257726 crest4-4.2.7/crest4/tests/custom_database/
--rw-r--r--   0 sinclair   (501) staff       (20)      110 2022-05-19 13:31:03.000000 crest4-4.2.7/crest4/tests/custom_database/README.md
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-01-19 16:15:21.258362 crest4-4.2.7/crest4/tests/custom_database/custom/
--rw-r--r--   0 sinclair   (501) staff       (20)     3049 2022-05-17 09:31:56.000000 crest4-4.2.7/crest4/tests/custom_database/custom/custom.fasta
--rw-r--r--   0 sinclair   (501) staff       (20)       21 2022-05-17 09:30:46.000000 crest4-4.2.7/crest4/tests/custom_database/custom/custom.map
--rw-r--r--   0 sinclair   (501) staff       (20)       28 2022-05-17 09:31:38.000000 crest4-4.2.7/crest4/tests/custom_database/custom/custom.names
--rw-r--r--   0 sinclair   (501) staff       (20)        5 2022-05-19 13:25:23.000000 crest4-4.2.7/crest4/tests/custom_database/custom/custom.tre
--rw-r--r--   0 sinclair   (501) staff       (20)     1283 2022-05-19 13:27:20.000000 crest4-4.2.7/crest4/tests/custom_database/run_test.py
--rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-04-30 12:29:37.000000 crest4-4.2.7/crest4/tests/custom_database/two_seqs.fasta
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-01-19 16:15:21.251899 crest4-4.2.7/crest4/tests/gio_hundred_seqs/
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-01-19 16:15:21.258614 crest4-4.2.7/crest4/tests/gio_hundred_seqs/expected_output/
--rw-r--r--   0 sinclair   (501) staff       (20)    51702 2021-04-08 11:31:48.000000 crest4-4.2.7/crest4/tests/gio_hundred_seqs/expected_output/assigned.fasta
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-01-19 16:15:21.259666 crest4-4.2.7/crest4/tests/ncbi_two_sequences/
--rw-r--r--   0 sinclair   (501) staff       (20)      505 2021-05-27 13:51:38.000000 crest4-4.2.7/crest4/tests/ncbi_two_sequences/README.md
--rw-r--r--   0 sinclair   (501) staff       (20)     1425 2021-05-27 13:51:38.000000 crest4-4.2.7/crest4/tests/ncbi_two_sequences/generate.py
--rw-r--r--   0 sinclair   (501) staff       (20)     1219 2022-05-28 21:42:52.000000 crest4-4.2.7/crest4/tests/ncbi_two_sequences/run_test.py
--rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-04-30 12:29:37.000000 crest4-4.2.7/crest4/tests/ncbi_two_sequences/two_seqs.fasta
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-01-19 16:15:21.260138 crest4-4.2.7/crest4/tests/no_hits_sequence/
--rw-r--r--   0 sinclair   (501) staff       (20)      127 2021-05-17 17:36:29.000000 crest4-4.2.7/crest4/tests/no_hits_sequence/README.md
--rw-r--r--   0 sinclair   (501) staff       (20)     1268 2021-05-16 19:12:40.000000 crest4-4.2.7/crest4/tests/no_hits_sequence/no_hits.fasta
--rw-r--r--   0 sinclair   (501) staff       (20)     1895 2022-05-28 21:47:24.000000 crest4-4.2.7/crest4/tests/no_hits_sequence/run_test.py
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-01-19 16:15:21.260728 crest4-4.2.7/crest4/tests/precomputed_hits/
--rw-r--r--   0 sinclair   (501) staff       (20)      116 2021-07-13 09:13:43.000000 crest4-4.2.7/crest4/tests/precomputed_hits/README.md
--rw-r--r--   0 sinclair   (501) staff       (20)     7287 2021-07-13 09:13:43.000000 crest4-4.2.7/crest4/tests/precomputed_hits/precomputed.hits
--rw-r--r--   0 sinclair   (501) staff       (20)     1421 2022-05-28 21:06:11.000000 crest4-4.2.7/crest4/tests/precomputed_hits/run_test.py
--rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-07-13 09:13:43.000000 crest4-4.2.7/crest4/tests/precomputed_hits/two_seqs.fasta
--rw-r--r--   0 sinclair   (501) staff       (20)       42 2021-05-17 17:16:58.000000 crest4-4.2.7/crest4/tests/pytest.ini
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-01-19 16:15:21.261161 crest4-4.2.7/crest4/tests/readme_example_seq/
--rw-r--r--   0 sinclair   (501) staff       (20)      307 2021-05-18 00:43:16.000000 crest4-4.2.7/crest4/tests/readme_example_seq/README.md
--rw-r--r--   0 sinclair   (501) staff       (20)      341 2021-05-17 18:22:13.000000 crest4-4.2.7/crest4/tests/readme_example_seq/readme_test.fasta
--rw-r--r--   0 sinclair   (501) staff       (20)     1156 2022-05-28 21:43:14.000000 crest4-4.2.7/crest4/tests/readme_example_seq/run_test.py
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-01-19 16:15:21.261595 crest4-4.2.7/crest4/tests/score_drop_change/
--rw-r--r--   0 sinclair   (501) staff       (20)      118 2021-10-17 13:39:41.000000 crest4-4.2.7/crest4/tests/score_drop_change/README.md
--rw-r--r--   0 sinclair   (501) staff       (20)     1352 2022-05-28 21:47:50.000000 crest4-4.2.7/crest4/tests/score_drop_change/run_test.py
--rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-04-30 12:29:37.000000 crest4-4.2.7/crest4/tests/score_drop_change/two_seqs.fasta
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-01-19 16:15:21.262043 crest4-4.2.7/crest4/tests/vsearch_test/
--rw-r--r--   0 sinclair   (501) staff       (20)       62 2021-07-13 09:13:43.000000 crest4-4.2.7/crest4/tests/vsearch_test/README.md
--rw-r--r--   0 sinclair   (501) staff       (20)     1250 2022-05-28 21:43:30.000000 crest4-4.2.7/crest4/tests/vsearch_test/run_test.py
--rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-07-13 09:13:43.000000 crest4-4.2.7/crest4/tests/vsearch_test/two_seqs.fasta
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-01-19 16:15:21.262784 crest4-4.2.7/crest4/tests/with_otu_table/
--rw-r--r--   0 sinclair   (501) staff       (20)      107 2021-07-13 09:13:43.000000 crest4-4.2.7/crest4/tests/with_otu_table/README.md
--rw-r--r--   0 sinclair   (501) staff       (20)      101 2021-07-13 09:13:43.000000 crest4-4.2.7/crest4/tests/with_otu_table/otu_table_bad.tsv
--rw-r--r--   0 sinclair   (501) staff       (20)      135 2021-07-13 09:13:43.000000 crest4-4.2.7/crest4/tests/with_otu_table/otu_table_good.tsv
--rw-r--r--   0 sinclair   (501) staff       (20)     2161 2022-05-28 21:07:24.000000 crest4-4.2.7/crest4/tests/with_otu_table/run_test.py
--rw-r--r--   0 sinclair   (501) staff       (20)     4639 2021-07-13 09:13:43.000000 crest4-4.2.7/crest4/tests/with_otu_table/seqs.fasta
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-01-19 16:15:21.256084 crest4-4.2.7/crest4.egg-info/
--rw-r--r--   0 sinclair   (501) staff       (20)    18895 2023-01-19 16:15:21.000000 crest4-4.2.7/crest4.egg-info/PKG-INFO
--rw-r--r--   0 sinclair   (501) staff       (20)     2011 2023-01-19 16:15:21.000000 crest4-4.2.7/crest4.egg-info/SOURCES.txt
--rw-r--r--   0 sinclair   (501) staff       (20)        1 2023-01-19 16:15:21.000000 crest4-4.2.7/crest4.egg-info/dependency_links.txt
--rw-r--r--   0 sinclair   (501) staff       (20)       48 2023-01-19 16:15:21.000000 crest4-4.2.7/crest4.egg-info/entry_points.txt
--rw-r--r--   0 sinclair   (501) staff       (20)      115 2023-01-19 16:15:21.000000 crest4-4.2.7/crest4.egg-info/requires.txt
--rw-r--r--   0 sinclair   (501) staff       (20)       17 2023-01-19 16:15:21.000000 crest4-4.2.7/crest4.egg-info/top_level.txt
--rw-r--r--   0 sinclair   (501) staff       (20)       38 2023-01-19 16:15:21.263193 crest4-4.2.7/setup.cfg
--rw-r--r--   0 sinclair   (501) staff       (20)     1442 2023-01-19 16:15:06.000000 crest4-4.2.7/setup.py
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.988650 crest4-4.2.9/
+-rw-r--r--   0 sinclair   (501) staff       (20)    35149 2021-04-19 16:21:09.000000 crest4-4.2.9/LICENSE.txt
+-rw-r--r--   0 sinclair   (501) staff       (20)      623 2022-05-20 08:41:00.000000 crest4-4.2.9/MANIFEST.in
+-rw-r--r--   0 sinclair   (501) staff       (20)    18815 2023-05-29 14:31:53.988505 crest4-4.2.9/PKG-INFO
+-rw-r--r--   0 sinclair   (501) staff       (20)    18337 2023-05-29 14:31:44.000000 crest4-4.2.9/README.md
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.980107 crest4-4.2.9/crest4/
+-rw-r--r--   0 sinclair   (501) staff       (20)      507 2023-05-29 14:31:44.000000 crest4-4.2.9/crest4/__init__.py
+-rw-r--r--   0 sinclair   (501) staff       (20)      478 2023-01-19 16:17:41.000000 crest4-4.2.9/crest4/__main__.py
+-rw-r--r--   0 sinclair   (501) staff       (20)    16194 2023-05-29 14:27:45.000000 crest4-4.2.9/crest4/classify.py
+-rw-r--r--   0 sinclair   (501) staff       (20)    11755 2023-05-29 14:25:07.000000 crest4-4.2.9/crest4/databases.py
+-rw-r--r--   0 sinclair   (501) staff       (20)     4616 2023-05-29 14:25:32.000000 crest4-4.2.9/crest4/otu_tables.py
+-rw-r--r--   0 sinclair   (501) staff       (20)     6339 2023-01-19 16:17:29.000000 crest4-4.2.9/crest4/query.py
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.981178 crest4-4.2.9/crest4/tests/
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.981736 crest4-4.2.9/crest4/tests/actualize_database/
+-rw-r--r--   0 sinclair   (501) staff       (20)      207 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/actualize_database/README.md
+-rw-r--r--   0 sinclair   (501) staff       (20)     1262 2021-10-17 14:02:01.000000 crest4-4.2.9/crest4/tests/actualize_database/run_test.py
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.982201 crest4-4.2.9/crest4/tests/cmd_line_tool/
+-rw-r--r--   0 sinclair   (501) staff       (20)       84 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/cmd_line_tool/README.md
+-rw-r--r--   0 sinclair   (501) staff       (20)     1343 2022-05-28 21:46:13.000000 crest4-4.2.9/crest4/tests/cmd_line_tool/run_test.py
+-rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/cmd_line_tool/two_seqs.fasta
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.982692 crest4-4.2.9/crest4/tests/custom_database/
+-rw-r--r--   0 sinclair   (501) staff       (20)      110 2022-05-19 13:31:03.000000 crest4-4.2.9/crest4/tests/custom_database/README.md
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.983488 crest4-4.2.9/crest4/tests/custom_database/custom/
+-rw-r--r--   0 sinclair   (501) staff       (20)     3049 2022-05-17 09:31:56.000000 crest4-4.2.9/crest4/tests/custom_database/custom/custom.fasta
+-rw-r--r--   0 sinclair   (501) staff       (20)       21 2022-05-17 09:30:46.000000 crest4-4.2.9/crest4/tests/custom_database/custom/custom.map
+-rw-r--r--   0 sinclair   (501) staff       (20)       28 2022-05-17 09:31:38.000000 crest4-4.2.9/crest4/tests/custom_database/custom/custom.names
+-rw-r--r--   0 sinclair   (501) staff       (20)        5 2022-05-19 13:25:23.000000 crest4-4.2.9/crest4/tests/custom_database/custom/custom.tre
+-rw-r--r--   0 sinclair   (501) staff       (20)     1283 2022-05-19 13:27:20.000000 crest4-4.2.9/crest4/tests/custom_database/run_test.py
+-rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-04-30 12:29:37.000000 crest4-4.2.9/crest4/tests/custom_database/two_seqs.fasta
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.977145 crest4-4.2.9/crest4/tests/gio_hundred_seqs/
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.983705 crest4-4.2.9/crest4/tests/gio_hundred_seqs/expected_output/
+-rw-r--r--   0 sinclair   (501) staff       (20)    51702 2021-04-08 11:31:48.000000 crest4-4.2.9/crest4/tests/gio_hundred_seqs/expected_output/assigned.fasta
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.984763 crest4-4.2.9/crest4/tests/ncbi_two_sequences/
+-rw-r--r--   0 sinclair   (501) staff       (20)      505 2021-05-27 13:51:38.000000 crest4-4.2.9/crest4/tests/ncbi_two_sequences/README.md
+-rw-r--r--   0 sinclair   (501) staff       (20)     1404 2023-01-19 16:17:26.000000 crest4-4.2.9/crest4/tests/ncbi_two_sequences/generate.py
+-rw-r--r--   0 sinclair   (501) staff       (20)     1219 2022-05-28 21:42:52.000000 crest4-4.2.9/crest4/tests/ncbi_two_sequences/run_test.py
+-rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-04-30 12:29:37.000000 crest4-4.2.9/crest4/tests/ncbi_two_sequences/two_seqs.fasta
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.985271 crest4-4.2.9/crest4/tests/no_hits_sequence/
+-rw-r--r--   0 sinclair   (501) staff       (20)      127 2021-05-17 17:36:29.000000 crest4-4.2.9/crest4/tests/no_hits_sequence/README.md
+-rw-r--r--   0 sinclair   (501) staff       (20)     1268 2021-05-16 19:12:40.000000 crest4-4.2.9/crest4/tests/no_hits_sequence/no_hits.fasta
+-rw-r--r--   0 sinclair   (501) staff       (20)     1895 2022-05-28 21:47:24.000000 crest4-4.2.9/crest4/tests/no_hits_sequence/run_test.py
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.985975 crest4-4.2.9/crest4/tests/precomputed_hits/
+-rw-r--r--   0 sinclair   (501) staff       (20)      116 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/precomputed_hits/README.md
+-rw-r--r--   0 sinclair   (501) staff       (20)     7287 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/precomputed_hits/precomputed.hits
+-rw-r--r--   0 sinclair   (501) staff       (20)     1421 2022-05-28 21:06:11.000000 crest4-4.2.9/crest4/tests/precomputed_hits/run_test.py
+-rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/precomputed_hits/two_seqs.fasta
+-rw-r--r--   0 sinclair   (501) staff       (20)       42 2021-05-17 17:16:58.000000 crest4-4.2.9/crest4/tests/pytest.ini
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.986444 crest4-4.2.9/crest4/tests/readme_example_seq/
+-rw-r--r--   0 sinclair   (501) staff       (20)      307 2021-05-18 00:43:16.000000 crest4-4.2.9/crest4/tests/readme_example_seq/README.md
+-rw-r--r--   0 sinclair   (501) staff       (20)      341 2021-05-17 18:22:13.000000 crest4-4.2.9/crest4/tests/readme_example_seq/readme_test.fasta
+-rw-r--r--   0 sinclair   (501) staff       (20)     1156 2022-05-28 21:43:14.000000 crest4-4.2.9/crest4/tests/readme_example_seq/run_test.py
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.986917 crest4-4.2.9/crest4/tests/score_drop_change/
+-rw-r--r--   0 sinclair   (501) staff       (20)      118 2021-10-17 13:39:41.000000 crest4-4.2.9/crest4/tests/score_drop_change/README.md
+-rw-r--r--   0 sinclair   (501) staff       (20)     1352 2022-05-28 21:47:50.000000 crest4-4.2.9/crest4/tests/score_drop_change/run_test.py
+-rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-04-30 12:29:37.000000 crest4-4.2.9/crest4/tests/score_drop_change/two_seqs.fasta
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.987408 crest4-4.2.9/crest4/tests/vsearch_test/
+-rw-r--r--   0 sinclair   (501) staff       (20)       62 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/vsearch_test/README.md
+-rw-r--r--   0 sinclair   (501) staff       (20)     1250 2022-05-28 21:43:30.000000 crest4-4.2.9/crest4/tests/vsearch_test/run_test.py
+-rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/vsearch_test/two_seqs.fasta
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.988162 crest4-4.2.9/crest4/tests/with_otu_table/
+-rw-r--r--   0 sinclair   (501) staff       (20)      107 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/with_otu_table/README.md
+-rw-r--r--   0 sinclair   (501) staff       (20)      101 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/with_otu_table/otu_table_bad.tsv
+-rw-r--r--   0 sinclair   (501) staff       (20)      135 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/with_otu_table/otu_table_good.tsv
+-rw-r--r--   0 sinclair   (501) staff       (20)     2161 2022-05-28 21:07:24.000000 crest4-4.2.9/crest4/tests/with_otu_table/run_test.py
+-rw-r--r--   0 sinclair   (501) staff       (20)     4639 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/with_otu_table/seqs.fasta
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.981047 crest4-4.2.9/crest4.egg-info/
+-rw-r--r--   0 sinclair   (501) staff       (20)    18815 2023-05-29 14:31:53.000000 crest4-4.2.9/crest4.egg-info/PKG-INFO
+-rw-r--r--   0 sinclair   (501) staff       (20)     2011 2023-05-29 14:31:53.000000 crest4-4.2.9/crest4.egg-info/SOURCES.txt
+-rw-r--r--   0 sinclair   (501) staff       (20)        1 2023-05-29 14:31:53.000000 crest4-4.2.9/crest4.egg-info/dependency_links.txt
+-rw-r--r--   0 sinclair   (501) staff       (20)       48 2023-05-29 14:31:53.000000 crest4-4.2.9/crest4.egg-info/entry_points.txt
+-rw-r--r--   0 sinclair   (501) staff       (20)      115 2023-05-29 14:31:53.000000 crest4-4.2.9/crest4.egg-info/requires.txt
+-rw-r--r--   0 sinclair   (501) staff       (20)       17 2023-05-29 14:31:53.000000 crest4-4.2.9/crest4.egg-info/top_level.txt
+-rw-r--r--   0 sinclair   (501) staff       (20)       38 2023-05-29 14:31:53.988686 crest4-4.2.9/setup.cfg
+-rw-r--r--   0 sinclair   (501) staff       (20)     1442 2023-05-29 14:31:44.000000 crest4-4.2.9/setup.py
```

### Comparing `crest4-4.2.7/LICENSE.txt` & `crest4-4.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/MANIFEST.in` & `crest4-4.2.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/PKG-INFO` & `crest4-4.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: crest4
-Version: 4.2.7
+Version: 4.2.9
 Summary: The `crest4` python package can automatically assign taxonomic names to DNA sequences obtained from environmental sequencing.
 Home-page: https://github.com/xapple/crest4/
 Author: Anders Lanzén and Lucas Sinclair
 Author-email: anders.lanzen@gmail.com
 License: GPL3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![PyPI version](https://badge.fury.io/py/crest4.svg)](https://badge.fury.io/py/crest4)
 ![Pytest passing](https://github.com/xapple/crest4/actions/workflows/pytest_master_branch.yml/badge.svg)
 
-# CREST version 4.2.7
+# CREST version 4.2.9
 
 `crest4` is a python package for automatically assigning taxonomic names to DNA sequences obtained from environmental sequencing.
 
 <p align="center">
 <img height="143" src="docs/logo.png?raw=true" alt="CREST Logo">
 </p>
 
@@ -60,15 +60,15 @@
 
     $ pip3 install crest4
 
 ### Notes and extras
 
 Once the installation completes you are ready to use the `crest4` executable command from the shell. Please note that the reference databases are downloaded automatically during first run, so this might take some time depending on your internet connection.
 
-In order to search the reference databases, you will also need either BLAST or VSEARCH installed. These are installed automatically with the `conda` method, but not with the `pip` method. You can obtain these with these commands on Linux:
+In order to search the reference databases, you will also need either BLAST or VSEARCH installed. These can be installed automatically with the `conda` package manager. If you don't use `conda`, you can obtain them with these commands on Linux:
 
     $ sudo apt update
     $ sudo apt install ncbi-blast+
     $ sudo apt install vsearch
 
 Or these commands on macOS:
 
@@ -133,17 +133,16 @@
                         similarity search. By default, parallelism is turned
                         off and this value is 1. If you pass the value `True`
                         we will run as many processes as there are CPUs but
                         no more than 32.
 
   --search_db DATABASE, -d DATABASE
                         The database used for the sequence similarity search.
-                        Either `midori248`, `silvamod138`, or `silvamod128`.
-                        No other values are currently supported.
-                        By default, `silvamod138`. Optionally, the user can
+                        Either `midori253darn`, or `silvamod138pr2`.
+                        By default, `silvamod138pr2`. Optionally, the user can
                         provide a custom database by specifying the full path
                         to a directory containing all required files under
                         `search_db`. See the README for more information.
 
   --output_dir DIR, -o DIR
                         The directory into which all the classification
                         results will be written to. This defaults to a
@@ -298,8 +297,8 @@
 
 The internal documentation of the `crest4` python package is available at:
 
 http://xapple.github.io/crest4/crest4
 
 This documentation is simply generated from the source code with this command:
 
-    $ pdoc3 --html --output-dir docs --force crest4
+    $ pdoc --output-dir docs crest4
```

### Comparing `crest4-4.2.7/README.md` & `crest4-4.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [![PyPI version](https://badge.fury.io/py/crest4.svg)](https://badge.fury.io/py/crest4)
 ![Pytest passing](https://github.com/xapple/crest4/actions/workflows/pytest_master_branch.yml/badge.svg)
 
-# CREST version 4.2.7
+# CREST version 4.2.9
 
 `crest4` is a python package for automatically assigning taxonomic names to DNA sequences obtained from environmental sequencing.
 
 <p align="center">
 <img height="143" src="docs/logo.png?raw=true" alt="CREST Logo">
 </p>
 
@@ -47,15 +47,15 @@
 
     $ pip3 install crest4
 
 ### Notes and extras
 
 Once the installation completes you are ready to use the `crest4` executable command from the shell. Please note that the reference databases are downloaded automatically during first run, so this might take some time depending on your internet connection.
 
-In order to search the reference databases, you will also need either BLAST or VSEARCH installed. These are installed automatically with the `conda` method, but not with the `pip` method. You can obtain these with these commands on Linux:
+In order to search the reference databases, you will also need either BLAST or VSEARCH installed. These can be installed automatically with the `conda` package manager. If you don't use `conda`, you can obtain them with these commands on Linux:
 
     $ sudo apt update
     $ sudo apt install ncbi-blast+
     $ sudo apt install vsearch
 
 Or these commands on macOS:
 
@@ -120,17 +120,16 @@
                         similarity search. By default, parallelism is turned
                         off and this value is 1. If you pass the value `True`
                         we will run as many processes as there are CPUs but
                         no more than 32.
 
   --search_db DATABASE, -d DATABASE
                         The database used for the sequence similarity search.
-                        Either `midori248`, `silvamod138`, or `silvamod128`.
-                        No other values are currently supported.
-                        By default, `silvamod138`. Optionally, the user can
+                        Either `midori253darn`, or `silvamod138pr2`.
+                        By default, `silvamod138pr2`. Optionally, the user can
                         provide a custom database by specifying the full path
                         to a directory containing all required files under
                         `search_db`. See the README for more information.
 
   --output_dir DIR, -o DIR
                         The directory into which all the classification
                         results will be written to. This defaults to a
@@ -285,8 +284,8 @@
 
 The internal documentation of the `crest4` python package is available at:
 
 http://xapple.github.io/crest4/crest4
 
 This documentation is simply generated from the source code with this command:
 
-    $ pdoc3 --html --output-dir docs --force crest4
+    $ pdoc --output-dir docs crest4
```

### Comparing `crest4-4.2.7/crest4/classify.py` & `crest4-4.2.9/crest4/classify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 Written by Lucas Sinclair.
 GNUv3 Licensed.
 Contact at www.sinclair.bio
+
 Created in May 2021.
-Last Updated in May 2022.
+Last updated in January 2023.
 """
 
 # Built-in modules #
 import os, multiprocessing
 
 # Internal modules #
 import crest4
 import crest4.databases
 from crest4.query import Query
 from crest4.databases import CrestDatabase
 
 # First party modules #
 from plumbing.cache      import property_cached
-from seqsearch.search    import SeqSearch
-from fasta               import FASTA
 from autopaths.file_path import FilePath
 from autopaths.dir_path  import DirectoryPath
 
 # Constants #
 all_db_choices = ('midori248', 'silvamod138', 'silvamod138pr2', 'silvamod128')
 
 ###############################################################################
@@ -43,15 +42,15 @@
     https://github.com/xapple/crest4/
     """
 
     def __init__(self,
                  fasta,
                  search_algo = 'blast',
                  num_threads = 1,
-                 search_db   = 'silvamod138',
+                 search_db   = 'silvamod138pr2',
                  output_dir  = None,
                  search_hits = None,
                  min_score   = None,
                  score_drop  = 2.0,
                  min_smlrty  = True,
                  otu_table   = None,
                  ):
@@ -71,17 +70,16 @@
             num_threads: The number of processors to use for the sequence
                          similarity search. By default, parallelism is turned
                          off and this value is 1. If you pass the value `True`
                          we will run as many processes as there are CPUs but
                          no more than 32.
 
             search_db: The database used for the sequence similarity search.
-                       Either `midori248`, `silvamod138`, or `silvamod128`.
-                       No other values are currently supported.
-                       By default, `silvamod138`. Optionally, the user can
+                       Either `midori253darn`, or `silvamod138pr2`.
+                       By default, `silvamod138pr2`. Optionally, the user can
                        provide a custom database by specifying the full path
                        to a directory containing all required files under
                        `search_db`. See the README for more information.
 
             output_dir: The directory into which all the classification
                         results will be written to. This defaults to a
                         directory with the same name as the original FASTA
@@ -145,14 +143,15 @@
     def transform(self):
         """
         This method will replace empty attributes with defaults when this is
         needed and will convert others to proper types.
         """
         # The fasta should be a FASTA object #
         if self.fasta is not None:
+            from fasta import FASTA
             self.fasta = FASTA(self.fasta)
         # Default for the number of threads #
         if not isinstance(self.num_threads, int):
             if self.num_threads is True:
                 self.num_threads = min(multiprocessing.cpu_count(), 32)
             elif self.num_threads is False:
                 self.num_threads = 1
@@ -265,14 +264,15 @@
             params = {'-outfmt': '7 qseqid sseqid bitscore length nident'}
         # In case the user chose VSEARCH we specify the minimum identify
         # and the minimum sequence match length
         if self.search_algo == 'vsearch':
             params = {'--id':      self.min_score,
                       '--mincols': 25}
         # Build and return the object #
+        from seqsearch.search import SeqSearch
         return SeqSearch(input_fasta = self.fasta,
                          database    = self.database,
                          seq_type    = 'nucl',
                          algorithm   = self.search_algo,
                          filtering   = {'max_targets': 100},
                          num_threads = self.num_threads,
                          out_path    = self.search_hits,
```

### Comparing `crest4-4.2.7/crest4/databases.py` & `crest4-4.2.9/crest4/databases.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 Written by Lucas Sinclair.
 GNUv3 Licensed.
 Contact at www.sinclair.bio
-Created in May 2021.
-Last updated in January 2023.
 """
 
 # Built-in modules #
 import os, json
 
 # Internal modules #
 import crest4
 
 # First party modules #
 from autopaths.dir_path import DirectoryPath
 from plumbing.cache     import property_cached
 from plumbing.scraping  import download_from_url, retrieve_from_url
-from seqsearch.search.blast   import BLASTdb
-from seqsearch.search.vsearch import VSEARCHdb
-
-# Third party modules #
-from ete3 import Tree
 
 ###############################################################################
 class CrestMetadata:
     """
     The databases that `crest4` needs are slightly too large to be distributed
     with the source tarball on PyPI. Therefore, we host them on a separate
     server. Currently, this is S3 on AWS.
@@ -147,14 +140,21 @@
 
     @property
     def url(self):
         """
         Retrieve the URL of the database file to download by first downloading
         a metadata file (see the `Metadata` class above).
         """
+        # Check that the key exists #
+        if self.short_name not in metadata.db_urls:
+            msg = "The database '%s' is not in the list of downloadable" \
+                  " databases. Please update the file `crest4_db_urls.json`" \
+                  " to include it."
+            raise Exception(msg % self.short_name)
+        # Get the URL #
         return metadata.db_urls[self.short_name]['url']
 
     def download(self):
         """
         Download the database file, uncompress it, and save it to disk.
         """
         # Compose a message so the user knows why it's taking time #
@@ -192,14 +192,15 @@
         """
         Return a `BLASTDb` object that can be used for the sequence
         similarity search.
         """
         # Download the database if it has not been done already #
         if not self.downloaded: self.download()
         # Create the database object #
+        from seqsearch.search.blast import BLASTdb
         db = BLASTdb(self.path, seq_type='nucl')
         # Create the database with `mkblastdb` if it's not made already #
         db.create_if_not_exists(verbose=True)
         # Return #
         return db
 
     @property_cached
@@ -207,29 +208,31 @@
         """
         Return a `VSEARCHdb` object that can be used for the sequence
         similarity search.
         """
         # Download the database if it has not been done already #
         if not self.downloaded: self.download()
         # Create the database object #
+        from seqsearch.search.vsearch import VSEARCHdb
         db = VSEARCHdb(self.path.replace_extension('udb'))
         # Create the database with `vsearch` if it's not made already #
         db.create_if_not_exists(verbose=True)
         # Return #
         return db
 
     #--------------------------- Loading the tree ----------------------------#
     @property_cached
     def tree(self):
         """
         Using the `.tre` file, we return an N-ary tree in memory.
-        Every node is characterised by a number. For instance between
+        Every node is characterized by a number. For instance between
         1 and 32477.
         """
         # Load the tree with ete3 #
+        from ete3 import Tree
         return Tree(self.path.replace_extension('tre'), format=8)
 
     @property_cached
     def node_to_name(self):
         """
         Using the `.names` file, we return a dictionary linking node numbers to
         a tuple of species names and a minimum similarity fraction like 0.97.
```

### Comparing `crest4-4.2.7/crest4/otu_tables.py` & `crest4-4.2.9/crest4/otu_tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 Written by Lucas Sinclair.
 GNUv3 Licensed.
 Contact at www.sinclair.bio
-Created in May 2021.
 """
 
 # Built-in modules #
 from collections import defaultdict
 
 # First party modules #
 from plumbing.cache import property_cached
 
-# Third party modules #
-import pandas
-
 ###############################################################################
 class InfoFromTableOTUs:
     """
     This class accepts a path to an OTU table as input.
     It will parse the table, along with the taxonomic assignments
     from the `Classify` object, and it will produce two extra output files.
     """
@@ -45,14 +41,15 @@
             return ','
         return '\t'
 
     @property_cached
     def otus_df(self):
         """Load the otu_table file as a pandas `DataFrame`."""
         # Load from a text file #
+        import pandas
         df = pandas.read_csv(str(self.otu_table), sep=self.format, index_col=0)
         # We only want the very first part of the IDs #
         df.index = df.index.map(lambda s: s.split()[0])
         # Return #
         return df
 
     @property_cached
@@ -79,14 +76,15 @@
                 msg = msg % (name, self.otu_table, self.classify.fasta)
                 raise ValueError(msg)
 
     def __call__(self, cumulative=False):
         # Let's first check all the IDs are found #
         self.check_id_match()
         # An empty pandas Series with each sample name and just zeros #
+        import pandas
         empty_samples = pandas.Series(0, index=self.otus_df.columns)
         # Build a empty new dataframe from a dictionary of empty series #
         result = defaultdict(lambda: empty_samples.copy())
         # Loop over every OTU in the user supplied table #
         for i, otu_counts in self.otus_df.iterrows():
             # The name or id of the current OTU #
             otu_name = otu_counts.name
@@ -112,8 +110,8 @@
         rank_names  = self.classify.database.rank_names
         tax_to_rank = lambda t: rank_names[len(t.split(';')) - 1]
         ranks       = result.taxonomy.apply(tax_to_rank)
         result.insert(loc=0, column='rank', value=ranks)
         # Sort the table by the taxonomy string #
         result = result.sort_values(by=['taxonomy'])
         # Return #
-        return result
+        return result
```

### Comparing `crest4-4.2.7/crest4/query.py` & `crest4-4.2.9/crest4/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 Written by Lucas Sinclair.
 GNUv3 Licensed.
 Contact at www.sinclair.bio
-Created in May 2021.
 """
 
 # First party modules #
 from plumbing.cache import property_cached
 
 ###############################################################################
 class Query:
```

### Comparing `crest4-4.2.7/crest4/tests/actualize_database/run_test.py` & `crest4-4.2.9/crest4/tests/actualize_database/run_test.py`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/crest4/tests/cmd_line_tool/run_test.py` & `crest4-4.2.9/crest4/tests/cmd_line_tool/run_test.py`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/crest4/tests/cmd_line_tool/two_seqs.fasta` & `crest4-4.2.9/crest4/tests/cmd_line_tool/two_seqs.fasta`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/crest4/tests/custom_database/custom/custom.fasta` & `crest4-4.2.9/crest4/tests/custom_database/custom/custom.fasta`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/crest4/tests/custom_database/run_test.py` & `crest4-4.2.9/crest4/tests/custom_database/run_test.py`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/crest4/tests/custom_database/two_seqs.fasta` & `crest4-4.2.9/crest4/tests/custom_database/two_seqs.fasta`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/crest4/tests/gio_hundred_seqs/expected_output/assigned.fasta` & `crest4-4.2.9/crest4/tests/gio_hundred_seqs/expected_output/assigned.fasta`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/crest4/tests/ncbi_two_sequences/generate.py` & `crest4-4.2.9/crest4/tests/ncbi_two_sequences/generate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 Written by Lucas Sinclair.
 GNUv3 Licensed.
 Contact at www.sinclair.bio
-Created in May 2021.
 """
 
 # Built-in modules #
 import inspect
 
 # First party modules #
 from seqsearch.databases.download import acc_to_fasta
```

### Comparing `crest4-4.2.7/crest4/tests/ncbi_two_sequences/run_test.py` & `crest4-4.2.9/crest4/tests/ncbi_two_sequences/run_test.py`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/crest4/tests/ncbi_two_sequences/two_seqs.fasta` & `crest4-4.2.9/crest4/tests/ncbi_two_sequences/two_seqs.fasta`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/crest4/tests/no_hits_sequence/no_hits.fasta` & `crest4-4.2.9/crest4/tests/no_hits_sequence/no_hits.fasta`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/crest4/tests/no_hits_sequence/run_test.py` & `crest4-4.2.9/crest4/tests/no_hits_sequence/run_test.py`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/crest4/tests/precomputed_hits/precomputed.hits` & `crest4-4.2.9/crest4/tests/precomputed_hits/precomputed.hits`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/crest4/tests/precomputed_hits/run_test.py` & `crest4-4.2.9/crest4/tests/precomputed_hits/run_test.py`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/crest4/tests/precomputed_hits/two_seqs.fasta` & `crest4-4.2.9/crest4/tests/precomputed_hits/two_seqs.fasta`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/crest4/tests/readme_example_seq/run_test.py` & `crest4-4.2.9/crest4/tests/readme_example_seq/run_test.py`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/crest4/tests/score_drop_change/run_test.py` & `crest4-4.2.9/crest4/tests/score_drop_change/run_test.py`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/crest4/tests/score_drop_change/two_seqs.fasta` & `crest4-4.2.9/crest4/tests/score_drop_change/two_seqs.fasta`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/crest4/tests/vsearch_test/run_test.py` & `crest4-4.2.9/crest4/tests/vsearch_test/run_test.py`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/crest4/tests/vsearch_test/two_seqs.fasta` & `crest4-4.2.9/crest4/tests/vsearch_test/two_seqs.fasta`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/crest4/tests/with_otu_table/run_test.py` & `crest4-4.2.9/crest4/tests/with_otu_table/run_test.py`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/crest4/tests/with_otu_table/seqs.fasta` & `crest4-4.2.9/crest4/tests/with_otu_table/seqs.fasta`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/crest4.egg-info/PKG-INFO` & `crest4-4.2.9/crest4.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: crest4
-Version: 4.2.7
+Version: 4.2.9
 Summary: The `crest4` python package can automatically assign taxonomic names to DNA sequences obtained from environmental sequencing.
 Home-page: https://github.com/xapple/crest4/
 Author: Anders Lanzén and Lucas Sinclair
 Author-email: anders.lanzen@gmail.com
 License: GPL3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![PyPI version](https://badge.fury.io/py/crest4.svg)](https://badge.fury.io/py/crest4)
 ![Pytest passing](https://github.com/xapple/crest4/actions/workflows/pytest_master_branch.yml/badge.svg)
 
-# CREST version 4.2.7
+# CREST version 4.2.9
 
 `crest4` is a python package for automatically assigning taxonomic names to DNA sequences obtained from environmental sequencing.
 
 <p align="center">
 <img height="143" src="docs/logo.png?raw=true" alt="CREST Logo">
 </p>
 
@@ -60,15 +60,15 @@
 
     $ pip3 install crest4
 
 ### Notes and extras
 
 Once the installation completes you are ready to use the `crest4` executable command from the shell. Please note that the reference databases are downloaded automatically during first run, so this might take some time depending on your internet connection.
 
-In order to search the reference databases, you will also need either BLAST or VSEARCH installed. These are installed automatically with the `conda` method, but not with the `pip` method. You can obtain these with these commands on Linux:
+In order to search the reference databases, you will also need either BLAST or VSEARCH installed. These can be installed automatically with the `conda` package manager. If you don't use `conda`, you can obtain them with these commands on Linux:
 
     $ sudo apt update
     $ sudo apt install ncbi-blast+
     $ sudo apt install vsearch
 
 Or these commands on macOS:
 
@@ -133,17 +133,16 @@
                         similarity search. By default, parallelism is turned
                         off and this value is 1. If you pass the value `True`
                         we will run as many processes as there are CPUs but
                         no more than 32.
 
   --search_db DATABASE, -d DATABASE
                         The database used for the sequence similarity search.
-                        Either `midori248`, `silvamod138`, or `silvamod128`.
-                        No other values are currently supported.
-                        By default, `silvamod138`. Optionally, the user can
+                        Either `midori253darn`, or `silvamod138pr2`.
+                        By default, `silvamod138pr2`. Optionally, the user can
                         provide a custom database by specifying the full path
                         to a directory containing all required files under
                         `search_db`. See the README for more information.
 
   --output_dir DIR, -o DIR
                         The directory into which all the classification
                         results will be written to. This defaults to a
@@ -298,8 +297,8 @@
 
 The internal documentation of the `crest4` python package is available at:
 
 http://xapple.github.io/crest4/crest4
 
 This documentation is simply generated from the source code with this command:
 
-    $ pdoc3 --html --output-dir docs --force crest4
+    $ pdoc --output-dir docs crest4
```

### Comparing `crest4-4.2.7/crest4.egg-info/SOURCES.txt` & `crest4-4.2.9/crest4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crest4-4.2.7/setup.py` & `crest4-4.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 this_dir = path.abspath(path.dirname(__file__))
 readme_path = path.join(this_dir, 'README.md')
 with open(readme_path, encoding='utf-8') as handle: readme = handle.read()
 
 # Call setup #
 setup(
     name             = 'crest4',
-    version          = '4.2.7',
+    version          = '4.2.9',
     description      = 'The `crest4` python package can automatically assign '
                        'taxonomic names to DNA sequences obtained from '
                        'environmental sequencing.',
     license          = 'GPL3',
     url              = 'https://github.com/xapple/crest4/',
     author           = 'Anders Lanzén and Lucas Sinclair',
     author_email     = 'anders.lanzen@gmail.com',
```

