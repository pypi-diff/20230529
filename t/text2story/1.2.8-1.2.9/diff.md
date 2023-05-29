# Comparing `tmp/text2story-1.2.8.tar.gz` & `tmp/text2story-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2story-1.2.8.tar", last modified: Wed May 24 22:21:08 2023, max compression
+gzip compressed data, was "text2story-1.2.9.tar", last modified: Wed May 24 22:29:11 2023, max compression
```

## Comparing `text2story-1.2.8.tar` & `text2story-1.2.9.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.954553 text2story-1.2.8/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    33470 2022-10-19 09:22:59.000000 text2story-1.2.8/LICENSE
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      442 2023-03-29 14:01:55.000000 text2story-1.2.8/MANIFEST.in
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9774 2023-05-24 22:21:08.954553 text2story-1.2.8/PKG-INFO
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     8575 2023-05-17 10:11:38.000000 text2story-1.2.8/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      114 2023-03-29 13:58:48.000000 text2story-1.2.8/pyproject.toml
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1581 2023-05-24 22:21:08.954553 text2story-1.2.8/setup.cfg
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       70 2023-03-29 13:48:56.000000 text2story-1.2.8/setup.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.946550 text2story-1.2.8/text2story/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      757 2022-10-19 09:12:42.000000 text2story-1.2.8/text2story/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       67 2022-10-19 09:12:42.000000 text2story-1.2.8/text2story/__main__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.946550 text2story-1.2.8/text2story/annotators/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.946550 text2story-1.2.8/text2story/annotators/ALLENNLP/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.942548 text2story-1.2.8/text2story/annotators/ALLENNLP/Models/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.946550 text2story-1.2.8/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.946550 text2story-1.2.8/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      739 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       14 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/non_padded_namespaces.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1343 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   265058 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10386 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/annotators/ALLENNLP/PropBankBr.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    25595 2023-05-22 15:42:56.000000 text2story-1.2.8/text2story/annotators/ALLENNLP/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13691 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/annotators/ALLENNLP/my_model.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    20375 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/annotators/ALLENNLP/my_reader.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6217 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/annotators/ALLENNLP/preprocess.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.950552 text2story-1.2.8/text2story/annotators/CUSTOMPT/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14794 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/annotators/CUSTOMPT/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   371646 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/annotators/CUSTOMPT/crf_v2.1.joblib
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15093 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/annotators/CUSTOMPT/event_model.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13972 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/annotators/CUSTOMPT/feature_extractor.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.950552 text2story-1.2.8/text2story/annotators/NLTK/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2948 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/annotators/NLTK/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.950552 text2story-1.2.8/text2story/annotators/PY_HEIDELTIME/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2721 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/annotators/PY_HEIDELTIME/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.950552 text2story-1.2.8/text2story/annotators/SPACY/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     4362 2023-04-28 09:04:12.000000 text2story-1.2.8/text2story/annotators/SPACY/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.950552 text2story-1.2.8/text2story/annotators/SPARKNLP/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9462 2022-10-26 12:28:21.000000 text2story-1.2.8/text2story/annotators/SPARKNLP/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.950552 text2story-1.2.8/text2story/annotators/SRLWeakLabeling/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3501 2023-05-22 15:42:57.000000 text2story-1.2.8/text2story/annotators/SRLWeakLabeling/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2394 2023-05-18 09:14:04.000000 text2story-1.2.8/text2story/annotators/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.950552 text2story-1.2.8/text2story/brat2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      548 2022-10-19 09:12:42.000000 text2story-1.2.8/text2story/brat2viz/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-10-19 09:12:42.000000 text2story-1.2.8/text2story/brat2viz/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.950552 text2story-1.2.8/text2story/brat2viz/brat2drs/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       37 2022-10-19 09:12:42.000000 text2story-1.2.8/text2story/brat2viz/brat2drs/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17253 2022-10-19 09:12:42.000000 text2story-1.2.8/text2story/brat2viz/brat2drs/brat2drs.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1059 2022-10-19 09:12:42.000000 text2story-1.2.8/text2story/brat2viz/brat2drs/files_monitor.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.950552 text2story-1.2.8/text2story/brat2viz/drs2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-19 09:12:42.000000 text2story-1.2.8/text2story/brat2viz/drs2viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2428 2022-10-19 09:12:42.000000 text2story-1.2.8/text2story/brat2viz/drs2viz/app.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13487 2022-10-19 09:12:42.000000 text2story-1.2.8/text2story/brat2viz/drs2viz/parser.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     4564 2022-11-04 13:39:56.000000 text2story-1.2.8/text2story/brat2viz/drs2viz/viz.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.950552 text2story-1.2.8/text2story/core/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:48:21.000000 text2story-1.2.8/text2story/core/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    12126 2023-05-03 10:32:35.000000 text2story-1.2.8/text2story/core/annotator.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2667 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/core/entity_structures.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      505 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/core/exceptions.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      529 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/core/link_structures.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17906 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/core/narrative.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5281 2023-05-03 09:45:52.000000 text2story-1.2.8/text2story/core/utils.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.950552 text2story-1.2.8/text2story/experiments/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:04.000000 text2story-1.2.8/text2story/experiments/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16454 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/experiments/evaluation.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14458 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/experiments/metrics.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1192 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/experiments/run_experiments.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1618 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/experiments/stats.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.954553 text2story-1.2.8/text2story/readers/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-09 12:20:40.000000 text2story-1.2.8/text2story/readers/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      380 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/readers/fn-lirics.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   312656 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/readers/pb-vn2.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      547 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/readers/read.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    22674 2023-03-27 13:07:12.000000 text2story-1.2.8/text2story/readers/read_brat.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16999 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/readers/read_ecb.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6081 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/readers/read_framenet.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11525 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/readers/read_propbank.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1180 2023-03-27 13:07:12.000000 text2story-1.2.8/text2story/readers/token_corpus.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1221 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/readers/utils.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      353 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/readers/vn-lirics.json
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.954553 text2story-1.2.8/text2story/select/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      121 2023-03-27 13:07:12.000000 text2story-1.2.8/text2story/select/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:09.000000 text2story-1.2.8/text2story/select/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14728 2023-03-27 13:07:12.000000 text2story-1.2.8/text2story/select/bubble.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5159 2023-03-27 13:07:12.000000 text2story-1.2.8/text2story/select/event.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.954553 text2story-1.2.8/text2story/text2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5371 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/text2viz/Text2Viz.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/text2viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      699 2022-10-13 08:54:40.000000 text2story-1.2.8/text2story/text2viz/visualization.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.954553 text2story-1.2.8/text2story/training/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-03 11:20:54.000000 text2story-1.2.8/text2story/training/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14422 2023-05-22 12:41:48.000000 text2story-1.2.8/text2story/training/participant_concept.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.954553 text2story-1.2.8/text2story/viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:13.000000 text2story-1.2.8/text2story/viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14759 2023-03-31 13:18:54.000000 text2story-1.2.8/text2story/viz/bubble_tikz.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:21:08.946550 text2story-1.2.8/text2story.egg-info/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9774 2023-05-24 22:21:08.000000 text2story-1.2.8/text2story.egg-info/PKG-INFO
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2728 2023-05-24 22:21:08.000000 text2story-1.2.8/text2story.egg-info/SOURCES.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-24 22:21:08.000000 text2story-1.2.8/text2story.egg-info/dependency_links.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      228 2023-05-24 22:21:08.000000 text2story-1.2.8/text2story.egg-info/requires.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       11 2023-05-24 22:21:08.000000 text2story-1.2.8/text2story.egg-info/top_level.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-03-29 13:58:12.000000 text2story-1.2.8/text2story.egg-info/zip-safe
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.893532 text2story-1.2.9/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    33470 2022-10-19 09:22:59.000000 text2story-1.2.9/LICENSE
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      442 2023-03-29 14:01:55.000000 text2story-1.2.9/MANIFEST.in
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9774 2023-05-24 22:29:11.893532 text2story-1.2.9/PKG-INFO
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     8575 2023-05-17 10:11:38.000000 text2story-1.2.9/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      114 2023-03-29 13:58:48.000000 text2story-1.2.9/pyproject.toml
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1591 2023-05-24 22:29:11.893532 text2story-1.2.9/setup.cfg
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       70 2023-03-29 13:48:56.000000 text2story-1.2.9/setup.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.885532 text2story-1.2.9/text2story/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      757 2022-10-19 09:12:42.000000 text2story-1.2.9/text2story/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       67 2022-10-19 09:12:42.000000 text2story-1.2.9/text2story/__main__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.885532 text2story-1.2.9/text2story/annotators/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.885532 text2story-1.2.9/text2story/annotators/ALLENNLP/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.881533 text2story-1.2.9/text2story/annotators/ALLENNLP/Models/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.885532 text2story-1.2.9/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.885532 text2story-1.2.9/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      739 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       14 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/non_padded_namespaces.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1343 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   265058 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10386 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/ALLENNLP/PropBankBr.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    25595 2023-05-22 15:42:56.000000 text2story-1.2.9/text2story/annotators/ALLENNLP/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13691 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/ALLENNLP/my_model.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    20375 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/ALLENNLP/my_reader.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6217 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/ALLENNLP/preprocess.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.885532 text2story-1.2.9/text2story/annotators/CUSTOMPT/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14794 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/CUSTOMPT/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   371646 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/CUSTOMPT/crf_v2.1.joblib
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15093 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/CUSTOMPT/event_model.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13972 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/CUSTOMPT/feature_extractor.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.885532 text2story-1.2.9/text2story/annotators/NLTK/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2948 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/NLTK/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.889532 text2story-1.2.9/text2story/annotators/PY_HEIDELTIME/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2721 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/PY_HEIDELTIME/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.889532 text2story-1.2.9/text2story/annotators/SPACY/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     4362 2023-04-28 09:04:12.000000 text2story-1.2.9/text2story/annotators/SPACY/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.889532 text2story-1.2.9/text2story/annotators/SPARKNLP/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9462 2022-10-26 12:28:21.000000 text2story-1.2.9/text2story/annotators/SPARKNLP/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.889532 text2story-1.2.9/text2story/annotators/SRLWeakLabeling/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3501 2023-05-22 15:42:57.000000 text2story-1.2.9/text2story/annotators/SRLWeakLabeling/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2394 2023-05-18 09:14:04.000000 text2story-1.2.9/text2story/annotators/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.889532 text2story-1.2.9/text2story/brat2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      548 2022-10-19 09:12:42.000000 text2story-1.2.9/text2story/brat2viz/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-10-19 09:12:42.000000 text2story-1.2.9/text2story/brat2viz/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.889532 text2story-1.2.9/text2story/brat2viz/brat2drs/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       37 2022-10-19 09:12:42.000000 text2story-1.2.9/text2story/brat2viz/brat2drs/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17253 2022-10-19 09:12:42.000000 text2story-1.2.9/text2story/brat2viz/brat2drs/brat2drs.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1059 2022-10-19 09:12:42.000000 text2story-1.2.9/text2story/brat2viz/brat2drs/files_monitor.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.889532 text2story-1.2.9/text2story/brat2viz/drs2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-19 09:12:42.000000 text2story-1.2.9/text2story/brat2viz/drs2viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2428 2022-10-19 09:12:42.000000 text2story-1.2.9/text2story/brat2viz/drs2viz/app.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13487 2022-10-19 09:12:42.000000 text2story-1.2.9/text2story/brat2viz/drs2viz/parser.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     4564 2022-11-04 13:39:56.000000 text2story-1.2.9/text2story/brat2viz/drs2viz/viz.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.889532 text2story-1.2.9/text2story/core/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:48:21.000000 text2story-1.2.9/text2story/core/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    12126 2023-05-03 10:32:35.000000 text2story-1.2.9/text2story/core/annotator.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2667 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/core/entity_structures.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      505 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/core/exceptions.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      529 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/core/link_structures.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17906 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/core/narrative.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5281 2023-05-03 09:45:52.000000 text2story-1.2.9/text2story/core/utils.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.889532 text2story-1.2.9/text2story/experiments/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:04.000000 text2story-1.2.9/text2story/experiments/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16454 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/experiments/evaluation.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14458 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/experiments/metrics.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1192 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/experiments/run_experiments.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1618 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/experiments/stats.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.889532 text2story-1.2.9/text2story/readers/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-09 12:20:40.000000 text2story-1.2.9/text2story/readers/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      380 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/readers/fn-lirics.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   312656 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/readers/pb-vn2.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      547 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/readers/read.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    22674 2023-03-27 13:07:12.000000 text2story-1.2.9/text2story/readers/read_brat.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16999 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/readers/read_ecb.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6081 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/readers/read_framenet.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11525 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/readers/read_propbank.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1180 2023-03-27 13:07:12.000000 text2story-1.2.9/text2story/readers/token_corpus.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1221 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/readers/utils.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      353 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/readers/vn-lirics.json
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.893532 text2story-1.2.9/text2story/select/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      121 2023-03-27 13:07:12.000000 text2story-1.2.9/text2story/select/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:09.000000 text2story-1.2.9/text2story/select/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14728 2023-03-27 13:07:12.000000 text2story-1.2.9/text2story/select/bubble.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5159 2023-03-27 13:07:12.000000 text2story-1.2.9/text2story/select/event.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.893532 text2story-1.2.9/text2story/text2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5371 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/text2viz/Text2Viz.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/text2viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      699 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/text2viz/visualization.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.893532 text2story-1.2.9/text2story/training/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-03 11:20:54.000000 text2story-1.2.9/text2story/training/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14422 2023-05-22 12:41:48.000000 text2story-1.2.9/text2story/training/participant_concept.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.893532 text2story-1.2.9/text2story/viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:13.000000 text2story-1.2.9/text2story/viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14759 2023-03-31 13:18:54.000000 text2story-1.2.9/text2story/viz/bubble_tikz.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.885532 text2story-1.2.9/text2story.egg-info/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9774 2023-05-24 22:29:11.000000 text2story-1.2.9/text2story.egg-info/PKG-INFO
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2728 2023-05-24 22:29:11.000000 text2story-1.2.9/text2story.egg-info/SOURCES.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-24 22:29:11.000000 text2story-1.2.9/text2story.egg-info/dependency_links.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      238 2023-05-24 22:29:11.000000 text2story-1.2.9/text2story.egg-info/requires.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       11 2023-05-24 22:29:11.000000 text2story-1.2.9/text2story.egg-info/top_level.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-03-29 13:58:12.000000 text2story-1.2.9/text2story.egg-info/zip-safe
```

### Comparing `text2story-1.2.8/LICENSE` & `text2story-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/PKG-INFO` & `text2story-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2story
-Version: 1.2.8
+Version: 1.2.9
 Summary: It provides a framework to label a text according to the main elements of narrative (events, participants,time) and their relations
 Home-page: https://www.inesctec.pt/pt/centros/liaad
 Author: LIAAD lab
 License: GNU Public Licence
 Keywords: natural-language-processing,nlp,natural-language-understanding,deep-learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `text2story-1.2.8/README.md` & `text2story-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/setup.cfg` & `text2story-1.2.9/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = text2story
-version = 1.2.8
+version = 1.2.9
 author = LIAAD lab
 url = https://www.inesctec.pt/pt/centros/liaad
 description = It provides a framework to label a text according to the main elements of narrative (events, participants,time) and their relations
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = natural-language-processing, nlp, natural-language-understanding, deep-learning
 license = GNU Public Licence
@@ -34,16 +34,16 @@
 	numpy
 	pandas
 	nltk
 	overrides==3.1.0
 	cached-path==1.1.2
 	joblib
 	requests
-	allennlp
-	allennlp-models
+	allennlp>2.10
+	allennlp-models>2.10
 	spacy>=3.5.0,<3.6
 	pyspark
 	spark-nlp
 	elementpath
 	sklearn-crfsuite
 	plantuml
 	pdflatex
```

### Comparing `text2story-1.2.8/text2story/__init__.py` & `text2story-1.2.9/text2story/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt` & `text2story-1.2.9/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json` & `text2story-1.2.9/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt` & `text2story-1.2.9/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/annotators/ALLENNLP/PropBankBr.py` & `text2story-1.2.9/text2story/annotators/ALLENNLP/PropBankBr.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/annotators/ALLENNLP/__init__.py` & `text2story-1.2.9/text2story/annotators/ALLENNLP/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/annotators/ALLENNLP/my_model.py` & `text2story-1.2.9/text2story/annotators/ALLENNLP/my_model.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/annotators/ALLENNLP/my_reader.py` & `text2story-1.2.9/text2story/annotators/ALLENNLP/my_reader.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/annotators/ALLENNLP/preprocess.py` & `text2story-1.2.9/text2story/annotators/ALLENNLP/preprocess.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/annotators/CUSTOMPT/__init__.py` & `text2story-1.2.9/text2story/annotators/CUSTOMPT/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/annotators/CUSTOMPT/crf_v2.1.joblib` & `text2story-1.2.9/text2story/annotators/CUSTOMPT/crf_v2.1.joblib`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/annotators/CUSTOMPT/event_model.py` & `text2story-1.2.9/text2story/annotators/CUSTOMPT/event_model.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/annotators/CUSTOMPT/feature_extractor.py` & `text2story-1.2.9/text2story/annotators/CUSTOMPT/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/annotators/NLTK/__init__.py` & `text2story-1.2.9/text2story/annotators/NLTK/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/annotators/PY_HEIDELTIME/__init__.py` & `text2story-1.2.9/text2story/annotators/PY_HEIDELTIME/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/annotators/SPACY/__init__.py` & `text2story-1.2.9/text2story/annotators/SPACY/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/annotators/SPARKNLP/__init__.py` & `text2story-1.2.9/text2story/annotators/SPARKNLP/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/annotators/SRLWeakLabeling/__init__.py` & `text2story-1.2.9/text2story/annotators/SRLWeakLabeling/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/annotators/__init__.py` & `text2story-1.2.9/text2story/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/brat2viz/README.md` & `text2story-1.2.9/text2story/brat2viz/README.md`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/brat2viz/brat2drs/brat2drs.py` & `text2story-1.2.9/text2story/brat2viz/brat2drs/brat2drs.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/brat2viz/brat2drs/files_monitor.py` & `text2story-1.2.9/text2story/brat2viz/brat2drs/files_monitor.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/brat2viz/drs2viz/app.py` & `text2story-1.2.9/text2story/brat2viz/drs2viz/app.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/brat2viz/drs2viz/parser.py` & `text2story-1.2.9/text2story/brat2viz/drs2viz/parser.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/brat2viz/drs2viz/viz.py` & `text2story-1.2.9/text2story/brat2viz/drs2viz/viz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/core/annotator.py` & `text2story-1.2.9/text2story/core/annotator.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/core/entity_structures.py` & `text2story-1.2.9/text2story/core/entity_structures.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/core/link_structures.py` & `text2story-1.2.9/text2story/core/link_structures.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/core/narrative.py` & `text2story-1.2.9/text2story/core/narrative.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/core/utils.py` & `text2story-1.2.9/text2story/core/utils.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/experiments/evaluation.py` & `text2story-1.2.9/text2story/experiments/evaluation.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/experiments/metrics.py` & `text2story-1.2.9/text2story/experiments/metrics.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/experiments/run_experiments.py` & `text2story-1.2.9/text2story/experiments/run_experiments.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/experiments/stats.py` & `text2story-1.2.9/text2story/experiments/stats.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/readers/pb-vn2.json` & `text2story-1.2.9/text2story/readers/pb-vn2.json`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/readers/read.py` & `text2story-1.2.9/text2story/readers/read.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/readers/read_brat.py` & `text2story-1.2.9/text2story/readers/read_brat.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/readers/read_ecb.py` & `text2story-1.2.9/text2story/readers/read_ecb.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/readers/read_framenet.py` & `text2story-1.2.9/text2story/readers/read_framenet.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/readers/read_propbank.py` & `text2story-1.2.9/text2story/readers/read_propbank.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/readers/token_corpus.py` & `text2story-1.2.9/text2story/readers/token_corpus.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/readers/utils.py` & `text2story-1.2.9/text2story/readers/utils.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/select/bubble.py` & `text2story-1.2.9/text2story/select/bubble.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/select/event.py` & `text2story-1.2.9/text2story/select/event.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/text2viz/Text2Viz.py` & `text2story-1.2.9/text2story/text2viz/Text2Viz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/text2viz/visualization.py` & `text2story-1.2.9/text2story/text2viz/visualization.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/training/participant_concept.py` & `text2story-1.2.9/text2story/training/participant_concept.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story/viz/bubble_tikz.py` & `text2story-1.2.9/text2story/viz/bubble_tikz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.8/text2story.egg-info/PKG-INFO` & `text2story-1.2.9/text2story.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2story
-Version: 1.2.8
+Version: 1.2.9
 Summary: It provides a framework to label a text according to the main elements of narrative (events, participants,time) and their relations
 Home-page: https://www.inesctec.pt/pt/centros/liaad
 Author: LIAAD lab
 License: GNU Public Licence
 Keywords: natural-language-processing,nlp,natural-language-understanding,deep-learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `text2story-1.2.8/text2story.egg-info/SOURCES.txt` & `text2story-1.2.9/text2story.egg-info/SOURCES.txt`

 * *Files identical despite different names*

