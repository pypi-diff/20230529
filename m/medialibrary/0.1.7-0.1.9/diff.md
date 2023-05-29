# Comparing `tmp/medialibrary-0.1.7.tar.gz` & `tmp/medialibrary-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medialibrary-0.1.7.tar", last modified: Thu Mar 16 00:29:04 2023, max compression
+gzip compressed data, was "medialibrary-0.1.9.tar", last modified: Mon May 29 20:52:24 2023, max compression
```

## Comparing `medialibrary-0.1.7.tar` & `medialibrary-0.1.9.tar`

### file list

```diff
@@ -1,98 +1,104 @@
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.692143 medialibrary-0.1.7/
--rw-r--r--   0 chrisj     (102) other        (1)     1071 2021-09-05 20:32:22.000000 medialibrary-0.1.7/LICENSE
--rw-r--r--   0 chrisj     (102) other        (1)     2928 2023-03-16 00:29:04.692273 medialibrary-0.1.7/PKG-INFO
--rw-r--r--   0 chrisj     (102) other        (1)     2023 2022-11-30 03:32:25.000000 medialibrary-0.1.7/README.md
--rw-r--r--   0 chrisj     (102) other        (1)     1055 2023-03-16 00:28:34.000000 medialibrary-0.1.7/pyproject.toml
--rw-r--r--   0 chrisj     (102) other        (1)      150 2023-03-16 00:29:04.692876 medialibrary-0.1.7/setup.cfg
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.660419 medialibrary-0.1.7/src/
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.662339 medialibrary-0.1.7/src/media/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/__init__.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.663580 medialibrary-0.1.7/src/media/data/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/data/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     2182 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/data/dates.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.664441 medialibrary-0.1.7/src/media/data/media/
--rw-r--r--   0 chrisj     (102) other        (1)     1259 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/data/media/__init__.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.664877 medialibrary-0.1.7/src/media/data/media/contents/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/data/media/contents/__init__.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.666203 medialibrary-0.1.7/src/media/data/media/contents/generic/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/data/media/contents/generic/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     5671 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/data/media/contents/generic/catalog.py
--rw-r--r--   0 chrisj     (102) other        (1)     8487 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/data/media/contents/generic/keywords.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.667987 medialibrary-0.1.7/src/media/data/media/contents/genericv/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/data/media/contents/genericv/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)    13540 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/data/media/contents/genericv/crew.py
--rw-r--r--   0 chrisj     (102) other        (1)     2740 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/data/media/contents/genericv/story.py
--rw-r--r--   0 chrisj     (102) other        (1)     3332 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/data/media/contents/genericv/technical.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.669320 medialibrary-0.1.7/src/media/data/media/contents/movie/
--rw-r--r--   0 chrisj     (102) other        (1)     1171 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/data/media/contents/movie/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     3810 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/data/media/contents/movie/classification.py
--rw-r--r--   0 chrisj     (102) other        (1)     6101 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/data/media/contents/movie/internal.py
--rw-r--r--   0 chrisj     (102) other        (1)     3863 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/data/media/internal.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.671038 medialibrary-0.1.7/src/media/data/media/library/
--rw-r--r--   0 chrisj     (102) other        (1)     1259 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/data/media/library/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     1853 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/data/media/library/filing.py
--rw-r--r--   0 chrisj     (102) other        (1)     5007 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/data/media/library/instances.py
--rw-r--r--   0 chrisj     (102) other        (1)     2070 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/data/media/library/internal.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.673679 medialibrary-0.1.7/src/media/data/media/medium/
--rw-r--r--   0 chrisj     (102) other        (1)     1259 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/data/media/medium/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     2498 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/data/media/medium/internal.py
--rw-r--r--   0 chrisj     (102) other        (1)     8439 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/data/media/medium/inventory.py
--rw-r--r--   0 chrisj     (102) other        (1)     3590 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/data/media/medium/productid.py
--rw-r--r--   0 chrisj     (102) other        (1)     4650 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/data/media/medium/productspecs.py
--rw-r--r--   0 chrisj     (102) other        (1)     3318 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/data/media/medium/release.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.674545 medialibrary-0.1.7/src/media/data/media/meta/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/data/media/meta/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)    12864 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/data/media/meta/authorship.py
--rw-r--r--   0 chrisj     (102) other        (1)     9135 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/data/nouns.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.676627 medialibrary-0.1.7/src/media/fileops/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/fileops/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     1564 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/fileops/filenames.py
--rw-r--r--   0 chrisj     (102) other        (1)     2013 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/fileops/loader.py
--rw-r--r--   0 chrisj     (102) other        (1)     3282 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/fileops/repo.py
--rw-r--r--   0 chrisj     (102) other        (1)     3132 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/fileops/scanner.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.677060 medialibrary-0.1.7/src/media/fmt/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/fmt/__init__.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.678769 medialibrary-0.1.7/src/media/fmt/text/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/fmt/text/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     4058 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/fmt/text/basics.py
--rw-r--r--   0 chrisj     (102) other        (1)     8180 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/fmt/text/media.py
--rw-r--r--   0 chrisj     (102) other        (1)     8922 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/fmt/text/movie.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.679627 medialibrary-0.1.7/src/media/generic/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/generic/__init__.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.680910 medialibrary-0.1.7/src/media/generic/sorting/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/generic/sorting/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     5470 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/generic/sorting/groups.py
--rw-r--r--   0 chrisj     (102) other        (1)     4307 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/generic/sorting/lists.py
--rw-r--r--   0 chrisj     (102) other        (1)     2351 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/generic/stringtools.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.681738 medialibrary-0.1.7/src/media/tools/
--rw-r--r--   0 chrisj     (102) other        (1)     1145 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/tools/__init__.py
--rwxr-xr-x   0 chrisj     (102) other        (1)     2321 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/tools/common.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.683414 medialibrary-0.1.7/src/media/tools/media/
--rw-r--r--   0 chrisj     (102) other        (1)     1150 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/tools/media/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     2645 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/tools/media/authorrecords.py
--rw-r--r--   0 chrisj     (102) other        (1)     2414 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/tools/media/list.py
--rw-r--r--   0 chrisj     (102) other        (1)     2371 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/tools/media/show.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.684259 medialibrary-0.1.7/src/media/tools/meta/
--rw-r--r--   0 chrisj     (102) other        (1)     1149 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/tools/meta/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     2291 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/tools/meta/authorship.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.688527 medialibrary-0.1.7/src/media/tools/movies/
--rw-r--r--   0 chrisj     (102) other        (1)     1151 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/tools/movies/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     8007 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/tools/movies/castlist.py
--rw-r--r--   0 chrisj     (102) other        (1)     3096 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/tools/movies/debuglist.py
--rw-r--r--   0 chrisj     (102) other        (1)     9675 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/tools/movies/genrebreakdown.py
--rw-r--r--   0 chrisj     (102) other        (1)     4211 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/tools/movies/keywordlist.py
--rw-r--r--   0 chrisj     (102) other        (1)     3808 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/tools/movies/list.py
--rw-r--r--   0 chrisj     (102) other        (1)     5747 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/tools/movies/namelist.py
--rwxr-xr-x   0 chrisj     (102) other        (1)     3431 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/tools/movies/show.py
--rwxr-xr-x   0 chrisj     (102) other        (1)     8719 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/tools/movies/timebuckets.py
--rw-r--r--   0 chrisj     (102) other        (1)     6440 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/tools/movies/validate.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.690185 medialibrary-0.1.7/src/media/xml/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/xml/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     1546 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/xml/functions.py
--rw-r--r--   0 chrisj     (102) other        (1)     1751 2023-03-16 00:27:27.000000 medialibrary-0.1.7/src/media/xml/namespaces.py
--rw-r--r--   0 chrisj     (102) other        (1)     2365 2022-11-30 03:32:25.000000 medialibrary-0.1.7/src/media/xml/parser.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-03-16 00:29:04.691852 medialibrary-0.1.7/src/medialibrary.egg-info/
--rw-r--r--   0 chrisj     (102) other        (1)     2928 2023-03-16 00:29:04.000000 medialibrary-0.1.7/src/medialibrary.egg-info/PKG-INFO
--rw-r--r--   0 chrisj     (102) other        (1)     2563 2023-03-16 00:29:04.000000 medialibrary-0.1.7/src/medialibrary.egg-info/SOURCES.txt
--rw-r--r--   0 chrisj     (102) other        (1)        1 2023-03-16 00:29:04.000000 medialibrary-0.1.7/src/medialibrary.egg-info/dependency_links.txt
--rw-r--r--   0 chrisj     (102) other        (1)        6 2023-03-16 00:29:04.000000 medialibrary-0.1.7/src/medialibrary.egg-info/top_level.txt
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.249885 medialibrary-0.1.9/
+-rw-r--r--   0 chrisj     (102) other        (1)     1071 2021-09-05 20:32:22.000000 medialibrary-0.1.9/LICENSE
+-rw-r--r--   0 chrisj     (102) other        (1)     2928 2023-05-29 20:52:24.250006 medialibrary-0.1.9/PKG-INFO
+-rw-r--r--   0 chrisj     (102) other        (1)     2023 2022-11-30 03:32:25.000000 medialibrary-0.1.9/README.md
+-rw-r--r--   0 chrisj     (102) other        (1)     1055 2023-05-29 20:51:38.000000 medialibrary-0.1.9/pyproject.toml
+-rw-r--r--   0 chrisj     (102) other        (1)      150 2023-05-29 20:52:24.250601 medialibrary-0.1.9/setup.cfg
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.217640 medialibrary-0.1.9/src/
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.219385 medialibrary-0.1.9/src/media/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/__init__.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.220546 medialibrary-0.1.9/src/media/data/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/data/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2182 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/data/dates.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.221324 medialibrary-0.1.9/src/media/data/media/
+-rw-r--r--   0 chrisj     (102) other        (1)     1259 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/data/media/__init__.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.221741 medialibrary-0.1.9/src/media/data/media/contents/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/data/media/contents/__init__.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.223036 medialibrary-0.1.9/src/media/data/media/contents/generic/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/data/media/contents/generic/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     5671 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/data/media/contents/generic/catalog.py
+-rw-r--r--   0 chrisj     (102) other        (1)     8487 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/data/media/contents/generic/keywords.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.224395 medialibrary-0.1.9/src/media/data/media/contents/generic/story/
+-rw-r--r--   0 chrisj     (102) other        (1)     1172 2023-05-29 20:51:00.000000 medialibrary-0.1.9/src/media/data/media/contents/generic/story/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     4319 2023-05-29 20:51:00.000000 medialibrary-0.1.9/src/media/data/media/contents/generic/story/characters.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2774 2023-05-29 20:51:00.000000 medialibrary-0.1.9/src/media/data/media/contents/generic/story/internal.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.225258 medialibrary-0.1.9/src/media/data/media/contents/genericv/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/data/media/contents/genericv/__init__.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.226639 medialibrary-0.1.9/src/media/data/media/contents/genericv/crew/
+-rw-r--r--   0 chrisj     (102) other        (1)     1198 2023-05-29 20:51:00.000000 medialibrary-0.1.9/src/media/data/media/contents/genericv/crew/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     8627 2023-05-29 20:51:00.000000 medialibrary-0.1.9/src/media/data/media/contents/genericv/crew/cast.py
+-rw-r--r--   0 chrisj     (102) other        (1)     5667 2023-05-29 20:51:00.000000 medialibrary-0.1.9/src/media/data/media/contents/genericv/crew/internal.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3332 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/data/media/contents/genericv/technical.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.227961 medialibrary-0.1.9/src/media/data/media/contents/movie/
+-rw-r--r--   0 chrisj     (102) other        (1)     1171 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/data/media/contents/movie/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3810 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/data/media/contents/movie/classification.py
+-rw-r--r--   0 chrisj     (102) other        (1)     6100 2023-05-29 20:51:00.000000 medialibrary-0.1.9/src/media/data/media/contents/movie/internal.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3863 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/data/media/internal.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.229647 medialibrary-0.1.9/src/media/data/media/library/
+-rw-r--r--   0 chrisj     (102) other        (1)     1259 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/data/media/library/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     1853 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/data/media/library/filing.py
+-rw-r--r--   0 chrisj     (102) other        (1)     5007 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/data/media/library/instances.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2070 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/data/media/library/internal.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.232149 medialibrary-0.1.9/src/media/data/media/medium/
+-rw-r--r--   0 chrisj     (102) other        (1)     1259 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/data/media/medium/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2498 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/data/media/medium/internal.py
+-rw-r--r--   0 chrisj     (102) other        (1)     8439 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/data/media/medium/inventory.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3590 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/data/media/medium/productid.py
+-rw-r--r--   0 chrisj     (102) other        (1)     4650 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/data/media/medium/productspecs.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3318 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/data/media/medium/release.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.232963 medialibrary-0.1.9/src/media/data/media/meta/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/data/media/meta/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)    12864 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/data/media/meta/authorship.py
+-rw-r--r--   0 chrisj     (102) other        (1)     9141 2023-05-29 20:51:00.000000 medialibrary-0.1.9/src/media/data/nouns.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.234964 medialibrary-0.1.9/src/media/fileops/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/fileops/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     1564 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/fileops/filenames.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2013 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/fileops/loader.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3282 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/fileops/repo.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3132 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/fileops/scanner.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.235360 medialibrary-0.1.9/src/media/fmt/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/fmt/__init__.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.237075 medialibrary-0.1.9/src/media/fmt/text/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/fmt/text/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     4058 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/fmt/text/basics.py
+-rw-r--r--   0 chrisj     (102) other        (1)     8180 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/fmt/text/media.py
+-rw-r--r--   0 chrisj     (102) other        (1)     8922 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/fmt/text/movie.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.237888 medialibrary-0.1.9/src/media/generic/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/generic/__init__.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.239114 medialibrary-0.1.9/src/media/generic/sorting/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/generic/sorting/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     5470 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/generic/sorting/groups.py
+-rw-r--r--   0 chrisj     (102) other        (1)     4307 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/generic/sorting/lists.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2351 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/generic/stringtools.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.239901 medialibrary-0.1.9/src/media/tools/
+-rw-r--r--   0 chrisj     (102) other        (1)     1145 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/tools/__init__.py
+-rwxr-xr-x   0 chrisj     (102) other        (1)     2321 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/tools/common.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.241569 medialibrary-0.1.9/src/media/tools/media/
+-rw-r--r--   0 chrisj     (102) other        (1)     1150 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/tools/media/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2645 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/tools/media/authorrecords.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2414 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/tools/media/list.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2371 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/tools/media/show.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.242380 medialibrary-0.1.9/src/media/tools/meta/
+-rw-r--r--   0 chrisj     (102) other        (1)     1149 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/tools/meta/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2291 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/tools/meta/authorship.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.246482 medialibrary-0.1.9/src/media/tools/movies/
+-rw-r--r--   0 chrisj     (102) other        (1)     1151 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/tools/movies/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     8007 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/tools/movies/castlist.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3096 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/tools/movies/debuglist.py
+-rw-r--r--   0 chrisj     (102) other        (1)     9675 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/tools/movies/genrebreakdown.py
+-rw-r--r--   0 chrisj     (102) other        (1)     4211 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/tools/movies/keywordlist.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3808 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/tools/movies/list.py
+-rw-r--r--   0 chrisj     (102) other        (1)     5747 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/tools/movies/namelist.py
+-rwxr-xr-x   0 chrisj     (102) other        (1)     3431 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/tools/movies/show.py
+-rwxr-xr-x   0 chrisj     (102) other        (1)     8719 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/tools/movies/timebuckets.py
+-rw-r--r--   0 chrisj     (102) other        (1)     6440 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/tools/movies/validate.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.248105 medialibrary-0.1.9/src/media/xml/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/xml/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     1546 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/xml/functions.py
+-rw-r--r--   0 chrisj     (102) other        (1)     1751 2023-03-16 00:41:46.000000 medialibrary-0.1.9/src/media/xml/namespaces.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2365 2022-11-30 03:32:25.000000 medialibrary-0.1.9/src/media/xml/parser.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2023-05-29 20:52:24.249619 medialibrary-0.1.9/src/medialibrary.egg-info/
+-rw-r--r--   0 chrisj     (102) other        (1)     2928 2023-05-29 20:52:24.000000 medialibrary-0.1.9/src/medialibrary.egg-info/PKG-INFO
+-rw-r--r--   0 chrisj     (102) other        (1)     2802 2023-05-29 20:52:24.000000 medialibrary-0.1.9/src/medialibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 chrisj     (102) other        (1)        1 2023-05-29 20:52:24.000000 medialibrary-0.1.9/src/medialibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 chrisj     (102) other        (1)        6 2023-05-29 20:52:24.000000 medialibrary-0.1.9/src/medialibrary.egg-info/top_level.txt
```

### Comparing `medialibrary-0.1.7/LICENSE` & `medialibrary-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/PKG-INFO` & `medialibrary-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medialibrary
-Version: 0.1.7
+Version: 0.1.9
 Summary: Library for reading vtmedia XML files
 Author-email: Chris J <cjcodeproj@fastmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/cjcodeproj/medialibrary
 Project-URL: bug tracker, https://github.com/cjcodeproj/medialibrary/issues
 Project-URL: repository, https://github.com/cjcodeproj/medialibrary
 Project-URL: changelog, https://github.com/cjcodeproj/medialibrary/blob/main/CHANGELOG.md
```

### Comparing `medialibrary-0.1.7/README.md` & `medialibrary-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/pyproject.toml` & `medialibrary-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "medialibrary"
-version = "0.1.7"
+version = "0.1.9"
 description = "Library for reading vtmedia XML files"
 readme = "README.md"
 requires-python = ">3.8"
 license = {text = "MIT License"}
 keywords = ["xml", "movies", "dvds"]
 authors = [
   {email = "cjcodeproj@fastmail.com", name = "Chris J"}
```

### Comparing `medialibrary-0.1.7/src/media/__init__.py` & `medialibrary-0.1.9/src/media/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/__init__.py` & `medialibrary-0.1.9/src/media/data/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/dates.py` & `medialibrary-0.1.9/src/media/data/dates.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/media/__init__.py` & `medialibrary-0.1.9/src/media/data/media/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/media/contents/__init__.py` & `medialibrary-0.1.9/src/media/data/media/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/media/contents/generic/__init__.py` & `medialibrary-0.1.9/src/media/data/media/contents/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/media/contents/generic/catalog.py` & `medialibrary-0.1.9/src/media/data/media/contents/generic/catalog.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/media/contents/generic/keywords.py` & `medialibrary-0.1.9/src/media/data/media/contents/generic/keywords.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/media/contents/genericv/__init__.py` & `medialibrary-0.1.9/src/media/data/media/contents/genericv/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/media/contents/genericv/story.py` & `medialibrary-0.1.9/src/media/data/media/contents/generic/story/internal.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 
 #
-# Copyright 2022 Chris Josephes
+# Copyright 2023 Chris Josephes
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -19,16 +19,16 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 '''
-Object classes related to the plot of a piece of
-visual media.
+Object classes related to the story/plot
+of a given piece of media.
 '''
 
 # pylint: disable=too-few-public-methods
 
 import re
 from media.xml.namespaces import Namespaces
 from media.data.media.contents.generic.keywords import Keywords
@@ -38,14 +38,15 @@
     '''
     The story is the main narrative of the film or other media.
     '''
     def __init__(self, in_element):
         self.plot = None
         self.keywords = None
         self.themes = []
+        self.characters = []
         self._process(in_element)
 
     def _process(self, in_element):
         for child in in_element:
             tagname = Namespaces.ns_strip(child.tag)
             if tagname == 'plot':
                 self.plot = Plot(child)
```

### Comparing `medialibrary-0.1.7/src/media/data/media/contents/genericv/technical.py` & `medialibrary-0.1.9/src/media/data/media/contents/genericv/technical.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/media/contents/movie/__init__.py` & `medialibrary-0.1.9/src/media/data/media/contents/movie/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/media/contents/movie/classification.py` & `medialibrary-0.1.9/src/media/data/media/contents/movie/classification.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/media/contents/movie/internal.py` & `medialibrary-0.1.9/src/media/data/media/contents/movie/internal.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # pylint: disable=too-many-instance-attributes
 
 from datetime import timedelta
 from media.xml.namespaces import Namespaces
 from media.data.media.contents.generic.catalog import (
         Title, TitleValueException, Catalog
         )
-from media.data.media.contents.genericv.story import Story
+from media.data.media.contents.generic.story import Story
 from media.data.media.contents.genericv.crew import Crew
 from media.data.media.contents.genericv.technical import Technical
 from media.data.media.contents.movie.classification import Classification
 from media.generic.sorting.lists import ContentIndex
 
 
 class Movie():
```

### Comparing `medialibrary-0.1.7/src/media/data/media/internal.py` & `medialibrary-0.1.9/src/media/data/media/internal.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/media/library/__init__.py` & `medialibrary-0.1.9/src/media/data/media/library/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/media/library/filing.py` & `medialibrary-0.1.9/src/media/data/media/library/filing.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/media/library/instances.py` & `medialibrary-0.1.9/src/media/data/media/library/instances.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/media/library/internal.py` & `medialibrary-0.1.9/src/media/data/media/library/internal.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/media/medium/__init__.py` & `medialibrary-0.1.9/src/media/data/media/medium/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/media/medium/internal.py` & `medialibrary-0.1.9/src/media/data/media/medium/internal.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/media/medium/inventory.py` & `medialibrary-0.1.9/src/media/data/media/medium/inventory.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/media/medium/productid.py` & `medialibrary-0.1.9/src/media/data/media/medium/productid.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/media/medium/productspecs.py` & `medialibrary-0.1.9/src/media/data/media/medium/productspecs.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/media/medium/release.py` & `medialibrary-0.1.9/src/media/data/media/medium/release.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/media/meta/__init__.py` & `medialibrary-0.1.9/src/media/data/media/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/media/meta/authorship.py` & `medialibrary-0.1.9/src/media/data/media/meta/authorship.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/data/nouns.py` & `medialibrary-0.1.9/src/media/data/nouns.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
         raw = ''
         if self.pref_complete:
             raw = self.pref_complete
         else:
             if self.prefix:
                 raw += self.prefix + ' '
             if self.pref_given:
-                raw += self.pref_given
+                raw += self.pref_given + ' '
             else:
                 if self.given:
                     raw += self.given + ' '
                 if self.middle:
                     raw += self.middle + ' '
             if self.family:
                 raw += self.family
```

### Comparing `medialibrary-0.1.7/src/media/fileops/__init__.py` & `medialibrary-0.1.9/src/media/fileops/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/fileops/filenames.py` & `medialibrary-0.1.9/src/media/fileops/filenames.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/fileops/loader.py` & `medialibrary-0.1.9/src/media/fileops/loader.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/fileops/repo.py` & `medialibrary-0.1.9/src/media/fileops/repo.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/fileops/scanner.py` & `medialibrary-0.1.9/src/media/fileops/scanner.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/fmt/__init__.py` & `medialibrary-0.1.9/src/media/fmt/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/fmt/text/__init__.py` & `medialibrary-0.1.9/src/media/fmt/text/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/fmt/text/basics.py` & `medialibrary-0.1.9/src/media/fmt/text/basics.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/fmt/text/media.py` & `medialibrary-0.1.9/src/media/fmt/text/media.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/fmt/text/movie.py` & `medialibrary-0.1.9/src/media/fmt/text/movie.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/generic/__init__.py` & `medialibrary-0.1.9/src/media/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/generic/sorting/__init__.py` & `medialibrary-0.1.9/src/media/generic/sorting/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/generic/sorting/groups.py` & `medialibrary-0.1.9/src/media/generic/sorting/groups.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/generic/sorting/lists.py` & `medialibrary-0.1.9/src/media/generic/sorting/lists.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/generic/stringtools.py` & `medialibrary-0.1.9/src/media/generic/stringtools.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/tools/__init__.py` & `medialibrary-0.1.9/src/media/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/tools/common.py` & `medialibrary-0.1.9/src/media/tools/common.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/tools/media/__init__.py` & `medialibrary-0.1.9/src/media/tools/media/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/tools/media/authorrecords.py` & `medialibrary-0.1.9/src/media/tools/media/authorrecords.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/tools/media/list.py` & `medialibrary-0.1.9/src/media/tools/media/list.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/tools/media/show.py` & `medialibrary-0.1.9/src/media/tools/media/show.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/tools/meta/__init__.py` & `medialibrary-0.1.9/src/media/tools/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/tools/meta/authorship.py` & `medialibrary-0.1.9/src/media/tools/meta/authorship.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/tools/movies/__init__.py` & `medialibrary-0.1.9/src/media/tools/movies/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/tools/movies/castlist.py` & `medialibrary-0.1.9/src/media/tools/movies/castlist.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/tools/movies/debuglist.py` & `medialibrary-0.1.9/src/media/tools/movies/debuglist.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/tools/movies/genrebreakdown.py` & `medialibrary-0.1.9/src/media/tools/movies/genrebreakdown.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/tools/movies/keywordlist.py` & `medialibrary-0.1.9/src/media/tools/movies/keywordlist.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/tools/movies/list.py` & `medialibrary-0.1.9/src/media/tools/movies/list.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/tools/movies/namelist.py` & `medialibrary-0.1.9/src/media/tools/movies/namelist.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/tools/movies/show.py` & `medialibrary-0.1.9/src/media/tools/movies/show.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/tools/movies/timebuckets.py` & `medialibrary-0.1.9/src/media/tools/movies/timebuckets.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/tools/movies/validate.py` & `medialibrary-0.1.9/src/media/tools/movies/validate.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/xml/__init__.py` & `medialibrary-0.1.9/src/media/xml/__init__.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/xml/functions.py` & `medialibrary-0.1.9/src/media/xml/functions.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/xml/namespaces.py` & `medialibrary-0.1.9/src/media/xml/namespaces.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/media/xml/parser.py` & `medialibrary-0.1.9/src/media/xml/parser.py`

 * *Files identical despite different names*

### Comparing `medialibrary-0.1.7/src/medialibrary.egg-info/PKG-INFO` & `medialibrary-0.1.9/src/medialibrary.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medialibrary
-Version: 0.1.7
+Version: 0.1.9
 Summary: Library for reading vtmedia XML files
 Author-email: Chris J <cjcodeproj@fastmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/cjcodeproj/medialibrary
 Project-URL: bug tracker, https://github.com/cjcodeproj/medialibrary/issues
 Project-URL: repository, https://github.com/cjcodeproj/medialibrary
 Project-URL: changelog, https://github.com/cjcodeproj/medialibrary/blob/main/CHANGELOG.md
```

### Comparing `medialibrary-0.1.7/src/medialibrary.egg-info/SOURCES.txt` & `medialibrary-0.1.9/src/medialibrary.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,18 +8,22 @@
 src/media/data/nouns.py
 src/media/data/media/__init__.py
 src/media/data/media/internal.py
 src/media/data/media/contents/__init__.py
 src/media/data/media/contents/generic/__init__.py
 src/media/data/media/contents/generic/catalog.py
 src/media/data/media/contents/generic/keywords.py
+src/media/data/media/contents/generic/story/__init__.py
+src/media/data/media/contents/generic/story/characters.py
+src/media/data/media/contents/generic/story/internal.py
 src/media/data/media/contents/genericv/__init__.py
-src/media/data/media/contents/genericv/crew.py
-src/media/data/media/contents/genericv/story.py
 src/media/data/media/contents/genericv/technical.py
+src/media/data/media/contents/genericv/crew/__init__.py
+src/media/data/media/contents/genericv/crew/cast.py
+src/media/data/media/contents/genericv/crew/internal.py
 src/media/data/media/contents/movie/__init__.py
 src/media/data/media/contents/movie/classification.py
 src/media/data/media/contents/movie/internal.py
 src/media/data/media/library/__init__.py
 src/media/data/media/library/filing.py
 src/media/data/media/library/instances.py
 src/media/data/media/library/internal.py
```

