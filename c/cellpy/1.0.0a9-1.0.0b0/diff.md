# Comparing `tmp/cellpy-1.0.0a9.tar.gz` & `tmp/cellpy-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellpy-1.0.0a9.tar", last modified: Thu May 25 17:56:35 2023, max compression
+gzip compressed data, was "cellpy-1.0.0b0.tar", last modified: Mon May 29 19:16:23 2023, max compression
```

## Comparing `cellpy-1.0.0a9.tar` & `cellpy-1.0.0b0.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.181958 cellpy-1.0.0a9/
--rw-rw-rw-   0        0        0      503 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/AUTHORS.rst
--rw-rw-rw-   0        0        0     3086 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     4001 2023-05-25 17:55:44.000000 cellpy-1.0.0a9/HISTORY.rst
--rw-rw-rw-   0        0        0     1089 2021-12-21 09:11:58.000000 cellpy-1.0.0a9/LICENSE
--rw-rw-rw-   0        0        0      645 2022-05-27 12:07:50.000000 cellpy-1.0.0a9/MANIFEST.in
--rw-rw-rw-   0        0        0     6767 2023-05-25 17:56:35.180958 cellpy-1.0.0a9/PKG-INFO
--rw-rw-rw-   0        0        0     1872 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.911380 cellpy-1.0.0a9/cellpy/
--rw-rw-rw-   0        0        0      805 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/__init__.py
--rw-rw-rw-   0        0        0       25 2023-05-25 17:56:19.000000 cellpy-1.0.0a9/cellpy/_version.py
--rw-rw-rw-   0        0        0    52893 2023-05-23 14:55:13.000000 cellpy-1.0.0a9/cellpy/cli.py
--rw-rw-rw-   0        0        0     1228 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.924379 cellpy-1.0.0a9/cellpy/internals/
--rw-rw-rw-   0        0        0        0 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/internals/__init__.py
--rw-rw-rw-   0        0        0    27994 2023-05-06 21:51:58.000000 cellpy-1.0.0a9/cellpy/internals/core.py
--rw-rw-rw-   0        0        0     4838 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/log.py
--rw-rw-rw-   0        0        0     1750 2021-12-21 09:11:58.000000 cellpy-1.0.0a9/cellpy/logging.json
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.931380 cellpy-1.0.0a9/cellpy/parameters/
--rw-rw-rw-   0        0        0     3183 2023-05-02 11:51:31.000000 cellpy-1.0.0a9/cellpy/parameters/.cellpy_prms_default.conf
--rw-rw-rw-   0        0        0        2 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/parameters/__init__.py
--rw-rw-rw-   0        0        0    23452 2023-05-14 17:34:31.000000 cellpy-1.0.0a9/cellpy/parameters/internal_settings.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.934380 cellpy-1.0.0a9/cellpy/parameters/legacy/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a9/cellpy/parameters/legacy/__init__.py
--rw-rw-rw-   0        0        0    24146 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/parameters/legacy/update_headers.py
--rw-rw-rw-   0        0        0    12261 2023-05-23 14:50:48.000000 cellpy-1.0.0a9/cellpy/parameters/prmreader.py
--rw-rw-rw-   0        0        0    12220 2023-05-02 11:49:22.000000 cellpy-1.0.0a9/cellpy/parameters/prms.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.943380 cellpy-1.0.0a9/cellpy/readers/
--rw-rw-rw-   0        0        0        2 2021-12-21 09:11:58.000000 cellpy-1.0.0a9/cellpy/readers/__init__.py
--rw-rw-rw-   0        0        0   235011 2023-05-25 17:44:20.000000 cellpy-1.0.0a9/cellpy/readers/cellreader.py
--rw-rw-rw-   0        0        0    38338 2023-05-25 16:54:28.000000 cellpy-1.0.0a9/cellpy/readers/core.py
--rw-rw-rw-   0        0        0    22998 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/dbreader.py
--rw-rw-rw-   0        0        0    13825 2023-05-06 21:51:58.000000 cellpy-1.0.0a9/cellpy/readers/filefinder.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.966380 cellpy-1.0.0a9/cellpy/readers/instruments/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a9/cellpy/readers/instruments/__init__.py
--rw-rw-rw-   0        0        0    49052 2023-05-12 17:21:48.000000 cellpy-1.0.0a9/cellpy/readers/instruments/arbin_res.py
--rw-rw-rw-   0        0        0    19381 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/arbin_sql.py
--rw-rw-rw-   0        0        0    21062 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/arbin_sql_7.py
--rw-rw-rw-   0        0        0    11134 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/arbin_sql_csv.py
--rw-rw-rw-   0        0        0     7126 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/arbin_sql_h5.py
--rw-rw-rw-   0        0        0     9883 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/arbin_sql_xlsx.py
--rw-rw-rw-   0        0        0    27324 2023-05-09 19:57:46.000000 cellpy-1.0.0a9/cellpy/readers/instruments/base.py
--rw-rw-rw-   0        0        0    22693 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/biologics_mpr.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.976379 cellpy-1.0.0a9/cellpy/readers/instruments/configurations/
--rw-rw-rw-   0        0        0     6607 2022-06-03 19:58:41.000000 cellpy-1.0.0a9/cellpy/readers/instruments/configurations/__init__.py
--rw-rw-rw-   0        0        0     1700 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/configurations/maccor_txt_four.py
--rw-rw-rw-   0        0        0     4084 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/configurations/maccor_txt_one.py
--rw-rw-rw-   0        0        0     1990 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/configurations/maccor_txt_three.py
--rw-rw-rw-   0        0        0     1788 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/configurations/maccor_txt_two.py
--rw-rw-rw-   0        0        0     3549 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/configurations/maccor_txt_zero.py
--rw-rw-rw-   0        0        0     2132 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/configurations/neware_txt_zero.py
--rw-rw-rw-   0        0        0    10327 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/custom.py
--rw-rw-rw-   0        0        0     3760 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/ext_nda_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.979380 cellpy-1.0.0a9/cellpy/readers/instruments/loader_specific_modules/
--rw-rw-rw-   0        0        0        0 2022-06-03 19:58:41.000000 cellpy-1.0.0a9/cellpy/readers/instruments/loader_specific_modules/__init__.py
--rw-rw-rw-   0        0        0    22115 2022-06-03 19:58:41.000000 cellpy-1.0.0a9/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py
--rw-rw-rw-   0        0        0     1067 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/local_instrument.py
--rw-rw-rw-   0        0        0    12886 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/maccor_txt.py
--rw-rw-rw-   0        0        0     3488 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/neware_txt.py
--rw-rw-rw-   0        0        0    16769 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/pec_csv.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.984379 cellpy-1.0.0a9/cellpy/readers/instruments/processors/
--rw-rw-rw-   0        0        0        0 2022-05-27 12:07:50.000000 cellpy-1.0.0a9/cellpy/readers/instruments/processors/__init__.py
--rw-rw-rw-   0        0        0    15265 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/processors/post_processors.py
--rw-rw-rw-   0        0        0     1450 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/processors/pre_processors.py
--rw-rw-rw-   0        0        0    26852 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/sql_dbreader.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.007380 cellpy-1.0.0a9/cellpy/utils/
--rw-rw-rw-   0        0        0      192 2021-12-21 09:11:58.000000 cellpy-1.0.0a9/cellpy/utils/__init__.py
--rw-rw-rw-   0        0        0    48182 2023-05-03 09:31:40.000000 cellpy-1.0.0a9/cellpy/utils/batch.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.027387 cellpy-1.0.0a9/cellpy/utils/batch_tools/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/__init__.py
--rw-rw-rw-   0        0        0     7578 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_analyzers.py
--rw-rw-rw-   0        0        0    19566 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_core.py
--rw-rw-rw-   0        0        0    40056 2023-05-16 14:17:12.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_experiments.py
--rw-rw-rw-   0        0        0     2931 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_exporters.py
--rw-rw-rw-   0        0        0    14090 2023-05-06 21:51:58.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_helpers.py
--rw-rw-rw-   0        0        0    27683 2023-05-02 13:39:36.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_journals.py
--rw-rw-rw-   0        0        0    29066 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_plotters.py
--rw-rw-rw-   0        0        0      245 2021-12-21 09:11:58.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_reporters.py
--rw-rw-rw-   0        0        0     3339 2022-05-27 12:03:59.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/dumpers.py
--rw-rw-rw-   0        0        0     9872 2023-05-02 10:20:24.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/engines.py
--rw-rw-rw-   0        0        0     5294 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/sqlite_from_excel_db.py
--rw-rw-rw-   0        0        0    63308 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/collectors.py
--rw-rw-rw-   0        0        0    45461 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/collectors_old.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.029379 cellpy-1.0.0a9/cellpy/utils/data/
--rw-rw-rw-   0        0        0  3700143 2023-05-25 17:51:11.000000 cellpy-1.0.0a9/cellpy/utils/data/20160805_test001_45_cc.h5
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.033380 cellpy-1.0.0a9/cellpy/utils/data/raw/
--rw-rw-rw-   0        0        0  1613824 2021-12-21 09:11:58.000000 cellpy-1.0.0a9/cellpy/utils/data/raw/20160805_test001_45_cc_01.res
--rw-rw-rw-   0        0        0      260 2022-05-27 12:07:50.000000 cellpy-1.0.0a9/cellpy/utils/diagnostics.py
--rw-rw-rw-   0        0        0    79016 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/easyplot.py
--rw-rw-rw-   0        0        0     1576 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/example_data.py
--rw-rw-rw-   0        0        0    39446 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/helpers.py
--rw-rw-rw-   0        0        0    38991 2023-05-06 21:51:58.000000 cellpy-1.0.0a9/cellpy/utils/ica.py
--rw-rw-rw-   0        0        0      189 2022-05-27 12:07:50.000000 cellpy-1.0.0a9/cellpy/utils/live.py
--rw-rw-rw-   0        0        0    31653 2023-05-19 21:09:17.000000 cellpy-1.0.0a9/cellpy/utils/ocv_rlx.py
--rw-rw-rw-   0        0        0    45397 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/plotutils.py
--rw-rw-rw-   0        0        0     1787 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/processor.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.921380 cellpy-1.0.0a9/cellpy.egg-info/
--rw-rw-rw-   0        0        0     6767 2023-05-25 17:56:34.000000 cellpy-1.0.0a9/cellpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7846 2023-05-25 17:56:34.000000 cellpy-1.0.0a9/cellpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 17:56:34.000000 cellpy-1.0.0a9/cellpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 17:56:34.000000 cellpy-1.0.0a9/cellpy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-25 17:56:33.000000 cellpy-1.0.0a9/cellpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      337 2023-05-25 17:56:34.000000 cellpy-1.0.0a9/cellpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-25 17:56:34.000000 cellpy-1.0.0a9/cellpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.042889 cellpy-1.0.0a9/docs/
--rw-rw-rw-   0        0        0     6939 2022-09-20 08:21:07.000000 cellpy-1.0.0a9/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.886380 cellpy-1.0.0a9/docs/_build/
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.886380 cellpy-1.0.0a9/docs/_build/.doctrees/
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.049889 cellpy-1.0.0a9/docs/_build/.doctrees/nbsphinx/
--rw-rw-rw-   0        0        0    15014 2023-04-30 13:53:57.000000 cellpy-1.0.0a9/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
--rw-rw-rw-   0        0        0    14599 2023-04-30 13:53:57.000000 cellpy-1.0.0a9/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
--rw-rw-rw-   0        0        0    13527 2023-04-30 13:53:57.000000 cellpy-1.0.0a9/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
--rw-rw-rw-   0        0        0    25669 2023-04-30 13:54:02.000000 cellpy-1.0.0a9/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.079958 cellpy-1.0.0a9/docs/_build/_images/
--rw-rw-rw-   0        0        0    15014 2023-04-27 15:02:55.000000 cellpy-1.0.0a9/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
--rw-rw-rw-   0        0        0    14599 2023-04-27 15:02:55.000000 cellpy-1.0.0a9/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
--rw-rw-rw-   0        0        0    13527 2023-04-27 15:02:55.000000 cellpy-1.0.0a9/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
--rw-rw-rw-   0        0        0    25669 2023-04-27 15:03:02.000000 cellpy-1.0.0a9/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
--rw-rw-rw-   0        0        0    11678 2023-04-29 14:19:31.000000 cellpy-1.0.0a9/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png
--rw-rw-rw-   0        0        0    22040 2023-04-29 14:33:27.000000 cellpy-1.0.0a9/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png
--rw-rw-rw-   0        0        0    21790 2023-04-29 14:26:00.000000 cellpy-1.0.0a9/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png
--rw-rw-rw-   0        0        0    32991 2023-04-29 14:26:01.000000 cellpy-1.0.0a9/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png
--rw-rw-rw-   0        0        0    32991 2023-04-30 20:02:23.000000 cellpy-1.0.0a9/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png
--rw-rw-rw-   0        0        0     7231 2023-04-29 14:12:31.000000 cellpy-1.0.0a9/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png
--rw-rw-rw-   0        0        0    13360 2023-04-29 14:36:26.000000 cellpy-1.0.0a9/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png
--rw-rw-rw-   0        0        0    21790 2023-04-30 20:02:22.000000 cellpy-1.0.0a9/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png
--rw-rw-rw-   0        0        0     5391 2023-04-29 14:10:02.000000 cellpy-1.0.0a9/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png
--rw-rw-rw-   0        0        0    20826 2023-04-29 14:29:06.000000 cellpy-1.0.0a9/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png
--rw-rw-rw-   0        0        0    88743 2023-04-19 13:49:30.000000 cellpy-1.0.0a9/docs/_build/_images/templates_jupyterlab_001.png
--rw-rw-rw-   0        0        0   296908 2022-05-27 12:07:51.000000 cellpy-1.0.0a9/docs/_build/_images/tutorials_utils_plotting_fig1.png
--rw-rw-rw-   0        0        0    54588 2022-05-27 12:07:51.000000 cellpy-1.0.0a9/docs/_build/_images/tutorials_utils_plotting_fig2.png
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.084957 cellpy-1.0.0a9/docs/_build/_static/
--rw-rw-rw-   0        0        0      286 2023-04-25 11:20:36.000000 cellpy-1.0.0a9/docs/_build/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0a9/docs/_build/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0a9/docs/_build/_static/plus.png
--rw-rw-rw-   0        0        0     1695 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/adapted_readme.rst
--rw-rw-rw-   0        0        0    10731 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/conf.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.097958 cellpy-1.0.0a9/docs/developers_guide/
--rw-rw-rw-   0        0        0     1334 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/developers_guide/dev_cellpy_data_structure.rst
--rw-rw-rw-   0        0        0     5904 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/developers_guide/dev_cellpy_folder_structure.rst
--rw-rw-rw-   0        0        0      935 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/developers_guide/dev_cellpy_packaging_pypi.rst
--rw-rw-rw-   0        0        0     3009 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/developers_guide/dev_cellpy_setup.rst
--rw-rw-rw-   0        0        0     1821 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/developers_guide/dev_conda_package.rst
--rw-rw-rw-   0        0        0     2136 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/developers_guide/dev_docs.rst
--rw-rw-rw-   0        0        0     5218 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/developers_guide/dev_loaders_and_instruments.rst
--rw-rw-rw-   0        0        0     1768 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/developers_guide/dev_various.rst
--rw-rw-rw-   0        0        0      326 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/developers_guide/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.106958 cellpy-1.0.0a9/docs/examples_and_tutorials/
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.117958 cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/
--rw-rw-rw-   0        0        0    15786 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst
--rw-rw-rw-   0        0        0     3909 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst
--rw-rw-rw-   0        0        0     5485 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst
--rw-rw-rw-   0        0        0     4465 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst
--rw-rw-rw-   0        0        0     5908 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/05_configuring.rst
--rw-rw-rw-   0        0        0     1052 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/06_pandas.rst
--rw-rw-rw-   0        0        0     1102 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst
--rw-rw-rw-   0        0        0     8224 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst
--rw-rw-rw-   0        0        0      484 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/basics.rst
--rw-rw-rw-   0        0        0      366 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/examples.rst
--rw-rw-rw-   0        0        0      174 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.126958 cellpy-1.0.0a9/docs/examples_and_tutorials/loaders/
--rw-rw-rw-   0        0        0       49 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/loaders/01_arbin.rst
--rw-rw-rw-   0        0        0       52 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/loaders/02_maccor.rst
--rw-rw-rw-   0        0        0       43 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/loaders/03_PEC.rst
--rw-rw-rw-   0        0        0       54 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/loaders/04_Neware.rst
--rw-rw-rw-   0        0        0       62 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/loaders/05_biologics.rst
--rw-rw-rw-   0        0        0       54 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/loaders/06_custom.rst
--rw-rw-rw-   0        0        0      260 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/loaders.rst
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.888380 cellpy-1.0.0a9/docs/examples_and_tutorials/notebooks/
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.129958 cellpy-1.0.0a9/docs/examples_and_tutorials/notebooks/images/
--rw-rw-rw-   0        0        0    88743 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png
--rw-rw-rw-   0        0        0    95663 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png
--rw-rw-rw-   0        0        0      231 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/notebooks.rst
--rw-rw-rw-   0        0        0     1797 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/tips_and_tricks.rst
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.140958 cellpy-1.0.0a9/docs/examples_and_tutorials/utils/
--rw-rw-rw-   0        0        0     4388 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/utils/batch.rst
--rw-rw-rw-   0        0        0       59 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/utils/collectors.rst
--rw-rw-rw-   0        0        0       53 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/utils/easyplot.rst
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.145957 cellpy-1.0.0a9/docs/examples_and_tutorials/utils/figures/
--rw-rw-rw-   0        0        0   296908 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png
--rw-rw-rw-   0        0        0    54588 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png
--rw-rw-rw-   0        0        0     1219 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/utils/ica.rst
--rw-rw-rw-   0        0        0     2063 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/utils/plotting.rst
--rw-rw-rw-   0        0        0      338 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/utils/templates.rst
--rw-rw-rw-   0        0        0     1379 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst
--rw-rw-rw-   0        0        0      371 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/utils.rst
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.148958 cellpy-1.0.0a9/docs/figures/
--rw-rw-rw-   0        0        0     9981 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/figures/cellpy-icon-bw.png
--rw-rw-rw-   0        0        0    10302 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/figures/cellpy-logo-v1.png
--rw-rw-rw-   0        0        0      593 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.160958 cellpy-1.0.0a9/docs/main_description/
--rw-rw-rw-   0        0        0       32 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/main_description/authors.rst
--rw-rw-rw-   0        0        0       37 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/main_description/contributing.rst
--rw-rw-rw-   0        0        0    16327 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/main_description/formats.rst
--rw-rw-rw-   0        0        0       32 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/main_description/history.rst
--rw-rw-rw-   0        0        0      182 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/main_description/index.rst
--rw-rw-rw-   0        0        0     4288 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/main_description/installation.rst
--rw-rw-rw-   0        0        0     3444 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/main_description/usage.rst
--rwxrwxrwx   0        0        0     6701 2022-09-20 08:21:07.000000 cellpy-1.0.0a9/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.179958 cellpy-1.0.0a9/docs/source/
--rw-rw-rw-   0        0        0      367 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/source/cellpy.internals.rst
--rw-rw-rw-   0        0        0      447 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/source/cellpy.parameters.legacy.rst
--rw-rw-rw-   0        0        0      847 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/source/cellpy.parameters.rst
--rw-rw-rw-   0        0        0     1911 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/source/cellpy.readers.instruments.configurations.rst
--rw-rw-rw-   0        0        0      631 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/source/cellpy.readers.instruments.loader_specific_modules.rst
--rw-rw-rw-   0        0        0      783 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/source/cellpy.readers.instruments.processors.rst
--rw-rw-rw-   0        0        0     3413 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/source/cellpy.readers.instruments.rst
--rw-rw-rw-   0        0        0     1139 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/source/cellpy.readers.rst
--rw-rw-rw-   0        0        0      721 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/source/cellpy.rst
--rw-rw-rw-   0        0        0     2610 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/source/cellpy.utils.batch_tools.rst
--rw-rw-rw-   0        0        0     2222 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/source/cellpy.utils.rst
--rw-rw-rw-   0        0        0       62 2023-05-01 10:14:23.000000 cellpy-1.0.0a9/docs/source/modules.rst
--rw-rw-rw-   0        0        0      281 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 17:56:35.181958 cellpy-1.0.0a9/setup.cfg
--rw-rw-rw-   0        0        0     2922 2023-05-12 17:21:47.000000 cellpy-1.0.0a9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.529624 cellpy-1.0.0b0/
+-rw-rw-rw-   0        0        0      503 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3086 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     4001 2023-05-25 17:55:44.000000 cellpy-1.0.0b0/HISTORY.rst
+-rw-rw-rw-   0        0        0     1089 2021-12-21 09:11:58.000000 cellpy-1.0.0b0/LICENSE
+-rw-rw-rw-   0        0        0      645 2022-05-27 12:07:50.000000 cellpy-1.0.0b0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6767 2023-05-29 19:16:23.529624 cellpy-1.0.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0     1872 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.237406 cellpy-1.0.0b0/cellpy/
+-rw-rw-rw-   0        0        0      805 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/__init__.py
+-rw-rw-rw-   0        0        0       24 2023-05-29 19:15:05.000000 cellpy-1.0.0b0/cellpy/_version.py
+-rw-rw-rw-   0        0        0    52885 2023-05-28 20:26:35.000000 cellpy-1.0.0b0/cellpy/cli.py
+-rw-rw-rw-   0        0        0     1228 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.249480 cellpy-1.0.0b0/cellpy/internals/
+-rw-rw-rw-   0        0        0        0 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/internals/__init__.py
+-rw-rw-rw-   0        0        0    27994 2023-05-06 21:51:58.000000 cellpy-1.0.0b0/cellpy/internals/core.py
+-rw-rw-rw-   0        0        0     4838 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/log.py
+-rw-rw-rw-   0        0        0     1750 2021-12-21 09:11:58.000000 cellpy-1.0.0b0/cellpy/logging.json
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.258478 cellpy-1.0.0b0/cellpy/parameters/
+-rw-rw-rw-   0        0        0     3183 2023-05-02 11:51:31.000000 cellpy-1.0.0b0/cellpy/parameters/.cellpy_prms_default.conf
+-rw-rw-rw-   0        0        0        2 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/parameters/__init__.py
+-rw-rw-rw-   0        0        0    23452 2023-05-14 17:34:31.000000 cellpy-1.0.0b0/cellpy/parameters/internal_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.261008 cellpy-1.0.0b0/cellpy/parameters/legacy/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0b0/cellpy/parameters/legacy/__init__.py
+-rw-rw-rw-   0        0        0    24146 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/parameters/legacy/update_headers.py
+-rw-rw-rw-   0        0        0    12261 2023-05-23 14:50:48.000000 cellpy-1.0.0b0/cellpy/parameters/prmreader.py
+-rw-rw-rw-   0        0        0    12241 2023-05-29 17:41:25.000000 cellpy-1.0.0b0/cellpy/parameters/prms.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.271128 cellpy-1.0.0b0/cellpy/readers/
+-rw-rw-rw-   0        0        0        2 2021-12-21 09:11:58.000000 cellpy-1.0.0b0/cellpy/readers/__init__.py
+-rw-rw-rw-   0        0        0   242077 2023-05-29 17:41:28.000000 cellpy-1.0.0b0/cellpy/readers/cellreader.py
+-rw-rw-rw-   0        0        0    38362 2023-05-29 18:12:16.000000 cellpy-1.0.0b0/cellpy/readers/core.py
+-rw-rw-rw-   0        0        0    22998 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/readers/dbreader.py
+-rw-rw-rw-   0        0        0    13825 2023-05-06 21:51:58.000000 cellpy-1.0.0b0/cellpy/readers/filefinder.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.296026 cellpy-1.0.0b0/cellpy/readers/instruments/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0b0/cellpy/readers/instruments/__init__.py
+-rw-rw-rw-   0        0        0    49052 2023-05-12 17:21:48.000000 cellpy-1.0.0b0/cellpy/readers/instruments/arbin_res.py
+-rw-rw-rw-   0        0        0    19381 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/readers/instruments/arbin_sql.py
+-rw-rw-rw-   0        0        0    21062 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/readers/instruments/arbin_sql_7.py
+-rw-rw-rw-   0        0        0    11134 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/readers/instruments/arbin_sql_csv.py
+-rw-rw-rw-   0        0        0     7126 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/readers/instruments/arbin_sql_h5.py
+-rw-rw-rw-   0        0        0     9883 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/readers/instruments/arbin_sql_xlsx.py
+-rw-rw-rw-   0        0        0    27324 2023-05-09 19:57:46.000000 cellpy-1.0.0b0/cellpy/readers/instruments/base.py
+-rw-rw-rw-   0        0        0    22693 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/readers/instruments/biologics_mpr.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.308026 cellpy-1.0.0b0/cellpy/readers/instruments/configurations/
+-rw-rw-rw-   0        0        0     6607 2022-06-03 19:58:41.000000 cellpy-1.0.0b0/cellpy/readers/instruments/configurations/__init__.py
+-rw-rw-rw-   0        0        0     1700 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/readers/instruments/configurations/maccor_txt_four.py
+-rw-rw-rw-   0        0        0     4084 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/readers/instruments/configurations/maccor_txt_one.py
+-rw-rw-rw-   0        0        0     1990 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/readers/instruments/configurations/maccor_txt_three.py
+-rw-rw-rw-   0        0        0     1788 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/readers/instruments/configurations/maccor_txt_two.py
+-rw-rw-rw-   0        0        0     3549 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/readers/instruments/configurations/maccor_txt_zero.py
+-rw-rw-rw-   0        0        0     2132 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/readers/instruments/configurations/neware_txt_zero.py
+-rw-rw-rw-   0        0        0    10327 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/readers/instruments/custom.py
+-rw-rw-rw-   0        0        0     3760 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/readers/instruments/ext_nda_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.310027 cellpy-1.0.0b0/cellpy/readers/instruments/loader_specific_modules/
+-rw-rw-rw-   0        0        0        0 2022-06-03 19:58:41.000000 cellpy-1.0.0b0/cellpy/readers/instruments/loader_specific_modules/__init__.py
+-rw-rw-rw-   0        0        0    22115 2022-06-03 19:58:41.000000 cellpy-1.0.0b0/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py
+-rw-rw-rw-   0        0        0     1067 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/readers/instruments/local_instrument.py
+-rw-rw-rw-   0        0        0    12886 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/readers/instruments/maccor_txt.py
+-rw-rw-rw-   0        0        0     3488 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/readers/instruments/neware_txt.py
+-rw-rw-rw-   0        0        0    16769 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/readers/instruments/pec_csv.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.315029 cellpy-1.0.0b0/cellpy/readers/instruments/processors/
+-rw-rw-rw-   0        0        0        0 2022-05-27 12:07:50.000000 cellpy-1.0.0b0/cellpy/readers/instruments/processors/__init__.py
+-rw-rw-rw-   0        0        0    15265 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/readers/instruments/processors/post_processors.py
+-rw-rw-rw-   0        0        0     1450 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/readers/instruments/processors/pre_processors.py
+-rw-rw-rw-   0        0        0    26852 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/readers/sql_dbreader.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.337026 cellpy-1.0.0b0/cellpy/utils/
+-rw-rw-rw-   0        0        0      192 2021-12-21 09:11:58.000000 cellpy-1.0.0b0/cellpy/utils/__init__.py
+-rw-rw-rw-   0        0        0    48182 2023-05-03 09:31:40.000000 cellpy-1.0.0b0/cellpy/utils/batch.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.358026 cellpy-1.0.0b0/cellpy/utils/batch_tools/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0b0/cellpy/utils/batch_tools/__init__.py
+-rw-rw-rw-   0        0        0     7578 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/utils/batch_tools/batch_analyzers.py
+-rw-rw-rw-   0        0        0    19566 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/utils/batch_tools/batch_core.py
+-rw-rw-rw-   0        0        0    40056 2023-05-16 14:17:12.000000 cellpy-1.0.0b0/cellpy/utils/batch_tools/batch_experiments.py
+-rw-rw-rw-   0        0        0     2931 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/utils/batch_tools/batch_exporters.py
+-rw-rw-rw-   0        0        0    14090 2023-05-06 21:51:58.000000 cellpy-1.0.0b0/cellpy/utils/batch_tools/batch_helpers.py
+-rw-rw-rw-   0        0        0    27683 2023-05-02 13:39:36.000000 cellpy-1.0.0b0/cellpy/utils/batch_tools/batch_journals.py
+-rw-rw-rw-   0        0        0    29066 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/utils/batch_tools/batch_plotters.py
+-rw-rw-rw-   0        0        0      245 2021-12-21 09:11:58.000000 cellpy-1.0.0b0/cellpy/utils/batch_tools/batch_reporters.py
+-rw-rw-rw-   0        0        0     3339 2022-05-27 12:03:59.000000 cellpy-1.0.0b0/cellpy/utils/batch_tools/dumpers.py
+-rw-rw-rw-   0        0        0     9872 2023-05-02 10:20:24.000000 cellpy-1.0.0b0/cellpy/utils/batch_tools/engines.py
+-rw-rw-rw-   0        0        0     5294 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/utils/batch_tools/sqlite_from_excel_db.py
+-rw-rw-rw-   0        0        0    61436 2023-05-29 17:36:47.000000 cellpy-1.0.0b0/cellpy/utils/collectors.py
+-rw-rw-rw-   0        0        0    44134 2023-05-29 17:41:12.000000 cellpy-1.0.0b0/cellpy/utils/collectors_old.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.359026 cellpy-1.0.0b0/cellpy/utils/data/
+-rw-rw-rw-   0        0        0  3700143 2023-05-29 17:38:03.000000 cellpy-1.0.0b0/cellpy/utils/data/20160805_test001_45_cc.h5
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.369553 cellpy-1.0.0b0/cellpy/utils/data/raw/
+-rw-rw-rw-   0        0        0  1613824 2021-12-21 09:11:58.000000 cellpy-1.0.0b0/cellpy/utils/data/raw/20160805_test001_45_cc_01.res
+-rw-rw-rw-   0        0        0      260 2022-05-27 12:07:50.000000 cellpy-1.0.0b0/cellpy/utils/diagnostics.py
+-rw-rw-rw-   0        0        0    79016 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/utils/easyplot.py
+-rw-rw-rw-   0        0        0     1576 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/utils/example_data.py
+-rw-rw-rw-   0        0        0    38296 2023-05-28 11:22:04.000000 cellpy-1.0.0b0/cellpy/utils/helpers.py
+-rw-rw-rw-   0        0        0    37902 2023-05-28 19:25:11.000000 cellpy-1.0.0b0/cellpy/utils/ica.py
+-rw-rw-rw-   0        0        0      189 2022-05-27 12:07:50.000000 cellpy-1.0.0b0/cellpy/utils/live.py
+-rw-rw-rw-   0        0        0    31789 2023-05-28 20:26:34.000000 cellpy-1.0.0b0/cellpy/utils/ocv_rlx.py
+-rw-rw-rw-   0        0        0    45397 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/utils/plotutils.py
+-rw-rw-rw-   0        0        0     1787 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/cellpy/utils/processor.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.246933 cellpy-1.0.0b0/cellpy.egg-info/
+-rw-rw-rw-   0        0        0     6767 2023-05-29 19:16:22.000000 cellpy-1.0.0b0/cellpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7846 2023-05-29 19:16:23.000000 cellpy-1.0.0b0/cellpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 19:16:22.000000 cellpy-1.0.0b0/cellpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 19:16:22.000000 cellpy-1.0.0b0/cellpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-29 19:16:22.000000 cellpy-1.0.0b0/cellpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      337 2023-05-29 19:16:22.000000 cellpy-1.0.0b0/cellpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-29 19:16:22.000000 cellpy-1.0.0b0/cellpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.381553 cellpy-1.0.0b0/docs/
+-rw-rw-rw-   0        0        0     6939 2022-09-20 08:21:07.000000 cellpy-1.0.0b0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.212675 cellpy-1.0.0b0/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.211676 cellpy-1.0.0b0/docs/_build/.doctrees/
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.388557 cellpy-1.0.0b0/docs/_build/.doctrees/nbsphinx/
+-rw-rw-rw-   0        0        0    15014 2023-04-30 13:53:57.000000 cellpy-1.0.0b0/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
+-rw-rw-rw-   0        0        0    14599 2023-04-30 13:53:57.000000 cellpy-1.0.0b0/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
+-rw-rw-rw-   0        0        0    13527 2023-04-30 13:53:57.000000 cellpy-1.0.0b0/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
+-rw-rw-rw-   0        0        0    25669 2023-04-30 13:54:02.000000 cellpy-1.0.0b0/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.422083 cellpy-1.0.0b0/docs/_build/_images/
+-rw-rw-rw-   0        0        0    15014 2023-04-27 15:02:55.000000 cellpy-1.0.0b0/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
+-rw-rw-rw-   0        0        0    14599 2023-04-27 15:02:55.000000 cellpy-1.0.0b0/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
+-rw-rw-rw-   0        0        0    13527 2023-04-27 15:02:55.000000 cellpy-1.0.0b0/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
+-rw-rw-rw-   0        0        0    25669 2023-04-27 15:03:02.000000 cellpy-1.0.0b0/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
+-rw-rw-rw-   0        0        0    11678 2023-04-29 14:19:31.000000 cellpy-1.0.0b0/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png
+-rw-rw-rw-   0        0        0    22040 2023-04-29 14:33:27.000000 cellpy-1.0.0b0/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png
+-rw-rw-rw-   0        0        0    21790 2023-04-29 14:26:00.000000 cellpy-1.0.0b0/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png
+-rw-rw-rw-   0        0        0    32991 2023-04-29 14:26:01.000000 cellpy-1.0.0b0/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png
+-rw-rw-rw-   0        0        0    32991 2023-04-30 20:02:23.000000 cellpy-1.0.0b0/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png
+-rw-rw-rw-   0        0        0     7231 2023-04-29 14:12:31.000000 cellpy-1.0.0b0/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png
+-rw-rw-rw-   0        0        0    13360 2023-04-29 14:36:26.000000 cellpy-1.0.0b0/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png
+-rw-rw-rw-   0        0        0    21790 2023-04-30 20:02:22.000000 cellpy-1.0.0b0/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png
+-rw-rw-rw-   0        0        0     5391 2023-04-29 14:10:02.000000 cellpy-1.0.0b0/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png
+-rw-rw-rw-   0        0        0    20826 2023-04-29 14:29:06.000000 cellpy-1.0.0b0/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png
+-rw-rw-rw-   0        0        0    88743 2023-04-19 13:49:30.000000 cellpy-1.0.0b0/docs/_build/_images/templates_jupyterlab_001.png
+-rw-rw-rw-   0        0        0   296908 2022-05-27 12:07:51.000000 cellpy-1.0.0b0/docs/_build/_images/tutorials_utils_plotting_fig1.png
+-rw-rw-rw-   0        0        0    54588 2022-05-27 12:07:51.000000 cellpy-1.0.0b0/docs/_build/_images/tutorials_utils_plotting_fig2.png
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.427113 cellpy-1.0.0b0/docs/_build/_static/
+-rw-rw-rw-   0        0        0      286 2023-04-25 11:20:36.000000 cellpy-1.0.0b0/docs/_build/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0b0/docs/_build/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0b0/docs/_build/_static/plus.png
+-rw-rw-rw-   0        0        0     1695 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/adapted_readme.rst
+-rw-rw-rw-   0        0        0    10731 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/conf.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.441590 cellpy-1.0.0b0/docs/developers_guide/
+-rw-rw-rw-   0        0        0     1334 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/developers_guide/dev_cellpy_data_structure.rst
+-rw-rw-rw-   0        0        0     5904 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/developers_guide/dev_cellpy_folder_structure.rst
+-rw-rw-rw-   0        0        0      935 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/developers_guide/dev_cellpy_packaging_pypi.rst
+-rw-rw-rw-   0        0        0     3009 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/developers_guide/dev_cellpy_setup.rst
+-rw-rw-rw-   0        0        0     1821 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/developers_guide/dev_conda_package.rst
+-rw-rw-rw-   0        0        0     2136 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/developers_guide/dev_docs.rst
+-rw-rw-rw-   0        0        0     5218 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/developers_guide/dev_loaders_and_instruments.rst
+-rw-rw-rw-   0        0        0     1768 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/developers_guide/dev_various.rst
+-rw-rw-rw-   0        0        0      326 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/developers_guide/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.452103 cellpy-1.0.0b0/docs/examples_and_tutorials/
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.465121 cellpy-1.0.0b0/docs/examples_and_tutorials/basic_interactions/
+-rw-rw-rw-   0        0        0    15786 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst
+-rw-rw-rw-   0        0        0     3909 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst
+-rw-rw-rw-   0        0        0     5485 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst
+-rw-rw-rw-   0        0        0     4465 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst
+-rw-rw-rw-   0        0        0     5908 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/basic_interactions/05_configuring.rst
+-rw-rw-rw-   0        0        0     1052 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/basic_interactions/06_pandas.rst
+-rw-rw-rw-   0        0        0     1102 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst
+-rw-rw-rw-   0        0        0     8224 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst
+-rw-rw-rw-   0        0        0      484 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/basics.rst
+-rw-rw-rw-   0        0        0      366 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/examples.rst
+-rw-rw-rw-   0        0        0      174 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.474120 cellpy-1.0.0b0/docs/examples_and_tutorials/loaders/
+-rw-rw-rw-   0        0        0       49 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/loaders/01_arbin.rst
+-rw-rw-rw-   0        0        0       52 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/loaders/02_maccor.rst
+-rw-rw-rw-   0        0        0       43 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/loaders/03_PEC.rst
+-rw-rw-rw-   0        0        0       54 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/loaders/04_Neware.rst
+-rw-rw-rw-   0        0        0       62 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/loaders/05_biologics.rst
+-rw-rw-rw-   0        0        0       54 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/loaders/06_custom.rst
+-rw-rw-rw-   0        0        0      260 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/loaders.rst
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.214675 cellpy-1.0.0b0/docs/examples_and_tutorials/notebooks/
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.477629 cellpy-1.0.0b0/docs/examples_and_tutorials/notebooks/images/
+-rw-rw-rw-   0        0        0    88743 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png
+-rw-rw-rw-   0        0        0    95663 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png
+-rw-rw-rw-   0        0        0      231 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/notebooks.rst
+-rw-rw-rw-   0        0        0     1797 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/tips_and_tricks.rst
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.487638 cellpy-1.0.0b0/docs/examples_and_tutorials/utils/
+-rw-rw-rw-   0        0        0     4388 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/utils/batch.rst
+-rw-rw-rw-   0        0        0       59 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/utils/collectors.rst
+-rw-rw-rw-   0        0        0       53 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/utils/easyplot.rst
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.491628 cellpy-1.0.0b0/docs/examples_and_tutorials/utils/figures/
+-rw-rw-rw-   0        0        0   296908 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png
+-rw-rw-rw-   0        0        0    54588 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png
+-rw-rw-rw-   0        0        0     1219 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/utils/ica.rst
+-rw-rw-rw-   0        0        0     2063 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/utils/plotting.rst
+-rw-rw-rw-   0        0        0      338 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/utils/templates.rst
+-rw-rw-rw-   0        0        0     1379 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst
+-rw-rw-rw-   0        0        0      371 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/examples_and_tutorials/utils.rst
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.498109 cellpy-1.0.0b0/docs/figures/
+-rw-rw-rw-   0        0        0     9981 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/figures/cellpy-icon-bw.png
+-rw-rw-rw-   0        0        0    10302 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/figures/cellpy-logo-v1.png
+-rw-rw-rw-   0        0        0      593 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.508625 cellpy-1.0.0b0/docs/main_description/
+-rw-rw-rw-   0        0        0       32 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/main_description/authors.rst
+-rw-rw-rw-   0        0        0       37 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/main_description/contributing.rst
+-rw-rw-rw-   0        0        0    16327 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/main_description/formats.rst
+-rw-rw-rw-   0        0        0       32 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/main_description/history.rst
+-rw-rw-rw-   0        0        0      182 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/main_description/index.rst
+-rw-rw-rw-   0        0        0     4288 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/main_description/installation.rst
+-rw-rw-rw-   0        0        0     3444 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/main_description/usage.rst
+-rwxrwxrwx   0        0        0     6701 2022-09-20 08:21:07.000000 cellpy-1.0.0b0/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-29 19:16:23.527631 cellpy-1.0.0b0/docs/source/
+-rw-rw-rw-   0        0        0      367 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/source/cellpy.internals.rst
+-rw-rw-rw-   0        0        0      447 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/source/cellpy.parameters.legacy.rst
+-rw-rw-rw-   0        0        0      847 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/source/cellpy.parameters.rst
+-rw-rw-rw-   0        0        0     1911 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/source/cellpy.readers.instruments.configurations.rst
+-rw-rw-rw-   0        0        0      631 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/source/cellpy.readers.instruments.loader_specific_modules.rst
+-rw-rw-rw-   0        0        0      783 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/source/cellpy.readers.instruments.processors.rst
+-rw-rw-rw-   0        0        0     3413 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/source/cellpy.readers.instruments.rst
+-rw-rw-rw-   0        0        0     1139 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/source/cellpy.readers.rst
+-rw-rw-rw-   0        0        0      721 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/source/cellpy.rst
+-rw-rw-rw-   0        0        0     2610 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/source/cellpy.utils.batch_tools.rst
+-rw-rw-rw-   0        0        0     2222 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/docs/source/cellpy.utils.rst
+-rw-rw-rw-   0        0        0       62 2023-05-01 10:14:23.000000 cellpy-1.0.0b0/docs/source/modules.rst
+-rw-rw-rw-   0        0        0      281 2023-05-01 18:24:45.000000 cellpy-1.0.0b0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 19:16:23.529624 cellpy-1.0.0b0/setup.cfg
+-rw-rw-rw-   0        0        0     2922 2023-05-12 17:21:47.000000 cellpy-1.0.0b0/setup.py
```

### Comparing `cellpy-1.0.0a9/CONTRIBUTING.rst` & `cellpy-1.0.0b0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/HISTORY.rst` & `cellpy-1.0.0b0/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/LICENSE` & `cellpy-1.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/MANIFEST.in` & `cellpy-1.0.0b0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/PKG-INFO` & `cellpy-1.0.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellpy
-Version: 1.0.0a9
+Version: 1.0.0b0
 Summary: Extract and manipulate data from battery data testers.
 Home-page: https://github.com/jepegit/cellpy
 Author: Jan Petter Maehlen
 Author-email: jepe@ife.no
 License: MIT license
 Keywords: cellpy
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cellpy-1.0.0a9/README.rst` & `cellpy-1.0.0b0/README.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/__init__.py` & `cellpy-1.0.0b0/cellpy/__init__.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/cli.py` & `cellpy-1.0.0b0/cellpy/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 from cellpy.parameters.internal_settings import OTHERPATHS
 from cellpy.internals.core import OtherPath
 
 VERSION = cellpy._version.__version__
 REPO = "jepegit/cellpy"
 USER = "jepegit"
 GITHUB_PWD_VAR_NAME = "GD_PWD"
-DEFAULT_EDITOR = 'vim'
-EDITORS = {'Windows': 'notepad'}
+DEFAULT_EDITOR = "vim"
+EDITORS = {"Windows": "notepad"}
 
 
 def save_prm_file(prm_filename):
     """saves (writes) the prms to file"""
     prmreader._write_prm_file(prm_filename)
 
 
@@ -678,17 +678,16 @@
 def _get_default_editor():
     """
     Return the default text editor.
 
     This code is based on the `editor` library by @rec.
     """
 
-    return os.environ.get('VISUAL') or (
-        os.environ.get('EDITOR')
-        or EDITORS.get(platform.system(), DEFAULT_EDITOR)
+    return os.environ.get("VISUAL") or (
+        os.environ.get("EDITOR") or EDITORS.get(platform.system(), DEFAULT_EDITOR)
     )
 
 
 # ----------------------- edit ---------------------------------------
 @click.command()
 @click.option(
     "--default-editor",
```

### Comparing `cellpy-1.0.0a9/cellpy/exceptions.py` & `cellpy-1.0.0b0/cellpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/internals/core.py` & `cellpy-1.0.0b0/cellpy/internals/core.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/log.py` & `cellpy-1.0.0b0/cellpy/log.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/logging.json` & `cellpy-1.0.0b0/cellpy/logging.json`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/parameters/.cellpy_prms_default.conf` & `cellpy-1.0.0b0/cellpy/parameters/.cellpy_prms_default.conf`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/parameters/internal_settings.py` & `cellpy-1.0.0b0/cellpy/parameters/internal_settings.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/parameters/legacy/update_headers.py` & `cellpy-1.0.0b0/cellpy/parameters/legacy/update_headers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/parameters/prmreader.py` & `cellpy-1.0.0b0/cellpy/parameters/prmreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/parameters/prms.py` & `cellpy-1.0.0b0/cellpy/parameters/prms.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,17 @@
     ] = None  # limit loading cycles to given cycle number
     ensure_step_table: bool = False
     ensure_summary_table: bool = False
     voltage_interpolation_step: float = 0.01
     time_interpolation_step: float = 10.0
     capacity_interpolation_step: float = 2.0
     use_cellpy_stat_file: bool = False
-    auto_dirs: bool = True  # search in prm-file for res and hdf5 dirs in cellpy.get()
+    auto_dirs: bool = (
+        True  # v2.0 search in prm-file for res and hdf5 dirs in cellpy.get()
+    )
 
 
 @dataclass
 class DbClass(CellPyConfig):
     db_type: str = "simple_excel_reader"
     db_table_name: str = "db_table"  # used for simple excel db reader
     db_header_row: int = 0  # used for simple excel db reader
```

### Comparing `cellpy-1.0.0a9/cellpy/readers/cellreader.py` & `cellpy-1.0.0b0/cellpy/readers/cellreader.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,21 +19,22 @@
 import numbers
 import os
 import sys
 import time
 import datetime
 import warnings
 from pathlib import Path
-from typing import Union, Sequence, List
+from typing import Union, Sequence, List, Optional, Iterable
 from dataclasses import asdict
 
 import numpy as np
 import openpyxl
 import pandas as pd
 from pandas.errors import PerformanceWarning
+from pint.errors import DimensionalityError
 from pint import Quantity
 from scipy import interpolate
 
 from cellpy.exceptions import (
     DeprecatedFeature,
     NullData,
     WrongFileVersion,
@@ -74,29 +75,29 @@
     xldate_as_datetime,
     generate_default_factory,
     Q,
     convert_from_simple_unit_label_to_string_unit_label,
 )
 from cellpy.internals.core import OtherPath
 
+DIGITS_C_RATE = 5
+
 HEADERS_NORMAL = get_headers_normal()  # TODO @jepe refactor this (not needed)
 HEADERS_SUMMARY = get_headers_summary()  # TODO @jepe refactor this (not needed)
 HEADERS_STEP_TABLE = get_headers_step_table()  # TODO @jepe refactor this (not needed)
 
 # TODO: @jepe - new feature - method for assigning new cycle numbers and step numbers
 #   - Sometimes the user forgets to increment the cycle number and it would be good
 #   to have a method so that its possible to set new cycle numbers manually
 #   - Some testers merges different steps into one (e.g CC-CV), it would be nice to have
 #   a method for "splitting that up"
 
 # TODO: @jepe - performance warnings - mixed types within cols (pytables)
-performance_warning_level = "ignore"  # "ignore", "error"
-warnings.filterwarnings(
-    performance_warning_level, category=pd.io.pytables.PerformanceWarning
-)
+
+warnings.filterwarnings("ignore", category=pd.io.pytables.PerformanceWarning)
 pd.set_option("mode.chained_assignment", None)  # "raise", "warn", None
 
 module_logger = logging.getLogger(__name__)
 
 
 class CellpyCell:
     """Main class for working and storing data.
@@ -106,32 +107,44 @@
     header definitions, both for the cellpy hdf5 format, and for the various
     cell-tester file-formats that can be read. The class can contain
     several cell-tests and each test is stored in a list. If you see what I mean...
 
     Attributes:
         # TODO v.1.0.1: update this
         data: cellpy.Data object
+        cellpy_units: cellpy.units object
+        cellpy_datadir: path to cellpy data directory
+        raw_datadir: path to raw data directory
+        filestatuschecker: filestatuschecker object
+        force_step_table_creation: force step table creation
+        ensure_step_table: ensure step table
+        limit_loaded_cycles: limit loaded cycles
+        profile: profile
+        select_minimal: select minimal
+        empty: empty
+        forced_errors: forced errors
+        capacity_modifiers: capacity modifiers
+        sep: separator
+        cycle_mode: cycle mode
+        tester: tester
+        cell_name: cell name
+        cellpy_file_version: cellpy file version
     """
 
     def __repr__(self):
-        txt = f"CellpyCell-object (id={hex(id(self))})"
-        if self.session_name:
-            txt += f"\nname: {self.session_name}"
-        if self.table_names:
-            txt += f"\ntable_names: {self.table_names}"
-        if self.tester:
-            txt += f"\ntester: {self.tester}"
+        txt = f"<CellpyCell> (id={hex(id(self))})"
+        if self.cell_name:
+            txt += f" [name={self.cell_name}]"
         return txt
 
     def _repr_html_(self):
         header = f"""
             <h2>CellpyCell-object</h2>
             <b>id</b>: {hex(id(self))} <br>
-            <b>name</b>: {self.session_name} <br>
-            <b>table names</b>: {self.table_names} <br>
+            <b>name</b>: {self.cell_name} <br>
             <b>tester</b>: {self.tester} <br>
             <b>cycle_mode</b>: {self.cycle_mode} <br>
             <b>sep</b>: {self.sep} <br>
             <b>cellpy_datadir</b>: {self.cellpy_datadir} <br>
             <b>raw_datadir</b>: {self.raw_datadir} <br>
         """
         all_vars = "<p>"
@@ -143,29 +156,27 @@
             <b>force_step_table_creation</b>: {self.force_step_table_creation} <br>
             <b>forced_errors</b>: {self.forced_errors} <br>
             <b>limit_loaded_cycles</b>: {self.limit_loaded_cycles} <br>
             <b>profile</b>: {self.profile} <br>
             <b>cellpy_units</b>: {self.cellpy_units} <br>
             <b>select_minimal</b>: {self.select_minimal} <br>
             <b>selected_scans</b>: {self.selected_scans} <br>
-            <b>summary_exists (deprecated)</b>: {self.summary_exists} <br>
         """
         all_vars += "</p>"
 
         cell_txt = ""
         cell_txt += f"<h3>data</h3>"
         cell_txt += f"<blockquote>{self.data._repr_html_()}</blockquote>"
         return header + all_vars + cell_txt
 
     def __str__(self):
-        txt = "<CellpyCell>\n"
-        if self.session_name:
-            txt += f"session name: {self.session_name}\n"
-        if self.table_names:
-            txt += f"table names: {self.table_names}\n"
+        txt = "CellpyCell\n"
+        txt += "----------\n"
+        if self.cell_name:
+            txt += f"session name: {self.cell_name}\n"
         if self.tester:
             txt += f"tester: {self.tester}\n"
         if self.data:
             txt += "data:\n"
             for t in str(self.data).split("\n"):
                 txt += "     "
                 txt += t
@@ -223,21 +234,20 @@
         else:
             self.tester = tester
 
         self.loader = None  # this will be set in the function set_instrument
         self.debug = debug
         logging.debug("created CellpyCell instance")
 
-        self._session_name = None
+        self._cell_name = None
         self.profile = profile
 
         self.minimum_selection = {}
         self.filestatuschecker = filestatuschecker or prms.Reader.filestatuschecker
         self.forced_errors = 0
-        self.summary_exists = False
 
         self.file_names = filenames or []
         if not self._is_listtype(self.file_names):
             self.file_names = [self.file_names]
 
         self.selected_scans = selected_scans or []
         if not self._is_listtype(self.selected_scans):
@@ -264,75 +274,81 @@
             "not_known",
         ]
         # - options
         self.force_step_table_creation = prms.Reader.force_step_table_creation
         self.force_all = prms.Reader.force_all
         self.sep = prms.Reader.sep
         self._cycle_mode = None
-        self._nom_cap_specifics = prms.Materials.default_nom_cap_specifics
         self.select_minimal = prms.Reader.select_minimal
         self.limit_loaded_cycles = prms.Reader.limit_loaded_cycles
         self.limit_data_points = None
         self.ensure_step_table = prms.Reader.ensure_step_table
         self.ensure_summary_table = prms.Reader.ensure_summary_table
         self.raw_datadir = OtherPath(prms.Paths.rawdatadir)
         self.cellpy_datadir = OtherPath(prms.Paths.cellpydatadir)
-        self.auto_dirs = prms.Reader.auto_dirs
+        self.auto_dirs = prms.Reader.auto_dirs  # v2.0
 
         # - headers and instruments
         self.headers_normal = headers_normal
         self.headers_summary = headers_summary
         self.headers_step_table = headers_step_table
-
-        self.table_names = None  # dictionary defined in set_instruments
         self.instrument_factory = None
         self.register_instrument_readers()
         self.set_instrument()
         # - units used by cellpy
         self.cellpy_units = get_cellpy_units(cellpy_units)
-        self.output_units = get_default_output_units(output_units)
+        self.output_units = get_default_output_units(output_units)  # v2.0
 
         if initialize:
             self.initialize()
 
     def initialize(self):
-        """Initialize the cellpycell object."""
+        """Initialize the CellpyCell object with empty Data instance."""
 
         logging.debug("Initializing...")
-        # TODO: v.1.0.0: replace this
         self._data = Data()
 
     # the batch utility might be using session name
     # the cycle and ica collector are using session name
     # improvement suggestion: use data.cell_name instead
     @property
-    def session_name(self):
+    def cell_name(self):
         """returns the session name"""
 
-        if not self._session_name:
+        if not self._cell_name:
             return self.data.cell_name
         else:
-            return self._session_name
+            return self._cell_name
 
-    @session_name.setter
-    def session_name(self, n):
+    @cell_name.setter
+    def cell_name(self, n):
         """sets the session name"""
 
-        self._session_name = n
+        self._cell_name = n
         if not self.data.cell_name:
             self.data.cell_name = n
 
-    def _invent_a_session_name(self, filename=None, override=False):
+    def _invent_a_cell_name(self, filename=None, override=False):
         if filename is None:
-            self.session_name = "nameless"
+            self.cell_name = "nameless"
             return
-        if self.session_name and not override:
+        if self.cell_name and not override:
             return
-        path = Path(filename)
-        self.session_name = path.with_suffix("").name
+        if isinstance(filename, (list, tuple)):
+            names = [Path(n).with_suffix("").name for n in filename]
+            names = [
+                n.replace(" ", "_").replace("-", "_").replace(".", "_") for n in names
+            ]
+            names = list(set(names))
+            if len(names) == 1:
+                self.cell_name = names[0]
+            else:
+                self.cell_name = "-".join(names)
+        else:
+            self.cell_name = Path(filename).with_suffix("").name
 
     @property
     def mass(self):
         """returns the mass"""
         return self.data.mass
 
     @mass.setter
@@ -371,31 +387,34 @@
             logging.debug(f"Could not parse {value}")
             return
         return c
 
     @property
     def nom_cap_specifics(self):
         """returns the nominal capacity specific"""
-        return self._nom_cap_specifics
-
-    # NEXT: update make_summary and make_step_table to use this. And update get() to use this.
+        return self.data.meta_common.nom_cap_specifics
 
     @nom_cap_specifics.setter
     def nom_cap_specifics(self, c):
         if c.lower() == "areal":
-            self.cellpy_units.nominal_capacity = f"{self.cellpy_units.charge}/{self.cellpy_units.specific_areal}"
+            self.cellpy_units.nominal_capacity = (
+                f"{self.cellpy_units.charge}/{self.cellpy_units.specific_areal}"
+            )
         elif c.lower() == "gravimetric":
-            self.cellpy_units.nominal_capacity = f"{self.cellpy_units.charge}/{self.cellpy_units.specific_gravimetric}"
+            self.cellpy_units.nominal_capacity = (
+                f"{self.cellpy_units.charge}/{self.cellpy_units.specific_gravimetric}"
+            )
         elif c.lower() == "volumetric":
-            self.cellpy_units.nominal_capacity = f"{self.cellpy_units.charge}/{self.cellpy_units.specific_volumetric}"
+            self.cellpy_units.nominal_capacity = (
+                f"{self.cellpy_units.charge}/{self.cellpy_units.specific_volumetric}"
+            )
         else:
             logging.warning(f"Unknown nominal capacity specific: {c}")
             return
-
-        self._nom_cap_specifics = c
+        self.data.meta_common.nom_cap_specifics = c
 
     @property
     def raw_units(self):
         """returns the raw_units dictionary"""
 
         return self.data.raw_units
 
@@ -715,28 +734,28 @@
         if len(_instrument) < 2:
             return instrument, None
 
         return _instrument
 
     @property
     def cycle_mode(self):
-        # TODO: edit this from scalar to list
+        # TODO: v2.0 edit this from scalar to list
         try:
             data = self.data
-            return data.meta_test_dependent.cycle_mode[0]
+            return data.meta_test_dependent.cycle_mode
         except NoDataFound:
             return self._cycle_mode
 
     @cycle_mode.setter
     def cycle_mode(self, cycle_mode):
-        # TODO: edit this from scalar to list
+        # TODO: v2.0 edit this from scalar to list
         logging.debug(f"-> cycle_mode: {cycle_mode}")
         try:
             data = self.data
-            data.meta_test_dependent.cycle_mode = [cycle_mode]
+            data.meta_test_dependent.cycle_mode = cycle_mode
             self._cycle_mode = cycle_mode
         except NoDataFound:
             self._cycle_mode = cycle_mode
 
     def set_raw_datadir(self, directory=None):
         """Set the directory containing .res-files.
 
@@ -1010,16 +1029,15 @@
             >>> ... mass = my_dbreader.get_mass(srno)
             >>> ... rawfiles, cellpyfiles = \
             >>> ...     filefinder.search_for_files(my_run_name)
             >>> ... cell_data = cellreader.CellpyCell()
             >>> ... cell_data.loadcell(raw_files=rawfiles,
             >>> ...                    cellpy_file=cellpyfiles)
             >>> ... cell_data.set_mass(mass)
-            >>> ... if not cell_data.summary_exists:
-            >>> ...     cell_data.make_summary() # etc. etc.
+            >>> ... cell_data.make_summary() # etc. etc.
             >>> ... cell_datas.append(cell_data)
             >>>
         """
         # This is a part of a dramatic API change. It will not be possible to
         # load more than one set of datasets (i.e. one single cellpy-file or
         # several raw-files that will be automatically merged)
 
@@ -1221,15 +1239,15 @@
 
         if not prms.Reader.sorted_data:
             logging.debug("sorting data")
             data = self._sort_data(data)
             data.raw_units = self._set_raw_units()
 
         self.data = data
-        self._invent_a_session_name()  # TODO (v1.0.0): fix me
+        self._invent_a_cell_name(self.file_names)  # TODO (v1.0.0): fix me
         return self
 
     def _validate_cell(self, level=0):
         logging.debug("validating test")
         # simple validation for finding empty datasets - should be expanded to
         # find not-complete datasets, datasets with missing parameters etc
         v = True
@@ -1312,15 +1330,15 @@
         if data:
             self.data = data
         else:
             # raise LoadError
             logging.warning("Could not load")
             logging.warning(str(cellpy_file))
 
-        self._invent_a_session_name(cellpy_file)
+        self._invent_a_cell_name(cellpy_file)
         if return_cls:
             return self
 
     # TODO @jepe: move this to its own module (e.g. as a cellpy-loader in instruments?):
     def _get_cellpy_file_version(self, filename, meta_dir=None, parent_level=None):
         if meta_dir is None:
             meta_dir = prms._cellpyfile_common_meta
@@ -2733,15 +2751,15 @@
                 area = self.data.active_electrode_area
                 nom_cap = self.nominal_capacity_as_absolute(
                     nom_cap, area, nom_cap_specifics
                 )
             df_steps[shdr.rate_avr] = abs(
                 round(
                     df_steps.loc[:, (shdr.current, "avr")] / nom_cap,
-                    3,
+                    DIGITS_C_RATE,
                 )
             )
         df_steps[shdr.type] = np.nan
         df_steps[shdr.sub_type] = np.nan
         df_steps[shdr.info] = np.nan
 
         if step_specifications is None:
@@ -3741,89 +3759,200 @@
 
         Returns:
             pandas.Series or None if empty
         """
         header = self.headers_normal.current_txt
         return self._sget(cycle, step, header, usteps=False)
 
-    def get_voltage(self, cycle=None, full=True):
-        """Returns voltage (in V).
+    def get_raw(
+        self,
+        header,
+        cycle: Optional[Union[Iterable, int]] = None,
+        with_index: bool = True,
+        with_step: bool = False,
+        with_time: bool = False,
+        additional_headers: Optional[list] = None,
+        as_frame: bool = True,
+        scaler: Optional[float] = None,
+    ) -> Union[pd.DataFrame, List[np.array]]:
+        """Returns the values for column with given header (in raw units).
 
         Args:
-            cycle: cycle number (all cycles if None)
-            full: valid only for cycle=None (i.e. all cycles), returns the full
-               pandas.Series if True, else a list of pandas.Series
+            header: header name.
+            cycle: cycle number (all cycles if None).
+            with_index: if True, includes the cycle index as a column in the returned pandas.DataFrame.
+            with_step: if True, includes the step index as a column in the returned pandas.DataFrame.
+            with_time: if True, includes the time as a column in the returned pandas.DataFrame.
+            additional_headers (list): additional headers to include in the returned pandas.DataFrame.
+            as_frame: if not True, returns a list of current values as numpy arrays (one for each cycle).
+                Remark that with_time and with_index will be False if as_frame is set to False.
+            scaler: if not None, the returned values are scaled by this value.
 
         Returns:
-            pandas.Series (or list of pandas.Series if cycle=None og full=False)
+            pandas.DataFrame (or list of numpy arrays if as_frame=False)
         """
-
+        y_header = header  # Consider including some lookup handling here
         cycle_index_header = self.headers_normal.cycle_index_txt
-        voltage_header = self.headers_normal.voltage_txt
-        # step_index_header  = self.headers_normal.step_index_txt
+        time_header = self.headers_normal.test_time_txt
+        step_index_header = self.headers_normal.step_index_txt
+
+        if not as_frame:
+            with_time = False
+            with_index = True
+            with_step = False
+            additional_headers = None
+
+        y_headers = [y_header]
+        if with_time:
+            y_headers.append(time_header)
+        if with_step:
+            y_headers.append(step_index_header)
+        if with_index:
+            y_headers.append(cycle_index_header)
+
+        y_headers = reversed(y_headers)
+        if additional_headers is not None:
+            y_headers.extend(additional_headers)
 
         data = self.data.raw
-        if cycle:
-            logging.debug("getting voltage curve for cycle")
-            c = data[(data[cycle_index_header] == cycle)]
-            if not self._is_empty_array(c):
-                v = c[voltage_header]
-                return v
-        else:
-            if not full:
-                logging.debug("getting list of voltage-curves for all cycles")
-                v = []
-                no_cycles = np.amax(data[cycle_index_header])
-                for j in range(1, no_cycles + 1):
-                    txt = "Cycle  %i:  " % j
-                    logging.debug(txt)
-                    c = data[(data[cycle_index_header] == j)]
-                    v.append(c[voltage_header])
-            else:
-                logging.debug("getting frame of all voltage-curves")
-                v = data[voltage_header]
-            return v
 
-    def get_current(self, cycle=None, full=True):
-        """Returns current (in mA).
+        if cycle is None:
+            cycle = self.get_cycle_numbers()
+        else:
+            if not isinstance(cycle, collections.abc.Iterable):
+                cycle = [cycle]
+
+        logging.debug(f"getting current for cycles {cycle}")
+        c = data.loc[(data[cycle_index_header].isin(cycle)), y_headers]
+
+        if scaler is not None:
+            c[y_header] = c[y_header] * scaler
+
+        if not as_frame:
+            gb = c.groupby(cycle_index_header)
+            c = [gb.get_group(x) for x in gb.groups]
+            c = [x[y_header].values for x in c]
+        return c
+
+    def get_voltage(self, cycle=None, with_index=True, with_time=False, as_frame=True):
+        """Returns voltage (in raw units).
 
         Args:
-            cycle: cycle number (all cycles if None)
-            full: valid only for cycle=None (i.e. all cycles), returns the full
-               pandas.Series if True, else a list of pandas.Series
+            cycle: cycle number (all cycles if None).
+            with_index: if True, includes the cycle index as a column in the returned pandas.DataFrame.
+            with_time: if True, includes the time as a column in the returned pandas.DataFrame.
+            as_frame: if not True, returns a list of current values as numpy arrays (one for each cycle).
+                Remark that with_time and with_index will be False if as_frame is set to False.
 
         Returns:
-            pandas.Series (or list of pandas.Series if cycle=None og full=False)
+            pandas.DataFrame (or list of pandas.Series if cycle=None and as_frame=False)
         """
 
-        cycle_index_header = self.headers_normal.cycle_index_txt
-        current_header = self.headers_normal.current_txt
-        # step_index_header  = self.headers_normal.step_index_txt
+        y_header = self.headers_normal.voltage_txt
+        return self.get_raw(
+            y_header,
+            cycle=cycle,
+            with_index=with_index,
+            with_time=with_time,
+            as_frame=as_frame,
+            with_step=False,
+            additional_headers=None,
+            scaler=None,
+        )
 
-        data = self.data.raw
-        if cycle:
-            logging.debug(f"getting current for cycle {cycle}")
-            c = data[(data[cycle_index_header] == cycle)]
-            if not self._is_empty_array(c):
-                v = c[current_header]
-                return v
-        else:
-            if not full:
-                logging.debug("getting a list of current-curves for all cycles")
-                v = []
-                no_cycles = np.amax(data[cycle_index_header])
-                for j in range(1, no_cycles + 1):
-                    txt = "Cycle  %i:  " % j
-                    logging.debug(txt)
-                    c = data[(data[cycle_index_header] == j)]
-                    v.append(c[current_header])
-            else:
-                logging.debug("getting all current-curves ")
-                v = data[current_header]
-            return v
+    def get_current(self, cycle=None, with_index=True, with_time=False, as_frame=True):
+        """Returns current (in raw units).
+
+        Args:
+            cycle: cycle number (all cycles if None).
+            with_index: if True, includes the cycle index as a column in the returned pandas.DataFrame.
+            with_time: if True, includes the time as a column in the returned pandas.DataFrame.
+            as_frame: if not True, returns a list of current values as numpy arrays (one for each cycle).
+                Remark that with_time and with_index will be False if as_frame is set to False.
+
+        Returns:
+            pandas.DataFrame (or list of pandas.Series if cycle=None and as_frame=False)
+        """
+
+        y_header = self.headers_normal.current_txt
+        return self.get_raw(
+            y_header,
+            cycle=cycle,
+            with_index=with_index,
+            with_time=with_time,
+            as_frame=as_frame,
+            with_step=False,
+            additional_headers=None,
+            scaler=None,
+        )
+
+    def get_datetime(self, cycle=None, with_index=True, with_time=False, as_frame=True):
+        """Returns datetime (in raw units).
+
+        Args:
+            cycle: cycle number (all cycles if None).
+            with_index: if True, includes the cycle index as a column in the returned pandas.DataFrame.
+            with_time: if True, includes the time as a column in the returned pandas.DataFrame.
+            as_frame: if not True, returns a list of current values as numpy arrays (one for each cycle).
+                Remark that with_time and with_index will be False if as_frame is set to False.
+
+        Returns:
+            pandas.DataFrame (or list of pandas.Series if cycle=None and as_frame=False)
+        """
+
+        y_header = self.headers_normal.datetime_txt
+        return self.get_raw(
+            y_header,
+            cycle=cycle,
+            with_index=with_index,
+            with_time=with_time,
+            as_frame=as_frame,
+            with_step=False,
+            additional_headers=None,
+            scaler=None,
+        )
+
+    def get_timestamp(
+        self, cycle=None, with_index=True, as_frame=True, in_minutes=False, units="raw"
+    ):
+        """Returns timestamp.
+
+        Args:
+            cycle: cycle number (all cycles if None).
+            with_index: if True, includes the cycle index as a column in the returned pandas.DataFrame.
+            as_frame: if not True, returns a list of current values as numpy arrays (one for each cycle).
+                Remark that with_time and with_index will be False if as_frame is set to False.
+            in_minutes: (deprecated, use units="minutes" instead) return values in minutes
+                instead of seconds if True.
+            units: return values in given time unit ("raw", "seconds", "minutes", "hours").
+
+        Returns:
+            pandas.DataFrame (or list of pandas.Series if cycle=None and as_frame=False)
+        """
+
+        y_header = self.headers_normal.test_time_txt
+
+        if in_minutes:
+            units = "minutes"
+
+        if units == "raw":
+            scaler = None
+        else:
+            scaler = self.unit_scaler_from_raw(units, "time")
+
+        return self.get_raw(
+            y_header,
+            cycle=cycle,
+            with_index=with_index,
+            with_time=False,
+            as_frame=as_frame,
+            with_step=False,
+            additional_headers=None,
+            scaler=scaler,
+        )
 
     def sget_steptime(self, cycle, step):
         """Returns step time for cycle, step.
 
         Convenience function; same as issuing
            raw[(raw[cycle_index_header] == cycle) &
                  (raw[step_index_header] == step)][step_time_header]
@@ -3899,142 +4028,74 @@
         Returns:
             pandas.Series
         """
 
         header = self.headers_normal.step_index_txt
         return self._sget(cycle, step, header, usteps=False)
 
-    def get_datetime(self, cycle=None, full=True):
-        cycle_index_header = self.headers_normal.cycle_index_txt
-        datetime_header = self.headers_normal.datetime_txt
-
-        v = pd.Series()
-        test = self.data.raw
-        if cycle:
-            c = test[(test[cycle_index_header] == cycle)]
-            if not self._is_empty_array(c):
-                v = c[datetime_header]
-
-        else:
-            if not full:
-                logging.debug("getting datetime for all cycles")
-                v = []
-                cycles = self.get_cycle_numbers()
-                for j in cycles:
-                    txt = "Cycle  %i:  " % j
-                    logging.debug(txt)
-                    c = test[(test[cycle_index_header] == j)]
-                    v.append(c[datetime_header])
-            else:
-                logging.debug("returning full datetime col")
-                v = test[datetime_header]
-        return v
-
-    def get_timestamp(self, cycle=None, in_minutes=False, full=True):
-        """Returns timestamps (in sec or minutes (if in_minutes==True)).
-
-        Args:
-            cycle: cycle number (all if None)
-            in_minutes: return values in minutes instead of seconds if True
-            full: valid only for cycle=None (i.e. all cycles), returns the full
-               pandas.Series if True, else a list of pandas.Series
-
-        Returns:
-            pandas.Series (or list of pandas.Series if cycle=None og full=False)
-        """
-
-        cycle_index_header = self.headers_normal.cycle_index_txt
-        timestamp_header = self.headers_normal.test_time_txt
-
-        v = pd.Series()
-        test = self.data.raw
-        if cycle:
-            c = test[(test[cycle_index_header] == cycle)]
-            if not self._is_empty_array(c):
-                v = c[timestamp_header]
-
-        else:
-            if not full:
-                logging.debug("getting timestapm for all cycles")
-                v = []
-                cycles = self.get_cycle_numbers()
-                for j in cycles:
-                    txt = "Cycle  %i:  " % j
-                    logging.debug(txt)
-                    c = test[(test[cycle_index_header] == j)]
-                    v.append(c[timestamp_header])
-            else:
-                logging.debug("returning full timestamp col")
-                v = test[timestamp_header]
-                if in_minutes and v is not None:
-                    v /= 60.0
-        if in_minutes and v is not None:
-            v /= 60.0
-        return v
-
     def get_dcap(
         self,
         cycle=None,
         converter=None,
         mode="gravimetric",
-        return_dataframe=True,
+        as_frame=True,
         **kwargs,
     ):
         """Returns discharge-capacity and voltage for the selected cycle
         Args:
             cycle (int): cycle number.
             converter (float): a multiplication factor that converts the values to specific values (i.e.
                 from Ah to mAh/g). If not provided (or None), the factor is obtained from the
                 self.get_converter_to_specific() method.
             mode (string): 'gravimetric', 'areal' or 'absolute'. Defaults to 'gravimetric'.
                 Used if converter is not provided (or None).
-            return_dataframe (bool): if True: returns pd.DataFrame instead of capacity, voltage series.
+            as_frame (bool): if True: returns pd.DataFrame instead of capacity, voltage series.
             **kwargs:
         Returns:
             discharge_capacity, voltage (pd.Series or pd.DataFrame if return_dataframe is True).
 
         """
 
         if converter is None:
             converter = self.get_converter_to_specific(mode=mode)
 
         dc, v = self._get_cap(cycle, "discharge", converter=converter, **kwargs)
-        if return_dataframe:
+        if as_frame:
             cycle_df = pd.concat([v, dc], axis=1)
             return cycle_df
         else:
             return dc, v
 
     def get_ccap(
         self,
         cycle=None,
         converter=None,
         mode="gravimetric",
-        return_dataframe=True,
+        as_frame=True,
         **kwargs,
     ):
         """Returns charge-capacity and voltage for the selected cycle.
         Args:
             cycle (int): cycle number.
             converter (float): a multiplication factor that converts the values to specific values (i.e.
                 from Ah to mAh/g). If not provided (or None), the factor is obtained from the
                 self.get_converter_to_specific() method.
             mode (string): 'gravimetric', 'areal' or 'absolute'. Defaults to 'gravimetric'.
                 Used if converter is not provided (or None).
-            return_dataframe (bool): if True: returns pd.DataFrame instead of capacity, voltage series.
+            as_frame (bool): if True: returns pd.DataFrame instead of capacity, voltage series.
         Returns:
             charge_capacity, voltage (pandas.Series or pandas.DataFrame if return_dataframe is True).
 
         """
 
         if converter is None:
             converter = self.get_converter_to_specific(mode=mode)
         cc, v = self._get_cap(cycle, "charge", converter=converter, **kwargs)
 
-        if return_dataframe:
+        if as_frame:
             cycle_df = pd.concat([v, cc], axis=1)
             return cycle_df
         else:
             return cc, v
 
     def get_cap(
         self,
@@ -4138,21 +4199,21 @@
         initial = True
         for current_cycle in cycle:
             error = False
             try:
                 cc, cv = self.get_ccap(
                     current_cycle,
                     converter=specific_converter,
-                    return_dataframe=False,
+                    as_frame=False,
                     **kwargs,
                 )
                 dc, dv = self.get_dcap(
                     current_cycle,
                     converter=specific_converter,
-                    return_dataframe=False,
+                    as_frame=False,
                     **kwargs,
                 )
 
             except NullData as e:
                 error = True
                 logging.debug(e)
                 if not ignore_errors:
@@ -4393,15 +4454,15 @@
         self,
         cycles=None,
         direction="up",
         remove_first=False,
         interpolated=False,
         dx=None,
         number_of_points=None,
-    ):
+    ) -> pd.DataFrame:
         """get the open circuit voltage relaxation curves.
 
         Args:
             cycles (list of ints or None): the cycles to extract from
                 (selects all if not given).
             direction ("up", "down", or "both"): extract only relaxations that
                 is performed during discharge for "up" (because then the
@@ -4487,26 +4548,14 @@
         if steptable is None:
             d = self.data.raw
             no_cycles = np.amax(d[self.headers_normal.cycle_index_txt])
         else:
             no_cycles = np.amax(steptable[self.headers_step_table.cycle])
         return no_cycles
 
-    def get_cycle_numbers_old(self, steptable=None):
-        """Get a list containing all the cycle numbers in the test."""
-        logging.debug("getting cycle numbers")
-        if steptable is None:
-            d = self.data.raw
-            cycles = d[self.headers_normal.cycle_index_txt].dropna().unique()
-        else:
-            logging.debug("steptable is not none")
-            cycles = steptable[self.headers_step_table.cycle].dropna().unique()
-        logging.debug(f"got {len(cycles)} cycle numbers")
-        return cycles
-
     def get_cycle_numbers(
         self,
         steptable=None,
         rate=None,
         rate_on=None,
         rate_std=None,
         rate_column=None,
@@ -4621,23 +4670,63 @@
         if convert_charge_units:
             conversion_factor_charge = Q(1, self.cellpy_units["charge"]) / Q(
                 1, self.data.raw_units["charge"]
             )
         else:
             conversion_factor_charge = 1.0
 
-        absolute_value = (
-            (value * conversion_factor_charge * specific).to_reduced_units().to("Ah")
-        )
+        try:
+            absolute_value = (
+                (value * conversion_factor_charge * specific)
+                .to_reduced_units()
+                .to("Ah")
+            )
+        except DimensionalityError as e:
+            print(" DimensionalityError ".center(80, "="))
+            print("Could not convert nominal capacity to absolute value!")
+            print(
+                "This is probably because the nominal capacity is given in "
+                "different unit than the given specifics."
+            )
+            print(
+                " - Maybe you have given nominal capacity in mAh/cm**2 and your "
+                "specifics is set to 'gravimetric'?"
+            )
+            print(
+                " - Maybe you have given nominal capacity in mAh/g and your "
+                "specifics is set to 'areal'?"
+            )
+            print("Please check your input parameters!")
+            print(
+                "\n[hint 1] try to set the parameter 'nom_cap_specifics' in the get function:\n"
+            )
+            print(
+                "    c = cellpy.get(filename, area=1.55, nom_cap='1.2 mAh/cm**2', nom_cap_specifics='areal')"
+            )
+            print(
+                "\n[hint 2] try to set it on the cellpy object directly after loading, "
+                "\n  but before processing (making the step-table etc):\n"
+            )
+            print("    c = cellpy.get(filename, auto_summary=False)")
+            print("    c.nom_cap_specifics = 'areal'")
+            print("    ... # set other stuff if needed")
+            print("    c.make_step_table()")
+            print("    c.make_summary()")
+            print("\nRe-raising the exception.")
+            print(80 * "=")
+            raise e
+
         if self.debug:
             print(f"{self.mass=}")
             print(f"{self.active_electrode_area=}")
             print(f"{self.nom_cap=}")
             print(f"{self.cellpy_units=}")
-            print(f"nominal capacity: {value} [{self.cellpy_units.nominal_capacity}] -> {absolute_value:.3f} [Ah]")
+            print(
+                f"nominal capacity: {value} [{self.cellpy_units.nominal_capacity}] -> {absolute_value:.3f} [Ah]"
+            )
             print(80 * "=")
         return absolute_value.m
 
     def with_cellpy_unit(self, parameter, as_str=False):
         """Return quantity as `pint.Quantity` object."""
         _look_up = {
             "nom_cap": "nominal_capacity",
@@ -4702,14 +4791,32 @@
             else:
                 value = Q(value)
 
         value = value.to(self.cellpy_units[physical_property])
 
         return value.m
 
+    def unit_scaler_from_raw(self, unit, physical_property):
+        """Get the conversion factor going from raw to given unit.
+
+        Args:
+            unit (str): what you want to convert to
+            physical_property (str): what this value is a measure of
+                (must correspond to one of the keys in the CellpyUnits class).
+
+        Returns (numeric):
+            conversion factor (scaler)
+        """
+        logging.debug(f"value {unit} is a pint quantity? {isinstance(unit, Quantity)}")
+
+        old_unit = self.data.raw_units[physical_property]
+        value = Q(1, old_unit)
+        value = value.to(unit)
+        return value.m
+
     def get_converter_to_specific(
         self,
         dataset: Data = None,
         value: float = None,
         from_units: CellpyUnits = None,
         to_units: CellpyUnits = None,
         mode: str = "gravimetric",
@@ -4826,33 +4933,32 @@
             else:
                 logging.debug("_set_run_attribute: this set is empty")
 
     def set_mass(self, mass, validated=None):
         """Sets the mass (masses) for the test (datasets)."""
 
         warnings.warn(
-            "This function is deprecated. " "Use the setter instead (mass = value).",
+            "This function is deprecated. Use the setter instead (mass = value).",
             DeprecationWarning,
             stacklevel=2,
         )
         self._set_run_attribute("mass", mass, validated=validated)
 
     def set_tot_mass(self, mass, validated=None):
         warnings.warn(
-            "This function is deprecated. "
-            "Use the setter instead (tot_mass = value).",
+            "This function is deprecated. Use the setter instead (tot_mass = value).",
             DeprecationWarning,
             stacklevel=2,
         )
 
         self._set_run_attribute("tot_mass", mass, validated=validated)
 
     def set_nom_cap(self, nom_cap, validated=None):
         warnings.warn(
-            "This function is deprecated. " "Use the setter instead (nom_cap = value).",
+            "This function is deprecated. Use the setter instead (nom_cap = value).",
             DeprecationWarning,
             stacklevel=2,
         )
 
         self._set_run_attribute("nom_cap", nom_cap, validated=validated)
 
     @staticmethod
@@ -5802,15 +5908,15 @@
 
             # test[set_number].raw_data_files.append(raw_data_file)
             # test[set_number].raw_data_files_length.append(file_size)
             # return test
         # cell[set_number].raw_units = self._set_raw_units()
         # self.cells.append(cell[set_number])
         # self.status_dataset = self._validate_cell()
-        # self._invent_a_session_name()
+        # self._invent_a_cell_name()
         return self
 
 
 def get(
     filename=None,
     instrument=None,
     instrument_file=None,
@@ -5827,14 +5933,15 @@
     auto_summary=True,
     units=None,
     step_kwargs=None,
     summary_kwargs=None,
     selector=None,
     testing=False,
     refuse_copying=False,
+    initialize=False,
     debug=False,
     **kwargs,
 ):
     """Create a CellpyCell object
 
     Args:
         filename (str, os.PathLike, OtherPath, or list of raw-file names): path to file(s) to load
@@ -5856,14 +5963,16 @@
         auto_summary (bool): (re-) create summary.
         units (dict): update cellpy units (used after the file is loaded, e.g. when creating summary).
         step_kwargs (dict): sent to make_steps
         summary_kwargs (dict): sent to make_summary
         selector (dict): passed to load (when loading cellpy-files).
         testing (bool): set to True if testing (will for example prevent making .log files)
         refuse_copying (bool): set to True if you do not want to copy the raw-file before loading.
+        initialize (bool): set to True if you want to initialize the CellpyCell object (probably only
+            useful if you want to return a cellpy-file with no data in it)
         debug (bool): set to True if you want to debug the loader.
         **kwargs: sent to the loader
 
     Returns:
         CellpyCell object (if successful, None if not)
 
     Examples:
@@ -5886,33 +5995,37 @@
         >>>
         >>> # load three subsequent raw-files (of one cell) and merge them:
         >>> c = cellpy.get(["my_data_01.res", "my_data_02.res", "my_data_03.res"])
         >>>
         >>> # load a data set and get the summary charge and discharge capacities
         >>> # in Ah/g:
         >>> c = cellpy.get("my_data.res", units=dict(capacity="Ah"))
+        >>>
+        >>> # get an empty CellpyCell instance:
+        >>> c = cellpy.get()  # or c = cellpy.get(initialize=True) if you want to initialize it.
 
     """
     from cellpy import log
 
-    db_readers = ["arbin_sql"]
+    db_readers = ["arbin_sql", "arbin_sql_7"]
     instruments_with_colliding_file_suffix = ["arbin_sql_h5"]
 
     step_kwargs = step_kwargs or {}
     summary_kwargs = summary_kwargs or {}
     load_cellpy_file = False
     logging_mode = "DEBUG" if testing else logging_mode
     log.setup_logging(default_level=logging_mode, testing=testing)
     logging.debug("-------running-get--------")
-    cellpy_instance = CellpyCell(debug=debug)
+    cellpy_instance = CellpyCell(debug=debug, initialize=initialize)
     logging.debug(f"created CellpyCell instance")
 
     logging.debug(f"{cellpy_file=}")
     logging.debug(f"{filename=}")
 
+    # used if all you want is an empty CellpyCell object
     if filename is None:
         if cellpy_file is None:
             logging.info("Running cellpy.get without a filename")
             logging.info("Returning an empty CellpyCell object.")
             cellpy_instance = _update_meta(
                 cellpy_instance,
                 cycle_mode=cycle_mode,
@@ -5974,31 +6087,32 @@
 
     elif instrument is not None:
         logging.debug(f"got instrument in stead of instrument file, {instrument=}")
         model = kwargs.pop("model", None)
         cellpy_instance.set_instrument(instrument=instrument, model=model, **kwargs)
 
     is_a_file = True
-    if cellpy_instance.tester not in db_readers:
+    if cellpy_instance.tester in db_readers:
         is_a_file = False
 
     logging.info(f"Loading raw-file: {filename}")
     cellpy_instance.from_raw(
         filename, is_a_file=is_a_file, refuse_copying=refuse_copying, **kwargs
     )
 
     if not cellpy_instance:
         print("Could not load file: check log!")
         print("Returning None")
         return
 
     # fix for allowing for setting nom_cap_specifics the "old" way:
-    nom_cap_specifics = summary_kwargs.pop("nom_cap_specifics", None)
     if nom_cap_specifics is None:
-        nom_cap_specifics = step_kwargs.pop("nom_cap_specifics", None)
+        nom_cap_specifics = summary_kwargs.pop("nom_cap_specifics", None)
+        if nom_cap_specifics is None:
+            nom_cap_specifics = step_kwargs.pop("nom_cap_specifics", None)
 
     cellpy_instance = _update_meta(
         cellpy_instance,
         cycle_mode=cycle_mode,
         mass=mass,
         nominal_capacity=nominal_capacity,
         nom_cap_specifics=nom_cap_specifics,
@@ -6025,15 +6139,21 @@
     nominal_capacity=None,
     nom_cap_specifics=None,
     area=None,
     loading=None,
     estimate_area=None,
     units=None,
 ):
-    # TODO: make this a method on CellpyCell
+    """Used by get to update metadata in the CellpyCell object."""
+    # Note: this is a bit messy, but it is a quick fix for now.
+    #       I will clean it up later.
+    # Note: if you want to add more metadata or similar for use by the get function,
+    #       please also add a property to the CellpyCell class (e.g. don't update
+    #       the data object directly, especially if handling units).
+
     if cycle_mode is not None:
         logging.debug("Setting cycle mode")
         cellpy_instance.cycle_mode = cycle_mode
 
     if nom_cap_specifics is not None:
         logging.debug("Setting nom_cap_specifics as given")
         cellpy_instance.nom_cap_specifics = nom_cap_specifics
@@ -6044,30 +6164,34 @@
 
     if mass is not None:
         logging.info(f"Setting mass: {mass}")
         cellpy_instance.mass = mass
 
     if nominal_capacity is not None:
         logging.info(f"Setting nominal capacity: {nominal_capacity}")
-        if nom_cap_specifics is not None and not isinstance(nominal_capacity, numbers.Number):
-            logging.info("Providing nominal capacity as string might override the given nom_cap_specifics")
+        if nom_cap_specifics is not None and not isinstance(
+            nominal_capacity, numbers.Number
+        ):
+            logging.info(
+                "Providing nominal capacity as string might override the given nom_cap_specifics"
+            )
         cellpy_instance.nom_cap = nominal_capacity
 
     if area is not None:
         logging.debug(f"got area: {area}")
-        cellpy_instance.data.meta_common.active_electrode_area = area
+        cellpy_instance.active_electrode_area = area
 
     elif loading and estimate_area:
         logging.debug("-------------AREA-CALC----------------")
         logging.debug(f"got loading: {logging}")
         area = cellpy_instance.data.mass / loading
         logging.debug(
             f"calculating area from loading ({loading}) and mass ({cellpy_instance.data.mass}): {area}"
         )
-        cellpy_instance.data.meta_common.active_electrode_area = area
+        cellpy_instance.active_electrode_area = area
     else:
         logging.debug("using default area")
 
     return cellpy_instance
 
 
 # ============== Internal tests =================
@@ -6177,32 +6301,48 @@
     # print(c.data.summary.columns)
     # print(c.data.steps.columns)
     # print(c.data.raw.columns)
 
 
 def load_and_save_to_excel():
     from pathlib import Path
+    from pprint import pprint
 
     print(" loading cellpy file and saving to excel ".center(80, "="))
 
     raw_file = Path("../../testdata/data/20160805_test001_45_cc_01.res")
     cellpy_file = Path("../../tmp/20160805_test001_45_cc.h5")
-    excel_file = Path("../../tmp/20160805_test001_45_cc.xlsx")
-
-    c = get(raw_file, area=1.55, nominal_capacity=2000, summary_kwargs={"nom_cap_specifics": "areal"}, debug=True)
-    c = get(raw_file, mass=1.55, nominal_capacity="3579 mAh/g", debug=True)
-    c = get(raw_file, area=1.55, nominal_capacity=2000, nom_cap_specifics="areal", debug=True)
-    print("loaded ...")
-    c.to_excel(excel_file)
-    print("saved ...")
+    # excel_file1 = Path("../../tmp/01_gravimetric_old_20160805_test001_45_cc.xlsx")
+    excel_file2 = Path("../../tmp/02_gravimetric_20160805_test001_45_cc.xlsx")
+    # excel_file3 = Path("../../tmp/03_areal_20160805_test001_45_cc.xlsx")
+    # excel_file4 = Path("../../tmp/04_areal_20160805_test001_45_cc.xlsx")
+    # excel_file5 = Path("../../tmp/05_areal_20160805_test001_45_cc.xlsx")
+
+    # c = get(raw_file, area=1.55, cycle_mode="anode", nominal_capacity=2.0, summary_kwargs={"nom_cap_specifics": "areal"}, debug=True)
+    # c.to_excel(excel_file1, cycles=True)
+    c = get(
+        raw_file,
+        mass=1.55,
+        cycle_mode="anode",
+        nominal_capacity="3579 mAh/g",
+        debug=True,
+    )
+    c.to_excel(excel_file2, cycles=True)
+    # c = get(raw_file, area=1.55, cycle_mode="anode", nominal_capacity=2.0, nom_cap_specifics="areal", debug=True)
+    # c.to_excel(excel_file3, cycles=True)
+    # c = get(raw_file, area="1.55 cm**2", cycle_mode="anode", nominal_capacity="2.0 mAh/cm**2", nom_cap_specifics="areal", debug=True)
+    # c.to_excel(excel_file4, cycles=True)
+    # print("saved ...")
     #
     # c.save(cellpy_file)
     # c2 = get(cellpy_file)
+    # pprint(c2.cellpy_units)
+    # pprint(c2.data.meta_common)
     # print("loaded again ...")
-    # c2.to_excel(excel_file, raw=True, cycles=True)
+    # c2.to_excel(excel_file5, raw=True, cycles=True)
     # print("saved again ...")
 
 
 def check_excel():
     import openpyxl
     from openpyxl.styles import Border, Side
     import pandas as pd
@@ -6231,9 +6371,57 @@
             print(cell)
             cell.border = border
             cell.fill = fill
 
     print("done")
 
 
+def check_new_dot_get_methods():
+    from pathlib import Path
+    from pprint import pprint
+    import numpy as np
+
+    print(" loading file and checking the .get methods ".center(80, "="))
+    raw_file = Path("../../testdata/data/20160805_test001_45_cc_01.res")
+    c = get(
+        raw_file,
+        mass=1.55,
+        cycle_mode="anode",
+        nominal_capacity="3579 mAh/g",
+        debug=True,
+    )
+    # pprint(c.headers_normal)
+    cycles_a = [1, 2, 3]
+    cycles_b = np.array([1, 2, 3])
+    cycles_c = [1, 2, 3]
+    a = c.get_timestamp(cycles_a, with_index=True, units="raw")
+    print(f"{cycles_a=} raw".center(80, "-"))
+    pprint(a)
+
+    a = c.get_timestamp(cycles_a, units="seconds")
+    print(f"{cycles_a=} seconds".center(80, "-"))
+    pprint(a)
+
+    a = c.get_timestamp(cycles_a, units="minutes")
+    print(f"{cycles_a=} minutes".center(80, "-"))
+    pprint(a)
+
+    a = c.get_timestamp(cycles_a, units="hours")
+    print(f"{cycles_a=} hours".center(80, "-"))
+    pprint(a)
+
+    a = c.get_timestamp(cycles_a, in_minutes=True, units="hours")
+    print(f"{cycles_a=} hours".center(80, "-"))
+    pprint(a)
+
+    #
+    #
+    # print(f"{cycles_b=}".center(80, "-"))
+    # b = c.get_timestamp(cycles_b)
+    # pprint(b)
+    # print(f"{cycles_c=}".center(80, "-"))
+    # c = c.get_timestamp(cycles_c, with_index=False, as_frame=False)
+    # pprint(c)
+
+
 if __name__ == "__main__":
-    load_and_save_to_excel()
+    check_new_dot_get_methods()
```

### Comparing `cellpy-1.0.0a9/cellpy/readers/core.py` & `cellpy-1.0.0b0/cellpy/readers/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,14 +352,15 @@
         self.raw_limits = get_default_raw_limits()
 
         self.raw = pd.DataFrame()
         self.summary = pd.DataFrame()
         self.steps = pd.DataFrame()
 
         self.meta_common = CellpyMetaCommon()
+        # TODO: v2.0 consider making this a list of several CellpyMetaIndividualTest
         self.meta_test_dependent = CellpyMetaIndividualTest()
 
         # custom meta-data
         for k in kwargs:
             if hasattr(self, k):
                 setattr(self, k, kwargs[k])
 
@@ -422,17 +423,17 @@
 
     @property
     def nom_cap(self):
         return self.meta_common.nom_cap
 
     @nom_cap.setter
     def nom_cap(self, value):
-        if value < 1.0:
+        if value < 0.1:
             warnings.warn(
-                f"POSSIBLE BUG: NOMINAL CAPACITY LESS THAN 1.0 ({value}).",
+                f"POSSIBLE BUG: NOMINAL CAPACITY LESS THAN 0.1 ({value}).",
                 DeprecationWarning,
                 stacklevel=2,
             )
         self.meta_common.nom_cap = value  # nominal capacity
 
     @staticmethod
     def _header_str(hdr):
@@ -490,16 +491,15 @@
             txt += str(self.steps.describe())
             txt += str(self.steps.head())
         except (AttributeError, ValueError):
             txt += "EMPTY (Not processed yet)\n"
 
         txt += self._header_str("RAW UNITS")
         try:
-            txt += str(self.raw.describe())
-            txt += str(self.raw.head())
+            txt += str(self.raw_units)
         except (AttributeError, ValueError):
             txt += "EMPTY (Not processed yet)\n"
         return txt
 
     def populate_defaults(self):
         # modify this method upon need
         logging.debug("checking and populating defaults for the cell")
@@ -849,23 +849,23 @@
         try:
             if direction == "charge":
                 q, v = cell.get_ccap(
                     cycle,
                     trim_taper_steps=trim_taper_steps,
                     steps_to_skip=steps_to_skip,
                     steptable=steptable,
-                    return_dataframe=False,
+                    as_frame=False,
                 )
             else:
                 q, v = cell.get_dcap(
                     cycle,
                     trim_taper_steps=trim_taper_steps,
                     steps_to_skip=steps_to_skip,
                     steptable=steptable,
-                    return_dataframe=False,
+                    as_frame=False,
                 )
 
         except NullData as e:
             logging.warning(e)
             d = pd.DataFrame()
             d.name = cycle
             charge_list.append(d)
```

### Comparing `cellpy-1.0.0a9/cellpy/readers/dbreader.py` & `cellpy-1.0.0b0/cellpy/readers/dbreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/filefinder.py` & `cellpy-1.0.0b0/cellpy/readers/filefinder.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/arbin_res.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/arbin_res.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/arbin_sql.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/arbin_sql.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/arbin_sql_7.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/arbin_sql_7.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/arbin_sql_csv.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/arbin_sql_csv.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/arbin_sql_h5.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/arbin_sql_h5.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/arbin_sql_xlsx.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/arbin_sql_xlsx.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/base.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/base.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/biologics_mpr.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/biologics_mpr.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/configurations/__init__.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/configurations/maccor_txt_four.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/configurations/maccor_txt_four.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/configurations/maccor_txt_one.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/configurations/maccor_txt_one.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/configurations/maccor_txt_three.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/configurations/maccor_txt_three.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/configurations/maccor_txt_two.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/configurations/maccor_txt_two.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/configurations/maccor_txt_zero.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/configurations/maccor_txt_zero.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/configurations/neware_txt_zero.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/configurations/neware_txt_zero.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/custom.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/custom.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/ext_nda_reader.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/ext_nda_reader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/local_instrument.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/local_instrument.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/maccor_txt.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/maccor_txt.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/neware_txt.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/neware_txt.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/pec_csv.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/pec_csv.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/processors/post_processors.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/processors/post_processors.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/instruments/processors/pre_processors.py` & `cellpy-1.0.0b0/cellpy/readers/instruments/processors/pre_processors.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/readers/sql_dbreader.py` & `cellpy-1.0.0b0/cellpy/readers/sql_dbreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/utils/batch.py` & `cellpy-1.0.0b0/cellpy/utils/batch.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_analyzers.py` & `cellpy-1.0.0b0/cellpy/utils/batch_tools/batch_analyzers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_core.py` & `cellpy-1.0.0b0/cellpy/utils/batch_tools/batch_core.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_experiments.py` & `cellpy-1.0.0b0/cellpy/utils/batch_tools/batch_experiments.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_exporters.py` & `cellpy-1.0.0b0/cellpy/utils/batch_tools/batch_exporters.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_helpers.py` & `cellpy-1.0.0b0/cellpy/utils/batch_tools/batch_helpers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_journals.py` & `cellpy-1.0.0b0/cellpy/utils/batch_tools/batch_journals.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_plotters.py` & `cellpy-1.0.0b0/cellpy/utils/batch_tools/batch_plotters.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/utils/batch_tools/dumpers.py` & `cellpy-1.0.0b0/cellpy/utils/batch_tools/dumpers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/utils/batch_tools/engines.py` & `cellpy-1.0.0b0/cellpy/utils/batch_tools/engines.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/utils/batch_tools/sqlite_from_excel_db.py` & `cellpy-1.0.0b0/cellpy/utils/batch_tools/sqlite_from_excel_db.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/utils/collectors_old.py` & `cellpy-1.0.0b0/cellpy/utils/collectors_old.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1309 +1,1309 @@
-"""Collectors are used for simplifying plotting and exporting batch objects."""
-
-import textwrap
-from pprint import pprint
-from pathlib import Path
-from typing import Any
-import inspect
-import logging
-
-import pandas as pd
-
-import cellpy
-from cellpy.readers.core import group_by_interpolate
-from cellpy.utils.batch import Batch
-from cellpy.utils.helpers import concatenate_summaries
-from cellpy.utils.plotutils import plot_concatenated
-from cellpy.utils import ica
-
-try:
-    import holoviews as hv
-    from holoviews.core.io import Pickler
-    from holoviews import opts
-
-    HOLOVIEWS_AVAILABLE = True
-except ImportError:
-    print("Could not import Holoviews. Plotting will be disabled.")
-    HOLOVIEWS_AVAILABLE = False
-
-CELLPY_MINIMUM_VERSION = "0.4.3"
-
-
-def _setup():
-    _welcome_message()
-    _register_holoviews_renderers()
-
-
-def _welcome_message():
-    cellpy_version = cellpy.__version__
-    logging.info(f"cellpy version: {cellpy_version}")
-    logging.info(f"collectors need at least: {CELLPY_MINIMUM_VERSION}")
-
-
-def _register_holoviews_renderers(extensions=None):
-    if HOLOVIEWS_AVAILABLE:
-        if extensions is None:
-            extensions = "bokeh", "matplotlib"
-        logging.info(
-            f"Registering Holoviews extensions {extensions} for the cellpy collectors."
-        )
-        hv.extension(*extensions)
-    else:
-        logging.info(
-            "Could not import Holoviews. Your collectors will not be able to make figures."
-        )
-
-
-def _set_holoviews_renderer(extension=None):
-    if HOLOVIEWS_AVAILABLE:
-        extension = extension.lower()
-        current_backend = hv.Store.current_backend
-        if not extension == current_backend:
-            logging.info(f"switching backend to {extension}")
-            hv.Store.set_current_backend(extension)
-
-
-def _get_current_holoviews_renderer():
-    return hv.Store.current_backend
-
-
-_setup()
-
-
-class BatchCollector:
-    collector_name: str = None
-    data: pd.DataFrame = None
-    figure: Any = None
-    name: str = None
-    nick: str = None
-    autorun: bool = True
-    figure_directory: Path = Path("out")
-    data_directory: Path = Path("data/processed/")
-    renderer: Any = None
-
-    # override default arguments:
-    elevated_data_collector_arguments: dict = None
-    elevated_plotter_arguments: dict = None
-
-    # defaults (and used also when resetting):
-    _default_data_collector_arguments = {}
-    _default_plotter_arguments = {}
-
-    # templates override everything when using autorun:
-    _templates = {
-        "bokeh": [],
-        "matplotlib": [],
-        "plotly": [],
-    }
-
-    def __init__(
-        self,
-        b,
-        data_collector,
-        plotter,
-        collector_name=None,
-        name=None,
-        nick=None,
-        autorun=True,
-        use_templates=True,
-        elevated_data_collector_arguments=None,
-        elevated_plotter_arguments=None,
-        data_collector_arguments: dict = None,
-        plotter_arguments: dict = None,
-        **kwargs,
-    ):
-        """Update both the collected data and the plot(s).
-        Args:
-            b (cellpy.utils.Batch): the batch object.
-            data_collector (callable): method that collects the data.
-            plotter (callable): method that crates the plots.
-            collector_name (str): name of collector.
-            name (str or bool): name used for auto-generating filenames etc.
-            autorun (bool): run collector and plotter immediately if True.
-            use_templates (bool): also apply template(s) in autorun mode if True.
-            elevated_data_collector_arguments (dict): arguments picked up by the child class' initializer.
-            elevated_plotter_arguments (dict): arguments picked up by the child class' initializer.
-            data_collector_arguments (dict): keyword arguments sent to the data collector.
-            plotter_arguments (dict): keyword arguments sent to the plotter.
-            update_name (bool): update the name (using automatic name generation) based on new settings.
-            **kwargs: set Collector attributes.
-        """
-        self.b = b
-        self.data_collector = data_collector
-        self.plotter = plotter
-        self.nick = nick
-        self.collector_name = collector_name or "base"
-
-        # Arguments given as default arguments in the subclass have "low" priority (below elevated arguments at least):
-        self._data_collector_arguments = self._default_data_collector_arguments.copy()
-        self._plotter_arguments = self._default_plotter_arguments.copy()
-        self._update_arguments(data_collector_arguments, plotter_arguments)
-
-        # Elevated arguments have preference above the data_collector and plotter argument dicts:
-        self._parse_elevated_arguments(
-            elevated_data_collector_arguments, elevated_plotter_arguments
-        )
-
-        self._set_attributes(**kwargs)
-
-        if nick is None:
-            self.nick = b.name
-
-        if name is None:
-            name = self.generate_name()
-        self.name = name
-
-        if autorun:
-            self.update(update_name=False)
-            if use_templates:
-                self.apply_templates()
-
-    @property
-    def data_collector_arguments(self):
-        return self._data_collector_arguments
-
-    @data_collector_arguments.setter
-    def data_collector_arguments(self, argument_dict: dict):
-        if argument_dict is not None:
-            self._data_collector_arguments = {
-                **self._data_collector_arguments,
-                **argument_dict,
-            }
-
-    @property
-    def plotter_arguments(self):
-        return self._plotter_arguments
-
-    @plotter_arguments.setter
-    def plotter_arguments(self, argument_dict: dict):
-        if argument_dict is not None:
-            self._plotter_arguments = {**self._plotter_arguments, **argument_dict}
-
-    def __str__(self):
-        class_name = self.__class__.__name__
-
-        txt = f"{class_name}\n{len(class_name) * '='}\n\n"
-        txt += "Attributes:\n"
-        txt += "-----------\n"
-        txt += f" -collector_name: {self.collector_name}\n"
-        txt += f" -autorun: {self.autorun}\n"
-        txt += f" -name: {self.name}\n"
-        txt += f" -nick: {self.nick}\n"
-        txt += f" -csv_include_index: {self.csv_include_index}\n"
-        txt += f" -csv_layout: {self.csv_layout}\n"
-        txt += f" -sep: {self.sep}\n"
-        txt += f" -toolbar: {self.toolbar}\n"
-        txt += f" -figure_directory: {self.figure_directory}\n"
-        txt += f" -data_directory: {self.data_directory}\n"
-        txt += f" -batch-instance: {self.b.name}\n"
-        txt += f" -data_collector_arguments: {self.data_collector_arguments}\n"
-        txt += f" -plotter_arguments: {self.plotter_arguments}\n"
-
-        txt += "\nfigure:\n"
-        txt += ".......\n"
-        txt += f"{self.figure}\n"
-
-        txt += "\ndata:\n"
-        txt += ".....\n"
-        txt += f"{self.data}\n"
-
-        txt += "\nData collector:\n"
-        txt += "---------------\n"
-        data_name = self.data_collector.__name__
-        data_sig = inspect.signature(self.data_collector)
-        data_doc = inspect.getdoc(self.data_collector)
-        txt = f"{txt}{data_name}"
-        txt = f"{txt}{data_sig}\n"
-        txt = f"{txt}\n{data_doc}\n"
-
-        txt += "\nPlotter:\n"
-        txt += "--------\n"
-        plotter_name = self.plotter.__name__
-        plotter_sig = inspect.signature(self.plotter)
-        plotter_doc = inspect.getdoc(self.plotter)
-        txt = f"{txt}{plotter_name}"
-        txt = f"{txt}{plotter_sig}\n"
-        txt = f"{txt}\n{plotter_doc}\n"
-
-        return txt
-
-    def _repr_html_(self):
-        class_name = self.__class__.__name__
-        txt = f"<h2>{class_name}</h2> id={hex(id(self))}"
-        _txt = self.__str__().replace("\n", "<br>")
-        txt += f"<blockquote><code>{_txt}</></blockquote>"
-
-        return txt
-
-    def _set_attributes(self, **kwargs):
-        self.sep = kwargs.get("sep", ";")
-        self.csv_include_index = kwargs.get("csv_include_index", True)
-        self.csv_layout = kwargs.get("csv_layout", "long")
-        self.dpi = kwargs.get("dpi", 200)
-        self.toolbar = kwargs.get("toolbar", True)
-
-    def generate_name(self):
-        names = ["collector", self.collector_name]
-        if self.nick:
-            names.insert(0, self.nick)
-        name = "_".join(names)
-        return name
-
-    def _parse_elevated_arguments(
-        self, data_collector_arguments: dict = None, plotter_arguments: dict = None
-    ):
-        if data_collector_arguments is not None:
-            logging.info(f"Updating elevated arguments")
-            elevated_data_collector_arguments = {}
-            for k, v in data_collector_arguments.items():
-                if v is not None:
-                    elevated_data_collector_arguments[k] = v
-            self._update_arguments(
-                elevated_data_collector_arguments, None, set_as_defaults=True
-            )
-
-        if plotter_arguments is not None:
-            logging.info(f"Updating elevated arguments")
-            elevated_plotter_arguments = {}
-            for k, v in plotter_arguments.items():
-                if v is not None:
-                    elevated_plotter_arguments[k] = v
-
-            self._update_arguments(
-                None, elevated_plotter_arguments, set_as_defaults=True
-            )
-
-    def _update_arguments(
-        self,
-        data_collector_arguments: dict = None,
-        plotter_arguments: dict = None,
-        set_as_defaults=False,
-    ):
-        self.data_collector_arguments = data_collector_arguments
-        self.plotter_arguments = plotter_arguments
-        logging.info(f"**data_collector_arguments: {self.data_collector_arguments}")
-        logging.info(f"**plotter_arguments: {self.plotter_arguments}")
-
-        # setting defaults also (py3.6 compatible):
-        if set_as_defaults:
-            logging.info("updating defaults for current instance")
-            if data_collector_arguments is not None:
-                self._default_data_collector_arguments = {
-                    **self._default_data_collector_arguments,
-                    **data_collector_arguments,
-                }
-            if plotter_arguments is not None:
-                self._default_plotter_arguments = {
-                    **self._default_plotter_arguments,
-                    **plotter_arguments,
-                }
-
-    def reset_arguments(
-        self, data_collector_arguments: dict = None, plotter_arguments: dict = None
-    ):
-        """Reset the arguments to the defaults.
-        Args:
-            data_collector_arguments (dict): optional additional keyword arguments for the data collector.
-            plotter_arguments (dict): optional additional keyword arguments for the plotter.
-        """
-        self._data_collector_arguments = self._default_data_collector_arguments.copy()
-        self._plotter_arguments = self._default_plotter_arguments.copy()
-        self._update_arguments(data_collector_arguments, plotter_arguments)
-
-    def update(
-        self,
-        data_collector_arguments: dict = None,
-        plotter_arguments: dict = None,
-        reset: bool = False,
-        update_data: bool = False,
-        update_name: bool = False,
-        update_plot: bool = True,
-    ):
-        """Update both the collected data and the plot(s).
-        Args:
-            data_collector_arguments (dict): keyword arguments sent to the data collector.
-            plotter_arguments (dict): keyword arguments sent to the plotter.
-            reset (bool): reset the arguments first.
-            update_data (bool): update the data before updating the plot even if data has been collected before.
-            update_name (bool): update the name (using automatic name generation) based on new settings.
-            update_plot (bool): update the plot.
-        """
-        if reset:
-            self.reset_arguments(data_collector_arguments, plotter_arguments)
-        else:
-            self._update_arguments(data_collector_arguments, plotter_arguments)
-        if update_data or self.data is None:
-            try:
-                self.data = self.data_collector(self.b, **self.data_collector_arguments)
-            except TypeError as e:
-                print("Type error:", e)
-                print("Registered data_collector_arguments:")
-                pprint(self.data_collector_arguments)
-                print("Hint: fix it and then re-run using reset=True")
-                return
-        if update_plot:
-            if HOLOVIEWS_AVAILABLE:
-                _set_holoviews_renderer(self.plotter_arguments.get("extension"))
-                try:
-                    self.figure = self.plotter(
-                        self.data, journal=self.b.journal, **self.plotter_arguments
-                    )
-                except TypeError as e:
-                    print("Type error:", e)
-                    print("Registered plotter_arguments:")
-                    pprint(self.plotter_arguments)
-                    print("Hint: fix it and then re-run using reset=True")
-                    return
-
-        if update_name:
-            self.name = self.generate_name()
-
-    def _dynamic_update_template_parameter(self, hv_opt, extension, *args, **kwargs):
-        return hv_opt
-
-    def _register_template(self, hv_opts, extension="bokeh", *args, **kwargs):
-        """Register template for given extension.
-
-        It is also possible to set the options directly in the constructor of the
-        class. But it is recommended to use this method instead to allow for
-        sanitation of the options in the templates
-
-        Args:
-            hv_opts: list of holoviews.core.options.Options- instances
-                e.g. [hv.opts.Curve(xlim=(0,2)), hv.opts.NdLayout(title="Super plot")]
-            extension: Holoviews backend ("matplotlib", "bokeh", or "plotly")
-
-        Returns:
-            None
-        """
-        if extension not in ["bokeh", "matplotlib", "plotly"]:
-            print(f"extension='{extension}' is not supported.")
-        if not isinstance(hv_opts, (list, tuple)):
-            hv_opts = [hv_opts]
-
-        cleaned_hv_opts = []
-        for o in hv_opts:
-            logging.debug(f"Setting prm: {o}")
-            o = self._dynamic_update_template_parameter(o, extension, *args, **kwargs)
-            # ensure all options are registered with correct backend:
-            o.kwargs["backend"] = extension
-            cleaned_hv_opts.append(o)
-
-        self._templates[extension] = cleaned_hv_opts
-
-    def apply_templates(self):
-        if not self._figure_valid():
-            return
-
-        for backend, hv_opt in self._templates.items():
-            try:
-                if len(hv_opt):
-                    print(f"Applying template for {backend}:{hv_opt}")
-                    self.figure = self._set_hv_opts(hv_opt)
-            except TypeError:
-                print("possible bug in apply_template experienced")
-                print(self._templates)
-
-    def _figure_valid(self):
-        # TODO: create a decorator
-        if self.figure is None:
-            print("No figure to show!")
-            return False
-        if not HOLOVIEWS_AVAILABLE:
-            print("Requires Holoviews - please install it first!")
-            return False
-        return True
-
-    def _set_hv_opts(self, hv_opts):
-        if hv_opts is None:
-            return self.figure
-        if isinstance(hv_opts, (tuple, list)):
-            return self.figure.options(*hv_opts)
-        else:
-            return self.figure.options(hv_opts)
-
-    def show(self, hv_opts=None):
-        if not self._figure_valid():
-            return
-
-        print(f"figure name: {self.name}")
-        return self._set_hv_opts(hv_opts)
-
-    def redraw(self, hv_opts=None, extension=None):
-        print("EXPERIMENTAL FEATURE! THIS MIGHT NOT WORK PROPERLY YET")
-        if not self._figure_valid():
-            return
-
-        if extension is not None:
-            _set_holoviews_renderer(extension)
-
-        print(f"figure name: {self.name}")
-        self.figure = self._set_hv_opts(hv_opts)
-        return self.figure
-
-    def render(self):
-        print("Not implemented yet!")
-
-    def preprocess_data_for_csv(self):
-        print(f"the data layout {self.csv_layout} is not supported yet!")
-        return self.data
-
-    def to_csv(self, serial_number=None):
-        filename = self._output_path(serial_number)
-        filename = filename.with_suffix(".csv")
-        if self.csv_layout != "long":
-            data = self.preprocess_data_for_csv()
-        else:
-            data = self.data
-
-        data.to_csv(
-            filename,
-            sep=self.sep,
-            index=self.csv_include_index,
-        )
-        print(f"saved csv file: {filename}")
-
-    def to_image_files(self, serial_number=None):
-        if not self._figure_valid():
-            return
-        filename_pre = self._output_path(serial_number)
-
-        filename_hv = filename_pre.with_suffix(".html")
-        hv.save(
-            self.figure,
-            filename_hv,
-            toolbar=self.toolbar,
-        )
-        print(f"saved file: {filename_hv}")
-
-        filename_png = filename_pre.with_suffix(".png")
-        try:
-            current_renderer = _get_current_holoviews_renderer()
-
-            _set_holoviews_renderer("matplotlib")
-            self.figure.opts(hv.opts.NdOverlay(legend_position="right"))
-            hv.save(
-                self.figure,
-                filename_png,
-                dpi=300,
-            )
-            print(f"saved file: {filename_png}")
-        except Exception as e:
-            print("Could not save png-file.")
-            print(e)
-        finally:
-            _set_holoviews_renderer(current_renderer)
-
-    def save(self, serial_number=None):
-        self.to_csv(serial_number=serial_number)
-
-        if self._figure_valid():
-            filename = self._output_path(serial_number)
-            filename = filename.with_suffix(".hvz")
-            try:
-                Pickler.save(
-                    self.figure,
-                    filename,
-                )
-                print(f"pickled holoviews file: {filename}")
-            except TypeError as e:
-                print("could not save as hvz file")
-            self.to_image_files(serial_number=serial_number)
-
-    def _output_path(self, serial_number=None):
-        d = Path(self.figure_directory)
-        n = self.name
-        if serial_number is not None:
-            n = f"{n}_{serial_number:03}"
-        f = d / n
-        return f
-
-
-# TODO: allow for storing more than one figure setup pr collector
-#    It is time-consuming and memory demanding to re-collect the data
-#    for each time we need a new figure for the collector. We should
-#    allow for creating multiple figures within one collector or for
-#    sharing (passing) collected data. One solution might be to extend
-#    the capabilities of the base class. Another solution might be to
-#    add another sub-class in the chain from the base class to the actual one:
-class BatchMultiFigureCollector(BatchCollector):
-    pass
-
-
-def pick_named_cell(b, label_mapper=None):
-    """generator that picks a cell from the batch object, yields its label and the cell itself.
-
-    Args:
-        b (cellpy.batch object): your batch object
-        label_mapper (callable or dict): function (or dict) that changes the cell names.
-            The dictionary must have the cell labels as given in the `journal.pages` index and new label as values.
-            Similarly, if it is a function it takes the cell label as input and returns the new label.
-            Remark! No check are performed to ensure that the new cell labels are unique.
-
-    Yields:
-        label, group, subgroup, cell
-
-    Example:
-        def my_mapper(n):
-            return "_".join(n.split("_")[1:-1])
-
-        # outputs "nnn_x" etc., if cell-names are of the form "date_nnn_x_y":
-        for label, group, subgroup, cell in pick_named_cell(b, label_mapper=my_mapper):
-            print(label)
-    """
-
-    cell_names = b.cell_names
-    for n in cell_names:
-        group = b.pages.loc[n, "group"]
-        sub_group = b.pages.loc[n, "sub_group"]
-
-        if label_mapper is not None:
-            try:
-                if isinstance(label_mapper, dict):
-                    label = label_mapper[n]
-                else:
-                    label = label_mapper(n)
-            except Exception as e:
-                logging.info(f"label_mapper-error: could not rename cell {n}")
-                logging.debug(f"caught exception: {e}")
-                label = n
-        else:
-            try:
-                label = b.pages.loc[n, "label"]
-            except Exception as e:
-                logging.info(f"lookup in pages failed: could not rename cell {n}")
-                logging.debug(f"caught exception: {e}")
-                label = n
-
-        logging.info(f"renaming {n} -> {label} (group={group}, subgroup={sub_group})")
-        yield label, group, sub_group, b.experiment.data[n]
-
-
-def cycles_collector(
-    b,
-    cycles=None,
-    interpolated=True,
-    number_of_points=100,
-    max_cycle=50,
-    abort_on_missing=False,
-    method="back-and-forth",
-    label_mapper=None,
-):
-    if cycles is None:
-        cycles = list(range(1, max_cycle + 1))
-    all_curves = []
-    keys = []
-    for n, g, sg, c in pick_named_cell(b, label_mapper):
-        curves = c.get_cap(
-            cycle=cycles,
-            label_cycle_number=True,
-            interpolated=interpolated,
-            number_of_points=number_of_points,
-            method=method,
-        )
-        logging.debug(f"processing {n} (session name: {c.session_name})")
-        if not curves.empty:
-            curves = curves.assign(group=g, sub_group=sg)
-            all_curves.append(curves)
-            keys.append(n)
-        else:
-            if abort_on_missing:
-                raise ValueError(f"{n} is empty - aborting!")
-            logging.critical(f"[{n} (session name: {c.session_name}) empty]")
-    collected_curves = pd.concat(
-        all_curves, keys=keys, axis=0, names=["cell", "point"]
-    ).reset_index(level="cell")
-    return collected_curves
-
-
-def cycles_plotter_simple_holo_map(collected_curves, journal=None, **kwargs):
-    p = hv.Curve(
-        collected_curves, kdims="capacity", vdims=["voltage", "cycle", "cell"]
-    ).groupby("cell")
-    return p
-
-
-def ica_plotter(
-    collected_curves,
-    journal=None,
-    palette="Blues",
-    palette_range=(0.2, 1.0),
-    method="fig_pr_cell",
-    extension="bokeh",
-    cycles_to_plot=None,
-    cols=1,
-    width=None,
-    height=None,
-    xlim_charge=(None, None),
-    xlim_discharge=(None, None),
-    **kwargs,
-):
-    if method == "film":
-        if extension == "matplotlib":
-            print("SORRY, PLOTTING FILM WITH MATPLOTLIB IS NOT IMPLEMENTED YET")
-            return
-
-        return ica_plotter_film_bokeh(
-            collected_curves,
-            journal=journal,
-            palette=palette,
-            extension="bokeh",
-            cycles=cycles_to_plot,
-            xlim_charge=xlim_charge,
-            xlim_discharge=xlim_discharge,
-            width=width,
-            height=height,
-            **kwargs,
-        )
-    else:
-        return sequence_plotter(
-            collected_curves,
-            x="voltage",
-            y="dq",
-            z="cycle",
-            g="cell",
-            journal=journal,
-            palette=palette,
-            palette_range=palette_range,
-            method=method,
-            extension=extension,
-            cycles=cycles_to_plot,
-            cols=cols,
-            width=width,
-        )
-
-
-def ica_plotter_film_bokeh(
-    collected_curves,
-    palette="Blues",
-    cycles=None,
-    xlim_charge=(None, None),
-    xlim_discharge=(None, None),
-    ylim=(None, None),
-    shared_axes=True,
-    width=400,
-    height=500,
-    cformatter="%02.0e",
-    **kwargs,
-):
-    if cycles is not None:
-        filtered_curves = collected_curves.loc[collected_curves.cycle.isin(cycles), :]
-    else:
-        filtered_curves = collected_curves
-
-    options = {
-        "xlabel": "Voltage (V)",
-        "ylabel": "Cycle",
-        "ylim": ylim,
-        "tools": ["hover"],
-        "width": width,
-        "height": height,
-        "cmap": palette,
-        "cformatter": cformatter,
-        "cnorm": "eq_hist",
-        "shared_axes": shared_axes,
-        "colorbar_opts": {
-            "title": "dQ/dV",
-        },
-    }
-
-    all_charge_plots = {}
-    all_discharge_plots = {}
-    for label, df in filtered_curves.groupby("cell"):
-        _charge = df.query("direction==1")
-        _discharge = df.query("direction==-1")
-        _dq_charge = group_by_interpolate(
-            _charge, x="voltage", y="dq", group_by="cycle", number_of_points=400
-        )
-        _dq_discharge = group_by_interpolate(
-            _discharge, x="voltage", y="dq", group_by="cycle", number_of_points=400
-        )
-
-        _v_charge = _dq_charge.index.values.ravel()
-        _v_discharge = _dq_discharge.index.values.ravel()
-
-        _cycles_charge = _charge.cycle.unique().ravel()
-        _cycles_discharge = _discharge.cycle.unique().ravel()
-
-        _dq_charge = -_dq_charge.values.T
-        _dq_discharge = _dq_discharge.values.T
-
-        charge_plot = hv.Image(
-            (_v_charge, _cycles_charge, _dq_charge), group="ica", label="charge"
-        ).opts(title=f"{label}", xlim=xlim_charge, colorbar=True, **options)
-
-        discharge_plot = hv.Image(
-            (_v_discharge, _cycles_discharge, _dq_discharge),
-            group="ica",
-            label="discharge",
-        ).opts(title=f"{label}", xlim=xlim_discharge, colorbar=True, **options)
-
-        all_charge_plots[f"{label}_charge"] = charge_plot
-        all_discharge_plots[f"{label}_discharge"] = discharge_plot
-
-    all_plots = {**all_charge_plots, **all_discharge_plots}
-    return (
-        hv.NdLayout(all_plots)
-        .opts(title="Incremental Capacity Analysis Film-plots")
-        .cols(2)
-    )
-
-
-def cycles_plotter(
-    collected_curves,
-    method="fig_pr_cell",
-    extension="bokeh",
-    cycles_to_plot=None,
-    width=None,
-    palette=None,
-    palette_range=(0.1, 1.0),
-    legend_position=None,
-    show_legend=None,
-    fig_title="",
-    cols=None,
-    **kwargs,
-):
-    if cols is None:
-        if extension == "matplotlib":
-            cols = 3
-        else:
-            cols = 3 if method == "fig_pr_cell" else 1
-
-    if width is None:
-        width = 400 if method == "fig_pr_cell" else int(800 / cols)
-
-    if palette is None:
-        palette = "Blues" if method == "fig_pr_cell" else "Category10"
-
-    if palette_range is None:
-        palette_range = (0.2, 1.0) if method == "fig_pr_cell" else (0, 1)
-
-    if legend_position is None:
-        legend_position = None if method == "fig_pr_cell" else "right"
-
-    if show_legend is None:
-        show_legend = True
-
-    reverse_palette = True if method == "fig_pr_cell" else False
-
-    backend_specific_kwargs = {
-        "NdLayout": {},
-        "NdOverlay": {},
-        "Curve": {},
-    }
-
-    if extension != "matplotlib":
-        logging.debug(f"setting width for bokeh and plotly: {width}")
-        backend_specific_kwargs["Curve"]["width"] = width
-
-    p = sequence_plotter(
-        collected_curves,
-        x="capacity",
-        y="voltage",
-        z="cycle",
-        g="cell",
-        method=method,
-        cycles=cycles_to_plot,
-        **kwargs,
-    ).cols(cols)
-
-    p.opts(
-        hv.opts.NdLayout(
-            title=fig_title,
-            **backend_specific_kwargs["NdLayout"],
-            backend=extension,
-        ),
-        hv.opts.NdOverlay(
-            **backend_specific_kwargs["NdOverlay"],
-            backend=extension,
-        ),
-        hv.opts.Curve(
-            # TODO: should replace this with custom mapping (see how it is done in plotutils):
-            color=hv.Palette(palette, reverse=reverse_palette, range=palette_range),
-            show_legend=show_legend,
-            **backend_specific_kwargs["Curve"],
-            backend=extension,
-        ),
-    )
-
-    if legend_position is not None:
-        p.opts(hv.opts.NdOverlay(legend_position=legend_position))
-
-    return p
-
-
-def sequence_plotter(
-    collected_curves,
-    x,
-    y,
-    z,
-    g,
-    method="fig_pr_cell",
-    group_label="group",
-    group_txt="cell-group",
-    z_lim=10,
-    cycles=None,
-    **kwargs,
-):
-    for k in kwargs:
-        logging.debug(f"keyword argument {k} given, but not used")
-
-    x_label = "Capacity"
-    x_unit = "mAh"
-
-    y_label = "Voltage"
-    y_unit = "V"
-
-    g_label = "Cell"
-    g_unit = ""
-
-    z_label = "Cycle"
-    z_unit = ""
-
-    x_dim = hv.Dimension(f"{x}", label=x_label, unit=x_unit)
-    y_dim = hv.Dimension(f"{y}", label=y_label, unit=y_unit)
-    g_dim = hv.Dimension(f"{g}", label=g_label, unit=g_unit)
-    z_dim = hv.Dimension(f"{z}", label=z_label, unit=z_unit)
-
-    family = {}
-    curves = None
-
-    if method == "fig_pr_cell":
-        if cycles is not None:
-            curves = collected_curves.loc[collected_curves.cycle.isin(cycles), :]
-        else:
-            curves = collected_curves
-        logging.debug(f"filtered_curves:\n{curves}")
-
-    elif method == "fig_pr_cycle":
-        if cycles is None:
-            unique_cycles = list(collected_curves.cycle.unique())
-            if len(unique_cycles) > 10:
-                cycles = [1, 10, 20]
-        if cycles is not None:
-            curves = collected_curves.loc[collected_curves.cycle.isin(cycles), :]
-        else:
-            curves = collected_curves
-        # g (what we split the figures by) : cycle
-        # z (the "dimension" of the individual curves in one figure): cell
-        z, g = g, z
-        z_dim, g_dim = g_dim, z_dim
-
-        # dirty (?) fix to make plots with a lot of cells look a bit better:
-        unique_z_values = collected_curves[z].unique()
-        no_unique_z_values = len(unique_z_values)
-        if no_unique_z_values > z_lim:
-            logging.critical(
-                f"number of cells ({no_unique_z_values}) larger than z_lim ({z_lim}): grouping"
-            )
-            logging.critical(
-                f"prevent this by modifying z_lim to your plotter_arguments"
-            )
-            z = group_label
-            z_dim = hv.Dimension(f"{z}", label=group_txt, unit="")
-
-    kdims = x_dim
-    vdims = [y_dim, z_dim]
-    for cyc, df in curves.groupby(g):
-        family[cyc] = hv.Curve(df, kdims=kdims, vdims=vdims).groupby(z).overlay()
-
-    return hv.NdLayout(family, kdims=g_dim)
-
-
-def ica_collector(
-    b,
-    cycles=None,
-    voltage_resolution=0.005,
-    max_cycle=50,
-    abort_on_missing=False,
-    label_direction=True,
-    number_of_points=None,
-    label_mapper=None,
-    **kwargs,
-):
-    if cycles is None:
-        cycles = list(range(1, max_cycle + 1))
-    all_curves = []
-    keys = []
-    for n, g, sg, c in pick_named_cell(b, label_mapper):
-        curves = ica.dqdv_frames(
-            c,
-            cycle=cycles,
-            voltage_resolution=voltage_resolution,
-            label_direction=label_direction,
-            number_of_points=number_of_points,
-            **kwargs,
-        )
-        logging.debug(f"processing {n} (session name: {c.session_name})")
-        if not curves.empty:
-            curves = curves.assign(group=g, sub_group=sg)
-            all_curves.append(curves)
-            keys.append(n)
-        else:
-            if abort_on_missing:
-                raise ValueError(f"{n} is empty - aborting!")
-            logging.critical(f"[{n} (session name: {c.session_name}) empty]")
-    collected_curves = pd.concat(
-        all_curves, keys=keys, axis=0, names=["cell", "point"]
-    ).reset_index(level="cell")
-    return collected_curves
-
-
-class BatchSummaryCollector(BatchCollector):
-    # Three main levels of arguments to the plotter and collector funcs is available:
-    #  - through dictionaries (`data_collector_arguments`, `plotter_arguments`) to init
-    #  - given as defaults in the subclass (`_default_data_collector_arguments`, `_default_plotter_arguments`)
-    #  - as elevated arguments (i.e. arguments normally given in the dictionaries elevated
-    #    to their own keyword parameters)
-
-    _default_data_collector_arguments = {
-        "columns": ["charge_capacity_gravimetric"],
-    }
-    _default_plotter_arguments = {
-        "extension": "bokeh",
-    }
-
-    _bokeh_template = [
-        hv.opts.Curve(fontsize={"title": "medium"}, width=800, backend="bokeh"),
-        hv.opts.NdOverlay(legend_position="right", backend="bokeh"),
-    ]
-
-    def __init__(
-        self,
-        b,
-        max_cycle: int = None,
-        rate=None,
-        on=None,
-        columns=None,
-        column_names=None,
-        normalize_capacity_on=None,
-        scale_by=None,
-        nom_cap=None,
-        normalize_cycles=None,
-        group_it=None,
-        rate_std=None,
-        rate_column=None,
-        inverse=None,
-        inverted: bool = None,
-        key_index_bounds=None,
-        extension: str = None,
-        title: str = None,
-        points: bool = None,
-        line: bool = None,
-        width: int = None,
-        height: int = None,
-        legend_title: str = None,
-        marker_size: int = None,
-        cmap=None,
-        spread: bool = None,
-        *args,
-        **kwargs,
-    ):
-        """Collects and shows summaries.
-
-        Elevated data collector args:
-            max_cycle (int): drop all cycles above this value.
-            rate (float): filter on rate (C-rate)
-            on (str or list of str): only select cycles if based on the rate of this step-type (e.g. on="charge").
-            columns (list): selected column(s) (using cellpy attribute name)
-                [defaults to "charge_capacity_gravimetric"]
-            column_names (list): selected column(s) (using exact column name)
-            normalize_capacity_on (list): list of cycle numbers that will be used for setting the basis of the
-                normalization (typically the first few cycles after formation)
-            scale_by (float or str): scale the normalized data with nominal capacity if "nom_cap",
-                or given value (defaults to one).
-            nom_cap (float): nominal capacity of the cell
-            normalize_cycles (bool): perform a normalization of the cycle numbers (also called equivalent cycle index)
-            group_it (bool): if True, average pr group.
-            rate_std (float): allow for this inaccuracy when selecting cycles based on rate
-            rate_column (str): name of the column containing the C-rates.
-            inverse (bool): select steps that do not have the given C-rate.
-            inverted (bool): select cycles that do not have the steps filtered by given C-rate.
-            key_index_bounds (list): used when creating a common label for the cells by splitting and combining from
-                key_index_bound[0] to key_index_bound[1].
-
-        Elevated plotter args:
-            extension (str): extension used (defaults to Bokeh)
-            points (bool): plot points if True
-            line (bool): plot line if True
-            width: width of plot
-            height: height of plot
-            legend_title: title to put over the legend
-            marker_size: size of the markers used
-            cmap: color-map to use
-            spread (bool): plot error-bands instead of error-bars if True
-        """
-
-        elevated_data_collector_arguments = dict(
-            max_cycle=max_cycle,
-            rate=rate,
-            on=on,
-            columns=columns,
-            column_names=column_names,
-            normalize_capacity_on=normalize_capacity_on,
-            scale_by=scale_by,
-            nom_cap=nom_cap,
-            normalize_cycles=normalize_cycles,
-            group_it=group_it,
-            rate_std=rate_std,
-            rate_column=rate_column,
-            inverse=inverse,
-            inverted=inverted,
-            key_index_bounds=key_index_bounds,
-        )
-
-        elevated_plotter_arguments = {
-            "extension": extension,
-            "title": title,
-            "points": points,
-            "line": line,
-            "width": width,
-            "height": height,
-            "legend_title": legend_title,
-            "marker_size": marker_size,
-            "cmap": cmap,
-            "spread": spread,
-        }
-
-        self._register_template(self._bokeh_template, extension="bokeh")
-
-        super().__init__(
-            b,
-            plotter=plot_concatenated,
-            data_collector=concatenate_summaries,
-            collector_name="summary",
-            elevated_data_collector_arguments=elevated_data_collector_arguments,
-            elevated_plotter_arguments=elevated_plotter_arguments,
-            *args,
-            **kwargs,
-        )
-
-    def generate_name(self):
-        names = ["collected_summaries"]
-        cols = self.data_collector_arguments.get("columns")
-        grouped = self.data_collector_arguments.get("group_it")
-        equivalent_cycles = self.data_collector_arguments.get("normalize_cycles")
-        normalized_cap = self.data_collector_arguments.get("normalize_capacity_on", [])
-        if self.nick:
-            names.insert(0, self.nick)
-        if cols:
-            names.extend(cols)
-        if grouped:
-            names.append("average")
-        if equivalent_cycles:
-            names.append("equivalents")
-        if len(normalized_cap):
-            names.append("norm")
-
-        name = "_".join(names)
-        return name
-
-
-class BatchICACollector(BatchCollector):
-    _default_data_collector_arguments = {}
-    _default_plotter_arguments = {
-        "extension": "bokeh",
-    }
-
-    def __init__(self, b, plot_type="fig_pr_cell", *args, **kwargs):
-        """Create a collection of ica (dQ/dV) plots."""
-
-        self.plot_type = plot_type
-
-        if plot_type == "fig_pr_cell":
-            _tight = True
-            _fig_inches = 3.5
-        else:
-            _tight = False
-            _fig_inches = 5.5
-
-        matplotlib_template = [
-            hv.opts.Curve(
-                show_frame=True,
-                fontsize={"title": "medium"},
-                backend="matplotlib",
-            ),
-            hv.opts.NdLayout(
-                fig_inches=_fig_inches, tight=_tight, backend="matplotlib"
-            ),
-        ]
-
-        bokeh_template = [
-            hv.opts.Curve(xlabel="Voltage (V)", backend="bokeh"),
-        ]
-        self._default_plotter_arguments["method"] = plot_type
-        self._register_template(matplotlib_template, extension="matplotlib")
-        self._register_template(bokeh_template, extension="bokeh")
-        super().__init__(
-            b,
-            plotter=ica_plotter,
-            data_collector=ica_collector,
-            collector_name="ica",
-            *args,
-            **kwargs,
-        )
-
-    def generate_name(self):
-        names = ["collected_ica"]
-
-        pm = self.plotter_arguments.get("method")
-        if pm == "fig_pr_cell":
-            names.append("pr_cell")
-        elif pm == "fig_pr_cycle":
-            names.append("pr_cyc")
-        elif pm == "film":
-            names.append("film")
-
-        if self.nick:
-            names.insert(0, self.nick)
-
-        name = "_".join(names)
-        return name
-
-
-class BatchCyclesCollector(BatchCollector):
-    _default_data_collector_arguments = {
-        "interpolated": True,
-        "number_of_points": 100,
-        "max_cycle": 50,
-        "abort_on_missing": False,
-        "method": "back-and-forth",
-    }
-    _default_plotter_arguments = {
-        "extension": "bokeh",
-    }
-
-    def __init__(
-        self,
-        b,
-        plot_type="fig_pr_cell",
-        collector_type="back-and-forth",
-        cycles=None,
-        max_cycle=None,
-        label_mapper=None,
-        extension=None,
-        cycles_to_plot=None,
-        width=None,
-        palette=None,
-        show_legend=None,
-        legend_position=None,
-        fig_title=None,
-        cols=None,
-        *args,
-        **kwargs,
-    ):
-        """Create a collection of capacity plots.
-
-        Args:
-            b:
-            plot_type (str): either 'fig_pr_cell' or 'fig_pr_cycle'
-            collector_type (str): how the curves are given
-                "back-and-forth" - standard back and forth; discharge
-                    (or charge) reversed from where charge (or discharge) ends.
-                "forth" - discharge (or charge) continues along x-axis.
-                "forth-and-forth" - discharge (or charge) also starts at 0
-            data_collector_arguments (dict) - arguments transferred to the plotter
-            plotter_arguments (dict) - arguments transferred to the plotter
-
-        Elevated data collector args:
-            cycles (int): drop all cycles above this value.
-            max_cycle (float): filter on rate (C-rate)
-            label_mapper (str or list of str): only select cycles if based on the rate of this step-type (e.g. on="charge").
-
-        Elevated plotter args:
-            extension (str): extension used (defaults to Bokeh)
-            cycles_to_plot (int): plot points if True
-            width (float): width of plot
-            legend_position (str): position of the legend
-            show_legend (bool): set to False if you don't want to show legend
-            fig_title (str): title (will be put above the figure)
-            palette (str): color-map to use
-            cols (int): number of columns
-        """
-
-        elevated_data_collector_arguments = dict(
-            cycles=cycles,
-            max_cycle=max_cycle,
-            label_mapper=label_mapper,
-        )
-        elevated_plotter_arguments = dict(
-            extension=extension,
-            cycles_to_plot=cycles_to_plot,
-            width=width,
-            palette=palette,
-            legend_position=legend_position,
-            show_legend=show_legend,
-            fig_title=fig_title,
-            cols=cols,
-        )
-
-        # internal attribute to keep track of plot type:
-        self.plot_type = plot_type
-
-        # moving it to after init to allow for using prms set in init
-        if plot_type == "fig_pr_cell":
-            _tight = True
-            _fig_inches = 3.5
-        else:
-            _tight = False
-            _fig_inches = 5.5
-
-        matplotlib_template = [
-            hv.opts.Curve(
-                show_frame=True,
-                fontsize={"title": "medium"},
-                ylim=(0, 1),
-                backend="matplotlib",
-            ),
-            hv.opts.NdLayout(
-                fig_inches=_fig_inches, tight=_tight, backend="matplotlib"
-            ),
-        ]
-
-        self._max_letters_in_cell_names = max(len(x) for x in b.cell_names)
-        self._register_template(matplotlib_template, extension="matplotlib")
-        self._default_data_collector_arguments["method"] = collector_type
-        self._default_plotter_arguments["method"] = plot_type
-
-        super().__init__(
-            b,
-            plotter=cycles_plotter,
-            data_collector=cycles_collector,
-            collector_name="cycles",
-            elevated_data_collector_arguments=elevated_data_collector_arguments,
-            elevated_plotter_arguments=elevated_plotter_arguments,
-            *args,
-            **kwargs,
-        )
-
-    def _dynamic_update_template_parameter(self, hv_opt, extension, *args, **kwargs):
-        k = hv_opt.key
-        if k == "NdLayout" and extension == "matplotlib":
-            if self.plot_type != "fig_pr_cycle":
-                hv_opt.kwargs["fig_inches"] = self._max_letters_in_cell_names * 0.14
-        return hv_opt
-
-    def generate_name(self):
-        names = ["collected_cycles"]
-
-        if self.data_collector_arguments.get("interpolated"):
-            names.append("intp")
-            if n := self.data_collector_arguments.get("number_of_points"):
-                names.append(f"p{n}")
-        cm = self.data_collector_arguments.get("method")
-        if cm.startswith("b"):
-            names.append("bf")
-        else:
-            names.append("ff")
-
-        pm = self.plotter_arguments.get("method")
-        if pm == "fig_pr_cell":
-            names.append("pr_cell")
-        elif pm == "fig_pr_cycle":
-            names.append("pr_cyc")
-
-        if self.nick:
-            names.insert(0, self.nick)
-
-        name = "_".join(names)
-        return name
+"""Collectors are used for simplifying plotting and exporting batch objects."""
+
+import textwrap
+from pprint import pprint
+from pathlib import Path
+from typing import Any
+import inspect
+import logging
+
+import pandas as pd
+
+import cellpy
+from cellpy.readers.core import group_by_interpolate
+from cellpy.utils.batch import Batch
+from cellpy.utils.helpers import concatenate_summaries
+from cellpy.utils.plotutils import plot_concatenated
+from cellpy.utils import ica
+
+try:
+    import holoviews as hv
+    from holoviews.core.io import Pickler
+    from holoviews import opts
+
+    HOLOVIEWS_AVAILABLE = True
+except ImportError:
+    print("Could not import Holoviews. Plotting will be disabled.")
+    HOLOVIEWS_AVAILABLE = False
+
+CELLPY_MINIMUM_VERSION = "0.4.3"
+
+
+def _setup():
+    _welcome_message()
+    _register_holoviews_renderers()
+
+
+def _welcome_message():
+    cellpy_version = cellpy.__version__
+    logging.info(f"cellpy version: {cellpy_version}")
+    logging.info(f"collectors need at least: {CELLPY_MINIMUM_VERSION}")
+
+
+def _register_holoviews_renderers(extensions=None):
+    if HOLOVIEWS_AVAILABLE:
+        if extensions is None:
+            extensions = "bokeh", "matplotlib"
+        logging.info(
+            f"Registering Holoviews extensions {extensions} for the cellpy collectors."
+        )
+        hv.extension(*extensions)
+    else:
+        logging.info(
+            "Could not import Holoviews. Your collectors will not be able to make figures."
+        )
+
+
+def _set_holoviews_renderer(extension=None):
+    if HOLOVIEWS_AVAILABLE:
+        extension = extension.lower()
+        current_backend = hv.Store.current_backend
+        if not extension == current_backend:
+            logging.info(f"switching backend to {extension}")
+            hv.Store.set_current_backend(extension)
+
+
+def _get_current_holoviews_renderer():
+    return hv.Store.current_backend
+
+
+_setup()
+
+
+class BatchCollector:
+    collector_name: str = None
+    data: pd.DataFrame = None
+    figure: Any = None
+    name: str = None
+    nick: str = None
+    autorun: bool = True
+    figure_directory: Path = Path("out")
+    data_directory: Path = Path("data/processed/")
+    renderer: Any = None
+
+    # override default arguments:
+    elevated_data_collector_arguments: dict = None
+    elevated_plotter_arguments: dict = None
+
+    # defaults (and used also when resetting):
+    _default_data_collector_arguments = {}
+    _default_plotter_arguments = {}
+
+    # templates override everything when using autorun:
+    _templates = {
+        "bokeh": [],
+        "matplotlib": [],
+        "plotly": [],
+    }
+
+    def __init__(
+        self,
+        b,
+        data_collector,
+        plotter,
+        collector_name=None,
+        name=None,
+        nick=None,
+        autorun=True,
+        use_templates=True,
+        elevated_data_collector_arguments=None,
+        elevated_plotter_arguments=None,
+        data_collector_arguments: dict = None,
+        plotter_arguments: dict = None,
+        **kwargs,
+    ):
+        """Update both the collected data and the plot(s).
+        Args:
+            b (cellpy.utils.Batch): the batch object.
+            data_collector (callable): method that collects the data.
+            plotter (callable): method that crates the plots.
+            collector_name (str): name of collector.
+            name (str or bool): name used for auto-generating filenames etc.
+            autorun (bool): run collector and plotter immediately if True.
+            use_templates (bool): also apply template(s) in autorun mode if True.
+            elevated_data_collector_arguments (dict): arguments picked up by the child class' initializer.
+            elevated_plotter_arguments (dict): arguments picked up by the child class' initializer.
+            data_collector_arguments (dict): keyword arguments sent to the data collector.
+            plotter_arguments (dict): keyword arguments sent to the plotter.
+            update_name (bool): update the name (using automatic name generation) based on new settings.
+            **kwargs: set Collector attributes.
+        """
+        self.b = b
+        self.data_collector = data_collector
+        self.plotter = plotter
+        self.nick = nick
+        self.collector_name = collector_name or "base"
+
+        # Arguments given as default arguments in the subclass have "low" priority (below elevated arguments at least):
+        self._data_collector_arguments = self._default_data_collector_arguments.copy()
+        self._plotter_arguments = self._default_plotter_arguments.copy()
+        self._update_arguments(data_collector_arguments, plotter_arguments)
+
+        # Elevated arguments have preference above the data_collector and plotter argument dicts:
+        self._parse_elevated_arguments(
+            elevated_data_collector_arguments, elevated_plotter_arguments
+        )
+
+        self._set_attributes(**kwargs)
+
+        if nick is None:
+            self.nick = b.name
+
+        if name is None:
+            name = self.generate_name()
+        self.name = name
+
+        if autorun:
+            self.update(update_name=False)
+            if use_templates:
+                self.apply_templates()
+
+    @property
+    def data_collector_arguments(self):
+        return self._data_collector_arguments
+
+    @data_collector_arguments.setter
+    def data_collector_arguments(self, argument_dict: dict):
+        if argument_dict is not None:
+            self._data_collector_arguments = {
+                **self._data_collector_arguments,
+                **argument_dict,
+            }
+
+    @property
+    def plotter_arguments(self):
+        return self._plotter_arguments
+
+    @plotter_arguments.setter
+    def plotter_arguments(self, argument_dict: dict):
+        if argument_dict is not None:
+            self._plotter_arguments = {**self._plotter_arguments, **argument_dict}
+
+    def __str__(self):
+        class_name = self.__class__.__name__
+
+        txt = f"{class_name}\n{len(class_name) * '='}\n\n"
+        txt += "Attributes:\n"
+        txt += "-----------\n"
+        txt += f" -collector_name: {self.collector_name}\n"
+        txt += f" -autorun: {self.autorun}\n"
+        txt += f" -name: {self.name}\n"
+        txt += f" -nick: {self.nick}\n"
+        txt += f" -csv_include_index: {self.csv_include_index}\n"
+        txt += f" -csv_layout: {self.csv_layout}\n"
+        txt += f" -sep: {self.sep}\n"
+        txt += f" -toolbar: {self.toolbar}\n"
+        txt += f" -figure_directory: {self.figure_directory}\n"
+        txt += f" -data_directory: {self.data_directory}\n"
+        txt += f" -batch-instance: {self.b.name}\n"
+        txt += f" -data_collector_arguments: {self.data_collector_arguments}\n"
+        txt += f" -plotter_arguments: {self.plotter_arguments}\n"
+
+        txt += "\nfigure:\n"
+        txt += ".......\n"
+        txt += f"{self.figure}\n"
+
+        txt += "\ndata:\n"
+        txt += ".....\n"
+        txt += f"{self.data}\n"
+
+        txt += "\nData collector:\n"
+        txt += "---------------\n"
+        data_name = self.data_collector.__name__
+        data_sig = inspect.signature(self.data_collector)
+        data_doc = inspect.getdoc(self.data_collector)
+        txt = f"{txt}{data_name}"
+        txt = f"{txt}{data_sig}\n"
+        txt = f"{txt}\n{data_doc}\n"
+
+        txt += "\nPlotter:\n"
+        txt += "--------\n"
+        plotter_name = self.plotter.__name__
+        plotter_sig = inspect.signature(self.plotter)
+        plotter_doc = inspect.getdoc(self.plotter)
+        txt = f"{txt}{plotter_name}"
+        txt = f"{txt}{plotter_sig}\n"
+        txt = f"{txt}\n{plotter_doc}\n"
+
+        return txt
+
+    def _repr_html_(self):
+        class_name = self.__class__.__name__
+        txt = f"<h2>{class_name}</h2> id={hex(id(self))}"
+        _txt = self.__str__().replace("\n", "<br>")
+        txt += f"<blockquote><code>{_txt}</></blockquote>"
+
+        return txt
+
+    def _set_attributes(self, **kwargs):
+        self.sep = kwargs.get("sep", ";")
+        self.csv_include_index = kwargs.get("csv_include_index", True)
+        self.csv_layout = kwargs.get("csv_layout", "long")
+        self.dpi = kwargs.get("dpi", 200)
+        self.toolbar = kwargs.get("toolbar", True)
+
+    def generate_name(self):
+        names = ["collector", self.collector_name]
+        if self.nick:
+            names.insert(0, self.nick)
+        name = "_".join(names)
+        return name
+
+    def _parse_elevated_arguments(
+        self, data_collector_arguments: dict = None, plotter_arguments: dict = None
+    ):
+        if data_collector_arguments is not None:
+            logging.info(f"Updating elevated arguments")
+            elevated_data_collector_arguments = {}
+            for k, v in data_collector_arguments.items():
+                if v is not None:
+                    elevated_data_collector_arguments[k] = v
+            self._update_arguments(
+                elevated_data_collector_arguments, None, set_as_defaults=True
+            )
+
+        if plotter_arguments is not None:
+            logging.info(f"Updating elevated arguments")
+            elevated_plotter_arguments = {}
+            for k, v in plotter_arguments.items():
+                if v is not None:
+                    elevated_plotter_arguments[k] = v
+
+            self._update_arguments(
+                None, elevated_plotter_arguments, set_as_defaults=True
+            )
+
+    def _update_arguments(
+        self,
+        data_collector_arguments: dict = None,
+        plotter_arguments: dict = None,
+        set_as_defaults=False,
+    ):
+        self.data_collector_arguments = data_collector_arguments
+        self.plotter_arguments = plotter_arguments
+        logging.info(f"**data_collector_arguments: {self.data_collector_arguments}")
+        logging.info(f"**plotter_arguments: {self.plotter_arguments}")
+
+        # setting defaults also (py3.6 compatible):
+        if set_as_defaults:
+            logging.info("updating defaults for current instance")
+            if data_collector_arguments is not None:
+                self._default_data_collector_arguments = {
+                    **self._default_data_collector_arguments,
+                    **data_collector_arguments,
+                }
+            if plotter_arguments is not None:
+                self._default_plotter_arguments = {
+                    **self._default_plotter_arguments,
+                    **plotter_arguments,
+                }
+
+    def reset_arguments(
+        self, data_collector_arguments: dict = None, plotter_arguments: dict = None
+    ):
+        """Reset the arguments to the defaults.
+        Args:
+            data_collector_arguments (dict): optional additional keyword arguments for the data collector.
+            plotter_arguments (dict): optional additional keyword arguments for the plotter.
+        """
+        self._data_collector_arguments = self._default_data_collector_arguments.copy()
+        self._plotter_arguments = self._default_plotter_arguments.copy()
+        self._update_arguments(data_collector_arguments, plotter_arguments)
+
+    def update(
+        self,
+        data_collector_arguments: dict = None,
+        plotter_arguments: dict = None,
+        reset: bool = False,
+        update_data: bool = False,
+        update_name: bool = False,
+        update_plot: bool = True,
+    ):
+        """Update both the collected data and the plot(s).
+        Args:
+            data_collector_arguments (dict): keyword arguments sent to the data collector.
+            plotter_arguments (dict): keyword arguments sent to the plotter.
+            reset (bool): reset the arguments first.
+            update_data (bool): update the data before updating the plot even if data has been collected before.
+            update_name (bool): update the name (using automatic name generation) based on new settings.
+            update_plot (bool): update the plot.
+        """
+        if reset:
+            self.reset_arguments(data_collector_arguments, plotter_arguments)
+        else:
+            self._update_arguments(data_collector_arguments, plotter_arguments)
+        if update_data or self.data is None:
+            try:
+                self.data = self.data_collector(self.b, **self.data_collector_arguments)
+            except TypeError as e:
+                print("Type error:", e)
+                print("Registered data_collector_arguments:")
+                pprint(self.data_collector_arguments)
+                print("Hint: fix it and then re-run using reset=True")
+                return
+        if update_plot:
+            if HOLOVIEWS_AVAILABLE:
+                _set_holoviews_renderer(self.plotter_arguments.get("extension"))
+                try:
+                    self.figure = self.plotter(
+                        self.data, journal=self.b.journal, **self.plotter_arguments
+                    )
+                except TypeError as e:
+                    print("Type error:", e)
+                    print("Registered plotter_arguments:")
+                    pprint(self.plotter_arguments)
+                    print("Hint: fix it and then re-run using reset=True")
+                    return
+
+        if update_name:
+            self.name = self.generate_name()
+
+    def _dynamic_update_template_parameter(self, hv_opt, extension, *args, **kwargs):
+        return hv_opt
+
+    def _register_template(self, hv_opts, extension="bokeh", *args, **kwargs):
+        """Register template for given extension.
+
+        It is also possible to set the options directly in the constructor of the
+        class. But it is recommended to use this method instead to allow for
+        sanitation of the options in the templates
+
+        Args:
+            hv_opts: list of holoviews.core.options.Options- instances
+                e.g. [hv.opts.Curve(xlim=(0,2)), hv.opts.NdLayout(title="Super plot")]
+            extension: Holoviews backend ("matplotlib", "bokeh", or "plotly")
+
+        Returns:
+            None
+        """
+        if extension not in ["bokeh", "matplotlib", "plotly"]:
+            print(f"extension='{extension}' is not supported.")
+        if not isinstance(hv_opts, (list, tuple)):
+            hv_opts = [hv_opts]
+
+        cleaned_hv_opts = []
+        for o in hv_opts:
+            logging.debug(f"Setting prm: {o}")
+            o = self._dynamic_update_template_parameter(o, extension, *args, **kwargs)
+            # ensure all options are registered with correct backend:
+            o.kwargs["backend"] = extension
+            cleaned_hv_opts.append(o)
+
+        self._templates[extension] = cleaned_hv_opts
+
+    def apply_templates(self):
+        if not self._figure_valid():
+            return
+
+        for backend, hv_opt in self._templates.items():
+            try:
+                if len(hv_opt):
+                    print(f"Applying template for {backend}:{hv_opt}")
+                    self.figure = self._set_hv_opts(hv_opt)
+            except TypeError:
+                print("possible bug in apply_template experienced")
+                print(self._templates)
+
+    def _figure_valid(self):
+        # TODO: create a decorator
+        if self.figure is None:
+            print("No figure to show!")
+            return False
+        if not HOLOVIEWS_AVAILABLE:
+            print("Requires Holoviews - please install it first!")
+            return False
+        return True
+
+    def _set_hv_opts(self, hv_opts):
+        if hv_opts is None:
+            return self.figure
+        if isinstance(hv_opts, (tuple, list)):
+            return self.figure.options(*hv_opts)
+        else:
+            return self.figure.options(hv_opts)
+
+    def show(self, hv_opts=None):
+        if not self._figure_valid():
+            return
+
+        print(f"figure name: {self.name}")
+        return self._set_hv_opts(hv_opts)
+
+    def redraw(self, hv_opts=None, extension=None):
+        print("EXPERIMENTAL FEATURE! THIS MIGHT NOT WORK PROPERLY YET")
+        if not self._figure_valid():
+            return
+
+        if extension is not None:
+            _set_holoviews_renderer(extension)
+
+        print(f"figure name: {self.name}")
+        self.figure = self._set_hv_opts(hv_opts)
+        return self.figure
+
+    def render(self):
+        print("Not implemented yet!")
+
+    def preprocess_data_for_csv(self):
+        print(f"the data layout {self.csv_layout} is not supported yet!")
+        return self.data
+
+    def to_csv(self, serial_number=None):
+        filename = self._output_path(serial_number)
+        filename = filename.with_suffix(".csv")
+        if self.csv_layout != "long":
+            data = self.preprocess_data_for_csv()
+        else:
+            data = self.data
+
+        data.to_csv(
+            filename,
+            sep=self.sep,
+            index=self.csv_include_index,
+        )
+        print(f"saved csv file: {filename}")
+
+    def to_image_files(self, serial_number=None):
+        if not self._figure_valid():
+            return
+        filename_pre = self._output_path(serial_number)
+
+        filename_hv = filename_pre.with_suffix(".html")
+        hv.save(
+            self.figure,
+            filename_hv,
+            toolbar=self.toolbar,
+        )
+        print(f"saved file: {filename_hv}")
+
+        filename_png = filename_pre.with_suffix(".png")
+        try:
+            current_renderer = _get_current_holoviews_renderer()
+
+            _set_holoviews_renderer("matplotlib")
+            self.figure.opts(hv.opts.NdOverlay(legend_position="right"))
+            hv.save(
+                self.figure,
+                filename_png,
+                dpi=300,
+            )
+            print(f"saved file: {filename_png}")
+        except Exception as e:
+            print("Could not save png-file.")
+            print(e)
+        finally:
+            _set_holoviews_renderer(current_renderer)
+
+    def save(self, serial_number=None):
+        self.to_csv(serial_number=serial_number)
+
+        if self._figure_valid():
+            filename = self._output_path(serial_number)
+            filename = filename.with_suffix(".hvz")
+            try:
+                Pickler.save(
+                    self.figure,
+                    filename,
+                )
+                print(f"pickled holoviews file: {filename}")
+            except TypeError as e:
+                print("could not save as hvz file")
+            self.to_image_files(serial_number=serial_number)
+
+    def _output_path(self, serial_number=None):
+        d = Path(self.figure_directory)
+        n = self.name
+        if serial_number is not None:
+            n = f"{n}_{serial_number:03}"
+        f = d / n
+        return f
+
+
+# TODO: allow for storing more than one figure setup pr collector
+#    It is time-consuming and memory demanding to re-collect the data
+#    for each time we need a new figure for the collector. We should
+#    allow for creating multiple figures within one collector or for
+#    sharing (passing) collected data. One solution might be to extend
+#    the capabilities of the base class. Another solution might be to
+#    add another sub-class in the chain from the base class to the actual one:
+class BatchMultiFigureCollector(BatchCollector):
+    pass
+
+
+def pick_named_cell(b, label_mapper=None):
+    """generator that picks a cell from the batch object, yields its label and the cell itself.
+
+    Args:
+        b (cellpy.batch object): your batch object
+        label_mapper (callable or dict): function (or dict) that changes the cell names.
+            The dictionary must have the cell labels as given in the `journal.pages` index and new label as values.
+            Similarly, if it is a function it takes the cell label as input and returns the new label.
+            Remark! No check are performed to ensure that the new cell labels are unique.
+
+    Yields:
+        label, group, subgroup, cell
+
+    Example:
+        def my_mapper(n):
+            return "_".join(n.split("_")[1:-1])
+
+        # outputs "nnn_x" etc., if cell-names are of the form "date_nnn_x_y":
+        for label, group, subgroup, cell in pick_named_cell(b, label_mapper=my_mapper):
+            print(label)
+    """
+
+    cell_names = b.cell_names
+    for n in cell_names:
+        group = b.pages.loc[n, "group"]
+        sub_group = b.pages.loc[n, "sub_group"]
+
+        if label_mapper is not None:
+            try:
+                if isinstance(label_mapper, dict):
+                    label = label_mapper[n]
+                else:
+                    label = label_mapper(n)
+            except Exception as e:
+                logging.info(f"label_mapper-error: could not rename cell {n}")
+                logging.debug(f"caught exception: {e}")
+                label = n
+        else:
+            try:
+                label = b.pages.loc[n, "label"]
+            except Exception as e:
+                logging.info(f"lookup in pages failed: could not rename cell {n}")
+                logging.debug(f"caught exception: {e}")
+                label = n
+
+        logging.info(f"renaming {n} -> {label} (group={group}, subgroup={sub_group})")
+        yield label, group, sub_group, b.experiment.data[n]
+
+
+def cycles_collector(
+    b,
+    cycles=None,
+    interpolated=True,
+    number_of_points=100,
+    max_cycle=50,
+    abort_on_missing=False,
+    method="back-and-forth",
+    label_mapper=None,
+):
+    if cycles is None:
+        cycles = list(range(1, max_cycle + 1))
+    all_curves = []
+    keys = []
+    for n, g, sg, c in pick_named_cell(b, label_mapper):
+        curves = c.get_cap(
+            cycle=cycles,
+            label_cycle_number=True,
+            interpolated=interpolated,
+            number_of_points=number_of_points,
+            method=method,
+        )
+        logging.debug(f"processing {n} (cell name: {c.cell_name})")
+        if not curves.empty:
+            curves = curves.assign(group=g, sub_group=sg)
+            all_curves.append(curves)
+            keys.append(n)
+        else:
+            if abort_on_missing:
+                raise ValueError(f"{n} is empty - aborting!")
+            logging.critical(f"[{n} (cell name: {c.cell_name}) empty]")
+    collected_curves = pd.concat(
+        all_curves, keys=keys, axis=0, names=["cell", "point"]
+    ).reset_index(level="cell")
+    return collected_curves
+
+
+def cycles_plotter_simple_holo_map(collected_curves, journal=None, **kwargs):
+    p = hv.Curve(
+        collected_curves, kdims="capacity", vdims=["voltage", "cycle", "cell"]
+    ).groupby("cell")
+    return p
+
+
+def ica_plotter(
+    collected_curves,
+    journal=None,
+    palette="Blues",
+    palette_range=(0.2, 1.0),
+    method="fig_pr_cell",
+    extension="bokeh",
+    cycles_to_plot=None,
+    cols=1,
+    width=None,
+    height=None,
+    xlim_charge=(None, None),
+    xlim_discharge=(None, None),
+    **kwargs,
+):
+    if method == "film":
+        if extension == "matplotlib":
+            print("SORRY, PLOTTING FILM WITH MATPLOTLIB IS NOT IMPLEMENTED YET")
+            return
+
+        return ica_plotter_film_bokeh(
+            collected_curves,
+            journal=journal,
+            palette=palette,
+            extension="bokeh",
+            cycles=cycles_to_plot,
+            xlim_charge=xlim_charge,
+            xlim_discharge=xlim_discharge,
+            width=width,
+            height=height,
+            **kwargs,
+        )
+    else:
+        return sequence_plotter(
+            collected_curves,
+            x="voltage",
+            y="dq",
+            z="cycle",
+            g="cell",
+            journal=journal,
+            palette=palette,
+            palette_range=palette_range,
+            method=method,
+            extension=extension,
+            cycles=cycles_to_plot,
+            cols=cols,
+            width=width,
+        )
+
+
+def ica_plotter_film_bokeh(
+    collected_curves,
+    palette="Blues",
+    cycles=None,
+    xlim_charge=(None, None),
+    xlim_discharge=(None, None),
+    ylim=(None, None),
+    shared_axes=True,
+    width=400,
+    height=500,
+    cformatter="%02.0e",
+    **kwargs,
+):
+    if cycles is not None:
+        filtered_curves = collected_curves.loc[collected_curves.cycle.isin(cycles), :]
+    else:
+        filtered_curves = collected_curves
+
+    options = {
+        "xlabel": "Voltage (V)",
+        "ylabel": "Cycle",
+        "ylim": ylim,
+        "tools": ["hover"],
+        "width": width,
+        "height": height,
+        "cmap": palette,
+        "cformatter": cformatter,
+        "cnorm": "eq_hist",
+        "shared_axes": shared_axes,
+        "colorbar_opts": {
+            "title": "dQ/dV",
+        },
+    }
+
+    all_charge_plots = {}
+    all_discharge_plots = {}
+    for label, df in filtered_curves.groupby("cell"):
+        _charge = df.query("direction==1")
+        _discharge = df.query("direction==-1")
+        _dq_charge = group_by_interpolate(
+            _charge, x="voltage", y="dq", group_by="cycle", number_of_points=400
+        )
+        _dq_discharge = group_by_interpolate(
+            _discharge, x="voltage", y="dq", group_by="cycle", number_of_points=400
+        )
+
+        _v_charge = _dq_charge.index.values.ravel()
+        _v_discharge = _dq_discharge.index.values.ravel()
+
+        _cycles_charge = _charge.cycle.unique().ravel()
+        _cycles_discharge = _discharge.cycle.unique().ravel()
+
+        _dq_charge = -_dq_charge.values.T
+        _dq_discharge = _dq_discharge.values.T
+
+        charge_plot = hv.Image(
+            (_v_charge, _cycles_charge, _dq_charge), group="ica", label="charge"
+        ).opts(title=f"{label}", xlim=xlim_charge, colorbar=True, **options)
+
+        discharge_plot = hv.Image(
+            (_v_discharge, _cycles_discharge, _dq_discharge),
+            group="ica",
+            label="discharge",
+        ).opts(title=f"{label}", xlim=xlim_discharge, colorbar=True, **options)
+
+        all_charge_plots[f"{label}_charge"] = charge_plot
+        all_discharge_plots[f"{label}_discharge"] = discharge_plot
+
+    all_plots = {**all_charge_plots, **all_discharge_plots}
+    return (
+        hv.NdLayout(all_plots)
+        .opts(title="Incremental Capacity Analysis Film-plots")
+        .cols(2)
+    )
+
+
+def cycles_plotter(
+    collected_curves,
+    method="fig_pr_cell",
+    extension="bokeh",
+    cycles_to_plot=None,
+    width=None,
+    palette=None,
+    palette_range=(0.1, 1.0),
+    legend_position=None,
+    show_legend=None,
+    fig_title="",
+    cols=None,
+    **kwargs,
+):
+    if cols is None:
+        if extension == "matplotlib":
+            cols = 3
+        else:
+            cols = 3 if method == "fig_pr_cell" else 1
+
+    if width is None:
+        width = 400 if method == "fig_pr_cell" else int(800 / cols)
+
+    if palette is None:
+        palette = "Blues" if method == "fig_pr_cell" else "Category10"
+
+    if palette_range is None:
+        palette_range = (0.2, 1.0) if method == "fig_pr_cell" else (0, 1)
+
+    if legend_position is None:
+        legend_position = None if method == "fig_pr_cell" else "right"
+
+    if show_legend is None:
+        show_legend = True
+
+    reverse_palette = True if method == "fig_pr_cell" else False
+
+    backend_specific_kwargs = {
+        "NdLayout": {},
+        "NdOverlay": {},
+        "Curve": {},
+    }
+
+    if extension != "matplotlib":
+        logging.debug(f"setting width for bokeh and plotly: {width}")
+        backend_specific_kwargs["Curve"]["width"] = width
+
+    p = sequence_plotter(
+        collected_curves,
+        x="capacity",
+        y="voltage",
+        z="cycle",
+        g="cell",
+        method=method,
+        cycles=cycles_to_plot,
+        **kwargs,
+    ).cols(cols)
+
+    p.opts(
+        hv.opts.NdLayout(
+            title=fig_title,
+            **backend_specific_kwargs["NdLayout"],
+            backend=extension,
+        ),
+        hv.opts.NdOverlay(
+            **backend_specific_kwargs["NdOverlay"],
+            backend=extension,
+        ),
+        hv.opts.Curve(
+            # TODO: should replace this with custom mapping (see how it is done in plotutils):
+            color=hv.Palette(palette, reverse=reverse_palette, range=palette_range),
+            show_legend=show_legend,
+            **backend_specific_kwargs["Curve"],
+            backend=extension,
+        ),
+    )
+
+    if legend_position is not None:
+        p.opts(hv.opts.NdOverlay(legend_position=legend_position))
+
+    return p
+
+
+def sequence_plotter(
+    collected_curves,
+    x,
+    y,
+    z,
+    g,
+    method="fig_pr_cell",
+    group_label="group",
+    group_txt="cell-group",
+    z_lim=10,
+    cycles=None,
+    **kwargs,
+):
+    for k in kwargs:
+        logging.debug(f"keyword argument {k} given, but not used")
+
+    x_label = "Capacity"
+    x_unit = "mAh"
+
+    y_label = "Voltage"
+    y_unit = "V"
+
+    g_label = "Cell"
+    g_unit = ""
+
+    z_label = "Cycle"
+    z_unit = ""
+
+    x_dim = hv.Dimension(f"{x}", label=x_label, unit=x_unit)
+    y_dim = hv.Dimension(f"{y}", label=y_label, unit=y_unit)
+    g_dim = hv.Dimension(f"{g}", label=g_label, unit=g_unit)
+    z_dim = hv.Dimension(f"{z}", label=z_label, unit=z_unit)
+
+    family = {}
+    curves = None
+
+    if method == "fig_pr_cell":
+        if cycles is not None:
+            curves = collected_curves.loc[collected_curves.cycle.isin(cycles), :]
+        else:
+            curves = collected_curves
+        logging.debug(f"filtered_curves:\n{curves}")
+
+    elif method == "fig_pr_cycle":
+        if cycles is None:
+            unique_cycles = list(collected_curves.cycle.unique())
+            if len(unique_cycles) > 10:
+                cycles = [1, 10, 20]
+        if cycles is not None:
+            curves = collected_curves.loc[collected_curves.cycle.isin(cycles), :]
+        else:
+            curves = collected_curves
+        # g (what we split the figures by) : cycle
+        # z (the "dimension" of the individual curves in one figure): cell
+        z, g = g, z
+        z_dim, g_dim = g_dim, z_dim
+
+        # dirty (?) fix to make plots with a lot of cells look a bit better:
+        unique_z_values = collected_curves[z].unique()
+        no_unique_z_values = len(unique_z_values)
+        if no_unique_z_values > z_lim:
+            logging.critical(
+                f"number of cells ({no_unique_z_values}) larger than z_lim ({z_lim}): grouping"
+            )
+            logging.critical(
+                f"prevent this by modifying z_lim to your plotter_arguments"
+            )
+            z = group_label
+            z_dim = hv.Dimension(f"{z}", label=group_txt, unit="")
+
+    kdims = x_dim
+    vdims = [y_dim, z_dim]
+    for cyc, df in curves.groupby(g):
+        family[cyc] = hv.Curve(df, kdims=kdims, vdims=vdims).groupby(z).overlay()
+
+    return hv.NdLayout(family, kdims=g_dim)
+
+
+def ica_collector(
+    b,
+    cycles=None,
+    voltage_resolution=0.005,
+    max_cycle=50,
+    abort_on_missing=False,
+    label_direction=True,
+    number_of_points=None,
+    label_mapper=None,
+    **kwargs,
+):
+    if cycles is None:
+        cycles = list(range(1, max_cycle + 1))
+    all_curves = []
+    keys = []
+    for n, g, sg, c in pick_named_cell(b, label_mapper):
+        curves = ica.dqdv_frames(
+            c,
+            cycle=cycles,
+            voltage_resolution=voltage_resolution,
+            label_direction=label_direction,
+            number_of_points=number_of_points,
+            **kwargs,
+        )
+        logging.debug(f"processing {n} (session name: {c.cell_name})")
+        if not curves.empty:
+            curves = curves.assign(group=g, sub_group=sg)
+            all_curves.append(curves)
+            keys.append(n)
+        else:
+            if abort_on_missing:
+                raise ValueError(f"{n} is empty - aborting!")
+            logging.critical(f"[{n} (session name: {c.cell_name}) empty]")
+    collected_curves = pd.concat(
+        all_curves, keys=keys, axis=0, names=["cell", "point"]
+    ).reset_index(level="cell")
+    return collected_curves
+
+
+class BatchSummaryCollector(BatchCollector):
+    # Three main levels of arguments to the plotter and collector funcs is available:
+    #  - through dictionaries (`data_collector_arguments`, `plotter_arguments`) to init
+    #  - given as defaults in the subclass (`_default_data_collector_arguments`, `_default_plotter_arguments`)
+    #  - as elevated arguments (i.e. arguments normally given in the dictionaries elevated
+    #    to their own keyword parameters)
+
+    _default_data_collector_arguments = {
+        "columns": ["charge_capacity_gravimetric"],
+    }
+    _default_plotter_arguments = {
+        "extension": "bokeh",
+    }
+
+    _bokeh_template = [
+        hv.opts.Curve(fontsize={"title": "medium"}, width=800, backend="bokeh"),
+        hv.opts.NdOverlay(legend_position="right", backend="bokeh"),
+    ]
+
+    def __init__(
+        self,
+        b,
+        max_cycle: int = None,
+        rate=None,
+        on=None,
+        columns=None,
+        column_names=None,
+        normalize_capacity_on=None,
+        scale_by=None,
+        nom_cap=None,
+        normalize_cycles=None,
+        group_it=None,
+        rate_std=None,
+        rate_column=None,
+        inverse=None,
+        inverted: bool = None,
+        key_index_bounds=None,
+        extension: str = None,
+        title: str = None,
+        points: bool = None,
+        line: bool = None,
+        width: int = None,
+        height: int = None,
+        legend_title: str = None,
+        marker_size: int = None,
+        cmap=None,
+        spread: bool = None,
+        *args,
+        **kwargs,
+    ):
+        """Collects and shows summaries.
+
+        Elevated data collector args:
+            max_cycle (int): drop all cycles above this value.
+            rate (float): filter on rate (C-rate)
+            on (str or list of str): only select cycles if based on the rate of this step-type (e.g. on="charge").
+            columns (list): selected column(s) (using cellpy attribute name)
+                [defaults to "charge_capacity_gravimetric"]
+            column_names (list): selected column(s) (using exact column name)
+            normalize_capacity_on (list): list of cycle numbers that will be used for setting the basis of the
+                normalization (typically the first few cycles after formation)
+            scale_by (float or str): scale the normalized data with nominal capacity if "nom_cap",
+                or given value (defaults to one).
+            nom_cap (float): nominal capacity of the cell
+            normalize_cycles (bool): perform a normalization of the cycle numbers (also called equivalent cycle index)
+            group_it (bool): if True, average pr group.
+            rate_std (float): allow for this inaccuracy when selecting cycles based on rate
+            rate_column (str): name of the column containing the C-rates.
+            inverse (bool): select steps that do not have the given C-rate.
+            inverted (bool): select cycles that do not have the steps filtered by given C-rate.
+            key_index_bounds (list): used when creating a common label for the cells by splitting and combining from
+                key_index_bound[0] to key_index_bound[1].
+
+        Elevated plotter args:
+            extension (str): extension used (defaults to Bokeh)
+            points (bool): plot points if True
+            line (bool): plot line if True
+            width: width of plot
+            height: height of plot
+            legend_title: title to put over the legend
+            marker_size: size of the markers used
+            cmap: color-map to use
+            spread (bool): plot error-bands instead of error-bars if True
+        """
+
+        elevated_data_collector_arguments = dict(
+            max_cycle=max_cycle,
+            rate=rate,
+            on=on,
+            columns=columns,
+            column_names=column_names,
+            normalize_capacity_on=normalize_capacity_on,
+            scale_by=scale_by,
+            nom_cap=nom_cap,
+            normalize_cycles=normalize_cycles,
+            group_it=group_it,
+            rate_std=rate_std,
+            rate_column=rate_column,
+            inverse=inverse,
+            inverted=inverted,
+            key_index_bounds=key_index_bounds,
+        )
+
+        elevated_plotter_arguments = {
+            "extension": extension,
+            "title": title,
+            "points": points,
+            "line": line,
+            "width": width,
+            "height": height,
+            "legend_title": legend_title,
+            "marker_size": marker_size,
+            "cmap": cmap,
+            "spread": spread,
+        }
+
+        self._register_template(self._bokeh_template, extension="bokeh")
+
+        super().__init__(
+            b,
+            plotter=plot_concatenated,
+            data_collector=concatenate_summaries,
+            collector_name="summary",
+            elevated_data_collector_arguments=elevated_data_collector_arguments,
+            elevated_plotter_arguments=elevated_plotter_arguments,
+            *args,
+            **kwargs,
+        )
+
+    def generate_name(self):
+        names = ["collected_summaries"]
+        cols = self.data_collector_arguments.get("columns")
+        grouped = self.data_collector_arguments.get("group_it")
+        equivalent_cycles = self.data_collector_arguments.get("normalize_cycles")
+        normalized_cap = self.data_collector_arguments.get("normalize_capacity_on", [])
+        if self.nick:
+            names.insert(0, self.nick)
+        if cols:
+            names.extend(cols)
+        if grouped:
+            names.append("average")
+        if equivalent_cycles:
+            names.append("equivalents")
+        if len(normalized_cap):
+            names.append("norm")
+
+        name = "_".join(names)
+        return name
+
+
+class BatchICACollector(BatchCollector):
+    _default_data_collector_arguments = {}
+    _default_plotter_arguments = {
+        "extension": "bokeh",
+    }
+
+    def __init__(self, b, plot_type="fig_pr_cell", *args, **kwargs):
+        """Create a collection of ica (dQ/dV) plots."""
+
+        self.plot_type = plot_type
+
+        if plot_type == "fig_pr_cell":
+            _tight = True
+            _fig_inches = 3.5
+        else:
+            _tight = False
+            _fig_inches = 5.5
+
+        matplotlib_template = [
+            hv.opts.Curve(
+                show_frame=True,
+                fontsize={"title": "medium"},
+                backend="matplotlib",
+            ),
+            hv.opts.NdLayout(
+                fig_inches=_fig_inches, tight=_tight, backend="matplotlib"
+            ),
+        ]
+
+        bokeh_template = [
+            hv.opts.Curve(xlabel="Voltage (V)", backend="bokeh"),
+        ]
+        self._default_plotter_arguments["method"] = plot_type
+        self._register_template(matplotlib_template, extension="matplotlib")
+        self._register_template(bokeh_template, extension="bokeh")
+        super().__init__(
+            b,
+            plotter=ica_plotter,
+            data_collector=ica_collector,
+            collector_name="ica",
+            *args,
+            **kwargs,
+        )
+
+    def generate_name(self):
+        names = ["collected_ica"]
+
+        pm = self.plotter_arguments.get("method")
+        if pm == "fig_pr_cell":
+            names.append("pr_cell")
+        elif pm == "fig_pr_cycle":
+            names.append("pr_cyc")
+        elif pm == "film":
+            names.append("film")
+
+        if self.nick:
+            names.insert(0, self.nick)
+
+        name = "_".join(names)
+        return name
+
+
+class BatchCyclesCollector(BatchCollector):
+    _default_data_collector_arguments = {
+        "interpolated": True,
+        "number_of_points": 100,
+        "max_cycle": 50,
+        "abort_on_missing": False,
+        "method": "back-and-forth",
+    }
+    _default_plotter_arguments = {
+        "extension": "bokeh",
+    }
+
+    def __init__(
+        self,
+        b,
+        plot_type="fig_pr_cell",
+        collector_type="back-and-forth",
+        cycles=None,
+        max_cycle=None,
+        label_mapper=None,
+        extension=None,
+        cycles_to_plot=None,
+        width=None,
+        palette=None,
+        show_legend=None,
+        legend_position=None,
+        fig_title=None,
+        cols=None,
+        *args,
+        **kwargs,
+    ):
+        """Create a collection of capacity plots.
+
+        Args:
+            b:
+            plot_type (str): either 'fig_pr_cell' or 'fig_pr_cycle'
+            collector_type (str): how the curves are given
+                "back-and-forth" - standard back and forth; discharge
+                    (or charge) reversed from where charge (or discharge) ends.
+                "forth" - discharge (or charge) continues along x-axis.
+                "forth-and-forth" - discharge (or charge) also starts at 0
+            data_collector_arguments (dict) - arguments transferred to the plotter
+            plotter_arguments (dict) - arguments transferred to the plotter
+
+        Elevated data collector args:
+            cycles (int): drop all cycles above this value.
+            max_cycle (float): filter on rate (C-rate)
+            label_mapper (str or list of str): only select cycles if based on the rate of this step-type (e.g. on="charge").
+
+        Elevated plotter args:
+            extension (str): extension used (defaults to Bokeh)
+            cycles_to_plot (int): plot points if True
+            width (float): width of plot
+            legend_position (str): position of the legend
+            show_legend (bool): set to False if you don't want to show legend
+            fig_title (str): title (will be put above the figure)
+            palette (str): color-map to use
+            cols (int): number of columns
+        """
+
+        elevated_data_collector_arguments = dict(
+            cycles=cycles,
+            max_cycle=max_cycle,
+            label_mapper=label_mapper,
+        )
+        elevated_plotter_arguments = dict(
+            extension=extension,
+            cycles_to_plot=cycles_to_plot,
+            width=width,
+            palette=palette,
+            legend_position=legend_position,
+            show_legend=show_legend,
+            fig_title=fig_title,
+            cols=cols,
+        )
+
+        # internal attribute to keep track of plot type:
+        self.plot_type = plot_type
+
+        # moving it to after init to allow for using prms set in init
+        if plot_type == "fig_pr_cell":
+            _tight = True
+            _fig_inches = 3.5
+        else:
+            _tight = False
+            _fig_inches = 5.5
+
+        matplotlib_template = [
+            hv.opts.Curve(
+                show_frame=True,
+                fontsize={"title": "medium"},
+                ylim=(0, 1),
+                backend="matplotlib",
+            ),
+            hv.opts.NdLayout(
+                fig_inches=_fig_inches, tight=_tight, backend="matplotlib"
+            ),
+        ]
+
+        self._max_letters_in_cell_names = max(len(x) for x in b.cell_names)
+        self._register_template(matplotlib_template, extension="matplotlib")
+        self._default_data_collector_arguments["method"] = collector_type
+        self._default_plotter_arguments["method"] = plot_type
+
+        super().__init__(
+            b,
+            plotter=cycles_plotter,
+            data_collector=cycles_collector,
+            collector_name="cycles",
+            elevated_data_collector_arguments=elevated_data_collector_arguments,
+            elevated_plotter_arguments=elevated_plotter_arguments,
+            *args,
+            **kwargs,
+        )
+
+    def _dynamic_update_template_parameter(self, hv_opt, extension, *args, **kwargs):
+        k = hv_opt.key
+        if k == "NdLayout" and extension == "matplotlib":
+            if self.plot_type != "fig_pr_cycle":
+                hv_opt.kwargs["fig_inches"] = self._max_letters_in_cell_names * 0.14
+        return hv_opt
+
+    def generate_name(self):
+        names = ["collected_cycles"]
+
+        if self.data_collector_arguments.get("interpolated"):
+            names.append("intp")
+            if n := self.data_collector_arguments.get("number_of_points"):
+                names.append(f"p{n}")
+        cm = self.data_collector_arguments.get("method")
+        if cm.startswith("b"):
+            names.append("bf")
+        else:
+            names.append("ff")
+
+        pm = self.plotter_arguments.get("method")
+        if pm == "fig_pr_cell":
+            names.append("pr_cell")
+        elif pm == "fig_pr_cycle":
+            names.append("pr_cyc")
+
+        if self.nick:
+            names.insert(0, self.nick)
+
+        name = "_".join(names)
+        return name
```

### Comparing `cellpy-1.0.0a9/cellpy/utils/data/20160805_test001_45_cc.h5` & `cellpy-1.0.0b0/cellpy/utils/data/20160805_test001_45_cc.h5`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/utils/data/raw/20160805_test001_45_cc_01.res` & `cellpy-1.0.0b0/cellpy/utils/data/raw/20160805_test001_45_cc_01.res`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/utils/easyplot.py` & `cellpy-1.0.0b0/cellpy/utils/easyplot.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/utils/example_data.py` & `cellpy-1.0.0b0/cellpy/utils/example_data.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/utils/ica.py` & `cellpy-1.0.0b0/cellpy/utils/ica.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1081 +1,1081 @@
-"""ica contains routines for creating and working with
-incremental capacity analysis data"""
-
-import os
-import logging
-import warnings
-
-import numpy as np
-import pandas as pd
-from scipy import stats
-from scipy.interpolate import interp1d
-from scipy.signal import savgol_filter
-from scipy.integrate import simps
-from scipy.ndimage.filters import gaussian_filter1d
-import pandas as pd
-
-from cellpy.exceptions import NullData
-from cellpy.readers.core import collect_capacity_curves
-
-
-# TODO: @jepe - documentation and tests
-# TODO: @jepe - fitting of o-c curves and differentiation
-# TODO: @jepe - modeling and fitting
-# TODO: @jepe - full-cell
-# TODO: @jepe - binning method (assigned to Asbjoern)
-
-
-class Converter:
-    """Class for dq-dv handling.
-
-    Typical usage is to (1) set the data, (2) inspect the data,
-    (3) pre-process the data,
-    (4) perform the dq-dv transform, and finally (5) post-process the data.
-
-    A short note about normalization:
-
-        - If ``normalization`` is set to ``False``, then no normalization will be done.
-        - If ``normalization`` is ``True``, and ``normalization_factor`` is ``None``, the total capacity of
-          the half cycle will be used for normalization, else the ``normalization_factor`` will be used.
-        - If ``normalization`` is ``True``, and ``normalization_roof`` is not ``None``,
-          the capacity divided by ``normalization_roof`` will be used for normalization.
-
-    """
-
-    def __init__(
-        self,
-        capacity=None,
-        voltage=None,
-        points_pr_split=10,
-        max_points=None,
-        voltage_resolution=None,
-        capacity_resolution=None,
-        minimum_splits=3,
-        interpolation_method="linear",
-        increment_method="diff",
-        pre_smoothing=False,
-        smoothing=False,
-        post_smoothing=True,
-        normalize=True,
-        normalizing_factor=None,
-        normalizing_roof=None,
-        savgol_filter_window_divisor_default=50,
-        savgol_filter_window_order=3,
-        voltage_fwhm=0.01,
-        gaussian_order=0,
-        gaussian_mode="reflect",
-        gaussian_cval=0.0,
-        gaussian_truncate=4.0,
-    ):
-        self.capacity = capacity
-        self.voltage = voltage
-
-        self.capacity_preprocessed = None
-        self.voltage_preprocessed = None
-        self.capacity_inverted = None
-        self.voltage_inverted = None
-
-        self.incremental_capacity = None
-        self._incremental_capacity = None  # before smoothing
-        self.voltage_processed = None
-        self._voltage_processed = None  # before shifting / centering
-
-        self.voltage_inverted_step = None
-
-        self.points_pr_split = points_pr_split
-        self.max_points = max_points
-        self.voltage_resolution = voltage_resolution
-        self.capacity_resolution = capacity_resolution
-        self.minimum_splits = minimum_splits
-        self.interpolation_method = interpolation_method
-        self.increment_method = increment_method
-        self.pre_smoothing = pre_smoothing
-        self.smoothing = smoothing
-        self.post_smoothing = post_smoothing
-        self.savgol_filter_window_divisor_default = savgol_filter_window_divisor_default
-        self.savgol_filter_window_order = savgol_filter_window_order
-        self.voltage_fwhm = voltage_fwhm
-        self.gaussian_order = gaussian_order
-        self.gaussian_mode = gaussian_mode
-        self.gaussian_cval = gaussian_cval
-        self.gaussian_truncate = gaussian_truncate
-        self.normalize = normalize
-        self.normalizing_factor = normalizing_factor
-        self.normalizing_roof = normalizing_roof
-
-        self.d_capacity_mean = None
-        self.d_voltage_mean = None
-        self.len_capacity = None
-        self.len_voltage = None
-        self.min_capacity = None
-        self.max_capacity = None
-        self.start_capacity = None
-        self.end_capacity = None
-        self.number_of_points = None
-        self.std_err_median = None
-        self.std_err_mean = None
-
-        self.fixed_voltage_range = False
-
-        self.errors = []
-
-    def __str__(self):
-        txt = f"[ica.converter] {str(type(self))}\n"
-        attrs = vars(self)
-        for name, att in attrs.items():
-            if isinstance(att, (pd.DataFrame, pd.Series, np.ndarray)):
-                str_att = f"<vector> ({str(type(att))})"
-            else:
-                str_att = str(att)
-            txt += f"{name}: {str_att}\n"
-
-        return txt
-
-    def set_data(self, capacity, voltage=None, capacity_label="q", voltage_label="v"):
-        """Set the data."""
-
-        logging.debug("setting data (capacity and voltage)")
-
-        if isinstance(capacity, pd.DataFrame):
-            logging.debug("received a pandas.DataFrame")
-            self.capacity = capacity[capacity_label]
-            self.voltage = capacity[voltage_label]
-        else:
-            assert len(capacity) == len(voltage)
-            self.capacity = capacity
-            self.voltage = voltage
-
-    def inspect_data(self, capacity=None, voltage=None, err_est=False, diff_est=False):
-        """Check and inspect the data."""
-
-        logging.debug("inspecting the data")
-
-        if capacity is None:
-            capacity = self.capacity
-        if voltage is None:
-            voltage = self.voltage
-
-        if capacity is None or voltage is None:
-            raise NullData
-
-        self.len_capacity = len(capacity)
-        self.len_voltage = len(voltage)
-
-        if self.len_capacity <= 1:
-            raise NullData
-        if self.len_voltage <= 1:
-            raise NullData
-
-        self.min_capacity, self.max_capacity = value_bounds(capacity)
-        self.start_capacity, self.end_capacity = index_bounds(capacity)
-
-        self.number_of_points = len(capacity)
-
-        if diff_est:
-            d_capacity = np.diff(capacity)
-            d_voltage = np.diff(voltage)
-
-            self.d_capacity_mean = np.mean(d_capacity)
-            self.d_voltage_mean = np.mean(d_voltage)
-
-        if err_est:
-            splits = int(self.number_of_points / self.points_pr_split)
-            rest = self.number_of_points % self.points_pr_split
-
-            if splits < self.minimum_splits:
-                txt = "no point in splitting, too little data"
-                logging.debug(txt)
-                self.errors.append("splitting: to few points")
-            else:
-                if rest > 0:
-                    _cap = capacity[:-rest]
-                    _vol = voltage[:-rest]
-                else:
-                    _cap = capacity
-                    _vol = voltage
-
-                c_pieces = np.split(_cap, splits)
-                v_pieces = np.split(_vol, splits)
-                # c_middle = int(np.amax(c_pieces) / 2)
-
-                std_err = []
-                c_pieces_avg = []
-                for c, v in zip(c_pieces, v_pieces):
-                    _slope, _intercept, _r_value, _p_value, _std_err = stats.linregress(
-                        c, v
-                    )
-                    std_err.append(_std_err)
-                    c_pieces_avg.append(np.mean(c))
-
-                self.std_err_median = np.median(std_err)
-                self.std_err_mean = np.mean(std_err)
-
-        if not self.start_capacity == self.min_capacity:
-            self.errors.append("capacity: start<>min")
-
-        if not self.end_capacity == self.max_capacity:
-            self.errors.append("capacity: end<>max")
-
-        if self.normalizing_factor is None:
-            self.normalizing_factor = self.end_capacity
-
-        if self.normalizing_roof is not None:
-            self.normalizing_factor = (
-                self.normalizing_factor * self.end_capacity / self.normalizing_roof
-            )
-
-    def pre_process_data(self):
-        """Perform some pre-processing of the data (i.e. interpolation)."""
-
-        logging.debug("pre-processing the data")
-
-        capacity = self.capacity
-        voltage = self.voltage
-
-        # performing an interpolation in v(q) space
-        logging.debug(" - interpolating voltage(capacity)")
-        c1, c2 = index_bounds(capacity)
-        if self.max_points is not None:
-            len_capacity = min(self.max_points, self.len_capacity)
-        elif self.capacity_resolution is not None:
-            len_capacity = int(round(abs(c2 - c1) / self.capacity_resolution, 0))
-        else:
-            len_capacity = self.len_capacity
-
-        f = interp1d(capacity, voltage, kind=self.interpolation_method)
-
-        self.capacity_preprocessed = np.linspace(c1, c2, len_capacity)
-        self.voltage_preprocessed = f(self.capacity_preprocessed)
-
-        if self.pre_smoothing:
-            logging.debug(" - pre-smoothing (savgol filter window)")
-            savgol_filter_window_divisor = np.amin(
-                (self.savgol_filter_window_divisor_default, len_capacity / 5)
-            )
-            savgol_filter_window_length = int(
-                len_capacity / savgol_filter_window_divisor
-            )
-
-            if savgol_filter_window_length % 2 == 0:
-                savgol_filter_window_length -= 1
-            savgol_filter_window_length = np.amax([3, savgol_filter_window_length])
-
-            self.voltage_preprocessed = savgol_filter(
-                self.voltage_preprocessed,
-                savgol_filter_window_length,
-                self.savgol_filter_window_order,
-            )
-
-    def increment_data(self):
-        """Perform the dq-dv transform."""
-
-        # NOTE TO ASBJOERN: Probably insert method for "binning" instead of
-        # TODO: Asbjørn will insert "binning" here
-        # differentiating here
-        # (use self.increment_method as the variable for selecting method for)
-
-        logging.debug("incrementing data")
-
-        # ---- shifting to y-x ----------------------------------------
-        v1, v2 = value_bounds(self.voltage_preprocessed)
-        if self.voltage_resolution is not None:
-            len_voltage = int(round(abs(v2 - v1) / self.voltage_resolution, 0))
-        else:
-            len_voltage = int(len(self.voltage_preprocessed))
-
-        # ---- interpolating ------------------------------------------
-        logging.debug(" - interpolating capacity(voltage)")
-        f = interp1d(
-            self.voltage_preprocessed,
-            self.capacity_preprocessed,
-            kind=self.interpolation_method,
-        )
-
-        self.voltage_inverted = np.linspace(v1, v2, len_voltage)
-        self.voltage_inverted_step = (v2 - v1) / (len_voltage - 1)
-        self.capacity_inverted = f(self.voltage_inverted)
-
-        if self.smoothing:
-            logging.debug(" - smoothing (savgol filter window)")
-            savgol_filter_window_divisor = np.amin(
-                (self.savgol_filter_window_divisor_default, len_voltage / 5)
-            )
-
-            savgol_filter_window_length = int(
-                len(self.voltage_inverted) / savgol_filter_window_divisor
-            )
-
-            if savgol_filter_window_length % 2 == 0:
-                savgol_filter_window_length -= 1
-
-            self.capacity_inverted = savgol_filter(
-                self.capacity_inverted,
-                np.amax([3, savgol_filter_window_length]),
-                self.savgol_filter_window_order,
-            )
-
-        # ---  diff --------------------
-        if self.increment_method == "diff":
-            logging.debug(" - diff using DIFF")
-            self.incremental_capacity = (
-                np.ediff1d(self.capacity_inverted) / self.voltage_inverted_step
-            )
-            self._incremental_capacity = self.incremental_capacity
-            # --- need to adjust voltage ---
-            self._voltage_processed = self.voltage_inverted[1:]
-            self.voltage_processed = (
-                self.voltage_inverted[1:] - 0.5 * self.voltage_inverted_step
-            )
-
-        elif self.increment_method == "hist":
-            logging.debug(" - diff using HIST")
-            logging.warning(
-                "Using the 'hist' method has not been thoroughly tested yet"
-            )
-            # raise NotImplementedError
-
-            df = pd.DataFrame(
-                {"Capacity": self.capacity_inverted, "Voltage": self.voltage_inverted}
-            )
-            df["dQ"] = df.Capacity.diff()
-            df["Voltage"] = df.Voltage.round(decimals=4)
-            df = df.groupby(["Voltage"])["dQ"].sum().to_frame().reset_index()
-            df["dV"] = df.Voltage.diff().rolling(1).sum()
-            df["dQdV"] = df.dQ / df.dV
-            # df = df[df.dQdV.notnull()]  # Might be needed, but could introduce an artefact
-
-            self.incremental_capacity = df.dQdV
-            self.voltage_processed = df.Voltage
-
-            # TODO: Asbjoern, maybe you can put your method here? Yes
-
-    def post_process_data(
-        self, voltage=None, incremental_capacity=None, voltage_step=None
-    ):
-        """Perform post-processing (smoothing, normalisation, interpolation) of the data."""
-
-        logging.debug("post-processing data")
-
-        if voltage is None:
-            voltage = self.voltage_processed
-            incremental_capacity = self.incremental_capacity
-            voltage_step = self.voltage_inverted_step
-
-        if self.post_smoothing:
-            logging.debug(" - post smoothing (gaussian)")
-            logging.debug(f"    * using voltage fwhm: {self.voltage_fwhm}")
-            points_fwhm = int(self.voltage_fwhm / voltage_step)
-
-            sigma = np.amax([1, points_fwhm / 2])
-
-            incremental_capacity = gaussian_filter1d(
-                incremental_capacity,
-                sigma=sigma,
-                order=self.gaussian_order,
-                mode=self.gaussian_mode,
-                cval=self.gaussian_cval,
-                truncate=self.gaussian_truncate,
-            )
-
-        if self.normalize:
-            logging.debug(" - normalizing")
-            area = simps(incremental_capacity, voltage)
-            incremental_capacity = (
-                incremental_capacity * self.normalizing_factor / abs(area)
-            )
-
-        self.incremental_capacity = incremental_capacity
-
-        fixed_range = False
-        if isinstance(self.fixed_voltage_range, np.ndarray):
-            fixed_range = True
-        else:
-            if self.fixed_voltage_range:
-                fixed_range = True
-        if fixed_range:
-            logging.debug(" - using fixed voltage range (interpolating)")
-            v1, v2, number_of_points = self.fixed_voltage_range
-            v = np.linspace(v1, v2, number_of_points)
-            f = interp1d(
-                x=self.voltage_processed,
-                y=incremental_capacity,
-                kind=self.interpolation_method,
-                bounds_error=False,
-                fill_value=np.NaN,
-            )
-            self.incremental_capacity = f(v)
-            self.voltage_processed = v
-
-
-def value_bounds(x):
-    """Returns tuple with min and max in x."""
-    return np.amin(x), np.amax(x)
-
-
-def index_bounds(x):
-    """Returns tuple with first and last item."""
-    if isinstance(x, (pd.DataFrame, pd.Series)):
-        return x.iloc[0], x.iloc[-1]
-    else:
-        return x[0], x[-1]
-
-
-def dqdv_cycle(cycle, splitter=True, label_direction=False, **kwargs):
-    """Convenience functions for creating dq-dv data from given capacity and
-    voltage cycle.
-
-    Returns the DataFrame with a 'voltage' and a 'incremental_capacity'
-    column.
-
-    Args:
-        cycle (pandas.DataFrame): the cycle data ('voltage', 'capacity', 'direction' (1 or -1)).
-        splitter (bool): insert a np.NaN row between charge and discharge.
-        label_direction (bool):
-
-    Returns:
-        List of step numbers corresponding to the selected steptype.
-        Returns a ``pandas.DataFrame`` instead of a list if ``pdtype`` is set to ``True``.
-
-    Additional key-word arguments are sent to Converter:
-
-    Keyword Args:
-        points_pr_split (int): only used when investigating data using splits, defaults to 10.
-        max_points: None
-        voltage_resolution (float): used for interpolating voltage data (e.g. 0.005)
-        capacity_resolution: used for interpolating capacity data
-        minimum_splits (int): defaults to 3.
-        interpolation_method: scipy interpolation method
-        increment_method (str): defaults to "diff"
-        pre_smoothing (bool): set to True for pre-smoothing (window)
-        smoothing (bool): set to True for smoothing during differentiation (window)
-        post_smoothing (bool): set to True for post-smoothing (gaussian)
-        normalize (bool): set to True for normalizing to capacity
-        normalizing_factor (float):
-        normalizing_roof  (float):
-        savgol_filter_window_divisor_default (int): used for window smoothing, defaults to 50
-        savgol_filter_window_order: used for window smoothing
-        voltage_fwhm (float): used for setting the post-processing gaussian sigma, defaults to 0.01
-        gaussian_order (int): defaults to 0
-        gaussian_mode (str): defaults to "reflect"
-        gaussian_cval (float): defaults to 0.0
-        gaussian_truncate (float): defaults to 4.0
-
-    Example:
-        >>> cycle_df = my_data.get_cap(
-        >>> ...   1,
-        >>> ...   categorical_column=True,
-        >>> ...   method = "forth-and-forth"
-        >>> ...   insert_nan=False,
-        >>> ... )
-        >>> voltage, incremental = ica.dqdv_cycle(cycle_df)
-
-    """
-
-    if cycle.empty:
-        raise NullData(f"The cycle (type={type(cycle)}) is empty.")
-
-    c_first = cycle.loc[cycle["direction"] == -1]
-    c_last = cycle.loc[cycle["direction"] == 1]
-
-    converter = Converter(**kwargs)
-
-    converter.set_data(c_first["capacity"], c_first["voltage"])
-    converter.inspect_data()
-    converter.pre_process_data()
-    converter.increment_data()
-    converter.post_process_data()
-    voltage_first = converter.voltage_processed
-    incremental_capacity_first = converter.incremental_capacity
-
-    if splitter:
-        voltage_first = np.append(voltage_first, np.NaN)
-        incremental_capacity_first = np.append(incremental_capacity_first, np.NaN)
-
-    converter = Converter(**kwargs)
-
-    converter.set_data(c_last["capacity"], c_last["voltage"])
-    converter.inspect_data()
-    converter.pre_process_data()
-    converter.increment_data()
-    converter.post_process_data()
-    voltage_last = converter.voltage_processed[::-1]
-    incremental_capacity_last = converter.incremental_capacity[::-1]
-
-    voltage = np.concatenate((voltage_first, voltage_last))
-    incremental_capacity = np.concatenate(
-        (incremental_capacity_first, incremental_capacity_last)
-    )
-
-    if label_direction:
-        direction_first = -np.ones(len(voltage_first))
-        direction_last = np.ones(len(voltage_last))
-        direction = np.concatenate((direction_first, direction_last))
-        return voltage, incremental_capacity, direction
-
-    return voltage, incremental_capacity
-
-
-def dqdv_cycles(cycles, not_merged=False, label_direction=False, **kwargs):
-    """Convenience functions for creating dq-dv data from given capacity and
-    voltage cycles.
-
-    Returns a DataFrame with a 'voltage' and a 'incremental_capacity'
-    column.
-
-    Args:
-        cycles (pandas.DataFrame): the cycle data ('cycle', 'voltage',
-             'capacity', 'direction' (1 or -1)).
-        not_merged (bool): return list of frames instead of concatenating (
-            defaults to False).
-        label_direction (bool): include 'direction' (1 or -1).
-
-    Returns:
-        ``pandas.DataFrame`` with columns 'cycle', 'voltage', 'dq' (and 'direction' if label_direction is True).
-
-    Additional key-word arguments are sent to Converter:
-
-    Keyword Args:
-        points_pr_split (int): only used when investigating data using
-            splits, defaults to 10.
-        max_points: None
-        voltage_resolution (float): used for interpolating voltage data
-            (e.g. 0.005)
-        capacity_resolution: used for interpolating capacity data
-        minimum_splits (int): defaults to 3.
-        interpolation_method: scipy interpolation method
-        increment_method (str): defaults to "diff"
-        pre_smoothing (bool): set to True for pre-smoothing (window)
-        smoothing (bool): set to True for smoothing during
-            differentiation (window)
-        post_smoothing (bool): set to True for post-smoothing (gaussian)
-        normalize (bool): set to True for normalizing to capacity
-        normalizing_factor (float):
-        normalizing_roof  (float):
-        savgol_filter_window_divisor_default (int): used for window
-            smoothing, defaults to 50
-        savgol_filter_window_order: used for window smoothing
-        voltage_fwhm (float): used for setting the post-processing
-            gaussian sigma, defaults to 0.01
-        gaussian_order (int): defaults to 0
-        gaussian_mode (str): defaults to "reflect"
-        gaussian_cval (float): defaults to 0.0
-        gaussian_truncate (float): defaults to 4.0
-
-    Example:
-        >>> cycles_df = my_data.get_cap(
-        >>> ...   categorical_column=True,
-        >>> ...   method = "forth-and-forth",
-        >>> ...   label_cycle_number=True,
-        >>> ...   insert_nan=False,
-        >>> ... )
-        >>> ica_df = ica.dqdv_cycles(cycles_df)
-
-    """
-
-    # TODO: should add option for normalising based on first cycle capacity
-    # this is e.g. done by first finding the first cycle capacity (nom_cap)
-    # (or use nominal capacity given as input) and then propagating this to
-    # Converter using the key-word arguments
-    #   normalize=True, normalization_factor=1.0, normalization_roof=nom_cap
-
-    if len(cycles) < 1:
-        logging.debug("The food was without nutrition")
-        return pd.DataFrame()
-
-    ica_dfs = list()
-    cycle_group = cycles.groupby("cycle")
-    keys = list()
-    for cycle_number, cycle in cycle_group:
-        cycle = cycle.dropna()
-        if label_direction:
-            v, dq, direction = dqdv_cycle(
-                cycle, splitter=True, label_direction=True, **kwargs
-            )
-            _d = {"voltage": v, "dq": dq, "direction": direction}
-            _cols = ["voltage", "dq", "direction"]
-        else:
-            v, dq = dqdv_cycle(cycle, splitter=True, label_direction=False, **kwargs)
-            _d = {"voltage": v, "dq": dq}
-            _cols = ["voltage", "dq"]
-
-        _ica_df = pd.DataFrame(_d)
-        if not not_merged:
-            _cols.insert(0, "cycle")
-            _ica_df["cycle"] = cycle_number
-            _ica_df = _ica_df[_cols]
-        else:
-            keys.append(cycle_number)
-            _ica_df = _ica_df[_cols]
-        ica_dfs.append(_ica_df)
-
-    if not_merged:
-        return keys, ica_dfs
-
-    ica_df = pd.concat(ica_dfs)
-    return ica_df
-
-
-def dqdv(
-    voltage,
-    capacity,
-    voltage_resolution=None,
-    capacity_resolution=None,
-    voltage_fwhm=0.01,
-    pre_smoothing=True,
-    diff_smoothing=False,
-    post_smoothing=True,
-    post_normalization=True,
-    interpolation_method=None,
-    gaussian_order=None,
-    gaussian_mode=None,
-    gaussian_cval=None,
-    gaussian_truncate=None,
-    points_pr_split=None,
-    savgol_filter_window_divisor_default=None,
-    savgol_filter_window_order=None,
-    max_points=None,
-    **kwargs,
-):
-    """Convenience functions for creating dq-dv data from given capacity
-    and voltage data.
-
-    Args:
-        voltage: nd.array or pd.Series
-        capacity: nd.array or pd.Series
-        voltage_resolution: used for interpolating voltage data (e.g. 0.005)
-        capacity_resolution: used for interpolating capacity data
-        voltage_fwhm: used for setting the post-processing gaussian sigma
-        pre_smoothing: set to True for pre-smoothing (window)
-        diff_smoothing: set to True for smoothing during differentiation
-            (window)
-        post_smoothing: set to True for post-smoothing (gaussian)
-        post_normalization: set to True for normalizing to capacity
-        interpolation_method: scipy interpolation method
-        gaussian_order: int
-        gaussian_mode: mode
-        gaussian_cval:
-        gaussian_truncate:
-        points_pr_split: only used when investigating data using splits
-        savgol_filter_window_divisor_default: used for window smoothing
-        savgol_filter_window_order: used for window smoothing
-        max_points: restricting to max points in vector (capacity-selected)
-
-    Returns:
-        (voltage, dqdv)
-
-    """
-    # Notes:
-    #     PEC data
-    #         pre_smoothing = False
-    #         diff_smoothing = False
-    #         pos_smoothing = False
-    #         voltage_resolution = 0.005
-    #     PEC data
-    #         ...
-    #     Arbin data (IFE)
-    #         ...
-
-    converter = Converter(**kwargs)
-    logging.debug("dqdv - starting")
-    logging.debug("dqdv - created Converter obj")
-    converter.pre_smoothing = pre_smoothing
-    converter.post_smoothing = post_smoothing
-    converter.smoothing = diff_smoothing
-    converter.normalize = post_normalization
-    converter.voltage_fwhm = voltage_fwhm
-    logging.debug(f"converter.pre_smoothing: {converter.pre_smoothing}")
-    logging.debug(f"converter.post_smoothing: {converter.post_smoothing}")
-    logging.debug(f"converter.smoothing: {converter.smoothing}")
-    logging.debug(f"converter.normalise: {converter.normalize}")
-    logging.debug(f"converter.voltage_fwhm: {converter.voltage_fwhm}")
-
-    if voltage_resolution is not None:
-        converter.voltage_resolution = voltage_resolution
-
-    if capacity_resolution is not None:
-        converter.capacity_resolution = capacity_resolution
-
-    if savgol_filter_window_divisor_default is not None:
-        converter.savgol_filter_window_divisor_default = (
-            savgol_filter_window_divisor_default
-        )
-
-        logging.debug(
-            f"converter.savgol_filter_window_divisor_default: "
-            f"{converter.savgol_filter_window_divisor_default}"
-        )
-
-    if savgol_filter_window_order is not None:
-        converter.savgol_filter_window_order = savgol_filter_window_order
-
-        logging.debug(
-            f"converter.savgol_filter_window_order: "
-            f"{converter.savgol_filter_window_order}"
-        )
-
-    if gaussian_mode is not None:
-        converter.gaussian_mode = gaussian_mode
-
-    if gaussian_order is not None:
-        converter.gaussian_order = gaussian_order
-
-    if gaussian_truncate is not None:
-        converter.gaussian_truncate = gaussian_truncate
-
-    if gaussian_cval is not None:
-        converter.gaussian_cval = gaussian_cval
-
-    if interpolation_method is not None:
-        converter.interpolation_method = interpolation_method
-
-    if points_pr_split is not None:
-        converter.points_pr_split = points_pr_split
-
-    if max_points is not None:
-        converter.max_points = max_points
-
-    converter.set_data(capacity, voltage)
-    converter.inspect_data()
-    converter.pre_process_data()
-    converter.increment_data()
-    converter.post_process_data()
-
-    return converter.voltage_processed, converter.incremental_capacity
-
-
-def dqdv_frames(cell, split=False, tidy=True, label_direction=False, **kwargs):
-    """Returns dqdv data as pandas.DataFrame(s) for all cycles.
-
-    Args:
-        cell (CellpyCell-object).
-        split (bool): return one frame for charge and one for
-            discharge if True (defaults to False).
-        tidy (bool): returns the split frames in wide format (defaults
-            to True. Remark that this option is currently not available
-            for non-split frames).
-
-    Returns:
-        one or two ``pandas.DataFrame`` with the following columns:
-        cycle: cycle number (if split is set to True).
-        voltage: voltage
-        dq: the incremental capacity
-
-
-    Additional key-word arguments are sent to Converter:
-
-    Keyword Args:
-        cycle (int or list of ints (cycle numbers)): will process all (or up to max_cycle_number)
-            if not given or equal to None.
-        points_pr_split (int): only used when investigating data
-            using splits, defaults to 10.
-        max_points: None
-        voltage_resolution (float): used for interpolating voltage
-            data (e.g. 0.005)
-        capacity_resolution: used for interpolating capacity data
-        minimum_splits (int): defaults to 3.
-        interpolation_method: scipy interpolation method
-        increment_method (str): defaults to "diff"
-        pre_smoothing (bool): set to True for pre-smoothing (window)
-        smoothing (bool): set to True for smoothing during
-            differentiation (window)
-        post_smoothing (bool): set to True for post-smoothing
-            (gaussian)
-        normalize (bool): set to True for normalizing to capacity
-        normalizing_factor (float):
-        normalizing_roof  (float):
-        savgol_filter_window_divisor_default (int): used for window
-            smoothing, defaults to 50
-        savgol_filter_window_order: used for window smoothing
-        voltage_fwhm (float): used for setting the post-processing
-            gaussian sigma, defaults to 0.01
-        gaussian_order (int): defaults to 0
-        gaussian_mode (str): defaults to "reflect"
-        gaussian_cval (float): defaults to 0.0
-        gaussian_truncate (float): defaults to 4.0
-
-    Example:
-        >>> from cellpy.utils import ica
-        >>> charge_df, dcharge_df = ica.ica_frames(my_cell, split=True)
-        >>> charge_df.plot(x=("voltage", "v"))
-
-    """
-    # TODO: should add option for normalizing based on first cycle capacity
-    # this is e.g. done by first finding the first cycle capacity (nom_cap)
-    # (or use nominal capacity given as input) and then propagating this to
-    # Converter using the key-word arguments
-    #   normalize=True, normalization_factor=1.0, normalization_roof=nom_cap
-
-    if split:
-        return _dqdv_split_frames(cell, tidy=tidy, **kwargs)
-    else:
-        return _dqdv_combinded_frame(
-            cell, tidy=tidy, label_direction=label_direction, **kwargs
-        )
-
-
-def _constrained_dq_dv_using_dataframes(capacity, minimum_v, maximum_v, **kwargs):
-    converter = Converter(**kwargs)
-    converter.set_data(capacity)
-    converter.inspect_data()
-    converter.pre_process_data()
-    converter.increment_data()
-    converter.fixed_voltage_range = [minimum_v, maximum_v, 100]
-    converter.post_process_data()
-    return converter.voltage_processed, converter.incremental_capacity
-
-
-def _make_ica_charge_curves(cycles_dfs, cycle_numbers, minimum_v, maximum_v, **kwargs):
-    incremental_charge_list = []
-
-    for c, n in zip(cycles_dfs, cycle_numbers):
-        if c.empty:
-            logging.info(f"{n} is empty")
-            v = [np.nan]
-            dq = [np.nan]
-        else:
-            v, dq = _constrained_dq_dv_using_dataframes(
-                c, minimum_v, maximum_v, **kwargs
-            )
-        if not incremental_charge_list:
-            d = pd.DataFrame({"v": v})
-            d.name = "voltage"
-            incremental_charge_list.append(d)
-
-            d = pd.DataFrame({f"dq": dq})
-            d.name = n
-            incremental_charge_list.append(d)
-
-        else:
-            d = pd.DataFrame({f"dq": dq})
-            # d.name = f"{cycle}"
-            d.name = n
-            incremental_charge_list.append(d)
-
-    return incremental_charge_list
-
-
-def _dqdv_combinded_frame(cell, tidy=True, label_direction=False, **kwargs):
-    """Returns full cycle dqdv data for all cycles as one pd.DataFrame.
-
-    Args:
-        cell: CellpyCell-object
-
-    Returns:
-        pandas.DataFrame with the following columns:
-            cycle: cycle number
-            voltage: voltage
-            dq: the incremental capacity
-    """
-    cycle = kwargs.pop("cycle", None)
-    number_of_points = kwargs.pop("number_of_points", None)
-    cycles = cell.get_cap(
-        cycle=cycle,
-        method="forth-and-forth",
-        categorical_column=True,
-        label_cycle_number=True,
-        insert_nan=False,
-        number_of_points=number_of_points,
-    )
-    ica_df = dqdv_cycles(
-        cycles, not_merged=not tidy, label_direction=label_direction, **kwargs
-    )
-
-    if not tidy:
-        # dqdv_cycles returns a list of cycle numbers and a list of DataFrames
-        # if not_merged is set to True (or not False)
-        keys, ica_df = ica_df
-        ica_df = pd.concat(ica_df, axis=1, keys=keys)
-        return ica_df
-
-    assert isinstance(ica_df, pd.DataFrame)
-    return ica_df
-
-
-def _dqdv_split_frames(
-    cell,
-    tidy=False,
-    trim_taper_steps=None,
-    steps_to_skip=None,
-    steptable=None,
-    max_cycle_number=None,
-    **kwargs,
-):
-    """Returns dqdv data as pandas.DataFrames for all cycles.
-
-    Args:
-        cell (CellpyCell-object).
-        tidy (bool): return in wide format if False (default),
-            long (tidy) format if True.
-
-    Returns:
-        (charge_ica_frame, discharge_ica_frame) where the frames are
-        pandas.DataFrames where the first column is voltage ('v') and
-        the following columns are the incremental capcaity for each
-        cycle (multi-indexed, where cycle number is on the top level).
-
-    Example:
-        >>> from cellpy.utils import ica
-        >>> charge_ica_df, dcharge_ica_df = ica.ica_frames(my_cell)
-        >>> charge_ica_df.plot(x=("voltage", "v"))
-
-    """
-    cycle = kwargs.pop("cycle", None)
-    if cycle and not isinstance(cycle, (list, tuple)):
-        cycle = [cycle]
-
-    charge_dfs, cycles, minimum_v, maximum_v = collect_capacity_curves(
-        cell,
-        direction="charge",
-        trim_taper_steps=trim_taper_steps,
-        steps_to_skip=steps_to_skip,
-        steptable=steptable,
-        max_cycle_number=max_cycle_number,
-        cycle=cycle,
-    )
-    logging.debug(f"retrieved {len(charge_dfs)} charge cycles")
-    # charge_df = pd.concat(
-    # charge_dfs, axis=1, keys=[k.name for k in charge_dfs])
-
-    ica_charge_dfs = _make_ica_charge_curves(
-        charge_dfs, cycles, minimum_v, maximum_v, **kwargs
-    )
-
-    ica_charge_df = pd.concat(
-        ica_charge_dfs, axis=1, keys=[k.name for k in ica_charge_dfs]
-    )
-
-    dcharge_dfs, cycles, minimum_v, maximum_v = collect_capacity_curves(
-        cell,
-        direction="discharge",
-        trim_taper_steps=trim_taper_steps,
-        steps_to_skip=steps_to_skip,
-        steptable=steptable,
-        max_cycle_number=max_cycle_number,
-        cycle=cycle,
-    )
-    logging.debug(f"retrieved {len(dcharge_dfs)} discharge cycles")
-    ica_dcharge_dfs = _make_ica_charge_curves(
-        dcharge_dfs, cycles, minimum_v, maximum_v, **kwargs
-    )
-    ica_discharge_df = pd.concat(
-        ica_dcharge_dfs, axis=1, keys=[k.name for k in ica_dcharge_dfs]
-    )
-    ica_charge_df.columns.names = ["cycle", "value"]
-    ica_discharge_df.columns.names = ["cycle", "value"]
-
-    if tidy:
-        ica_charge_df = ica_charge_df.melt(
-            "voltage", var_name="cycle", value_name="dq", col_level=0
-        )
-        ica_discharge_df = ica_discharge_df.melt(
-            "voltage", var_name="cycle", value_name="dq", col_level=0
-        )
-
-    return ica_charge_df, ica_discharge_df
-
-
-def _check_class_ica():
-    print(40 * "=")
-    print("running check_class_ica")
-    print(40 * "-")
-
-    import matplotlib.pyplot as plt
-
-    cell = _get_a_cell_to_play_with()
-    cycle = 5
-    print("looking at cycle %i" % cycle)
-
-    # ---------- processing and plotting ----------------
-    fig, (ax1, ax2) = plt.subplots(2, 1)
-    capacity, voltage = cell.get_ccap(cycle, return_dataframe=False)
-    ax1.plot(capacity, voltage, "b.-", label="raw")
-    converter = Converter()
-    converter.set_data(capacity, voltage)
-    converter.inspect_data()
-    converter.pre_process_data()
-    ax1.plot(
-        converter.capacity_preprocessed,
-        converter.voltage_preprocessed,
-        "r.-",
-        alpha=0.3,
-        label="pre-processed",
-    )
-
-    converter.increment_data()
-    ax2.plot(
-        converter.voltage_processed,
-        converter.incremental_capacity,
-        "b.-",
-        label="incremented",
-    )
-
-    converter.fixed_voltage_range = False
-    converter.post_smoothing = True
-    converter.normalize = False
-    converter.post_process_data()
-    ax2.plot(
-        converter.voltage_processed,
-        converter.incremental_capacity,
-        "y-",
-        alpha=0.3,
-        lw=4.0,
-        label="smoothed",
-    )
-
-    converter.fixed_voltage_range = np.array((0.1, 1.2, 100))
-    converter.post_smoothing = False
-    converter.normalize = False
-    converter.post_process_data()
-    ax2.plot(
-        converter.voltage_processed,
-        converter.incremental_capacity,
-        "go",
-        alpha=0.7,
-        label="fixed voltage range",
-    )
-    ax1.legend(numpoints=1)
-    ax2.legend(numpoints=1)
-    ax1.set_ylabel("Voltage (V)")
-    ax1.set_xlabel("Capacity (mAh/g)")
-    ax2.set_xlabel("Voltage (V)")
-    ax2.set_ylabel("dQ/dV (mAh/g/V)")
-    plt.show()
-
-
-def _get_a_cell_to_play_with():
-    from cellpy import cellreader
-
-    # -------- defining overall path-names etc ----------
-    current_file_path = os.path.dirname(os.path.realpath(__file__))
-    print(current_file_path)
-    relative_test_data_dir = "../../testdata/hdf5"
-    test_data_dir = os.path.abspath(
-        os.path.join(current_file_path, relative_test_data_dir)
-    )
-    # test_data_dir_out = os.path.join(test_data_dir, "out")
-    test_cellpy_file = "20160805_test001_45_cc.h5"
-    test_cellpy_file_full = os.path.join(test_data_dir, test_cellpy_file)
-    # mass = 0.078609164
-
-    # ---------- loading test-data ----------------------
-    cell = cellreader.CellpyCell()
-    cell.load(test_cellpy_file_full)
-    list_of_cycles = cell.get_cycle_numbers()
-    number_of_cycles = len(list_of_cycles)
-    print("you have %i cycles" % number_of_cycles)
-    # cell.save(test_cellpy_file_full)
-    return cell
-
-
-def _check_if_works():
-    import pandas as pd
-    from cellpy import cellreader
-
-    cell = _get_a_cell_to_play_with()
-
-    a = dqdv_frames(cell)
-    print("Hei")
-
-
-if __name__ == "__main__":
-    _check_if_works()
+"""ica contains routines for creating and working with
+incremental capacity analysis data"""
+
+import os
+import logging
+import warnings
+
+import numpy as np
+import pandas as pd
+from scipy import stats
+from scipy.interpolate import interp1d
+from scipy.signal import savgol_filter
+from scipy.integrate import simps
+from scipy.ndimage.filters import gaussian_filter1d
+import pandas as pd
+
+from cellpy.exceptions import NullData
+from cellpy.readers.core import collect_capacity_curves
+
+
+# TODO: @jepe - documentation and tests
+# TODO: @jepe - fitting of o-c curves and differentiation
+# TODO: @jepe - modeling and fitting
+# TODO: @jepe - full-cell
+# TODO: @jepe - binning method (assigned to Asbjoern)
+
+
+class Converter:
+    """Class for dq-dv handling.
+
+    Typical usage is to (1) set the data, (2) inspect the data,
+    (3) pre-process the data,
+    (4) perform the dq-dv transform, and finally (5) post-process the data.
+
+    A short note about normalization:
+
+        - If ``normalization`` is set to ``False``, then no normalization will be done.
+        - If ``normalization`` is ``True``, and ``normalization_factor`` is ``None``, the total capacity of
+          the half cycle will be used for normalization, else the ``normalization_factor`` will be used.
+        - If ``normalization`` is ``True``, and ``normalization_roof`` is not ``None``,
+          the capacity divided by ``normalization_roof`` will be used for normalization.
+
+    """
+
+    def __init__(
+        self,
+        capacity=None,
+        voltage=None,
+        points_pr_split=10,
+        max_points=None,
+        voltage_resolution=None,
+        capacity_resolution=None,
+        minimum_splits=3,
+        interpolation_method="linear",
+        increment_method="diff",
+        pre_smoothing=False,
+        smoothing=False,
+        post_smoothing=True,
+        normalize=True,
+        normalizing_factor=None,
+        normalizing_roof=None,
+        savgol_filter_window_divisor_default=50,
+        savgol_filter_window_order=3,
+        voltage_fwhm=0.01,
+        gaussian_order=0,
+        gaussian_mode="reflect",
+        gaussian_cval=0.0,
+        gaussian_truncate=4.0,
+    ):
+        self.capacity = capacity
+        self.voltage = voltage
+
+        self.capacity_preprocessed = None
+        self.voltage_preprocessed = None
+        self.capacity_inverted = None
+        self.voltage_inverted = None
+
+        self.incremental_capacity = None
+        self._incremental_capacity = None  # before smoothing
+        self.voltage_processed = None
+        self._voltage_processed = None  # before shifting / centering
+
+        self.voltage_inverted_step = None
+
+        self.points_pr_split = points_pr_split
+        self.max_points = max_points
+        self.voltage_resolution = voltage_resolution
+        self.capacity_resolution = capacity_resolution
+        self.minimum_splits = minimum_splits
+        self.interpolation_method = interpolation_method
+        self.increment_method = increment_method
+        self.pre_smoothing = pre_smoothing
+        self.smoothing = smoothing
+        self.post_smoothing = post_smoothing
+        self.savgol_filter_window_divisor_default = savgol_filter_window_divisor_default
+        self.savgol_filter_window_order = savgol_filter_window_order
+        self.voltage_fwhm = voltage_fwhm
+        self.gaussian_order = gaussian_order
+        self.gaussian_mode = gaussian_mode
+        self.gaussian_cval = gaussian_cval
+        self.gaussian_truncate = gaussian_truncate
+        self.normalize = normalize
+        self.normalizing_factor = normalizing_factor
+        self.normalizing_roof = normalizing_roof
+
+        self.d_capacity_mean = None
+        self.d_voltage_mean = None
+        self.len_capacity = None
+        self.len_voltage = None
+        self.min_capacity = None
+        self.max_capacity = None
+        self.start_capacity = None
+        self.end_capacity = None
+        self.number_of_points = None
+        self.std_err_median = None
+        self.std_err_mean = None
+
+        self.fixed_voltage_range = False
+
+        self.errors = []
+
+    def __str__(self):
+        txt = f"[ica.converter] {str(type(self))}\n"
+        attrs = vars(self)
+        for name, att in attrs.items():
+            if isinstance(att, (pd.DataFrame, pd.Series, np.ndarray)):
+                str_att = f"<vector> ({str(type(att))})"
+            else:
+                str_att = str(att)
+            txt += f"{name}: {str_att}\n"
+
+        return txt
+
+    def set_data(self, capacity, voltage=None, capacity_label="q", voltage_label="v"):
+        """Set the data."""
+
+        logging.debug("setting data (capacity and voltage)")
+
+        if isinstance(capacity, pd.DataFrame):
+            logging.debug("received a pandas.DataFrame")
+            self.capacity = capacity[capacity_label]
+            self.voltage = capacity[voltage_label]
+        else:
+            assert len(capacity) == len(voltage)
+            self.capacity = capacity
+            self.voltage = voltage
+
+    def inspect_data(self, capacity=None, voltage=None, err_est=False, diff_est=False):
+        """Check and inspect the data."""
+
+        logging.debug("inspecting the data")
+
+        if capacity is None:
+            capacity = self.capacity
+        if voltage is None:
+            voltage = self.voltage
+
+        if capacity is None or voltage is None:
+            raise NullData
+
+        self.len_capacity = len(capacity)
+        self.len_voltage = len(voltage)
+
+        if self.len_capacity <= 1:
+            raise NullData
+        if self.len_voltage <= 1:
+            raise NullData
+
+        self.min_capacity, self.max_capacity = value_bounds(capacity)
+        self.start_capacity, self.end_capacity = index_bounds(capacity)
+
+        self.number_of_points = len(capacity)
+
+        if diff_est:
+            d_capacity = np.diff(capacity)
+            d_voltage = np.diff(voltage)
+
+            self.d_capacity_mean = np.mean(d_capacity)
+            self.d_voltage_mean = np.mean(d_voltage)
+
+        if err_est:
+            splits = int(self.number_of_points / self.points_pr_split)
+            rest = self.number_of_points % self.points_pr_split
+
+            if splits < self.minimum_splits:
+                txt = "no point in splitting, too little data"
+                logging.debug(txt)
+                self.errors.append("splitting: to few points")
+            else:
+                if rest > 0:
+                    _cap = capacity[:-rest]
+                    _vol = voltage[:-rest]
+                else:
+                    _cap = capacity
+                    _vol = voltage
+
+                c_pieces = np.split(_cap, splits)
+                v_pieces = np.split(_vol, splits)
+                # c_middle = int(np.amax(c_pieces) / 2)
+
+                std_err = []
+                c_pieces_avg = []
+                for c, v in zip(c_pieces, v_pieces):
+                    _slope, _intercept, _r_value, _p_value, _std_err = stats.linregress(
+                        c, v
+                    )
+                    std_err.append(_std_err)
+                    c_pieces_avg.append(np.mean(c))
+
+                self.std_err_median = np.median(std_err)
+                self.std_err_mean = np.mean(std_err)
+
+        if not self.start_capacity == self.min_capacity:
+            self.errors.append("capacity: start<>min")
+
+        if not self.end_capacity == self.max_capacity:
+            self.errors.append("capacity: end<>max")
+
+        if self.normalizing_factor is None:
+            self.normalizing_factor = self.end_capacity
+
+        if self.normalizing_roof is not None:
+            self.normalizing_factor = (
+                self.normalizing_factor * self.end_capacity / self.normalizing_roof
+            )
+
+    def pre_process_data(self):
+        """Perform some pre-processing of the data (i.e. interpolation)."""
+
+        logging.debug("pre-processing the data")
+
+        capacity = self.capacity
+        voltage = self.voltage
+
+        # performing an interpolation in v(q) space
+        logging.debug(" - interpolating voltage(capacity)")
+        c1, c2 = index_bounds(capacity)
+        if self.max_points is not None:
+            len_capacity = min(self.max_points, self.len_capacity)
+        elif self.capacity_resolution is not None:
+            len_capacity = int(round(abs(c2 - c1) / self.capacity_resolution, 0))
+        else:
+            len_capacity = self.len_capacity
+
+        f = interp1d(capacity, voltage, kind=self.interpolation_method)
+
+        self.capacity_preprocessed = np.linspace(c1, c2, len_capacity)
+        self.voltage_preprocessed = f(self.capacity_preprocessed)
+
+        if self.pre_smoothing:
+            logging.debug(" - pre-smoothing (savgol filter window)")
+            savgol_filter_window_divisor = np.amin(
+                (self.savgol_filter_window_divisor_default, len_capacity / 5)
+            )
+            savgol_filter_window_length = int(
+                len_capacity / savgol_filter_window_divisor
+            )
+
+            if savgol_filter_window_length % 2 == 0:
+                savgol_filter_window_length -= 1
+            savgol_filter_window_length = np.amax([3, savgol_filter_window_length])
+
+            self.voltage_preprocessed = savgol_filter(
+                self.voltage_preprocessed,
+                savgol_filter_window_length,
+                self.savgol_filter_window_order,
+            )
+
+    def increment_data(self):
+        """Perform the dq-dv transform."""
+
+        # NOTE TO ASBJOERN: Probably insert method for "binning" instead of
+        # TODO: Asbjørn will insert "binning" here
+        # differentiating here
+        # (use self.increment_method as the variable for selecting method for)
+
+        logging.debug("incrementing data")
+
+        # ---- shifting to y-x ----------------------------------------
+        v1, v2 = value_bounds(self.voltage_preprocessed)
+        if self.voltage_resolution is not None:
+            len_voltage = int(round(abs(v2 - v1) / self.voltage_resolution, 0))
+        else:
+            len_voltage = int(len(self.voltage_preprocessed))
+
+        # ---- interpolating ------------------------------------------
+        logging.debug(" - interpolating capacity(voltage)")
+        f = interp1d(
+            self.voltage_preprocessed,
+            self.capacity_preprocessed,
+            kind=self.interpolation_method,
+        )
+
+        self.voltage_inverted = np.linspace(v1, v2, len_voltage)
+        self.voltage_inverted_step = (v2 - v1) / (len_voltage - 1)
+        self.capacity_inverted = f(self.voltage_inverted)
+
+        if self.smoothing:
+            logging.debug(" - smoothing (savgol filter window)")
+            savgol_filter_window_divisor = np.amin(
+                (self.savgol_filter_window_divisor_default, len_voltage / 5)
+            )
+
+            savgol_filter_window_length = int(
+                len(self.voltage_inverted) / savgol_filter_window_divisor
+            )
+
+            if savgol_filter_window_length % 2 == 0:
+                savgol_filter_window_length -= 1
+
+            self.capacity_inverted = savgol_filter(
+                self.capacity_inverted,
+                np.amax([3, savgol_filter_window_length]),
+                self.savgol_filter_window_order,
+            )
+
+        # ---  diff --------------------
+        if self.increment_method == "diff":
+            logging.debug(" - diff using DIFF")
+            self.incremental_capacity = (
+                np.ediff1d(self.capacity_inverted) / self.voltage_inverted_step
+            )
+            self._incremental_capacity = self.incremental_capacity
+            # --- need to adjust voltage ---
+            self._voltage_processed = self.voltage_inverted[1:]
+            self.voltage_processed = (
+                self.voltage_inverted[1:] - 0.5 * self.voltage_inverted_step
+            )
+
+        elif self.increment_method == "hist":
+            logging.debug(" - diff using HIST")
+            logging.warning(
+                "Using the 'hist' method has not been thoroughly tested yet"
+            )
+            # raise NotImplementedError
+
+            df = pd.DataFrame(
+                {"Capacity": self.capacity_inverted, "Voltage": self.voltage_inverted}
+            )
+            df["dQ"] = df.Capacity.diff()
+            df["Voltage"] = df.Voltage.round(decimals=4)
+            df = df.groupby(["Voltage"])["dQ"].sum().to_frame().reset_index()
+            df["dV"] = df.Voltage.diff().rolling(1).sum()
+            df["dQdV"] = df.dQ / df.dV
+            # df = df[df.dQdV.notnull()]  # Might be needed, but could introduce an artefact
+
+            self.incremental_capacity = df.dQdV
+            self.voltage_processed = df.Voltage
+
+            # TODO: Asbjoern, maybe you can put your method here? Yes
+
+    def post_process_data(
+        self, voltage=None, incremental_capacity=None, voltage_step=None
+    ):
+        """Perform post-processing (smoothing, normalisation, interpolation) of the data."""
+
+        logging.debug("post-processing data")
+
+        if voltage is None:
+            voltage = self.voltage_processed
+            incremental_capacity = self.incremental_capacity
+            voltage_step = self.voltage_inverted_step
+
+        if self.post_smoothing:
+            logging.debug(" - post smoothing (gaussian)")
+            logging.debug(f"    * using voltage fwhm: {self.voltage_fwhm}")
+            points_fwhm = int(self.voltage_fwhm / voltage_step)
+
+            sigma = np.amax([1, points_fwhm / 2])
+
+            incremental_capacity = gaussian_filter1d(
+                incremental_capacity,
+                sigma=sigma,
+                order=self.gaussian_order,
+                mode=self.gaussian_mode,
+                cval=self.gaussian_cval,
+                truncate=self.gaussian_truncate,
+            )
+
+        if self.normalize:
+            logging.debug(" - normalizing")
+            area = simps(incremental_capacity, voltage)
+            incremental_capacity = (
+                incremental_capacity * self.normalizing_factor / abs(area)
+            )
+
+        self.incremental_capacity = incremental_capacity
+
+        fixed_range = False
+        if isinstance(self.fixed_voltage_range, np.ndarray):
+            fixed_range = True
+        else:
+            if self.fixed_voltage_range:
+                fixed_range = True
+        if fixed_range:
+            logging.debug(" - using fixed voltage range (interpolating)")
+            v1, v2, number_of_points = self.fixed_voltage_range
+            v = np.linspace(v1, v2, number_of_points)
+            f = interp1d(
+                x=self.voltage_processed,
+                y=incremental_capacity,
+                kind=self.interpolation_method,
+                bounds_error=False,
+                fill_value=np.NaN,
+            )
+            self.incremental_capacity = f(v)
+            self.voltage_processed = v
+
+
+def value_bounds(x):
+    """Returns tuple with min and max in x."""
+    return np.amin(x), np.amax(x)
+
+
+def index_bounds(x):
+    """Returns tuple with first and last item."""
+    if isinstance(x, (pd.DataFrame, pd.Series)):
+        return x.iloc[0], x.iloc[-1]
+    else:
+        return x[0], x[-1]
+
+
+def dqdv_cycle(cycle, splitter=True, label_direction=False, **kwargs):
+    """Convenience functions for creating dq-dv data from given capacity and
+    voltage cycle.
+
+    Returns the DataFrame with a 'voltage' and a 'incremental_capacity'
+    column.
+
+    Args:
+        cycle (pandas.DataFrame): the cycle data ('voltage', 'capacity', 'direction' (1 or -1)).
+        splitter (bool): insert a np.NaN row between charge and discharge.
+        label_direction (bool):
+
+    Returns:
+        List of step numbers corresponding to the selected steptype.
+        Returns a ``pandas.DataFrame`` instead of a list if ``pdtype`` is set to ``True``.
+
+    Additional key-word arguments are sent to Converter:
+
+    Keyword Args:
+        points_pr_split (int): only used when investigating data using splits, defaults to 10.
+        max_points: None
+        voltage_resolution (float): used for interpolating voltage data (e.g. 0.005)
+        capacity_resolution: used for interpolating capacity data
+        minimum_splits (int): defaults to 3.
+        interpolation_method: scipy interpolation method
+        increment_method (str): defaults to "diff"
+        pre_smoothing (bool): set to True for pre-smoothing (window)
+        smoothing (bool): set to True for smoothing during differentiation (window)
+        post_smoothing (bool): set to True for post-smoothing (gaussian)
+        normalize (bool): set to True for normalizing to capacity
+        normalizing_factor (float):
+        normalizing_roof  (float):
+        savgol_filter_window_divisor_default (int): used for window smoothing, defaults to 50
+        savgol_filter_window_order: used for window smoothing
+        voltage_fwhm (float): used for setting the post-processing gaussian sigma, defaults to 0.01
+        gaussian_order (int): defaults to 0
+        gaussian_mode (str): defaults to "reflect"
+        gaussian_cval (float): defaults to 0.0
+        gaussian_truncate (float): defaults to 4.0
+
+    Example:
+        >>> cycle_df = my_data.get_cap(
+        >>> ...   1,
+        >>> ...   categorical_column=True,
+        >>> ...   method = "forth-and-forth"
+        >>> ...   insert_nan=False,
+        >>> ... )
+        >>> voltage, incremental = ica.dqdv_cycle(cycle_df)
+
+    """
+
+    if cycle.empty:
+        raise NullData(f"The cycle (type={type(cycle)}) is empty.")
+
+    c_first = cycle.loc[cycle["direction"] == -1]
+    c_last = cycle.loc[cycle["direction"] == 1]
+
+    converter = Converter(**kwargs)
+
+    converter.set_data(c_first["capacity"], c_first["voltage"])
+    converter.inspect_data()
+    converter.pre_process_data()
+    converter.increment_data()
+    converter.post_process_data()
+    voltage_first = converter.voltage_processed
+    incremental_capacity_first = converter.incremental_capacity
+
+    if splitter:
+        voltage_first = np.append(voltage_first, np.NaN)
+        incremental_capacity_first = np.append(incremental_capacity_first, np.NaN)
+
+    converter = Converter(**kwargs)
+
+    converter.set_data(c_last["capacity"], c_last["voltage"])
+    converter.inspect_data()
+    converter.pre_process_data()
+    converter.increment_data()
+    converter.post_process_data()
+    voltage_last = converter.voltage_processed[::-1]
+    incremental_capacity_last = converter.incremental_capacity[::-1]
+
+    voltage = np.concatenate((voltage_first, voltage_last))
+    incremental_capacity = np.concatenate(
+        (incremental_capacity_first, incremental_capacity_last)
+    )
+
+    if label_direction:
+        direction_first = -np.ones(len(voltage_first))
+        direction_last = np.ones(len(voltage_last))
+        direction = np.concatenate((direction_first, direction_last))
+        return voltage, incremental_capacity, direction
+
+    return voltage, incremental_capacity
+
+
+def dqdv_cycles(cycles, not_merged=False, label_direction=False, **kwargs):
+    """Convenience functions for creating dq-dv data from given capacity and
+    voltage cycles.
+
+    Returns a DataFrame with a 'voltage' and a 'incremental_capacity'
+    column.
+
+    Args:
+        cycles (pandas.DataFrame): the cycle data ('cycle', 'voltage',
+             'capacity', 'direction' (1 or -1)).
+        not_merged (bool): return list of frames instead of concatenating (
+            defaults to False).
+        label_direction (bool): include 'direction' (1 or -1).
+
+    Returns:
+        ``pandas.DataFrame`` with columns 'cycle', 'voltage', 'dq' (and 'direction' if label_direction is True).
+
+    Additional key-word arguments are sent to Converter:
+
+    Keyword Args:
+        points_pr_split (int): only used when investigating data using
+            splits, defaults to 10.
+        max_points: None
+        voltage_resolution (float): used for interpolating voltage data
+            (e.g. 0.005)
+        capacity_resolution: used for interpolating capacity data
+        minimum_splits (int): defaults to 3.
+        interpolation_method: scipy interpolation method
+        increment_method (str): defaults to "diff"
+        pre_smoothing (bool): set to True for pre-smoothing (window)
+        smoothing (bool): set to True for smoothing during
+            differentiation (window)
+        post_smoothing (bool): set to True for post-smoothing (gaussian)
+        normalize (bool): set to True for normalizing to capacity
+        normalizing_factor (float):
+        normalizing_roof  (float):
+        savgol_filter_window_divisor_default (int): used for window
+            smoothing, defaults to 50
+        savgol_filter_window_order: used for window smoothing
+        voltage_fwhm (float): used for setting the post-processing
+            gaussian sigma, defaults to 0.01
+        gaussian_order (int): defaults to 0
+        gaussian_mode (str): defaults to "reflect"
+        gaussian_cval (float): defaults to 0.0
+        gaussian_truncate (float): defaults to 4.0
+
+    Example:
+        >>> cycles_df = my_data.get_cap(
+        >>> ...   categorical_column=True,
+        >>> ...   method = "forth-and-forth",
+        >>> ...   label_cycle_number=True,
+        >>> ...   insert_nan=False,
+        >>> ... )
+        >>> ica_df = ica.dqdv_cycles(cycles_df)
+
+    """
+
+    # TODO: should add option for normalising based on first cycle capacity
+    # this is e.g. done by first finding the first cycle capacity (nom_cap)
+    # (or use nominal capacity given as input) and then propagating this to
+    # Converter using the key-word arguments
+    #   normalize=True, normalization_factor=1.0, normalization_roof=nom_cap
+
+    if len(cycles) < 1:
+        logging.debug("The food was without nutrition")
+        return pd.DataFrame()
+
+    ica_dfs = list()
+    cycle_group = cycles.groupby("cycle")
+    keys = list()
+    for cycle_number, cycle in cycle_group:
+        cycle = cycle.dropna()
+        if label_direction:
+            v, dq, direction = dqdv_cycle(
+                cycle, splitter=True, label_direction=True, **kwargs
+            )
+            _d = {"voltage": v, "dq": dq, "direction": direction}
+            _cols = ["voltage", "dq", "direction"]
+        else:
+            v, dq = dqdv_cycle(cycle, splitter=True, label_direction=False, **kwargs)
+            _d = {"voltage": v, "dq": dq}
+            _cols = ["voltage", "dq"]
+
+        _ica_df = pd.DataFrame(_d)
+        if not not_merged:
+            _cols.insert(0, "cycle")
+            _ica_df["cycle"] = cycle_number
+            _ica_df = _ica_df[_cols]
+        else:
+            keys.append(cycle_number)
+            _ica_df = _ica_df[_cols]
+        ica_dfs.append(_ica_df)
+
+    if not_merged:
+        return keys, ica_dfs
+
+    ica_df = pd.concat(ica_dfs)
+    return ica_df
+
+
+def dqdv(
+    voltage,
+    capacity,
+    voltage_resolution=None,
+    capacity_resolution=None,
+    voltage_fwhm=0.01,
+    pre_smoothing=True,
+    diff_smoothing=False,
+    post_smoothing=True,
+    post_normalization=True,
+    interpolation_method=None,
+    gaussian_order=None,
+    gaussian_mode=None,
+    gaussian_cval=None,
+    gaussian_truncate=None,
+    points_pr_split=None,
+    savgol_filter_window_divisor_default=None,
+    savgol_filter_window_order=None,
+    max_points=None,
+    **kwargs,
+):
+    """Convenience functions for creating dq-dv data from given capacity
+    and voltage data.
+
+    Args:
+        voltage: nd.array or pd.Series
+        capacity: nd.array or pd.Series
+        voltage_resolution: used for interpolating voltage data (e.g. 0.005)
+        capacity_resolution: used for interpolating capacity data
+        voltage_fwhm: used for setting the post-processing gaussian sigma
+        pre_smoothing: set to True for pre-smoothing (window)
+        diff_smoothing: set to True for smoothing during differentiation
+            (window)
+        post_smoothing: set to True for post-smoothing (gaussian)
+        post_normalization: set to True for normalizing to capacity
+        interpolation_method: scipy interpolation method
+        gaussian_order: int
+        gaussian_mode: mode
+        gaussian_cval:
+        gaussian_truncate:
+        points_pr_split: only used when investigating data using splits
+        savgol_filter_window_divisor_default: used for window smoothing
+        savgol_filter_window_order: used for window smoothing
+        max_points: restricting to max points in vector (capacity-selected)
+
+    Returns:
+        (voltage, dqdv)
+
+    """
+    # Notes:
+    #     PEC data
+    #         pre_smoothing = False
+    #         diff_smoothing = False
+    #         pos_smoothing = False
+    #         voltage_resolution = 0.005
+    #     PEC data
+    #         ...
+    #     Arbin data (IFE)
+    #         ...
+
+    converter = Converter(**kwargs)
+    logging.debug("dqdv - starting")
+    logging.debug("dqdv - created Converter obj")
+    converter.pre_smoothing = pre_smoothing
+    converter.post_smoothing = post_smoothing
+    converter.smoothing = diff_smoothing
+    converter.normalize = post_normalization
+    converter.voltage_fwhm = voltage_fwhm
+    logging.debug(f"converter.pre_smoothing: {converter.pre_smoothing}")
+    logging.debug(f"converter.post_smoothing: {converter.post_smoothing}")
+    logging.debug(f"converter.smoothing: {converter.smoothing}")
+    logging.debug(f"converter.normalise: {converter.normalize}")
+    logging.debug(f"converter.voltage_fwhm: {converter.voltage_fwhm}")
+
+    if voltage_resolution is not None:
+        converter.voltage_resolution = voltage_resolution
+
+    if capacity_resolution is not None:
+        converter.capacity_resolution = capacity_resolution
+
+    if savgol_filter_window_divisor_default is not None:
+        converter.savgol_filter_window_divisor_default = (
+            savgol_filter_window_divisor_default
+        )
+
+        logging.debug(
+            f"converter.savgol_filter_window_divisor_default: "
+            f"{converter.savgol_filter_window_divisor_default}"
+        )
+
+    if savgol_filter_window_order is not None:
+        converter.savgol_filter_window_order = savgol_filter_window_order
+
+        logging.debug(
+            f"converter.savgol_filter_window_order: "
+            f"{converter.savgol_filter_window_order}"
+        )
+
+    if gaussian_mode is not None:
+        converter.gaussian_mode = gaussian_mode
+
+    if gaussian_order is not None:
+        converter.gaussian_order = gaussian_order
+
+    if gaussian_truncate is not None:
+        converter.gaussian_truncate = gaussian_truncate
+
+    if gaussian_cval is not None:
+        converter.gaussian_cval = gaussian_cval
+
+    if interpolation_method is not None:
+        converter.interpolation_method = interpolation_method
+
+    if points_pr_split is not None:
+        converter.points_pr_split = points_pr_split
+
+    if max_points is not None:
+        converter.max_points = max_points
+
+    converter.set_data(capacity, voltage)
+    converter.inspect_data()
+    converter.pre_process_data()
+    converter.increment_data()
+    converter.post_process_data()
+
+    return converter.voltage_processed, converter.incremental_capacity
+
+
+def dqdv_frames(cell, split=False, tidy=True, label_direction=False, **kwargs):
+    """Returns dqdv data as pandas.DataFrame(s) for all cycles.
+
+    Args:
+        cell (CellpyCell-object).
+        split (bool): return one frame for charge and one for
+            discharge if True (defaults to False).
+        tidy (bool): returns the split frames in wide format (defaults
+            to True. Remark that this option is currently not available
+            for non-split frames).
+
+    Returns:
+        one or two ``pandas.DataFrame`` with the following columns:
+        cycle: cycle number (if split is set to True).
+        voltage: voltage
+        dq: the incremental capacity
+
+
+    Additional key-word arguments are sent to Converter:
+
+    Keyword Args:
+        cycle (int or list of ints (cycle numbers)): will process all (or up to max_cycle_number)
+            if not given or equal to None.
+        points_pr_split (int): only used when investigating data
+            using splits, defaults to 10.
+        max_points: None
+        voltage_resolution (float): used for interpolating voltage
+            data (e.g. 0.005)
+        capacity_resolution: used for interpolating capacity data
+        minimum_splits (int): defaults to 3.
+        interpolation_method: scipy interpolation method
+        increment_method (str): defaults to "diff"
+        pre_smoothing (bool): set to True for pre-smoothing (window)
+        smoothing (bool): set to True for smoothing during
+            differentiation (window)
+        post_smoothing (bool): set to True for post-smoothing
+            (gaussian)
+        normalize (bool): set to True for normalizing to capacity
+        normalizing_factor (float):
+        normalizing_roof  (float):
+        savgol_filter_window_divisor_default (int): used for window
+            smoothing, defaults to 50
+        savgol_filter_window_order: used for window smoothing
+        voltage_fwhm (float): used for setting the post-processing
+            gaussian sigma, defaults to 0.01
+        gaussian_order (int): defaults to 0
+        gaussian_mode (str): defaults to "reflect"
+        gaussian_cval (float): defaults to 0.0
+        gaussian_truncate (float): defaults to 4.0
+
+    Example:
+        >>> from cellpy.utils import ica
+        >>> charge_df, dcharge_df = ica.ica_frames(my_cell, split=True)
+        >>> charge_df.plot(x=("voltage", "v"))
+
+    """
+    # TODO: should add option for normalizing based on first cycle capacity
+    # this is e.g. done by first finding the first cycle capacity (nom_cap)
+    # (or use nominal capacity given as input) and then propagating this to
+    # Converter using the key-word arguments
+    #   normalize=True, normalization_factor=1.0, normalization_roof=nom_cap
+
+    if split:
+        return _dqdv_split_frames(cell, tidy=tidy, **kwargs)
+    else:
+        return _dqdv_combinded_frame(
+            cell, tidy=tidy, label_direction=label_direction, **kwargs
+        )
+
+
+def _constrained_dq_dv_using_dataframes(capacity, minimum_v, maximum_v, **kwargs):
+    converter = Converter(**kwargs)
+    converter.set_data(capacity)
+    converter.inspect_data()
+    converter.pre_process_data()
+    converter.increment_data()
+    converter.fixed_voltage_range = [minimum_v, maximum_v, 100]
+    converter.post_process_data()
+    return converter.voltage_processed, converter.incremental_capacity
+
+
+def _make_ica_charge_curves(cycles_dfs, cycle_numbers, minimum_v, maximum_v, **kwargs):
+    incremental_charge_list = []
+
+    for c, n in zip(cycles_dfs, cycle_numbers):
+        if c.empty:
+            logging.info(f"{n} is empty")
+            v = [np.nan]
+            dq = [np.nan]
+        else:
+            v, dq = _constrained_dq_dv_using_dataframes(
+                c, minimum_v, maximum_v, **kwargs
+            )
+        if not incremental_charge_list:
+            d = pd.DataFrame({"v": v})
+            d.name = "voltage"
+            incremental_charge_list.append(d)
+
+            d = pd.DataFrame({f"dq": dq})
+            d.name = n
+            incremental_charge_list.append(d)
+
+        else:
+            d = pd.DataFrame({f"dq": dq})
+            # d.name = f"{cycle}"
+            d.name = n
+            incremental_charge_list.append(d)
+
+    return incremental_charge_list
+
+
+def _dqdv_combinded_frame(cell, tidy=True, label_direction=False, **kwargs):
+    """Returns full cycle dqdv data for all cycles as one pd.DataFrame.
+
+    Args:
+        cell: CellpyCell-object
+
+    Returns:
+        pandas.DataFrame with the following columns:
+            cycle: cycle number
+            voltage: voltage
+            dq: the incremental capacity
+    """
+    cycle = kwargs.pop("cycle", None)
+    number_of_points = kwargs.pop("number_of_points", None)
+    cycles = cell.get_cap(
+        cycle=cycle,
+        method="forth-and-forth",
+        categorical_column=True,
+        label_cycle_number=True,
+        insert_nan=False,
+        number_of_points=number_of_points,
+    )
+    ica_df = dqdv_cycles(
+        cycles, not_merged=not tidy, label_direction=label_direction, **kwargs
+    )
+
+    if not tidy:
+        # dqdv_cycles returns a list of cycle numbers and a list of DataFrames
+        # if not_merged is set to True (or not False)
+        keys, ica_df = ica_df
+        ica_df = pd.concat(ica_df, axis=1, keys=keys)
+        return ica_df
+
+    assert isinstance(ica_df, pd.DataFrame)
+    return ica_df
+
+
+def _dqdv_split_frames(
+    cell,
+    tidy=False,
+    trim_taper_steps=None,
+    steps_to_skip=None,
+    steptable=None,
+    max_cycle_number=None,
+    **kwargs,
+):
+    """Returns dqdv data as pandas.DataFrames for all cycles.
+
+    Args:
+        cell (CellpyCell-object).
+        tidy (bool): return in wide format if False (default),
+            long (tidy) format if True.
+
+    Returns:
+        (charge_ica_frame, discharge_ica_frame) where the frames are
+        pandas.DataFrames where the first column is voltage ('v') and
+        the following columns are the incremental capcaity for each
+        cycle (multi-indexed, where cycle number is on the top level).
+
+    Example:
+        >>> from cellpy.utils import ica
+        >>> charge_ica_df, dcharge_ica_df = ica.ica_frames(my_cell)
+        >>> charge_ica_df.plot(x=("voltage", "v"))
+
+    """
+    cycle = kwargs.pop("cycle", None)
+    if cycle and not isinstance(cycle, (list, tuple)):
+        cycle = [cycle]
+
+    charge_dfs, cycles, minimum_v, maximum_v = collect_capacity_curves(
+        cell,
+        direction="charge",
+        trim_taper_steps=trim_taper_steps,
+        steps_to_skip=steps_to_skip,
+        steptable=steptable,
+        max_cycle_number=max_cycle_number,
+        cycle=cycle,
+    )
+    logging.debug(f"retrieved {len(charge_dfs)} charge cycles")
+    # charge_df = pd.concat(
+    # charge_dfs, axis=1, keys=[k.name for k in charge_dfs])
+
+    ica_charge_dfs = _make_ica_charge_curves(
+        charge_dfs, cycles, minimum_v, maximum_v, **kwargs
+    )
+
+    ica_charge_df = pd.concat(
+        ica_charge_dfs, axis=1, keys=[k.name for k in ica_charge_dfs]
+    )
+
+    dcharge_dfs, cycles, minimum_v, maximum_v = collect_capacity_curves(
+        cell,
+        direction="discharge",
+        trim_taper_steps=trim_taper_steps,
+        steps_to_skip=steps_to_skip,
+        steptable=steptable,
+        max_cycle_number=max_cycle_number,
+        cycle=cycle,
+    )
+    logging.debug(f"retrieved {len(dcharge_dfs)} discharge cycles")
+    ica_dcharge_dfs = _make_ica_charge_curves(
+        dcharge_dfs, cycles, minimum_v, maximum_v, **kwargs
+    )
+    ica_discharge_df = pd.concat(
+        ica_dcharge_dfs, axis=1, keys=[k.name for k in ica_dcharge_dfs]
+    )
+    ica_charge_df.columns.names = ["cycle", "value"]
+    ica_discharge_df.columns.names = ["cycle", "value"]
+
+    if tidy:
+        ica_charge_df = ica_charge_df.melt(
+            "voltage", var_name="cycle", value_name="dq", col_level=0
+        )
+        ica_discharge_df = ica_discharge_df.melt(
+            "voltage", var_name="cycle", value_name="dq", col_level=0
+        )
+
+    return ica_charge_df, ica_discharge_df
+
+
+def _check_class_ica():
+    print(40 * "=")
+    print("running check_class_ica")
+    print(40 * "-")
+
+    import matplotlib.pyplot as plt
+
+    cell = _get_a_cell_to_play_with()
+    cycle = 5
+    print("looking at cycle %i" % cycle)
+
+    # ---------- processing and plotting ----------------
+    fig, (ax1, ax2) = plt.subplots(2, 1)
+    capacity, voltage = cell.get_ccap(cycle, as_frame=False)
+    ax1.plot(capacity, voltage, "b.-", label="raw")
+    converter = Converter()
+    converter.set_data(capacity, voltage)
+    converter.inspect_data()
+    converter.pre_process_data()
+    ax1.plot(
+        converter.capacity_preprocessed,
+        converter.voltage_preprocessed,
+        "r.-",
+        alpha=0.3,
+        label="pre-processed",
+    )
+
+    converter.increment_data()
+    ax2.plot(
+        converter.voltage_processed,
+        converter.incremental_capacity,
+        "b.-",
+        label="incremented",
+    )
+
+    converter.fixed_voltage_range = False
+    converter.post_smoothing = True
+    converter.normalize = False
+    converter.post_process_data()
+    ax2.plot(
+        converter.voltage_processed,
+        converter.incremental_capacity,
+        "y-",
+        alpha=0.3,
+        lw=4.0,
+        label="smoothed",
+    )
+
+    converter.fixed_voltage_range = np.array((0.1, 1.2, 100))
+    converter.post_smoothing = False
+    converter.normalize = False
+    converter.post_process_data()
+    ax2.plot(
+        converter.voltage_processed,
+        converter.incremental_capacity,
+        "go",
+        alpha=0.7,
+        label="fixed voltage range",
+    )
+    ax1.legend(numpoints=1)
+    ax2.legend(numpoints=1)
+    ax1.set_ylabel("Voltage (V)")
+    ax1.set_xlabel("Capacity (mAh/g)")
+    ax2.set_xlabel("Voltage (V)")
+    ax2.set_ylabel("dQ/dV (mAh/g/V)")
+    plt.show()
+
+
+def _get_a_cell_to_play_with():
+    from cellpy import cellreader
+
+    # -------- defining overall path-names etc ----------
+    current_file_path = os.path.dirname(os.path.realpath(__file__))
+    print(current_file_path)
+    relative_test_data_dir = "../../testdata/hdf5"
+    test_data_dir = os.path.abspath(
+        os.path.join(current_file_path, relative_test_data_dir)
+    )
+    # test_data_dir_out = os.path.join(test_data_dir, "out")
+    test_cellpy_file = "20160805_test001_45_cc.h5"
+    test_cellpy_file_full = os.path.join(test_data_dir, test_cellpy_file)
+    # mass = 0.078609164
+
+    # ---------- loading test-data ----------------------
+    cell = cellreader.CellpyCell()
+    cell.load(test_cellpy_file_full)
+    list_of_cycles = cell.get_cycle_numbers()
+    number_of_cycles = len(list_of_cycles)
+    print("you have %i cycles" % number_of_cycles)
+    # cell.save(test_cellpy_file_full)
+    return cell
+
+
+def _check_if_works():
+    import pandas as pd
+    from cellpy import cellreader
+
+    cell = _get_a_cell_to_play_with()
+
+    a = dqdv_frames(cell)
+    print("Hei")
+
+
+if __name__ == "__main__":
+    _check_if_works()
```

### Comparing `cellpy-1.0.0a9/cellpy/utils/ocv_rlx.py` & `cellpy-1.0.0b0/cellpy/utils/ocv_rlx.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,14 +240,15 @@
         where the OCV relaxation is performed according to the standard protocol
         implemented at IFE in the battery development group.
 
         If you want to use this for other data or protocols, please report an issue
         on the GitHub page.
 
     """
+
     def __init__(self, cellpydata, cycles, circuits=3):
         """Object for performing fitting of multiple cycles.
 
         Args:
             cellpydata: ``CellpyCell-object``
             cycles (list): cycles to fit.
             circuits (int): number of circuits to use in fitting.
@@ -317,23 +318,27 @@
 
         for cycle in self.cycles:
             print("Fitting cycle " + str(cycle))
             if cycle == 1 and direction == "down":
                 remove_first = True
             else:
                 remove_first = False
-            time_voltage = self.data.get_ocv(direction=direction, cycles=cycle, remove_first=remove_first)
+            time_voltage = self.data.get_ocv(
+                direction=direction, cycles=cycle, remove_first=remove_first
+            )
             time_step = time_voltage.step_time
             voltage = time_voltage.voltage
 
             if voltage is not None:
                 try:
                     end_current, end_voltage = self.find_zero(cycle, direction)
                 except IndexError as e:
-                    warnings.warn(f"Could not find zero current and voltage for cycle {cycle}")
+                    warnings.warn(
+                        f"Could not find zero current and voltage for cycle {cycle}"
+                    )
                     print(e)
                 else:
                     ocv_fitter.set_zero_voltage(end_voltage)
                     ocv_fitter.set_zero_current(end_current)
                     ocv_fitter.set_data(time_step, voltage)
                     if weighted:
                         ocv_fitter.set_weights_power_law()
@@ -342,46 +347,46 @@
                         ocv_fitter.run_fit()
                     except Exception as e:
                         print(f"COULD NOT FIT CYCLE {cycle}")
                         print(e)
                     else:
                         self.fit_cycles.append(cycle)
                         self.result.append(ocv_fitter.get_result())
-                        self.best_fit_parameters.append(ocv_fitter.get_best_fit_parameters())
+                        self.best_fit_parameters.append(
+                            ocv_fitter.get_best_fit_parameters()
+                        )
                         self.best_fit_parameters_translated.append(
                             ocv_fitter.get_best_fit_parameters_translated()
                         )
                         self.best_fit_data.append(ocv_fitter.get_best_fit_data())
 
     def find_zero(self, cycle, direction):
         step_table = self.data.data.steps
         hdr = self.data.headers_step_table
         end_current = 0
         end_voltage = 0
         if direction == "up":
             end_voltage = step_table[
                 (step_table["cycle"] == cycle)
                 & (step_table["type"].isin(["discharge"]))
-                ][hdr.voltage + "_last"].values[0]
+            ][hdr.voltage + "_last"].values[0]
 
             end_current = step_table[
                 (step_table["cycle"] == cycle)
                 & (step_table["type"].isin(["discharge"]))
-                ][hdr.current + "_last"].values[0]
+            ][hdr.current + "_last"].values[0]
 
         elif direction == "down":
             end_voltage = step_table[
-                (step_table["cycle"] == cycle)
-                & (step_table["type"].isin(["charge"]))
-                ][hdr.voltage + "_last"].values[0]
+                (step_table["cycle"] == cycle) & (step_table["type"].isin(["charge"]))
+            ][hdr.voltage + "_last"].values[0]
 
             end_current = step_table[
-                (step_table["cycle"] == cycle)
-                & (step_table["type"].isin(["charge"]))
-                ][hdr.current + "_last"].values[0]
+                (step_table["cycle"] == cycle) & (step_table["type"].isin(["charge"]))
+            ][hdr.current + "_last"].values[0]
 
         return end_current, end_voltage
 
     def get_best_fit_data(self):
         """Returns the best fit data."""
         return self.best_fit_data
 
@@ -437,15 +442,17 @@
 
     @staticmethod
     def create_colormap(name="plasma", cycles=None):
         if cycles is None:
             cycles = np.arange(1, 101)
         colormap_proxy = np.array(cycles)
         colors = mpl.colormaps.get_cmap(name)
-        norm = mpl.colors.Normalize(vmin=colormap_proxy.min(), vmax=colormap_proxy.max())
+        norm = mpl.colors.Normalize(
+            vmin=colormap_proxy.min(), vmax=colormap_proxy.max()
+        )
         cmap = mpl.cm.ScalarMappable(norm=norm, cmap=colors)
         cmap.set_array([])
         return cmap
 
     def plot_summary(self, cycles=None):
         """Convenience function for plotting the summary of the fit"""
         if cycles is None:
@@ -557,15 +564,17 @@
         primarily used for fitting data that does not originate from cellpy,
         but it can also be used for fitting cellpy-data.
 
         If you have cellpy-data, you should use the MultiCycleOcvFit class instead.
 
     """
 
-    def __init__(self, circuits=None, direction=None, zero_current=0.1, zero_voltage=0.05):
+    def __init__(
+        self, circuits=None, direction=None, zero_current=0.1, zero_voltage=0.05
+    ):
         """Initializes the class.
 
         Args:
             circuits (int): The number of circuits to be fitted (including R0).
             direction (str): The direction of the relaxation (up or down).
             zero_current (float): Last current observed before turning the current off.
             zero_voltage (float): Last voltage observed before turning the current off.
@@ -874,21 +883,23 @@
     ocv_fit = OcvFit()
     ocv_fit.set_cellpydata(c, 1)
     ocv_fit.set_circuits(n)
     ocv_fit.create_model()
     ocv_fit.run_fit()
 
     # Plotting
-    fig1, (ax1, ax2) = plt.subplots(2, 1, sharex="col", gridspec_kw={"height_ratios": [3, 1]})
+    fig1, (ax1, ax2) = plt.subplots(
+        2, 1, sharex="col", gridspec_kw={"height_ratios": [3, 1]}
+    )
     fig1.suptitle("Fit")
 
     x, y0, y1 = ocv_fit.get_best_fit_data()
-    diff = 100*(y0 - y1)/y0
+    diff = 100 * (y0 - y1) / y0
     ax1.plot(x, y0, "x", label="measured")
-    ax1.plot(x, y1, "-",  label="fit")
+    ax1.plot(x, y1, "-", label="fit")
     ax1.legend()
     ax2.plot(x, diff, "-", label="dV (%)")
     ax2.set_xlabel("time (s)")
     ax2.set_ylabel("dV (%)")
     ax1.set_ylabel("voltage (V)")
     print(ocv_fit.get_best_fit_parameters_translated())
     print(ocv_fit.result.fit_report())
@@ -930,15 +941,15 @@
     ocv_fit = MultiCycleOcvFit(c, cycles, circuits=n)
     ocv_fit.run_fitting(direction="down")
     ocv_fit.plot_summary()
     ocv_fit.plot_summary_translated()
 
     # Printing best fit parameters
     for best_fit_parameters in ocv_fit.get_best_fit_parameters():
-        print(50 * '-')
+        print(50 * "-")
         print(best_fit_parameters)
 
     print("SUMMARY")
     print(50 * "-")
     print(ocv_fit.summary_translated())
```

### Comparing `cellpy-1.0.0a9/cellpy/utils/plotutils.py` & `cellpy-1.0.0b0/cellpy/utils/plotutils.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy/utils/processor.py` & `cellpy-1.0.0b0/cellpy/utils/processor.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/cellpy.egg-info/PKG-INFO` & `cellpy-1.0.0b0/cellpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellpy
-Version: 1.0.0a9
+Version: 1.0.0b0
 Summary: Extract and manipulate data from battery data testers.
 Home-page: https://github.com/jepegit/cellpy
 Author: Jan Petter Maehlen
 Author-email: jepe@ife.no
 License: MIT license
 Keywords: cellpy
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cellpy-1.0.0a9/cellpy.egg-info/SOURCES.txt` & `cellpy-1.0.0b0/cellpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/Makefile` & `cellpy-1.0.0b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png` & `cellpy-1.0.0b0/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png` & `cellpy-1.0.0b0/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png` & `cellpy-1.0.0b0/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png` & `cellpy-1.0.0b0/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png` & `cellpy-1.0.0b0/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png` & `cellpy-1.0.0b0/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png` & `cellpy-1.0.0b0/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png` & `cellpy-1.0.0b0/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png` & `cellpy-1.0.0b0/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png` & `cellpy-1.0.0b0/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png` & `cellpy-1.0.0b0/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png` & `cellpy-1.0.0b0/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png` & `cellpy-1.0.0b0/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png` & `cellpy-1.0.0b0/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png` & `cellpy-1.0.0b0/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png` & `cellpy-1.0.0b0/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png` & `cellpy-1.0.0b0/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png` & `cellpy-1.0.0b0/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/_build/_images/templates_jupyterlab_001.png` & `cellpy-1.0.0b0/docs/_build/_images/templates_jupyterlab_001.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/_build/_images/tutorials_utils_plotting_fig1.png` & `cellpy-1.0.0b0/docs/_build/_images/tutorials_utils_plotting_fig1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/_build/_images/tutorials_utils_plotting_fig2.png` & `cellpy-1.0.0b0/docs/_build/_images/tutorials_utils_plotting_fig2.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/adapted_readme.rst` & `cellpy-1.0.0b0/docs/adapted_readme.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/conf.py` & `cellpy-1.0.0b0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/developers_guide/dev_cellpy_data_structure.rst` & `cellpy-1.0.0b0/docs/developers_guide/dev_cellpy_data_structure.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/developers_guide/dev_cellpy_folder_structure.rst` & `cellpy-1.0.0b0/docs/developers_guide/dev_cellpy_folder_structure.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/developers_guide/dev_cellpy_packaging_pypi.rst` & `cellpy-1.0.0b0/docs/developers_guide/dev_cellpy_packaging_pypi.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/developers_guide/dev_cellpy_setup.rst` & `cellpy-1.0.0b0/docs/developers_guide/dev_cellpy_setup.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/developers_guide/dev_conda_package.rst` & `cellpy-1.0.0b0/docs/developers_guide/dev_conda_package.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/developers_guide/dev_docs.rst` & `cellpy-1.0.0b0/docs/developers_guide/dev_docs.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/developers_guide/dev_loaders_and_instruments.rst` & `cellpy-1.0.0b0/docs/developers_guide/dev_loaders_and_instruments.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/developers_guide/dev_various.rst` & `cellpy-1.0.0b0/docs/developers_guide/dev_various.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst` & `cellpy-1.0.0b0/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst` & `cellpy-1.0.0b0/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst` & `cellpy-1.0.0b0/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst` & `cellpy-1.0.0b0/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/05_configuring.rst` & `cellpy-1.0.0b0/docs/examples_and_tutorials/basic_interactions/05_configuring.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/06_pandas.rst` & `cellpy-1.0.0b0/docs/examples_and_tutorials/basic_interactions/06_pandas.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst` & `cellpy-1.0.0b0/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst` & `cellpy-1.0.0b0/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png` & `cellpy-1.0.0b0/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png` & `cellpy-1.0.0b0/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/examples_and_tutorials/tips_and_tricks.rst` & `cellpy-1.0.0b0/docs/examples_and_tutorials/tips_and_tricks.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/examples_and_tutorials/utils/batch.rst` & `cellpy-1.0.0b0/docs/examples_and_tutorials/utils/batch.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png` & `cellpy-1.0.0b0/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png` & `cellpy-1.0.0b0/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/examples_and_tutorials/utils/ica.rst` & `cellpy-1.0.0b0/docs/examples_and_tutorials/utils/ica.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/examples_and_tutorials/utils/plotting.rst` & `cellpy-1.0.0b0/docs/examples_and_tutorials/utils/plotting.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst` & `cellpy-1.0.0b0/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/figures/cellpy-icon-bw.png` & `cellpy-1.0.0b0/docs/figures/cellpy-icon-bw.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/figures/cellpy-logo-v1.png` & `cellpy-1.0.0b0/docs/figures/cellpy-logo-v1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/index.rst` & `cellpy-1.0.0b0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/main_description/formats.rst` & `cellpy-1.0.0b0/docs/main_description/formats.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/main_description/installation.rst` & `cellpy-1.0.0b0/docs/main_description/installation.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/main_description/usage.rst` & `cellpy-1.0.0b0/docs/main_description/usage.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/make.bat` & `cellpy-1.0.0b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/source/cellpy.parameters.rst` & `cellpy-1.0.0b0/docs/source/cellpy.parameters.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/source/cellpy.readers.instruments.configurations.rst` & `cellpy-1.0.0b0/docs/source/cellpy.readers.instruments.configurations.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/source/cellpy.readers.instruments.loader_specific_modules.rst` & `cellpy-1.0.0b0/docs/source/cellpy.readers.instruments.loader_specific_modules.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/source/cellpy.readers.instruments.processors.rst` & `cellpy-1.0.0b0/docs/source/cellpy.readers.instruments.processors.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/source/cellpy.readers.instruments.rst` & `cellpy-1.0.0b0/docs/source/cellpy.readers.instruments.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/source/cellpy.readers.rst` & `cellpy-1.0.0b0/docs/source/cellpy.readers.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/source/cellpy.rst` & `cellpy-1.0.0b0/docs/source/cellpy.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/source/cellpy.utils.batch_tools.rst` & `cellpy-1.0.0b0/docs/source/cellpy.utils.batch_tools.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/docs/source/cellpy.utils.rst` & `cellpy-1.0.0b0/docs/source/cellpy.utils.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a9/setup.py` & `cellpy-1.0.0b0/setup.py`

 * *Files identical despite different names*

