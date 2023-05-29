# Comparing `tmp/ocha-anticipy-1.0.1.tar.gz` & `tmp/ocha-anticipy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocha-anticipy-1.0.1.tar", last modified: Fri Feb  3 19:29:51 2023, max compression
+gzip compressed data, was "ocha-anticipy-1.0.2.tar", last modified: Mon May 29 11:23:47 2023, max compression
```

## Comparing `ocha-anticipy-1.0.1.tar` & `ocha-anticipy-1.0.2.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.769283 ocha-anticipy-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.757283 ocha-anticipy-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.761283 ocha-anticipy-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1535 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/.github/workflows/run-python-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1943 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      363 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     5034 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5371 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4133 2023-02-03 19:29:51.769283 ocha-anticipy-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3018 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.757283 ocha-anticipy-1.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.761283 ocha-anticipy-1.0.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     2394 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/docs/source/config.rst
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/docs/source/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.761283 ocha-anticipy-1.0.1/docs/source/datasources/
--rw-r--r--   0 runner    (1001) docker     (122)     4362 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/docs/source/datasources/chirps.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3861 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/docs/source/datasources/codab.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4187 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/docs/source/datasources/fewsnet.rst
--rw-r--r--   0 runner    (1001) docker     (122)    12584 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/docs/source/datasources/glofas.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3978 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/docs/source/datasources/iri_seasonal_forecast.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6354 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/docs/source/datasources/usgs_ndvi.rst
--rw-r--r--   0 runner    (1001) docker     (122)      504 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/docs/source/datasources.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/docs/source/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/docs/source/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/docs/source/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.761283 ocha-anticipy-1.0.1/docs/source/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/docs/source/utilities/raster.rst
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/docs/source/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.765283 ocha-anticipy-1.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (122)    16115 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1160 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/requirements/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (122)     7169 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/requirements/tests.in
--rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-02-03 19:29:51.769283 ocha-anticipy-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.757283 ocha-anticipy-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.765283 ocha-anticipy-1.0.1/src/ocha_anticipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4133 2023-02-03 19:29:51.000000 ocha-anticipy-1.0.1/src/ocha_anticipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3166 2023-02-03 19:29:51.000000 ocha-anticipy-1.0.1/src/ocha_anticipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-03 19:29:51.000000 ocha-anticipy-1.0.1/src/ocha_anticipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-02-03 19:29:51.000000 ocha-anticipy-1.0.1/src/ocha_anticipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-02-03 19:29:51.000000 ocha-anticipy-1.0.1/src/ocha_anticipy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.765283 ocha-anticipy-1.0.1/src/ochanticipy/
--rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-02-03 19:29:51.000000 ocha-anticipy-1.0.1/src/ochanticipy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.765283 ocha-anticipy-1.0.1/src/ochanticipy/config/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.765283 ocha-anticipy-1.0.1/src/ochanticipy/config/countries/
--rw-r--r--   0 runner    (1001) docker     (122)      823 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/config/countries/bfa.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/config/countries/bgd.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/config/countries/cod.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1566 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/config/countries/eth.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/config/countries/mwi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/config/countries/npl.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     7912 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/config/countryconfig.py
--rw-r--r--   0 runner    (1001) docker     (122)      503 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/config/pathconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.765283 ocha-anticipy-1.0.1/src/ochanticipy/datasources/
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/datasources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.765283 ocha-anticipy-1.0.1/src/ochanticipy/datasources/chirps/
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/datasources/chirps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19881 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/datasources/chirps/chirps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.765283 ocha-anticipy-1.0.1/src/ochanticipy/datasources/codab/
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/datasources/codab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6113 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/datasources/codab/codab.py
--rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/datasources/datasource.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.765283 ocha-anticipy-1.0.1/src/ochanticipy/datasources/fewsnet/
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/datasources/fewsnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13942 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/datasources/fewsnet/fewsnet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.765283 ocha-anticipy-1.0.1/src/ochanticipy/datasources/glofas/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/datasources/glofas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9852 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/datasources/glofas/forecast.py
--rw-r--r--   0 runner    (1001) docker     (122)    18347 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/datasources/glofas/glofas.py
--rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/datasources/glofas/reanalysis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.769283 ocha-anticipy-1.0.1/src/ochanticipy/datasources/iri/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/datasources/iri/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10406 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/datasources/iri/iri_seasonal_forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.769283 ocha-anticipy-1.0.1/src/ochanticipy/datasources/usgs/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/datasources/usgs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28079 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/datasources/usgs/ndvi_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    10009 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/datasources/usgs/ndvi_products.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.769283 ocha-anticipy-1.0.1/src/ochanticipy/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2321 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/utils/check_file_existence.py
--rw-r--r--   0 runner    (1001) docker     (122)     6071 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (122)     7202 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/utils/geoboundingbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     1874 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/utils/hdx_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1814 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (122)    25540 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/src/ochanticipy/utils/raster.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.769283 ocha-anticipy-1.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.769283 ocha-anticipy-1.0.1/tests/datasources/
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/tests/datasources/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      377 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/tests/datasources/fake_config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    14174 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/tests/datasources/test_chirps.py
--rw-r--r--   0 runner    (1001) docker     (122)     3631 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/tests/datasources/test_codab.py
--rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/tests/datasources/test_datasource.py
--rw-r--r--   0 runner    (1001) docker     (122)     7536 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/tests/datasources/test_fewsnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     3582 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/tests/datasources/test_glofas.py
--rw-r--r--   0 runner    (1001) docker     (122)     6255 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/tests/datasources/test_glofas_download.py
--rw-r--r--   0 runner    (1001) docker     (122)     9524 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/tests/datasources/test_glofas_process.py
--rw-r--r--   0 runner    (1001) docker     (122)     7158 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/tests/datasources/test_iri.py
--rw-r--r--   0 runner    (1001) docker     (122)     8883 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/tests/datasources/test_ndvi.py
--rw-r--r--   0 runner    (1001) docker     (122)     5252 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/tests/test_country_config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 19:29:51.769283 ocha-anticipy-1.0.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     1683 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/tests/utils/test_check_file_existence.py
--rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/tests/utils/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2915 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/tests/utils/test_geoboundingbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     1537 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/tests/utils/test_hdx_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     6621 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/tests/utils/test_raster.py
--rw-r--r--   0 runner    (1001) docker     (122)      394 2023-02-03 19:29:38.000000 ocha-anticipy-1.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.999639 ocha-anticipy-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.983638 ocha-anticipy-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.987638 ocha-anticipy-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1535 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1943 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     5246 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5371 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4133 2023-05-29 11:23:46.999639 ocha-anticipy-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3018 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.983638 ocha-anticipy-1.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.987638 ocha-anticipy-1.0.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     2394 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/config.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.991639 ocha-anticipy-1.0.2/docs/source/datasources/
+-rw-r--r--   0 runner    (1001) docker     (122)     4362 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/datasources/chirps.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3861 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/datasources/codab.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4187 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/datasources/fewsnet.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    12584 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/datasources/glofas.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3978 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/datasources/iri_seasonal_forecast.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6354 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/datasources/usgs_ndvi.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/datasources.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.991639 ocha-anticipy-1.0.2/docs/source/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/utilities/raster.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/docs/source/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.991639 ocha-anticipy-1.0.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (122)    16115 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1160 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/requirements/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     7169 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/requirements/tests.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-05-29 11:23:46.999639 ocha-anticipy-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.983638 ocha-anticipy-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.991639 ocha-anticipy-1.0.2/src/ocha_anticipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4133 2023-05-29 11:23:46.000000 ocha-anticipy-1.0.2/src/ocha_anticipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3166 2023-05-29 11:23:46.000000 ocha-anticipy-1.0.2/src/ocha_anticipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 11:23:46.000000 ocha-anticipy-1.0.2/src/ocha_anticipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-29 11:23:46.000000 ocha-anticipy-1.0.2/src/ocha_anticipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-29 11:23:46.000000 ocha-anticipy-1.0.2/src/ocha_anticipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.991639 ocha-anticipy-1.0.2/src/ochanticipy/
+-rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-29 11:23:46.000000 ocha-anticipy-1.0.2/src/ochanticipy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.991639 ocha-anticipy-1.0.2/src/ochanticipy/config/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.991639 ocha-anticipy-1.0.2/src/ochanticipy/config/countries/
+-rw-r--r--   0 runner    (1001) docker     (122)      823 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/config/countries/bfa.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/config/countries/bgd.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/config/countries/cod.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1566 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/config/countries/eth.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/config/countries/mwi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/config/countries/npl.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     7912 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/config/countryconfig.py
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/config/pathconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.991639 ocha-anticipy-1.0.2/src/ochanticipy/datasources/
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.991639 ocha-anticipy-1.0.2/src/ochanticipy/datasources/chirps/
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/chirps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19881 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/chirps/chirps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.991639 ocha-anticipy-1.0.2/src/ochanticipy/datasources/codab/
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/codab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6156 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/codab/codab.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/datasource.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.995638 ocha-anticipy-1.0.2/src/ochanticipy/datasources/fewsnet/
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/fewsnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13942 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/fewsnet/fewsnet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.995638 ocha-anticipy-1.0.2/src/ochanticipy/datasources/glofas/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/glofas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9852 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/glofas/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18347 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/glofas/glofas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/glofas/reanalysis.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.995638 ocha-anticipy-1.0.2/src/ochanticipy/datasources/iri/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/iri/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10406 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/iri/iri_seasonal_forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.995638 ocha-anticipy-1.0.2/src/ochanticipy/datasources/usgs/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/usgs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28079 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/usgs/ndvi_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10009 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/datasources/usgs/ndvi_products.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.995638 ocha-anticipy-1.0.2/src/ochanticipy/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2321 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/utils/check_file_existence.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6071 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7202 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/utils/geoboundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1874 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/utils/hdx_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1814 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25520 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/src/ochanticipy/utils/raster.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.995638 ocha-anticipy-1.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.995638 ocha-anticipy-1.0.2/tests/datasources/
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/datasources/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      377 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/datasources/fake_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    14174 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/datasources/test_chirps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3631 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/datasources/test_codab.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/datasources/test_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7536 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/datasources/test_fewsnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3582 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/datasources/test_glofas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6255 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/datasources/test_glofas_download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9524 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/datasources/test_glofas_process.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7158 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/datasources/test_iri.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8883 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/datasources/test_ndvi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5252 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/test_country_config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 11:23:46.999639 ocha-anticipy-1.0.2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     1683 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/utils/test_check_file_existence.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/utils/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2915 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/utils/test_geoboundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1537 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/utils/test_hdx_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6621 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tests/utils/test_raster.py
+-rw-r--r--   0 runner    (1001) docker     (122)      394 2023-05-29 11:23:32.000000 ocha-anticipy-1.0.2/tox.ini
```

### Comparing `ocha-anticipy-1.0.1/.github/workflows/publish-to-pypi.yaml` & `ocha-anticipy-1.0.2/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/.github/workflows/run-python-tests.yaml` & `ocha-anticipy-1.0.2/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/.gitignore` & `ocha-anticipy-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/.pre-commit-config.yaml` & `ocha-anticipy-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/CHANGELOG.rst` & `ocha-anticipy-1.0.2/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,30 @@
 All notable changes to OCHA AnticiPy will be documented in this file.
 
 The format is based on `Keep a
 Changelog <https://keepachangelog.com/en/1.0.0/>`__, and this project
 adheres to `Semantic
 Versioning <https://semver.org/spec/v2.0.0.html>`__.
 
+[1.0.2] - 2023-05-29
+--------------------
+
+Fixed
+~~~~~
+
+- Fixed bug for loading COD AB shapefiles in Windows
+- pandas ``Index`` used in raster module docstrings in lieu of
+  the now deprecated ``Int64Index``
+
 [1.0.1] - 2023-02-03
 --------------------
 
 Removed
 ~~~~~~~
+
 - ``sphinx-rtd-theme`` dependency for docs (switch to Alabaster theme)
 
 Fixed
 ~~~~~
 
 - Dropped support for Python 3.7 as it was dropped in dependencies
 - Fixed badge link in README.md and deprecated PyPI GHA
@@ -46,18 +57,20 @@
 ~~~~~~~
 
 - Documented and moved the raster processing module to the top level
   for public access
 
 Removed
 ~~~~~~~
+
 - Python 3.6 support
 
 Fixed
 ~~~~~
+
 - The check in ``DataSource`` for the required configuration file
   section now also checks if the section is ``None``
 - All available admin levels for DRC and Ethiopia are now accessible
 - IRI download method now checks request headers to verify authentication
 
 [0.4.2] - 2022-05-13
 --------------------
```

### Comparing `ocha-anticipy-1.0.1/CONTRIBUTING.rst` & `ocha-anticipy-1.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/LICENSE` & `ocha-anticipy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/PKG-INFO` & `ocha-anticipy-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocha-anticipy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Access data for anticipating humanitarian risk
 Home-page: https://github.com/OCHA-DAP/ocha-anticipy
 Author: Data Science Team, UN OCHA Centre for Humanitarian Data
 Author-email: centrehumdata@un.org
 License: GPLv3
 Project-URL: Documentation, https://ocha-anticipy.readthedocs.io/en/latest/
 Project-URL: Changes, https://github.com/OCHA-DAP/ocha-anticipy/blob/main/CHANGELOG.rst
```

### Comparing `ocha-anticipy-1.0.1/README.md` & `ocha-anticipy-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/docs/source/api.rst` & `ocha-anticipy-1.0.2/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/docs/source/conf.py` & `ocha-anticipy-1.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/docs/source/config.rst` & `ocha-anticipy-1.0.2/docs/source/config.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/docs/source/datasources/chirps.rst` & `ocha-anticipy-1.0.2/docs/source/datasources/chirps.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/docs/source/datasources/codab.rst` & `ocha-anticipy-1.0.2/docs/source/datasources/codab.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/docs/source/datasources/fewsnet.rst` & `ocha-anticipy-1.0.2/docs/source/datasources/fewsnet.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/docs/source/datasources/glofas.rst` & `ocha-anticipy-1.0.2/docs/source/datasources/glofas.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/docs/source/datasources/iri_seasonal_forecast.rst` & `ocha-anticipy-1.0.2/docs/source/datasources/iri_seasonal_forecast.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/docs/source/datasources/usgs_ndvi.rst` & `ocha-anticipy-1.0.2/docs/source/datasources/usgs_ndvi.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/docs/source/index.rst` & `ocha-anticipy-1.0.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/docs/source/introduction.rst` & `ocha-anticipy-1.0.2/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/docs/source/quickstart.rst` & `ocha-anticipy-1.0.2/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/docs/source/utilities/raster.rst` & `ocha-anticipy-1.0.2/docs/source/utilities/raster.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/requirements/requirements-dev.txt` & `ocha-anticipy-1.0.2/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/requirements/requirements-docs.txt` & `ocha-anticipy-1.0.2/requirements/requirements-docs.txt`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/requirements/requirements-tests.txt` & `ocha-anticipy-1.0.2/requirements/requirements-tests.txt`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/requirements/requirements.txt` & `ocha-anticipy-1.0.2/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/setup.cfg` & `ocha-anticipy-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ocha_anticipy.egg-info/PKG-INFO` & `ocha-anticipy-1.0.2/src/ocha_anticipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocha-anticipy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Access data for anticipating humanitarian risk
 Home-page: https://github.com/OCHA-DAP/ocha-anticipy
 Author: Data Science Team, UN OCHA Centre for Humanitarian Data
 Author-email: centrehumdata@un.org
 License: GPLv3
 Project-URL: Documentation, https://ocha-anticipy.readthedocs.io/en/latest/
 Project-URL: Changes, https://github.com/OCHA-DAP/ocha-anticipy/blob/main/CHANGELOG.rst
```

### Comparing `ocha-anticipy-1.0.1/src/ocha_anticipy.egg-info/SOURCES.txt` & `ocha-anticipy-1.0.2/src/ocha_anticipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/__init__.py` & `ocha-anticipy-1.0.2/src/ochanticipy/__init__.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/config/countries/bfa.yaml` & `ocha-anticipy-1.0.2/src/ochanticipy/config/countries/bfa.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/config/countries/bgd.yaml` & `ocha-anticipy-1.0.2/src/ochanticipy/config/countries/bgd.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/config/countries/cod.yaml` & `ocha-anticipy-1.0.2/src/ochanticipy/config/countries/cod.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/config/countries/eth.yaml` & `ocha-anticipy-1.0.2/src/ochanticipy/config/countries/eth.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/config/countries/mwi.yaml` & `ocha-anticipy-1.0.2/src/ochanticipy/config/countries/mwi.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/config/countries/npl.yaml` & `ocha-anticipy-1.0.2/src/ochanticipy/config/countries/npl.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/config/countryconfig.py` & `ocha-anticipy-1.0.2/src/ochanticipy/config/countryconfig.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/datasources/chirps/chirps.py` & `ocha-anticipy-1.0.2/src/ochanticipy/datasources/chirps/chirps.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/datasources/codab/codab.py` & `ocha-anticipy-1.0.2/src/ochanticipy/datasources/codab/codab.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,15 +155,17 @@
                 f"{custom_layer_number}th custom layer requested but not "
                 f"available in {self._country_config.iso3.upper()} config file"
             ) from err
         return self._load_admin_layer(layer_name=layer_name)
 
     def _load_admin_layer(self, layer_name: str) -> gpd.GeoDataFrame:
         try:
-            return gpd.read_file(f"zip://{self._raw_filepath / layer_name}")
+            return gpd.read_file(
+                f"zip://{(self._raw_filepath / layer_name).as_posix()}"
+            )
         except DriverError as err:
             raise FileNotFoundError(
                 f"Could not read boundary shapefile. Make sure that "
                 f"you have already called the 'download' method and "
                 f"that the file {self._raw_filepath} exists. If it does "
                 f"exist, please check the validity of the layer name: "
                 f"'{layer_name}'."
```

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/datasources/datasource.py` & `ocha-anticipy-1.0.2/src/ochanticipy/datasources/datasource.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/datasources/fewsnet/fewsnet.py` & `ocha-anticipy-1.0.2/src/ochanticipy/datasources/fewsnet/fewsnet.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/datasources/glofas/forecast.py` & `ocha-anticipy-1.0.2/src/ochanticipy/datasources/glofas/forecast.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/datasources/glofas/glofas.py` & `ocha-anticipy-1.0.2/src/ochanticipy/datasources/glofas/glofas.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/datasources/glofas/reanalysis.py` & `ocha-anticipy-1.0.2/src/ochanticipy/datasources/glofas/reanalysis.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/datasources/iri/iri_seasonal_forecast.py` & `ocha-anticipy-1.0.2/src/ochanticipy/datasources/iri/iri_seasonal_forecast.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/datasources/usgs/ndvi_base.py` & `ocha-anticipy-1.0.2/src/ochanticipy/datasources/usgs/ndvi_base.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/datasources/usgs/ndvi_products.py` & `ocha-anticipy-1.0.2/src/ochanticipy/datasources/usgs/ndvi_products.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/utils/check_file_existence.py` & `ocha-anticipy-1.0.2/src/ochanticipy/utils/check_file_existence.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/utils/dates.py` & `ocha-anticipy-1.0.2/src/ochanticipy/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/utils/geoboundingbox.py` & `ocha-anticipy-1.0.2/src/ochanticipy/utils/geoboundingbox.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/utils/hdx_api.py` & `ocha-anticipy-1.0.2/src/ochanticipy/utils/hdx_api.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/utils/io.py` & `ocha-anticipy-1.0.2/src/ochanticipy/utils/io.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/src/ochanticipy/utils/raster.py` & `ocha-anticipy-1.0.2/src/ochanticipy/utils/raster.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,17 +254,17 @@
         >>> da = xarray.DataArray(
         ...  numpy.arange(16).reshape(4,4),
         ...  coords={"lat":numpy.array([87, 88, 89, 90]),
         ...          "lon":numpy.array([70, 69, 68, 67])}
         ... )
         >>> da.oap.invert_coordinates(inplace=True)
         >>> da.get_index("lon")
-        Int64Index([67, 68, 69, 70], dtype='int64', name='lon')
+        Index([67, 68, 69, 70], dtype='int64', name='lon')
         >>> da.get_index("lat")
-        Int64Index([90, 89, 88, 87], dtype='int64', name='lat')
+        Index([90, 89, 88, 87], dtype='int64', name='lat')
         """
         data_obj = self._get_obj_oap(inplace=inplace)
         lon_inv, lat_inv = self._check_coords_inverted()
 
         if lon_inv:
             logger.info("Longitude was inverted, reversing coordinates.")
             data_obj[self.x_dim] = data_obj[self.x_dim][::-1]
@@ -342,19 +342,19 @@
         ...     "lat":numpy.array([87, 88, 89, 90]),
         ...     "lon":numpy.array([5, 120, 199, 360]),
         ...     "time": pandas.date_range("2014-09-06", periods=3)
         ...   }
         ... )
         >>> ds_inv = ds.oap.change_longitude_range()
         >>> ds_inv.get_index("lon")
-        Int64Index([-161, 0, 5, 120], dtype='int64', name='lon')
+        Index([-161, 0, 5, 120], dtype='int64', name='lon')
         >>> # invert coordinates back to original, in place
         >>> ds_inv.oap.change_longitude_range(to_180_range=False, inplace=True)
         >>> ds_inv.get_index("lon")
-        Int64Index([0, 5, 120, 199], dtype='int64', name='lon')
+        Index([0, 5, 120, 199], dtype='int64', name='lon')
         """
         data_obj = self._get_obj_oap(inplace=inplace)
 
         if to_180_range and self.longitude_range == "360":
             logger.info("Converting longitude from 0 360 to -180 to 180.")
 
             data_obj[self.x_dim] = np.sort(
```

### Comparing `ocha-anticipy-1.0.1/tests/datasources/conftest.py` & `ocha-anticipy-1.0.2/tests/datasources/conftest.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/tests/datasources/test_chirps.py` & `ocha-anticipy-1.0.2/tests/datasources/test_chirps.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/tests/datasources/test_codab.py` & `ocha-anticipy-1.0.2/tests/datasources/test_codab.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/tests/datasources/test_datasource.py` & `ocha-anticipy-1.0.2/tests/datasources/test_datasource.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/tests/datasources/test_fewsnet.py` & `ocha-anticipy-1.0.2/tests/datasources/test_fewsnet.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/tests/datasources/test_glofas.py` & `ocha-anticipy-1.0.2/tests/datasources/test_glofas.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/tests/datasources/test_glofas_download.py` & `ocha-anticipy-1.0.2/tests/datasources/test_glofas_download.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/tests/datasources/test_glofas_process.py` & `ocha-anticipy-1.0.2/tests/datasources/test_glofas_process.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/tests/datasources/test_iri.py` & `ocha-anticipy-1.0.2/tests/datasources/test_iri.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/tests/datasources/test_ndvi.py` & `ocha-anticipy-1.0.2/tests/datasources/test_ndvi.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/tests/test_country_config.py` & `ocha-anticipy-1.0.2/tests/test_country_config.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/tests/utils/test_check_file_existence.py` & `ocha-anticipy-1.0.2/tests/utils/test_check_file_existence.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/tests/utils/test_dates.py` & `ocha-anticipy-1.0.2/tests/utils/test_dates.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/tests/utils/test_geoboundingbox.py` & `ocha-anticipy-1.0.2/tests/utils/test_geoboundingbox.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/tests/utils/test_hdx_api.py` & `ocha-anticipy-1.0.2/tests/utils/test_hdx_api.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.0.1/tests/utils/test_raster.py` & `ocha-anticipy-1.0.2/tests/utils/test_raster.py`

 * *Files identical despite different names*

