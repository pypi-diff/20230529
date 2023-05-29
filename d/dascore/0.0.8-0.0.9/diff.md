# Comparing `tmp/dascore-0.0.8.tar.gz` & `tmp/dascore-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dascore-0.0.8.tar", last modified: Mon Dec 19 22:21:14 2022, max compression
+gzip compressed data, was "dascore-0.0.9.tar", last modified: Wed Feb  1 02:44:26 2023, max compression
```

## Comparing `dascore-0.0.8.tar` & `dascore-0.0.9.tar`

### file list

```diff
@@ -1,196 +1,202 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.993130 dascore-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-19 22:20:06.000000 dascore-0.0.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.965130 dascore-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.965130 dascore-0.0.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2022-12-19 22:20:06.000000 dascore-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      383 2022-12-19 22:20:06.000000 dascore-0.0.8/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2022-12-19 22:20:06.000000 dascore-0.0.8/.github/pull_reqest_template.md
--rw-r--r--   0 runner    (1001) docker     (123)       65 2022-12-19 22:20:06.000000 dascore-0.0.8/.github/test_condarc.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.965130 dascore-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2022-12-19 22:20:06.000000 dascore-0.0.8/.github/workflows/build_deploy_docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      902 2022-12-19 22:20:06.000000 dascore-0.0.8/.github/workflows/get_coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      469 2022-12-19 22:20:06.000000 dascore-0.0.8/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2022-12-19 22:20:06.000000 dascore-0.0.8/.github/workflows/runtests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      671 2022-12-19 22:20:06.000000 dascore-0.0.8/.github/workflows/upload_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      973 2022-12-19 22:20:06.000000 dascore-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2022-12-19 22:20:06.000000 dascore-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2022-12-19 22:21:13.993130 dascore-0.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.969130 dascore-0.0.8/dascore/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      620 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.969130 dascore-0.0.8/dascore/clients/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/clients/dirspool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/clients/filespool.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.969130 dascore-0.0.8/dascore/core/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9462 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/core/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/core/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    11918 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/core/spool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/data_registry.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5844 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.969130 dascore-0.0.8/dascore/io/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17226 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/io/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.973130 dascore-0.0.8/dascore/io/dasdae/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/io/dasdae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/io/dasdae/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/io/dasdae/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8025 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/io/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.973130 dascore-0.0.8/dascore/io/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/io/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/io/pickle/core.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/io/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.973130 dascore-0.0.8/dascore/io/tdms/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/io/tdms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/io/tdms/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    13979 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/io/tdms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.973130 dascore-0.0.8/dascore/io/terra15/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/io/terra15/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/io/terra15/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/io/terra15/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.973130 dascore-0.0.8/dascore/io/wav/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/io/wav/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/io/wav/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.973130 dascore-0.0.8/dascore/proc/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/proc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/proc/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/proc/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/proc/detrend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/proc/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/proc/resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/proc/select.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.973130 dascore-0.0.8/dascore/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/transform/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/transform/spectro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/transform/strain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.977130 dascore-0.0.8/dascore/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/utils/chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/utils/coords.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/utils/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/utils/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13186 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/utils/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/utils/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    24037 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/utils/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12641 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/utils/pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.977130 dascore-0.0.8/dascore/viz/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/viz/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/viz/spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2022-12-19 22:20:06.000000 dascore-0.0.8/dascore/viz/waterfall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.969130 dascore-0.0.8/dascore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2022-12-19 22:21:13.000000 dascore-0.0.8/dascore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2022-12-19 22:21:13.000000 dascore-0.0.8/dascore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 22:21:13.000000 dascore-0.0.8/dascore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2022-12-19 22:21:13.000000 dascore-0.0.8/dascore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2022-12-19 22:21:13.000000 dascore-0.0.8/dascore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-19 22:21:13.000000 dascore-0.0.8/dascore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.981130 dascore-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/_quarto.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.981130 dascore-0.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   203131 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   201049 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)   893070 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/_static/patch_n_spool.png
--rw-r--r--   0 runner    (1001) docker     (123)      204 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/acknowledgements.md
--rw-r--r--   0 runner    (1001) docker     (123)      188 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.985130 dascore-0.0.8/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/contributing/adding_test_data.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     5639 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/contributing/code_of_conduct.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/contributing/contributing.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/contributing/dev_install.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/contributing/documentation.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/contributing/general_guidelines.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/contributing/new_format.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      956 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/contributing/style_and_linting.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/contributing/testing.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      470 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/contributors.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.985130 dascore-0.0.8/docs/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/filters/fill_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/index.css
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/index.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/quickstart.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.985130 dascore-0.0.8/docs/recipes/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/recipes/overview.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.985130 dascore-0.0.8/docs/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/tutorial/concepts.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/tutorial/file_io.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/tutorial/patch.qmd
--rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/tutorial/processing.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/tutorial/spool.qmd
--rw-r--r--   0 runner    (1001) docker     (123)       29 2022-12-19 22:20:06.000000 dascore-0.0.8/docs/tutorial/visualization.qmd
--rwxr-xr-x   0 runner    (1001) docker     (123)      232 2022-12-19 22:20:06.000000 dascore-0.0.8/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2022-12-19 22:20:06.000000 dascore-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      936 2022-12-19 22:20:06.000000 dascore-0.0.8/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.985130 dascore-0.0.8/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2022-12-19 22:20:06.000000 dascore-0.0.8/scripts/_index_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15739 2022-12-19 22:20:06.000000 dascore-0.0.8/scripts/_render_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.985130 dascore-0.0.8/scripts/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2022-12-19 22:20:06.000000 dascore-0.0.8/scripts/_templates/notes.md
--rw-r--r--   0 runner    (1001) docker     (123)      231 2022-12-19 22:20:06.000000 dascore-0.0.8/scripts/_templates/parent_source_block.html
--rw-r--r--   0 runner    (1001) docker     (123)      256 2022-12-19 22:20:06.000000 dascore-0.0.8/scripts/_templates/signature.html
--rw-r--r--   0 runner    (1001) docker     (123)      474 2022-12-19 22:20:06.000000 dascore-0.0.8/scripts/_templates/table.html
--rw-r--r--   0 runner    (1001) docker     (123)      323 2022-12-19 22:20:06.000000 dascore-0.0.8/scripts/build_api_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2022-12-19 22:21:13.993130 dascore-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.985130 dascore-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.989130 dascore-0.0.8/tests/test_clients/
--rw-r--r--   0 runner    (1001) docker     (123)     8973 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_clients/test_dirspool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_clients/test_filespool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.989130 dascore-0.0.8/tests/test_core/
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_core/test_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_core/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    15226 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_core/test_spool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.989130 dascore-0.0.8/tests/test_io/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.989130 dascore-0.0.8/tests/test_io/test_dasdae/
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_io/test_dasdae/test_dasdae.py
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_io/test_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_io/test_io_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.989130 dascore-0.0.8/tests/test_io/test_pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      996 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_io/test_pickle/test_pickle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.989130 dascore-0.0.8/tests/test_io/test_tdms/
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_io/test_tdms/test_tdms_v4713.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.989130 dascore-0.0.8/tests/test_io/test_terra15/
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_io/test_terra15/test_terra15_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_io/test_terra15/test_terra15_v5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.989130 dascore-0.0.8/tests/test_io/test_wav/
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_io/test_wav/test_wav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.989130 dascore-0.0.8/tests/test_proc/
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_proc/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_proc/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_proc/test_detrend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_proc/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8958 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_proc/test_resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_proc/test_select.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.993130 dascore-0.0.8/tests/test_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_transform/test_fft_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_transform/test_spectro_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_transform/test_velocity_to_strainrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.993130 dascore-0.0.8/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_utils/test_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9679 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_utils/test_chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_utils/test_coord_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_utils/test_doc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_utils/test_frozen_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_utils/test_hdf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_utils/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9475 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_utils/test_patch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_utils/test_pd.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_utils/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    12337 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_utils/test_time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 22:21:13.993130 dascore-0.0.8/tests/test_viz/
--rw-r--r--   0 runner    (1001) docker     (123)      993 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_viz/test_spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2022-12-19 22:20:06.000000 dascore-0.0.8/tests/test_viz/test_waterfall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.690258 dascore-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-01 02:43:26.000000 dascore-0.0.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.658257 dascore-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.658257 dascore-0.0.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-02-01 02:43:26.000000 dascore-0.0.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-02-01 02:43:26.000000 dascore-0.0.9/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-02-01 02:43:26.000000 dascore-0.0.9/.github/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-01 02:43:26.000000 dascore-0.0.9/.github/test_condarc.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.658257 dascore-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-02-01 02:43:26.000000 dascore-0.0.9/.github/workflows/build_deploy_docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-02-01 02:43:26.000000 dascore-0.0.9/.github/workflows/get_coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-02-01 02:43:26.000000 dascore-0.0.9/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-02-01 02:43:26.000000 dascore-0.0.9/.github/workflows/runtests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-02-01 02:43:26.000000 dascore-0.0.9/.github/workflows/upload_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-02-01 02:43:26.000000 dascore-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-02-01 02:43:26.000000 dascore-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-02-01 02:44:26.690258 dascore-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.662257 dascore-0.0.9/dascore/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.662257 dascore-0.0.9/dascore/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/clients/dirspool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/clients/filespool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.662257 dascore-0.0.9/dascore/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/core/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/core/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/core/spool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/data_registry.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.666257 dascore-0.0.9/dascore/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17668 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/io/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.666257 dascore-0.0.9/dascore/io/dasdae/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/io/dasdae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/io/dasdae/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/io/dasdae/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/io/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.666257 dascore-0.0.9/dascore/io/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/io/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/io/pickle/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/io/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.666257 dascore-0.0.9/dascore/io/tdms/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/io/tdms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/io/tdms/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13975 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/io/tdms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.666257 dascore-0.0.9/dascore/io/terra15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/io/terra15/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/io/terra15/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/io/terra15/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.666257 dascore-0.0.9/dascore/io/wav/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/io/wav/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/io/wav/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.670257 dascore-0.0.9/dascore/proc/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/proc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/proc/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/proc/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/proc/detrend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/proc/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/proc/resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/proc/select.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.670257 dascore-0.0.9/dascore/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/transform/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/transform/spectro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/transform/strain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.670257 dascore-0.0.9/dascore/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/utils/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/utils/coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/utils/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/utils/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12996 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/utils/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/utils/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23703 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/utils/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12641 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/utils/pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.674258 dascore-0.0.9/dascore/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/viz/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/viz/spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/viz/waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-02-01 02:43:26.000000 dascore-0.0.9/dascore/viz/wiggle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.662257 dascore-0.0.9/dascore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-02-01 02:44:26.000000 dascore-0.0.9/dascore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-02-01 02:44:26.000000 dascore-0.0.9/dascore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 02:44:26.000000 dascore-0.0.9/dascore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-02-01 02:44:26.000000 dascore-0.0.9/dascore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-01 02:44:26.000000 dascore-0.0.9/dascore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-01 02:44:26.000000 dascore-0.0.9/dascore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.674258 dascore-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/_quarto.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.674258 dascore-0.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   203131 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   201049 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   893070 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/_static/patch_n_spool.png
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/acknowledgements.md
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.678258 dascore-0.0.9/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/contributing/adding_test_data.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/contributing/code_of_conduct.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/contributing/contributing.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/contributing/dev_install.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/contributing/documentation.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/contributing/general_guidelines.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/contributing/new_format.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/contributing/style_and_linting.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/contributing/testing.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/contributors.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.678258 dascore-0.0.9/docs/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/filters/fill_links.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.678258 dascore-0.0.9/docs/filters/filter_test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    19133 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/filters/filter_test_data/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)   173712 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/filters/filter_test_data/test_data_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.678258 dascore-0.0.9/docs/recipes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/recipes/contributing_to_documentation.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/recipes/how_to_contribute.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/recipes/overview.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.682258 dascore-0.0.9/docs/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/tutorial/concepts.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/tutorial/file_io.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/tutorial/patch.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/tutorial/processing.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/tutorial/spool.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-01 02:43:26.000000 dascore-0.0.9/docs/tutorial/visualization.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-01 02:43:26.000000 dascore-0.0.9/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-02-01 02:43:26.000000 dascore-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-02-01 02:43:26.000000 dascore-0.0.9/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.682258 dascore-0.0.9/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-02-01 02:43:26.000000 dascore-0.0.9/scripts/_index_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16454 2023-02-01 02:43:26.000000 dascore-0.0.9/scripts/_render_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.682258 dascore-0.0.9/scripts/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-01 02:43:26.000000 dascore-0.0.9/scripts/_templates/notes.md
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-01 02:43:26.000000 dascore-0.0.9/scripts/_templates/parent_source_block.html
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-02-01 02:43:26.000000 dascore-0.0.9/scripts/_templates/signature.html
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-02-01 02:43:26.000000 dascore-0.0.9/scripts/_templates/table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-02-01 02:43:26.000000 dascore-0.0.9/scripts/build_api_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-02-01 02:44:26.690258 dascore-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.682258 dascore-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.682258 dascore-0.0.9/tests/test_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_clients/test_dirspool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_clients/test_filespool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.682258 dascore-0.0.9/tests/test_core/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_core/test_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_core/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15226 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_core/test_spool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.682258 dascore-0.0.9/tests/test_io/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.686258 dascore-0.0.9/tests/test_io/test_dasdae/
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_io/test_dasdae/test_dasdae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_io/test_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_io/test_io_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.686258 dascore-0.0.9/tests/test_io/test_pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_io/test_pickle/test_pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.686258 dascore-0.0.9/tests/test_io/test_tdms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_io/test_tdms/test_tdms_v4713.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.686258 dascore-0.0.9/tests/test_io/test_terra15/
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_io/test_terra15/test_terra15_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_io/test_terra15/test_terra15_v5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.686258 dascore-0.0.9/tests/test_io/test_wav/
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_io/test_wav/test_wav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.686258 dascore-0.0.9/tests/test_proc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_proc/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_proc/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_proc/test_detrend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_proc/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_proc/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_proc/test_select.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.686258 dascore-0.0.9/tests/test_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_transform/test_fft_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_transform/test_spectro_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_transform/test_velocity_to_strainrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.690258 dascore-0.0.9/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_utils/test_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_utils/test_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_utils/test_coord_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_utils/test_doc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_utils/test_frozen_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_utils/test_hdf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_utils/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_utils/test_patch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_utils/test_pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_utils/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_utils/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 02:44:26.690258 dascore-0.0.9/tests/test_viz/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_viz/test_spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_viz/test_waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-02-01 02:43:26.000000 dascore-0.0.9/tests/test_viz/test_wiggle.py
```

### Comparing `dascore-0.0.8/.github/pull_reqest_template.md` & `dascore-0.0.9/.github/pull_request_template.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-
+ <!--
 Thanks for contributing to DASCore, community contributions are most welcomed!
 
 Before contributing, please read through the [contributors doc](https://dascore.org/contributing/contributing.html)
 
 Before making big changes to the code or adding large complex features, it is a good idea to
 [open a discussion](https://github.com/DASDAE/dascore/discussions). Don't hesitate to ask a question or for
 help if something isn't clear.
+-->
 
 ## Description
 
+<!--
 Please describe your PR here. What problem are you trying to solve, or what feature are you adding?
 
 Also link any relevant issues/discussions (this can be done using the issue/discussion number preceded by a
 pound sign, e.g. `#12` without the backticks)
+-->
 
 ## Checklist
 
 I have (if applicable):
 
 - [ ] referenced the GitHub issue this PR closes.
-- [ ] [run pre-commit](https://dascore.org/contributing/style_and_linting.html) to ensure new code conform to DASCore's style guide.
-- [ ] documented the new feature in docstrings or appropriate doc page.
-- [ ] updated the changelog file (docs/changelog.md).
+- [ ] documented the new feature with docstrings or appropriate doc page.
 - [ ] included a test. See [testing guidelines](https://dascore.org/contributing/testing.html).
-- [ ] first time contributors have been added to the contributors page (docs/contributors.md).
+- [ ] your name has been added to the contributors page (docs/contributors.md).
+- [ ] added the "ready_for_review" tag once the PR is ready to be reviewed.
```

### Comparing `dascore-0.0.8/.github/workflows/build_deploy_docs.yaml` & `dascore-0.0.9/.github/workflows/build_deploy_docs.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     steps:
       - uses: actions/checkout@v3
 
       - name: Setup conda
         uses: conda-incubator/setup-miniconda@v2
         with:
           miniconda-version: 'latest'
-          python-version: ${{ matrix.python-version }}
+          python-version: "3.10"
           activate-environment: dascore
           environment-file: environment.yml
           condarc-file: .github/test_condarc.yml
 
       - name: install dascore with docbuild reqs
         shell: bash -l {0}
         run: |
```

### Comparing `dascore-0.0.8/.github/workflows/get_coverage.yml` & `dascore-0.0.9/.github/workflows/get_coverage.yml`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     steps:
       - uses: actions/checkout@v1
 
       - name: Setup conda
         uses: conda-incubator/setup-miniconda@v2
         with:
           miniconda-version: 'latest'
-          python-version: 3.9
+          python-version: 3.10
           channels: conda-forge
 
       - name: install dascore
         shell: bash -l {0}
         run: |
           python -m pip install -e .[test]
```

### Comparing `dascore-0.0.8/.github/workflows/runtests.yml` & `dascore-0.0.9/.github/workflows/runtests.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 name: TestCode
-on: [push]
+on:
+  push:
+    branches:
+    - master
+  pull_request:
+    branches:
+    - master
 
 # Cancel previous runs when this one starts.
 concurrency:
   group: TestCode-${{ github.event.pull_request.number || github.run_id }}
   cancel-in-progress: true
 
 
@@ -11,15 +17,15 @@
   # Runs the tests on combinations of the supported python/os matrix.
   test_code:
 
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: ['3.9', '3.10']
+        python-version: ['3.9', '3.10', '3.11']
 
     # only run if CI isn't turned off
     if: github.event_name == 'push' || !contains(github.event.pull_request.labels.*.name, 'no_ci')
 
     steps:
       - uses: actions/checkout@v2
```

### Comparing `dascore-0.0.8/.github/workflows/upload_pypi.yml` & `dascore-0.0.9/.github/workflows/upload_pypi.yml`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/.gitignore` & `dascore-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/.pre-commit-config.yaml` & `dascore-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/__init__.py` & `dascore-0.0.9/dascore/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """DASCore - A library for fiber optic sensing."""
 # set xarray settings
 from xarray import set_options
 
 from dascore.core.patch import Patch
+from dascore.core.schema import PatchAttrs
 from dascore.core.spool import BaseSpool, spool
 from dascore.examples import get_example_patch, get_example_spool
 from dascore.io.core import get_format, read, scan, scan_to_df, write
 from dascore.utils.patch import patch_function
 from dascore.utils.time import to_datetime64, to_timedelta64
 from dascore.version import __last_version__, __version__
```

### Comparing `dascore-0.0.8/dascore/clients/dirspool.py` & `dascore-0.0.9/dascore/clients/dirspool.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/clients/filespool.py` & `dascore-0.0.9/dascore/clients/filespool.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,47 @@
 """
 A spool for working with a single file.
 """
 
 from pathlib import Path
-from typing import Union
+from typing import Optional, Union
 
 from typing_extensions import Self
 
 import dascore as dc
 from dascore.constants import SpoolType
 from dascore.core.spool import DataFrameSpool
 from dascore.io.core import FiberIO
 
 
 class FileSpool(DataFrameSpool):
     """
     A spool for a single file.
 
+    Parameters
+    ----------
+    path
+        The path to the file.
+    file_format
+        The format name, optional.
+    file_version
+        The version string of the format, optional.
+
+    Notes
+    -----
     Some file formats support storing multiple patches, this is most useful
     for those formats, but should work on all dascore supported formats.
     """
 
-    def __init__(self, path: Union[str, Path], file_format=None, file_version=None):
-        """"""
+    def __init__(
+        self,
+        path: Union[str, Path],
+        file_format: Optional[str] = None,
+        file_version: Optional[str] = None,
+    ):
         super().__init__()
         self._path = Path(path)
         if not self._path.exists() or self._path.is_dir():
             msg = f"{path} does not exist or is a directory"
             raise FileNotFoundError(msg)
 
         _format, _version = dc.get_format(path, file_format, file_version)
```

### Comparing `dascore-0.0.8/dascore/core/patch.py` & `dascore-0.0.9/dascore/core/patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 
 import numpy as np
 import pandas as pd
 from numpy.typing import ArrayLike
 from xarray import DataArray
 
 import dascore.proc
-from dascore.constants import DEFAULT_PATCH_ATTRS, PatchType
+from dascore.constants import PatchType
+from dascore.core.schema import PatchAttrs
 from dascore.io import PatchIO
 from dascore.transform import TransformPatchNameSpace
 from dascore.utils.coords import Coords, assign_coords
-from dascore.utils.mapping import FrozenDict
+
+# from dascore.utils.mapping import FrozenDict
 from dascore.utils.patch import _AttrsCoordsMixer
 from dascore.viz import VizPatchNameSpace
 
 
 class Patch:
     """
     A Class for managing data and metadata.
@@ -41,14 +43,19 @@
         Optional attributes (non-coordinate metadata) passed as a dict.
 
     Notes
     -----
     Unless data is a DataArray or Patch, data, coords, and dims are required.
     """
 
+    data: ArrayLike
+    coords: Mapping[str, ArrayLike]
+    dims: tuple[str, ...]
+    attrs: PatchAttrs
+
     def __init__(
         self,
         data: ArrayLike | DataArray | None = None,
         coords: Mapping[str, ArrayLike] | None = None,
         dims: Sequence[str] | None = None,
         attrs: Optional[Mapping] = None,
     ):
@@ -99,15 +106,15 @@
             A Trace2D object
         only_required_attrs
             If True, only compare required attributes. This helps avoid issues
             with comparing histories or custom attrs of patches, for example.
         """
 
         if only_required_attrs:
-            attrs_to_compare = set(DEFAULT_PATCH_ATTRS) - {"history"}
+            attrs_to_compare = set(PatchAttrs.get_defaults()) - {"history"}
             attrs1 = {x: self.attrs.get(x, None) for x in attrs_to_compare}
             attrs2 = {x: other.attrs.get(x, None) for x in attrs_to_compare}
         else:
             attrs1, attrs2 = dict(self.attrs), dict(other.attrs)
         if set(attrs1) != set(attrs2):  # attrs don't have same keys; not equal
             return False
         if attrs1 != attrs2:
@@ -201,17 +208,17 @@
 
     @property
     def dims(self) -> tuple[str, ...]:
         """Return the dimensions contained in patch."""
         return self._data_array.dims
 
     @property
-    def attrs(self) -> FrozenDict:
+    def attrs(self) -> PatchAttrs:
         """Return the attributes of the trace."""
-        return FrozenDict(self._data_array.attrs)
+        return PatchAttrs(**self._data_array.attrs)
 
     @property
     def shape(self) -> tuple[int, ...]:
         """Return the shape of the data array."""
         return self._data_array.shape
 
     def to_xarray(self):
@@ -228,20 +235,23 @@
 
     # --- processing funcs
 
     select = dascore.proc.select
     decimate = dascore.proc.decimate
     detrend = dascore.proc.detrend
     pass_filter = dascore.proc.pass_filter
+    sobel_filter = dascore.proc.sobel_filter
+    median_filter = dascore.proc.median_filter
     aggregate = dascore.proc.aggregate
     abs = dascore.proc.abs
     resample = dascore.proc.resample
     iresample = dascore.proc.iresample
     interpolate = dascore.proc.interpolate
     normalize = dascore.proc.normalize
+    standardize = dascore.proc.standardize
 
     # --- Method Namespaces
     # Note: these can't be cached_property (from functools) or references
     # to self stick around and keep large arrays in memory.
 
     @property
     def viz(self) -> VizPatchNameSpace:
```

### Comparing `dascore-0.0.8/dascore/core/spool.py` & `dascore-0.0.9/dascore/core/spool.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,14 +91,15 @@
         pass
 
 
 class DataFrameSpool(BaseSpool):
     """
     An abstract class for spools whose contents are managed by a dataframe.
     """
+
     # A dataframe which represents contents as they will be output
     _df: pd.DataFrame = CacheDescriptor("_cache", "_get_df")
     # A dataframe which shows patches in the source
     _source_df: pd.DataFrame = CacheDescriptor("_cache", "_get_source_df")
     # A dataframe of instructions for going from source_df to df
     _instruction_df: pd.DataFrame = CacheDescriptor("_cache", "_get_instruction_df")
     # kwargs for filtering contents
```

### Comparing `dascore-0.0.8/dascore/data_registry.txt` & `dascore-0.0.9/dascore/data_registry.txt`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/examples.py` & `dascore-0.0.9/dascore/examples.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """A module for loading examples."""
 
 import tempfile
 from pathlib import Path
+from typing import Sequence, Union
 
 import numpy as np
 
 import dascore as dc
 from dascore.utils.misc import register_func
 from dascore.utils.patch import get_default_patch_name
 from dascore.utils.time import to_datetime64, to_timedelta64
@@ -38,15 +39,14 @@
     rand = np.random.RandomState(13)
     array = rand.random(size=(300, 2_000))
     t1 = np.datetime64(starttime)
     attrs = dict(
         d_distance=1,
         d_time=to_timedelta64(1 / 250),
         category="DAS",
-        id="test_data1",
         time_min=t1,
         network=network,
         station=station,
         tag=tag,
     )
     coords = dict(
         distance=np.arange(array.shape[0]) * attrs["d_distance"],
@@ -55,18 +55,19 @@
     out = dict(data=array, coords=coords, attrs=attrs, dims=("distance", "time"))
     return dc.Patch(**out)
 
 
 @register_func(EXAMPLE_PATCHES, key="sin_wav")
 def sin_wave_patch(
     sample_rate=44100,
-    frequency=100,
+    frequency: Union[Sequence[float], float] = 100.0,
     time_min="2020-01-01",
     channel_count=3,
     duration=1,
+    amplitude=10,
 ):
     """
     Return a Patch composed of simple 1 second sin waves.
 
     This is useful for debugging output to audio formats.
 
     Parameters
@@ -77,21 +78,27 @@
         The frequency of the sin wave.
     time_min
         The start time in the metadata.
     channel_count
         The number of  distance channels to include.
     duration
         Duration of signal in seconds.
-
+    amplitude
+        The amplitude of the sin wave.
     """
     t_array = np.linspace(0.0, duration, sample_rate * duration)
-    sin_data = 10 * np.sin(2.0 * np.pi * frequency * t_array)
-    data = np.stack([sin_data] * channel_count).T
-    time = to_timedelta64(t_array) + np.datetime64(time_min)
+    # Get time and distance coords
     distance = np.arange(1, channel_count + 1, 1)
+    time = to_timedelta64(t_array) + np.datetime64(time_min)
+    freqs = [frequency] if isinstance(frequency, (float, int)) else frequency
+    # init empty data and add frequencies.
+    data = np.zeros((len(time), len(distance)))
+    for freq in freqs:
+        sin_data = amplitude * np.sin(2.0 * np.pi * freq * t_array)
+        data += sin_data[..., np.newaxis]
 
     patch = dc.Patch(
         data=data,
         coords={"time": time, "distance": distance},
         dims=("time", "distance"),
         attrs={
             "time_min": to_datetime64(time_min),
@@ -154,21 +161,21 @@
     There are various gaps, tags, station names, etc.
     """
     spool_no_gaps = _random_spool()
     spool_no_gaps_different_network = _random_spool(network="das2")
     spool_big_gaps = _random_spool(d_time=np.timedelta64(1, "s"), station="big_gaps")
     spool_overlaps = _random_spool(d_time=-np.timedelta64(10, "ms"), station="overlaps")
     dt = to_timedelta64(spool_big_gaps[0].attrs["d_time"] / np.timedelta64(1, "s"))
-    spool_small_gaps = _random_spool(d_time=dt, station="small_gaps")
+    spool_small_gaps = _random_spool(d_time=dt, station="smallg")
     spool_way_late = _random_spool(
-        length=1, starttime=np.datetime64("2030-01-01"), station="way_out"
+        length=1, starttime=np.datetime64("2030-01-01"), station="wayout"
     )
     spool_new_tag = _random_spool(tag="some_tag", length=1)
     spool_way_early = _random_spool(
-        length=1, starttime=np.datetime64("1989-05-04"), station="way_out"
+        length=1, starttime=np.datetime64("1989-05-04"), station="wayout"
     )
 
     all_spools = [
         spool_no_gaps,
         spool_no_gaps_different_network,
         spool_big_gaps,
         spool_overlaps,
```

### Comparing `dascore-0.0.8/dascore/exceptions.py` & `dascore-0.0.9/dascore/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,7 +55,11 @@
 
 class InvalidFileHandler(TypeError, DASCoreError):
     """Raised when a writable file handler is requested from a read handle."""
 
 
 class InvalidIndexVersionError(ValueError, DASCoreError):
     """Raised when a version mismatch occurs in index."""
+
+
+class MissingOptionalDependency(ImportError, DASCoreError):
+    """Raised when an optional package needed for some functionality is missing."""
```

### Comparing `dascore-0.0.8/dascore/io/core.py` & `dascore-0.0.9/dascore/io/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 Base functionality for reading, writing, determining file formats, and scanning
 Das Data.
 """
 import os.path
 from abc import ABC
 from collections import defaultdict
-from functools import cache, cached_property
+from functools import cache, cached_property, reduce
 from importlib.metadata import entry_points
+from operator import add
 from pathlib import Path
 from typing import List, Optional, Union
 
 import pandas as pd
+from typing_extensions import Self
 
-import dascore
+import dascore as dc
 from dascore.constants import PatchType, SpoolType, timeable_types
 from dascore.core.schema import PatchFileSummary
 from dascore.exceptions import (
     DASCoreError,
     InvalidFiberFile,
     InvalidFileFormatter,
     UnknownFiberFormat,
@@ -104,15 +106,15 @@
         self._format_version[forma][ver] = fiberio
 
     def get_fiberio(
         self,
         format: Optional[str] = None,
         version: Optional[str] = None,
         extension: Optional[str] = None,
-    ):
+    ) -> "FiberIO":
         """
         Return the most likely formatter for given inputs.
 
         If no such formatter exists, raise UnknownFiberFormat error.
 
         Parameters
         ----------
@@ -132,15 +134,15 @@
             return formatter
 
     def yield_fiberio(
         self,
         format: Optional[str] = None,
         version: Optional[str] = None,
         extension: Optional[str] = None,
-    ):
+    ) -> Self:
         """
         Yields fiber IO object based on input priorities.
 
         The order is sorted in likelihood of the formatter being correct. For
         example, if file format is specified but file_version is not, all
         formatters for the format will be yielded with the newest versions
         first in the list.
@@ -374,24 +376,24 @@
         file_format=file_format,
         file_version=file_version,
         ignore=ignore,
     )
     df = pd.DataFrame([dict(x) for x in info]).assign(
         dims=lambda x: list_ser_to_str(x["dims"])
     )
-    return df
+    return df[list(PatchFileSummary.get_index_columns())]
 
 
 @compose_docstring(fields=list(PatchFileSummary.__annotations__))
 def scan(
     path_or_spool: Union[Path, str, PatchType, SpoolType],
     file_format: Optional[str] = None,
     file_version: Optional[str] = None,
     ignore: bool = False,
-) -> List[PatchFileSummary]:
+) -> list[PatchFileSummary]:
     """
     Scan a file, return the summary dictionary.
 
     Parameters
     ----------
     path_or_spool
         The path the to file to scan
@@ -407,33 +409,45 @@
 
     Notes
     -----
     The summary dictionaries contain the following fields:
         {fields}
     """
     if isinstance(path_or_spool, (str, Path)):
-        return _scan_from_path(
+        out = _scan_from_path(
             path_or_spool,
             file_format=file_format,
             file_version=file_version,
             ignore=ignore,
         )
-    return scan_patches(path_or_spool)
+    else:
+        out = scan_patches(path_or_spool)
+    return out
 
 
 def _scan_from_path(
     path: Union[Path, str, PatchType, SpoolType],
     file_format: Optional[str] = None,
     file_version: Optional[str] = None,
     ignore: bool = False,
-):
+) -> list[PatchFileSummary]:
     """Scan from a single path."""
-    if not os.path.exists(path) or os.path.isdir(path):
-        msg = f"{path} does not exist or is a directory"
+    if not os.path.exists(path):
+        msg = f"{path} does not exist"
         raise InvalidFiberFile(msg)
+    # recursively handle directory files
+    if os.path.isdir(path):
+        out = [
+            _scan_from_path(x, file_format, file_version, ignore=True)
+            for x in Path(path).glob("*")
+        ]
+        if len(out):
+            return reduce(add, out)
+        else:
+            return []
     # dispatch to file format handlers
     if not file_format or not file_version:
         try:
             file_format, file_version = get_format(
                 path,
                 file_format=file_format,
                 file_version=file_version,
@@ -513,11 +527,11 @@
         version.
 
     Raises
     ------
     dascore.exceptions.UnknownFiberFormat - Could not determine the fiber format.
     """
     formatter = FiberIO.manager.get_fiberio(file_format, file_version)
-    if not isinstance(patch_or_spool, dascore.BaseSpool):
-        patch_or_spool = dascore.spool([patch_or_spool])
+    if not isinstance(patch_or_spool, dc.BaseSpool):
+        patch_or_spool = dc.spool([patch_or_spool])
     formatter.write(patch_or_spool, path, **kwargs)
     return path
```

### Comparing `dascore-0.0.8/dascore/io/dasdae/core.py` & `dascore-0.0.9/dascore/io/dasdae/core.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/io/dasdae/utils.py` & `dascore-0.0.9/dascore/io/dasdae/utils.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/io/indexer.py` & `dascore-0.0.9/dascore/io/indexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     Parameters
     ----------
     path
         The path to a directory containing DAS files.
     cache_size
         The number of queries to store in memory to avoid frequent reads
-        of the index file.
+        of the index file. It is rare this needs to be modified.
     """
 
     # hdf5 compression defaults
     ext = ""
     namespace = ""
     index_name = ".dascore_index.h5"  # name of index file
     executor = None  # an executor for using parallelism
```

### Comparing `dascore-0.0.8/dascore/io/pickle/core.py` & `dascore-0.0.9/dascore/io/pickle/core.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/io/tdms/core.py` & `dascore-0.0.9/dascore/io/tdms/core.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/io/tdms/utils.py` & `dascore-0.0.9/dascore/io/tdms/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 import datetime
 import mmap
 import os
 import struct
 
 import numpy as np
 
-from dascore.core.schema import PatchSummary
+from dascore.core.schema import PatchAttrs
 from dascore.utils.misc import get_slice
 from dascore.utils.time import to_datetime64
 
-DEFAULT_ATTRS = tuple(PatchSummary.__fields__)
+DEFAULT_ATTRS = tuple(PatchAttrs.__fields__)
 
 
 def type_not_supported(vargin):
     """Function raises a NotImplementedException."""
     raise NotImplementedError("Reading of this tdsDataType is not implemented")
 
 
@@ -213,15 +213,15 @@
 
     # loop through and read each property
     out = [_read_attr(tdms_file) for _ in range(var)]
     # Returns a pandas dataframe that we convert to dictionary
     out = dict(out)
     # Add other attributes not yet included
     out["n_channels"] = n_channels
-    out["data_type"] = "strain rate"
+    out["data_type"] = "strain_rate"
     out["data_units"] = ""
     out["dims"] = "time, distance"
     out["d_time"] = 1 / out["SamplingFrequency[Hz]"]
     out["time_min"] = to_datetime64(str(out["GPSTimeStamp"]))
     # Rename some attributes to preferred names
     _root_attrs = {
         "SpatialResolution[m]": "d_distance",
```

### Comparing `dascore-0.0.8/dascore/io/terra15/__init__.py` & `dascore-0.0.9/dascore/io/terra15/__init__.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/io/terra15/core.py` & `dascore-0.0.9/dascore/io/terra15/core.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/io/terra15/utils.py` & `dascore-0.0.9/dascore/io/terra15/utils.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/io/wav/core.py` & `dascore-0.0.9/dascore/io/wav/core.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/proc/aggregate.py` & `dascore-0.0.9/dascore/proc/aggregate.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/proc/resample.py` & `dascore-0.0.9/dascore/proc/resample.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,78 +1,89 @@
 """
 Module for re-sampling patches.
 """
-from typing import Union
+from typing import Literal, Union
 
 import numpy as np
+from scipy.signal import decimate as scipy_decimate
 
-import dascore
+import dascore as dc
 import dascore.compat as compat
 from dascore.constants import PatchType
 from dascore.exceptions import FilterValueError
-from dascore.proc.filter import _get_sampling_rate, _lowpass_cheby_2
 from dascore.utils.misc import check_evenly_sampled
 from dascore.utils.patch import (
     get_dim_value_from_kwargs,
     get_start_stop_step,
     patch_function,
 )
 from dascore.utils.time import to_number, to_timedelta64
 
 
 @patch_function()
 def decimate(
     patch: PatchType,
-    lowpass: bool = True,
+    filter_type: Literal["iir", "fir", None] = "iir",
     copy=True,
     **kwargs,
 ) -> PatchType:
     """
     Decimate a patch along a dimension.
 
     Parameters
     ----------
-    lowpass
-        If True, first apply a low-pass (anti-alis) filter.
+    filter_type
+        filter type to use to avoid aliasing. Options are:
+            iir - infinite impulse response
+            fir - finite impulse response
+            None - No pre-filtering
     copy
         If True, copy the decimated data array. This is needed if you want
         the old array to get gc'ed to free memory otherwise a view is returned.
+        Only applies when filter_type == None.
     **kwargs
-        Used to pass dimension and factor. For example time=10 is 10x
+        Used to pass dimension and factor. For example `time=10` is 10x
         decimation along the time axis.
+
+    Notes
+    -----
+    Simply uses scipy.signal.decimate if filter_type is specified. Otherwise,
+    just slice data long specified dimension only including every n samples.
+
+    Examples
+    --------
+    # Simple example using iir
+    >>> import dascore as dc
+    >>> patch = dc.get_example_patch()
+    >>> decimated_irr = patch.decimate(time=10, filter_type='iir')
+    >>> # Example using fir along distance dimension
+    >>> decimated_fir = patch.decimate(distance=10, filter_type='fir')
     """
-    # Note: We can't simply use scipy.signal.decimate due to this issue:
-    # https://github.com/scipy/scipy/issues/15072
     dim, axis, factor = get_dim_value_from_kwargs(patch, kwargs)
-    if lowpass:
-        # get new niquest
-        if factor > 16:
+    # Apply scipy.signal.decimate and geet new coords
+    if filter_type:
+        if filter_type == "IRR" and factor > 13:
             msg = (
-                "Automatic filter design is unstable for decimation "
-                + "factors above 16. Manual decimation is necessary."
+                "IRR filter is unstable for decimation factors above"
+                " 13. Call decimate multiple times."
             )
             raise FilterValueError(msg)
-        sr = _get_sampling_rate(patch, dim)
-        freq = sr * 0.5 / float(factor)
-        fdata = _lowpass_cheby_2(patch.data, freq, sr, axis=axis)
-        patch = dascore.Patch(
-            fdata, coords=patch.coords, attrs=patch.attrs, dims=patch.dims
-        )
-
-    kwargs = {dim: slice(None, None, factor)}
-    dar = patch._data_array.sel(**kwargs)
-    # need to create a new xarray so the old, probably large, numpy array
-    # gets gc'ed, otherwise it stays in memory (if lowpass isn't called)
-    data = dar.data if not copy else dar.data.copy()
-    attrs = dar.attrs
-    # update delta_dim since spacing along dimension has changed
-    d_attr = f"d_{dim}"
-    attrs[d_attr] = patch.attrs[d_attr] * factor
-
-    return dascore.Patch(data=data, coords=dar.coords, attrs=dar.attrs, dims=dar.dims)
+        data = scipy_decimate(patch.data, factor, ftype=filter_type, axis=axis)
+        coords = {x: patch.coords[x] for x in patch.dims}
+        coords[dim] = coords[dim][::factor]
+    else:  # No filter, simply slice along specified dimension.
+        dar = patch._data_array.sel(**{dim: slice(None, None, factor)})
+        # Need to copy so array isn't a slice and holds onto reference of parent
+        data = dar.data if not copy else dar.data.copy()
+        coords = dar.coords
+    # Update delta_dim since spacing along dimension has changed.
+    attrs = dict(patch.attrs)
+    attrs[f"d_{dim}"] = patch.attrs[f"d_{dim}"] * factor
+    out = dc.Patch(data=data, coords=coords, attrs=attrs, dims=patch.dims)
+    return out
 
 
 @patch_function()
 def interpolate(
     patch: PatchType, kind: Union[str, int] = "linear", **kwargs
 ) -> PatchType:
     """
@@ -92,15 +103,15 @@
 
     **kwargs
         Used to specify dimension and interpolation values.
 
     Notes
     -----
     This function just uses scipy's interp1d function under the hood.
-    See scipy.inpterp.interp1d for information.
+    See scipy.interpolate.interp1d for information.
 
     Values for interpolation must be evenly-spaced.
     """
     dim, axis, samples = get_dim_value_from_kwargs(patch, kwargs)
     # ensure samples are evenly sampled
     check_evenly_sampled(samples)
     # we need to make sure only real numbers are used, interp1d doesn't support
```

### Comparing `dascore-0.0.8/dascore/proc/select.py` & `dascore-0.0.9/dascore/proc/select.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/transform/fft.py` & `dascore-0.0.9/dascore/transform/fft.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/transform/spectro.py` & `dascore-0.0.9/dascore/transform/spectro.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/transform/strain.py` & `dascore-0.0.9/dascore/transform/strain.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/utils/chunk.py` & `dascore-0.0.9/dascore/utils/chunk.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/utils/coords.py` & `dascore-0.0.9/dascore/utils/coords.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/utils/docs.py` & `dascore-0.0.9/dascore/utils/docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         {some_value}
         '''
     ```
     """
 
     def _wrap(func):
         docstring = func.__doc__
+        assert isinstance(docstring, str)
         # iterate each provided value and look for it in the docstring
         for key, value in kwargs.items():
             value = value if isinstance(value, str) else "\n".join(value)
             # strip out first line if needed
             value = textwrap.dedent(value).lstrip()
             search_value = "{%s}" % key
             # find all lines that match values
```

### Comparing `dascore-0.0.8/dascore/utils/downloader.py` & `dascore-0.0.9/dascore/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/utils/hdf5.py` & `dascore-0.0.9/dascore/utils/hdf5.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import numpy as np
 import pandas as pd
 import tables
 from packaging.version import parse as get_version
 from tables import ClosedNodeError
 
 import dascore as dc
-from dascore.constants import ONE_SECOND_IN_NS
+from dascore.constants import ONE_SECOND_IN_NS, max_lens
 from dascore.core.schema import PatchFileSummary
 from dascore.exceptions import InvalidFileHandler, InvalidIndexVersionError
 from dascore.utils.misc import suppress_warnings
 from dascore.utils.pd import (
     _remove_base_path,
     fill_defaults_from_pydantic,
     list_ser_to_str,
@@ -111,25 +111,15 @@
     """
 
     _complib = "blosc"
     _complevel = 9
     # attributes subclasses need to define
     buffer = ONE_SECOND_IN_NS
     # string column sizes in hdf5 table
-    _min_itemsize = {
-        "path": 120,
-        "file_format": 15,
-        "tag": 8,
-        "network": 8,
-        "station": 8,
-        "dims": 40,
-        "file_version": 9,
-        "cable_id": 40,
-        "instrument_id": 40,
-    }
+    _min_itemsize = max_lens
     # columns which should be indexed for fast querying
     _query_columns = ("time_min", "time_max", "distance_min", "distance_max")
     # functions applied to encode dataframe before saving to hdf5
     _column_encoders = {
         "time_min": to_number,
         "time_max": to_number,
         "d_time": to_number,
@@ -138,15 +128,15 @@
     # functions to apply to decode dataframe after loading from hdf file
     _column_decorders = {
         "time_min": ns_to_datetime,
         "time_max": ns_to_datetime,
         "d_time": ns_to_timedelta,
     }
     _base_model = PatchFileSummary
-    index_columns = tuple(_base_model.__fields__)
+    index_columns = tuple(_base_model.get_index_columns())
     # The minimum version of dascore required to read this index. If an older
     # version is used an error will be raised.
     _min_version = "0.0.1"
 
     def __init__(self, path, namespace=""):
         super().__init__()
         self.namespace = namespace
```

### Comparing `dascore-0.0.8/dascore/utils/mapping.py` & `dascore-0.0.9/dascore/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/utils/misc.py` & `dascore-0.0.9/dascore/utils/misc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 Misc Utilities.
 """
 import contextlib
 import functools
+import importlib
 import os
 import warnings
+from types import ModuleType
 from typing import Iterable, Optional, Union
 
 import numpy as np
 import numpy.typing as nt
 import pandas as pd
 
-from dascore.exceptions import ParameterError
+from dascore.exceptions import MissingOptionalDependency, ParameterError
 
 
 def register_func(list_or_dict: Union[list, dict], key: Optional[str] = None):
     """
     Decorator for registering a function name in a list or dict.
 
     If list_or_dict is a list only append the name of the function. If it is
@@ -262,7 +264,43 @@
             cache[self._name] = out
         return cache[self._name]
 
     def __set__(self, instance, value):
         """Set the cache contents."""
         cache = getattr(instance, self._cache_name)
         cache[self._name] = value
+
+
+def optional_import(package_name: str) -> ModuleType:
+    """
+    Import a module and return the module object if installed, else raise error.
+
+    Parameters
+    ----------
+    package_name
+        The name of the package which may or may not be installed. Can
+        also be sub-packages/modules (eg dascore.core).
+
+    Raises
+    ------
+    MissingOptionalDependency if the package is not installed.
+
+    Examples
+    --------
+    >>> from dascore.utils.misc import optional_import
+    >>> from dascore.exceptions import MissingOptionalDependency
+    >>> # import a module (this is the same as import dascore as dc)
+    >>> dc = optional_import('dascore')
+    >>> try:
+    ...     optional_import('boblib5')  # doesn't exist so this raises
+    ... except MissingOptionalDependency:
+    ...     pass
+    """
+    try:
+        mod = importlib.import_module(package_name)
+    except ImportError:
+        msg = (
+            f"{package_name} is not installed but is required for the "
+            f"requested functionality"
+        )
+        raise MissingOptionalDependency(msg)
+    return mod
```

### Comparing `dascore-0.0.8/dascore/utils/patch.py` & `dascore-0.0.9/dascore/utils/patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,35 +8,29 @@
 import re
 import warnings
 from fnmatch import translate
 from typing import (
     Any,
     Callable,
     Dict,
-    List,
     Literal,
     Mapping,
     Optional,
     Sequence,
     Tuple,
     Union,
 )
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 
-import dascore
-from dascore.constants import (
-    DEFAULT_PATCH_ATTRS,
-    PATCH_MERGE_ATTRS,
-    PatchType,
-    SpoolType,
-)
-from dascore.core.schema import PatchSummaryWithHistory
+import dascore as dc
+from dascore.constants import PATCH_MERGE_ATTRS, PatchType, SpoolType
+from dascore.core.schema import PatchAttrs, PatchFileSummary
 from dascore.exceptions import PatchAttributeError, PatchDimError
 from dascore.utils.coords import Coords
 from dascore.utils.docs import compose_docstring, format_dtypes
 from dascore.utils.misc import append_func
 from dascore.utils.time import to_datetime64, to_timedelta64
 
 attr_type = Union[Dict[str, Any], str, Sequence[str], None]
@@ -143,15 +137,15 @@
     patch_attrs = patch.attrs
     if isinstance(required_attrs, Mapping):
         sub = {i: patch_attrs[i] for i in required_attrs}
         if sub != dict(required_attrs):
             msg = f"Patch's attrs {sub} are not required attrs: {required_attrs}"
             raise PatchAttributeError(msg)
     else:
-        missing = set(required_attrs) - set(patch.attrs)
+        missing = set(required_attrs) - set(dict(patch.attrs))
         if missing:
             msg = f"Patch is missing the following attributes: {missing}"
             raise PatchAttributeError(msg)
     return patch
 
 
 def patch_function(
@@ -375,28 +369,22 @@
     @functools.cached_property
     def copied_coords(self):
         """Make a copy of the coords before mutating."""
         # TODO I don't like having this deep copy but shallow still caused
         return copy.deepcopy(self.coords)
 
     def __call__(self, *args, **kwargs):
-        return self.attrs, self.coords
+        return PatchAttrs(**self.attrs), self.coords
 
     def _set_default_attrs(self):
         """Get the attribute dict, add required keys if not yet defined."""
         # add default values if they are not in out or attrs yet
-        missing = set(DEFAULT_PATCH_ATTRS) - set(self.attrs)
-        if not missing:
-            return
-        self._missing_attr_keys = missing
-        out = copy_attrs(self.attrs)
-        for key in missing:
-            value = DEFAULT_PATCH_ATTRS[key]
-            out[key] = value if not callable(value) else value()
-        self.attrs = out
+        defaults = PatchAttrs.get_defaults()
+        defaults.update(self.attrs)
+        self.attrs = defaults
 
     # --- Coordinate bits
 
     def _update_attrs_from_coords(self, fill_keys=None):
         """Fill in missing attributes that can be inferred."""
         fill_keys = fill_keys if fill_keys else set(self.attrs)
         # iterate each dimension, fill in missing values with data from coords
@@ -442,15 +430,15 @@
         """Make sure time attrs are expected types"""
         for key, (expected_type, func) in self._expected_types.items():
             val = self.attrs[key]
             if not isinstance(val, expected_type):
                 self.copied_attrs[key] = func(val)
 
 
-@compose_docstring(fields=PatchSummaryWithHistory.__annotations__)
+@compose_docstring(fields=PatchAttrs.__annotations__)
 def patches_to_df(
     patches: Union[Sequence[PatchType], SpoolType, pd.DataFrame]
 ) -> pd.DataFrame:
     """
     Return a dataframe
 
     Parameters
@@ -461,22 +449,25 @@
     Returns
     -------
     A dataframe with the following fields:
         {fields}
     plus a field called 'patch' which contains a reference to each patch.
     """
 
-    if isinstance(patches, dascore.BaseSpool):
+    if isinstance(patches, dc.BaseSpool):
         df = patches._df
+    # Handle spool case
+    elif hasattr(patches, "get_contents"):
+        return patches.get_contents()
     elif isinstance(patches, pd.DataFrame):
         return patches
     else:
-        df = pd.DataFrame(scan_patches(patches))
+        df = pd.DataFrame([dict(x) for x in scan_patches(patches)])
         if df.empty:  # create empty df with appropriate columns
-            cols = list(PatchSummaryWithHistory().dict())
+            cols = list(PatchAttrs().dict())
             df = pd.DataFrame(columns=cols).assign(patch=None, history=None)
         else:  # else populate with patches and concat history
             history = df["history"].apply(lambda x: ",".join(x))
             df = df.assign(patch=patches, history=history)
     # Ensure history is in df
     if "history" not in df.columns:
         df = df.assign(history="")
@@ -561,15 +552,15 @@
             _trim_or_fill(x, start) if needs_action else x
             for x, start, needs_action in zip(dars, overlap_start, has_overlap)
         ]
         dar = xr.concat(dars, dim=dim)
         dar.attrs[min_name] = np.NaN
         dar.attrs[max_name] = np.NaN
         dims = tuple(dar.dims)
-        return dascore.Patch(dar.data, coords=dar.coords, attrs=dar.attrs, dims=dims)
+        return dc.Patch(dar.data, coords=dar.coords, attrs=dar.attrs, dims=dims)
 
     def _trim_or_fill(dar, new_start):
         """Trim or fill data array."""
         return dar.loc[{dim: dar.coords[dim] > new_start}]
 
     # get a dataframe
     if not isinstance(patches, pd.DataFrame):
@@ -592,36 +583,32 @@
         sub_df["_dist_to_previous"] = dist_to_previous
         # determine if each patch should be merged with the previous one
         for _, merge_patch_df in sub_df.groupby(no_merge.astype(int).cumsum()):
             out.append(_merge_compatible_patches(merge_patch_df))
     return out
 
 
-@compose_docstring(fields=format_dtypes(PatchSummaryWithHistory.__annotations__))
+@compose_docstring(fields=format_dtypes(PatchFileSummary.__annotations__))
 def scan_patches(
-    patch: Union[PatchType, Sequence[PatchType]]
-) -> List[PatchSummaryWithHistory]:
+    patches: Union[PatchType, Sequence[PatchType]]
+) -> list[PatchFileSummary]:
     """
-    Scan a sequence of patches and return a list of summary dicts.
+    Scan a sequence of patches and return a list of summaries.
 
     The summary dicts have the following fields:
         {fields}
 
     Parameters
     ----------
-    patch
+    patches
         A single patch or a sequence of patches.
     """
-    if isinstance(patch, dascore.Patch):
-        patch = [patch]  # make sure we have an iterable
-    out = []
-    for pa in patch:
-        attrs = pa.attrs
-        summary = {i: attrs.get(i, DEFAULT_PATCH_ATTRS[i]) for i in DEFAULT_PATCH_ATTRS}
-        out.append(PatchSummaryWithHistory.parse_obj(summary).dict())
+    if isinstance(patches, dc.Patch):
+        patches = [patches]  # make sure we have an iterable
+    out = [PatchFileSummary(**dict(pa.attrs)) for pa in patches]
     return out
 
 
 def get_start_stop_step(patch: PatchType, dim):
     """
     Convenience method for getting start, stop, step for a given dimension.
     """
```

### Comparing `dascore-0.0.8/dascore/utils/pd.py` & `dascore-0.0.9/dascore/utils/pd.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/utils/plotting.py` & `dascore-0.0.9/dascore/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/utils/progress.py` & `dascore-0.0.9/dascore/utils/progress.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/utils/time.py` & `dascore-0.0.9/dascore/utils/time.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
 
 from dascore.constants import (
     LARGEDT64,
-    NUMPY_TIME_UNIT_MAPPPING,
+    NUMPY_TIME_UNIT_MAPPING,
     ONE_SECOND,
     SMALLDT64,
     timeable_types,
 )
 from dascore.exceptions import TimeError
 
 
@@ -195,15 +195,15 @@
 def _time_delta_from_str(time_delta_str: str):
     """simply return the time delta."""
     split = time_delta_str.split(" ")
     assert len(split) == 2
     val, units = split
     if units[-1] == "s":
         units = units[:-1]
-    new_unit = NUMPY_TIME_UNIT_MAPPPING[units]
+    new_unit = NUMPY_TIME_UNIT_MAPPING[units]
     return np.timedelta64(int(val), new_unit)
 
 
 def get_select_time(
     time: Union[float, int, np.datetime64, np.timedelta64, str, datetime],
     time_min: Optional[np.datetime64] = None,
     time_max: Optional[np.datetime64] = None,
```

### Comparing `dascore-0.0.8/dascore/viz/spectrogram.py` & `dascore-0.0.9/dascore/viz/spectrogram.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/dascore/viz/waterfall.py` & `dascore-0.0.9/dascore/viz/waterfall.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,21 @@
         are:
             relative - scale based on half the dynamic range in patch
             absolute - scale based on absolute values provided to `scale`
     colorbar
         If True, show the color bar.
     show
         If True, show the plot, else just return axis.
+
+    Examples
+    --------
+    >>> # Plot the default patch
+    >>> import dascore as dc
+    >>> patch = dc.get_example_patch()
+    >>> _ = patch.viz.waterfall(scale=0.1)
     """
     ax = _get_ax(ax)
     cmap = _get_cmap(cmap)
     data = patch.data
     dims = patch.dims
     assert len(dims) == 2, "Can only make waterfall plot of 2D Patch"
     dims_r = tuple(reversed(dims))
```

### Comparing `dascore-0.0.8/dascore.egg-info/SOURCES.txt` & `dascore-0.0.9/dascore.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
 environment.yml
 pyproject.toml
 readme.md
 setup.cfg
-.github/pull_reqest_template.md
+.github/pull_request_template.md
 .github/test_condarc.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/config.yml
 .github/workflows/build_deploy_docs.yaml
 .github/workflows/get_coverage.yml
 .github/workflows/lint.yml
 .github/workflows/runtests.yml
@@ -76,23 +76,23 @@
 dascore/utils/plotting.py
 dascore/utils/progress.py
 dascore/utils/time.py
 dascore/viz/__init__.py
 dascore/viz/core.py
 dascore/viz/spectrogram.py
 dascore/viz/waterfall.py
+dascore/viz/wiggle.py
 docs/.gitignore
 docs/LICENSE
 docs/_quarto.yml
 docs/acknowledgements.md
 docs/changelog.md
 docs/contributors.md
 docs/index.css
 docs/index.qmd
-docs/quickstart.qmd
 docs/references.bib
 docs/styles.css
 docs/_static/logo.png
 docs/_static/logo.svg
 docs/_static/patch_n_spool.png
 docs/contributing/adding_test_data.qmd
 docs/contributing/code_of_conduct.qmd
@@ -100,14 +100,18 @@
 docs/contributing/dev_install.qmd
 docs/contributing/documentation.qmd
 docs/contributing/general_guidelines.qmd
 docs/contributing/new_format.qmd
 docs/contributing/style_and_linting.qmd
 docs/contributing/testing.qmd
 docs/filters/fill_links.py
+docs/filters/filter_test_data/test.json
+docs/filters/filter_test_data/test_data_2.json
+docs/recipes/contributing_to_documentation.qmd
+docs/recipes/how_to_contribute.qmd
 docs/recipes/overview.qmd
 docs/tutorial/concepts.qmd
 docs/tutorial/file_io.qmd
 docs/tutorial/patch.qmd
 docs/tutorial/processing.qmd
 docs/tutorial/spool.qmd
 docs/tutorial/visualization.qmd
@@ -149,8 +153,9 @@
 tests/test_utils/test_hdf_utils.py
 tests/test_utils/test_misc.py
 tests/test_utils/test_patch_utils.py
 tests/test_utils/test_pd.py
 tests/test_utils/test_progress.py
 tests/test_utils/test_time.py
 tests/test_viz/test_spectrogram.py
-tests/test_viz/test_waterfall.py
+tests/test_viz/test_waterfall.py
+tests/test_viz/test_wiggle.py
```

### Comparing `dascore-0.0.8/docs/LICENSE` & `dascore-0.0.9/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/docs/_quarto.yml` & `dascore-0.0.9/docs/_quarto.yml`

 * *Files 7% similar despite different names*

```diff
@@ -90,21 +90,27 @@
 
         - text: Processing
           href: tutorial/processing.qmd
 
         - text: Visualization
           href: tutorial/visualization.qmd
 
-        - text: FIle IO
+        - text: File IO
           href: tutorial/file_io.qmd
 
     - title: 'Recipes'
       contents:
         - recipes/overview.qmd
 
+        - text: How to Contribute?
+          href: recipes/how_to_contribute.qmd
+
+        - text: Contributing to Documentation
+          href: recipes/contributing_to_documentation.qmd
+
     - title: "Contributing"
       contents:
         - contributing/contributing.qmd
 
         - text: Dev Install
           href: contributing/dev_install.qmd
```

### Comparing `dascore-0.0.8/docs/_static/logo.png` & `dascore-0.0.9/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/docs/_static/logo.svg` & `dascore-0.0.9/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/docs/_static/patch_n_spool.png` & `dascore-0.0.9/docs/_static/patch_n_spool.png`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/docs/contributing/adding_test_data.qmd` & `dascore-0.0.9/docs/contributing/adding_test_data.qmd`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/docs/contributing/code_of_conduct.qmd` & `dascore-0.0.9/docs/contributing/code_of_conduct.qmd`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/docs/contributing/contributing.qmd` & `dascore-0.0.9/docs/contributing/contributing.qmd`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ---
 
 Contributions to DASCore are welcomed and appreciated. Before contributing
 please be aware of our [code of conduct](code_of_conduct.qmd).
 
 # Prerequisites
 
-To start, clone DASCore and [install it in development mode](dev_install.qmd).
+To start, clone DASCore and [install it in development mode](dev_install.qmd). If you are new to contributing to open-source projects, this [recipe](../recipes/how_to_contribute.qmd) provides step-by-step instructions.
 
 Review how [DASCore's testing](testing.qmd) works, [how DASCore is documented](documentation.qmd),
 [DAScore style and linting](style_and_linting.qmd), and the [general guidelines](general_guidelines.qmd).
 
 
 
 # Planning
```

### Comparing `dascore-0.0.8/docs/contributing/documentation.qmd` & `dascore-0.0.9/docs/contributing/documentation.qmd`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 just restate obvious parts of the code. Consider refactoring with better named variables or
 smaller, well named functions if you find yourself making lots of these types of comments.
 
 Don't be afraid to make multi-line comments if needed.
 
 # Doc-Strings
 
-Use [numpy style docstrings](https://docs.scipy.org/doc/numpy/docs/howto_document.html). All public code
+Use [numpy style docstrings](https://numpydoc.readthedocs.io/en/latest/format.html). All public code
 (doesn't start with a `_`) should have a "full" docstring but private code (starts with a `_`) can have an
 abbreviated docstring.
 
 DASCore makes extensive use of Python 3's [type hints](https://docs.python.org/3/library/typing.html).
 Please make an effort to accurately annotate public functions/classes/methods.
 
 Here is an example:
@@ -80,15 +80,15 @@
 [quarto code blocks](https://quarto.org/docs/output-formats/html-code.html)
 can be used directly. The latter gives more control over outputs and display options.
 
 # Generating Documentation
 
 DASCore's documentation is built with [quarto](https://quarto.org/). In order to build the documentation, you
 must first [install DASCore in development mode](dev_install.qmd) then
-[install quarto](https://quarto.org/docs/get-started/).
+[install quarto](https://quarto.org/docs/get-started/) and [install panflute](http://scorreia.com/software/panflute/).
 
 Next, the automatic API documents are created with scripts/build_api_docs.py
 
 ```bash
 python scripts/build_api_docs.py
 ```
```

### Comparing `dascore-0.0.8/docs/contributing/general_guidelines.qmd` & `dascore-0.0.9/docs/contributing/general_guidelines.qmd`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/docs/contributing/new_format.qmd` & `dascore-0.0.9/docs/contributing/new_format.qmd`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/docs/contributing/style_and_linting.qmd` & `dascore-0.0.9/docs/contributing/style_and_linting.qmd`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/docs/contributing/testing.qmd` & `dascore-0.0.9/docs/contributing/testing.qmd`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
 Title: "Testing"
 ---
 
 # Testing
 
 DASCore's test suite is run with [pytest](https://docs.pytest.org/en/stable/). While in the base dascore repo
-(and after [installing DASCore for development](dev_install.md)) invoke pytest from the command line:
+(and after [installing DASCore for development](dev_install.qmd)) invoke pytest from the command line:
 
 <!--pytest-codeblocks:skip-->
 ```bash
 pytest tests
 ```
 
 You can also use the cov flags to check coverage. Please make sure you don't
```

### Comparing `dascore-0.0.8/docs/index.css` & `dascore-0.0.9/docs/index.css`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/docs/index.qmd` & `dascore-0.0.9/docs/index.qmd`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/docs/references.bib` & `dascore-0.0.9/docs/references.bib`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/docs/styles.css` & `dascore-0.0.9/docs/styles.css`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/docs/tutorial/concepts.qmd` & `dascore-0.0.9/docs/tutorial/concepts.qmd`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/docs/tutorial/file_io.qmd` & `dascore-0.0.9/docs/tutorial/file_io.qmd`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/docs/tutorial/patch.qmd` & `dascore-0.0.9/docs/tutorial/patch.qmd`

 * *Files 2% similar despite different names*

```diff
@@ -16,26 +16,27 @@
 ## Load an Example Patch
 
 This example patch contains some artificially generated data. They are mostly used
 for simple demonstrations or testing.
 
 ```{python}
 import dascore as dc
+
 pa = dc.get_example_patch()
 ```
 
 ## Load a File
 
 We first download a small example fiber file from a URL in the DASCore library (you need an internet connection).
 Next, we simply read it into a [spool](spool.qmd) object then get the first (and only) patch.
 
 ```{python}
-# get a fiber file
 import dascore as dc
 from dascore.utils.downloader import fetch
+
 path = fetch("terra15_das_1_trimmed.hdf5")  # path to a datafile
 
 pa = dc.read(path)[0]
 # or
 pa = dc.spool(path)[0]
 ```
 
@@ -58,19 +59,18 @@
 
 ```{python}
 import numpy as np
 
 import dascore as dc
 from dascore.utils.time import to_timedelta64
 
-
-## Create the patch data
+# Create the patch data
 array = np.random.random(size=(300, 2_000))
 
-## Create attributes, or metadata
+# Create attributes, or metadata
 t1 = np.datetime64("2017-09-18")
 attrs = dict(
     d_distance=1,
     d_time=to_timedelta64(1 / 250),
     category="DAS",
     id="test_data1",
     time_min=t1,
@@ -85,15 +85,29 @@
 # define dimensions (first label corresponds to data axis 0)
 dims = ('distance', 'time')
 
 pa = dc.Patch(data=array, coords=coords, attrs=attrs, dims=dims)
 print(pa)
 ```
 
+# Attrs
+
+The metadata stored in `Patch.attrs` is a
+[pydnatic model](https://docs.pydantic.dev/usage/models/) which enforces some
+basic schema validation. You can print the schema info like this:
+
+```{python}
+import dascore as dc
+
+print(dc.PatchAttrs.__doc__)
+```
+
+
 # Processing
+
 For various reasons, Patches should be treated as *immutable*, meaning they should
 not be modified in place, but rather new patches created when something needs to be
 modified.
 
 The patch has several methods which are intended to be chained together via a
 [fluent interface](https://en.wikipedia.org/wiki/Fluent_interface), meaning each
 method returns a new `Patch` instance.
@@ -138,36 +152,38 @@
 pa = dc.get_example_patch()
 
 # create a copy of patch with new data but coords and attrs stay the same
 new = pa.new(data=pa.data * 10)
 ```
 
 ## Update Attrs
+
 [`Patch.update_attrs`](`dascore.core.patch.Patch.update_attrs`) is for making small changes
 to the patch attrs (metadata) while keeping the unaffected metadata (`Patch.new` would require
 you replace the entirety of attrs).
 
 ```{python}
 import dascore as dc
 pa = dc.get_example_patch()
 
 # update existing attribute 'network' and create new attr 'new_attr'
-pa1 = pa.update_attrs(**{'network': 'experiment_1', 'new_attr': 42})
+pa1 = pa.update_attrs(**{'network': 'exp1', 'new_attr': 42})
 ```
 
 `Patch.update_attrs` also tries to keep the patch attributes consistent.
 For example, changing the start, end, or sampling of a dimension should
 update the other attributes affected by the change.
 
 ```{python}
 import dascore as dc
 pa = dc.get_example_patch()
 
 # update start time should also shift endtime
 pa1 = pa.update_attrs(time_min='2000-01-01')
+
 print(pa.attrs['time_min'])
 print(pa1.attrs['time_min'])
 ```
 
 # Method Chaining
 
 In most cases, you should use method chaining as part of a
```

### Comparing `dascore-0.0.8/docs/tutorial/spool.qmd` & `dascore-0.0.9/docs/tutorial/spool.qmd`

 * *Files 12% similar despite different names*

```diff
@@ -2,82 +2,85 @@
 title: Spool
 ---
 
 Spools are containers/managers of [patches](patch.qmd). Spools come in a few varieties which
 can manage a group of patches loaded into memory, archives of local files,
 and (in the future) a variety of clients for accessing remote resources.
 
+# Data Sources
+
 The simplest way to get the appropriate spool for a specified input is to use
 the `spool` function, which should work in the vast majority of cases.
 
+## Patches (in-memory)
 
 ```{python}
-#| echo: false
-
 import dascore as dc
 
-# create a list of patches
 patch_list = [dc.get_example_patch()]
 
-# get a spool for managing in-memory patches
 spool1 = dc.spool(patch_list)
+```
+
+## A Single File
 
-# get a spool from a das file
+```{python}
+import dascore as dc
 from dascore.utils.downloader import fetch
+
 path_to_das_file = fetch("terra15_das_1_trimmed.hdf5")
+
 spool2 = dc.spool(path_to_das_file)
+```
+
+## A Directory of DAS Files
+
+```{python}
+import dascore as dc
+from dascore.utils.downloader import fetch
 
-# get a spool from a directory of DAS files. The update
-# command is only needed the first time or if new files are added.
+path_to_das_file = fetch("terra15_das_1_trimmed.hdf5")
 directory_path = path_to_das_file.parent
+
 spool3 = dc.spool(directory_path).update()
 ```
 
 Despite some implementation differences, all spools have common behavior/methods.
 
 # Accessing patches
 
 Patches are extracted from the spool via simple iteration or indexing. New
 spools are returned via slicing.
 
 ```{python}
 import dascore as dc
+
 spool = dc.get_example_spool()
 
 patch = spool[0]  # extract first patch
 
 # iterate patchs
 for patch in spool:
     ...
 
 # slice spool to create new spool which excludes first patch.
 new_spool = spool[1:]
 ```
 
-
 # get_contents
 
 Returns a dataframe listing contents. This method may not be supported on all
 spools, especially those interfacing with vast remote resources.
 
 ```{python}
 #| output: false
 import dascore as dc
 spool = dc.get_example_spool()
 
 # Return dataframe with contents of spool (each row has metadata of a patch)
-print(spool.get_contents())
-```
-
-```{python}
-#| output: false
-import dascore as dc
-spool = dc.get_example_spool()
-
-# Return dataframe with contents of spool (each row has metadata of a patch)
 contents = spool.get_contents()
 print(contents)
 ```
 
 ```{python}
 #| echo: false
 from IPython.display import display
```

### Comparing `dascore-0.0.8/pyproject.toml` & `dascore-0.0.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -21,22 +21,23 @@
 dynamic = ["version"]  # version is fetched by setuptools-git-versioning
 
 authors = [
   { name="Derrick Chambers", email="chambers.ja.derrick@gmail.com" },
 ]
 
 description = "A python library distributed fiber optic sensing"
-readme = ".github/README.md"
-license = { file="LICENSE" }
+readme = "readme.md"
+license = { file="docs/LICENSE" }
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
 ]
 
 keywords = ["geophysics", "distributed-acoustic-sensing"]
 
 # --- Dependencies
 
@@ -45,23 +46,22 @@
      "matplotlib",
      "numpy",
      "packaging",
      "pandas",
      "pooch>=1.2",
      "pydantic>=1.9.0",
      "rich",
-     "scipy",
+     "scipy>=1.10.0",
      "tables",
      "typing_extensions",
      "xarray",
 ]
 
 [project.optional-dependencies]
 docs = [
-    "panflute",
     "jinja2",
 ]
 test = [
     "coverage",
     "coveralls",
     "pre-commit",
     "pytest",
```

### Comparing `dascore-0.0.8/readme.md` & `dascore-0.0.9/readme.md`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/scripts/_index_api.py` & `dascore-0.0.9/scripts/_index_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,17 +194,14 @@
     base_path = Path(_get_file_path(obj)).parent.parent
     data_dict = {}
     traverse(obj, data_dict, base_path)
     # traverse(obj, key, data_dict, str(base_path), parent_path=base_path)
     return data_dict
 
 
-# --- Rendering
-
-
 def get_alias_mapping(module, key=None):
     """Return a dict of {object_path: id} to construct cross refs."""
 
     def traverse_simple(obj, key, data_dict, base_path):
         """Traverse the tree and write out markdown."""
         obj = _unwrap_obj(obj)
         obj_id = str(id(obj))
```

### Comparing `dascore-0.0.8/scripts/_render_api.py` & `dascore-0.0.9/scripts/_render_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Create the html tables for parameters and such from dataframes.
 """
+import hashlib
 import inspect
 import json
 import os
-import shutil
 import typing
 from functools import cache
 from pathlib import Path
 
 import pandas as pd
 from jinja2 import Environment, FileSystemLoader
 
@@ -41,14 +41,22 @@
 def _simple_plural(text):
     """return plural form of string"""
     if text.endswith("s"):
         return text + "es"
     return text + "s"
 
 
+def sha_256(path_or_str: Path | str) -> str:
+    """Get the Sha256 hash of a file or a string."""
+    if isinstance(path_or_str, Path) and Path(path_or_str).exists():
+        with open(path_or_str) as fi:
+            path_or_str = fi.read()
+    return hashlib.sha256(str(path_or_str).encode('utf-8')).hexdigest()
+
+
 def build_table(df: pd.DataFrame, caption=None):
     """
     An opinionated function to make a dataframe into html table.
     """
     df = df.drop_duplicates()
     template = get_template("table.html")
     columns = [x.capitalize() for x in df.columns]
@@ -407,32 +415,40 @@
         main_key = data_dict[obj_id]["key"]
         out[alias] = out[main_key]
     return out
 
 
 def write_api_markdown(data_dict, api_path, address_dict, debug=False):
     """write all the markdown to disk."""
+    files_to_delete = set(Path(api_path).rglob('*.qmd'))
     for obj_id, data in data_dict.items():
         # get path and ensure parents exist
         sub_dir = api_path / "/".join(data["key"].split(".")[:-1])
         path = api_path / sub_dir / f"{data['name']}.qmd"
         path.parent.mkdir(exist_ok=True, parents=True)
+        # remove path from files to delete
+        if path in files_to_delete:
+            files_to_delete.remove(path)
         # dont render non-target file if debugging
         if debug and data['name'] != 'read':
             continue
         # render and write
         render = Render(data_dict, obj_id, address_dict)
         markdown = render.render_markdown()
+        # check if file has changed, if not don't write
+        if path.exists() and sha_256(path) == sha_256(markdown):
+            continue
         path.write_text(markdown)
+    # remove files that are no longer writen. This can happen when the code is
+    # refactored or objects are deleted.
+    for path in files_to_delete:
+        path.unlink()
 
 
 def render_project(data_dict, address_dict, api_path=API_DOC_PATH, debug=False):
     """Render the markdown files."""
-    # clear old contents from API directory
-    if api_path.exists() and api_path.is_dir():
-        shutil.rmtree(api_path)
-    # write each of the markdown files
+    # Create and write the qmd files for each function/class/module
     write_api_markdown(data_dict, api_path, address_dict, debug=debug)
     # dump the json mapping to disk in doc folder
     path_mapping = create_json_mapping(data_dict, address_dict, api_path)
     with open(Path(api_path) / "cross_ref.json", "w") as fi:
         json.dump(path_mapping, fi, indent=2)
```

### Comparing `dascore-0.0.8/tests/conftest.py` & `dascore-0.0.9/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 """
 pytest configuration for dascore
 """
+import os
 import shutil
 from pathlib import Path
 
+import matplotlib
 import numpy as np
 import pytest
 import tables as tb
+import tables.parameters
 
 import dascore as dc
 import dascore.examples as ex
 from dascore.clients.dirspool import DirectorySpool
 from dascore.constants import SpoolType
 from dascore.core import Patch
 from dascore.io.core import read
 from dascore.utils.downloader import fetch
 from dascore.utils.misc import register_func
 
 test_data_path = Path(__file__).parent.absolute() / "test_data"
 
 # A list to register functions that return general spools or patches
-# These are to be used for running many different patches/spools through
+# These are to be used for running many patches/spools through
 # Generic tests.
 SPOOL_FIXTURES = []
 PATCH_FIXTURES = []
 
 
 # --- Pytest configuration
 
@@ -72,19 +75,23 @@
     """
     Hook to run before any other tests.
 
     Used to ensure a non-visual backend is used so plots don't pop up
     and to set debug hook to True to avoid showing progress bars,
     except when explicitly being tested.
     """
-    import matplotlib
-
-    import dascore as dc
+    # If running in CI make sure to turn off matplotlib.
+    if os.environ.get("CI", False):
+        matplotlib.use("Agg")
 
+    # need to set nodes to 32 to avoid crash on p3.11. See pytables#977.
+    tables.parameters.NODE_CACHE_SLOTS = 32
     matplotlib.use("Agg")
+
+    # Ensure debug is set. This disables progress bars which disrupt debugging.
     dc._debug = True
 
 
 # --- Patch Paths
 
 
 @pytest.fixture(scope="session")
```

### Comparing `dascore-0.0.8/tests/test_clients/test_dirspool.py` & `dascore-0.0.9/tests/test_clients/test_dirspool.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         """An index should be returned."""
         bank_paths = list(Path(two_patch_directory).rglob("*hdf5"))
         assert isinstance(basic_index_df, pd.DataFrame)
         assert len(bank_paths) == len(basic_index_df)
 
     def test_index_columns(self, basic_index_df):
         """Ensure expected columns show up in the index."""
-        schema_fields = PatchFileSummary.__fields__
+        schema_fields = PatchFileSummary.get_index_columns()
         assert set(basic_index_df).issuperset(schema_fields)
 
     def test_patches_extracted(self, basic_file_spool):
         """Ensure the patches can be extracted."""
         index = basic_file_spool.get_contents()
         patches = [x for x in basic_file_spool]
         assert len(index) == len(patches)
@@ -73,14 +73,22 @@
 
     def test_str_(self, basic_file_spool):
         """Ensure the filespool has a useful str/repr."""
         out = str(basic_file_spool)
         # ensure the default str is not used.
         assert "object at" not in out
 
+    def test_long_tags(self, random_patch, tmp_path):
+        """Ensure a long tag still works."""
+        new = random_patch.update_attrs(tag="hey" * 15)
+        path = tmp_path / "test.h5"
+        new.io.write(path, "dasdae")
+        spool = dc.spool(path).update()
+        isinstance(spool, dc.BaseSpool)
+
 
 class TestSelect:
     """tests for subselecting data."""
 
     @pytest.fixture(scope="class")
     def spool_tag(self, basic_file_spool):
         """Return a string of a tag in the basic_file_spool."""
```

### Comparing `dascore-0.0.8/tests/test_clients/test_filespool.py` & `dascore-0.0.9/tests/test_clients/test_filespool.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/tests/test_core/test_patch.py` & `dascore-0.0.9/tests/test_core/test_patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,17 @@
         """Ensure the time_max is populated when not explicitly given."""
         end_time = random_patch.attrs["time_max"]
         assert not pd.isnull(end_time)
 
     def test_min_max_populated(self, random_patch):
         """The min/max values of the distance attrs should have been populated."""
         attrs = random_patch.attrs
-        expected_filled_in = [x for x in attrs if x.startswith("distance")]
+        expected_filled_in = [
+            x for x in list(attrs.__fields__) if x.startswith("distance")
+        ]
         for attr in expected_filled_in:
             assert not pd.isnull(attrs[attr])
 
     def test_dt_is_datetime64(self, random_patch):
         """Ensure dt gets changed into timedelta64."""
         d_time = random_patch.attrs["d_time"]
         assert isinstance(d_time, np.timedelta64)
@@ -110,16 +112,16 @@
         new = dascore.Patch(
             data=random_patch.data, attrs=attrs, coords=coords, dims=list(coords)
         )
         assert new.attrs["d_time"] == to_timedelta64(10)
 
     def test_had_default_attrs(self, patch):
         """Test that all patches used in the test suite have default attrs."""
-        attr_set = set(patch.attrs)
-        assert attr_set.issubset(set(patch.attrs))
+        attr_set = set(patch.attrs.dict())
+        assert attr_set.issubset(set(patch.attrs.dict()))
 
     def test_no_attrs(self):
         """Ensure a patch with no attrs can be created."""
         pa = Patch(
             data=np.random.random((100, 100)),
             coords={"time": np.random.random(100), "distance": np.random.random(100)},
             dims=("time", "distance"),
@@ -209,15 +211,15 @@
         assert not patch2.equals(random_patch)
 
     def test_one_null_value_in_attrs(self, random_patch):
         """
         Ensure setting a value to null in attrs doesn't eval to equal.
         """
         attrs = dict(random_patch.attrs)
-        attrs["tag"] = None
+        attrs["tag"] = ""
         patch2 = random_patch.new(attrs=attrs)
         patch2.equals(random_patch)
         assert not patch2.equals(random_patch)
 
     def test_extra_attrs(self, random_patch):
         """
         Ensure extra attrs in one patch still eval equal unless only_required
@@ -267,21 +269,21 @@
     Note: Most of the testing for this functionality is actually done on
     dascore.util.patch.AttrsCoordsMixer.
     """
 
     def test_add_attr(self, random_patch):
         """Tests for adding an attribute."""
         new = random_patch.update_attrs(bob=1)
-        assert "bob" in new.attrs and new.attrs["bob"] == 1
+        assert "bob" in new.attrs.dict() and new.attrs["bob"] == 1
 
     def test_original_unchanged(self, random_patch):
         """Updating attributes shouldn't change original patch in any way."""
         old_attrs = dict(random_patch.attrs)
         _ = random_patch.update_attrs(bob=2)
-        assert "bob" not in random_patch.attrs
+        assert "bob" not in dict(random_patch.attrs)
         assert random_patch.attrs == old_attrs
 
     def test_update_starttime(self, random_patch):
         """Ensure coords are updated with attrs."""
         t1 = np.datetime64("2000-01-01")
         pa = random_patch.update_attrs(time_min=t1)
         assert pa.attrs["time_min"] == t1
```

### Comparing `dascore-0.0.8/tests/test_core/test_spool.py` & `dascore-0.0.9/tests/test_core/test_spool.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/tests/test_io/test_dasdae/test_dasdae.py` & `dascore-0.0.9/tests/test_io/test_dasdae/test_dasdae.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 class TestScanDASDAE:
     """Tests for scanning the dasdae format."""
 
     def test_scan_returns_info(self, written_dascore_v1_random, random_patch):
         """Ensure scanning returns expected values."""
         info1 = dc.scan(written_dascore_v1_random)[0].dict()
         info2 = dict(random_patch.attrs)
-        common_keys = set(info1) & set(info2)
+        common_keys = set(info1) & set(info2) - {"history"}
         for key in common_keys:
             assert info1[key] == info2[key]
 
     def test_scan_format_version(self, written_dascore_v1_random):
         """Ensure scanning returns expected values."""
         formatter = DASDAEV1()
         df = dc.scan_to_df(written_dascore_v1_random)
```

### Comparing `dascore-0.0.8/tests/test_io/test_indexer.py` & `dascore-0.0.9/tests/test_io/test_indexer.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/tests/test_io/test_io_core.py` & `dascore-0.0.9/tests/test_io/test_io_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,17 +175,23 @@
         with pytest.raises(UnknownFiberFormat):
             _ = dascore.scan(dummy_file)
         out = dascore.scan(dummy_file, ignore=True)
         assert not len(out)
         assert out == []
 
     def test_scan_directory(self, tmp_path):
+        """Trying to scan an empty directory should return empty list."""
+        out = dascore.scan(tmp_path)
+        assert len(out) == 0
+
+    def test_scan_bad_files(self, tmp_path):
         """Trying to scan a directory should raise a nice error"""
-        with pytest.raises(InvalidFiberFile, match="a directory"):
-            _ = dascore.scan(tmp_path)
+        new = tmp_path / "myfile.txt"
+        with pytest.raises(InvalidFiberFile):
+            _ = dascore.scan(new)
 
     def test_scan_patch(self, random_patch):
         """Scan should also work on a patch"""
         out = dascore.scan_to_df(random_patch)
         attrs = random_patch.attrs
         assert len(out) == 1
         ser = out.iloc[0]
```

### Comparing `dascore-0.0.8/tests/test_io/test_pickle/test_pickle.py` & `dascore-0.0.9/tests/test_io/test_pickle/test_pickle.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/tests/test_io/test_tdms/test_tdms_v4713.py` & `dascore-0.0.9/tests/test_io/test_tdms/test_tdms_v4713.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,21 +51,21 @@
 
     def test_type(self, tdms_das_patch):
         """Ensure the expected type is returned."""
         assert isinstance(tdms_das_patch, dascore.Patch)
 
     def test_attributes(self, tdms_das_patch):
         """Ensure a few of the expected attrs exist in array."""
-        attrs = tdms_das_patch.attrs
+        attrs = dict(tdms_das_patch.attrs)
         expected_attrs = {"time_min", "time_max", "distance_min", "data_units"}
         assert set(expected_attrs).issubset(set(attrs))
 
     def test_has_required_attrs(self, tdms_das_patch):
         """ "Ensure the required das attrs are found"""
-        assert set(REQUIRED_DAS_ATTRS).issubset(set(tdms_das_patch.attrs))
+        assert set(REQUIRED_DAS_ATTRS).issubset(set(dict(tdms_das_patch.attrs)))
 
     def test_coord_attr_time_equal(self, tdms_das_patch):
         """The time reported in the attrs and coords should match"""
         attr_time = tdms_das_patch.attrs["time_max"]
         coord_time = tdms_das_patch.coords["time"].max()
         assert attr_time == coord_time
```

### Comparing `dascore-0.0.8/tests/test_io/test_terra15/test_terra15_v4.py` & `dascore-0.0.9/tests/test_io/test_terra15/test_terra15_v4.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 
     def test_type(self, terra15_das_patch):
         """Ensure the expected type is returned."""
         assert isinstance(terra15_das_patch, dascore.Patch)
 
     def test_attributes(self, terra15_das_patch):
         """Ensure a few of the expected attrs exist in array."""
-        attrs = terra15_das_patch.attrs
+        attrs = dict(terra15_das_patch.attrs)
         expected_attrs = {"time_min", "time_max", "distance_min", "data_units"}
         assert set(expected_attrs).issubset(set(attrs))
 
     def test_has_required_attrs(self, terra15_das_patch):
         """Ensure the required das attrs are found."""
-        assert set(REQUIRED_DAS_ATTRS).issubset(set(terra15_das_patch.attrs))
+        assert set(REQUIRED_DAS_ATTRS).issubset(set(dict(terra15_das_patch.attrs)))
 
     def test_coord_attr_time_equal(self, terra15_das_patch):
         """The time reported in the attrs and coords should match."""
         attr_time = terra15_das_patch.attrs["time_max"]
         coord_time = terra15_das_patch.coords["time"].max()
         assert attr_time == coord_time
```

### Comparing `dascore-0.0.8/tests/test_io/test_terra15/test_terra15_v5.py` & `dascore-0.0.9/tests/test_io/test_terra15/test_terra15_v5.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 
     def test_type(self, terra15_v5_patch):
         """Ensure the expected type is returned."""
         assert isinstance(terra15_v5_patch, dc.Patch)
 
     def test_attributes(self, terra15_v5_patch):
         """Ensure a few of the expected attrs exist in array."""
-        attrs = terra15_v5_patch.attrs
+        attrs = dict(terra15_v5_patch.attrs)
         expected_attrs = {"time_min", "time_max", "distance_min", "data_units"}
         assert set(expected_attrs).issubset(set(attrs))
 
     def test_has_required_attrs(self, terra15_v5_patch):
         """ "Ensure the required das attrs are found"""
-        assert set(REQUIRED_DAS_ATTRS).issubset(set(terra15_v5_patch.attrs))
+        assert set(REQUIRED_DAS_ATTRS).issubset(set(dict(terra15_v5_patch.attrs)))
 
     def test_coord_attr_time_equal(self, terra15_v5_patch):
         """The time reported in the attrs and coords should match"""
         attr_time = terra15_v5_patch.attrs["time_max"]
         coord_time = terra15_v5_patch.coords["time"].max()
         assert attr_time == coord_time
```

### Comparing `dascore-0.0.8/tests/test_io/test_wav/test_wav.py` & `dascore-0.0.9/tests/test_io/test_wav/test_wav.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/tests/test_proc/test_aggregate.py` & `dascore-0.0.9/tests/test_proc/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/tests/test_proc/test_resample.py` & `dascore-0.0.9/tests/test_proc/test_resample.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Tests for decimation
 """
 import numpy as np
+import pandas as pd
 import pytest
 
+import dascore as dc
 from dascore.exceptions import ParameterError
 from dascore.utils.patch import get_start_stop_step
 
 
 class TestInterpolate:
     """Tests for interpolating data along an axis in patch."""
 
@@ -86,14 +88,40 @@
         """
         Since decimate changes the spacing of dimension this should be updated.
         """
         dt1 = random_patch.attrs["d_time"]
         out = random_patch.decimate(time=10)
         assert out.attrs["d_time"] == dt1 * 10
 
+    def test_float_32_stability(self, random_patch):
+        """
+        Ensure float32 works for decimation.
+
+        See scipy#15072.
+        """
+        ar = np.random.random((10_000, 2)).astype("float32")
+        dt = dc.to_timedelta64(0.001)
+        t1 = dc.to_datetime64("2020-01-01")
+        coords = {
+            "distance": [1, 2],
+            "time": np.arange(0, ar.shape[0]) * dt + t1,
+        }
+        dims = ("time", "distance")
+        attrs = {"d_time": dt, "time_min": t1}
+        patch = dc.Patch(data=ar, coords=coords, dims=dims, attrs=attrs)
+        # ensure all modes of decimation don't produce NaN values.
+        decimated_iir = patch.decimate(time=10, filter_type="iir")
+        assert not np.any(pd.isnull(decimated_iir.data))
+
+        decimated_fir = patch.decimate(time=10, filter_type="fir")
+        assert not np.any(pd.isnull(decimated_fir.data))
+
+        decimated_none = patch.decimate(time=10, filter_type=None)
+        assert not np.any(pd.isnull(decimated_none.data))
+
 
 class TestResample:
     """
     Tests for resampling along a given dimension.
     """
 
     def test_downsample_time(self, random_patch):
```

### Comparing `dascore-0.0.8/tests/test_proc/test_select.py` & `dascore-0.0.9/tests/test_proc/test_select.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/tests/test_transform/test_fft_transforms.py` & `dascore-0.0.9/tests/test_transform/test_fft_transforms.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/tests/test_transform/test_spectro_transform.py` & `dascore-0.0.9/tests/test_transform/test_spectro_transform.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/tests/test_transform/test_velocity_to_strainrate.py` & `dascore-0.0.9/tests/test_transform/test_velocity_to_strainrate.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/tests/test_utils/test_chunk.py` & `dascore-0.0.9/tests/test_utils/test_chunk.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/tests/test_utils/test_coord_utils.py` & `dascore-0.0.9/tests/test_utils/test_coord_utils.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/tests/test_utils/test_doc_utils.py` & `dascore-0.0.9/tests/test_utils/test_doc_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Tests for docstring utils."""
 
 import textwrap
 
-from dascore.core.schema import PatchSummary
+from dascore.core.schema import PatchAttrs
 from dascore.utils.docs import compose_docstring, format_dtypes
 
 
 class TestFormatDtypes:
     """Tests for formatting datatypes to display in docstrings."""
 
     def test_formatting(self):
         """Test for formatting StationDtypes."""
-        out = format_dtypes(PatchSummary.__annotations__)
+        out = format_dtypes(PatchAttrs.__annotations__)
         assert isinstance(out, str)
 
 
 class TestDocsting:
     """tests for obsplus' simple docstring substitution function."""
 
     def count_white_space(self, some_str):
```

### Comparing `dascore-0.0.8/tests/test_utils/test_frozen_dict.py` & `dascore-0.0.9/tests/test_utils/test_frozen_dict.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/tests/test_utils/test_hdf_utils.py` & `dascore-0.0.9/tests/test_utils/test_hdf_utils.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/tests/test_utils/test_misc.py` & `dascore-0.0.9/tests/test_utils/test_misc.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 import os
 import time
 from pathlib import Path
 
 import numpy as np
 import pytest
 
-from dascore.exceptions import ParameterError
+from dascore.exceptions import MissingOptionalDependency, ParameterError
 from dascore.utils.misc import (
     MethodNameSpace,
     check_evenly_sampled,
     get_slice,
     iter_files,
     iterate,
+    optional_import,
 )
 
 
 class ParentClass:
     """A test parent class."""
 
     @property
@@ -249,7 +250,25 @@
     def test_object(self):
         """A single object should be returned in a tuple"""
         assert iterate(1) == (1,)
 
     def test_str(self):
         """A single string object should be returned as a tuple"""
         assert iterate("hey") == ("hey",)
+
+
+class TestOptionalImport:
+    """Ensure the optional import works."""
+
+    def test_import_installed_module(self):
+        """Test to ensure an installed module imports."""
+        import dascore as dc
+
+        mod = optional_import("dascore")
+        assert mod is dc
+        sub_mod = optional_import("dascore.core")
+        assert sub_mod is dc.core
+
+    def test_missing_module_raises(self):
+        """Ensure a module which is missing raises the appropriate Error."""
+        with pytest.raises(MissingOptionalDependency, match="boblib4"):
+            optional_import("boblib4")
```

### Comparing `dascore-0.0.8/tests/test_utils/test_patch_utils.py` & `dascore-0.0.9/tests/test_utils/test_patch_utils.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/tests/test_utils/test_pd.py` & `dascore-0.0.9/tests/test_utils/test_pd.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/tests/test_utils/test_time.py` & `dascore-0.0.9/tests/test_utils/test_time.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/tests/test_viz/test_spectrogram.py` & `dascore-0.0.9/tests/test_viz/test_spectrogram.py`

 * *Files identical despite different names*

### Comparing `dascore-0.0.8/tests/test_viz/test_waterfall.py` & `dascore-0.0.9/tests/test_viz/test_waterfall.py`

 * *Files identical despite different names*

