# Comparing `tmp/intake-0.6.8.tar.gz` & `tmp/intake-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intake-0.6.8.tar", last modified: Sat Mar 11 21:21:32 2023, max compression
+gzip compressed data, was "intake-0.7.0.tar", last modified: Mon May 29 19:22:32 2023, max compression
```

## Comparing `intake-0.6.8.tar` & `intake-0.7.0.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.333839 intake-0.6.8/
--rw-r--r--   0 mdurant    (502) staff       (20)     1286 2022-09-18 01:28:48.000000 intake-0.6.8/LICENSE
--rw-r--r--   0 mdurant    (502) staff       (20)      532 2023-02-23 03:44:29.000000 intake-0.6.8/MANIFEST.in
--rw-r--r--   0 mdurant    (502) staff       (20)     3184 2023-03-11 21:21:32.333931 intake-0.6.8/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)     2520 2023-03-10 19:57:14.000000 intake-0.6.8/README.md
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.334603 intake-0.6.8/intake/
--rw-r--r--   0 mdurant    (502) staff       (20)     5346 2023-03-10 22:11:03.000000 intake-0.6.8/intake/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)      497 2023-03-11 21:21:32.334686 intake-0.6.8/intake/_version.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.315314 intake-0.6.8/intake/auth/
--rw-r--r--   0 mdurant    (502) staff       (20)      328 2023-02-23 03:44:29.000000 intake-0.6.8/intake/auth/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2380 2023-02-23 03:44:29.000000 intake-0.6.8/intake/auth/base.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1855 2023-02-23 03:44:29.000000 intake-0.6.8/intake/auth/secret.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.317451 intake-0.6.8/intake/catalog/
--rw-r--r--   0 mdurant    (502) staff       (20)      844 2023-02-23 03:44:29.000000 intake-0.6.8/intake/catalog/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)    17369 2023-03-01 20:40:48.000000 intake-0.6.8/intake/catalog/base.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3132 2023-02-23 03:44:29.000000 intake-0.6.8/intake/catalog/default.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5335 2023-02-23 03:44:29.000000 intake-0.6.8/intake/catalog/entry.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2514 2023-02-23 03:44:29.000000 intake-0.6.8/intake/catalog/exceptions.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3754 2023-02-23 03:44:29.000000 intake-0.6.8/intake/catalog/gui.py
--rw-r--r--   0 mdurant    (502) staff       (20)    32511 2023-02-23 03:44:29.000000 intake-0.6.8/intake/catalog/local.py
--rw-r--r--   0 mdurant    (502) staff       (20)    20263 2023-02-23 03:44:29.000000 intake-0.6.8/intake/catalog/remote.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.306748 intake-0.6.8/intake/catalog/tests/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.317641 intake-0.6.8/intake/catalog/tests/catalog_search/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.307084 intake-0.6.8/intake/catalog/tests/catalog_search/example_packages/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.317855 intake-0.6.8/intake/catalog/tests/catalog_search/example_packages/ep/
--rw-r--r--   0 mdurant    (502) staff       (20)       27 2022-09-18 01:28:48.000000 intake-0.6.8/intake/catalog/tests/catalog_search/example_packages/ep/__init__.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.318059 intake-0.6.8/intake/catalog/tests/catalog_search/example_packages/ep-0.1.dist-info/
--rw-r--r--   0 mdurant    (502) staff       (20)       39 2022-09-18 01:28:48.000000 intake-0.6.8/intake/catalog/tests/catalog_search/example_packages/ep-0.1.dist-info/entry_points.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      169 2023-02-23 03:44:29.000000 intake-0.6.8/intake/catalog/tests/catalog_search/yaml.yml
--rw-r--r--   0 mdurant    (502) staff       (20)    11256 2023-03-10 19:57:14.000000 intake-0.6.8/intake/catalog/utils.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3087 2023-02-23 03:44:29.000000 intake-0.6.8/intake/catalog/zarr.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.318658 intake-0.6.8/intake/cli/
--rw-r--r--   0 mdurant    (502) staff       (20)      439 2023-02-23 03:44:29.000000 intake-0.6.8/intake/cli/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2101 2023-02-23 03:44:29.000000 intake-0.6.8/intake/cli/bootstrap.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.319028 intake-0.6.8/intake/cli/client/
--rw-r--r--   0 mdurant    (502) staff       (20)      328 2023-02-23 03:44:29.000000 intake-0.6.8/intake/cli/client/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1080 2023-02-23 03:44:29.000000 intake-0.6.8/intake/cli/client/__main__.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.321320 intake-0.6.8/intake/cli/client/subcommands/
--rw-r--r--   0 mdurant    (502) staff       (20)      722 2023-02-23 03:44:29.000000 intake-0.6.8/intake/cli/client/subcommands/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2663 2023-02-23 03:44:29.000000 intake-0.6.8/intake/cli/client/subcommands/cache.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2579 2023-02-23 03:44:29.000000 intake-0.6.8/intake/cli/client/subcommands/config.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1285 2023-02-23 03:44:29.000000 intake-0.6.8/intake/cli/client/subcommands/describe.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1291 2023-02-23 03:44:29.000000 intake-0.6.8/intake/cli/client/subcommands/discover.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2892 2023-02-23 03:44:29.000000 intake-0.6.8/intake/cli/client/subcommands/drivers.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1922 2023-02-23 03:44:29.000000 intake-0.6.8/intake/cli/client/subcommands/example.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1271 2023-02-23 03:44:29.000000 intake-0.6.8/intake/cli/client/subcommands/exists.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1272 2023-02-23 03:44:29.000000 intake-0.6.8/intake/cli/client/subcommands/get.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1810 2023-02-23 03:44:29.000000 intake-0.6.8/intake/cli/client/subcommands/info.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1361 2023-02-23 03:44:29.000000 intake-0.6.8/intake/cli/client/subcommands/list.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1463 2023-02-23 03:44:29.000000 intake-0.6.8/intake/cli/client/subcommands/precache.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.321927 intake-0.6.8/intake/cli/sample/
--rw-r--r--   0 mdurant    (502) staff       (20)    14735 2022-09-18 01:28:48.000000 intake-0.6.8/intake/cli/sample/states_1.csv
--rw-r--r--   0 mdurant    (502) staff       (20)    15657 2023-02-23 03:44:29.000000 intake-0.6.8/intake/cli/sample/states_2.csv
--rw-r--r--   0 mdurant    (502) staff       (20)      284 2022-09-18 01:28:48.000000 intake-0.6.8/intake/cli/sample/us_states.yml
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.322497 intake-0.6.8/intake/cli/server/
--rw-r--r--   0 mdurant    (502) staff       (20)      328 2023-02-23 03:44:29.000000 intake-0.6.8/intake/cli/server/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2977 2023-02-23 03:44:29.000000 intake-0.6.8/intake/cli/server/__main__.py
--rw-r--r--   0 mdurant    (502) staff       (20)    14884 2023-02-23 03:44:29.000000 intake-0.6.8/intake/cli/server/server.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.322698 intake-0.6.8/intake/cli/server/templates/
--rw-r--r--   0 mdurant    (502) staff       (20)     2168 2023-02-23 03:44:29.000000 intake-0.6.8/intake/cli/server/templates/index.html
--rw-r--r--   0 mdurant    (502) staff       (20)     3277 2023-02-23 03:44:29.000000 intake-0.6.8/intake/cli/util.py
--rw-r--r--   0 mdurant    (502) staff       (20)      915 2023-02-23 03:44:29.000000 intake-0.6.8/intake/compat.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4092 2023-02-23 03:44:29.000000 intake-0.6.8/intake/config.py
--rw-r--r--   0 mdurant    (502) staff       (20)     6361 2023-02-23 03:44:29.000000 intake-0.6.8/intake/conftest.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.324103 intake-0.6.8/intake/container/
--rw-r--r--   0 mdurant    (502) staff       (20)     3671 2023-02-23 03:44:29.000000 intake-0.6.8/intake/container/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4108 2023-02-23 03:44:29.000000 intake-0.6.8/intake/container/base.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5999 2023-02-23 03:44:29.000000 intake-0.6.8/intake/container/dataframe.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3417 2023-03-08 16:16:28.000000 intake-0.6.8/intake/container/ndarray.py
--rw-r--r--   0 mdurant    (502) staff       (20)     6354 2023-02-23 03:44:29.000000 intake-0.6.8/intake/container/persist.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3337 2023-02-23 03:44:29.000000 intake-0.6.8/intake/container/semistructured.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4189 2023-02-23 03:44:29.000000 intake-0.6.8/intake/container/serializer.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.324983 intake-0.6.8/intake/interface/
--rw-r--r--   0 mdurant    (502) staff       (20)     1717 2023-02-23 03:44:29.000000 intake-0.6.8/intake/interface/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     8872 2023-02-23 03:44:29.000000 intake-0.6.8/intake/interface/base.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.325862 intake-0.6.8/intake/interface/catalog/
--rw-r--r--   0 mdurant    (502) staff       (20)      328 2023-02-23 03:44:29.000000 intake-0.6.8/intake/interface/catalog/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10906 2023-02-23 03:44:29.000000 intake-0.6.8/intake/interface/catalog/add.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5782 2023-02-23 03:44:29.000000 intake-0.6.8/intake/interface/catalog/gui.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5233 2023-02-23 03:44:29.000000 intake-0.6.8/intake/interface/catalog/search.py
--rw-r--r--   0 mdurant    (502) staff       (20)     6129 2023-02-23 03:44:29.000000 intake-0.6.8/intake/interface/catalog/select.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1728 2023-02-23 03:44:29.000000 intake-0.6.8/intake/interface/conftest.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3673 2023-02-23 03:44:29.000000 intake-0.6.8/intake/interface/gui.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.326025 intake-0.6.8/intake/interface/icons/
--rw-r--r--   0 mdurant    (502) staff       (20)     1556 2022-09-18 01:28:48.000000 intake-0.6.8/intake/interface/icons/logo.png
--rw-r--r--   0 mdurant    (502) staff       (20)      532 2023-02-23 03:44:29.000000 intake-0.6.8/intake/interface/server.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.326888 intake-0.6.8/intake/interface/source/
--rw-r--r--   0 mdurant    (502) staff       (20)      328 2023-02-23 03:44:29.000000 intake-0.6.8/intake/interface/source/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)    14360 2023-02-23 03:44:29.000000 intake-0.6.8/intake/interface/source/defined_plots.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2121 2023-02-23 03:44:29.000000 intake-0.6.8/intake/interface/source/description.py
--rw-r--r--   0 mdurant    (502) staff       (20)     8343 2023-02-23 03:44:29.000000 intake-0.6.8/intake/interface/source/gui.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4512 2023-02-23 03:44:29.000000 intake-0.6.8/intake/interface/source/select.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.331029 intake-0.6.8/intake/source/
--rw-r--r--   0 mdurant    (502) staff       (20)     2521 2023-02-23 03:44:29.000000 intake-0.6.8/intake/source/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)    16817 2023-02-23 03:44:29.000000 intake-0.6.8/intake/source/base.py
--rw-r--r--   0 mdurant    (502) staff       (20)    19217 2023-02-23 03:44:29.000000 intake-0.6.8/intake/source/cache.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5198 2023-02-23 03:44:29.000000 intake-0.6.8/intake/source/csv.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1998 2023-02-23 03:44:29.000000 intake-0.6.8/intake/source/decompress.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9575 2023-02-23 03:44:29.000000 intake-0.6.8/intake/source/derived.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9604 2023-03-10 22:11:03.000000 intake-0.6.8/intake/source/discovery.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5413 2023-02-23 03:44:29.000000 intake-0.6.8/intake/source/jsonfiles.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5705 2023-03-10 19:57:14.000000 intake-0.6.8/intake/source/npy.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.308573 intake-0.6.8/intake/source/tests/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.309037 intake-0.6.8/intake/source/tests/plugin_searchpath/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.331381 intake-0.6.8/intake/source/tests/plugin_searchpath/collision_foo/
--rw-r--r--   0 mdurant    (502) staff       (20)      496 2023-02-23 03:44:29.000000 intake-0.6.8/intake/source/tests/plugin_searchpath/collision_foo/__init__.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.331647 intake-0.6.8/intake/source/tests/plugin_searchpath/collision_foo2/
--rw-r--r--   0 mdurant    (502) staff       (20)      496 2023-02-23 03:44:29.000000 intake-0.6.8/intake/source/tests/plugin_searchpath/collision_foo2/__init__.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.331890 intake-0.6.8/intake/source/tests/plugin_searchpath/driver_with_entrypoints/
--rw-r--r--   0 mdurant    (502) staff       (20)       30 2022-09-18 01:28:48.000000 intake-0.6.8/intake/source/tests/plugin_searchpath/driver_with_entrypoints/__init__.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.332108 intake-0.6.8/intake/source/tests/plugin_searchpath/intake_foo/
--rw-r--r--   0 mdurant    (502) staff       (20)      544 2023-02-23 03:44:29.000000 intake-0.6.8/intake/source/tests/plugin_searchpath/intake_foo/__init__.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.332346 intake-0.6.8/intake/source/tests/plugin_searchpath/not_intake_foo/
--rw-r--r--   0 mdurant    (502) staff       (20)      549 2023-02-23 03:44:29.000000 intake-0.6.8/intake/source/tests/plugin_searchpath/not_intake_foo/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4280 2023-02-23 03:44:29.000000 intake-0.6.8/intake/source/textfiles.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4376 2023-02-23 03:44:29.000000 intake-0.6.8/intake/source/tiled.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9694 2023-02-23 03:44:29.000000 intake-0.6.8/intake/source/utils.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2763 2023-02-23 03:44:29.000000 intake-0.6.8/intake/source/zarr.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1735 2023-02-23 03:44:29.000000 intake-0.6.8/intake/util_tests.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9286 2023-02-23 03:44:29.000000 intake-0.6.8/intake/utils.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.314604 intake-0.6.8/intake.egg-info/
--rw-r--r--   0 mdurant    (502) staff       (20)     3184 2023-03-11 21:21:32.000000 intake-0.6.8/intake.egg-info/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)     3466 2023-03-11 21:21:32.000000 intake-0.6.8/intake.egg-info/SOURCES.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-03-11 21:21:32.000000 intake-0.6.8/intake.egg-info/dependency_links.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      762 2023-03-11 21:21:32.000000 intake-0.6.8/intake.egg-info/entry_points.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-09-21 20:58:10.000000 intake-0.6.8/intake.egg-info/not-zip-safe
--rw-r--r--   0 mdurant    (502) staff       (20)      346 2023-03-11 21:21:32.000000 intake-0.6.8/intake.egg-info/requires.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        7 2023-03-11 21:21:32.000000 intake-0.6.8/intake.egg-info/top_level.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      304 2023-02-23 03:44:29.000000 intake-0.6.8/pyproject.toml
--rw-r--r--   0 mdurant    (502) staff       (20)       74 2023-02-15 12:19:41.000000 intake-0.6.8/requirements.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      290 2023-03-11 21:21:32.334319 intake-0.6.8/setup.cfg
--rw-r--r--   0 mdurant    (502) staff       (20)     2995 2023-02-23 03:44:29.000000 intake-0.6.8/setup.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.332538 intake-0.6.8/templates/
--rw-r--r--   0 mdurant    (502) staff       (20)      529 2022-09-18 01:28:48.000000 intake-0.6.8/templates/README.md
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.332739 intake-0.6.8/templates/data_package/
--rw-r--r--   0 mdurant    (502) staff       (20)      285 2022-09-18 01:28:48.000000 intake-0.6.8/templates/data_package/cookiecutter.json
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.332956 intake-0.6.8/templates/data_package/hooks/
--rw-r--r--   0 mdurant    (502) staff       (20)      747 2023-02-23 03:44:29.000000 intake-0.6.8/templates/data_package/hooks/post_gen_project.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-11 21:21:32.333644 intake-0.6.8/templates/data_package/{{cookiecutter.package_name}}/
--rw-r--r--   0 mdurant    (502) staff       (20)      333 2022-09-18 01:28:48.000000 intake-0.6.8/templates/data_package/{{cookiecutter.package_name}}/build.sh
--rw-r--r--   0 mdurant    (502) staff       (20)      521 2023-02-23 03:44:29.000000 intake-0.6.8/templates/data_package/{{cookiecutter.package_name}}/meta.yaml
--rw-r--r--   0 mdurant    (502) staff       (20)      210 2022-09-18 01:28:48.000000 intake-0.6.8/templates/data_package/{{cookiecutter.package_name}}/{{cookiecutter.dataset_name}}.yaml
--rw-r--r--   0 mdurant    (502) staff       (20)    67803 2023-02-23 03:44:29.000000 intake-0.6.8/versioneer.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.320659 intake-0.7.0/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1286 2022-09-18 01:28:48.000000 intake-0.7.0/LICENSE
+-rw-r--r--   0 mdurant    (502) staff       (20)      532 2023-02-23 03:44:29.000000 intake-0.7.0/MANIFEST.in
+-rw-r--r--   0 mdurant    (502) staff       (20)     3184 2023-05-29 19:22:32.320749 intake-0.7.0/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     2520 2023-03-10 19:57:14.000000 intake-0.7.0/README.md
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.321386 intake-0.7.0/intake/
+-rw-r--r--   0 mdurant    (502) staff       (20)     5997 2023-05-29 19:06:25.000000 intake-0.7.0/intake/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      497 2023-05-29 19:22:32.321443 intake-0.7.0/intake/_version.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.295617 intake-0.7.0/intake/auth/
+-rw-r--r--   0 mdurant    (502) staff       (20)      328 2023-02-23 03:44:29.000000 intake-0.7.0/intake/auth/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2390 2023-05-17 00:57:11.000000 intake-0.7.0/intake/auth/base.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1855 2023-02-23 03:44:29.000000 intake-0.7.0/intake/auth/secret.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.298147 intake-0.7.0/intake/catalog/
+-rw-r--r--   0 mdurant    (502) staff       (20)      844 2023-02-23 03:44:29.000000 intake-0.7.0/intake/catalog/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    17369 2023-03-01 20:40:48.000000 intake-0.7.0/intake/catalog/base.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3132 2023-05-16 20:05:35.000000 intake-0.7.0/intake/catalog/default.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     5335 2023-02-23 03:44:29.000000 intake-0.7.0/intake/catalog/entry.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2514 2023-02-23 03:44:29.000000 intake-0.7.0/intake/catalog/exceptions.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3754 2023-02-23 03:44:29.000000 intake-0.7.0/intake/catalog/gui.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    32641 2023-05-29 19:06:25.000000 intake-0.7.0/intake/catalog/local.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    20263 2023-02-23 03:44:29.000000 intake-0.7.0/intake/catalog/remote.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.288353 intake-0.7.0/intake/catalog/tests/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.298525 intake-0.7.0/intake/catalog/tests/catalog_search/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.288616 intake-0.7.0/intake/catalog/tests/catalog_search/example_packages/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.298743 intake-0.7.0/intake/catalog/tests/catalog_search/example_packages/ep/
+-rw-r--r--   0 mdurant    (502) staff       (20)       27 2022-09-18 01:28:48.000000 intake-0.7.0/intake/catalog/tests/catalog_search/example_packages/ep/__init__.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.299044 intake-0.7.0/intake/catalog/tests/catalog_search/example_packages/ep-0.1.dist-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)       39 2022-09-18 01:28:48.000000 intake-0.7.0/intake/catalog/tests/catalog_search/example_packages/ep-0.1.dist-info/entry_points.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      169 2023-02-23 03:44:29.000000 intake-0.7.0/intake/catalog/tests/catalog_search/yaml.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)    11256 2023-03-10 19:57:14.000000 intake-0.7.0/intake/catalog/utils.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3087 2023-02-23 03:44:29.000000 intake-0.7.0/intake/catalog/zarr.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.300883 intake-0.7.0/intake/cli/
+-rw-r--r--   0 mdurant    (502) staff       (20)      439 2023-02-23 03:44:29.000000 intake-0.7.0/intake/cli/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2101 2023-02-23 03:44:29.000000 intake-0.7.0/intake/cli/bootstrap.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.301609 intake-0.7.0/intake/cli/client/
+-rw-r--r--   0 mdurant    (502) staff       (20)      328 2023-02-23 03:44:29.000000 intake-0.7.0/intake/cli/client/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1080 2023-02-23 03:44:29.000000 intake-0.7.0/intake/cli/client/__main__.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.304431 intake-0.7.0/intake/cli/client/subcommands/
+-rw-r--r--   0 mdurant    (502) staff       (20)      722 2023-02-23 03:44:29.000000 intake-0.7.0/intake/cli/client/subcommands/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2663 2023-02-23 03:44:29.000000 intake-0.7.0/intake/cli/client/subcommands/cache.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2579 2023-02-23 03:44:29.000000 intake-0.7.0/intake/cli/client/subcommands/config.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1285 2023-02-23 03:44:29.000000 intake-0.7.0/intake/cli/client/subcommands/describe.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1291 2023-02-23 03:44:29.000000 intake-0.7.0/intake/cli/client/subcommands/discover.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2892 2023-02-23 03:44:29.000000 intake-0.7.0/intake/cli/client/subcommands/drivers.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1922 2023-02-23 03:44:29.000000 intake-0.7.0/intake/cli/client/subcommands/example.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1271 2023-02-23 03:44:29.000000 intake-0.7.0/intake/cli/client/subcommands/exists.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1272 2023-02-23 03:44:29.000000 intake-0.7.0/intake/cli/client/subcommands/get.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1810 2023-02-23 03:44:29.000000 intake-0.7.0/intake/cli/client/subcommands/info.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1361 2023-02-23 03:44:29.000000 intake-0.7.0/intake/cli/client/subcommands/list.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1463 2023-02-23 03:44:29.000000 intake-0.7.0/intake/cli/client/subcommands/precache.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.305299 intake-0.7.0/intake/cli/sample/
+-rw-r--r--   0 mdurant    (502) staff       (20)    14735 2022-09-18 01:28:48.000000 intake-0.7.0/intake/cli/sample/states_1.csv
+-rw-r--r--   0 mdurant    (502) staff       (20)    15657 2023-02-23 03:44:29.000000 intake-0.7.0/intake/cli/sample/states_2.csv
+-rw-r--r--   0 mdurant    (502) staff       (20)      284 2022-09-18 01:28:48.000000 intake-0.7.0/intake/cli/sample/us_states.yml
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.306151 intake-0.7.0/intake/cli/server/
+-rw-r--r--   0 mdurant    (502) staff       (20)      328 2023-02-23 03:44:29.000000 intake-0.7.0/intake/cli/server/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2977 2023-02-23 03:44:29.000000 intake-0.7.0/intake/cli/server/__main__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    14884 2023-02-23 03:44:29.000000 intake-0.7.0/intake/cli/server/server.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.306385 intake-0.7.0/intake/cli/server/templates/
+-rw-r--r--   0 mdurant    (502) staff       (20)     2168 2023-02-23 03:44:29.000000 intake-0.7.0/intake/cli/server/templates/index.html
+-rw-r--r--   0 mdurant    (502) staff       (20)     3277 2023-02-23 03:44:29.000000 intake-0.7.0/intake/cli/util.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      915 2023-02-23 03:44:29.000000 intake-0.7.0/intake/compat.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4113 2023-05-17 00:57:11.000000 intake-0.7.0/intake/config.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     6400 2023-05-17 00:57:11.000000 intake-0.7.0/intake/conftest.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.308366 intake-0.7.0/intake/container/
+-rw-r--r--   0 mdurant    (502) staff       (20)     3671 2023-02-23 03:44:29.000000 intake-0.7.0/intake/container/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4108 2023-02-23 03:44:29.000000 intake-0.7.0/intake/container/base.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     5982 2023-05-17 00:57:11.000000 intake-0.7.0/intake/container/dataframe.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3417 2023-03-08 16:16:28.000000 intake-0.7.0/intake/container/ndarray.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     6353 2023-05-17 00:57:11.000000 intake-0.7.0/intake/container/persist.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3337 2023-02-23 03:44:29.000000 intake-0.7.0/intake/container/semistructured.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4517 2023-05-09 18:13:01.000000 intake-0.7.0/intake/container/serializer.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.309698 intake-0.7.0/intake/interface/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1717 2023-02-23 03:44:29.000000 intake-0.7.0/intake/interface/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     8989 2023-05-23 02:32:42.000000 intake-0.7.0/intake/interface/base.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.311089 intake-0.7.0/intake/interface/catalog/
+-rw-r--r--   0 mdurant    (502) staff       (20)      328 2023-02-23 03:44:29.000000 intake-0.7.0/intake/interface/catalog/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    10906 2023-02-23 03:44:29.000000 intake-0.7.0/intake/interface/catalog/add.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     5782 2023-05-23 01:57:08.000000 intake-0.7.0/intake/interface/catalog/gui.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     5233 2023-02-23 03:44:29.000000 intake-0.7.0/intake/interface/catalog/search.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     6129 2023-05-23 01:47:51.000000 intake-0.7.0/intake/interface/catalog/select.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1728 2023-02-23 03:44:29.000000 intake-0.7.0/intake/interface/conftest.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3673 2023-02-23 03:44:29.000000 intake-0.7.0/intake/interface/gui.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.311398 intake-0.7.0/intake/interface/icons/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1556 2022-09-18 01:28:48.000000 intake-0.7.0/intake/interface/icons/logo.png
+-rw-r--r--   0 mdurant    (502) staff       (20)      532 2023-02-23 03:44:29.000000 intake-0.7.0/intake/interface/server.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.312481 intake-0.7.0/intake/interface/source/
+-rw-r--r--   0 mdurant    (502) staff       (20)      328 2023-02-23 03:44:29.000000 intake-0.7.0/intake/interface/source/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    14360 2023-02-23 03:44:29.000000 intake-0.7.0/intake/interface/source/defined_plots.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2121 2023-02-23 03:44:29.000000 intake-0.7.0/intake/interface/source/description.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     8343 2023-02-23 03:44:29.000000 intake-0.7.0/intake/interface/source/gui.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4512 2023-02-23 03:44:29.000000 intake-0.7.0/intake/interface/source/select.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.316513 intake-0.7.0/intake/source/
+-rw-r--r--   0 mdurant    (502) staff       (20)     2521 2023-02-23 03:44:29.000000 intake-0.7.0/intake/source/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    17029 2023-05-19 20:19:40.000000 intake-0.7.0/intake/source/base.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    19083 2023-05-17 00:57:11.000000 intake-0.7.0/intake/source/cache.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     7588 2023-05-16 17:13:52.000000 intake-0.7.0/intake/source/csv.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1998 2023-05-16 20:04:06.000000 intake-0.7.0/intake/source/decompress.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    16158 2023-05-09 18:20:46.000000 intake-0.7.0/intake/source/derived.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9604 2023-03-10 22:11:03.000000 intake-0.7.0/intake/source/discovery.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     5413 2023-02-23 03:44:29.000000 intake-0.7.0/intake/source/jsonfiles.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     5705 2023-03-10 19:57:14.000000 intake-0.7.0/intake/source/npy.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.289786 intake-0.7.0/intake/source/tests/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.290186 intake-0.7.0/intake/source/tests/plugin_searchpath/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.316805 intake-0.7.0/intake/source/tests/plugin_searchpath/collision_foo/
+-rw-r--r--   0 mdurant    (502) staff       (20)      496 2023-02-23 03:44:29.000000 intake-0.7.0/intake/source/tests/plugin_searchpath/collision_foo/__init__.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.316976 intake-0.7.0/intake/source/tests/plugin_searchpath/collision_foo2/
+-rw-r--r--   0 mdurant    (502) staff       (20)      496 2023-02-23 03:44:29.000000 intake-0.7.0/intake/source/tests/plugin_searchpath/collision_foo2/__init__.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.317154 intake-0.7.0/intake/source/tests/plugin_searchpath/driver_with_entrypoints/
+-rw-r--r--   0 mdurant    (502) staff       (20)       30 2022-09-18 01:28:48.000000 intake-0.7.0/intake/source/tests/plugin_searchpath/driver_with_entrypoints/__init__.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.317550 intake-0.7.0/intake/source/tests/plugin_searchpath/intake_foo/
+-rw-r--r--   0 mdurant    (502) staff       (20)      544 2023-02-23 03:44:29.000000 intake-0.7.0/intake/source/tests/plugin_searchpath/intake_foo/__init__.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.317824 intake-0.7.0/intake/source/tests/plugin_searchpath/not_intake_foo/
+-rw-r--r--   0 mdurant    (502) staff       (20)      549 2023-02-23 03:44:29.000000 intake-0.7.0/intake/source/tests/plugin_searchpath/not_intake_foo/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4330 2023-05-17 00:57:11.000000 intake-0.7.0/intake/source/textfiles.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4376 2023-05-29 19:06:25.000000 intake-0.7.0/intake/source/tiled.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9787 2023-05-17 00:57:11.000000 intake-0.7.0/intake/source/utils.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2974 2023-05-23 02:32:42.000000 intake-0.7.0/intake/source/zarr.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1756 2023-05-17 00:57:11.000000 intake-0.7.0/intake/util_tests.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9337 2023-05-17 00:57:11.000000 intake-0.7.0/intake/utils.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.294934 intake-0.7.0/intake.egg-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)     3184 2023-05-29 19:22:32.000000 intake-0.7.0/intake.egg-info/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     3466 2023-05-29 19:22:32.000000 intake-0.7.0/intake.egg-info/SOURCES.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-05-29 19:22:32.000000 intake-0.7.0/intake.egg-info/dependency_links.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      762 2023-05-29 19:22:32.000000 intake-0.7.0/intake.egg-info/entry_points.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-09-21 20:58:10.000000 intake-0.7.0/intake.egg-info/not-zip-safe
+-rw-r--r--   0 mdurant    (502) staff       (20)      346 2023-05-29 19:22:32.000000 intake-0.7.0/intake.egg-info/requires.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        7 2023-05-29 19:22:32.000000 intake-0.7.0/intake.egg-info/top_level.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      304 2023-02-23 03:44:29.000000 intake-0.7.0/pyproject.toml
+-rw-r--r--   0 mdurant    (502) staff       (20)       74 2023-02-15 12:19:41.000000 intake-0.7.0/requirements.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      290 2023-05-29 19:22:32.321175 intake-0.7.0/setup.cfg
+-rw-r--r--   0 mdurant    (502) staff       (20)     2995 2023-02-23 03:44:29.000000 intake-0.7.0/setup.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.318042 intake-0.7.0/templates/
+-rw-r--r--   0 mdurant    (502) staff       (20)      529 2022-09-18 01:28:48.000000 intake-0.7.0/templates/README.md
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.318326 intake-0.7.0/templates/data_package/
+-rw-r--r--   0 mdurant    (502) staff       (20)      285 2022-09-18 01:28:48.000000 intake-0.7.0/templates/data_package/cookiecutter.json
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.319562 intake-0.7.0/templates/data_package/hooks/
+-rw-r--r--   0 mdurant    (502) staff       (20)      747 2023-02-23 03:44:29.000000 intake-0.7.0/templates/data_package/hooks/post_gen_project.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 19:22:32.320375 intake-0.7.0/templates/data_package/{{cookiecutter.package_name}}/
+-rw-r--r--   0 mdurant    (502) staff       (20)      333 2022-09-18 01:28:48.000000 intake-0.7.0/templates/data_package/{{cookiecutter.package_name}}/build.sh
+-rw-r--r--   0 mdurant    (502) staff       (20)      521 2023-02-23 03:44:29.000000 intake-0.7.0/templates/data_package/{{cookiecutter.package_name}}/meta.yaml
+-rw-r--r--   0 mdurant    (502) staff       (20)      210 2022-09-18 01:28:48.000000 intake-0.7.0/templates/data_package/{{cookiecutter.package_name}}/{{cookiecutter.dataset_name}}.yaml
+-rw-r--r--   0 mdurant    (502) staff       (20)    67803 2023-02-23 03:44:29.000000 intake-0.7.0/versioneer.py
```

### Comparing `intake-0.6.8/LICENSE` & `intake-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/MANIFEST.in` & `intake-0.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/PKG-INFO` & `intake-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake
-Version: 0.6.8
+Version: 0.7.0
 Summary: Data load and catalog system
 Home-page: https://github.com/intake/intake
 Maintainer: Martin Durant
 Maintainer-email: mdurant@anaconda.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `intake-0.6.8/README.md` & `intake-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/__init__.py` & `intake-0.7.0/intake/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,17 +57,26 @@
         logger.debug("Importing: %s" % modname)
         mod = importlib.import_module(modname)
         if ":" in dest:
             mod = getattr(mod, dest.split(":")[1])
         gl[attr] = mod
         return mod
 
-    if attr[:5] == "open_" and attr[5:] in registry.drivers.enabled_plugins():
-        driver = registry[attr[5:]]  # "open_..."
-        return driver
+    if attr[:5] == "open_":
+        if attr[5:] in registry.drivers.enabled_plugins():
+            driver = registry[attr[5:]]  # "open_..."
+            return driver
+        else:
+            registered_methods = [f"open_{driver}" for driver in registry.drivers.enabled_plugins()]
+            raise AttributeError(
+                f"Unknown open method '{attr}'. "
+                "Do you need to install a new driver from the plugin directory? "
+                "https://intake.readthedocs.io/en/latest/plugin-directory.html\n"
+                f"Registered opener methods: {registered_methods}"
+            )
 
     raise AttributeError(attr)
 
 
 def __dir__(*_, **__):
     openers = ["open_" + name for name in registry.drivers.enabled_plugins()]
     return sorted(list(globals()) + list(imports) + openers)
@@ -141,9 +150,14 @@
                 raise ValueError("URI not understood: %s" % uri)
         else:
             # empty cat
             driver = "catalog"
     if "_file" not in driver:
         kwargs.pop("fs", None)
     if driver not in registry:
-        raise ValueError("Unknown catalog driver (%s), supply one of: %s" % (driver, list(sorted(registry))))
+        raise ValueError(
+            f"Unknown catalog driver '{driver}'. "
+            "Do you need to install a new driver from the plugin directory? "
+            "https://intake.readthedocs.io/en/latest/plugin-directory.html\n"
+            f"Current registry: {list(sorted(registry))}"
+        )
     return registry[driver](uri, **kwargs)
```

### Comparing `intake-0.6.8/intake/auth/base.py` & `intake-0.7.0/intake/auth/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         self.args = args
 
     def __dask_tokenize__(self):
         return hash(self)
 
     @property
     def _tok(self):
-        from dask.base import tokenize
+        from intake.source.utils import tokenize
 
         return tokenize({"cls": type(self).__name__, "args": self.args})
 
     def __hash__(self):
         return int(self._tok, 16)
 
     def get_headers(self):
```

### Comparing `intake-0.6.8/intake/auth/secret.py` & `intake-0.7.0/intake/auth/secret.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/catalog/__init__.py` & `intake-0.7.0/intake/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/catalog/base.py` & `intake-0.7.0/intake/catalog/base.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/catalog/default.py` & `intake-0.7.0/intake/catalog/default.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/catalog/entry.py` & `intake-0.7.0/intake/catalog/entry.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/catalog/exceptions.py` & `intake-0.7.0/intake/catalog/exceptions.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/catalog/gui.py` & `intake-0.7.0/intake/catalog/gui.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/catalog/local.py` & `intake-0.7.0/intake/catalog/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -814,17 +814,22 @@
             "module_name": self._entrypoint.module_name,
             "object_name": self._entrypoint.object_name,
             "distro": self._entrypoint.distro,
             "extras": self._entrypoint.extras,
             "container": self._container,
         }
 
-    def get(self):
+    def __call__(self, **kwargs):
         """Instantiate the DataSource for the given parameters"""
-        return self._entrypoint.load()
+        source = self._entrypoint.load()
+        if kwargs:
+            source = source.configure_new(**kwargs)
+        return source
+
+    get = __call__
 
 
 class EntrypointsCatalog(Catalog):
     """
     A catalog of discovered entrypoint catalogs.
     """
```

### Comparing `intake-0.6.8/intake/catalog/remote.py` & `intake-0.7.0/intake/catalog/remote.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/catalog/utils.py` & `intake-0.7.0/intake/catalog/utils.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/catalog/zarr.py` & `intake-0.7.0/intake/catalog/zarr.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/cli/bootstrap.py` & `intake-0.7.0/intake/cli/bootstrap.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/cli/client/__main__.py` & `intake-0.7.0/intake/cli/client/__main__.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/cli/client/subcommands/__init__.py` & `intake-0.7.0/intake/cli/client/subcommands/__init__.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/cli/client/subcommands/cache.py` & `intake-0.7.0/intake/cli/client/subcommands/cache.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/cli/client/subcommands/config.py` & `intake-0.7.0/intake/cli/client/subcommands/config.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/cli/client/subcommands/describe.py` & `intake-0.7.0/intake/cli/client/subcommands/describe.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/cli/client/subcommands/discover.py` & `intake-0.7.0/intake/cli/client/subcommands/discover.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/cli/client/subcommands/drivers.py` & `intake-0.7.0/intake/cli/client/subcommands/drivers.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/cli/client/subcommands/example.py` & `intake-0.7.0/intake/cli/client/subcommands/example.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/cli/client/subcommands/exists.py` & `intake-0.7.0/intake/cli/client/subcommands/exists.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/cli/client/subcommands/get.py` & `intake-0.7.0/intake/cli/client/subcommands/get.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/cli/client/subcommands/info.py` & `intake-0.7.0/intake/cli/client/subcommands/info.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/cli/client/subcommands/list.py` & `intake-0.7.0/intake/cli/client/subcommands/list.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/cli/client/subcommands/precache.py` & `intake-0.7.0/intake/cli/client/subcommands/precache.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/cli/sample/states_1.csv` & `intake-0.7.0/intake/cli/sample/states_1.csv`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/cli/sample/states_2.csv` & `intake-0.7.0/intake/cli/sample/states_2.csv`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/cli/server/__main__.py` & `intake-0.7.0/intake/cli/server/__main__.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/cli/server/server.py` & `intake-0.7.0/intake/cli/server/server.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/cli/server/templates/index.html` & `intake-0.7.0/intake/cli/server/templates/index.html`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/cli/util.py` & `intake-0.7.0/intake/cli/util.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/compat.py` & `intake-0.7.0/intake/compat.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/config.py` & `intake-0.7.0/intake/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,18 @@
 
 import logging
 import os
 import posixpath
 from os.path import expanduser
 
 import yaml
+from fsspec.implementations.local import make_path_posix
 
 from intake.utils import yaml_load
 
-from .utils import make_path_posix
-
 logger = logging.getLogger("intake")
 
 confdir = make_path_posix(os.getenv("INTAKE_CONF_DIR", os.path.join(expanduser("~"), ".intake")))
 
 
 defaults = {
     "auth": {"cls": "intake.auth.base.BaseAuth"},
```

### Comparing `intake-0.6.8/intake/conftest.py` & `intake-0.7.0/intake/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 #
 # The full license is in the LICENSE file, distributed with this software.
 # -----------------------------------------------------------------------------
 
 import os
 import posixpath
 import subprocess
+import sys
 import tempfile
 import time
 
 import pytest
 import requests
+from fsspec.implementations.local import make_path_posix
 
 from intake import config, open_catalog, register_driver
 from intake.container import persist
 from intake.source.base import DataSource, Schema
 from intake.tests.test_utils import copy_test_file
 from intake.util_tests import PY2, ex
-from intake.utils import make_path_posix
 
 here = os.path.dirname(__file__)
 
 
 MIN_PORT = 7480
 MAX_PORT = 7489
 PORT = MIN_PORT
@@ -138,17 +139,17 @@
         p.kill()
 
 
 @pytest.fixture(scope="module")
 def http_server():
     port_as_str = str(pick_port())
     if PY2:
-        cmd = ["python", "-m", "SimpleHTTPServer", port_as_str]
+        cmd = [sys.executable, "-m", "SimpleHTTPServer", port_as_str]
     else:
-        cmd = ["python", "-m", "http.server", port_as_str]
+        cmd = [sys.executable, "-m", "http.server", port_as_str]
     p = subprocess.Popen(cmd, cwd=os.path.join(here, "catalog", "tests"))
     url = "http://localhost:{}/".format(port_as_str)
     timeout = 5
     while True:
         try:
             requests.get(url)
             break
```

### Comparing `intake-0.6.8/intake/container/__init__.py` & `intake-0.7.0/intake/container/__init__.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/container/base.py` & `intake-0.7.0/intake/container/base.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/container/dataframe.py` & `intake-0.7.0/intake/container/dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -----------------------------------------------------------------------------
 # Copyright (c) 2012 - 2018, Anaconda, Inc. and Intake contributors
 # All rights reserved.
 #
 # The full license is in the LICENSE file, distributed with this software.
 # -----------------------------------------------------------------------------
+from fsspec import open_files
 from packaging.version import Version
 
 from intake.source.base import DataSource, Schema
 
 from .base import RemoteSource, get_partition
 
 
@@ -84,15 +85,15 @@
         try:
             from intake_parquet import ParquetSource
         except ImportError:
             raise ImportError("Please install intake-parquet to use persistence" " on dataframe container sources.")
         if not hasattr(df, "npartitions"):
             df = dd.from_pandas(df, npartitions=1)
         df.to_parquet(path, **kwargs)
-        source = ParquetSource(path, meta={})
+        source = ParquetSource(path)
         return source
 
 
 def is_dataframe_like(df):
     """Looks like a Pandas DataFrame
 
     Copied from dask.utils
@@ -133,15 +134,14 @@
         super().__init__(metadata=kwargs.pop("metadata", {}))
         self.kwargs = kwargs
         self.dataframe = None
 
     def _load_metadata(self):
         import dask.dataframe as dd
         import dask.delayed
-        from fsspec import open_files
 
         self.files = open_files(self.url, **self.storage_options)
 
         def read_a_file(open_file, reader, kwargs):
             with open_file as of:
                 df = reader(of, **kwargs)
                 df["path"] = open_file.path
```

### Comparing `intake-0.6.8/intake/container/ndarray.py` & `intake-0.7.0/intake/container/ndarray.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/container/persist.py` & `intake-0.7.0/intake/container/persist.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,21 @@
 # The full license is in the LICENSE file, distributed with this software.
 # -----------------------------------------------------------------------------
 
 import posixpath
 import time
 
 import yaml
+from fsspec import filesystem
+from fsspec.core import split_protocol
 
 from ..catalog.local import CatalogEntry, YAMLFileCatalog
 from ..config import conf, logger
 from ..source import DataSource, import_name
+from ..source.utils import tokenize
 from ..utils import make_path_posix
 
 
 class PersistStore(YAMLFileCatalog):
     """
     Specialised catalog for persisted data-sources
     """
@@ -29,17 +32,14 @@
             o = object.__new__(cls)
             o._captured_init_args = args
             o._captured_init_kwargs = kwargs
             cls._singleton[0] = o
         return cls._singleton[0]
 
     def __init__(self, path=None, **storage_options):
-        from fsspec import filesystem
-        from fsspec.core import split_protocol
-
         self.pdir = make_path_posix(path or conf.get("persist_path"))
         protocol, _ = split_protocol(self.pdir)
         path = posixpath.join(self.pdir, "cat.yaml")
         self.fs = filesystem(protocol, **storage_options)
         super(PersistStore, self).__init__(path)
 
     def _load(self):
@@ -53,15 +53,15 @@
         except Exception:
             # if destination doesn't load, we have no entries
             # likely will get exceptions if try to persist
             self._entries = {}
 
     def getdir(self, source):
         """Clear/create a directory to store a persisted dataset into"""
-        from dask.base import tokenize
+        from intake.source.utils import tokenize
 
         subdir = posixpath.join(self.pdir, tokenize(source))
         try:
             self.fs.rm(subdir, True)
         except Exception as e:
             logger.debug("Directory clear failed: %s" % e)
         self.fs.mkdirs(subdir)
@@ -94,16 +94,14 @@
     def get_tok(self, source):
         """Get string token from object
 
         Strings are assumed to already be a token; if source or entry, see
         if it is a persisted thing ("original_tok" is in its metadata), else
         generate its own token.
         """
-        from dask.base import tokenize
-
         if isinstance(source, str):
             return source
 
         if isinstance(source, CatalogEntry):
             return source._metadata.get("original_tok", tokenize(source))
 
         if isinstance(source, DataSource):
@@ -160,15 +158,15 @@
 
     def needs_refresh(self, source):
         """Has the (persisted) source expired in the store
 
         Will return True if the source is not in the store at all, if it's
         TTL is set to None, or if more seconds have passed than the TTL.
         """
-        from dask.base import tokenize
+        from intake.source.utils import tokenize
 
         now = time.time()
         token = tokenize(source)
         if token in self:
             s0 = self[token]
             if self[token].metadata.get("ttl", None):
                 then = s0.metadata["timestamp"]
```

### Comparing `intake-0.6.8/intake/container/semistructured.py` & `intake-0.7.0/intake/container/semistructured.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/container/serializer.py` & `intake-0.7.0/intake/container/serializer.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,37 +60,46 @@
 
     def encode(self, obj, container):
         if container in ["ndarray", "xarray"] and msgpack_numpy:
             from ..compat import np_pack_kwargs
 
             return msgpack.packb(obj, **np_pack_kwargs)
         elif container == "dataframe":
+            pickle.dumps(obj)
             # Use pyarrow for serializing DataFrames, rather than
             # msgpack: https://github.com/intake/intake/issues/460
             pa = check_pyarrow()
 
-            context = pa.default_serialization_context()
-            # This eventually goes to msgpack.packb, which doesn't
-            # directly accept PyArrow Buffer objects. Need to wrap
-            # it in a memoryview to avoid a TypeError.
-            return memoryview(context.serialize(obj).to_buffer())
+            if pa.__version__.split(".") < [
+                "12",
+            ]:
+                context = pa.default_serialization_context()
+                # This eventually goes to msgpack.packb, which doesn't
+                # directly accept PyArrow Buffer objects. Need to wrap
+                # it in a memoryview to avoid a TypeError.
+                return memoryview(context.serialize(obj).to_buffer())
+            return memoryview(pa.serialize_pandas(obj))
         else:
             return msgpack.packb(obj, **pack_kwargs)
 
     def decode(self, bytestr, container):
         from ..compat import unpack_kwargs
 
         if container in ["ndarray", "xarray"] and msgpack_numpy:
             from ..compat import np_unpack_kwargs
 
             return msgpack.unpackb(bytestr, **np_unpack_kwargs)
         elif container == "dataframe":
             pa = check_pyarrow()
-            context = pa.default_serialization_context()
-            return context.deserialize(bytestr)
+            if pa.__version__.split(".") < [
+                "12",
+            ]:
+                context = pa.default_serialization_context()
+                return context.deserialize(bytestr)
+            return pa.deserialize_pandas(bytestr)
         else:
             return msgpack.unpackb(bytestr, **unpack_kwargs)
 
 
 class PickleSerializer(object):
     def __init__(self, protocol_level):
         self._protocol_level = protocol_level
```

### Comparing `intake-0.6.8/intake/interface/__init__.py` & `intake-0.7.0/intake/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/interface/base.py` & `intake-0.7.0/intake/interface/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,16 @@
         new_options = {k: v for k, v in self.options.items() if v not in items}
         self.widget.options = new_options
         self.widget.param.trigger("options")
 
     @property
     def selected(self):
         """Value selected on the widget"""
-        return self.widget.value
+        ops = self.widget.options
+        return [val for val in self.widget.value if (val in ops.values() if isinstance(ops, dict) else val in ops)]
 
     @selected.setter
     def selected(self, new):
         """Set selected from list or instance of object or name.
 
         Over-writes existing selection
         """
```

### Comparing `intake-0.6.8/intake/interface/catalog/add.py` & `intake-0.7.0/intake/interface/catalog/add.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/interface/catalog/gui.py` & `intake-0.7.0/intake/interface/catalog/gui.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/interface/catalog/search.py` & `intake-0.7.0/intake/interface/catalog/search.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/interface/catalog/select.py` & `intake-0.7.0/intake/interface/catalog/select.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/interface/conftest.py` & `intake-0.7.0/intake/interface/conftest.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/interface/gui.py` & `intake-0.7.0/intake/interface/gui.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/interface/icons/logo.png` & `intake-0.7.0/intake/interface/icons/logo.png`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/interface/server.py` & `intake-0.7.0/intake/interface/server.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/interface/source/defined_plots.py` & `intake-0.7.0/intake/interface/source/defined_plots.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/interface/source/description.py` & `intake-0.7.0/intake/interface/source/description.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/interface/source/gui.py` & `intake-0.7.0/intake/interface/source/gui.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/interface/source/select.py` & `intake-0.7.0/intake/interface/source/select.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/source/__init__.py` & `intake-0.7.0/intake/source/__init__.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/source/base.py` & `intake-0.7.0/intake/source/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 Base classes for Data Loader interface
 """
 
 from yaml import dump
 
 from ..utils import DictSerialiseMixin, make_path_posix, pretty_describe
 from .cache import make_caches
+from .utils import tokenize
 
 
 class Schema(dict):
     """Holds details of data description for any type of data-source
 
     This should always be pickleable, so that it can be sent from a server
     to a client, and contain all information needed to recreate a RemoteSource
@@ -46,15 +47,18 @@
 
 
 class NoEntry(AttributeError):
     pass
 
 
 class CacheMixin:
-    """Allows "old style" caching for Data Source"""
+    """Allows "old style" caching for Data Source
+
+    NOTE: to be removed
+    """
 
     _cache = None
 
     @property
     def cache_dirs(self):
         return [c._cache_dir for c in self.cache]
 
@@ -171,29 +175,25 @@
         return super().__call__(*args, **kwargs)
 
 
 class PersistMixin:
     """Adds interaction with PersistStore to DataSource"""
 
     def get_persisted(self):
-        from dask.base import tokenize
-
         from ..container.persist import store
 
         return store[tokenize(self)]()
 
     @staticmethod
     def _persist(source, path, **kwargs):
         """To be implemented by 'container' sources for locally persisting"""
         raise NotImplementedError
 
     @property
     def has_been_persisted(self):
-        from dask.base import tokenize
-
         from ..container.persist import store
 
         return tokenize(self) in store
 
     @property
     def is_persisted(self):
         from ..container.persist import store
@@ -208,16 +208,14 @@
         ttl: numeric, optional
             Time to live in seconds. If provided, the original source will
             be accessed and a new persisted version written transparently
             when more than ``ttl`` seconds have passed since the old persisted
             version was written.
         kargs: passed to the _persist method on the base container.
         """
-        from dask.base import tokenize
-
         from ..container.persist import PersistStore
 
         if "original_tok" in self.metadata:
             raise ValueError("Cannot persist a source taken from the persist " "store")
         if ttl is not None and not isinstance(ttl, (int, float)):
             raise ValueError("Cannot persist using a time to live that is " f"non-numeric. User-provided ttl was {ttl}")
         store = PersistStore()
@@ -265,14 +263,20 @@
     def _get_partition(self, i):
         """Subclasses should return a container object for this partition
 
         This function will never be called with an out-of-range value for i.
         """
         raise NotImplementedError
 
+    def __eq__(self, other):
+        return type(self) is type(other) and self._captured_init_args == other._captured_init_args and self._captured_init_kwargs == other._captured_init_kwargs
+
+    def __hash__(self):
+        return hash((type(self), str(self._captured_init_args), str(self._captured_init_kwargs)))
+
     def _close(self):
         """Subclasses should close all open resources"""
         raise NotImplementedError
 
     def _load_metadata(self):
         """load metadata only if needed"""
         if self._schema is None:
@@ -429,16 +433,14 @@
         representation (``.yaml()``).
         """
         return self._export(path, **kwargs)
 
     def _export(self, path, **kwargs):
         import time
 
-        from dask.base import tokenize
-
         from ..container import container_map
 
         method = container_map[self.container]._persist
         # may need to create path - access file-system method
         out = method(self, path=path, **kwargs)
         out.description = self.description
         metadata = {
```

### Comparing `intake-0.6.8/intake/source/cache.py` & `intake-0.7.0/intake/source/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,21 @@
 import collections
 import json
 import logging
 import os
 import posixpath
 import re
 import shutil
+import subprocess
 import warnings
 from datetime import datetime
 from hashlib import md5
 
+from fsspec import open_files
+
 from intake.config import conf
 from intake.utils import is_notebook, make_path_posix
 
 logger = logging.getLogger("intake")
 
 
 def sanitize_path(path):
@@ -310,16 +313,14 @@
     """Cache specific set of files
 
     Input is a single file URL, URL with glob characters or list of URLs. Output
     is a specific set of local files.
     """
 
     def _make_files(self, urlpath, **kwargs):
-        from fsspec import open_files
-
         self._ensure_cache_dir()
         if isinstance(urlpath, (list, tuple)):
             subdir = self._hash(":".join(urlpath))
         else:
             subdir = self._hash(urlpath)
         files_in = open_files(urlpath, "rb", **self._storage_options)
         files_out = [open_files([self._path(f.path, subdir)], "wb", **self._storage_options)[0] for f in files_in]
@@ -334,16 +335,14 @@
 
     Input is a directory root URL, plus a ``depth`` parameter for how many
     levels of subdirectories to search. All regular files will be copied. Output
     is the resultant local directory tree.
     """
 
     def _make_files(self, urlpath, **kwargs):
-        from fsspec import open_files
-
         self._ensure_cache_dir()
         subdir = self._hash(urlpath)
         depth = self._spec["depth"]
         files_in = []
         for i in range(1, depth + 1):
             files_in.extend(open_files("/".join([urlpath] + ["*"] * i)))
         files_out = [open_files([self._path(f.path, subdir)], "wb", **self._storage_options)[0] for f in files_in]
@@ -379,16 +378,14 @@
     Output is the list of extracted files.
     """
 
     def _make_files(self, urlpath, **kwargs):
         import tempfile
 
         d = tempfile.mkdtemp()
-        from fsspec import open_files
-
         self._ensure_cache_dir()
         self._urlpath = urlpath
         files_in = open_files(urlpath, "rb", **self._storage_options)
         files_out = [open_files([make_path_posix(os.path.join(d, os.path.basename(f.path)))], "wb")[0] for f in files_in]
         super(CompressedCache, self)._load(files_in, files_out, urlpath, meta=False)
         return files_in, files_out
 
@@ -450,18 +447,14 @@
     """
 
     def _make_files(self, urlpath, **kwargs):
         self._ensure_cache_dir()
         return None, None
 
     def _load(self, _, __, urlpath, meta=True):
-        import subprocess
-
-        from fsspec import open_files
-
         path = os.path.join(self._cache_dir, self._hash(urlpath))
         dat, part = os.path.split(urlpath)
         cmd = ["dat", "clone", dat, path, "--no-watch"]
         try:
             subprocess.call(cmd, stdout=subprocess.PIPE)
         except (IOError, OSError):  # pragma: no cover
             logger.info("Calling DAT failed")
```

### Comparing `intake-0.6.8/intake/source/decompress.py` & `intake-0.7.0/intake/source/decompress.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/source/discovery.py` & `intake-0.7.0/intake/source/discovery.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/source/jsonfiles.py` & `intake-0.7.0/intake/source/jsonfiles.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/source/npy.py` & `intake-0.7.0/intake/source/npy.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/source/tests/plugin_searchpath/intake_foo/__init__.py` & `intake-0.7.0/intake/source/tests/plugin_searchpath/intake_foo/__init__.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/source/tests/plugin_searchpath/not_intake_foo/__init__.py` & `intake-0.7.0/intake/source/tests/plugin_searchpath/not_intake_foo/__init__.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/source/textfiles.py` & `intake-0.7.0/intake/source/textfiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         return base.Schema(dtype=None, shape=(None,), npartitions=self.npartitions, extra_metadata=self.metadata)
 
     def _get_partition(self, i):
         return get_file(self._files[i], self.decoder, self._read)
 
     def read(self):
         self._get_schema()
-        return self.to_dask().compute()
+        return [line for i in range(len(self._files)) for line in self._get_partition(i)]
 
     def to_spark(self):
         from intake_spark.base import SparkHolder
 
         h = SparkHolder(False, [("textFile", (self._urlpath,))], {})
         return h.setup()
```

### Comparing `intake-0.6.8/intake/source/tiled.py` & `intake-0.7.0/intake/source/tiled.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake/source/utils.py` & `intake-0.7.0/intake/source/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # -----------------------------------------------------------------------------
 # Copyright (c) 2012 - 2018, Anaconda, Inc. and Intake contributors
 # All rights reserved.
 #
 # The full license is in the LICENSE file, distributed with this software.
 # -----------------------------------------------------------------------------
+from hashlib import md5
 
-from packaging.version import Version
+from ..utils import make_path_posix
 
-try:
-    import dask
 
-    DASK_VERSION = Version(dask.__version__)
-except ImportError:
-    DASK_VERSION = None
-from ..utils import make_path_posix
+def tokenize(*args, **kwargs):
+    """Deterministic token
+
+    copied from dask
+    """
+    hasher = md5(str(tuple(args)).encode())
+    if kwargs:
+        hasher.update(str(args).encode())
+    return hasher.hexdigest()
 
 
 def _validate_format_spec(format_spec):
     if not format_spec:
-        raise ValueError(("Format specifier must be set if " "no separator between fields."))
+        raise ValueError("Format specifier must be set if " "no separator between fields.")
     if format_spec[-1].isalpha():
         format_spec = format_spec[:-1]
     if not format_spec.isdigit():
         raise ValueError("Format specifier must have a set width")
     return int(format_spec)
```

### Comparing `intake-0.6.8/intake/source/zarr.py` & `intake-0.7.0/intake/source/zarr.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,49 +32,51 @@
             Location of data file(s), possibly including protocol
             information
         storage_options : dict
             Passed on to storage backend for remote files
         component : str or None
             If None, assume the URL points to an array. If given, assume
             the URL points to a group, and descend the group to find the
-            array at this location in the hierarchy.
+            array at this location in the hierarchy; components are separated
+            by the "/" character.
         kwargs : passed on to dask.array.from_zarr
         """
         self.urlpath = urlpath
         self.storage_options = storage_options or {}
         self.component = component
         self.kwargs = kwargs
         self.chunks = None
         self._arr = None
         super(ZarrArraySource, self).__init__(metadata=metadata)
 
     def _get_schema(self):
-        import dask.array as da
+        import zarr
 
         if self._arr is None:
-            self._arr = da.from_zarr(self.urlpath, component=self.component, storage_options=self.storage_options, **self.kwargs)
+            self._arr = zarr.open(self.urlpath, storage_options=self.storage_options)
+            if self.component:
+                comp = self.component.split("/")
+                for sub in comp:
+                    self._arr = self._arr[sub]
             self.chunks = self._arr.chunks
             self.shape = self._arr.shape
             self.dtype = self._arr.dtype
-            self.npartitions = self._arr.npartitions
+            self.npartitions = self._arr.nchunks
         return Schema(dtype=str(self.dtype), shape=self.shape, extra_metadata=self.metadata, npartitions=self.npartitions, chunks=self.chunks)
 
-    def _get_partition(self, i):
-        if isinstance(i, list):
-            i = tuple(i)
-        return self._arr.blocks[i].compute()
-
     def read_partition(self, i):
         self._get_schema()
-        return self._get_partition(i)
+        chunks = self._arr.chunks
+        sel = tuple(slice(ch * j, ch * (j + 1), None) for ch, j in zip(chunks, i))
+        return self._arr.__getitem__(sel)
 
     def to_dask(self):
-        self._get_schema()
-        return self._arr
+        import dask.array as da
+
+        return da.from_zarr(self.urlpath, component=self.component, storage_options=self.storage_options, **self.kwargs)
 
     def read(self):
         self._get_schema()
-        return self._arr.compute()
+        return self._arr[:]
 
     def _close(self):
         self._arr = None
-        self._mapper = None
```

### Comparing `intake-0.6.8/intake/util_tests.py` & `intake-0.7.0/intake/util_tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 import sys
 import tempfile
 import time
 from contextlib import contextmanager
 
 import requests
 import yaml
-
-from .utils import make_path_posix
+from fsspec.implementations.local import make_path_posix
 
 ex = sys.executable
 here = os.path.dirname(__file__)
 defcat = make_path_posix(os.path.join(here, "cli", "server", "tests", "catalog1.yml"))
 PY2 = sys.version_info[0] == 2
```

### Comparing `intake-0.6.8/intake/utils.py` & `intake-0.7.0/intake/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from contextlib import contextmanager
 
 import yaml
 
 
 def make_path_posix(path):
     """Make path generic"""
+    # TODO: migrate to fsspec' implementation
     if "://" in path:
         return path
     return path.replace("\\", "/").replace("//", "/")
 
 
 def no_duplicates_constructor(loader, node, deep=False):
     """Check for duplicate keys while loading YAML
@@ -93,17 +94,17 @@
 
     @property
     def classname(self):
         return classname(self)
 
     def __dask_tokenize__(self):
         if self.__tok_cache is None:
-            from dask.base import tokenize
+            from intake.source.utils import tokenize
 
-            self.__tok_cache = tokenize(self.__getstate__())
+            self.__tok_cache = tokenize(self)
         return self.__tok_cache
 
     def __getstate__(self):
         args = [arg.__getstate__() if isinstance(arg, DictSerialiseMixin) else arg for arg in self._captured_init_args]
         # We employ OrderedDict in several places. The motivation
         # is to speed up dask tokenization. When dask tokenizes a plain dict,
         # it sorts the keys, and it turns out that this sort operation
@@ -116,15 +117,15 @@
         # reconstitute instances here
         self._captured_init_kwargs = state["kwargs"]
         self._captured_init_args = state["args"]
         state.pop("cls", None)
         self.__init__(*state["args"], **state["kwargs"])
 
     def __hash__(self):
-        from dask.base import tokenize
+        from intake.source.utils import tokenize
 
         return int(tokenize(self), 16)
 
     def __eq__(self, other):
         return hash(self) == hash(other)
```

### Comparing `intake-0.6.8/intake.egg-info/PKG-INFO` & `intake-0.7.0/intake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake
-Version: 0.6.8
+Version: 0.7.0
 Summary: Data load and catalog system
 Home-page: https://github.com/intake/intake
 Maintainer: Martin Durant
 Maintainer-email: mdurant@anaconda.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `intake-0.6.8/intake.egg-info/SOURCES.txt` & `intake-0.7.0/intake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/intake.egg-info/entry_points.txt` & `intake-0.7.0/intake.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/setup.py` & `intake-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/templates/README.md` & `intake-0.7.0/templates/README.md`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/templates/data_package/hooks/post_gen_project.py` & `intake-0.7.0/templates/data_package/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/templates/data_package/{{cookiecutter.package_name}}/meta.yaml` & `intake-0.7.0/templates/data_package/{{cookiecutter.package_name}}/meta.yaml`

 * *Files identical despite different names*

### Comparing `intake-0.6.8/versioneer.py` & `intake-0.7.0/versioneer.py`

 * *Files identical despite different names*

