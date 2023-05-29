# Comparing `tmp/intake-xarray-0.6.1.tar.gz` & `tmp/intake-xarray-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intake-xarray-0.6.1.tar", last modified: Fri Aug 26 19:25:45 2022, max compression
+gzip compressed data, was "intake-xarray-0.7.0.tar", last modified: Mon May 29 20:06:36 2023, max compression
```

## Comparing `intake-xarray-0.6.1.tar` & `intake-xarray-0.7.0.tar`

### file list

```diff
@@ -1,137 +1,47 @@
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.185757 intake-xarray-0.6.1/
--rw-r--r--   0 mdurant    (502) staff       (20)     3695 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/.ciocheck
--rw-r--r--   0 mdurant    (502) staff       (20)       39 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/.gitattributes
--rw-r--r--   0 mdurant    (502) staff       (20)       84 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/.gitignore
--rw-r--r--   0 mdurant    (502) staff       (20)     1330 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/LICENSE
--rw-r--r--   0 mdurant    (502) staff       (20)      152 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/MANIFEST.in
--rw-r--r--   0 mdurant    (502) staff       (20)     1346 2022-08-26 19:25:45.185861 intake-xarray-0.6.1/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)     1037 2021-03-17 15:06:01.000000 intake-xarray-0.6.1/README.md
--rw-r--r--   0 mdurant    (502) staff       (20)      680 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/appveyor.yml
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.117296 intake-xarray-0.6.1/ci/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.122247 intake-xarray-0.6.1/ci/appveyor/
--rw-r--r--   0 mdurant    (502) staff       (20)      192 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/ci/appveyor/build.ps1
--rw-r--r--   0 mdurant    (502) staff       (20)      145 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/ci/appveyor/install.ps1
--rw-r--r--   0 mdurant    (502) staff       (20)      185 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/ci/appveyor/test.ps1
--rw-r--r--   0 mdurant    (502) staff       (20)      324 2022-07-28 18:24:56.000000 intake-xarray-0.6.1/ci/environment-py310.yml
--rw-r--r--   0 mdurant    (502) staff       (20)      323 2022-07-28 18:24:56.000000 intake-xarray-0.6.1/ci/environment-py38.yml
--rw-r--r--   0 mdurant    (502) staff       (20)      323 2022-07-28 18:24:56.000000 intake-xarray-0.6.1/ci/environment-py39.yml
--rw-r--r--   0 mdurant    (502) staff       (20)      504 2022-07-28 18:24:56.000000 intake-xarray-0.6.1/ci/environment-upstream.yml
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.122877 intake-xarray-0.6.1/ci/travis/
--rw-r--r--   0 mdurant    (502) staff       (20)      171 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/ci/travis/install.sh
--rwxr-xr-x   0 mdurant    (502) staff       (20)      414 2020-08-18 17:23:06.000000 intake-xarray-0.6.1/ci/travis/test.sh
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.123376 intake-xarray-0.6.1/conda/
--rw-r--r--   0 mdurant    (502) staff       (20)      669 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/conda/meta.yaml
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.124794 intake-xarray-0.6.1/docs/
--rw-r--r--   0 mdurant    (502) staff       (20)      615 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/docs/Makefile
--rw-r--r--   0 mdurant    (502) staff       (20)      262 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/docs/README.md
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.104754 intake-xarray-0.6.1/docs/build/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.119467 intake-xarray-0.6.1/docs/build/html/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.120076 intake-xarray-0.6.1/docs/build/html/_modules/
--rwxrwxrwx   0 mdurant    (502) staff       (20)     4578 2020-04-14 14:06:00.000000 intake-xarray-0.6.1/docs/build/html/_modules/index.html
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.121091 intake-xarray-0.6.1/docs/build/html/_modules/intake_xarray/
--rwxrwxrwx   0 mdurant    (502) staff       (20)     9007 2020-04-14 14:06:00.000000 intake-xarray-0.6.1/docs/build/html/_modules/intake_xarray/netcdf.html
--rwxrwxrwx   0 mdurant    (502) staff       (20)    12728 2020-04-14 14:06:00.000000 intake-xarray-0.6.1/docs/build/html/_modules/intake_xarray/xzarr.html
--rwxrwxrwx   0 mdurant    (502) staff       (20)    17630 2020-04-14 14:06:00.000000 intake-xarray-0.6.1/docs/build/html/_modules/intake_xarray.html
--rwxrwxrwx   0 mdurant    (502) staff       (20)    17788 2020-04-14 14:06:00.000000 intake-xarray-0.6.1/docs/build/html/api.html
--rwxrwxrwx   0 mdurant    (502) staff       (20)     6030 2020-04-14 14:06:00.000000 intake-xarray-0.6.1/docs/build/html/genindex.html
--rwxrwxrwx   0 mdurant    (502) staff       (20)     6049 2020-04-14 14:06:00.000000 intake-xarray-0.6.1/docs/build/html/index.html
--rwxrwxrwx   0 mdurant    (502) staff       (20)     8289 2020-04-14 14:05:59.000000 intake-xarray-0.6.1/docs/build/html/quickstart.html
--rwxrwxrwx   0 mdurant    (502) staff       (20)     4689 2020-04-14 14:06:00.000000 intake-xarray-0.6.1/docs/build/html/search.html
--rw-r--r--   0 mdurant    (502) staff       (20)      165 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/docs/environment.yml
--rw-r--r--   0 mdurant    (502) staff       (20)      783 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/docs/make.bat
--rw-r--r--   0 mdurant    (502) staff       (20)       34 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/docs/requirements.txt
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.126452 intake-xarray-0.6.1/docs/source/
--rw-r--r--   0 mdurant    (502) staff       (20)      544 2020-12-29 15:55:01.000000 intake-xarray-0.6.1/docs/source/api.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     5245 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/docs/source/conf.py
--rw-r--r--   0 mdurant    (502) staff       (20)      417 2020-12-29 15:55:01.000000 intake-xarray-0.6.1/docs/source/index.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     2505 2022-07-24 20:18:06.000000 intake-xarray-0.6.1/docs/source/quickstart.rst
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.127456 intake-xarray-0.6.1/examples/
--rw-r--r--   0 mdurant    (502) staff       (20)     6172 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/examples/OPeNDAP.ipynb
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/examples/README.md
--rw-r--r--   0 mdurant    (502) staff       (20)     3090 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/examples/catalog.yml
--rw-r--r--   0 mdurant    (502) staff       (20)     6760 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/examples/intake_xarray.ipynb
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.186452 intake-xarray-0.6.1/intake_xarray/
--rw-r--r--   0 mdurant    (502) staff       (20)      564 2022-07-24 20:18:06.000000 intake-xarray-0.6.1/intake_xarray/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)      497 2022-08-26 19:25:45.186507 intake-xarray-0.6.1/intake_xarray/_version.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2392 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/base.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1844 2022-07-24 20:18:06.000000 intake-xarray-0.6.1/intake_xarray/derived.py
--rw-r--r--   0 mdurant    (502) staff       (20)    17900 2022-07-24 20:18:06.000000 intake-xarray-0.6.1/intake_xarray/image.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4265 2022-07-24 20:18:06.000000 intake-xarray-0.6.1/intake_xarray/netcdf.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3656 2022-07-28 18:24:56.000000 intake-xarray-0.6.1/intake_xarray/opendap.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5114 2022-07-24 20:15:46.000000 intake-xarray-0.6.1/intake_xarray/raster.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.160209 intake-xarray-0.6.1/intake_xarray/tests/
--rw-r--r--   0 mdurant    (502) staff       (20)       24 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)      961 2020-12-29 15:54:38.000000 intake-xarray-0.6.1/intake_xarray/tests/conftest.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.170612 intake-xarray-0.6.1/intake_xarray/tests/data/
--rw-r--r--   0 mdurant    (502) staff       (20)  1743350 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/RGB.byte.tif
--rw-r--r--   0 mdurant    (502) staff       (20)     1184 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/bears.nc
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.172967 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/
--rw-r--r--   0 mdurant    (502) staff       (20)       42 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/.zattrs
--rw-r--r--   0 mdurant    (502) staff       (20)       24 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/.zgroup
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.174040 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/lat/
--rw-r--r--   0 mdurant    (502) staff       (20)      312 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/lat/.zarray
--rw-r--r--   0 mdurant    (502) staff       (20)       80 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/lat/.zattrs
--rw-r--r--   0 mdurant    (502) staff       (20)       36 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/lat/0
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.175110 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/level/
--rw-r--r--   0 mdurant    (502) staff       (20)      312 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/level/.zarray
--rw-r--r--   0 mdurant    (502) staff       (20)       78 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/level/.zattrs
--rw-r--r--   0 mdurant    (502) staff       (20)       32 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/level/0
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.176303 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/lon/
--rw-r--r--   0 mdurant    (502) staff       (20)      314 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/lon/.zarray
--rw-r--r--   0 mdurant    (502) staff       (20)       79 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/lon/.zattrs
--rw-r--r--   0 mdurant    (502) staff       (20)       56 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/lon/0
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.178510 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/rh/
--rw-r--r--   0 mdurant    (502) staff       (20)      358 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/rh/.zarray
--rw-r--r--   0 mdurant    (502) staff       (20)      172 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/rh/.zattrs
--rw-r--r--   0 mdurant    (502) staff       (20)       56 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/rh/0.0.0
--rw-r--r--   0 mdurant    (502) staff       (20)       56 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/rh/0.0.1
--rw-r--r--   0 mdurant    (502) staff       (20)       56 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/rh/0.0.2
--rw-r--r--   0 mdurant    (502) staff       (20)       56 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/rh/0.0.3
--rw-r--r--   0 mdurant    (502) staff       (20)       56 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/rh/0.0.4
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.181343 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/temp/
--rw-r--r--   0 mdurant    (502) staff       (20)      380 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/temp/.zarray
--rw-r--r--   0 mdurant    (502) staff       (20)      154 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/temp/.zattrs
--rw-r--r--   0 mdurant    (502) staff       (20)       45 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/temp/0.0.0.0
--rw-r--r--   0 mdurant    (502) staff       (20)       45 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/temp/0.0.0.1
--rw-r--r--   0 mdurant    (502) staff       (20)       45 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/temp/0.0.0.2
--rw-r--r--   0 mdurant    (502) staff       (20)       45 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/temp/0.0.0.3
--rw-r--r--   0 mdurant    (502) staff       (20)       45 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/temp/0.0.0.4
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.182279 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/time/
--rw-r--r--   0 mdurant    (502) staff       (20)      312 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/time/.zarray
--rw-r--r--   0 mdurant    (502) staff       (20)      129 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/time/.zattrs
--rw-r--r--   0 mdurant    (502) staff       (20)       18 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/blank.zarr/time/0
--rw-r--r--   0 mdurant    (502) staff       (20)     3737 2022-07-24 20:18:06.000000 intake-xarray-0.6.1/intake_xarray/tests/data/catalog.yaml
--rw-r--r--   0 mdurant    (502) staff       (20)    12806 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/color_with_special_2.tif
--rw-r--r--   0 mdurant    (502) staff       (20)    12806 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/color_with_special{}.tif
--rw-r--r--   0 mdurant    (502) staff       (20)    11710 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/dog.jpg
--rw-r--r--   0 mdurant    (502) staff       (20)     1736 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/example_1.nc
--rw-r--r--   0 mdurant    (502) staff       (20)     1736 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/example_2.nc
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.184855 intake-xarray-0.6.1/intake_xarray/tests/data/images/
--rw-r--r--   0 mdurant    (502) staff       (20)   208660 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/images/beach01.tif
--rw-r--r--   0 mdurant    (502) staff       (20)   203116 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/images/beach57.tif
--rw-r--r--   0 mdurant    (502) staff       (20)   196280 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/images/buildings96.tif
--rw-r--r--   0 mdurant    (502) staff       (20)    12806 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/little_green.tif
--rw-r--r--   0 mdurant    (502) staff       (20)    12806 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/little_red.tif
--rw-r--r--   0 mdurant    (502) staff       (20)   340748 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/wafsgfs_L_t06z_intdsk60.grib2
--rw-r--r--   0 mdurant    (502) staff       (20)   340748 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/data/wafsgfs_L_t06z_intdsk61.grib2
--rw-r--r--   0 mdurant    (502) staff       (20)      903 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/intake_xarray/tests/test_catalog.py
--rw-r--r--   0 mdurant    (502) staff       (20)      614 2022-07-24 20:18:06.000000 intake-xarray-0.6.1/intake_xarray/tests/test_derived.py
--rw-r--r--   0 mdurant    (502) staff       (20)     6035 2022-07-24 20:18:06.000000 intake-xarray-0.6.1/intake_xarray/tests/test_image.py
--rw-r--r--   0 mdurant    (502) staff       (20)    13200 2022-07-28 18:24:56.000000 intake-xarray-0.6.1/intake_xarray/tests/test_intake_xarray.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3332 2022-07-24 20:18:06.000000 intake-xarray-0.6.1/intake_xarray/tests/test_network.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10115 2022-07-28 18:24:56.000000 intake-xarray-0.6.1/intake_xarray/tests/test_remote.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5876 2022-07-24 20:18:06.000000 intake-xarray-0.6.1/intake_xarray/xarray_container.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1845 2022-07-24 20:18:06.000000 intake-xarray-0.6.1/intake_xarray/xzarr.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2022-08-26 19:25:45.156239 intake-xarray-0.6.1/intake_xarray.egg-info/
--rwxrwxrwx   0 mdurant    (502) staff       (20)     1346 2022-08-26 19:25:44.000000 intake-xarray-0.6.1/intake_xarray.egg-info/PKG-INFO
--rwxrwxrwx   0 mdurant    (502) staff       (20)     3830 2022-08-26 19:25:44.000000 intake-xarray-0.6.1/intake_xarray.egg-info/SOURCES.txt
--rwxrwxrwx   0 mdurant    (502) staff       (20)        1 2022-08-26 19:25:44.000000 intake-xarray-0.6.1/intake_xarray.egg-info/dependency_links.txt
--rwxrwxrwx   0 mdurant    (502) staff       (20)      298 2022-08-26 19:25:44.000000 intake-xarray-0.6.1/intake_xarray.egg-info/entry_points.txt
--rwxrwxrwx   0 mdurant    (502) staff       (20)        1 2020-04-14 14:05:59.000000 intake-xarray-0.6.1/intake_xarray.egg-info/not-zip-safe
--rwxrwxrwx   0 mdurant    (502) staff       (20)       46 2020-04-14 14:05:59.000000 intake-xarray-0.6.1/intake_xarray.egg-info/pbr.json
--rwxrwxrwx   0 mdurant    (502) staff       (20)       80 2022-08-26 19:25:44.000000 intake-xarray-0.6.1/intake_xarray.egg-info/requires.txt
--rwxrwxrwx   0 mdurant    (502) staff       (20)       14 2022-08-26 19:25:44.000000 intake-xarray-0.6.1/intake_xarray.egg-info/top_level.txt
--rw-r--r--   0 mdurant    (502) staff       (20)       38 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/readthedocs.yml
--rw-r--r--   0 mdurant    (502) staff       (20)      184 2022-08-26 19:25:45.186231 intake-xarray-0.6.1/setup.cfg
--rw-r--r--   0 mdurant    (502) staff       (20)     1610 2022-08-26 19:25:00.000000 intake-xarray-0.6.1/setup.py
--rw-r--r--   0 mdurant    (502) staff       (20)    68522 2020-04-21 12:54:39.000000 intake-xarray-0.6.1/versioneer.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:06:36.281659 intake-xarray-0.7.0/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1330 2022-09-18 01:28:53.000000 intake-xarray-0.7.0/LICENSE
+-rw-r--r--   0 mdurant    (502) staff       (20)      152 2022-09-18 01:28:53.000000 intake-xarray-0.7.0/MANIFEST.in
+-rw-r--r--   0 mdurant    (502) staff       (20)     1321 2023-05-29 20:06:36.281743 intake-xarray-0.7.0/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     1037 2022-09-18 01:28:53.000000 intake-xarray-0.7.0/README.md
+-rw-r--r--   0 mdurant    (502) staff       (20)      680 2022-09-18 01:28:53.000000 intake-xarray-0.7.0/appveyor.yml
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:06:36.274560 intake-xarray-0.7.0/ci/
+-rw-r--r--   0 mdurant    (502) staff       (20)      338 2023-05-09 20:11:36.000000 intake-xarray-0.7.0/ci/environment-py310.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)      337 2023-05-09 20:11:36.000000 intake-xarray-0.7.0/ci/environment-py38.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)      337 2023-05-09 20:11:36.000000 intake-xarray-0.7.0/ci/environment-py39.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)      518 2023-05-09 20:11:36.000000 intake-xarray-0.7.0/ci/environment-upstream.yml
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:06:36.274762 intake-xarray-0.7.0/docs/
+-rw-r--r--   0 mdurant    (502) staff       (20)      165 2022-09-18 01:28:53.000000 intake-xarray-0.7.0/docs/environment.yml
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:06:36.275120 intake-xarray-0.7.0/examples/
+-rw-r--r--   0 mdurant    (502) staff       (20)     3090 2022-09-18 01:28:53.000000 intake-xarray-0.7.0/examples/catalog.yml
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:06:36.282362 intake-xarray-0.7.0/intake_xarray/
+-rw-r--r--   0 mdurant    (502) staff       (20)      564 2022-09-18 01:28:53.000000 intake-xarray-0.7.0/intake_xarray/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      497 2023-05-29 20:06:36.282416 intake-xarray-0.7.0/intake_xarray/_version.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2392 2022-09-18 01:28:53.000000 intake-xarray-0.7.0/intake_xarray/base.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1844 2022-09-18 01:28:53.000000 intake-xarray-0.7.0/intake_xarray/derived.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    17900 2022-09-18 01:28:53.000000 intake-xarray-0.7.0/intake_xarray/image.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4265 2022-09-18 01:28:53.000000 intake-xarray-0.7.0/intake_xarray/netcdf.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3656 2022-09-18 01:28:53.000000 intake-xarray-0.7.0/intake_xarray/opendap.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     5169 2023-05-09 20:11:36.000000 intake-xarray-0.7.0/intake_xarray/raster.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:06:36.281478 intake-xarray-0.7.0/intake_xarray/tests/
+-rw-r--r--   0 mdurant    (502) staff       (20)       24 2022-09-18 01:28:53.000000 intake-xarray-0.7.0/intake_xarray/tests/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      961 2022-09-18 01:28:53.000000 intake-xarray-0.7.0/intake_xarray/tests/conftest.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      903 2023-05-09 20:08:00.000000 intake-xarray-0.7.0/intake_xarray/tests/test_catalog.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      614 2022-09-18 01:28:53.000000 intake-xarray-0.7.0/intake_xarray/tests/test_derived.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     6034 2023-05-09 20:11:36.000000 intake-xarray-0.7.0/intake_xarray/tests/test_image.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    13200 2022-09-18 01:28:53.000000 intake-xarray-0.7.0/intake_xarray/tests/test_intake_xarray.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3293 2023-05-09 20:11:36.000000 intake-xarray-0.7.0/intake_xarray/tests/test_network.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    10269 2023-05-09 20:11:36.000000 intake-xarray-0.7.0/intake_xarray/tests/test_remote.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     5987 2023-05-09 20:11:36.000000 intake-xarray-0.7.0/intake_xarray/xarray_container.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1845 2022-09-18 01:28:53.000000 intake-xarray-0.7.0/intake_xarray/xzarr.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:06:36.279301 intake-xarray-0.7.0/intake_xarray.egg-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1321 2023-05-29 20:06:36.000000 intake-xarray-0.7.0/intake_xarray.egg-info/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     1045 2023-05-29 20:06:36.000000 intake-xarray-0.7.0/intake_xarray.egg-info/SOURCES.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-05-29 20:06:36.000000 intake-xarray-0.7.0/intake_xarray.egg-info/dependency_links.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      298 2023-05-29 20:06:36.000000 intake-xarray-0.7.0/intake_xarray.egg-info/entry_points.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-10-27 18:28:43.000000 intake-xarray-0.7.0/intake_xarray.egg-info/not-zip-safe
+-rw-r--r--   0 mdurant    (502) staff       (20)       80 2023-05-29 20:06:36.000000 intake-xarray-0.7.0/intake_xarray.egg-info/requires.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)       14 2023-05-29 20:06:36.000000 intake-xarray-0.7.0/intake_xarray.egg-info/top_level.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)       38 2022-09-18 01:28:53.000000 intake-xarray-0.7.0/readthedocs.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)      184 2023-05-29 20:06:36.282148 intake-xarray-0.7.0/setup.cfg
+-rw-r--r--   0 mdurant    (502) staff       (20)     1605 2022-12-19 14:22:55.000000 intake-xarray-0.7.0/setup.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    68522 2022-09-18 01:28:53.000000 intake-xarray-0.7.0/versioneer.py
```

### Comparing `intake-xarray-0.6.1/LICENSE` & `intake-xarray-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `intake-xarray-0.6.1/PKG-INFO` & `intake-xarray-0.7.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: intake-xarray
-Version: 0.6.1
-Summary: xarray plugins for Intake
-Home-page: https://github.com/ContinuumIO/intake-xarray
-Maintainer: Martin Durant
-Maintainer-email: mdurant@anaconda.com
-License: BSD
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # intake-xarray
 
 ![CI](https://github.com/intake/intake-xarray/workflows/CI/badge.svg)
 
 Intake-xarray: xarray Plugin for [Intake](https://github.com/intake/intake)
 
 See [Intake docs](https://intake.readthedocs.io/en/latest/overview.html) for a general introduction and usage
@@ -40,9 +28,7 @@
 ```
 
 To install optional dependencies:
 
 ```
 conda install -c conda-forge pydap rasterio
 ```
-
-
```

### Comparing `intake-xarray-0.6.1/README.md` & `intake-xarray-0.7.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: intake-xarray
+Version: 0.7.0
+Summary: xarray plugins for Intake
+Home-page: https://github.com/intake/intake-xarray
+Maintainer: Martin Durant
+Maintainer-email: mdurant@anaconda.com
+License: BSD
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # intake-xarray
 
 ![CI](https://github.com/intake/intake-xarray/workflows/CI/badge.svg)
 
 Intake-xarray: xarray Plugin for [Intake](https://github.com/intake/intake)
 
 See [Intake docs](https://intake.readthedocs.io/en/latest/overview.html) for a general introduction and usage
```

### Comparing `intake-xarray-0.6.1/appveyor.yml` & `intake-xarray-0.7.0/appveyor.yml`

 * *Files identical despite different names*

### Comparing `intake-xarray-0.6.1/examples/catalog.yml` & `intake-xarray-0.7.0/examples/catalog.yml`

 * *Files identical despite different names*

### Comparing `intake-xarray-0.6.1/intake_xarray/__init__.py` & `intake-xarray-0.7.0/intake_xarray/__init__.py`

 * *Files identical despite different names*

### Comparing `intake-xarray-0.6.1/intake_xarray/base.py` & `intake-xarray-0.7.0/intake_xarray/base.py`

 * *Files identical despite different names*

### Comparing `intake-xarray-0.6.1/intake_xarray/derived.py` & `intake-xarray-0.7.0/intake_xarray/derived.py`

 * *Files identical despite different names*

### Comparing `intake-xarray-0.6.1/intake_xarray/image.py` & `intake-xarray-0.7.0/intake_xarray/image.py`

 * *Files identical despite different names*

### Comparing `intake-xarray-0.6.1/intake_xarray/netcdf.py` & `intake-xarray-0.7.0/intake_xarray/netcdf.py`

 * *Files identical despite different names*

### Comparing `intake-xarray-0.6.1/intake_xarray/opendap.py` & `intake-xarray-0.7.0/intake_xarray/opendap.py`

 * *Files identical despite different names*

### Comparing `intake-xarray-0.6.1/intake_xarray/raster.py` & `intake-xarray-0.7.0/intake_xarray/raster.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import numpy as np
 import fsspec
 from intake.source.base import PatternMixin
 from intake.source.utils import reverse_formats
 from .base import DataSourceMixin, Schema
 
-import glob
-
 
 class RasterIOSource(DataSourceMixin, PatternMixin):
     """Open a xarray dataset via RasterIO.
 
     This creates an xarray.array, not a dataset (i.e., there is exactly one
     variable).
 
@@ -55,15 +53,17 @@
             self._can_be_local = fsspec.utils.can_be_local(self.urlpath[0])
         else:
             self._can_be_local = fsspec.utils.can_be_local(self.urlpath)
         super(RasterIOSource, self).__init__(metadata=metadata)
 
     def _open_files(self, files):
         import xarray as xr
-        das = [xr.open_rasterio(f, chunks=self.chunks, **self._kwargs)
+        import rioxarray as rio
+
+        das = [rio.open_rasterio(f, chunks=self.chunks, **self._kwargs)
                for f in files]
         out = xr.concat(das, dim=self.dim)
 
         coords = {}
         if self.pattern:
             coords = {
                 k: xr.concat(
@@ -74,25 +74,26 @@
                 for k, values in reverse_formats(self.pattern, files).items()
             }
 
         return out.assign_coords(**coords).chunk(self.chunks)
 
     def _open_dataset(self):
         import xarray as xr
+        import rioxarray as rio
         if self._can_be_local:
             files = fsspec.open_local(self.urlpath, **self.storage_options)
         else:
             # pass URLs to delegate remote opening to rasterio library
             files = self.urlpath
             #files = fsspec.open(self.urlpath, **self.storage_options).open()
         if isinstance(files, list):
             self._ds = self._open_files(files)
         else:
-            self._ds = xr.open_rasterio(files, chunks=self.chunks,
-                                        **self._kwargs)
+            self._ds = rio.open_rasterio(files, chunks=self.chunks,
+                                         **self._kwargs)
 
     def _get_schema(self):
         """Make schema object, which embeds xarray object and some details"""
         from .xarray_container import serialize_zarr_ds
         import msgpack
         import xarray as xr
```

### Comparing `intake-xarray-0.6.1/intake_xarray/tests/conftest.py` & `intake-xarray-0.7.0/intake_xarray/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `intake-xarray-0.6.1/intake_xarray/tests/test_catalog.py` & `intake-xarray-0.7.0/intake_xarray/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `intake-xarray-0.6.1/intake_xarray/tests/test_derived.py` & `intake-xarray-0.7.0/intake_xarray/tests/test_derived.py`

 * *Files identical despite different names*

### Comparing `intake-xarray-0.6.1/intake_xarray/tests/test_image.py` & `intake-xarray-0.7.0/intake_xarray/tests/test_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
 def test_coerce_shape_array_non_int():
     shape = (2, 3)
     array = np.random.random((3, 2))
     expected = np.append(array[:2, :], [[0], [0]], axis=1)
     actual = _coerce_shape(array, shape)
     assert (expected == actual).all()
-    assert expected.dtype == np.float
+    assert expected.dtype == "float"
 
 
 def test_read_image():
     pytest.importorskip('skimage')
     urlpath = os.path.join(here, 'data', 'images', 'beach57.tif')
     source = ImageSource(urlpath=urlpath)
     array = source.read()
```

### Comparing `intake-xarray-0.6.1/intake_xarray/tests/test_intake_xarray.py` & `intake-xarray-0.7.0/intake_xarray/tests/test_intake_xarray.py`

 * *Files identical despite different names*

### Comparing `intake-xarray-0.6.1/intake_xarray/tests/test_network.py` & `intake-xarray-0.7.0/intake_xarray/tests/test_network.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Tests that read public data over the internet
 import intake
 import pytest
 import xarray as xr
-import s3fs
-import gcsfs
+
 
 # RasterIOSource
+@pytest.mark.xfail
 def test_open_rasterio_http():
     prefix = 'https://landsat-pds.s3.us-west-2.amazonaws.com/L8/139/045'
     image = 'LC81390452014295LGN00/LC81390452014295LGN00_B1.TIF'
     url = f'{prefix}/{image}'
     source = intake.open_rasterio(url,
                                   chunks=dict(band=1))
     ds = source.to_dask()
@@ -33,30 +33,32 @@
     key = 'bedmachine/BedMachineAntarctica_2019-11-05_v01.nc'
     url = f'{bucket}/{key}'
     source = intake.open_netcdf(url,
                                 chunks=3000,
                                 xarray_kwargs=dict(engine='h5netcdf'),
                                 )
     ds = source.to_dask()
-    assert isinstance(ds._file_obj, xr.backends.h5netcdf_.H5NetCDFStore)
     assert isinstance(ds, xr.core.dataarray.Dataset)
 
+
+@pytest.mark.xfail
 def test_open_netcdf_s3():
     bucket = 's3://its-live-data.jpl.nasa.gov'
     key = 'icesat2/alt06/rel003/ATL06_20181230162257_00340206_003_01.h5'
     url = f'{bucket}/{key}'
     source = intake.open_netcdf(url,
                                 xarray_kwargs=dict(group='gt1l/land_ice_segments', engine='h5netcdf'),
                                 storage_options=dict(anon=True),
                                 )
     ds = source.to_dask()
     assert isinstance(ds._file_obj, xr.backends.h5netcdf_.H5NetCDFStore)
     assert isinstance(ds, xr.core.dataarray.Dataset)
 
 
+@pytest.mark.xfail
 def test_open_netcdf_s3_simplecache():
     bucket = 's3://its-live-data.jpl.nasa.gov'
     key = 'icesat2/alt06/rel003/ATL06_20181230162257_00340206_003_01.h5'
     url = f'simplecache::{bucket}/{key}'
     source = intake.open_netcdf(url,
                                 xarray_kwargs=dict(group='gt1l/land_ice_segments', engine='h5netcdf'),
                                 storage_options=dict(s3={'anon': True}),
```

### Comparing `intake-xarray-0.6.1/intake_xarray/tests/test_remote.py` & `intake-xarray-0.7.0/intake_xarray/tests/test_remote.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,16 @@
 
 
 def test_http_read_rasterio(data_server):
     url = f'{data_server}/RGB.byte.tif'
     source = intake.open_rasterio(url)
     da = source.read()
     # Following line: original file CRS appears to be updated
-    assert "+init" in da.attrs['crs'] or "+proj" in da.attrs['crs']
+    assert ("+init" in da.attrs.get('crs', "") or "+proj" in da.attrs.get('crs', "") or
+            "PROJCS" in da.spatial_ref.attrs["crs_wkt"])
     assert da.attrs['AREA_OR_POINT'] == 'Area'
     assert da.dtype == 'uint8'
     assert da.isel(band=2,x=300,y=500).values == 129
 
 
 def test_http_open_rasterio_dask(data_server):
     url = f'{data_server}/RGB.byte.tif'
@@ -227,15 +228,16 @@
     os.environ['AWS_HTTPS']= 'NO'
     os.environ['GDAL_DISABLE_READDIR_ON_OPEN']='EMPTY_DIR'
     os.environ['CPL_CURL_VERBOSE']='YES'
     url = f's3://{test_bucket_name}/RGB.byte.tif'
     source = intake.open_rasterio(url)
     da = source.read()
     # Following line: original file CRS appears to be updated
-    assert "+init" in da.attrs['crs'] or "+proj" in da.attrs['crs']
+    assert ("+init" in da.attrs.get('crs', "") or "+proj" in da.attrs.get('crs', "") or
+            "PROJCS" in da.spatial_ref.attrs["crs_wkt"])
     assert da.attrs['AREA_OR_POINT'] == 'Area'
     assert da.dtype == 'uint8'
     assert da.isel(band=2,x=300,y=500).values == 129
 
 
 def test_s3_read_netcdf(s3):
     url = f's3://{test_bucket_name}/example_1.nc'
```

### Comparing `intake-xarray-0.6.1/intake_xarray/xarray_container.py` & `intake-xarray-0.7.0/intake_xarray/xarray_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,16 +93,19 @@
             # TODO: in the future, these could be functions from the metadata?
             self._ds = self._ds.assign_coords(**{c: self._get_partition((c, ))
                                                  for c in metadata['coords']})
             for var in list(self._ds.data_vars):
                 # recreate dask arrays
                 name = '-'.join(['remote-xarray', var, self._source_id])
                 arr = self._ds[var].data
-                chunks = arr.chunks
-                nparts = (range(len(n)) for n in chunks)
+                if hasattr(arr, "chunks"):
+                    chunks = arr.chunks
+                    nparts = (range(len(n)) for n in chunks)
+                else:
+                    nparts = ((1,), )
                 if self.metadata.get('array', False):
                     # original was an array, not dataset - no variable name
                     extra = ()
                 else:
                     extra = (var, )
                 dask = {
                     (name, ) + part: (get_partition, self.url, self.headers,
```

### Comparing `intake-xarray-0.6.1/intake_xarray/xzarr.py` & `intake-xarray-0.7.0/intake_xarray/xzarr.py`

 * *Files identical despite different names*

### Comparing `intake-xarray-0.6.1/intake_xarray.egg-info/PKG-INFO` & `intake-xarray-0.7.0/intake_xarray.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: intake-xarray
-Version: 0.6.1
+Version: 0.7.0
 Summary: xarray plugins for Intake
-Home-page: https://github.com/ContinuumIO/intake-xarray
+Home-page: https://github.com/intake/intake-xarray
 Maintainer: Martin Durant
 Maintainer-email: mdurant@anaconda.com
 License: BSD
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # intake-xarray
 
 ![CI](https://github.com/intake/intake-xarray/workflows/CI/badge.svg)
 
@@ -40,9 +39,7 @@
 ```
 
 To install optional dependencies:
 
 ```
 conda install -c conda-forge pydap rasterio
 ```
-
-
```

### Comparing `intake-xarray-0.6.1/setup.py` & `intake-xarray-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                     'msgpack', 'requests']
 
 setup(
     name='intake-xarray',
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     description='xarray plugins for Intake',
-    url='https://github.com/ContinuumIO/intake-xarray',
+    url='https://github.com/intake/intake-xarray',
     maintainer='Martin Durant',
     maintainer_email='mdurant@anaconda.com',
     license='BSD',
     py_modules=['intake_xarray'],
     packages=find_packages(),
     entry_points={
         'intake.drivers': [
```

### Comparing `intake-xarray-0.6.1/versioneer.py` & `intake-xarray-0.7.0/versioneer.py`

 * *Files identical despite different names*

