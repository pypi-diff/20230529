# Comparing `tmp/intake-parquet-0.2.3.tar.gz` & `tmp/intake-parquet-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/intake-parquet-0.2.3.tar", last modified: Mon Nov 11 20:20:23 2019, max compression
+gzip compressed data, was "intake-parquet-0.3.0.tar", last modified: Mon May 29 20:02:21 2023, max compression
```

## Comparing `intake-parquet-0.2.3.tar` & `intake-parquet-0.3.0.tar`

### file list

```diff
@@ -1,115 +1,97 @@
-drwxr-xr-x   0 mdurant    (501) staff       (20)        0 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/
--rw-r--r--   0 mdurant    (501) staff       (20)     1552 2019-05-23 18:19:30.000000 intake-parquet-0.2.3/.travis.yml
--rw-r--r--   0 mdurant    (501) staff       (20)     1330 2018-01-05 15:44:00.000000 intake-parquet-0.2.3/LICENSE
--rw-r--r--   0 mdurant    (501) staff       (20)      282 2018-12-03 16:37:39.000000 intake-parquet-0.2.3/MANIFEST.in
--rw-r--r--   0 mdurant    (501) staff       (20)     2013 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/PKG-INFO
--rw-r--r--   0 mdurant    (501) staff       (20)     1456 2019-01-17 18:30:21.000000 intake-parquet-0.2.3/README.md
-drwxr-xr-x   0 mdurant    (501) staff       (20)        0 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/conda/
--rw-r--r--   0 mdurant    (501) staff       (20)      676 2018-12-03 16:40:19.000000 intake-parquet-0.2.3/conda/meta.yaml
-drwxr-xr-x   0 mdurant    (501) staff       (20)        0 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/docs/
-drwxr-xr-x   0 mdurant    (501) staff       (20)        0 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/docs/build/
-drwxr-xr-x   0 mdurant    (501) staff       (20)        0 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/docs/build/html/
-drwxr-xr-x   0 mdurant    (501) staff       (20)        0 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/docs/build/html/_modules/
--rw-r--r--   0 mdurant    (501) staff       (20)     4519 2018-08-24 19:46:35.000000 intake-parquet-0.2.3/docs/build/html/_modules/index.html
-drwxr-xr-x   0 mdurant    (501) staff       (20)        0 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/docs/build/html/_modules/intake_parquet/
--rw-r--r--   0 mdurant    (501) staff       (20)    29229 2018-02-20 17:34:29.000000 intake-parquet-0.2.3/docs/build/html/_modules/intake_parquet/__init__.html
--rw-r--r--   0 mdurant    (501) staff       (20)    29302 2018-08-24 19:46:35.000000 intake-parquet-0.2.3/docs/build/html/_modules/intake_parquet/source.html
--rw-r--r--   0 mdurant    (501) staff       (20)     8463 2018-08-24 19:46:35.000000 intake-parquet-0.2.3/docs/build/html/_modules/intake_parquet.html
--rw-r--r--   0 mdurant    (501) staff       (20)    11236 2018-08-24 19:45:45.000000 intake-parquet-0.2.3/docs/build/html/api.html
--rw-r--r--   0 mdurant    (501) staff       (20)     5295 2018-08-24 19:46:35.000000 intake-parquet-0.2.3/docs/build/html/genindex.html
--rw-r--r--   0 mdurant    (501) staff       (20)     6059 2018-08-24 19:46:35.000000 intake-parquet-0.2.3/docs/build/html/index.html
--rw-r--r--   0 mdurant    (501) staff       (20)    14547 2018-08-24 19:46:35.000000 intake-parquet-0.2.3/docs/build/html/quickstart.html
--rw-r--r--   0 mdurant    (501) staff       (20)     4694 2018-08-24 19:46:35.000000 intake-parquet-0.2.3/docs/build/html/search.html
--rw-r--r--   0 mdurant    (501) staff       (20)      166 2018-04-17 13:35:18.000000 intake-parquet-0.2.3/docs/environment.yml
-drwxr-xr-x   0 mdurant    (501) staff       (20)        0 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/examples/
--rw-r--r--   0 mdurant    (501) staff       (20)      184 2018-04-16 17:35:13.000000 intake-parquet-0.2.3/examples/sample.yml
-drwxr-xr-x   0 mdurant    (501) staff       (20)        0 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/examples/test.parq/
--rw-r--r--   0 mdurant    (501) staff       (20)     2179 2018-01-07 22:02:06.000000 intake-parquet-0.2.3/examples/test.parq/_metadata
--rw-r--r--   0 mdurant    (501) staff       (20)    41809 2018-01-07 22:02:06.000000 intake-parquet-0.2.3/examples/test.parq/part.0.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)    41809 2018-01-07 22:02:06.000000 intake-parquet-0.2.3/examples/test.parq/part.1.parquet
-drwxr-xr-x   0 mdurant    (501) staff       (20)        0 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/intake_parquet/
--rw-r--r--   0 mdurant    (501) staff       (20)      156 2019-11-11 20:19:13.000000 intake-parquet-0.2.3/intake_parquet/__init__.py
--rw-r--r--   0 mdurant    (501) staff       (20)      497 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/intake_parquet/_version.py
--rw-r--r--   0 mdurant    (501) staff       (20)     3791 2019-11-11 19:48:52.000000 intake-parquet-0.2.3/intake_parquet/source.py
-drwxr-xr-x   0 mdurant    (501) staff       (20)        0 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/intake_parquet.egg-info/
--rw-r--r--   0 mdurant    (501) staff       (20)     2013 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/intake_parquet.egg-info/PKG-INFO
--rw-r--r--   0 mdurant    (501) staff       (20)     5710 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/intake_parquet.egg-info/SOURCES.txt
--rw-r--r--   0 mdurant    (501) staff       (20)        1 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/intake_parquet.egg-info/dependency_links.txt
--rw-r--r--   0 mdurant    (501) staff       (20)       64 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/intake_parquet.egg-info/entry_points.txt
--rw-r--r--   0 mdurant    (501) staff       (20)        1 2018-03-15 17:46:26.000000 intake-parquet-0.2.3/intake_parquet.egg-info/not-zip-safe
--rw-r--r--   0 mdurant    (501) staff       (20)       46 2018-12-03 16:38:13.000000 intake-parquet-0.2.3/intake_parquet.egg-info/pbr.json
--rw-r--r--   0 mdurant    (501) staff       (20)       39 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/intake_parquet.egg-info/requires.txt
--rw-r--r--   0 mdurant    (501) staff       (20)       21 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/intake_parquet.egg-info/top_level.txt
--rw-r--r--   0 mdurant    (501) staff       (20)       38 2018-04-16 15:17:00.000000 intake-parquet-0.2.3/readthedocs.yml
--rw-r--r--   0 mdurant    (501) staff       (20)       39 2018-11-20 21:02:36.000000 intake-parquet-0.2.3/requirements.txt
--rw-r--r--   0 mdurant    (501) staff       (20)      186 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/setup.cfg
--rw-r--r--   0 mdurant    (501) staff       (20)      775 2019-07-26 21:27:37.000000 intake-parquet-0.2.3/setup.py
-drwxr-xr-x   0 mdurant    (501) staff       (20)        0 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/tests/
--rw-r--r--   0 mdurant    (501) staff       (20)        0 2018-01-05 15:44:00.000000 intake-parquet-0.2.3/tests/__init__.py
--rw-r--r--   0 mdurant    (501) staff       (20)      200 2019-11-11 20:11:10.000000 intake-parquet-0.2.3/tests/cache_cat.yaml
-drwxr-xr-x   0 mdurant    (501) staff       (20)        0 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/tests/split/
--rw-r--r--   0 mdurant    (501) staff       (20)     7051 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/_metadata
-drwxr-xr-x   0 mdurant    (501) staff       (20)        0 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/tests/split/cat=fred/
-drwxr-xr-x   0 mdurant    (501) staff       (20)        0 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=1/
--rw-r--r--   0 mdurant    (501) staff       (20)      434 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=1/part-r-00000-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      438 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=1/part-r-00001-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      439 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=1/part-r-00002-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      439 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=1/part-r-00003-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      441 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=1/part-r-00004-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      439 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=1/part-r-00005-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      438 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=1/part-r-00006-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      441 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=1/part-r-00007-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
-drwxr-xr-x   0 mdurant    (501) staff       (20)        0 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=2/
--rw-r--r--   0 mdurant    (501) staff       (20)      436 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=2/part-r-00000-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      435 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=2/part-r-00001-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      440 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=2/part-r-00002-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      439 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=2/part-r-00003-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      439 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=2/part-r-00004-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      442 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=2/part-r-00005-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      440 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=2/part-r-00006-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      438 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=2/part-r-00007-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
-drwxr-xr-x   0 mdurant    (501) staff       (20)        0 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=3/
--rw-r--r--   0 mdurant    (501) staff       (20)      437 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=3/part-r-00000-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      437 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=3/part-r-00001-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      438 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=3/part-r-00002-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      440 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=3/part-r-00003-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      439 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=3/part-r-00004-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      439 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=3/part-r-00005-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      442 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=3/part-r-00006-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      441 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=fred/catnum=3/part-r-00007-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
-drwxr-xr-x   0 mdurant    (501) staff       (20)        0 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/tests/split/cat=freda/
-drwxr-xr-x   0 mdurant    (501) staff       (20)        0 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=1/
--rw-r--r--   0 mdurant    (501) staff       (20)      438 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=1/part-r-00000-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      438 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=1/part-r-00001-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      439 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=1/part-r-00002-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      442 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=1/part-r-00003-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      439 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=1/part-r-00004-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      441 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=1/part-r-00005-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      443 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=1/part-r-00006-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      440 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=1/part-r-00007-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
-drwxr-xr-x   0 mdurant    (501) staff       (20)        0 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=2/
--rw-r--r--   0 mdurant    (501) staff       (20)      436 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=2/part-r-00000-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      440 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=2/part-r-00001-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      439 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=2/part-r-00002-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      440 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=2/part-r-00003-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      442 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=2/part-r-00004-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      439 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=2/part-r-00005-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      441 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=2/part-r-00006-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      443 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=2/part-r-00007-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
-drwxr-xr-x   0 mdurant    (501) staff       (20)        0 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=3/
--rw-r--r--   0 mdurant    (501) staff       (20)      436 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=3/part-r-00000-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      437 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=3/part-r-00001-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      442 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=3/part-r-00002-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      439 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=3/part-r-00003-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      441 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=3/part-r-00004-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      443 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=3/part-r-00005-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      440 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=3/part-r-00006-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      440 2018-09-04 14:23:40.000000 intake-parquet-0.2.3/tests/split/cat=freda/catnum=3/part-r-00007-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
-drwxr-xr-x   0 mdurant    (501) staff       (20)        0 2019-11-11 20:20:23.000000 intake-parquet-0.2.3/tests/test.parq/
--rw-r--r--   0 mdurant    (501) staff       (20)     2179 2018-01-07 22:02:06.000000 intake-parquet-0.2.3/tests/test.parq/_metadata
--rw-r--r--   0 mdurant    (501) staff       (20)    41809 2018-01-07 22:02:06.000000 intake-parquet-0.2.3/tests/test.parq/part.0.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)    41809 2018-01-07 22:02:06.000000 intake-parquet-0.2.3/tests/test.parq/part.1.parquet
--rw-r--r--   0 mdurant    (501) staff       (20)      404 2019-11-11 20:19:13.000000 intake-parquet-0.2.3/tests/test_discovery.py
--rw-r--r--   0 mdurant    (501) staff       (20)     4223 2019-11-11 20:11:18.000000 intake-parquet-0.2.3/tests/test_source.py
--rw-r--r--   0 mdurant    (501) staff       (20)      225 2018-01-05 15:44:00.000000 intake-parquet-0.2.3/tests/utils.py
--rw-r--r--   0 mdurant    (501) staff       (20)    68611 2018-04-16 17:35:13.000000 intake-parquet-0.2.3/versioneer.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:02:21.008161 intake-parquet-0.3.0/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1552 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/.travis.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)     1330 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/LICENSE
+-rw-r--r--   0 mdurant    (502) staff       (20)      282 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/MANIFEST.in
+-rw-r--r--   0 mdurant    (502) staff       (20)     1708 2023-05-29 20:02:21.008403 intake-parquet-0.3.0/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     1456 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/README.md
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:02:20.989865 intake-parquet-0.3.0/conda/
+-rw-r--r--   0 mdurant    (502) staff       (20)      676 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/conda/meta.yaml
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:02:20.990217 intake-parquet-0.3.0/docs/
+-rw-r--r--   0 mdurant    (502) staff       (20)      166 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/docs/environment.yml
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:02:20.990485 intake-parquet-0.3.0/examples/
+-rw-r--r--   0 mdurant    (502) staff       (20)      184 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/examples/sample.yml
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:02:20.991117 intake-parquet-0.3.0/examples/test.parq/
+-rw-r--r--   0 mdurant    (502) staff       (20)    15738 2023-05-29 19:14:36.000000 intake-parquet-0.3.0/examples/test.parq/part.0.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)    15738 2023-05-29 19:14:36.000000 intake-parquet-0.3.0/examples/test.parq/part.1.parquet
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:02:21.009231 intake-parquet-0.3.0/intake_parquet/
+-rw-r--r--   0 mdurant    (502) staff       (20)      156 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/intake_parquet/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      497 2023-05-29 20:02:21.009301 intake-parquet-0.3.0/intake_parquet/_version.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4064 2023-05-29 19:14:36.000000 intake-parquet-0.3.0/intake_parquet/source.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:02:21.007518 intake-parquet-0.3.0/intake_parquet.egg-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1708 2023-05-29 20:02:20.000000 intake-parquet-0.3.0/intake_parquet.egg-info/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     5238 2023-05-29 20:02:20.000000 intake-parquet-0.3.0/intake_parquet.egg-info/SOURCES.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-05-29 20:02:20.000000 intake-parquet-0.3.0/intake_parquet.egg-info/dependency_links.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)       63 2023-05-29 20:02:20.000000 intake-parquet-0.3.0/intake_parquet.egg-info/entry_points.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-05-09 17:47:35.000000 intake-parquet-0.3.0/intake_parquet.egg-info/not-zip-safe
+-rw-r--r--   0 mdurant    (502) staff       (20)       34 2023-05-29 20:02:20.000000 intake-parquet-0.3.0/intake_parquet.egg-info/requires.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)       15 2023-05-29 20:02:20.000000 intake-parquet-0.3.0/intake_parquet.egg-info/top_level.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)       38 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/readthedocs.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)       34 2023-05-29 19:18:18.000000 intake-parquet-0.3.0/requirements.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      186 2023-05-29 20:02:21.008851 intake-parquet-0.3.0/setup.cfg
+-rw-r--r--   0 mdurant    (502) staff       (20)      792 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/setup.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:02:21.007970 intake-parquet-0.3.0/tests/
+-rw-r--r--   0 mdurant    (502) staff       (20)      200 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/cache_cat.yaml
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:02:20.991764 intake-parquet-0.3.0/tests/split/
+-rw-r--r--   0 mdurant    (502) staff       (20)     7051 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/_metadata
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:02:20.985983 intake-parquet-0.3.0/tests/split/cat=fred/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:02:20.994168 intake-parquet-0.3.0/tests/split/cat=fred/catnum=1/
+-rw-r--r--   0 mdurant    (502) staff       (20)      434 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=1/part-r-00000-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      438 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=1/part-r-00001-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      439 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=1/part-r-00002-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      439 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=1/part-r-00003-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      441 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=1/part-r-00004-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      439 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=1/part-r-00005-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      438 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=1/part-r-00006-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      441 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=1/part-r-00007-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:02:20.996611 intake-parquet-0.3.0/tests/split/cat=fred/catnum=2/
+-rw-r--r--   0 mdurant    (502) staff       (20)      436 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=2/part-r-00000-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      435 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=2/part-r-00001-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      440 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=2/part-r-00002-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      439 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=2/part-r-00003-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      439 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=2/part-r-00004-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      442 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=2/part-r-00005-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      440 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=2/part-r-00006-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      438 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=2/part-r-00007-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:02:20.998865 intake-parquet-0.3.0/tests/split/cat=fred/catnum=3/
+-rw-r--r--   0 mdurant    (502) staff       (20)      437 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=3/part-r-00000-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      437 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=3/part-r-00001-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      438 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=3/part-r-00002-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      440 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=3/part-r-00003-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      439 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=3/part-r-00004-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      439 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=3/part-r-00005-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      442 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=3/part-r-00006-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      441 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=fred/catnum=3/part-r-00007-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:02:20.986500 intake-parquet-0.3.0/tests/split/cat=freda/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:02:21.000936 intake-parquet-0.3.0/tests/split/cat=freda/catnum=1/
+-rw-r--r--   0 mdurant    (502) staff       (20)      438 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=1/part-r-00000-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      438 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=1/part-r-00001-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      439 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=1/part-r-00002-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      442 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=1/part-r-00003-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      439 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=1/part-r-00004-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      441 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=1/part-r-00005-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      443 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=1/part-r-00006-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      440 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=1/part-r-00007-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:02:21.002623 intake-parquet-0.3.0/tests/split/cat=freda/catnum=2/
+-rw-r--r--   0 mdurant    (502) staff       (20)      436 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=2/part-r-00000-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      440 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=2/part-r-00001-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      439 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=2/part-r-00002-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      440 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=2/part-r-00003-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      442 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=2/part-r-00004-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      439 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=2/part-r-00005-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      441 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=2/part-r-00006-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      443 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=2/part-r-00007-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:02:21.004625 intake-parquet-0.3.0/tests/split/cat=freda/catnum=3/
+-rw-r--r--   0 mdurant    (502) staff       (20)      436 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=3/part-r-00000-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      437 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=3/part-r-00001-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      442 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=3/part-r-00002-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      439 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=3/part-r-00003-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      441 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=3/part-r-00004-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      443 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=3/part-r-00005-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      440 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=3/part-r-00006-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      440 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/split/cat=freda/catnum=3/part-r-00007-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:02:21.005159 intake-parquet-0.3.0/tests/test.parq/
+-rw-r--r--   0 mdurant    (502) staff       (20)    15738 2023-05-29 19:14:36.000000 intake-parquet-0.3.0/tests/test.parq/part.0.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)    15738 2023-05-29 19:14:36.000000 intake-parquet-0.3.0/tests/test.parq/part.1.parquet
+-rw-r--r--   0 mdurant    (502) staff       (20)      404 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/tests/test_discovery.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2564 2023-05-29 19:14:36.000000 intake-parquet-0.3.0/tests/test_source.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    68611 2023-05-09 17:47:26.000000 intake-parquet-0.3.0/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `intake-parquet-0.2.3/.travis.yml` & `intake-parquet-0.3.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `intake-parquet-0.2.3/LICENSE` & `intake-parquet-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `intake-parquet-0.2.3/PKG-INFO` & `intake-parquet-0.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: intake-parquet
-Version: 0.2.3
+Version: 0.3.0
 Summary: Intake parquet plugin
 Home-page: https://github.com/ContinuumIO/intake-parquet
 Maintainer: Martin Durant
 Maintainer-email: martin.durant@utoronto.ca
 License: BSD
-Description: # Intake-parquet
-        
-        [![Build Status](https://travis-ci.org/ContinuumIO/intake-parquet.svg?branch=master)](https://travis-ci.org/ContinuumIO/intake-parquet)
-        [![Documentation Status](https://readthedocs.org/projects/intake-parquet/badge/?version=latest)](http://intake-parquet.readthedocs.io/en/latest/?badge=latest)
-        
-        [Intake data loader](https://github.com/ContinuumIO/intake/) interface to the parquet binary tabular data format.
-        
-        Parquet is very popular in the big-data ecosystem, because it provides columnar
-        and chunk-wise access to the data, with efficient encodings and compression. This makes
-        the format particularly effective for streaming through large subsections of even
-        larger data-sets, hence it's common use with Hadoop and Spark.
-        
-        Parquet data may be single files, directories of files, or nested directories, where
-        the directory names are meaningful in the partitioning of the data.
-        
-        ### Features
-        
-        The parquet plugin allows for:
-        
-        - efficient metadata parsing, so you know the data types and number of records without
-          loading any data
-        - random access of partitions
-        - column and index selection, load only the data you need
-        - passing of value-based filters, that you only load those partitions containing some
-          valid data (NB: does not filter the values within a partition)
-        
-        ### Installation
-        
-        The conda install instructions are:
-        
-        ```
-        conda install -c conda-forge intake-parquet
-        ```
-        
-        ### Examples
-        
-        See the notebook in the examples/ directory.
-        
-Platform: UNKNOWN
+License-File: LICENSE
+
+# Intake-parquet
+
+[![Build Status](https://travis-ci.org/ContinuumIO/intake-parquet.svg?branch=master)](https://travis-ci.org/ContinuumIO/intake-parquet)
+[![Documentation Status](https://readthedocs.org/projects/intake-parquet/badge/?version=latest)](http://intake-parquet.readthedocs.io/en/latest/?badge=latest)
+
+[Intake data loader](https://github.com/ContinuumIO/intake/) interface to the parquet binary tabular data format.
+
+Parquet is very popular in the big-data ecosystem, because it provides columnar
+and chunk-wise access to the data, with efficient encodings and compression. This makes
+the format particularly effective for streaming through large subsections of even
+larger data-sets, hence it's common use with Hadoop and Spark.
+
+Parquet data may be single files, directories of files, or nested directories, where
+the directory names are meaningful in the partitioning of the data.
+
+### Features
+
+The parquet plugin allows for:
+
+- efficient metadata parsing, so you know the data types and number of records without
+  loading any data
+- random access of partitions
+- column and index selection, load only the data you need
+- passing of value-based filters, that you only load those partitions containing some
+  valid data (NB: does not filter the values within a partition)
+
+### Installation
+
+The conda install instructions are:
+
+```
+conda install -c conda-forge intake-parquet
+```
+
+### Examples
+
+See the notebook in the examples/ directory.
```

### Comparing `intake-parquet-0.2.3/README.md` & `intake-parquet-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `intake-parquet-0.2.3/conda/meta.yaml` & `intake-parquet-0.3.0/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `intake-parquet-0.2.3/intake_parquet/source.py` & `intake-parquet-0.3.0/intake_parquet/source.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import fsspec
 from intake.source import base
+
 from . import __version__
 
 
 class ParquetSource(base.DataSource):
     """
     Source to load parquet datasets.
 
@@ -10,40 +12,30 @@
 
     A parquet dataset may be a single file, a set of files in a single
     directory or a nested set of directories containing data-files.
 
     The implementation uses either fastparquet or pyarrow, select with the
     `engine=` kwarg.
 
-    Keyword parameters accepted by this Source:
+    Common keyword parameters accepted by this Source:
 
     - columns: list of str or None
         column names to load. If None, loads all
 
-    - index: str or None
-        column to make into the index of the dataframe. If None, may be
-        inferred from the saved matadata in certain cases.
-
     - filters: list of tuples
         row-group level filtering; a tuple like ``('x', '>', 1)`` would mean
         that if a row-group has a maximum value less than 1 for the column
         ``x``, then it will be skipped. Row-level filtering is *not*
         performed.
 
     - engine: 'fastparquet' or 'pyarrow'
         Which backend to read with.
 
-
-    - gather_statistics : bool or None (default).
-        Gather the statistics for each dataset partition. By default,
-        this will only be done if the _metadata file is available. Otherwise,
-        statistics will only be gathered if True, because the footer of
-        every file will be parsed (which is very slow on some systems).
-
-    - see dd.read_parquet() for the other named parameters that can be passed through.
+    - see pd.read_parquet and dd.read_parquet() for the other named parameters that
+      can be passed through.
     """
     container = 'dataframe'
     name = 'parquet'
     version = __version__
     partition_access = True
 
     def __init__(self, urlpath, metadata=None,
@@ -53,33 +45,48 @@
         self._kwargs = parquet_kwargs or {}
         self._df = None
 
         super(ParquetSource, self).__init__(metadata=metadata)
 
     def _get_schema(self):
         if self._df is None:
-            self._df = self._to_dask()
-        dtypes = {k: str(v) for k, v in self._df._meta.dtypes.items()}
-        self._schema = base.Schema(datashape=None,
-                                   dtype=dtypes,
-                                   shape=(None, len(self._df.columns)),
-                                   npartitions=self._df.npartitions,
-                                   extra_metadata={})
-        return self._schema
+            engine = self._kwargs.get("engine", "fastparquet")
+            fs, _, _ = fsspec.core.get_fs_token_paths(self._urlpath, **self._storage_options)
+            if engine == "fastparquet":
+                import fastparquet
+                pf = fastparquet.ParquetFile(self._urlpath, fs=fs)
+                lc = len(self._kwargs.get("columns") or []) or len(pf.columns)
+                dt = {k: str(v) for k, v in pf.dtypes.items()}
+                schema = base.Schema(dtype=dt, shape=(pf.count(), lc),
+                                npartitions=len(pf.row_groups), extra_metadata=pf.key_value_metadata)
+            else:
+                import pyarrow.parquet as pq
+                pf = pq.ParquetDataset(self._urlpath, filesystem=fs)
+                lc = len(self._kwargs.get("columns") or []) or len(pf.schema)
+                dt = {k: str(v) for k, v in zip(pf.schema.names, pf.schema.types)}
+                schema = base.Schema(dtype=dt, shape=(None, lc),
+                                npartitions=len(pf.fragments))
+        else:
+            npartitions = getattr(self._df, "npartitions", None)
+            schema = base.Schema(dtype=self._df.dtypes, shape=self._df.shape,
+                            npartitions=npartitions)
+        return schema
 
     def _get_partition(self, i):
-        self._get_schema()
-        return self._df.get_partition(i).compute()
+        return self.to_dask().get_partition(i).compute()
 
     def read(self):
         """
         Create single pandas dataframe from the whole data-set
         """
-        self._load_metadata()
-        return self._df.compute()
+        import pandas as pd
+        df = pd.read_parquet(self._urlpath, storage_options=self._storage_options,
+                             **self._kwargs)
+        self._df = df.iloc[:0]
+        return df
 
     def to_spark(self):
         """Produce Spark DataFrame equivalent
 
         This will ignore all arguments except the urlpath, which will be
         directly interpreted by Spark. If you need to configure the storage,
         that must be done on the spark side.
@@ -92,23 +99,15 @@
             ['read'],
             ['parquet', [self._urlpath]]
         ]
         sh = SparkHolder(True, args, {})
         return sh.setup()
 
     def to_dask(self):
-        self._load_metadata()
-        return self._df
-
-    def _to_dask(self):
-        """
-        Create a lazy dask-dataframe from the parquet data
-        """
         import dask.dataframe as dd
-        urlpath = self._get_cache(self._urlpath)[0]
-        self._df = dd.read_parquet(urlpath,
-                                   storage_options=self._storage_options, **self._kwargs)
-        self._load_metadata()
+        df = dd.read_parquet(self._urlpath, storage_options=self._storage_options,
+                             **self._kwargs)
+        self._df = df
         return self._df
 
     def _close(self):
         self._df = None
```

### Comparing `intake-parquet-0.2.3/intake_parquet.egg-info/PKG-INFO` & `intake-parquet-0.3.0/intake_parquet.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: intake-parquet
-Version: 0.2.3
+Version: 0.3.0
 Summary: Intake parquet plugin
 Home-page: https://github.com/ContinuumIO/intake-parquet
 Maintainer: Martin Durant
 Maintainer-email: martin.durant@utoronto.ca
 License: BSD
-Description: # Intake-parquet
-        
-        [![Build Status](https://travis-ci.org/ContinuumIO/intake-parquet.svg?branch=master)](https://travis-ci.org/ContinuumIO/intake-parquet)
-        [![Documentation Status](https://readthedocs.org/projects/intake-parquet/badge/?version=latest)](http://intake-parquet.readthedocs.io/en/latest/?badge=latest)
-        
-        [Intake data loader](https://github.com/ContinuumIO/intake/) interface to the parquet binary tabular data format.
-        
-        Parquet is very popular in the big-data ecosystem, because it provides columnar
-        and chunk-wise access to the data, with efficient encodings and compression. This makes
-        the format particularly effective for streaming through large subsections of even
-        larger data-sets, hence it's common use with Hadoop and Spark.
-        
-        Parquet data may be single files, directories of files, or nested directories, where
-        the directory names are meaningful in the partitioning of the data.
-        
-        ### Features
-        
-        The parquet plugin allows for:
-        
-        - efficient metadata parsing, so you know the data types and number of records without
-          loading any data
-        - random access of partitions
-        - column and index selection, load only the data you need
-        - passing of value-based filters, that you only load those partitions containing some
-          valid data (NB: does not filter the values within a partition)
-        
-        ### Installation
-        
-        The conda install instructions are:
-        
-        ```
-        conda install -c conda-forge intake-parquet
-        ```
-        
-        ### Examples
-        
-        See the notebook in the examples/ directory.
-        
-Platform: UNKNOWN
+License-File: LICENSE
+
+# Intake-parquet
+
+[![Build Status](https://travis-ci.org/ContinuumIO/intake-parquet.svg?branch=master)](https://travis-ci.org/ContinuumIO/intake-parquet)
+[![Documentation Status](https://readthedocs.org/projects/intake-parquet/badge/?version=latest)](http://intake-parquet.readthedocs.io/en/latest/?badge=latest)
+
+[Intake data loader](https://github.com/ContinuumIO/intake/) interface to the parquet binary tabular data format.
+
+Parquet is very popular in the big-data ecosystem, because it provides columnar
+and chunk-wise access to the data, with efficient encodings and compression. This makes
+the format particularly effective for streaming through large subsections of even
+larger data-sets, hence it's common use with Hadoop and Spark.
+
+Parquet data may be single files, directories of files, or nested directories, where
+the directory names are meaningful in the partitioning of the data.
+
+### Features
+
+The parquet plugin allows for:
+
+- efficient metadata parsing, so you know the data types and number of records without
+  loading any data
+- random access of partitions
+- column and index selection, load only the data you need
+- passing of value-based filters, that you only load those partitions containing some
+  valid data (NB: does not filter the values within a partition)
+
+### Installation
+
+The conda install instructions are:
+
+```
+conda install -c conda-forge intake-parquet
+```
+
+### Examples
+
+See the notebook in the examples/ directory.
```

### Comparing `intake-parquet-0.2.3/intake_parquet.egg-info/SOURCES.txt` & `intake-parquet-0.3.0/intake_parquet.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,25 +5,15 @@
 setup.cfg
 setup.py
 versioneer.py
 ./.travis.yml
 ./readthedocs.yml
 ./conda/meta.yaml
 ./docs/environment.yml
-./docs/build/html/api.html
-./docs/build/html/genindex.html
-./docs/build/html/index.html
-./docs/build/html/quickstart.html
-./docs/build/html/search.html
-./docs/build/html/_modules/index.html
-./docs/build/html/_modules/intake_parquet.html
-./docs/build/html/_modules/intake_parquet/__init__.html
-./docs/build/html/_modules/intake_parquet/source.html
 ./examples/sample.yml
-./examples/test.parq/_metadata
 ./examples/test.parq/part.0.parquet
 ./examples/test.parq/part.1.parquet
 ./tests/cache_cat.yaml
 ./tests/split/_metadata
 ./tests/split/cat=fred/catnum=1/part-r-00000-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
 ./tests/split/cat=fred/catnum=1/part-r-00001-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
 ./tests/split/cat=fred/catnum=1/part-r-00002-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
@@ -68,25 +58,21 @@
 ./tests/split/cat=freda/catnum=3/part-r-00001-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
 ./tests/split/cat=freda/catnum=3/part-r-00002-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
 ./tests/split/cat=freda/catnum=3/part-r-00003-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
 ./tests/split/cat=freda/catnum=3/part-r-00004-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
 ./tests/split/cat=freda/catnum=3/part-r-00005-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
 ./tests/split/cat=freda/catnum=3/part-r-00006-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
 ./tests/split/cat=freda/catnum=3/part-r-00007-4805f816-a859-4b75-8659-285a6617386f.gz.parquet
-./tests/test.parq/_metadata
 ./tests/test.parq/part.0.parquet
 ./tests/test.parq/part.1.parquet
 intake_parquet/__init__.py
 intake_parquet/_version.py
 intake_parquet/source.py
 intake_parquet.egg-info/PKG-INFO
 intake_parquet.egg-info/SOURCES.txt
 intake_parquet.egg-info/dependency_links.txt
 intake_parquet.egg-info/entry_points.txt
 intake_parquet.egg-info/not-zip-safe
-intake_parquet.egg-info/pbr.json
 intake_parquet.egg-info/requires.txt
 intake_parquet.egg-info/top_level.txt
-tests/__init__.py
 tests/test_discovery.py
-tests/test_source.py
-tests/utils.py
+tests/test_source.py
```

### Comparing `intake-parquet-0.2.3/setup.py` & `intake-parquet-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     description='Intake parquet plugin',
     url='https://github.com/ContinuumIO/intake-parquet',
     maintainer='Martin Durant',
     maintainer_email='martin.durant@utoronto.ca',
     license='BSD',
-    packages=find_packages(),
+    packages=find_packages(exclude=['tests']),
     # package_data={'': ['*.pcap', '*.yml', '*.html']},
     entry_points={
         'intake.drivers': ['parquet = intake_parquet.source:ParquetSource']},
     include_package_data=True,
     install_requires=requires,
     long_description=open('README.md').read(),
     zip_safe=False,
```

### Comparing `intake-parquet-0.2.3/tests/split/_metadata` & `intake-parquet-0.3.0/tests/split/_metadata`

 * *Files identical despite different names*

### Comparing `intake-parquet-0.2.3/tests/test_source.py` & `intake-parquet-0.3.0/tests/test_source.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,44 +5,44 @@
 import pickle
 import pytest
 import shutil
 
 from intake_parquet.source import ParquetSource
 import intake
 
-intake.registry['parquet'] = ParquetSource  # because pytest defers import
+# intake.register_driver('parquet', ParquetSource, clobber=True)  # because pytest defers import
 here = os.path.dirname(__file__)
 path = os.path.join(here, 'test.parq')
 path2 = os.path.join(here, 'test2.parq')
 pf = fastparquet.ParquetFile(path)
 data = next(pf.iter_row_groups())
 data2 = pf.to_pandas()
 
 
 @pytest.mark.parametrize('url', [path,
                                  [os.path.join(path, 'part.0.parquet'),
                                   os.path.join(path, 'part.1.parquet')],
-                                 path2])
+                                 ])
 @pytest.mark.parametrize('columns', [None,
                                      ['bhello', 'f', 'i32'],
                                      ['bhello']])
 def test_source(url, columns):
     if columns:
         d = data[columns]
         d2 = data2[columns]
     else:
         d = data
         d2 = data2
-    source = ParquetSource(url, columns=columns)
+    source = ParquetSource(url, columns=columns, engine="fastparquet")
     source.discover()
     assert source.npartitions == 2
-    assert source.shape == (None, len(d2.columns))
+    assert source.shape == (2000, len(d2.columns))
     assert source.dtype['bhello'] == 'object'
     part0 = source.read_partition(0)
-    assert len(part0) == 1001
+    assert len(part0) == 1000
     assert part0.reset_index(drop=True).equals(d)
     it = source.read_chunked()
     assert next(it).reset_index(drop=True).equals(part0)
     assert next(it).reset_index(drop=True).equals(part0)
     with pytest.raises(StopIteration):
         next(it)
     with pytest.raises(IndexError):
@@ -61,70 +61,19 @@
     assert d2['dtype'] == d['dtype']
     assert d2['shape'] == d['shape']
     # dask index starts at 0 for each partition
     assert df.compute().reset_index(drop=True).equals(
         source.read().reset_index(drop=True))
 
 
-def test_discover_serialize():
-    source = ParquetSource(path)
+@pytest.mark.parametrize("engine", ["fastparquet", "pyarrow"])
+def test_discover_serialize(engine):
+    source = ParquetSource(path, engine=engine)
     assert msgpack.packb(source.discover())
 
 
 def test_pickle():
     source = ParquetSource(path)
     d = source.read()
     source2 = pickle.loads(pickle.dumps(source))
     d2 = source2.read()
     assert d.equals(d2)
-
-
-def test_on_s3():
-    pytest.importorskip('s3fs')
-    s = ParquetSource('s3://MDtemp/gzip-nation.impala.parquet')
-    s.read()
-    assert s.shape == (None, 4)
-
-
-def test_filter():
-    import tempfile
-    import pandas as pd
-    import numpy as np
-    d = str(tempfile.mkdtemp())
-    try:
-        df = pd.DataFrame({'a': np.random.randint(10, size=100),
-                           'b': np.random.choice(['oi', 'hi'], size=100)})
-        df.index.name = 'index'
-        fastparquet.write(d, df, partition_on=['b'], file_scheme='hive',
-                          write_index=True)
-        s = ParquetSource(d, filters=[('b', '==', 'hi')])
-        disc = s.discover()
-        assert disc['npartitions'] == 1
-        # TODO: this fails because the index appears as a column
-        # assert disc['shape'] == df[df.b == 'hi'].shape
-        out = s.read()
-        assert 'oi' not in out.b
-        assert df[df.b == 'hi'].a.equals(out.a)
-    finally:
-        import shutil
-        shutil.rmtree(d)
-
-
-def test_with_cache():
-    import tempfile
-    d = tempfile.mkdtemp()
-    old = intake.config.conf['cache_dir']
-    expected = fastparquet.ParquetFile(os.path.join(here, 'split')).to_pandas()
-    try:
-        intake.config.conf['cache_dir'] = d
-        cat = intake.open_catalog(os.path.join(here, 'cache_cat.yaml'))
-        s = cat.split()
-        assert isinstance(s.cache[0], intake.source.cache.DirCache)
-        outfiles = s.cache[0].load(s._urlpath, output=False)
-        assert outfiles
-        assert outfiles[0].startswith(s.cache_dirs[0])
-        loc = s.cache[0]._path(s._urlpath)
-        assert glob.glob(loc + '/*/*/*.parquet')
-        assert s.read().reset_index(drop=True).equals(expected)
-    finally:
-        shutil.rmtree(d)
-        intake.config.conf['cache_dir'] = old
```

### Comparing `intake-parquet-0.2.3/versioneer.py` & `intake-parquet-0.3.0/versioneer.py`

 * *Files identical despite different names*

