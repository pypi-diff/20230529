# Comparing `tmp/traveltimepy-3.3.0.tar.gz` & `tmp/traveltimepy-3.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traveltimepy-3.3.0.tar", last modified: Mon May 15 14:52:44 2023, max compression
+gzip compressed data, was "traveltimepy-3.3.0b1.tar", last modified: Mon May 29 08:59:50 2023, max compression
```

## Comparing `traveltimepy-3.3.0.tar` & `traveltimepy-3.3.0b1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:52:44.649499 traveltimepy-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    24509 2023-05-15 14:52:44.649499 traveltimepy-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24259 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:52:44.641499 traveltimepy-3.3.0/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/benchmarks/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/benchmarks/time_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/benchmarks/time_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-15 14:52:44.649499 traveltimepy-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:52:44.641499 traveltimepy-3.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/tests/geocoding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/tests/map_info_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/tests/postcodes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/tests/routes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/tests/supported_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/tests/time_filter_fast_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/tests/time_filter_proto_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/tests/time_filter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/tests/time_map_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:52:44.645499 traveltimepy-3.3.0/traveltimepy/
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-15 14:52:22.000000 traveltimepy-3.3.0/traveltimepy/TimeFilterFastRequest_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-15 14:52:22.000000 traveltimepy-3.3.0/traveltimepy/TimeFilterFastResponse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/accept_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:52:44.645499 traveltimepy-3.3.0/traveltimepy/dto/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:52:44.649499 traveltimepy-3.3.0/traveltimepy/dto/requests/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/requests/postcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/requests/postcodes_zones.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/requests/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/requests/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/requests/supported_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/requests/time_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/requests/time_filter_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/requests/time_filter_proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/requests/time_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:52:44.649499 traveltimepy-3.3.0/traveltimepy/dto/responses/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/responses/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/responses/map_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/responses/postcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/responses/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/responses/supported_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/responses/time_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/responses/time_filter_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/responses/time_filter_proto.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/responses/time_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/responses/zones.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/dto/transportation.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)    20427 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/proto_http.py
--rw-r--r--   0 runner    (1001) docker     (123)    24669 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 14:52:14.000000 traveltimepy-3.3.0/traveltimepy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:52:44.645499 traveltimepy-3.3.0/traveltimepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24509 2023-05-15 14:52:44.000000 traveltimepy-3.3.0/traveltimepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-15 14:52:44.000000 traveltimepy-3.3.0/traveltimepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:52:44.000000 traveltimepy-3.3.0/traveltimepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:52:44.000000 traveltimepy-3.3.0/traveltimepy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-15 14:52:44.000000 traveltimepy-3.3.0/traveltimepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-15 14:52:44.000000 traveltimepy-3.3.0/traveltimepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:59:50.549339 traveltimepy-3.3.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    24511 2023-05-29 08:59:50.549339 traveltimepy-3.3.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24259 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:59:50.537338 traveltimepy-3.3.0b1/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/benchmarks/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/benchmarks/time_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/benchmarks/time_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-29 08:59:50.549339 traveltimepy-3.3.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:59:50.541339 traveltimepy-3.3.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/tests/geocoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/tests/map_info_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/tests/postcodes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/tests/routes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/tests/supported_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/tests/time_filter_fast_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/tests/time_filter_proto_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/tests/time_filter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/tests/time_map_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:59:50.545339 traveltimepy-3.3.0b1/traveltimepy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-29 08:59:39.000000 traveltimepy-3.3.0b1/traveltimepy/TimeFilterFastRequest_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-29 08:59:39.000000 traveltimepy-3.3.0b1/traveltimepy/TimeFilterFastResponse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/accept_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:59:50.545339 traveltimepy-3.3.0b1/traveltimepy/dto/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:59:50.549339 traveltimepy-3.3.0b1/traveltimepy/dto/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/requests/postcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/requests/postcodes_zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/requests/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/requests/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/requests/supported_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/requests/time_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/requests/time_filter_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/requests/time_filter_proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/requests/time_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:59:50.549339 traveltimepy-3.3.0b1/traveltimepy/dto/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/responses/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/responses/map_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/responses/postcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/responses/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/responses/supported_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/responses/time_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/responses/time_filter_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/responses/time_filter_proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/responses/time_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/responses/zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/dto/transportation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20427 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/proto_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24669 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-29 08:59:34.000000 traveltimepy-3.3.0b1/traveltimepy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:59:50.545339 traveltimepy-3.3.0b1/traveltimepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24511 2023-05-29 08:59:50.000000 traveltimepy-3.3.0b1/traveltimepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-29 08:59:50.000000 traveltimepy-3.3.0b1/traveltimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 08:59:50.000000 traveltimepy-3.3.0b1/traveltimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 08:59:50.000000 traveltimepy-3.3.0b1/traveltimepy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-29 08:59:50.000000 traveltimepy-3.3.0b1/traveltimepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 08:59:50.000000 traveltimepy-3.3.0b1/traveltimepy.egg-info/top_level.txt
```

### Comparing `traveltimepy-3.3.0/LICENSE` & `traveltimepy-3.3.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/PKG-INFO` & `traveltimepy-3.3.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traveltimepy
-Version: 3.3.0
+Version: 3.3.0b1
 Summary: "Python Interface to Travel Time."
 Author: TravelTime
 License: MIT
 Keywords: traveltimepy,api,maps
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `traveltimepy-3.3.0/README.md` & `traveltimepy-3.3.0b1/README.md`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/benchmarks/common.py` & `traveltimepy-3.3.0b1/benchmarks/common.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/benchmarks/time_filter.py` & `traveltimepy-3.3.0b1/benchmarks/time_filter.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/benchmarks/time_map.py` & `traveltimepy-3.3.0b1/benchmarks/time_map.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/tests/conftest.py` & `traveltimepy-3.3.0b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/tests/postcodes_test.py` & `traveltimepy-3.3.0b1/tests/postcodes_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/tests/routes_test.py` & `traveltimepy-3.3.0b1/tests/routes_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/tests/supported_locations.py` & `traveltimepy-3.3.0b1/tests/supported_locations.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/tests/time_filter_fast_test.py` & `traveltimepy-3.3.0b1/tests/time_filter_fast_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/tests/time_filter_proto_test.py` & `traveltimepy-3.3.0b1/tests/time_filter_proto_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/tests/time_filter_test.py` & `traveltimepy-3.3.0b1/tests/time_filter_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/tests/time_map_test.py` & `traveltimepy-3.3.0b1/tests/time_map_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/traveltimepy/TimeFilterFastRequest_pb2.py` & `traveltimepy-3.3.0b1/traveltimepy/TimeFilterFastRequest_pb2.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/traveltimepy/TimeFilterFastResponse_pb2.py` & `traveltimepy-3.3.0b1/traveltimepy/TimeFilterFastResponse_pb2.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/traveltimepy/__init__.py` & `traveltimepy-3.3.0b1/traveltimepy/__init__.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/traveltimepy/dto/common.py` & `traveltimepy-3.3.0b1/traveltimepy/dto/common.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/traveltimepy/dto/requests/postcodes.py` & `traveltimepy-3.3.0b1/traveltimepy/dto/requests/postcodes.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/traveltimepy/dto/requests/postcodes_zones.py` & `traveltimepy-3.3.0b1/traveltimepy/dto/requests/postcodes_zones.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/traveltimepy/dto/requests/routes.py` & `traveltimepy-3.3.0b1/traveltimepy/dto/requests/routes.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/traveltimepy/dto/requests/supported_locations.py` & `traveltimepy-3.3.0b1/traveltimepy/dto/requests/supported_locations.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/traveltimepy/dto/requests/time_filter.py` & `traveltimepy-3.3.0b1/traveltimepy/dto/requests/time_filter.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/traveltimepy/dto/requests/time_filter_fast.py` & `traveltimepy-3.3.0b1/traveltimepy/dto/requests/time_filter_fast.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/traveltimepy/dto/requests/time_filter_proto.py` & `traveltimepy-3.3.0b1/traveltimepy/dto/requests/time_filter_proto.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/traveltimepy/dto/requests/time_map.py` & `traveltimepy-3.3.0b1/traveltimepy/dto/requests/time_map.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/traveltimepy/dto/responses/time_filter.py` & `traveltimepy-3.3.0b1/traveltimepy/dto/responses/time_filter.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/traveltimepy/dto/responses/time_filter_fast.py` & `traveltimepy-3.3.0b1/traveltimepy/dto/responses/time_filter_fast.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/traveltimepy/dto/responses/zones.py` & `traveltimepy-3.3.0b1/traveltimepy/dto/responses/zones.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/traveltimepy/dto/transportation.py` & `traveltimepy-3.3.0b1/traveltimepy/dto/transportation.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/traveltimepy/http.py` & `traveltimepy-3.3.0b1/traveltimepy/http.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/traveltimepy/itertools.py` & `traveltimepy-3.3.0b1/traveltimepy/itertools.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/traveltimepy/mapper.py` & `traveltimepy-3.3.0b1/traveltimepy/mapper.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/traveltimepy/proto_http.py` & `traveltimepy-3.3.0b1/traveltimepy/proto_http.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/traveltimepy/sdk.py` & `traveltimepy-3.3.0b1/traveltimepy/sdk.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.3.0/traveltimepy.egg-info/PKG-INFO` & `traveltimepy-3.3.0b1/traveltimepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traveltimepy
-Version: 3.3.0
+Version: 3.3.0b1
 Summary: "Python Interface to Travel Time."
 Author: TravelTime
 License: MIT
 Keywords: traveltimepy,api,maps
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `traveltimepy-3.3.0/traveltimepy.egg-info/SOURCES.txt` & `traveltimepy-3.3.0b1/traveltimepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

