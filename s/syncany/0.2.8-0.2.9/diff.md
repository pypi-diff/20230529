# Comparing `tmp/syncany-0.2.8.tar.gz` & `tmp/syncany-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncany-0.2.8.tar", last modified: Tue May  2 08:48:46 2023, max compression
+gzip compressed data, was "syncany-0.2.9.tar", last modified: Fri May 12 09:48:41 2023, max compression
```

## Comparing `syncany-0.2.8.tar` & `syncany-0.2.9.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:46.435967 syncany-0.2.8/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2022-08-13 12:36:15.000000 syncany-0.2.8/LICENSE
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7103 2023-05-02 08:48:46.437967 syncany-0.2.8/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5832 2022-08-13 12:36:15.000000 syncany-0.2.8/README.md
--rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-05-02 08:48:46.447486 syncany-0.2.8/setup.cfg
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1928 2023-04-29 02:27:19.000000 syncany-0.2.8/setup.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:40.958386 syncany-0.2.8/syncany/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      607 2023-04-29 02:27:19.000000 syncany-0.2.8/syncany/__init__.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:41.670417 syncany-0.2.8/syncany/calculaters/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4962 2023-04-25 03:51:51.000000 syncany-0.2.8/syncany/calculaters/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    39895 2023-04-28 09:52:26.000000 syncany-0.2.8/syncany/calculaters/builtin.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4394 2023-03-24 09:30:00.000000 syncany-0.2.8/syncany/calculaters/calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7999 2023-03-27 08:30:23.000000 syncany-0.2.8/syncany/calculaters/convert_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4573 2023-03-23 03:10:08.000000 syncany-0.2.8/syncany/calculaters/datetime_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2731 2023-04-27 09:47:49.000000 syncany-0.2.8/syncany/calculaters/import_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3167 2023-03-23 03:10:08.000000 syncany-0.2.8/syncany/calculaters/textline_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    13898 2023-04-27 03:28:48.000000 syncany-0.2.8/syncany/calculaters/transform_calculater.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:42.732953 syncany-0.2.8/syncany/database/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5187 2023-04-25 03:51:51.000000 syncany-0.2.8/syncany/database/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8756 2023-03-24 06:27:35.000000 syncany-0.2.8/syncany/database/beanstalk.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    15594 2023-04-25 03:41:03.000000 syncany-0.2.8/syncany/database/clickhouse.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    15749 2023-04-25 02:15:32.000000 syncany-0.2.8/syncany/database/csv.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    10484 2023-04-26 02:09:40.000000 syncany-0.2.8/syncany/database/database.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12481 2023-02-24 09:33:28.000000 syncany-0.2.8/syncany/database/elasticsearch.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14490 2023-04-25 02:15:32.000000 syncany-0.2.8/syncany/database/excel.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14218 2023-02-22 05:00:17.000000 syncany-0.2.8/syncany/database/http.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    17931 2023-02-24 09:33:28.000000 syncany-0.2.8/syncany/database/influxdb.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12051 2023-04-25 02:15:32.000000 syncany-0.2.8/syncany/database/json.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    11954 2023-04-25 02:15:32.000000 syncany-0.2.8/syncany/database/memory.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14642 2023-04-25 03:15:38.000000 syncany-0.2.8/syncany/database/mongodb.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14723 2023-04-25 03:35:50.000000 syncany-0.2.8/syncany/database/mysql.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14858 2023-04-25 03:37:13.000000 syncany-0.2.8/syncany/database/postgresql.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    18023 2023-04-25 02:22:52.000000 syncany-0.2.8/syncany/database/redis.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    13949 2023-03-28 03:39:46.000000 syncany-0.2.8/syncany/database/sqlite.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    15489 2023-04-25 03:39:10.000000 syncany-0.2.8/syncany/database/sqlserver.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    17928 2023-04-23 08:27:57.000000 syncany-0.2.8/syncany/database/textline.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      685 2022-08-23 12:03:29.000000 syncany-0.2.8/syncany/errors.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:42.915979 syncany-0.2.8/syncany/filters/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2275 2023-04-25 03:51:51.000000 syncany-0.2.8/syncany/filters/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    19439 2023-04-01 08:20:13.000000 syncany-0.2.8/syncany/filters/builtin.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      309 2022-08-13 12:36:15.000000 syncany-0.2.8/syncany/filters/filter.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1957 2023-02-16 02:10:09.000000 syncany-0.2.8/syncany/hook.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:43.331493 syncany-0.2.8/syncany/loaders/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      927 2023-03-25 04:34:57.000000 syncany-0.2.8/syncany/loaders/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1403 2023-04-27 03:37:21.000000 syncany-0.2.8/syncany/loaders/cache.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1001 2023-04-27 10:25:51.000000 syncany-0.2.8/syncany/loaders/const.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6587 2023-05-01 07:54:55.000000 syncany-0.2.8/syncany/loaders/db.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8832 2023-04-28 01:46:51.000000 syncany-0.2.8/syncany/loaders/db_join.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1754 2023-04-27 03:37:21.000000 syncany-0.2.8/syncany/loaders/db_pull.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     9616 2023-04-30 15:15:40.000000 syncany-0.2.8/syncany/loaders/loader.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      214 2022-08-13 12:36:15.000000 syncany-0.2.8/syncany/logger.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    13966 2023-03-24 04:36:02.000000 syncany-0.2.8/syncany/main.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:43.750243 syncany-0.2.8/syncany/outputers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1161 2023-03-25 04:34:57.000000 syncany-0.2.8/syncany/outputers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1491 2023-02-24 04:31:16.000000 syncany-0.2.8/syncany/outputers/db.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1962 2023-04-25 03:15:38.000000 syncany-0.2.8/syncany/outputers/db_delete_insert.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      932 2023-04-25 03:15:38.000000 syncany-0.2.8/syncany/outputers/db_insert.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5697 2023-04-25 03:15:38.000000 syncany-0.2.8/syncany/outputers/db_update_delete_insert.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4210 2023-04-25 03:15:38.000000 syncany-0.2.8/syncany/outputers/db_update_insert.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2864 2023-03-22 02:35:53.000000 syncany-0.2.8/syncany/outputers/outputer.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:44.054012 syncany-0.2.8/syncany/taskers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)       52 2022-08-13 12:36:15.000000 syncany-0.2.8/syncany/taskers/__init__.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:44.561012 syncany-0.2.8/syncany/taskers/config/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1794 2023-03-25 04:34:57.000000 syncany-0.2.8/syncany/taskers/config/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      405 2022-08-23 12:07:09.000000 syncany-0.2.8/syncany/taskers/config/file_reader.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      937 2022-08-23 12:07:09.000000 syncany-0.2.8/syncany/taskers/config/http_reader.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      195 2022-08-13 12:36:15.000000 syncany-0.2.8/syncany/taskers/config/json_parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      208 2022-08-13 12:36:15.000000 syncany-0.2.8/syncany/taskers/config/parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      204 2022-08-23 11:55:44.000000 syncany-0.2.8/syncany/taskers/config/reader.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5006 2022-08-13 12:36:15.000000 syncany-0.2.8/syncany/taskers/config/yaml_parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1377 2023-02-24 02:44:01.000000 syncany-0.2.8/syncany/taskers/context.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:45.069025 syncany-0.2.8/syncany/taskers/core/
--rwxrwxrwx   0 snower    (1000) snower    (1000)    73709 2023-05-01 07:47:08.000000 syncany-0.2.8/syncany/taskers/core/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2192 2023-03-21 06:17:51.000000 syncany-0.2.8/syncany/taskers/core/loader_creater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      256 2022-08-13 12:36:15.000000 syncany-0.2.8/syncany/taskers/core/option.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2592 2023-02-10 08:39:32.000000 syncany-0.2.8/syncany/taskers/core/outputer_creater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4736 2022-08-13 12:36:15.000000 syncany-0.2.8/syncany/taskers/core/states.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    15689 2023-02-25 11:47:43.000000 syncany-0.2.8/syncany/taskers/core/valuer_compiler.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    42975 2023-04-28 01:45:52.000000 syncany-0.2.8/syncany/taskers/core/valuer_creater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      760 2023-02-25 12:43:51.000000 syncany-0.2.8/syncany/taskers/iterator.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      245 2022-08-13 12:36:15.000000 syncany-0.2.8/syncany/taskers/manager.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7122 2023-04-20 05:48:37.000000 syncany-0.2.8/syncany/taskers/tasker.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    11025 2023-04-20 03:35:47.000000 syncany-0.2.8/syncany/utils.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:46.390869 syncany-0.2.8/syncany/valuers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2193 2023-04-27 03:26:45.000000 syncany-0.2.8/syncany/valuers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5565 2023-04-27 07:59:50.000000 syncany-0.2.8/syncany/valuers/aggregate.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5094 2023-04-27 07:59:50.000000 syncany-0.2.8/syncany/valuers/assign.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7021 2023-04-27 06:17:05.000000 syncany-0.2.8/syncany/valuers/cache.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5314 2023-04-27 08:52:53.000000 syncany-0.2.8/syncany/valuers/calculate.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8936 2023-04-27 06:17:04.000000 syncany-0.2.8/syncany/valuers/call.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6980 2023-04-28 06:13:22.000000 syncany-0.2.8/syncany/valuers/case.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6243 2023-04-28 06:13:22.000000 syncany-0.2.8/syncany/valuers/condition.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      548 2023-04-27 03:12:59.000000 syncany-0.2.8/syncany/valuers/const.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4916 2023-04-28 05:47:00.000000 syncany-0.2.8/syncany/valuers/data.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     9997 2023-04-28 03:45:24.000000 syncany-0.2.8/syncany/valuers/db_join.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3424 2023-04-27 04:30:58.000000 syncany-0.2.8/syncany/valuers/db_load.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3082 2023-04-27 04:30:58.000000 syncany-0.2.8/syncany/valuers/function.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8557 2023-04-27 08:06:54.000000 syncany-0.2.8/syncany/valuers/generator.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5698 2023-05-01 07:19:03.000000 syncany-0.2.8/syncany/valuers/inherit.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5129 2023-04-27 06:17:05.000000 syncany-0.2.8/syncany/valuers/let.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    16860 2023-04-27 06:17:04.000000 syncany-0.2.8/syncany/valuers/loop.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8197 2023-04-28 06:13:22.000000 syncany-0.2.8/syncany/valuers/make.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12466 2023-04-28 06:13:22.000000 syncany-0.2.8/syncany/valuers/match.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2308 2023-04-27 06:17:04.000000 syncany-0.2.8/syncany/valuers/schema.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5717 2023-04-27 06:17:04.000000 syncany-0.2.8/syncany/valuers/state.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8187 2023-04-30 16:14:31.000000 syncany-0.2.8/syncany/valuers/valuer.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:48:41.226388 syncany-0.2.8/syncany.egg-info/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7103 2023-05-02 08:48:39.000000 syncany-0.2.8/syncany.egg-info/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2889 2023-05-02 08:48:40.000000 syncany-0.2.8/syncany.egg-info/SOURCES.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-05-02 08:48:39.000000 syncany-0.2.8/syncany.egg-info/dependency_links.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       47 2023-05-02 08:48:39.000000 syncany-0.2.8/syncany.egg-info/entry_points.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2022-08-15 03:43:33.000000 syncany-0.2.8/syncany.egg-info/not-zip-safe
--rwxrwxrwx   0 snower    (1000) snower    (1000)      371 2023-05-02 08:48:39.000000 syncany-0.2.8/syncany.egg-info/requires.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        8 2023-05-02 08:48:39.000000 syncany-0.2.8/syncany.egg-info/top_level.txt
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:48:41.129071 syncany-0.2.9/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2022-08-13 12:36:15.000000 syncany-0.2.9/LICENSE
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7103 2023-05-12 09:48:41.130069 syncany-0.2.9/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5832 2022-08-13 12:36:15.000000 syncany-0.2.9/README.md
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-05-12 09:48:41.140046 syncany-0.2.9/setup.cfg
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1928 2023-05-08 07:05:44.000000 syncany-0.2.9/setup.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:48:35.402367 syncany-0.2.9/syncany/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      607 2023-05-08 07:05:44.000000 syncany-0.2.9/syncany/__init__.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:48:36.180316 syncany-0.2.9/syncany/calculaters/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4962 2023-04-25 03:51:51.000000 syncany-0.2.9/syncany/calculaters/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    39895 2023-04-28 09:52:26.000000 syncany-0.2.9/syncany/calculaters/builtin.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4394 2023-03-24 09:30:00.000000 syncany-0.2.9/syncany/calculaters/calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7999 2023-03-27 08:30:23.000000 syncany-0.2.9/syncany/calculaters/convert_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4573 2023-03-23 03:10:08.000000 syncany-0.2.9/syncany/calculaters/datetime_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2731 2023-04-27 09:47:49.000000 syncany-0.2.9/syncany/calculaters/import_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3167 2023-03-23 03:10:08.000000 syncany-0.2.9/syncany/calculaters/textline_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    13898 2023-04-27 03:28:48.000000 syncany-0.2.9/syncany/calculaters/transform_calculater.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:48:37.318836 syncany-0.2.9/syncany/database/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5187 2023-04-25 03:51:51.000000 syncany-0.2.9/syncany/database/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8711 2023-05-08 06:45:36.000000 syncany-0.2.9/syncany/database/beanstalk.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    15594 2023-04-25 03:41:03.000000 syncany-0.2.9/syncany/database/clickhouse.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    15886 2023-05-08 06:45:36.000000 syncany-0.2.9/syncany/database/csv.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14308 2023-05-08 06:40:40.000000 syncany-0.2.9/syncany/database/database.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12481 2023-02-24 09:33:28.000000 syncany-0.2.9/syncany/database/elasticsearch.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14627 2023-05-08 06:45:36.000000 syncany-0.2.9/syncany/database/excel.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14218 2023-02-22 05:00:17.000000 syncany-0.2.9/syncany/database/http.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    17931 2023-02-24 09:33:28.000000 syncany-0.2.9/syncany/database/influxdb.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12188 2023-05-08 06:45:36.000000 syncany-0.2.9/syncany/database/json.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12097 2023-05-08 06:45:36.000000 syncany-0.2.9/syncany/database/memory.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14642 2023-04-25 03:15:38.000000 syncany-0.2.9/syncany/database/mongodb.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14723 2023-04-25 03:35:50.000000 syncany-0.2.9/syncany/database/mysql.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14858 2023-04-25 03:37:13.000000 syncany-0.2.9/syncany/database/postgresql.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    18166 2023-05-08 06:45:36.000000 syncany-0.2.9/syncany/database/redis.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    13949 2023-03-28 03:39:46.000000 syncany-0.2.9/syncany/database/sqlite.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    15489 2023-04-25 03:39:10.000000 syncany-0.2.9/syncany/database/sqlserver.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    18031 2023-05-08 06:45:36.000000 syncany-0.2.9/syncany/database/textline.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      685 2022-08-23 12:03:29.000000 syncany-0.2.9/syncany/errors.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:48:37.504862 syncany-0.2.9/syncany/filters/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2275 2023-04-25 03:51:51.000000 syncany-0.2.9/syncany/filters/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    19439 2023-04-01 08:20:13.000000 syncany-0.2.9/syncany/filters/builtin.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      309 2022-08-13 12:36:15.000000 syncany-0.2.9/syncany/filters/filter.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1957 2023-02-16 02:10:09.000000 syncany-0.2.9/syncany/hook.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:48:37.948469 syncany-0.2.9/syncany/loaders/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      927 2023-03-25 04:34:57.000000 syncany-0.2.9/syncany/loaders/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1403 2023-04-27 03:37:21.000000 syncany-0.2.9/syncany/loaders/cache.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1001 2023-04-27 10:25:51.000000 syncany-0.2.9/syncany/loaders/const.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6587 2023-05-01 07:54:55.000000 syncany-0.2.9/syncany/loaders/db.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8832 2023-04-28 01:46:51.000000 syncany-0.2.9/syncany/loaders/db_join.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1754 2023-04-27 03:37:21.000000 syncany-0.2.9/syncany/loaders/db_pull.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     9616 2023-04-30 15:15:40.000000 syncany-0.2.9/syncany/loaders/loader.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      214 2022-08-13 12:36:15.000000 syncany-0.2.9/syncany/logger.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    13966 2023-03-24 04:36:02.000000 syncany-0.2.9/syncany/main.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:48:38.363532 syncany-0.2.9/syncany/outputers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1161 2023-03-25 04:34:57.000000 syncany-0.2.9/syncany/outputers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1491 2023-02-24 04:31:16.000000 syncany-0.2.9/syncany/outputers/db.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1962 2023-04-25 03:15:38.000000 syncany-0.2.9/syncany/outputers/db_delete_insert.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      932 2023-04-25 03:15:38.000000 syncany-0.2.9/syncany/outputers/db_insert.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5697 2023-04-25 03:15:38.000000 syncany-0.2.9/syncany/outputers/db_update_delete_insert.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4210 2023-04-25 03:15:38.000000 syncany-0.2.9/syncany/outputers/db_update_insert.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2864 2023-03-22 02:35:53.000000 syncany-0.2.9/syncany/outputers/outputer.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:48:38.679926 syncany-0.2.9/syncany/taskers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       52 2022-08-13 12:36:15.000000 syncany-0.2.9/syncany/taskers/__init__.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:48:39.166761 syncany-0.2.9/syncany/taskers/config/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1794 2023-03-25 04:34:57.000000 syncany-0.2.9/syncany/taskers/config/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      405 2022-08-23 12:07:09.000000 syncany-0.2.9/syncany/taskers/config/file_reader.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      937 2022-08-23 12:07:09.000000 syncany-0.2.9/syncany/taskers/config/http_reader.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      195 2022-08-13 12:36:15.000000 syncany-0.2.9/syncany/taskers/config/json_parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      208 2022-08-13 12:36:15.000000 syncany-0.2.9/syncany/taskers/config/parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      204 2022-08-23 11:55:44.000000 syncany-0.2.9/syncany/taskers/config/reader.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5006 2022-08-13 12:36:15.000000 syncany-0.2.9/syncany/taskers/config/yaml_parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1377 2023-02-24 02:44:01.000000 syncany-0.2.9/syncany/taskers/context.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:48:39.683902 syncany-0.2.9/syncany/taskers/core/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    73709 2023-05-01 07:47:08.000000 syncany-0.2.9/syncany/taskers/core/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2192 2023-03-21 06:17:51.000000 syncany-0.2.9/syncany/taskers/core/loader_creater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      256 2022-08-13 12:36:15.000000 syncany-0.2.9/syncany/taskers/core/option.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2592 2023-02-10 08:39:32.000000 syncany-0.2.9/syncany/taskers/core/outputer_creater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4736 2022-08-13 12:36:15.000000 syncany-0.2.9/syncany/taskers/core/states.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    15689 2023-02-25 11:47:43.000000 syncany-0.2.9/syncany/taskers/core/valuer_compiler.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    42975 2023-04-28 01:45:52.000000 syncany-0.2.9/syncany/taskers/core/valuer_creater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      760 2023-02-25 12:43:51.000000 syncany-0.2.9/syncany/taskers/iterator.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      245 2022-08-13 12:36:15.000000 syncany-0.2.9/syncany/taskers/manager.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7122 2023-04-20 05:48:37.000000 syncany-0.2.9/syncany/taskers/tasker.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    11028 2023-05-08 06:40:40.000000 syncany-0.2.9/syncany/utils.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:48:41.076047 syncany-0.2.9/syncany/valuers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2193 2023-04-27 03:26:45.000000 syncany-0.2.9/syncany/valuers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5565 2023-04-27 07:59:50.000000 syncany-0.2.9/syncany/valuers/aggregate.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5094 2023-04-27 07:59:50.000000 syncany-0.2.9/syncany/valuers/assign.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7021 2023-04-27 06:17:05.000000 syncany-0.2.9/syncany/valuers/cache.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5314 2023-04-27 08:52:53.000000 syncany-0.2.9/syncany/valuers/calculate.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8936 2023-04-27 06:17:04.000000 syncany-0.2.9/syncany/valuers/call.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6980 2023-04-28 06:13:22.000000 syncany-0.2.9/syncany/valuers/case.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6243 2023-04-28 06:13:22.000000 syncany-0.2.9/syncany/valuers/condition.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      548 2023-04-27 03:12:59.000000 syncany-0.2.9/syncany/valuers/const.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4916 2023-04-28 05:47:00.000000 syncany-0.2.9/syncany/valuers/data.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     9997 2023-04-28 03:45:24.000000 syncany-0.2.9/syncany/valuers/db_join.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3424 2023-04-27 04:30:58.000000 syncany-0.2.9/syncany/valuers/db_load.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3082 2023-04-27 04:30:58.000000 syncany-0.2.9/syncany/valuers/function.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8557 2023-04-27 08:06:54.000000 syncany-0.2.9/syncany/valuers/generator.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5698 2023-05-01 07:19:03.000000 syncany-0.2.9/syncany/valuers/inherit.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5129 2023-04-27 06:17:05.000000 syncany-0.2.9/syncany/valuers/let.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    16860 2023-04-27 06:17:04.000000 syncany-0.2.9/syncany/valuers/loop.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8197 2023-04-28 06:13:22.000000 syncany-0.2.9/syncany/valuers/make.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12466 2023-04-28 06:13:22.000000 syncany-0.2.9/syncany/valuers/match.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2308 2023-04-27 06:17:04.000000 syncany-0.2.9/syncany/valuers/schema.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5717 2023-04-27 06:17:04.000000 syncany-0.2.9/syncany/valuers/state.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8187 2023-04-30 16:14:31.000000 syncany-0.2.9/syncany/valuers/valuer.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:48:35.712321 syncany-0.2.9/syncany.egg-info/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7103 2023-05-12 09:48:33.000000 syncany-0.2.9/syncany.egg-info/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2889 2023-05-12 09:48:34.000000 syncany-0.2.9/syncany.egg-info/SOURCES.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-05-12 09:48:33.000000 syncany-0.2.9/syncany.egg-info/dependency_links.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       47 2023-05-12 09:48:33.000000 syncany-0.2.9/syncany.egg-info/entry_points.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2022-08-15 03:43:33.000000 syncany-0.2.9/syncany.egg-info/not-zip-safe
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      371 2023-05-12 09:48:33.000000 syncany-0.2.9/syncany.egg-info/requires.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        8 2023-05-12 09:48:33.000000 syncany-0.2.9/syncany.egg-info/top_level.txt
```

### Comparing `syncany-0.2.8/LICENSE` & `syncany-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/PKG-INFO` & `syncany-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncany
-Version: 0.2.8
+Version: 0.2.9
 Summary: 简单易用的数据同步转换导出框架
 Home-page: https://github.com/snower/syncany
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # syncany
```

### Comparing `syncany-0.2.8/README.md` & `syncany-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/setup.py` & `syncany-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 18/8/6
 # create by: snower
 
 import sys
 import os
 from setuptools import find_packages, setup
 
-version = "0.2.8"
+version = "0.2.9"
 
 if os.path.exists("README.md"):
     if sys.version_info[0] >= 3:
         try:
             with open("README.md", encoding="utf-8") as fp:
                 long_description = fp.read()
         except Exception as e:
```

### Comparing `syncany-0.2.8/syncany/__init__.py` & `syncany-0.2.9/syncany/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # 18/8/6
 # create by: snower
 
-version = "0.2.8"
-version_info = (0, 2, 8)
+version = "0.2.9"
+version_info = (0, 2, 9)
 
 from .loaders import Loader, register_loader
 from .outputers import Outputer, register_outputer
 from .valuers import Valuer, register_valuer
 from .filters import Filter, register_filter
 from .database import DataBase, register_database
 from .calculaters import Calculater, TypeFormatCalculater, TypingCalculater, MathematicalCalculater, \
```

### Comparing `syncany-0.2.8/syncany/calculaters/__init__.py` & `syncany-0.2.9/syncany/calculaters/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/calculaters/builtin.py` & `syncany-0.2.9/syncany/calculaters/builtin.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/calculaters/calculater.py` & `syncany-0.2.9/syncany/calculaters/calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/calculaters/convert_calculater.py` & `syncany-0.2.9/syncany/calculaters/convert_calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/calculaters/datetime_calculater.py` & `syncany-0.2.9/syncany/calculaters/datetime_calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/calculaters/import_calculater.py` & `syncany-0.2.9/syncany/calculaters/import_calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/calculaters/textline_calculater.py` & `syncany-0.2.9/syncany/calculaters/textline_calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/calculaters/transform_calculater.py` & `syncany-0.2.9/syncany/calculaters/transform_calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/database/__init__.py` & `syncany-0.2.9/syncany/database/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/database/beanstalk.py` & `syncany-0.2.9/syncany/database/beanstalk.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # create by: snower
 
 
 import time
 import pickle
 import json
 from ..utils import human_repr_object, sorted_by_keys
-from .database import QueryBuilder, InsertBuilder, UpdateBuilder, DeleteBuilder, DataBase, DatabaseFactory
+from .database import Cmper, QueryBuilder, InsertBuilder, UpdateBuilder, DeleteBuilder, DataBase, DatabaseFactory
 
 
 class StringSerialize(object):
     def loads(self, data):
         return str(data)
 
     def dumps(self, value):
@@ -54,36 +54,36 @@
 class BeanstalkQueryBuilder(QueryBuilder):
     def __init__(self, *args, **kwargs):
         super(BeanstalkQueryBuilder, self).__init__(*args, **kwargs)
 
         self.limit = (0, self.db.bulk_size)
 
     def filter_gt(self, key, value):
-        self.query[(key, '>')] = (value, lambda a, b: a > b)
+        self.query[(key, '>')] = (value, Cmper.cmp_gt)
 
     def filter_gte(self, key, value):
-        self.query[(key, ">=")] = (value, lambda a, b: a >= b)
+        self.query[(key, ">=")] = (value, Cmper.cmp_gte)
 
     def filter_lt(self, key, value):
-        self.query[(key, "<")] = (value, lambda a, b: a < b)
+        self.query[(key, "<")] = (value, Cmper.cmp_lt)
 
     def filter_lte(self, key, value):
-        self.query[(key, "<=")] = (value, lambda a, b: a <= b)
+        self.query[(key, "<=")] = (value, Cmper.cmp_lte)
 
     def filter_eq(self, key, value):
-        self.query[(key, "==")] = (value, lambda a, b: a == b)
+        self.query[(key, "==")] = (value, Cmper.cmp_eq)
 
     def filter_ne(self, key, value):
-        self.query[(key, "!=")] = (value, lambda a, b: a != b)
+        self.query[(key, "!=")] = (value, Cmper.cmp_ne)
 
     def filter_in(self, key, value):
         try:
-            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, lambda a, b: a in b)
+            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, Cmper.cmp_in)
         except:
-            self.query[(key, "in")] = (value, lambda a, b: a in b)
+            self.query[(key, "in")] = (value, Cmper.cmp_in)
 
     def filter_limit(self, count, start=None):
         if not start:
             self.limit = (0, count)
         else:
             self.limit = (start, start + count)
```

### Comparing `syncany-0.2.8/syncany/database/clickhouse.py` & `syncany-0.2.9/syncany/database/clickhouse.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/database/csv.py` & `syncany-0.2.9/syncany/database/csv.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,48 +3,48 @@
 # create by: snower
 
 import os
 import datetime
 from ..taskers.context import TaskerContext
 from ..taskers.iterator import TaskerDataIterator, TaskerFileIterator
 from ..utils import human_repr_object, sorted_by_keys
-from .database import QueryBuilder, InsertBuilder, UpdateBuilder, DeleteBuilder, DataBase
+from .database import Cmper, QueryBuilder, InsertBuilder, UpdateBuilder, DeleteBuilder, DataBase
 
 
 class CsvFileNotFound(Exception):
     pass
 
 
 class CsvQueryBuilder(QueryBuilder):
     def __init__(self, *args, **kwargs):
         super(CsvQueryBuilder, self).__init__(*args, **kwargs)
 
     def filter_gt(self, key, value):
-        self.query[(key, '>')] = (value, lambda a, b: a > b)
+        self.query[(key, '>')] = (value, Cmper.cmp_gt)
 
     def filter_gte(self, key, value):
-        self.query[(key, ">=")] = (value, lambda a, b: a >= b)
+        self.query[(key, ">=")] = (value, Cmper.cmp_gte)
 
     def filter_lt(self, key, value):
-        self.query[(key, "<")] = (value, lambda a, b: a < b)
+        self.query[(key, "<")] = (value, Cmper.cmp_lt)
 
     def filter_lte(self, key, value):
-        self.query[(key, "<=")] = (value, lambda a, b: a <= b)
+        self.query[(key, "<=")] = (value, Cmper.cmp_lte)
 
     def filter_eq(self, key, value):
-        self.query[(key, "==")] = (value, lambda a, b: a == b)
+        self.query[(key, "==")] = (value, Cmper.cmp_eq)
 
     def filter_ne(self, key, value):
-        self.query[(key, "!=")] = (value, lambda a, b: a != b)
+        self.query[(key, "!=")] = (value, Cmper.cmp_ne)
 
     def filter_in(self, key, value):
         try:
-            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, lambda a, b: a in b)
+            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, Cmper.cmp_in)
         except:
-            self.query[(key, "in")] = (value, lambda a, b: a in b)
+            self.query[(key, "in")] = (value, Cmper.cmp_in)
 
     def filter_limit(self, count, start=None):
         if not start:
             self.limit = (0, count)
         else:
             self.limit = (start, start + count)
 
@@ -177,33 +177,36 @@
 
 
 class CsvUpdateBuilder(UpdateBuilder):
     def __init__(self, *args, **kwargs):
         super(CsvUpdateBuilder, self).__init__(*args, **kwargs)
 
     def filter_gt(self, key, value):
-        self.query[(key, '>')] = (value, lambda a, b: a > b)
+        self.query[(key, '>')] = (value, Cmper.cmp_gt)
 
     def filter_gte(self, key, value):
-        self.query[(key, ">=")] = (value, lambda a, b: a >= b)
+        self.query[(key, ">=")] = (value, Cmper.cmp_gte)
 
     def filter_lt(self, key, value):
-        self.query[(key, "<")] = (value, lambda a, b: a < b)
+        self.query[(key, "<")] = (value, Cmper.cmp_lt)
 
     def filter_lte(self, key, value):
-        self.query[(key, "<=")] = (value, lambda a, b: a <= b)
+        self.query[(key, "<=")] = (value, Cmper.cmp_lte)
 
     def filter_eq(self, key, value):
-        self.query[(key, "==")] = (value, lambda a, b: a == b)
+        self.query[(key, "==")] = (value, Cmper.cmp_eq)
 
     def filter_ne(self, key, value):
-        self.query[(key, "!=")] = (value, lambda a, b: a != b)
+        self.query[(key, "!=")] = (value, Cmper.cmp_ne)
 
     def filter_in(self, key, value):
-        self.query[(key, "in")] = (value, lambda a, b: a in b)
+        try:
+            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, Cmper.cmp_in)
+        except:
+            self.query[(key, "in")] = (value, Cmper.cmp_in)
 
     def commit(self):
         csv_file = self.db.ensure_open_file(self.name)
         csv_file.fields = self.fields
         datas = []
         for data in csv_file.datas:
             succed = True
@@ -234,33 +237,36 @@
 
 
 class CsvDeleteBuilder(DeleteBuilder):
     def __init__(self, *args, **kwargs):
         super(CsvDeleteBuilder, self).__init__(*args, **kwargs)
 
     def filter_gt(self, key, value):
-        self.query[(key, '>')] = (value, lambda a, b: a > b)
+        self.query[(key, '>')] = (value, Cmper.cmp_gt)
 
     def filter_gte(self, key, value):
-        self.query[(key, ">=")] = (value, lambda a, b: a >= b)
+        self.query[(key, ">=")] = (value, Cmper.cmp_gte)
 
     def filter_lt(self, key, value):
-        self.query[(key, "<")] = (value, lambda a, b: a < b)
+        self.query[(key, "<")] = (value, Cmper.cmp_lt)
 
     def filter_lte(self, key, value):
-        self.query[(key, "<=")] = (value, lambda a, b: a <= b)
+        self.query[(key, "<=")] = (value, Cmper.cmp_lte)
 
     def filter_eq(self, key, value):
-        self.query[(key, "==")] = (value, lambda a, b: a == b)
+        self.query[(key, "==")] = (value, Cmper.cmp_eq)
 
     def filter_ne(self, key, value):
-        self.query[(key, "!=")] = (value, lambda a, b: a != b)
+        self.query[(key, "!=")] = (value, Cmper.cmp_ne)
 
     def filter_in(self, key, value):
-        self.query[(key, "in")] = (value, lambda a, b: a in b)
+        try:
+            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, Cmper.cmp_in)
+        except:
+            self.query[(key, "in")] = (value, Cmper.cmp_in)
 
     def commit(self):
         csv_file = self.db.ensure_open_file(self.name)
         datas = []
         for data in csv_file.datas:
             succed = True
             for (key, exp), (value, cmp) in self.query.items():
```

### Comparing `syncany-0.2.8/syncany/database/database.py` & `syncany-0.2.9/syncany/database/database.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,145 @@
 # -*- coding: utf-8 -*-
 # 18/8/6
 # create by: snower
 
 import time
+import datetime
 from collections import deque
 import threading
+from ..utils import parse_datetime, parse_date, parse_time, get_timezone
+
+
+class Cmper(object):
+    @classmethod
+    def ensure_value_type(cls, a, b):
+        if isinstance(a, datetime.date):
+            if isinstance(a, datetime.datetime):
+                if isinstance(b, datetime.date):
+                    return a, datetime.datetime(b.year, b.month, b.day, tzinfo=get_timezone())
+                if isinstance(b, datetime.time):
+                    now = datetime.datetime.now()
+                    return a, datetime.datetime(now.year, now.month, now.day, b.hour, b.minute, b.second,
+                                                b.microsecond, tzinfo=get_timezone())
+                try:
+                    return a, parse_datetime(b, None, get_timezone())
+                except:
+                    return a, None
+            if isinstance(b, datetime.datetime):
+                return a, datetime.date(b.year, b.month, b.day)
+            try:
+                return a, parse_date(b, None, get_timezone())
+            except:
+                return a, None
+        if isinstance(a, datetime.time):
+            if isinstance(b, datetime.datetime):
+                return datetime.time(b.hour, b.minute, b.second, b.microsecond)
+            try:
+                return a, parse_time(b, None, get_timezone())
+            except:
+                return a, None
+        if isinstance(a, int):
+            try:
+                return a, int(b)
+            except ValueError:
+                return a, 0
+        if isinstance(a, float):
+            try:
+                return a, float(b)
+            except ValueError:
+                return a, 0.0
+        try:
+            return a, type(a)(b)
+        except:
+            return a, None
+
+    @classmethod
+    def cmp_gt(cls, a, b):
+        try:
+            return a > b
+        except TypeError:
+            if a is None:
+                return False
+            if b is None:
+                return True
+            a, b = cls.ensure_value_type(a, b)
+            if b is None:
+                return True
+            return a > b
+
+    @classmethod
+    def cmp_gte(cls, a, b):
+        try:
+            return a >= b
+        except TypeError:
+            if a is None:
+                return True if b is None else False
+            if b is None:
+                return True
+            a, b = cls.ensure_value_type(a, b)
+            if b is None:
+                return True
+            return a >= b
+
+    @classmethod
+    def cmp_lt(cls, a, b):
+        try:
+            return a < b
+        except TypeError:
+            if a is None:
+                return False if b is None else True
+            if b is None:
+                return False
+            a, b = cls.ensure_value_type(a, b)
+            if b is None:
+                return False
+            return a < b
+
+    @classmethod
+    def cmp_lte(cls, a, b):
+        try:
+            return a <= b
+        except TypeError:
+            if a is None:
+                return True
+            if b is None:
+                return True
+            a, b = cls.ensure_value_type(a, b)
+            if b is None:
+                return False
+            return a <= b
+
+    @classmethod
+    def cmp_eq(cls, a, b):
+        if a == b:
+            return True
+        if a is None or b is None:
+            return False
+        a, b = cls.ensure_value_type(a, b)
+        if b is None:
+            return False
+        return a == b
+
+    @classmethod
+    def cmp_ne(cls, a, b):
+        if a == b:
+            return False
+        if a is None or b is None:
+            return True
+        a, b = cls.ensure_value_type(a, b)
+        if b is None:
+            return True
+        return a != b
+
+    @classmethod
+    def cmp_in(cls, a, b):
+        if b is None:
+            return False
+        return a in b
+
 
 
 class QueryBuilder(object):
     def __init__(self, db, name, primary_keys, fields):
         self.db = db
         self.name = name
         self.primary_keys = primary_keys or []
```

### Comparing `syncany-0.2.8/syncany/database/elasticsearch.py` & `syncany-0.2.9/syncany/database/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/database/excel.py` & `syncany-0.2.9/syncany/database/excel.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,48 +8,48 @@
 try:
     from bson.objectid import ObjectId
 except ImportError:
     ObjectId = None
 from ..utils import get_timezone, human_repr_object, sorted_by_keys
 from ..taskers.context import TaskerContext
 from ..taskers.iterator import TaskerDataIterator
-from .database import QueryBuilder, InsertBuilder, UpdateBuilder, DeleteBuilder, DataBase
+from .database import Cmper, QueryBuilder, InsertBuilder, UpdateBuilder, DeleteBuilder, DataBase
 
 
 class ExeclFileNotFound(Exception):
     pass
 
 
 class ExeclQueryBuilder(QueryBuilder):
     def __init__(self, *args, **kwargs):
         super(ExeclQueryBuilder, self).__init__(*args, **kwargs)
 
     def filter_gt(self, key, value):
-        self.query[(key, '>')] = (value, lambda a, b: a > b)
+        self.query[(key, '>')] = (value, Cmper.cmp_gt)
 
     def filter_gte(self, key, value):
-        self.query[(key, ">=")] = (value, lambda a, b: a >= b)
+        self.query[(key, ">=")] = (value, Cmper.cmp_gte)
 
     def filter_lt(self, key, value):
-        self.query[(key, "<")] = (value, lambda a, b: a < b)
+        self.query[(key, "<")] = (value, Cmper.cmp_lt)
 
     def filter_lte(self, key, value):
-        self.query[(key, "<=")] = (value, lambda a, b: a <= b)
+        self.query[(key, "<=")] = (value, Cmper.cmp_lte)
 
     def filter_eq(self, key, value):
-        self.query[(key, "==")] = (value, lambda a, b: a == b)
+        self.query[(key, "==")] = (value, Cmper.cmp_eq)
 
     def filter_ne(self, key, value):
-        self.query[(key, "!=")] = (value, lambda a, b: a != b)
+        self.query[(key, "!=")] = (value, Cmper.cmp_ne)
 
     def filter_in(self, key, value):
         try:
-            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, lambda a, b: a in b)
+            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, Cmper.cmp_in)
         except:
-            self.query[(key, "in")] = (value, lambda a, b: a in b)
+            self.query[(key, "in")] = (value, Cmper.cmp_in)
 
     def filter_limit(self, count, start=None):
         if not start:
             self.limit = (0, count)
         else:
             self.limit = (start, start + count)
 
@@ -125,33 +125,36 @@
 
 
 class ExeclUpdateBuilder(UpdateBuilder):
     def __init__(self, *args, **kwargs):
         super(ExeclUpdateBuilder, self).__init__(*args, **kwargs)
 
     def filter_gt(self, key, value):
-        self.query[(key, '>')] = (value, lambda a, b: a > b)
+        self.query[(key, '>')] = (value, Cmper.cmp_gt)
 
     def filter_gte(self, key, value):
-        self.query[(key, ">=")] = (value, lambda a, b: a >= b)
+        self.query[(key, ">=")] = (value, Cmper.cmp_gte)
 
     def filter_lt(self, key, value):
-        self.query[(key, "<")] = (value, lambda a, b: a < b)
+        self.query[(key, "<")] = (value, Cmper.cmp_lt)
 
     def filter_lte(self, key, value):
-        self.query[(key, "<=")] = (value, lambda a, b: a <= b)
+        self.query[(key, "<=")] = (value, Cmper.cmp_lte)
 
     def filter_eq(self, key, value):
-        self.query[(key, "==")] = (value, lambda a, b: a == b)
+        self.query[(key, "==")] = (value, Cmper.cmp_eq)
 
     def filter_ne(self, key, value):
-        self.query[(key, "!=")] = (value, lambda a, b: a != b)
+        self.query[(key, "!=")] = (value, Cmper.cmp_ne)
 
     def filter_in(self, key, value):
-        self.query[(key, "in")] = (value, lambda a, b: a in b)
+        try:
+            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, Cmper.cmp_in)
+        except:
+            self.query[(key, "in")] = (value, Cmper.cmp_in)
 
     def commit(self):
         execl_sheet = self.db.ensure_open_file(self.name)
         execl_sheet.sheet_descriptions = self.fields
         datas = []
         for data in execl_sheet.sheet_datas:
             succed = True
@@ -182,33 +185,36 @@
 
 
 class ExeclDeleteBuilder(DeleteBuilder):
     def __init__(self, *args, **kwargs):
         super(ExeclDeleteBuilder, self).__init__(*args, **kwargs)
 
     def filter_gt(self, key, value):
-        self.query[(key, '>')] = (value, lambda a, b: a > b)
+        self.query[(key, '>')] = (value, Cmper.cmp_gt)
 
     def filter_gte(self, key, value):
-        self.query[(key, ">=")] = (value, lambda a, b: a >= b)
+        self.query[(key, ">=")] = (value, Cmper.cmp_gte)
 
     def filter_lt(self, key, value):
-        self.query[(key, "<")] = (value, lambda a, b: a < b)
+        self.query[(key, "<")] = (value, Cmper.cmp_lt)
 
     def filter_lte(self, key, value):
-        self.query[(key, "<=")] = (value, lambda a, b: a <= b)
+        self.query[(key, "<=")] = (value, Cmper.cmp_lte)
 
     def filter_eq(self, key, value):
-        self.query[(key, "==")] = (value, lambda a, b: a == b)
+        self.query[(key, "==")] = (value, Cmper.cmp_eq)
 
     def filter_ne(self, key, value):
-        self.query[(key, "!=")] = (value, lambda a, b: a != b)
+        self.query[(key, "!=")] = (value, Cmper.cmp_ne)
 
     def filter_in(self, key, value):
-        self.query[(key, "in")] = (value, lambda a, b: a in b)
+        try:
+            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, Cmper.cmp_in)
+        except:
+            self.query[(key, "in")] = (value, Cmper.cmp_in)
 
     def commit(self):
         execl_sheet = self.db.ensure_open_file(self.name)
         datas = []
         for data in execl_sheet.sheet_datas:
             succed = True
             for (key, exp), (value, cmp) in self.query.items():
```

### Comparing `syncany-0.2.8/syncany/database/http.py` & `syncany-0.2.9/syncany/database/http.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/database/influxdb.py` & `syncany-0.2.9/syncany/database/influxdb.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/database/json.py` & `syncany-0.2.9/syncany/database/json.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,48 +4,48 @@
 
 import os
 import json
 import datetime
 from ..utils import human_repr_object, sorted_by_keys
 from ..taskers.context import TaskerContext
 from ..taskers.iterator import TaskerDataIterator
-from .database import QueryBuilder, InsertBuilder, UpdateBuilder, DeleteBuilder, DataBase
+from .database import Cmper, QueryBuilder, InsertBuilder, UpdateBuilder, DeleteBuilder, DataBase
 
 
 class JsonFileNotFound(Exception):
     pass
 
 
 class JsonQueryBuilder(QueryBuilder):
     def __init__(self, *args, **kwargs):
         super(JsonQueryBuilder, self).__init__(*args, **kwargs)
 
     def filter_gt(self, key, value):
-        self.query[(key, '>')] = (value, lambda a, b: a > b)
+        self.query[(key, '>')] = (value, Cmper.cmp_gt)
 
     def filter_gte(self, key, value):
-        self.query[(key, ">=")] = (value, lambda a, b: a >= b)
+        self.query[(key, ">=")] = (value, Cmper.cmp_gte)
 
     def filter_lt(self, key, value):
-        self.query[(key, "<")] = (value, lambda a, b: a < b)
+        self.query[(key, "<")] = (value, Cmper.cmp_lt)
 
     def filter_lte(self, key, value):
-        self.query[(key, "<=")] = (value, lambda a, b: a <= b)
+        self.query[(key, "<=")] = (value, Cmper.cmp_lte)
 
     def filter_eq(self, key, value):
-        self.query[(key, "==")] = (value, lambda a, b: a == b)
+        self.query[(key, "==")] = (value, Cmper.cmp_eq)
 
     def filter_ne(self, key, value):
-        self.query[(key, "!=")] = (value, lambda a, b: a != b)
+        self.query[(key, "!=")] = (value, Cmper.cmp_ne)
 
     def filter_in(self, key, value):
         try:
-            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, lambda a, b: a in b)
+            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, Cmper.cmp_in)
         except:
-            self.query[(key, "in")] = (value, lambda a, b: a in b)
+            self.query[(key, "in")] = (value, Cmper.cmp_in)
 
     def filter_limit(self, count, start=None):
         if not start:
             self.limit = (0, count)
         else:
             self.limit = (start, start + count)
 
@@ -120,33 +120,36 @@
 
 
 class JsonUpdateBuilder(UpdateBuilder):
     def __init__(self, *args, **kwargs):
         super(JsonUpdateBuilder, self).__init__(*args, **kwargs)
 
     def filter_gt(self, key, value):
-        self.query[(key, '>')] = (value, lambda a, b: a > b)
+        self.query[(key, '>')] = (value, Cmper.cmp_gt)
 
     def filter_gte(self, key, value):
-        self.query[(key, ">=")] = (value, lambda a, b: a >= b)
+        self.query[(key, ">=")] = (value, Cmper.cmp_gte)
 
     def filter_lt(self, key, value):
-        self.query[(key, "<")] = (value, lambda a, b: a < b)
+        self.query[(key, "<")] = (value, Cmper.cmp_lt)
 
     def filter_lte(self, key, value):
-        self.query[(key, "<=")] = (value, lambda a, b: a <= b)
+        self.query[(key, "<=")] = (value, Cmper.cmp_lte)
 
     def filter_eq(self, key, value):
-        self.query[(key, "==")] = (value, lambda a, b: a == b)
+        self.query[(key, "==")] = (value, Cmper.cmp_eq)
 
     def filter_ne(self, key, value):
-        self.query[(key, "!=")] = (value, lambda a, b: a != b)
+        self.query[(key, "!=")] = (value, Cmper.cmp_ne)
 
     def filter_in(self, key, value):
-        self.query[(key, "in")] = (value, lambda a, b: a in b)
+        try:
+            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, Cmper.cmp_in)
+        except:
+            self.query[(key, "in")] = (value, Cmper.cmp_in)
 
     def commit(self):
         json_file = self.db.ensure_open_file(self.name)
         datas = []
         for data in json_file.datas:
             succed = True
             for (key, exp), (value, cmp) in self.query.items():
@@ -176,33 +179,36 @@
 
 
 class JsonDeleteBuilder(DeleteBuilder):
     def __init__(self, *args, **kwargs):
         super(JsonDeleteBuilder, self).__init__(*args, **kwargs)
 
     def filter_gt(self, key, value):
-        self.query[(key, '>')] = (value, lambda a, b: a > b)
+        self.query[(key, '>')] = (value, Cmper.cmp_gt)
 
     def filter_gte(self, key, value):
-        self.query[(key, ">=")] = (value, lambda a, b: a >= b)
+        self.query[(key, ">=")] = (value, Cmper.cmp_gte)
 
     def filter_lt(self, key, value):
-        self.query[(key, "<")] = (value, lambda a, b: a < b)
+        self.query[(key, "<")] = (value, Cmper.cmp_lt)
 
     def filter_lte(self, key, value):
-        self.query[(key, "<=")] = (value, lambda a, b: a <= b)
+        self.query[(key, "<=")] = (value, Cmper.cmp_lte)
 
     def filter_eq(self, key, value):
-        self.query[(key, "==")] = (value, lambda a, b: a == b)
+        self.query[(key, "==")] = (value, Cmper.cmp_eq)
 
     def filter_ne(self, key, value):
-        self.query[(key, "!=")] = (value, lambda a, b: a != b)
+        self.query[(key, "!=")] = (value, Cmper.cmp_ne)
 
     def filter_in(self, key, value):
-        self.query[(key, "in")] = (value, lambda a, b: a in b)
+        try:
+            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, Cmper.cmp_in)
+        except:
+            self.query[(key, "in")] = (value, Cmper.cmp_in)
 
     def commit(self):
         json_file = self.db.ensure_open_file(self.name)
         datas = []
         for data in json_file.datas:
             succed = True
             for (key, exp), (value, cmp) in self.query.items():
```

### Comparing `syncany-0.2.8/syncany/database/memory.py` & `syncany-0.2.9/syncany/database/memory.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,44 +2,44 @@
 # 2020/7/6
 # create by: snower
 
 import time
 from ..utils import human_repr_object, sorted_by_keys
 from ..taskers.context import TaskerContext
 from ..taskers.iterator import TaskerDataIterator
-from .database import QueryBuilder, InsertBuilder, UpdateBuilder, DeleteBuilder, CacheBuilder, DataBase, DatabaseFactory
+from .database import Cmper, QueryBuilder, InsertBuilder, UpdateBuilder, DeleteBuilder, CacheBuilder, DataBase, DatabaseFactory
 
 
 class MemoryQueryBuilder(QueryBuilder):
     def __init__(self, *args, **kwargs):
         super(MemoryQueryBuilder, self).__init__(*args, **kwargs)
 
     def filter_gt(self, key, value):
-        self.query[(key, '>')] = (value, lambda a, b: a > b)
+        self.query[(key, '>')] = (value, Cmper.cmp_gt)
 
     def filter_gte(self, key, value):
-        self.query[(key, ">=")] = (value, lambda a, b: a >= b)
+        self.query[(key, ">=")] = (value, Cmper.cmp_gte)
 
     def filter_lt(self, key, value):
-        self.query[(key, "<")] = (value, lambda a, b: a < b)
+        self.query[(key, "<")] = (value, Cmper.cmp_lt)
 
     def filter_lte(self, key, value):
-        self.query[(key, "<=")] = (value, lambda a, b: a <= b)
+        self.query[(key, "<=")] = (value, Cmper.cmp_lte)
 
     def filter_eq(self, key, value):
-        self.query[(key, "==")] = (value, lambda a, b: a == b)
+        self.query[(key, "==")] = (value, Cmper.cmp_eq)
 
     def filter_ne(self, key, value):
-        self.query[(key, "!=")] = (value, lambda a, b: a != b)
+        self.query[(key, "!=")] = (value, Cmper.cmp_ne)
 
     def filter_in(self, key, value):
         try:
-            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, lambda a, b: a in b)
+            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, Cmper.cmp_in)
         except:
-            self.query[(key, "in")] = (value, lambda a, b: a in b)
+            self.query[(key, "in")] = (value, Cmper.cmp_in)
 
     def filter_limit(self, count, start=None):
         if not start:
             self.limit = (0, count)
         else:
             self.limit = (start, start + count)
 
@@ -131,33 +131,36 @@
 
 
 class MemoryUpdateBuilder(UpdateBuilder):
     def __init__(self, *args, **kwargs):
         super(MemoryUpdateBuilder, self).__init__(*args, **kwargs)
 
     def filter_gt(self, key, value):
-        self.query[(key, '>')] = (value, lambda a, b: a > b)
+        self.query[(key, '>')] = (value, Cmper.cmp_gt)
 
     def filter_gte(self, key, value):
-        self.query[(key, ">=")] = (value, lambda a, b: a >= b)
+        self.query[(key, ">=")] = (value, Cmper.cmp_gte)
 
     def filter_lt(self, key, value):
-        self.query[(key, "<")] = (value, lambda a, b: a < b)
+        self.query[(key, "<")] = (value, Cmper.cmp_lt)
 
     def filter_lte(self, key, value):
-        self.query[(key, "<=")] = (value, lambda a, b: a <= b)
+        self.query[(key, "<=")] = (value, Cmper.cmp_lte)
 
     def filter_eq(self, key, value):
-        self.query[(key, "==")] = (value, lambda a, b: a == b)
+        self.query[(key, "==")] = (value, Cmper.cmp_eq)
 
     def filter_ne(self, key, value):
-        self.query[(key, "!=")] = (value, lambda a, b: a != b)
+        self.query[(key, "!=")] = (value, Cmper.cmp_ne)
 
     def filter_in(self, key, value):
-        self.query[(key, "in")] = (value, lambda a, b: a in b)
+        try:
+            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, Cmper.cmp_in)
+        except:
+            self.query[(key, "in")] = (value, Cmper.cmp_in)
 
     def commit(self):
         if ".--" in self.name:
             cache_keys = self.name.split(".")
             if len(cache_keys) == 2 or cache_keys[1][:2] == "--":
                 return
 
@@ -190,33 +193,36 @@
 
 
 class MemoryDeleteBuilder(DeleteBuilder):
     def __init__(self, *args, **kwargs):
         super(MemoryDeleteBuilder, self).__init__(*args, **kwargs)
 
     def filter_gt(self, key, value):
-        self.query[(key, '>')] = (value, lambda a, b: a > b)
+        self.query[(key, '>')] = (value, Cmper.cmp_gt)
 
     def filter_gte(self, key, value):
-        self.query[(key, ">=")] = (value, lambda a, b: a >= b)
+        self.query[(key, ">=")] = (value, Cmper.cmp_gte)
 
     def filter_lt(self, key, value):
-        self.query[(key, "<")] = (value, lambda a, b: a < b)
+        self.query[(key, "<")] = (value, Cmper.cmp_lt)
 
     def filter_lte(self, key, value):
-        self.query[(key, "<=")] = (value, lambda a, b: a <= b)
+        self.query[(key, "<=")] = (value, Cmper.cmp_lte)
 
     def filter_eq(self, key, value):
-        self.query[(key, "==")] = (value, lambda a, b: a == b)
+        self.query[(key, "==")] = (value, Cmper.cmp_eq)
 
     def filter_ne(self, key, value):
-        self.query[(key, "!=")] = (value, lambda a, b: a != b)
+        self.query[(key, "!=")] = (value, Cmper.cmp_ne)
 
     def filter_in(self, key, value):
-        self.query[(key, "in")] = (value, lambda a, b: a in b)
+        try:
+            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, Cmper.cmp_in)
+        except:
+            self.query[(key, "in")] = (value, Cmper.cmp_in)
 
     def commit(self):
         if ".--" in self.name:
             cache_keys = self.name.split(".")
             if len(cache_keys) == 2 or cache_keys[1][:2] == "--":
                 return
```

### Comparing `syncany-0.2.8/syncany/database/mongodb.py` & `syncany-0.2.9/syncany/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/database/mysql.py` & `syncany-0.2.9/syncany/database/mysql.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/database/postgresql.py` & `syncany-0.2.9/syncany/database/postgresql.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/database/redis.py` & `syncany-0.2.9/syncany/database/redis.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # create by: snower
 
 import pickle
 import json
 from ..utils import human_repr_object, sorted_by_keys
 from ..taskers.context import TaskerContext
 from ..taskers.iterator import TaskerDataIterator
-from .database import QueryBuilder, InsertBuilder, UpdateBuilder, DeleteBuilder, CacheBuilder, DataBase, DatabaseFactory
+from .database import Cmper, QueryBuilder, InsertBuilder, UpdateBuilder, DeleteBuilder, CacheBuilder, DataBase, DatabaseFactory
 
 
 class StringSerialize(object):
     def loads(self, data):
         return str(data)
 
     def dumps(self, value):
@@ -156,36 +156,36 @@
 
 class RedisQueryBuilder(QueryBuilder, RedisCommand):
     def __init__(self, *args, **kwargs):
         QueryBuilder.__init__(self, *args, **kwargs)
         RedisCommand.__init__(self, self.db.serialize, self.db.base_prefix, self.name)
 
     def filter_gt(self, key, value):
-        self.query[(key, '>')] = (value, lambda a, b: a > b)
+        self.query[(key, '>')] = (value, Cmper.cmp_gt)
 
     def filter_gte(self, key, value):
-        self.query[(key, ">=")] = (value, lambda a, b: a >= b)
+        self.query[(key, ">=")] = (value, Cmper.cmp_gte)
 
     def filter_lt(self, key, value):
-        self.query[(key, "<")] = (value, lambda a, b: a < b)
+        self.query[(key, "<")] = (value, Cmper.cmp_lt)
 
     def filter_lte(self, key, value):
-        self.query[(key, "<=")] = (value, lambda a, b: a <= b)
+        self.query[(key, "<=")] = (value, Cmper.cmp_lte)
 
     def filter_eq(self, key, value):
-        self.query[(key, "==")] = (value, lambda a, b: a == b)
+        self.query[(key, "==")] = (value, Cmper.cmp_eq)
 
     def filter_ne(self, key, value):
-        self.query[(key, "!=")] = (value, lambda a, b: a != b)
+        self.query[(key, "!=")] = (value, Cmper.cmp_ne)
 
     def filter_in(self, key, value):
         try:
-            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, lambda a, b: a in b)
+            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, Cmper.cmp_in)
         except:
-            self.query[(key, "in")] = (value, lambda a, b: a in b)
+            self.query[(key, "in")] = (value, Cmper.cmp_in)
 
     def filter_limit(self, count, start=None):
         if not start:
             self.limit = (0, count)
         else:
             self.limit = (start, start + count)
 
@@ -266,33 +266,36 @@
 
 class RedisUpdateBuilder(UpdateBuilder, RedisCommand):
     def __init__(self, *args, **kwargs):
         UpdateBuilder.__init__(self, *args, **kwargs)
         RedisCommand.__init__(self, self.db.serialize, self.db.base_prefix, self.name)
 
     def filter_gt(self, key, value):
-        self.query[(key, '>')] = (value, lambda a, b: a > b)
+        self.query[(key, '>')] = (value, Cmper.cmp_gt)
 
     def filter_gte(self, key, value):
-        self.query[(key, ">=")] = (value, lambda a, b: a >= b)
+        self.query[(key, ">=")] = (value, Cmper.cmp_gte)
 
     def filter_lt(self, key, value):
-        self.query[(key, "<")] = (value, lambda a, b: a < b)
+        self.query[(key, "<")] = (value, Cmper.cmp_lt)
 
     def filter_lte(self, key, value):
-        self.query[(key, "<=")] = (value, lambda a, b: a <= b)
+        self.query[(key, "<=")] = (value, Cmper.cmp_lte)
 
     def filter_eq(self, key, value):
-        self.query[(key, "==")] = (value, lambda a, b: a == b)
+        self.query[(key, "==")] = (value, Cmper.cmp_eq)
 
     def filter_ne(self, key, value):
-        self.query[(key, "!=")] = (value, lambda a, b: a != b)
+        self.query[(key, "!=")] = (value, Cmper.cmp_ne)
 
     def filter_in(self, key, value):
-        self.query[(key, "in")] = (value, lambda a, b: a in b)
+        try:
+            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, Cmper.cmp_in)
+        except:
+            self.query[(key, "in")] = (value, Cmper.cmp_in)
 
     def commit(self):
         try:
             connection = self.db.ensure_connection()
             datas = []
             for data in self.load_datas(connection):
                 succed = True
@@ -325,33 +328,36 @@
 
 class RedisDeleteBuilder(DeleteBuilder, RedisCommand):
     def __init__(self, *args, **kwargs):
         DeleteBuilder.__init__(self, *args, **kwargs)
         RedisCommand.__init__(self, self.db.serialize, self.db.base_prefix, self.name)
 
     def filter_gt(self, key, value):
-        self.query[(key, '>')] = (value, lambda a, b: a > b)
+        self.query[(key, '>')] = (value, Cmper.cmp_gt)
 
     def filter_gte(self, key, value):
-        self.query[(key, ">=")] = (value, lambda a, b: a >= b)
+        self.query[(key, ">=")] = (value, Cmper.cmp_gte)
 
     def filter_lt(self, key, value):
-        self.query[(key, "<")] = (value, lambda a, b: a < b)
+        self.query[(key, "<")] = (value, Cmper.cmp_lt)
 
     def filter_lte(self, key, value):
-        self.query[(key, "<=")] = (value, lambda a, b: a <= b)
+        self.query[(key, "<=")] = (value, Cmper.cmp_lte)
 
     def filter_eq(self, key, value):
-        self.query[(key, "==")] = (value, lambda a, b: a == b)
+        self.query[(key, "==")] = (value, Cmper.cmp_eq)
 
     def filter_ne(self, key, value):
-        self.query[(key, "!=")] = (value, lambda a, b: a != b)
+        self.query[(key, "!=")] = (value, Cmper.cmp_ne)
 
     def filter_in(self, key, value):
-        self.query[(key, "in")] = (value, lambda a, b: a in b)
+        try:
+            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, Cmper.cmp_in)
+        except:
+            self.query[(key, "in")] = (value, Cmper.cmp_in)
 
     def commit(self):
         try:
             connection = self.db.ensure_connection()
             if not self.query:
                 self.delete_datas(connection)
                 return []
```

### Comparing `syncany-0.2.8/syncany/database/sqlite.py` & `syncany-0.2.9/syncany/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/database/sqlserver.py` & `syncany-0.2.9/syncany/database/sqlserver.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/database/textline.py` & `syncany-0.2.9/syncany/database/textline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding: utf-8 -*-
 # 2020/7/2
 # create by: snower
+
 import datetime
 import os
 import csv
 import json
 from ..utils import print_object, get_rich, human_repr_object, human_format_object, sorted_by_keys
 from ..taskers.context import TaskerContext
 from ..taskers.iterator import TaskerFileIterator
-from .database import QueryBuilder, InsertBuilder, UpdateBuilder, DeleteBuilder, DataBase
+from .database import Cmper, QueryBuilder, InsertBuilder, UpdateBuilder, DeleteBuilder, DataBase
 
 
 class TextLineSpliter(object):
     ESCAPE_CHARS = ['\a', '\b', '\f', '\n', '\r', '\t', '\v', '\\', '\'', '"', '\0']
 
     def __init__(self, sep=' ', escapes=('"', "'"), boundarys=None):
         self.sep = sep
@@ -92,33 +93,36 @@
 
 
 class TextLineQueryBuilder(QueryBuilder):
     def __init__(self, *args, **kwargs):
         super(TextLineQueryBuilder, self).__init__(*args, **kwargs)
 
     def filter_gt(self, key, value):
-        self.query[(key, '>')] = (value, lambda a, b: a > b)
+        self.query[(key, '>')] = (value, Cmper.cmp_gt)
 
     def filter_gte(self, key, value):
-        self.query[(key, ">=")] = (value, lambda a, b: a >= b)
+        self.query[(key, ">=")] = (value, Cmper.cmp_gte)
 
     def filter_lt(self, key, value):
-        self.query[(key, "<")] = (value, lambda a, b: a < b)
+        self.query[(key, "<")] = (value, Cmper.cmp_lt)
 
     def filter_lte(self, key, value):
-        self.query[(key, "<=")] = (value, lambda a, b: a <= b)
+        self.query[(key, "<=")] = (value, Cmper.cmp_lte)
 
     def filter_eq(self, key, value):
-        self.query[(key, "==")] = (value, lambda a, b: a == b)
+        self.query[(key, "==")] = (value, Cmper.cmp_eq)
 
     def filter_ne(self, key, value):
-        self.query[(key, "!=")] = (value, lambda a, b: a != b)
+        self.query[(key, "!=")] = (value, Cmper.cmp_ne)
 
     def filter_in(self, key, value):
-        self.query[(key, "in")] = (value, lambda a, b: a in b)
+        try:
+            self.query[(key, "in")] = (set(value) if isinstance(value, list) else value, Cmper.cmp_in)
+        except:
+            self.query[(key, "in")] = (value, Cmper.cmp_in)
 
     def filter_limit(self, count, start=None):
         if not start:
             self.limit = (0, count)
         else:
             self.limit = (start, start + count)
```

### Comparing `syncany-0.2.8/syncany/errors.py` & `syncany-0.2.9/syncany/errors.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/filters/__init__.py` & `syncany-0.2.9/syncany/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/filters/builtin.py` & `syncany-0.2.9/syncany/filters/builtin.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/hook.py` & `syncany-0.2.9/syncany/hook.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/loaders/__init__.py` & `syncany-0.2.9/syncany/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/loaders/cache.py` & `syncany-0.2.9/syncany/loaders/cache.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/loaders/const.py` & `syncany-0.2.9/syncany/loaders/const.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/loaders/db.py` & `syncany-0.2.9/syncany/loaders/db.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/loaders/db_join.py` & `syncany-0.2.9/syncany/loaders/db_join.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/loaders/db_pull.py` & `syncany-0.2.9/syncany/loaders/db_pull.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/loaders/loader.py` & `syncany-0.2.9/syncany/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/main.py` & `syncany-0.2.9/syncany/main.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/outputers/__init__.py` & `syncany-0.2.9/syncany/outputers/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/outputers/db.py` & `syncany-0.2.9/syncany/outputers/db.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/outputers/db_delete_insert.py` & `syncany-0.2.9/syncany/outputers/db_delete_insert.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/outputers/db_insert.py` & `syncany-0.2.9/syncany/outputers/db_insert.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/outputers/db_update_delete_insert.py` & `syncany-0.2.9/syncany/outputers/db_update_delete_insert.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/outputers/db_update_insert.py` & `syncany-0.2.9/syncany/outputers/db_update_insert.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/outputers/outputer.py` & `syncany-0.2.9/syncany/outputers/outputer.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/taskers/config/__init__.py` & `syncany-0.2.9/syncany/taskers/config/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/taskers/config/http_reader.py` & `syncany-0.2.9/syncany/taskers/config/http_reader.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/taskers/config/yaml_parser.py` & `syncany-0.2.9/syncany/taskers/config/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/taskers/context.py` & `syncany-0.2.9/syncany/taskers/context.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/taskers/core/__init__.py` & `syncany-0.2.9/syncany/taskers/core/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/taskers/core/loader_creater.py` & `syncany-0.2.9/syncany/taskers/core/loader_creater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/taskers/core/outputer_creater.py` & `syncany-0.2.9/syncany/taskers/core/outputer_creater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/taskers/core/states.py` & `syncany-0.2.9/syncany/taskers/core/states.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/taskers/core/valuer_compiler.py` & `syncany-0.2.9/syncany/taskers/core/valuer_compiler.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/taskers/core/valuer_creater.py` & `syncany-0.2.9/syncany/taskers/core/valuer_creater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/taskers/iterator.py` & `syncany-0.2.9/syncany/taskers/iterator.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/taskers/tasker.py` & `syncany-0.2.9/syncany/taskers/tasker.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/utils.py` & `syncany-0.2.9/syncany/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,24 +154,24 @@
         pass
     dt = datetime.datetime.strptime(value, fmt or "%Y-%m-%d")
     return datetime.date(dt.year, dt.month, dt.day)
 
 def parse_time(value, fmt, tz):
     try:
         dt = parse_datetime(value, fmt, tz)
+        if isinstance(dt, datetime.time):
+            return dt
         if isinstance(dt, datetime.datetime):
             if tz != dt.tzinfo:
                 dt = dt.astimezone(tz=tz)
-            return datetime.time(dt.hour, dt.minute, dt.second, dt.microsecond)
-        if isinstance(dt, datetime.time):
-            return datetime.date.today()
+            return datetime.time(dt.hour, dt.minute, dt.second, dt.microsecond, tzinfo=tz)
     except ParserError:
         pass
     dt = datetime.datetime.strptime("2000-01-01 " + value, "%Y-%m-%d " + (fmt or "%H:%M:%S"))
-    return datetime.time(dt.hour, dt.minute, dt.second, dt.microsecond)
+    return datetime.time(dt.hour, dt.minute, dt.second, dt.microsecond, tzinfo=tz)
 
 def get_rich():
     if os.environ.get("USE_RICH", 'true').lower() != "true":
         return None
 
     try:
         import rich
```

### Comparing `syncany-0.2.8/syncany/valuers/__init__.py` & `syncany-0.2.9/syncany/valuers/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/valuers/aggregate.py` & `syncany-0.2.9/syncany/valuers/aggregate.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/valuers/assign.py` & `syncany-0.2.9/syncany/valuers/assign.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/valuers/cache.py` & `syncany-0.2.9/syncany/valuers/cache.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/valuers/calculate.py` & `syncany-0.2.9/syncany/valuers/calculate.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/valuers/call.py` & `syncany-0.2.9/syncany/valuers/call.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/valuers/case.py` & `syncany-0.2.9/syncany/valuers/case.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/valuers/condition.py` & `syncany-0.2.9/syncany/valuers/condition.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/valuers/const.py` & `syncany-0.2.9/syncany/valuers/const.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/valuers/data.py` & `syncany-0.2.9/syncany/valuers/data.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/valuers/db_join.py` & `syncany-0.2.9/syncany/valuers/db_join.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/valuers/db_load.py` & `syncany-0.2.9/syncany/valuers/db_load.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/valuers/function.py` & `syncany-0.2.9/syncany/valuers/function.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/valuers/generator.py` & `syncany-0.2.9/syncany/valuers/generator.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/valuers/inherit.py` & `syncany-0.2.9/syncany/valuers/inherit.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/valuers/let.py` & `syncany-0.2.9/syncany/valuers/let.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/valuers/loop.py` & `syncany-0.2.9/syncany/valuers/loop.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/valuers/make.py` & `syncany-0.2.9/syncany/valuers/make.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/valuers/match.py` & `syncany-0.2.9/syncany/valuers/match.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/valuers/schema.py` & `syncany-0.2.9/syncany/valuers/schema.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/valuers/state.py` & `syncany-0.2.9/syncany/valuers/state.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany/valuers/valuer.py` & `syncany-0.2.9/syncany/valuers/valuer.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.8/syncany.egg-info/PKG-INFO` & `syncany-0.2.9/syncany.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncany
-Version: 0.2.8
+Version: 0.2.9
 Summary: 简单易用的数据同步转换导出框架
 Home-page: https://github.com/snower/syncany
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # syncany
```

### Comparing `syncany-0.2.8/syncany.egg-info/SOURCES.txt` & `syncany-0.2.9/syncany.egg-info/SOURCES.txt`

 * *Files identical despite different names*

