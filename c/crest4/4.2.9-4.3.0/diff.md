# Comparing `tmp/crest4-4.2.9.tar.gz` & `tmp/crest4-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crest4-4.2.9.tar", last modified: Mon May 29 14:31:53 2023, max compression
+gzip compressed data, was "crest4-4.3.0.tar", last modified: Mon May 29 15:32:50 2023, max compression
```

## Comparing `crest4-4.2.9.tar` & `crest4-4.3.0.tar`

### file list

```diff
@@ -1,74 +1,78 @@
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.988650 crest4-4.2.9/
--rw-r--r--   0 sinclair   (501) staff       (20)    35149 2021-04-19 16:21:09.000000 crest4-4.2.9/LICENSE.txt
--rw-r--r--   0 sinclair   (501) staff       (20)      623 2022-05-20 08:41:00.000000 crest4-4.2.9/MANIFEST.in
--rw-r--r--   0 sinclair   (501) staff       (20)    18815 2023-05-29 14:31:53.988505 crest4-4.2.9/PKG-INFO
--rw-r--r--   0 sinclair   (501) staff       (20)    18337 2023-05-29 14:31:44.000000 crest4-4.2.9/README.md
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.980107 crest4-4.2.9/crest4/
--rw-r--r--   0 sinclair   (501) staff       (20)      507 2023-05-29 14:31:44.000000 crest4-4.2.9/crest4/__init__.py
--rw-r--r--   0 sinclair   (501) staff       (20)      478 2023-01-19 16:17:41.000000 crest4-4.2.9/crest4/__main__.py
--rw-r--r--   0 sinclair   (501) staff       (20)    16194 2023-05-29 14:27:45.000000 crest4-4.2.9/crest4/classify.py
--rw-r--r--   0 sinclair   (501) staff       (20)    11755 2023-05-29 14:25:07.000000 crest4-4.2.9/crest4/databases.py
--rw-r--r--   0 sinclair   (501) staff       (20)     4616 2023-05-29 14:25:32.000000 crest4-4.2.9/crest4/otu_tables.py
--rw-r--r--   0 sinclair   (501) staff       (20)     6339 2023-01-19 16:17:29.000000 crest4-4.2.9/crest4/query.py
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.981178 crest4-4.2.9/crest4/tests/
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.981736 crest4-4.2.9/crest4/tests/actualize_database/
--rw-r--r--   0 sinclair   (501) staff       (20)      207 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/actualize_database/README.md
--rw-r--r--   0 sinclair   (501) staff       (20)     1262 2021-10-17 14:02:01.000000 crest4-4.2.9/crest4/tests/actualize_database/run_test.py
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.982201 crest4-4.2.9/crest4/tests/cmd_line_tool/
--rw-r--r--   0 sinclair   (501) staff       (20)       84 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/cmd_line_tool/README.md
--rw-r--r--   0 sinclair   (501) staff       (20)     1343 2022-05-28 21:46:13.000000 crest4-4.2.9/crest4/tests/cmd_line_tool/run_test.py
--rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/cmd_line_tool/two_seqs.fasta
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.982692 crest4-4.2.9/crest4/tests/custom_database/
--rw-r--r--   0 sinclair   (501) staff       (20)      110 2022-05-19 13:31:03.000000 crest4-4.2.9/crest4/tests/custom_database/README.md
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.983488 crest4-4.2.9/crest4/tests/custom_database/custom/
--rw-r--r--   0 sinclair   (501) staff       (20)     3049 2022-05-17 09:31:56.000000 crest4-4.2.9/crest4/tests/custom_database/custom/custom.fasta
--rw-r--r--   0 sinclair   (501) staff       (20)       21 2022-05-17 09:30:46.000000 crest4-4.2.9/crest4/tests/custom_database/custom/custom.map
--rw-r--r--   0 sinclair   (501) staff       (20)       28 2022-05-17 09:31:38.000000 crest4-4.2.9/crest4/tests/custom_database/custom/custom.names
--rw-r--r--   0 sinclair   (501) staff       (20)        5 2022-05-19 13:25:23.000000 crest4-4.2.9/crest4/tests/custom_database/custom/custom.tre
--rw-r--r--   0 sinclair   (501) staff       (20)     1283 2022-05-19 13:27:20.000000 crest4-4.2.9/crest4/tests/custom_database/run_test.py
--rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-04-30 12:29:37.000000 crest4-4.2.9/crest4/tests/custom_database/two_seqs.fasta
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.977145 crest4-4.2.9/crest4/tests/gio_hundred_seqs/
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.983705 crest4-4.2.9/crest4/tests/gio_hundred_seqs/expected_output/
--rw-r--r--   0 sinclair   (501) staff       (20)    51702 2021-04-08 11:31:48.000000 crest4-4.2.9/crest4/tests/gio_hundred_seqs/expected_output/assigned.fasta
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.984763 crest4-4.2.9/crest4/tests/ncbi_two_sequences/
--rw-r--r--   0 sinclair   (501) staff       (20)      505 2021-05-27 13:51:38.000000 crest4-4.2.9/crest4/tests/ncbi_two_sequences/README.md
--rw-r--r--   0 sinclair   (501) staff       (20)     1404 2023-01-19 16:17:26.000000 crest4-4.2.9/crest4/tests/ncbi_two_sequences/generate.py
--rw-r--r--   0 sinclair   (501) staff       (20)     1219 2022-05-28 21:42:52.000000 crest4-4.2.9/crest4/tests/ncbi_two_sequences/run_test.py
--rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-04-30 12:29:37.000000 crest4-4.2.9/crest4/tests/ncbi_two_sequences/two_seqs.fasta
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.985271 crest4-4.2.9/crest4/tests/no_hits_sequence/
--rw-r--r--   0 sinclair   (501) staff       (20)      127 2021-05-17 17:36:29.000000 crest4-4.2.9/crest4/tests/no_hits_sequence/README.md
--rw-r--r--   0 sinclair   (501) staff       (20)     1268 2021-05-16 19:12:40.000000 crest4-4.2.9/crest4/tests/no_hits_sequence/no_hits.fasta
--rw-r--r--   0 sinclair   (501) staff       (20)     1895 2022-05-28 21:47:24.000000 crest4-4.2.9/crest4/tests/no_hits_sequence/run_test.py
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.985975 crest4-4.2.9/crest4/tests/precomputed_hits/
--rw-r--r--   0 sinclair   (501) staff       (20)      116 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/precomputed_hits/README.md
--rw-r--r--   0 sinclair   (501) staff       (20)     7287 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/precomputed_hits/precomputed.hits
--rw-r--r--   0 sinclair   (501) staff       (20)     1421 2022-05-28 21:06:11.000000 crest4-4.2.9/crest4/tests/precomputed_hits/run_test.py
--rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/precomputed_hits/two_seqs.fasta
--rw-r--r--   0 sinclair   (501) staff       (20)       42 2021-05-17 17:16:58.000000 crest4-4.2.9/crest4/tests/pytest.ini
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.986444 crest4-4.2.9/crest4/tests/readme_example_seq/
--rw-r--r--   0 sinclair   (501) staff       (20)      307 2021-05-18 00:43:16.000000 crest4-4.2.9/crest4/tests/readme_example_seq/README.md
--rw-r--r--   0 sinclair   (501) staff       (20)      341 2021-05-17 18:22:13.000000 crest4-4.2.9/crest4/tests/readme_example_seq/readme_test.fasta
--rw-r--r--   0 sinclair   (501) staff       (20)     1156 2022-05-28 21:43:14.000000 crest4-4.2.9/crest4/tests/readme_example_seq/run_test.py
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.986917 crest4-4.2.9/crest4/tests/score_drop_change/
--rw-r--r--   0 sinclair   (501) staff       (20)      118 2021-10-17 13:39:41.000000 crest4-4.2.9/crest4/tests/score_drop_change/README.md
--rw-r--r--   0 sinclair   (501) staff       (20)     1352 2022-05-28 21:47:50.000000 crest4-4.2.9/crest4/tests/score_drop_change/run_test.py
--rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-04-30 12:29:37.000000 crest4-4.2.9/crest4/tests/score_drop_change/two_seqs.fasta
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.987408 crest4-4.2.9/crest4/tests/vsearch_test/
--rw-r--r--   0 sinclair   (501) staff       (20)       62 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/vsearch_test/README.md
--rw-r--r--   0 sinclair   (501) staff       (20)     1250 2022-05-28 21:43:30.000000 crest4-4.2.9/crest4/tests/vsearch_test/run_test.py
--rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/vsearch_test/two_seqs.fasta
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.988162 crest4-4.2.9/crest4/tests/with_otu_table/
--rw-r--r--   0 sinclair   (501) staff       (20)      107 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/with_otu_table/README.md
--rw-r--r--   0 sinclair   (501) staff       (20)      101 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/with_otu_table/otu_table_bad.tsv
--rw-r--r--   0 sinclair   (501) staff       (20)      135 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/with_otu_table/otu_table_good.tsv
--rw-r--r--   0 sinclair   (501) staff       (20)     2161 2022-05-28 21:07:24.000000 crest4-4.2.9/crest4/tests/with_otu_table/run_test.py
--rw-r--r--   0 sinclair   (501) staff       (20)     4639 2021-07-13 09:13:43.000000 crest4-4.2.9/crest4/tests/with_otu_table/seqs.fasta
-drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 14:31:53.981047 crest4-4.2.9/crest4.egg-info/
--rw-r--r--   0 sinclair   (501) staff       (20)    18815 2023-05-29 14:31:53.000000 crest4-4.2.9/crest4.egg-info/PKG-INFO
--rw-r--r--   0 sinclair   (501) staff       (20)     2011 2023-05-29 14:31:53.000000 crest4-4.2.9/crest4.egg-info/SOURCES.txt
--rw-r--r--   0 sinclair   (501) staff       (20)        1 2023-05-29 14:31:53.000000 crest4-4.2.9/crest4.egg-info/dependency_links.txt
--rw-r--r--   0 sinclair   (501) staff       (20)       48 2023-05-29 14:31:53.000000 crest4-4.2.9/crest4.egg-info/entry_points.txt
--rw-r--r--   0 sinclair   (501) staff       (20)      115 2023-05-29 14:31:53.000000 crest4-4.2.9/crest4.egg-info/requires.txt
--rw-r--r--   0 sinclair   (501) staff       (20)       17 2023-05-29 14:31:53.000000 crest4-4.2.9/crest4.egg-info/top_level.txt
--rw-r--r--   0 sinclair   (501) staff       (20)       38 2023-05-29 14:31:53.988686 crest4-4.2.9/setup.cfg
--rw-r--r--   0 sinclair   (501) staff       (20)     1442 2023-05-29 14:31:44.000000 crest4-4.2.9/setup.py
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 15:32:50.236786 crest4-4.3.0/
+-rw-r--r--   0 sinclair   (501) staff       (20)    35149 2021-04-19 16:21:09.000000 crest4-4.3.0/LICENSE.txt
+-rw-r--r--   0 sinclair   (501) staff       (20)      623 2022-05-20 08:41:00.000000 crest4-4.3.0/MANIFEST.in
+-rw-r--r--   0 sinclair   (501) staff       (20)    18815 2023-05-29 15:32:50.236629 crest4-4.3.0/PKG-INFO
+-rw-r--r--   0 sinclair   (501) staff       (20)    18337 2023-05-29 15:32:41.000000 crest4-4.3.0/README.md
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 15:32:50.227187 crest4-4.3.0/crest4/
+-rw-r--r--   0 sinclair   (501) staff       (20)      507 2023-05-29 15:32:41.000000 crest4-4.3.0/crest4/__init__.py
+-rw-r--r--   0 sinclair   (501) staff       (20)      478 2023-01-19 16:17:41.000000 crest4-4.3.0/crest4/__main__.py
+-rw-r--r--   0 sinclair   (501) staff       (20)    16229 2023-05-29 15:24:14.000000 crest4-4.3.0/crest4/classify.py
+-rw-r--r--   0 sinclair   (501) staff       (20)    11867 2023-05-29 15:24:45.000000 crest4-4.3.0/crest4/databases.py
+-rw-r--r--   0 sinclair   (501) staff       (20)     4616 2023-05-29 14:25:32.000000 crest4-4.3.0/crest4/otu_tables.py
+-rw-r--r--   0 sinclair   (501) staff       (20)     6339 2023-01-19 16:17:29.000000 crest4-4.3.0/crest4/query.py
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 15:32:50.228185 crest4-4.3.0/crest4/tests/
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 15:32:50.228652 crest4-4.3.0/crest4/tests/actualize_database/
+-rw-r--r--   0 sinclair   (501) staff       (20)      207 2021-07-13 09:13:43.000000 crest4-4.3.0/crest4/tests/actualize_database/README.md
+-rw-r--r--   0 sinclair   (501) staff       (20)     1337 2023-05-29 15:17:11.000000 crest4-4.3.0/crest4/tests/actualize_database/run_test.py
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 15:32:50.229319 crest4-4.3.0/crest4/tests/cmd_line_tool/
+-rw-r--r--   0 sinclair   (501) staff       (20)       84 2021-07-13 09:13:43.000000 crest4-4.3.0/crest4/tests/cmd_line_tool/README.md
+-rw-r--r--   0 sinclair   (501) staff       (20)     1286 2023-05-29 15:16:12.000000 crest4-4.3.0/crest4/tests/cmd_line_tool/run_test.py
+-rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-07-13 09:13:43.000000 crest4-4.3.0/crest4/tests/cmd_line_tool/two_seqs.fasta
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 15:32:50.229823 crest4-4.3.0/crest4/tests/custom_database/
+-rw-r--r--   0 sinclair   (501) staff       (20)      110 2022-05-19 13:31:03.000000 crest4-4.3.0/crest4/tests/custom_database/README.md
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 15:32:50.230621 crest4-4.3.0/crest4/tests/custom_database/custom/
+-rw-r--r--   0 sinclair   (501) staff       (20)     3049 2022-05-17 09:31:56.000000 crest4-4.3.0/crest4/tests/custom_database/custom/custom.fasta
+-rw-r--r--   0 sinclair   (501) staff       (20)       21 2022-05-17 09:30:46.000000 crest4-4.3.0/crest4/tests/custom_database/custom/custom.map
+-rw-r--r--   0 sinclair   (501) staff       (20)       28 2022-05-17 09:31:38.000000 crest4-4.3.0/crest4/tests/custom_database/custom/custom.names
+-rw-r--r--   0 sinclair   (501) staff       (20)        5 2022-05-19 13:25:23.000000 crest4-4.3.0/crest4/tests/custom_database/custom/custom.tre
+-rw-r--r--   0 sinclair   (501) staff       (20)     1283 2022-05-19 13:27:20.000000 crest4-4.3.0/crest4/tests/custom_database/run_test.py
+-rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-04-30 12:29:37.000000 crest4-4.3.0/crest4/tests/custom_database/two_seqs.fasta
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 15:32:50.224408 crest4-4.3.0/crest4/tests/gio_hundred_seqs/
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 15:32:50.230826 crest4-4.3.0/crest4/tests/gio_hundred_seqs/expected_output/
+-rw-r--r--   0 sinclair   (501) staff       (20)    51702 2021-04-08 11:31:48.000000 crest4-4.3.0/crest4/tests/gio_hundred_seqs/expected_output/assigned.fasta
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 15:32:50.231855 crest4-4.3.0/crest4/tests/midori_test/
+-rw-r--r--   0 sinclair   (501) staff       (20)       62 2023-05-29 15:22:06.000000 crest4-4.3.0/crest4/tests/midori_test/README.md
+-rw-r--r--   0 sinclair   (501) staff       (20)     1237 2023-05-29 15:23:13.000000 crest4-4.3.0/crest4/tests/midori_test/run_test.py
+-rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-07-13 09:13:43.000000 crest4-4.3.0/crest4/tests/midori_test/two_seqs.fasta
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 15:32:50.232606 crest4-4.3.0/crest4/tests/ncbi_two_sequences/
+-rw-r--r--   0 sinclair   (501) staff       (20)      505 2021-05-27 13:51:38.000000 crest4-4.3.0/crest4/tests/ncbi_two_sequences/README.md
+-rw-r--r--   0 sinclair   (501) staff       (20)     1404 2023-01-19 16:17:26.000000 crest4-4.3.0/crest4/tests/ncbi_two_sequences/generate.py
+-rw-r--r--   0 sinclair   (501) staff       (20)     1172 2023-05-29 15:15:44.000000 crest4-4.3.0/crest4/tests/ncbi_two_sequences/run_test.py
+-rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-04-30 12:29:37.000000 crest4-4.3.0/crest4/tests/ncbi_two_sequences/two_seqs.fasta
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 15:32:50.233022 crest4-4.3.0/crest4/tests/no_hits_sequence/
+-rw-r--r--   0 sinclair   (501) staff       (20)      127 2021-05-17 17:36:29.000000 crest4-4.3.0/crest4/tests/no_hits_sequence/README.md
+-rw-r--r--   0 sinclair   (501) staff       (20)     1268 2021-05-16 19:12:40.000000 crest4-4.3.0/crest4/tests/no_hits_sequence/no_hits.fasta
+-rw-r--r--   0 sinclair   (501) staff       (20)     1889 2023-05-29 15:14:45.000000 crest4-4.3.0/crest4/tests/no_hits_sequence/run_test.py
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 15:32:50.233856 crest4-4.3.0/crest4/tests/precomputed_hits/
+-rw-r--r--   0 sinclair   (501) staff       (20)      116 2021-07-13 09:13:43.000000 crest4-4.3.0/crest4/tests/precomputed_hits/README.md
+-rw-r--r--   0 sinclair   (501) staff       (20)     7287 2021-07-13 09:13:43.000000 crest4-4.3.0/crest4/tests/precomputed_hits/precomputed.hits
+-rw-r--r--   0 sinclair   (501) staff       (20)     1375 2023-05-29 15:15:27.000000 crest4-4.3.0/crest4/tests/precomputed_hits/run_test.py
+-rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-07-13 09:13:43.000000 crest4-4.3.0/crest4/tests/precomputed_hits/two_seqs.fasta
+-rw-r--r--   0 sinclair   (501) staff       (20)       42 2021-05-17 17:16:58.000000 crest4-4.3.0/crest4/tests/pytest.ini
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 15:32:50.234331 crest4-4.3.0/crest4/tests/readme_example_seq/
+-rw-r--r--   0 sinclair   (501) staff       (20)      307 2021-05-18 00:43:16.000000 crest4-4.3.0/crest4/tests/readme_example_seq/README.md
+-rw-r--r--   0 sinclair   (501) staff       (20)      341 2021-05-17 18:22:13.000000 crest4-4.3.0/crest4/tests/readme_example_seq/readme_test.fasta
+-rw-r--r--   0 sinclair   (501) staff       (20)     1110 2023-05-29 15:15:19.000000 crest4-4.3.0/crest4/tests/readme_example_seq/run_test.py
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 15:32:50.234902 crest4-4.3.0/crest4/tests/score_drop_change/
+-rw-r--r--   0 sinclair   (501) staff       (20)      118 2021-10-17 13:39:41.000000 crest4-4.3.0/crest4/tests/score_drop_change/README.md
+-rw-r--r--   0 sinclair   (501) staff       (20)     1295 2023-05-29 15:15:13.000000 crest4-4.3.0/crest4/tests/score_drop_change/run_test.py
+-rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-04-30 12:29:37.000000 crest4-4.3.0/crest4/tests/score_drop_change/two_seqs.fasta
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 15:32:50.235497 crest4-4.3.0/crest4/tests/vsearch_test/
+-rw-r--r--   0 sinclair   (501) staff       (20)       62 2021-07-13 09:13:43.000000 crest4-4.3.0/crest4/tests/vsearch_test/README.md
+-rw-r--r--   0 sinclair   (501) staff       (20)     1191 2023-05-29 15:23:20.000000 crest4-4.3.0/crest4/tests/vsearch_test/run_test.py
+-rw-r--r--   0 sinclair   (501) staff       (20)     3082 2021-07-13 09:13:43.000000 crest4-4.3.0/crest4/tests/vsearch_test/two_seqs.fasta
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 15:32:50.236302 crest4-4.3.0/crest4/tests/with_otu_table/
+-rw-r--r--   0 sinclair   (501) staff       (20)      107 2021-07-13 09:13:43.000000 crest4-4.3.0/crest4/tests/with_otu_table/README.md
+-rw-r--r--   0 sinclair   (501) staff       (20)      101 2021-07-13 09:13:43.000000 crest4-4.3.0/crest4/tests/with_otu_table/otu_table_bad.tsv
+-rw-r--r--   0 sinclair   (501) staff       (20)      135 2021-07-13 09:13:43.000000 crest4-4.3.0/crest4/tests/with_otu_table/otu_table_good.tsv
+-rw-r--r--   0 sinclair   (501) staff       (20)     2068 2023-05-29 15:14:56.000000 crest4-4.3.0/crest4/tests/with_otu_table/run_test.py
+-rw-r--r--   0 sinclair   (501) staff       (20)     4639 2021-07-13 09:13:43.000000 crest4-4.3.0/crest4/tests/with_otu_table/seqs.fasta
+drwxr-xr-x   0 sinclair   (501) staff       (20)        0 2023-05-29 15:32:50.228062 crest4-4.3.0/crest4.egg-info/
+-rw-r--r--   0 sinclair   (501) staff       (20)    18815 2023-05-29 15:32:50.000000 crest4-4.3.0/crest4.egg-info/PKG-INFO
+-rw-r--r--   0 sinclair   (501) staff       (20)     2123 2023-05-29 15:32:50.000000 crest4-4.3.0/crest4.egg-info/SOURCES.txt
+-rw-r--r--   0 sinclair   (501) staff       (20)        1 2023-05-29 15:32:50.000000 crest4-4.3.0/crest4.egg-info/dependency_links.txt
+-rw-r--r--   0 sinclair   (501) staff       (20)       48 2023-05-29 15:32:50.000000 crest4-4.3.0/crest4.egg-info/entry_points.txt
+-rw-r--r--   0 sinclair   (501) staff       (20)      115 2023-05-29 15:32:50.000000 crest4-4.3.0/crest4.egg-info/requires.txt
+-rw-r--r--   0 sinclair   (501) staff       (20)       17 2023-05-29 15:32:50.000000 crest4-4.3.0/crest4.egg-info/top_level.txt
+-rw-r--r--   0 sinclair   (501) staff       (20)       38 2023-05-29 15:32:50.236831 crest4-4.3.0/setup.cfg
+-rw-r--r--   0 sinclair   (501) staff       (20)     1442 2023-05-29 15:32:41.000000 crest4-4.3.0/setup.py
```

### Comparing `crest4-4.2.9/LICENSE.txt` & `crest4-4.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crest4-4.2.9/MANIFEST.in` & `crest4-4.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `crest4-4.2.9/PKG-INFO` & `crest4-4.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: crest4
-Version: 4.2.9
+Version: 4.3.0
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
 
-# CREST version 4.2.9
+# CREST version 4.3.0
 
 `crest4` is a python package for automatically assigning taxonomic names to DNA sequences obtained from environmental sequencing.
 
 <p align="center">
 <img height="143" src="docs/logo.png?raw=true" alt="CREST Logo">
 </p>
```

### Comparing `crest4-4.2.9/README.md` & `crest4-4.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [![PyPI version](https://badge.fury.io/py/crest4.svg)](https://badge.fury.io/py/crest4)
 ![Pytest passing](https://github.com/xapple/crest4/actions/workflows/pytest_master_branch.yml/badge.svg)
 
-# CREST version 4.2.9
+# CREST version 4.3.0
 
 `crest4` is a python package for automatically assigning taxonomic names to DNA sequences obtained from environmental sequencing.
 
 <p align="center">
 <img height="143" src="docs/logo.png?raw=true" alt="CREST Logo">
 </p>
```

### Comparing `crest4-4.2.9/crest4/classify.py` & `crest4-4.3.0/crest4/classify.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 
 # First party modules #
 from plumbing.cache      import property_cached
 from autopaths.file_path import FilePath
 from autopaths.dir_path  import DirectoryPath
 
 # Constants #
-all_db_choices = ('midori248', 'silvamod138', 'silvamod138pr2', 'silvamod128')
+all_db_choices = ('midori248', 'midori253darn', 'silvamod138',
+                  'silvamod138pr2', 'silvamod128')
 
 ###############################################################################
 class Classify:
     """
     This is the main object offered by the `crest4` package.
     It enables you to automatically assign taxonomic names to DNA sequences
     obtained from environmental sequencing.
```

### Comparing `crest4-4.2.9/crest4/databases.py` & `crest4-4.3.0/crest4/databases.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,16 +284,19 @@
                 'Strain',         # 11
                 'Strain',         # 12
                 'Strain',         # 13 (There is a problem with too many ranks
                 'Strain']         # 14  in some databases requiring this)
 
 ###############################################################################
 # As our databases should only be stored on disk once, so we have singletons #
-midori248   = CrestDatabase('midori248',
-                            'The midori248darn database for CREST')
+midori248 = CrestDatabase('midori248',
+                          'The midori248darn database for CREST')
+
+midori253darn = CrestDatabase('midori253darn',
+                            'The midori253darn database for CREST')
 
 silvamod138 = CrestDatabase('silvamod138',
                             'Silva version 138 modified for CREST')
 
 silvamod128 = CrestDatabase('silvamod128',
                             'Silva version 128 modified for CREST')
```

### Comparing `crest4-4.2.9/crest4/otu_tables.py` & `crest4-4.3.0/crest4/otu_tables.py`

 * *Files identical despite different names*

### Comparing `crest4-4.2.9/crest4/query.py` & `crest4-4.3.0/crest4/query.py`

 * *Files identical despite different names*

### Comparing `crest4-4.2.9/crest4/tests/actualize_database/run_test.py` & `crest4-4.3.0/crest4/tests/actualize_database/run_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,36 +9,39 @@
 import os
 
 # First party modules #
 
 # Third party modules #
 
 # Internal modules #
-from crest4.databases import metadata, silvamod138, CrestDatabase
+from crest4.databases import metadata, silvamod138pr2, CrestDatabase
+
+# Constants #
+env_val = os.environ.get(CrestDatabase.environ_var)
 
 ###############################################################################
 def test_download_metadata():
     urls = metadata.db_urls
     assert urls
 
 def test_blast_index():
-    db = silvamod138.blast_db
+    db = silvamod138pr2.blast_db
     assert db
 
 def test_vsearch_index():
-    db = silvamod138.vsearch_db
+    db = silvamod138pr2.vsearch_db
     assert db
 
 ###############################################################################
 if __name__ == '__main__':
     # Some debug information #
-    print("Default directory: ",      CrestDatabase.default_dir)
-    print("Environment variable: ",   CrestDatabase.environ_var)
-    print("Environment value: ",      os.environ.get(CrestDatabase.environ_var))
-    print("Silvamod138 path: ",       silvamod138.path)
-    print("Silvamod138 exists: ",     silvamod138.path.exists)
-    print("Silvamod138 downloaded: ", silvamod138.downloaded)
-    print("Silvamod138 URL: ",        silvamod138.url)
+    print("Default directory: ",         CrestDatabase.default_dir)
+    print("Environment variable: ",      CrestDatabase.environ_var)
+    print("Environment value: ",         env_val)
+    print("silvamod138pr2 path: ",       silvamod138pr2.path)
+    print("silvamod138pr2 exists: ",     silvamod138pr2.path.exists)
+    print("silvamod138pr2 downloaded: ", silvamod138pr2.downloaded)
+    print("silvamod138pr2 URL: ",        silvamod138pr2.url)
     # Run the three tests #
     test_download_metadata()
     test_blast_index()
     test_vsearch_index()
```

### Comparing `crest4-4.2.9/crest4/tests/cmd_line_tool/run_test.py` & `crest4-4.3.0/crest4/tests/cmd_line_tool/run_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     output_dir.remove()
     # Get the path of the current python executable #
     import sh
     this_python = sh.Command(sys.executable)
     # Call via the command line tool #
     result = this_python('-m',            'crest4',
                          '--fasta',       fasta,
-                         '--search_db',   'silvamod138',
                          '--output_dir',  output_dir,
                          '--num_threads', 'True')
     # Check that the results were created #
     created_file = output_dir + 'assignments.txt'
     assert created_file
     # Return #
     return result
```

### Comparing `crest4-4.2.9/crest4/tests/cmd_line_tool/two_seqs.fasta` & `crest4-4.3.0/crest4/tests/cmd_line_tool/two_seqs.fasta`

 * *Files identical despite different names*

### Comparing `crest4-4.2.9/crest4/tests/custom_database/custom/custom.fasta` & `crest4-4.3.0/crest4/tests/custom_database/custom/custom.fasta`

 * *Files identical despite different names*

### Comparing `crest4-4.2.9/crest4/tests/custom_database/run_test.py` & `crest4-4.3.0/crest4/tests/custom_database/run_test.py`

 * *Files identical despite different names*

### Comparing `crest4-4.2.9/crest4/tests/custom_database/two_seqs.fasta` & `crest4-4.3.0/crest4/tests/custom_database/two_seqs.fasta`

 * *Files identical despite different names*

### Comparing `crest4-4.2.9/crest4/tests/gio_hundred_seqs/expected_output/assigned.fasta` & `crest4-4.3.0/crest4/tests/gio_hundred_seqs/expected_output/assigned.fasta`

 * *Files identical despite different names*

### Comparing `crest4-4.2.9/crest4/tests/ncbi_two_sequences/generate.py` & `crest4-4.3.0/crest4/tests/ncbi_two_sequences/generate.py`

 * *Files identical despite different names*

### Comparing `crest4-4.2.9/crest4/tests/ncbi_two_sequences/run_test.py` & `crest4-4.3.0/crest4/tests/ncbi_two_sequences/run_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,20 +26,19 @@
     fasta = this_dir.find('*.fasta')
     # The output directory #
     output_dir = this_dir + 'results/'
     output_dir.remove()
     # Create object #
     c = Classify(fasta       = fasta,
                  output_dir  = output_dir,
-                 search_db   = 'silvamod138',
                  num_threads = True)
     # Run it #
     c()
     # Check that the results are good #
     assert c.queries_by_id['Kocuria'].taxonomy[0] == "Kocuria"
     assert c.queries_by_id['Marmoricola'].taxonomy[0] == "Marmoricola"
     # Return #
     return c
 
 ###############################################################################
 if __name__ == '__main__':
-    classify = test_ncbi_two_seqs()
+    classify = test_ncbi_two_seqs()
```

### Comparing `crest4-4.2.9/crest4/tests/ncbi_two_sequences/two_seqs.fasta` & `crest4-4.3.0/crest4/tests/midori_test/two_seqs.fasta`

 * *Files identical despite different names*

### Comparing `crest4-4.2.9/crest4/tests/no_hits_sequence/no_hits.fasta` & `crest4-4.3.0/crest4/tests/no_hits_sequence/no_hits.fasta`

 * *Files identical despite different names*

### Comparing `crest4-4.2.9/crest4/tests/no_hits_sequence/run_test.py` & `crest4-4.3.0/crest4/tests/no_hits_sequence/run_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     fasta = this_dir.find('*.fasta')
     # The output directory #
     output_dir = this_dir + 'results_blast/'
     output_dir.remove()
     # Create object #
     c = Classify(fasta       = fasta,
                  output_dir  = output_dir,
-                 search_db   = 'silvamod138',
+                 search_algo = 'blast',
                  num_threads = True)
     # Run it #
     c()
     # Check there was no hits for the second sequence #
     expected = "homopolymer\tNo hits"
     got = c.out_file.lines[1]
     assert got == expected
```

### Comparing `crest4-4.2.9/crest4/tests/precomputed_hits/precomputed.hits` & `crest4-4.3.0/crest4/tests/precomputed_hits/precomputed.hits`

 * *Files identical despite different names*

### Comparing `crest4-4.2.9/crest4/tests/precomputed_hits/run_test.py` & `crest4-4.3.0/crest4/tests/midori_test/run_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-Script to run the `precomputed_hits` integration test.
+Script to run the `vsearch` integration test.
 """
 
 # Built-in modules #
 import inspect
 
 # First party modules #
 from autopaths import Path
@@ -17,34 +17,30 @@
 from crest4 import Classify
 
 # Get the current directory of this python script #
 this_file = Path((inspect.stack()[0])[1])
 this_dir  = this_file.directory
 
 ###############################################################################
-def test_precomputed_hits():
+def test_midori():
     # The input fasta #
     fasta = this_dir.find('*.fasta')
-    # The input BLAST hits #
-    hits = this_dir.find('precomputed.hits')
     # The output directory #
     output_dir = this_dir + 'results/'
     output_dir.remove()
     # Create object #
     c = Classify(fasta       = fasta,
-                 search_hits = hits,
-                 search_db   = 'silvamod138',
                  output_dir  = output_dir,
+                 search_algo = 'vsearch',
+                 search_db   = 'midori253darn',
                  num_threads = True)
-    # Patch the search method so that it can't be called #
-    c.search = lambda x: x/0
     # Run it #
     c()
     # Check that the results are good #
     assert c.queries_by_id['Kocuria'].taxonomy[0] == "Kocuria"
     assert c.queries_by_id['Marmoricola'].taxonomy[0] == "Marmoricola"
     # Return #
     return c
 
 ###############################################################################
 if __name__ == '__main__':
-    classify = test_precomputed_hits()
+    classify = test_midori()
```

### Comparing `crest4-4.2.9/crest4/tests/precomputed_hits/two_seqs.fasta` & `crest4-4.3.0/crest4/tests/ncbi_two_sequences/two_seqs.fasta`

 * *Files identical despite different names*

### Comparing `crest4-4.2.9/crest4/tests/readme_example_seq/run_test.py` & `crest4-4.3.0/crest4/tests/readme_example_seq/run_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     fasta = this_dir.find('*.fasta')
     # The output directory #
     output_dir = this_dir + 'results/'
     output_dir.remove()
     # Create object #
     c = Classify(fasta       = fasta,
                  output_dir  = output_dir,
-                 search_db   = 'silvamod138',
                  num_threads = True)
     # Run it #
     c()
     # Check that the results are good #
     assert c.queries[0].taxonomy[0] == "Nodosilinea PCC-7104"
     # Return #
     return c
```

### Comparing `crest4-4.2.9/crest4/tests/score_drop_change/run_test.py` & `crest4-4.3.0/crest4/tests/score_drop_change/run_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     output_dir.remove()
     # Get the path of the current python executable #
     import sh
     this_python = sh.Command(sys.executable)
     # Call via the command line tool #
     result = this_python('-m',            'crest4',
                          '--fasta',       fasta,
-                         '--search_db',   'silvamod138',
                          '--output_dir',  output_dir,
                          '--score_drop',  '1')
     # Check that the results were created #
     created_file = output_dir + 'assignments.txt'
     assert created_file
     # Return #
     return result
```

### Comparing `crest4-4.2.9/crest4/tests/score_drop_change/two_seqs.fasta` & `crest4-4.3.0/crest4/tests/precomputed_hits/two_seqs.fasta`

 * *Files identical despite different names*

### Comparing `crest4-4.2.9/crest4/tests/vsearch_test/run_test.py` & `crest4-4.3.0/crest4/tests/vsearch_test/run_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,30 +17,29 @@
 from crest4 import Classify
 
 # Get the current directory of this python script #
 this_file = Path((inspect.stack()[0])[1])
 this_dir  = this_file.directory
 
 ###############################################################################
-def test_vsearch(verbose=True):
+def test_vsearch():
     # The input fasta #
     fasta = this_dir.find('*.fasta')
     # The output directory #
     output_dir = this_dir + 'results/'
     output_dir.remove()
     # Create object #
     c = Classify(fasta       = fasta,
                  output_dir  = output_dir,
                  search_algo = 'vsearch',
-                 search_db   = 'silvamod138',
                  num_threads = True)
     # Run it #
     c()
     # Check that the results are good #
     assert c.queries_by_id['Kocuria'].taxonomy[0] == "Kocuria"
     assert c.queries_by_id['Marmoricola'].taxonomy[0] == "Marmoricola"
     # Return #
     return c
 
 ###############################################################################
 if __name__ == '__main__':
-    classify = test_vsearch()
+    classify = test_vsearch()
```

### Comparing `crest4-4.2.9/crest4/tests/vsearch_test/two_seqs.fasta` & `crest4-4.3.0/crest4/tests/score_drop_change/two_seqs.fasta`

 * *Files identical despite different names*

### Comparing `crest4-4.2.9/crest4/tests/with_otu_table/run_test.py` & `crest4-4.3.0/crest4/tests/with_otu_table/run_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     otu_table = this_dir.find('*bad.tsv')
     # The output directory #
     output_dir = this_dir + 'results_bad/'
     output_dir.remove()
     # Create object #
     c = Classify(fasta       = fasta,
                  output_dir  = output_dir,
-                 search_db   = 'silvamod138',
                  num_threads = True,
                  otu_table   = otu_table)
     # It should complain when we run it #
     with pytest.raises(ValueError): c()
 
 ###############################################################################
 def test_with_good_otu_table():
@@ -47,15 +46,14 @@
     otu_table = this_dir.find('*good.tsv')
     # The output directory #
     output_dir = this_dir + 'results_good/'
     output_dir.remove()
     # Create object #
     c = Classify(fasta       = fasta,
                  output_dir  = output_dir,
-                 search_db   = 'silvamod138',
                  num_threads = True,
                  otu_table   = otu_table)
     # Run it #
     c()
     # Check that the results are good #
     assert all(c.otu_info.otus_by_rank['river'].array == [51, 10])
     assert all(c.otu_info.otus_by_rank['lake'].array  == [102, 50])
@@ -64,8 +62,8 @@
     return c
 
 ###############################################################################
 if __name__ == '__main__':
     # The bad case #
     classify_bad = test_with_bad_otu_table()
     # The good case #
-    classify_good = test_with_good_otu_table()
+    classify_good = test_with_good_otu_table()
```

### Comparing `crest4-4.2.9/crest4/tests/with_otu_table/seqs.fasta` & `crest4-4.3.0/crest4/tests/with_otu_table/seqs.fasta`

 * *Files identical despite different names*

### Comparing `crest4-4.2.9/crest4.egg-info/PKG-INFO` & `crest4-4.3.0/crest4.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: crest4
-Version: 4.2.9
+Version: 4.3.0
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
 
-# CREST version 4.2.9
+# CREST version 4.3.0
 
 `crest4` is a python package for automatically assigning taxonomic names to DNA sequences obtained from environmental sequencing.
 
 <p align="center">
 <img height="143" src="docs/logo.png?raw=true" alt="CREST Logo">
 </p>
```

### Comparing `crest4-4.2.9/crest4.egg-info/SOURCES.txt` & `crest4-4.3.0/crest4.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 crest4/tests/custom_database/run_test.py
 crest4/tests/custom_database/two_seqs.fasta
 crest4/tests/custom_database/custom/custom.fasta
 crest4/tests/custom_database/custom/custom.map
 crest4/tests/custom_database/custom/custom.names
 crest4/tests/custom_database/custom/custom.tre
 crest4/tests/gio_hundred_seqs/expected_output/assigned.fasta
+crest4/tests/midori_test/README.md
+crest4/tests/midori_test/run_test.py
+crest4/tests/midori_test/two_seqs.fasta
 crest4/tests/ncbi_two_sequences/README.md
 crest4/tests/ncbi_two_sequences/generate.py
 crest4/tests/ncbi_two_sequences/run_test.py
 crest4/tests/ncbi_two_sequences/two_seqs.fasta
 crest4/tests/no_hits_sequence/README.md
 crest4/tests/no_hits_sequence/no_hits.fasta
 crest4/tests/no_hits_sequence/run_test.py
```

### Comparing `crest4-4.2.9/setup.py` & `crest4-4.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 this_dir = path.abspath(path.dirname(__file__))
 readme_path = path.join(this_dir, 'README.md')
 with open(readme_path, encoding='utf-8') as handle: readme = handle.read()
 
 # Call setup #
 setup(
     name             = 'crest4',
-    version          = '4.2.9',
+    version          = '4.3.0',
     description      = 'The `crest4` python package can automatically assign '
                        'taxonomic names to DNA sequences obtained from '
                        'environmental sequencing.',
     license          = 'GPL3',
     url              = 'https://github.com/xapple/crest4/',
     author           = 'Anders Lanzén and Lucas Sinclair',
     author_email     = 'anders.lanzen@gmail.com',
```

