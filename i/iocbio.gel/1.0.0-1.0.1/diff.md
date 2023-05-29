# Comparing `tmp/iocbio.gel-1.0.0.tar.gz` & `tmp/iocbio.gel-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iocbio.gel-1.0.0.tar", last modified: Wed Apr  5 14:11:12 2023, max compression
+gzip compressed data, was "iocbio.gel-1.0.1.tar", last modified: Mon May 29 05:30:41 2023, max compression
```

## Comparing `iocbio.gel-1.0.0.tar` & `iocbio.gel-1.0.1.tar`

### file list

```diff
@@ -1,284 +1,284 @@
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.925061 iocbio.gel-1.0.0/
--rw-r--r--   0 markov    (1000) markov    (1000)      149 2022-10-20 13:58:54.000000 iocbio.gel-1.0.0/.gitignore
--rw-r--r--   0 markov    (1000) markov    (1000)     2286 2023-04-05 13:20:14.000000 iocbio.gel-1.0.0/.gitlab-ci.yml
--rw-r--r--   0 markov    (1000) markov    (1000)      668 2023-03-01 10:05:44.000000 iocbio.gel-1.0.0/AUTHORS.md
--rw-r--r--   0 markov    (1000) markov    (1000)     2016 2023-04-05 14:09:49.000000 iocbio.gel-1.0.0/CHANGELOG.md
--rw-r--r--   0 markov    (1000) markov    (1000)     1639 2023-03-29 06:51:40.000000 iocbio.gel-1.0.0/CONTRIBUTING.md
--rw-r--r--   0 markov    (1000) markov    (1000)    32198 2023-02-08 15:18:05.000000 iocbio.gel-1.0.0/LICENSE.md
--rw-r--r--   0 markov    (1000) markov    (1000)     1791 2023-04-05 14:11:12.925061 iocbio.gel-1.0.0/PKG-INFO
--rw-r--r--   0 markov    (1000) markov    (1000)     1231 2022-10-20 13:58:54.000000 iocbio.gel-1.0.0/README.md
--rw-r--r--   0 markov    (1000) markov    (1000)     1257 2022-11-17 06:54:58.000000 iocbio.gel-1.0.0/RELEASING.md
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.895060 iocbio.gel-1.0.0/docs/
--rw-r--r--   0 markov    (1000) markov    (1000)      590 2022-10-20 13:58:54.000000 iocbio.gel-1.0.0/docs/development.md
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.898393 iocbio.gel-1.0.0/docs/img/
--rw-r--r--   0 markov    (1000) markov    (1000)   123881 2023-04-05 12:49:25.000000 iocbio.gel-1.0.0/docs/img/curved_lane.png
--rw-r--r--   0 markov    (1000) markov    (1000)   140271 2023-04-05 12:39:19.000000 iocbio.gel-1.0.0/docs/img/lanes.png
--rw-r--r--   0 markov    (1000) markov    (1000)   141782 2023-04-05 12:46:11.000000 iocbio.gel-1.0.0/docs/img/measurement_lanes.png
--rw-r--r--   0 markov    (1000) markov    (1000)    93091 2023-04-05 12:38:33.000000 iocbio.gel-1.0.0/docs/img/projects.png
--rw-r--r--   0 markov    (1000) markov    (1000)    60215 2023-04-05 12:37:47.000000 iocbio.gel-1.0.0/docs/img/types_and_edit_mode.png
--rw-r--r--   0 markov    (1000) markov    (1000)     2019 2023-04-05 14:07:55.000000 iocbio.gel-1.0.0/docs/index.md
--rw-r--r--   0 markov    (1000) markov    (1000)     4865 2023-03-27 13:56:58.000000 iocbio.gel-1.0.0/docs/install.md
--rw-r--r--   0 markov    (1000) markov    (1000)    19234 2023-04-05 14:09:32.000000 iocbio.gel-1.0.0/docs/users.md
--rw-r--r--   0 markov    (1000) markov    (1000)      790 2022-10-20 13:58:54.000000 iocbio.gel-1.0.0/install.ps1
--rwxr-xr-x   0 markov    (1000) markov    (1000)      597 2022-10-20 13:58:54.000000 iocbio.gel-1.0.0/install.sh
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.898393 iocbio.gel-1.0.0/iocbio/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-08-03 18:28:50.000000 iocbio.gel-1.0.0/iocbio/__init__.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.898393 iocbio.gel-1.0.0/iocbio/gel/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.0/iocbio/gel/__init__.py
--rw-r--r--   0 markov    (1000) markov    (1000)     7005 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/app.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.898393 iocbio.gel-1.0.0/iocbio/gel/application/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.0/iocbio/gel/application/__init__.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.898393 iocbio.gel-1.0.0/iocbio/gel/application/application_state/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.0/iocbio/gel/application/application_state/__init__.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2341 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/application/application_state/context.py
--rw-r--r--   0 markov    (1000) markov    (1000)      362 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/application/application_state/mode.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1785 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/application/application_state/state.py
--rw-r--r--   0 markov    (1000) markov    (1000)    19495 2023-03-29 06:51:40.000000 iocbio.gel-1.0.0/iocbio/gel/application/container.py
--rw-r--r--   0 markov    (1000) markov    (1000)      950 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/application/event_consumer.py
--rw-r--r--   0 markov    (1000) markov    (1000)     3443 2023-03-20 14:26:15.000000 iocbio.gel-1.0.0/iocbio/gel/application/event_registry.py
--rw-r--r--   0 markov    (1000) markov    (1000)      724 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/application/file_digest.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.901727 iocbio.gel-1.0.0/iocbio/gel/application/image/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-07-01 16:47:54.000000 iocbio.gel-1.0.0/iocbio/gel/application/image/__init__.py
--rw-r--r--   0 markov    (1000) markov    (1000)      733 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/application/image/background_method.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1368 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/application/image/image.py
--rw-r--r--   0 markov    (1000) markov    (1000)      301 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/application/image/image_source.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2527 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/application/image/image_source_setup.py
--rw-r--r--   0 markov    (1000) markov    (1000)      260 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/application/image/image_state.py
--rw-r--r--   0 markov    (1000) markov    (1000)     4025 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/application/image/omero_client.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1929 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/application/image/processing_cache.py
--rw-r--r--   0 markov    (1000) markov    (1000)      640 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/application/image/region.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1015 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/application/image/repository_backend.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1215 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/application/image/repository_backend_local.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2593 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/application/image/repository_backend_omero.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1026 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/application/number_list.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1220 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/application/settings_proxy.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.901727 iocbio.gel-1.0.0/iocbio/gel/application/thread/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-07-14 08:43:25.000000 iocbio.gel-1.0.0/iocbio/gel/application/thread/__init__.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1011 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/application/thread/fetch_image_from_omero.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1568 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/application/thread/job.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1636 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/application/thread/load_image_preview.py
--rw-r--r--   0 markov    (1000) markov    (1000)      915 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/application/thread/pool_worker.py
--rw-r--r--   0 markov    (1000) markov    (1000)     3992 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/application/thread/rolling_ball.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1500 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/application/thread/sequential_worker.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2211 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/application/thread/thread_pool.py
--rw-r--r--   0 markov    (1000) markov    (1000)      542 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/application/thread/worker.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.905060 iocbio.gel-1.0.0/iocbio/gel/command/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.0/iocbio/gel/command/__init__.py
--rw-r--r--   0 markov    (1000) markov    (1000)      507 2023-03-01 10:12:11.000000 iocbio.gel-1.0.0/iocbio/gel/command/command.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1192 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/command/command_set.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1615 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/command/create_entity.py
--rw-r--r--   0 markov    (1000) markov    (1000)     3078 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/command/delete_collector.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1611 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/command/delete_entity.py
--rw-r--r--   0 markov    (1000) markov    (1000)     3029 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/command/history_manager.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2387 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/command/project_delete_collector.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1082 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/command/transaction_set.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1292 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/command/update_entity.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2501 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/command/update_many_relationship.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1357 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/command/update_project.py
--rw-r--r--   0 markov    (1000) markov    (1000)      163 2023-04-05 13:40:38.000000 iocbio.gel-1.0.0/iocbio/gel/const.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.905060 iocbio.gel-1.0.0/iocbio/gel/db/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.0/iocbio/gel/db/__init__.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.905060 iocbio.gel-1.0.0/iocbio/gel/db/alembic/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.0/iocbio/gel/db/alembic/__init__.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2427 2022-06-28 08:47:54.000000 iocbio.gel-1.0.0/iocbio/gel/db/alembic/alembic.ini
--rw-r--r--   0 markov    (1000) markov    (1000)     2770 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/db/alembic/env.py
--rw-r--r--   0 markov    (1000) markov    (1000)      352 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/db/alembic/execute_sqlfile.py
--rw-r--r--   0 markov    (1000) markov    (1000)      495 2022-06-28 06:13:47.000000 iocbio.gel-1.0.0/iocbio/gel/db/alembic/script.py.mako
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.905060 iocbio.gel-1.0.0/iocbio/gel/db/alembic/versions/
--rw-r--r--   0 markov    (1000) markov    (1000)      704 2023-03-29 06:51:40.000000 iocbio.gel-1.0.0/iocbio/gel/db/alembic/versions/8b8ae59755af_synced_lane_widths.py
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.0/iocbio/gel/db/alembic/versions/__init__.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1341 2022-10-11 07:06:04.000000 iocbio.gel-1.0.0/iocbio/gel/db/alembic/versions/create_views_set_1.sql
--rw-r--r--   0 markov    (1000) markov    (1000)      519 2023-03-29 06:51:40.000000 iocbio.gel-1.0.0/iocbio/gel/db/alembic/versions/d8d292a431fe_allow_to_sync_measurement_rois.py
--rw-r--r--   0 markov    (1000) markov    (1000)      175 2022-08-23 14:17:34.000000 iocbio.gel-1.0.0/iocbio/gel/db/alembic/versions/drop_views_set_1.sql
--rw-r--r--   0 markov    (1000) markov    (1000)      813 2023-03-29 06:51:40.000000 iocbio.gel-1.0.0/iocbio/gel/db/alembic/versions/e78898a9c9f1_change_transfer_to_ref_time.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1259 2023-03-29 06:51:40.000000 iocbio.gel-1.0.0/iocbio/gel/db/alembic/versions/fbf8b6944c61_limit_protein_to_non_negative_value.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2274 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/db/alembic/versions/fd339f2a6eb4_projects.py
--rw-r--r--   0 markov    (1000) markov    (1000)      407 2022-08-30 09:24:14.000000 iocbio.gel-1.0.0/iocbio/gel/db/alembic/versions/fd339f2a6eb4_upgrade.sql
--rw-r--r--   0 markov    (1000) markov    (1000)      682 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/db/alembic/versions/nrobvvzilln3_create_views.py
--rw-r--r--   0 markov    (1000) markov    (1000)     6589 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/db/alembic/versions/wrsc7ffn1q95_revised_initial_version.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2176 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/db/base.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.908393 iocbio.gel-1.0.0/iocbio/gel/db/connection_parameters/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-28 08:47:54.000000 iocbio.gel-1.0.0/iocbio/gel/db/connection_parameters/__init__.py
--rw-r--r--   0 markov    (1000) markov    (1000)      455 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/db/connection_parameters/connection_parameters.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2029 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/db/connection_parameters/postgresql_parameters.py
--rw-r--r--   0 markov    (1000) markov    (1000)      614 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/db/connection_parameters/sqlite_parameters.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2986 2023-03-27 13:03:45.000000 iocbio.gel-1.0.0/iocbio/gel/db/database_client.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2471 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/db/database_setup.py
--rw-r--r--   0 markov    (1000) markov    (1000)      733 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/db/database_type.py
--rw-r--r--   0 markov    (1000) markov    (1000)      368 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/db/entity_visitor.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.908393 iocbio.gel-1.0.0/iocbio/gel/domain/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.0/iocbio/gel/domain/__init__.py
--rw-r--r--   0 markov    (1000) markov    (1000)     3420 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/domain/curved_lane_region.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1247 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/domain/detect_analysis_region.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1526 2023-03-29 06:51:40.000000 iocbio.gel-1.0.0/iocbio/gel/domain/gel.py
--rw-r--r--   0 markov    (1000) markov    (1000)     4844 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/domain/gel_image.py
--rw-r--r--   0 markov    (1000) markov    (1000)     4325 2023-03-20 14:52:12.000000 iocbio.gel-1.0.0/iocbio/gel/domain/gel_image_lane.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1114 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/domain/gel_lane.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1616 2023-03-29 06:51:40.000000 iocbio.gel-1.0.0/iocbio/gel/domain/measurement.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2246 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/domain/measurement_lane.py
--rw-r--r--   0 markov    (1000) markov    (1000)      855 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/domain/measurement_type.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1026 2023-03-20 14:26:15.000000 iocbio.gel-1.0.0/iocbio/gel/domain/plot.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2336 2023-03-20 14:26:15.000000 iocbio.gel-1.0.0/iocbio/gel/domain/plot_region.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2518 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/domain/project.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1594 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/domain/xls_writer.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.908393 iocbio.gel-1.0.0/iocbio/gel/gui/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.0/iocbio/gel/gui/__init__.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.908393 iocbio.gel-1.0.0/iocbio/gel/gui/contexts/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-08-03 18:28:50.000000 iocbio.gel-1.0.0/iocbio/gel/gui/contexts/__init__.py
--rw-r--r--   0 markov    (1000) markov    (1000)     5770 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/contexts/analysis.py
--rw-r--r--   0 markov    (1000) markov    (1000)     3738 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/contexts/gels.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1647 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/contexts/measurement_types.py
--rw-r--r--   0 markov    (1000) markov    (1000)     3346 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/contexts/projects.py
--rw-r--r--   0 markov    (1000) markov    (1000)     4425 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/contexts/settings.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2180 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/contexts/single_gel.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.911727 iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/__init__.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.911727 iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/database_connection_settings/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/database_connection_settings/__init__.py
--rw-r--r--   0 markov    (1000) markov    (1000)      445 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/database_connection_settings/database_connection_settings.py
--rw-r--r--   0 markov    (1000) markov    (1000)     4717 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/database_connection_settings/db_selection_form.py
--rw-r--r--   0 markov    (1000) markov    (1000)     3210 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/database_connection_settings/postgresql_connection_settings.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2088 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/database_connection_settings/sqlite_connection_settings.py
--rw-r--r--   0 markov    (1000) markov    (1000)      734 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/db_selection.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.911727 iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/image_source_settings/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/image_source_settings/__init__.py
--rw-r--r--   0 markov    (1000) markov    (1000)     5236 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/image_source_settings/image_source_form.py
--rw-r--r--   0 markov    (1000) markov    (1000)      751 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/image_source_settings/image_source_settings.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1515 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/image_source_settings/local_settings.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1894 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/image_source_settings/omero_settings.py
--rw-r--r--   0 markov    (1000) markov    (1000)      389 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/select_image.py
--rw-r--r--   0 markov    (1000) markov    (1000)      867 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/select_image_factory.py
--rw-r--r--   0 markov    (1000) markov    (1000)     3072 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/select_image_local.py
--rw-r--r--   0 markov    (1000) markov    (1000)     4840 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/select_image_omero.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1263 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/icons.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.915060 iocbio.gel-1.0.0/iocbio/gel/gui/models/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-08-02 17:55:02.000000 iocbio.gel-1.0.0/iocbio/gel/gui/models/__init__.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1682 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/models/checkbox_proxy.py
--rw-r--r--   0 markov    (1000) markov    (1000)     6570 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/models/gel_images_model.py
--rw-r--r--   0 markov    (1000) markov    (1000)     4009 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/models/gel_lanes_model.py
--rw-r--r--   0 markov    (1000) markov    (1000)     6801 2023-03-29 06:51:40.000000 iocbio.gel-1.0.0/iocbio/gel/gui/models/gels_model.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.915060 iocbio.gel-1.0.0/iocbio/gel/gui/models/items/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-08-25 10:26:29.000000 iocbio.gel-1.0.0/iocbio/gel/gui/models/items/__init__.py
--rw-r--r--   0 markov    (1000) markov    (1000)     4827 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/models/items/tree_item.py
--rw-r--r--   0 markov    (1000) markov    (1000)     3677 2023-03-15 14:17:53.000000 iocbio.gel-1.0.0/iocbio/gel/gui/models/measurement_lanes_model.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2791 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/models/measurement_types_model.py
--rw-r--r--   0 markov    (1000) markov    (1000)     6343 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/models/measurements_model.py
--rw-r--r--   0 markov    (1000) markov    (1000)     6675 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/models/projects_gels_model.py
--rw-r--r--   0 markov    (1000) markov    (1000)     9682 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/models/projects_tree_model.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2802 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/models/proxy_table_model.py
--rw-r--r--   0 markov    (1000) markov    (1000)    12718 2023-03-15 12:40:42.000000 iocbio.gel-1.0.0/iocbio/gel/gui/models/table_model.py
--rw-r--r--   0 markov    (1000) markov    (1000)     3078 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/models/tracking_model.py
--rw-r--r--   0 markov    (1000) markov    (1000)     7312 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/models/tree_model.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.915060 iocbio.gel-1.0.0/iocbio/gel/gui/resources/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-08-31 08:05:40.000000 iocbio.gel-1.0.0/iocbio/gel/gui/resources/__init__.py
--rw-r--r--   0 markov    (1000) markov    (1000)    66219 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/resources/rc_icons.py
--rw-r--r--   0 markov    (1000) markov    (1000)      484 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/style.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1002 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/user_resized.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.915060 iocbio.gel-1.0.0/iocbio/gel/gui/views/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-08-02 17:55:02.000000 iocbio.gel-1.0.0/iocbio/gel/gui/views/__init__.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.915060 iocbio.gel-1.0.0/iocbio/gel/gui/views/delegates/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-08-02 17:55:02.000000 iocbio.gel-1.0.0/iocbio/gel/gui/views/delegates/__init__.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1246 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/views/delegates/combobox_delegate.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1430 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/views/delegates/datetime_delegate.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1537 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/views/delegates/multiselect_delegate.py
--rw-r--r--   0 markov    (1000) markov    (1000)      962 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/views/delegates/nobackground_delegate.py
--rw-r--r--   0 markov    (1000) markov    (1000)      707 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/views/delegates/non_negative_double.py
--rw-r--r--   0 markov    (1000) markov    (1000)      864 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/views/delegates/selectable_row_delegate.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1520 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/views/gel_images_view.py
--rw-r--r--   0 markov    (1000) markov    (1000)     4395 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/views/table_view.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2476 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/views/tree_view.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.918394 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/__init__.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.918394 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/__init__.py
--rw-r--r--   0 markov    (1000) markov    (1000)     7678 2023-03-28 08:03:43.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/active_lanes.py
--rw-r--r--   0 markov    (1000) markov    (1000)     9727 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/adjust.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1761 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/adjust_roi.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.918394 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/background/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-18 06:19:23.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/background/__init__.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2062 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/background/ball_layout.py
--rw-r--r--   0 markov    (1000) markov    (1000)      903 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/background/bg_color_box.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2621 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/background/bg_subtraction_box.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1385 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/background/ellipsoid_layout.py
--rw-r--r--   0 markov    (1000) markov    (1000)      386 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/background/parameters.py
--rw-r--r--   0 markov    (1000) markov    (1000)    15799 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/background_subtraction.py
--rw-r--r--   0 markov    (1000) markov    (1000)    17885 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/curved_line_roi.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.918394 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/intensity/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/intensity/__init__.py
--rw-r--r--   0 markov    (1000) markov    (1000)     3121 2023-03-29 06:51:40.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/intensity/intensity_plot.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2479 2023-03-20 14:26:15.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/intensity/lane_intensity_plot.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1681 2023-03-20 14:26:15.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/intensity/lane_plot_list.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2904 2023-03-28 13:48:06.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/intensity/measurement_intensity_plot.py
--rw-r--r--   0 markov    (1000) markov    (1000)     9219 2023-03-29 06:51:40.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/intensity/measurement_plot_list.py
--rw-r--r--   0 markov    (1000) markov    (1000)     9268 2023-03-20 14:26:15.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/intensity/plot_list.py
--rw-r--r--   0 markov    (1000) markov    (1000)     4807 2023-03-20 14:26:15.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/intensity/zero_line.py
--rw-r--r--   0 markov    (1000) markov    (1000)     8827 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/passive_lanes.py
--rw-r--r--   0 markov    (1000) markov    (1000)     3252 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/raw.py
--rw-r--r--   0 markov    (1000) markov    (1000)      558 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/confirm_popup.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1794 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/control_slider.py
--rw-r--r--   0 markov    (1000) markov    (1000)     6247 2023-03-29 06:51:40.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/gel_form.py
--rw-r--r--   0 markov    (1000) markov    (1000)     4503 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/gel_image_form.py
--rw-r--r--   0 markov    (1000) markov    (1000)     3328 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/gel_measurements.py
--rw-r--r--   0 markov    (1000) markov    (1000)      749 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/mandatory_line_edit.py
--rw-r--r--   0 markov    (1000) markov    (1000)      569 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/measurement_lanes.py
--rw-r--r--   0 markov    (1000) markov    (1000)     3028 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/multiple_project_selection.py
--rw-r--r--   0 markov    (1000) markov    (1000)     4605 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/project_selection.py
--rw-r--r--   0 markov    (1000) markov    (1000)     6046 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/sidebar.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1166 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/status_bar.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.918394 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/toolbars/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/toolbars/__init__.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1692 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/toolbars/add_gel.py
--rw-r--r--   0 markov    (1000) markov    (1000)     3175 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/toolbars/main.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1793 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/viewbox_empty_contextmenu.py
--rw-r--r--   0 markov    (1000) markov    (1000)      444 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/widgets/warning_popup.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.918394 iocbio.gel-1.0.0/iocbio/gel/gui/windows/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.0/iocbio/gel/gui/windows/__init__.py
--rw-r--r--   0 markov    (1000) markov    (1000)     3627 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/gui/windows/main.py
--rw-r--r--   0 markov    (1000) markov    (1000)      960 2022-07-12 16:54:56.000000 iocbio.gel-1.0.0/iocbio/gel/logging.ini
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.921727 iocbio.gel-1.0.0/iocbio/gel/repository/
--rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.0/iocbio/gel/repository/__init__.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2075 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/repository/entity_repository.py
--rw-r--r--   0 markov    (1000) markov    (1000)     9557 2023-03-29 06:51:40.000000 iocbio.gel-1.0.0/iocbio/gel/repository/export_repository.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2865 2023-03-16 12:43:44.000000 iocbio.gel-1.0.0/iocbio/gel/repository/gel_image_lane_repository.py
--rw-r--r--   0 markov    (1000) markov    (1000)     4976 2023-03-16 12:43:44.000000 iocbio.gel-1.0.0/iocbio/gel/repository/gel_image_repository.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1378 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/repository/gel_lane_repository.py
--rw-r--r--   0 markov    (1000) markov    (1000)     2455 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/repository/gel_repository.py
--rw-r--r--   0 markov    (1000) markov    (1000)     8562 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/repository/image_repository.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1427 2023-03-29 06:51:40.000000 iocbio.gel-1.0.0/iocbio/gel/repository/measurement_lane_repository.py
--rw-r--r--   0 markov    (1000) markov    (1000)     3880 2023-03-29 06:51:40.000000 iocbio.gel-1.0.0/iocbio/gel/repository/measurement_repository.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1126 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/repository/measurement_type_repository.py
--rw-r--r--   0 markov    (1000) markov    (1000)     1547 2023-03-01 10:12:12.000000 iocbio.gel-1.0.0/iocbio/gel/repository/project_repository.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.898393 iocbio.gel-1.0.0/iocbio.gel.egg-info/
--rw-r--r--   0 markov    (1000) markov    (1000)     1791 2023-04-05 14:11:12.000000 iocbio.gel-1.0.0/iocbio.gel.egg-info/PKG-INFO
--rw-r--r--   0 markov    (1000) markov    (1000)    10018 2023-04-05 14:11:12.000000 iocbio.gel-1.0.0/iocbio.gel.egg-info/SOURCES.txt
--rw-r--r--   0 markov    (1000) markov    (1000)        1 2023-04-05 14:11:12.000000 iocbio.gel-1.0.0/iocbio.gel.egg-info/dependency_links.txt
--rw-r--r--   0 markov    (1000) markov    (1000)       47 2023-04-05 14:11:12.000000 iocbio.gel-1.0.0/iocbio.gel.egg-info/entry_points.txt
--rw-r--r--   0 markov    (1000) markov    (1000)      233 2023-04-05 14:11:12.000000 iocbio.gel-1.0.0/iocbio.gel.egg-info/requires.txt
--rw-r--r--   0 markov    (1000) markov    (1000)        7 2023-04-05 14:11:12.000000 iocbio.gel-1.0.0/iocbio.gel.egg-info/top_level.txt
--rw-r--r--   0 markov    (1000) markov    (1000)      185 2023-03-27 13:56:58.000000 iocbio.gel-1.0.0/mkdocs.yml
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.891726 iocbio.gel-1.0.0/packaging/
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.921727 iocbio.gel-1.0.0/packaging/pyinstaller/
--rw-r--r--   0 markov    (1000) markov    (1000)     1585 2022-08-31 08:05:40.000000 iocbio.gel-1.0.0/packaging/pyinstaller/app.spec
--rw-r--r--   0 markov    (1000) markov    (1000)       19 2022-06-18 06:19:23.000000 iocbio.gel-1.0.0/packaging/pyinstaller/gel.bat
--rw-r--r--   0 markov    (1000) markov    (1000)       57 2022-07-26 08:44:53.000000 iocbio.gel-1.0.0/pyproject.toml
--rw-r--r--   0 markov    (1000) markov    (1000)      796 2023-03-01 13:09:32.000000 iocbio.gel-1.0.0/requirements.txt
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.921727 iocbio.gel-1.0.0/resources/
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.921727 iocbio.gel-1.0.0/resources/icons/
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.925061 iocbio.gel-1.0.0/resources/icons/feather/
--rw-r--r--   0 markov    (1000) markov    (1000)      307 2022-08-31 08:05:40.000000 iocbio.gel-1.0.0/resources/icons/feather/arrow-right.svg
--rw-r--r--   0 markov    (1000) markov    (1000)      440 2022-08-31 08:05:40.000000 iocbio.gel-1.0.0/resources/icons/feather/coffee.svg
--rw-r--r--   0 markov    (1000) markov    (1000)      304 2022-08-31 08:05:40.000000 iocbio.gel-1.0.0/resources/icons/feather/folder.svg
--rw-r--r--   0 markov    (1000) markov    (1000)      362 2022-08-31 08:05:40.000000 iocbio.gel-1.0.0/resources/icons/feather/image.svg
--rw-r--r--   0 markov    (1000) markov    (1000)      304 2022-12-05 07:00:27.000000 iocbio.gel-1.0.0/resources/icons/feather/plus.svg
--rw-r--r--   0 markov    (1000) markov    (1000)     1217 2022-08-31 08:05:40.000000 iocbio.gel-1.0.0/resources/icons/feather/readme-and-license.md
--rw-r--r--   0 markov    (1000) markov    (1000)      292 2022-08-31 08:05:40.000000 iocbio.gel-1.0.0/resources/icons/feather/x.svg
--rw-r--r--   0 markov    (1000) markov    (1000)    53514 2022-10-26 08:47:00.000000 iocbio.gel-1.0.0/resources/icons/gel.svg
--rw-r--r--   0 markov    (1000) markov    (1000)      346 2022-12-05 07:00:27.000000 iocbio.gel-1.0.0/resources/icons.qrc
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.925061 iocbio.gel-1.0.0/scripts/
--rw-r--r--   0 markov    (1000) markov    (1000)      377 2023-03-20 14:26:15.000000 iocbio.gel-1.0.0/scripts/generate_image.py
--rw-r--r--   0 markov    (1000) markov    (1000)      444 2023-04-05 14:11:12.925061 iocbio.gel-1.0.0/setup.cfg
--rw-r--r--   0 markov    (1000) markov    (1000)     2485 2023-04-05 13:40:46.000000 iocbio.gel-1.0.0/setup.py
-drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-04-05 14:11:12.925061 iocbio.gel-1.0.0/sql/
--rw-r--r--   0 markov    (1000) markov    (1000)      642 2023-04-03 09:05:03.000000 iocbio.gel-1.0.0/sql/README.md
--rw-r--r--   0 markov    (1000) markov    (1000)      855 2023-04-03 08:00:25.000000 iocbio.gel-1.0.0/sql/gel_raw_data.sql
--rw-r--r--   0 markov    (1000) markov    (1000)     1005 2023-04-03 08:01:51.000000 iocbio.gel-1.0.0/sql/gel_relative_data.sql
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.108047 iocbio.gel-1.0.1/
+-rw-r--r--   0 markov    (1000) markov    (1000)      149 2022-10-20 13:58:54.000000 iocbio.gel-1.0.1/.gitignore
+-rw-r--r--   0 markov    (1000) markov    (1000)     2286 2023-04-05 13:20:14.000000 iocbio.gel-1.0.1/.gitlab-ci.yml
+-rw-r--r--   0 markov    (1000) markov    (1000)      668 2023-03-01 10:05:44.000000 iocbio.gel-1.0.1/AUTHORS.md
+-rw-r--r--   0 markov    (1000) markov    (1000)     2095 2023-05-29 05:28:58.000000 iocbio.gel-1.0.1/CHANGELOG.md
+-rw-r--r--   0 markov    (1000) markov    (1000)     1639 2023-03-29 06:51:40.000000 iocbio.gel-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0 markov    (1000) markov    (1000)    32198 2023-02-08 15:18:05.000000 iocbio.gel-1.0.1/LICENSE.md
+-rw-r--r--   0 markov    (1000) markov    (1000)     1791 2023-05-29 05:30:41.108047 iocbio.gel-1.0.1/PKG-INFO
+-rw-r--r--   0 markov    (1000) markov    (1000)     1231 2022-10-20 13:58:54.000000 iocbio.gel-1.0.1/README.md
+-rw-r--r--   0 markov    (1000) markov    (1000)     1273 2023-05-29 05:30:05.000000 iocbio.gel-1.0.1/RELEASING.md
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.094714 iocbio.gel-1.0.1/docs/
+-rw-r--r--   0 markov    (1000) markov    (1000)      590 2022-10-20 13:58:54.000000 iocbio.gel-1.0.1/docs/development.md
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.094714 iocbio.gel-1.0.1/docs/img/
+-rw-r--r--   0 markov    (1000) markov    (1000)   123881 2023-04-05 12:49:25.000000 iocbio.gel-1.0.1/docs/img/curved_lane.png
+-rw-r--r--   0 markov    (1000) markov    (1000)   140271 2023-04-05 12:39:19.000000 iocbio.gel-1.0.1/docs/img/lanes.png
+-rw-r--r--   0 markov    (1000) markov    (1000)   141782 2023-04-05 12:46:11.000000 iocbio.gel-1.0.1/docs/img/measurement_lanes.png
+-rw-r--r--   0 markov    (1000) markov    (1000)    93091 2023-04-05 12:38:33.000000 iocbio.gel-1.0.1/docs/img/projects.png
+-rw-r--r--   0 markov    (1000) markov    (1000)    60215 2023-04-05 12:37:47.000000 iocbio.gel-1.0.1/docs/img/types_and_edit_mode.png
+-rw-r--r--   0 markov    (1000) markov    (1000)     2019 2023-04-05 14:07:55.000000 iocbio.gel-1.0.1/docs/index.md
+-rw-r--r--   0 markov    (1000) markov    (1000)     4859 2023-04-05 14:17:22.000000 iocbio.gel-1.0.1/docs/install.md
+-rw-r--r--   0 markov    (1000) markov    (1000)    19234 2023-04-05 14:09:32.000000 iocbio.gel-1.0.1/docs/users.md
+-rw-r--r--   0 markov    (1000) markov    (1000)      788 2023-04-05 14:16:43.000000 iocbio.gel-1.0.1/install.ps1
+-rwxr-xr-x   0 markov    (1000) markov    (1000)      593 2023-04-05 14:16:31.000000 iocbio.gel-1.0.1/install.sh
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.094714 iocbio.gel-1.0.1/iocbio/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-08-03 18:28:50.000000 iocbio.gel-1.0.1/iocbio/__init__.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.094714 iocbio.gel-1.0.1/iocbio/gel/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.1/iocbio/gel/__init__.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     7005 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/app.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.094714 iocbio.gel-1.0.1/iocbio/gel/application/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.1/iocbio/gel/application/__init__.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.094714 iocbio.gel-1.0.1/iocbio/gel/application/application_state/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.1/iocbio/gel/application/application_state/__init__.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2341 2023-03-01 10:12:11.000000 iocbio.gel-1.0.1/iocbio/gel/application/application_state/context.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      362 2023-03-01 10:12:11.000000 iocbio.gel-1.0.1/iocbio/gel/application/application_state/mode.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1785 2023-03-01 10:12:11.000000 iocbio.gel-1.0.1/iocbio/gel/application/application_state/state.py
+-rw-r--r--   0 markov    (1000) markov    (1000)    19495 2023-03-29 06:51:40.000000 iocbio.gel-1.0.1/iocbio/gel/application/container.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      950 2023-03-01 10:12:11.000000 iocbio.gel-1.0.1/iocbio/gel/application/event_consumer.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     3443 2023-03-20 14:26:15.000000 iocbio.gel-1.0.1/iocbio/gel/application/event_registry.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      724 2023-03-01 10:12:11.000000 iocbio.gel-1.0.1/iocbio/gel/application/file_digest.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.094714 iocbio.gel-1.0.1/iocbio/gel/application/image/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-07-01 16:47:54.000000 iocbio.gel-1.0.1/iocbio/gel/application/image/__init__.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      733 2023-03-01 10:12:11.000000 iocbio.gel-1.0.1/iocbio/gel/application/image/background_method.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1368 2023-05-25 08:41:21.000000 iocbio.gel-1.0.1/iocbio/gel/application/image/image.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      301 2023-03-01 10:12:11.000000 iocbio.gel-1.0.1/iocbio/gel/application/image/image_source.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2527 2023-03-01 10:12:11.000000 iocbio.gel-1.0.1/iocbio/gel/application/image/image_source_setup.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      260 2023-03-01 10:12:11.000000 iocbio.gel-1.0.1/iocbio/gel/application/image/image_state.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     4025 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/application/image/omero_client.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1929 2023-05-25 12:03:22.000000 iocbio.gel-1.0.1/iocbio/gel/application/image/processing_cache.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      640 2023-03-01 10:12:11.000000 iocbio.gel-1.0.1/iocbio/gel/application/image/region.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1015 2023-03-01 10:12:11.000000 iocbio.gel-1.0.1/iocbio/gel/application/image/repository_backend.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1215 2023-03-01 10:12:11.000000 iocbio.gel-1.0.1/iocbio/gel/application/image/repository_backend_local.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2593 2023-03-01 10:12:11.000000 iocbio.gel-1.0.1/iocbio/gel/application/image/repository_backend_omero.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1026 2023-03-01 10:12:11.000000 iocbio.gel-1.0.1/iocbio/gel/application/number_list.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1220 2023-03-01 10:12:11.000000 iocbio.gel-1.0.1/iocbio/gel/application/settings_proxy.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.098047 iocbio.gel-1.0.1/iocbio/gel/application/thread/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-07-14 08:43:25.000000 iocbio.gel-1.0.1/iocbio/gel/application/thread/__init__.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1011 2023-03-01 10:12:11.000000 iocbio.gel-1.0.1/iocbio/gel/application/thread/fetch_image_from_omero.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1568 2023-03-01 10:12:11.000000 iocbio.gel-1.0.1/iocbio/gel/application/thread/job.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1636 2023-03-01 10:12:11.000000 iocbio.gel-1.0.1/iocbio/gel/application/thread/load_image_preview.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      915 2023-03-01 10:12:11.000000 iocbio.gel-1.0.1/iocbio/gel/application/thread/pool_worker.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     4092 2023-05-29 05:27:09.000000 iocbio.gel-1.0.1/iocbio/gel/application/thread/rolling_ball.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1500 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/application/thread/sequential_worker.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2211 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/application/thread/thread_pool.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      542 2023-03-01 10:12:11.000000 iocbio.gel-1.0.1/iocbio/gel/application/thread/worker.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.098047 iocbio.gel-1.0.1/iocbio/gel/command/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.1/iocbio/gel/command/__init__.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      507 2023-03-01 10:12:11.000000 iocbio.gel-1.0.1/iocbio/gel/command/command.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1192 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/command/command_set.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1615 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/command/create_entity.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     3078 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/command/delete_collector.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1611 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/command/delete_entity.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     3029 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/command/history_manager.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2387 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/command/project_delete_collector.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1082 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/command/transaction_set.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1292 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/command/update_entity.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2501 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/command/update_many_relationship.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1357 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/command/update_project.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      163 2023-05-29 05:27:16.000000 iocbio.gel-1.0.1/iocbio/gel/const.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.098047 iocbio.gel-1.0.1/iocbio/gel/db/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.1/iocbio/gel/db/__init__.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.098047 iocbio.gel-1.0.1/iocbio/gel/db/alembic/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.1/iocbio/gel/db/alembic/__init__.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2427 2022-06-28 08:47:54.000000 iocbio.gel-1.0.1/iocbio/gel/db/alembic/alembic.ini
+-rw-r--r--   0 markov    (1000) markov    (1000)     2770 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/db/alembic/env.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      352 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/db/alembic/execute_sqlfile.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      495 2022-06-28 06:13:47.000000 iocbio.gel-1.0.1/iocbio/gel/db/alembic/script.py.mako
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.098047 iocbio.gel-1.0.1/iocbio/gel/db/alembic/versions/
+-rw-r--r--   0 markov    (1000) markov    (1000)      704 2023-03-29 06:51:40.000000 iocbio.gel-1.0.1/iocbio/gel/db/alembic/versions/8b8ae59755af_synced_lane_widths.py
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.1/iocbio/gel/db/alembic/versions/__init__.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1341 2022-10-11 07:06:04.000000 iocbio.gel-1.0.1/iocbio/gel/db/alembic/versions/create_views_set_1.sql
+-rw-r--r--   0 markov    (1000) markov    (1000)      519 2023-03-29 06:51:40.000000 iocbio.gel-1.0.1/iocbio/gel/db/alembic/versions/d8d292a431fe_allow_to_sync_measurement_rois.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      175 2022-08-23 14:17:34.000000 iocbio.gel-1.0.1/iocbio/gel/db/alembic/versions/drop_views_set_1.sql
+-rw-r--r--   0 markov    (1000) markov    (1000)      813 2023-03-29 06:51:40.000000 iocbio.gel-1.0.1/iocbio/gel/db/alembic/versions/e78898a9c9f1_change_transfer_to_ref_time.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1259 2023-03-29 06:51:40.000000 iocbio.gel-1.0.1/iocbio/gel/db/alembic/versions/fbf8b6944c61_limit_protein_to_non_negative_value.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2274 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/db/alembic/versions/fd339f2a6eb4_projects.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      407 2022-08-30 09:24:14.000000 iocbio.gel-1.0.1/iocbio/gel/db/alembic/versions/fd339f2a6eb4_upgrade.sql
+-rw-r--r--   0 markov    (1000) markov    (1000)      682 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/db/alembic/versions/nrobvvzilln3_create_views.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     6589 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/db/alembic/versions/wrsc7ffn1q95_revised_initial_version.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2176 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/db/base.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.098047 iocbio.gel-1.0.1/iocbio/gel/db/connection_parameters/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-28 08:47:54.000000 iocbio.gel-1.0.1/iocbio/gel/db/connection_parameters/__init__.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      455 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/db/connection_parameters/connection_parameters.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2029 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/db/connection_parameters/postgresql_parameters.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      614 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/db/connection_parameters/sqlite_parameters.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2986 2023-03-27 13:03:45.000000 iocbio.gel-1.0.1/iocbio/gel/db/database_client.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2471 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/db/database_setup.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      733 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/db/database_type.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      368 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/db/entity_visitor.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.101380 iocbio.gel-1.0.1/iocbio/gel/domain/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.1/iocbio/gel/domain/__init__.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     3420 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/domain/curved_lane_region.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1247 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/domain/detect_analysis_region.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1526 2023-03-29 06:51:40.000000 iocbio.gel-1.0.1/iocbio/gel/domain/gel.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     4844 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/domain/gel_image.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     4325 2023-03-20 14:52:12.000000 iocbio.gel-1.0.1/iocbio/gel/domain/gel_image_lane.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1114 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/domain/gel_lane.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1616 2023-03-29 06:51:40.000000 iocbio.gel-1.0.1/iocbio/gel/domain/measurement.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2246 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/domain/measurement_lane.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      855 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/domain/measurement_type.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1026 2023-03-20 14:26:15.000000 iocbio.gel-1.0.1/iocbio/gel/domain/plot.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2336 2023-03-20 14:26:15.000000 iocbio.gel-1.0.1/iocbio/gel/domain/plot_region.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2518 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/domain/project.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1594 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/domain/xls_writer.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.101380 iocbio.gel-1.0.1/iocbio/gel/gui/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.1/iocbio/gel/gui/__init__.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.101380 iocbio.gel-1.0.1/iocbio/gel/gui/contexts/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-08-03 18:28:50.000000 iocbio.gel-1.0.1/iocbio/gel/gui/contexts/__init__.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     5770 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/contexts/analysis.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     3738 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/contexts/gels.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1647 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/contexts/measurement_types.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     3346 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/contexts/projects.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     4425 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/contexts/settings.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2180 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/contexts/single_gel.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.101380 iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/__init__.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.101380 iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/database_connection_settings/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/database_connection_settings/__init__.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      445 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/database_connection_settings/database_connection_settings.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     4717 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/database_connection_settings/db_selection_form.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     3210 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/database_connection_settings/postgresql_connection_settings.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2088 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/database_connection_settings/sqlite_connection_settings.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      734 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/db_selection.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.101380 iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/image_source_settings/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/image_source_settings/__init__.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     5236 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/image_source_settings/image_source_form.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      751 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/image_source_settings/image_source_settings.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1515 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/image_source_settings/local_settings.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1894 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/image_source_settings/omero_settings.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      389 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/select_image.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      867 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/select_image_factory.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     3072 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/select_image_local.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     4840 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/select_image_omero.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1263 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/icons.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.104714 iocbio.gel-1.0.1/iocbio/gel/gui/models/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-08-02 17:55:02.000000 iocbio.gel-1.0.1/iocbio/gel/gui/models/__init__.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1682 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/models/checkbox_proxy.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     6570 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/models/gel_images_model.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     4009 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/models/gel_lanes_model.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     6801 2023-03-29 06:51:40.000000 iocbio.gel-1.0.1/iocbio/gel/gui/models/gels_model.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.104714 iocbio.gel-1.0.1/iocbio/gel/gui/models/items/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-08-25 10:26:29.000000 iocbio.gel-1.0.1/iocbio/gel/gui/models/items/__init__.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     4827 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/models/items/tree_item.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     3677 2023-03-15 14:17:53.000000 iocbio.gel-1.0.1/iocbio/gel/gui/models/measurement_lanes_model.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2791 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/models/measurement_types_model.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     6343 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/models/measurements_model.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     6675 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/models/projects_gels_model.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     9682 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/models/projects_tree_model.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2802 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/models/proxy_table_model.py
+-rw-r--r--   0 markov    (1000) markov    (1000)    12718 2023-03-15 12:40:42.000000 iocbio.gel-1.0.1/iocbio/gel/gui/models/table_model.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     3078 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/models/tracking_model.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     7312 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/models/tree_model.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.104714 iocbio.gel-1.0.1/iocbio/gel/gui/resources/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-08-31 08:05:40.000000 iocbio.gel-1.0.1/iocbio/gel/gui/resources/__init__.py
+-rw-r--r--   0 markov    (1000) markov    (1000)    66219 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/resources/rc_icons.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      484 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/style.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1002 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/user_resized.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.104714 iocbio.gel-1.0.1/iocbio/gel/gui/views/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-08-02 17:55:02.000000 iocbio.gel-1.0.1/iocbio/gel/gui/views/__init__.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.104714 iocbio.gel-1.0.1/iocbio/gel/gui/views/delegates/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-08-02 17:55:02.000000 iocbio.gel-1.0.1/iocbio/gel/gui/views/delegates/__init__.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1246 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/views/delegates/combobox_delegate.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1430 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/views/delegates/datetime_delegate.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1537 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/views/delegates/multiselect_delegate.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      962 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/views/delegates/nobackground_delegate.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      707 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/views/delegates/non_negative_double.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      864 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/views/delegates/selectable_row_delegate.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1520 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/views/gel_images_view.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     4395 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/views/table_view.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2476 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/views/tree_view.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.104714 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/__init__.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.104714 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/__init__.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     7678 2023-03-28 08:03:43.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/active_lanes.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     9727 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/adjust.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1761 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/adjust_roi.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.104714 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/background/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-18 06:19:23.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/background/__init__.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2062 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/background/ball_layout.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      903 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/background/bg_color_box.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2621 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/background/bg_subtraction_box.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1385 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/background/ellipsoid_layout.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      386 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/background/parameters.py
+-rw-r--r--   0 markov    (1000) markov    (1000)    15799 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/background_subtraction.py
+-rw-r--r--   0 markov    (1000) markov    (1000)    17885 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/curved_line_roi.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.108047 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/intensity/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/intensity/__init__.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     3121 2023-03-29 06:51:40.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/intensity/intensity_plot.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2479 2023-03-20 14:26:15.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/intensity/lane_intensity_plot.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1681 2023-03-20 14:26:15.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/intensity/lane_plot_list.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2904 2023-03-28 13:48:06.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/intensity/measurement_intensity_plot.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     9219 2023-03-29 06:51:40.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/intensity/measurement_plot_list.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     9268 2023-05-25 09:59:06.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/intensity/plot_list.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     4807 2023-03-20 14:26:15.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/intensity/zero_line.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     8827 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/passive_lanes.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     3252 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/raw.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      558 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/confirm_popup.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1794 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/control_slider.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     6247 2023-03-29 06:51:40.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/gel_form.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     4503 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/gel_image_form.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     3328 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/gel_measurements.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      749 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/mandatory_line_edit.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      569 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/measurement_lanes.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     3028 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/multiple_project_selection.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     4605 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/project_selection.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     6046 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/sidebar.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1166 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/status_bar.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.108047 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/toolbars/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/toolbars/__init__.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1692 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/toolbars/add_gel.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     3175 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/toolbars/main.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1793 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/viewbox_empty_contextmenu.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      444 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/widgets/warning_popup.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.108047 iocbio.gel-1.0.1/iocbio/gel/gui/windows/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.1/iocbio/gel/gui/windows/__init__.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     3627 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/gui/windows/main.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      960 2022-07-12 16:54:56.000000 iocbio.gel-1.0.1/iocbio/gel/logging.ini
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.108047 iocbio.gel-1.0.1/iocbio/gel/repository/
+-rw-r--r--   0 markov    (1000) markov    (1000)        0 2022-06-09 18:05:59.000000 iocbio.gel-1.0.1/iocbio/gel/repository/__init__.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2075 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/repository/entity_repository.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     9557 2023-03-29 06:51:40.000000 iocbio.gel-1.0.1/iocbio/gel/repository/export_repository.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2865 2023-03-16 12:43:44.000000 iocbio.gel-1.0.1/iocbio/gel/repository/gel_image_lane_repository.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     4976 2023-03-16 12:43:44.000000 iocbio.gel-1.0.1/iocbio/gel/repository/gel_image_repository.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1378 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/repository/gel_lane_repository.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     2455 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/repository/gel_repository.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     9005 2023-05-29 05:27:09.000000 iocbio.gel-1.0.1/iocbio/gel/repository/image_repository.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1427 2023-03-29 06:51:40.000000 iocbio.gel-1.0.1/iocbio/gel/repository/measurement_lane_repository.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     3880 2023-03-29 06:51:40.000000 iocbio.gel-1.0.1/iocbio/gel/repository/measurement_repository.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1126 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/repository/measurement_type_repository.py
+-rw-r--r--   0 markov    (1000) markov    (1000)     1547 2023-03-01 10:12:12.000000 iocbio.gel-1.0.1/iocbio/gel/repository/project_repository.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.094714 iocbio.gel-1.0.1/iocbio.gel.egg-info/
+-rw-r--r--   0 markov    (1000) markov    (1000)     1791 2023-05-29 05:30:41.000000 iocbio.gel-1.0.1/iocbio.gel.egg-info/PKG-INFO
+-rw-r--r--   0 markov    (1000) markov    (1000)    10018 2023-05-29 05:30:41.000000 iocbio.gel-1.0.1/iocbio.gel.egg-info/SOURCES.txt
+-rw-r--r--   0 markov    (1000) markov    (1000)        1 2023-05-29 05:30:41.000000 iocbio.gel-1.0.1/iocbio.gel.egg-info/dependency_links.txt
+-rw-r--r--   0 markov    (1000) markov    (1000)       47 2023-05-29 05:30:41.000000 iocbio.gel-1.0.1/iocbio.gel.egg-info/entry_points.txt
+-rw-r--r--   0 markov    (1000) markov    (1000)      233 2023-05-29 05:30:41.000000 iocbio.gel-1.0.1/iocbio.gel.egg-info/requires.txt
+-rw-r--r--   0 markov    (1000) markov    (1000)        7 2023-05-29 05:30:41.000000 iocbio.gel-1.0.1/iocbio.gel.egg-info/top_level.txt
+-rw-r--r--   0 markov    (1000) markov    (1000)      185 2023-03-27 13:56:58.000000 iocbio.gel-1.0.1/mkdocs.yml
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.091380 iocbio.gel-1.0.1/packaging/
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.108047 iocbio.gel-1.0.1/packaging/pyinstaller/
+-rw-r--r--   0 markov    (1000) markov    (1000)     1585 2022-08-31 08:05:40.000000 iocbio.gel-1.0.1/packaging/pyinstaller/app.spec
+-rw-r--r--   0 markov    (1000) markov    (1000)       19 2022-06-18 06:19:23.000000 iocbio.gel-1.0.1/packaging/pyinstaller/gel.bat
+-rw-r--r--   0 markov    (1000) markov    (1000)       57 2022-07-26 08:44:53.000000 iocbio.gel-1.0.1/pyproject.toml
+-rw-r--r--   0 markov    (1000) markov    (1000)      796 2023-03-01 13:09:32.000000 iocbio.gel-1.0.1/requirements.txt
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.108047 iocbio.gel-1.0.1/resources/
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.108047 iocbio.gel-1.0.1/resources/icons/
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.108047 iocbio.gel-1.0.1/resources/icons/feather/
+-rw-r--r--   0 markov    (1000) markov    (1000)      307 2022-08-31 08:05:40.000000 iocbio.gel-1.0.1/resources/icons/feather/arrow-right.svg
+-rw-r--r--   0 markov    (1000) markov    (1000)      440 2022-08-31 08:05:40.000000 iocbio.gel-1.0.1/resources/icons/feather/coffee.svg
+-rw-r--r--   0 markov    (1000) markov    (1000)      304 2022-08-31 08:05:40.000000 iocbio.gel-1.0.1/resources/icons/feather/folder.svg
+-rw-r--r--   0 markov    (1000) markov    (1000)      362 2022-08-31 08:05:40.000000 iocbio.gel-1.0.1/resources/icons/feather/image.svg
+-rw-r--r--   0 markov    (1000) markov    (1000)      304 2022-12-05 07:00:27.000000 iocbio.gel-1.0.1/resources/icons/feather/plus.svg
+-rw-r--r--   0 markov    (1000) markov    (1000)     1217 2022-08-31 08:05:40.000000 iocbio.gel-1.0.1/resources/icons/feather/readme-and-license.md
+-rw-r--r--   0 markov    (1000) markov    (1000)      292 2022-08-31 08:05:40.000000 iocbio.gel-1.0.1/resources/icons/feather/x.svg
+-rw-r--r--   0 markov    (1000) markov    (1000)    53514 2022-10-26 08:47:00.000000 iocbio.gel-1.0.1/resources/icons/gel.svg
+-rw-r--r--   0 markov    (1000) markov    (1000)      346 2022-12-05 07:00:27.000000 iocbio.gel-1.0.1/resources/icons.qrc
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.108047 iocbio.gel-1.0.1/scripts/
+-rw-r--r--   0 markov    (1000) markov    (1000)      377 2023-03-20 14:26:15.000000 iocbio.gel-1.0.1/scripts/generate_image.py
+-rw-r--r--   0 markov    (1000) markov    (1000)      444 2023-05-29 05:30:41.108047 iocbio.gel-1.0.1/setup.cfg
+-rw-r--r--   0 markov    (1000) markov    (1000)     2485 2023-05-29 05:27:26.000000 iocbio.gel-1.0.1/setup.py
+drwxr-xr-x   0 markov    (1000) markov    (1000)        0 2023-05-29 05:30:41.108047 iocbio.gel-1.0.1/sql/
+-rw-r--r--   0 markov    (1000) markov    (1000)      642 2023-04-03 09:05:03.000000 iocbio.gel-1.0.1/sql/README.md
+-rw-r--r--   0 markov    (1000) markov    (1000)      855 2023-04-03 08:00:25.000000 iocbio.gel-1.0.1/sql/gel_raw_data.sql
+-rw-r--r--   0 markov    (1000) markov    (1000)     1005 2023-04-03 08:01:51.000000 iocbio.gel-1.0.1/sql/gel_relative_data.sql
```

### Comparing `iocbio.gel-1.0.0/.gitlab-ci.yml` & `iocbio.gel-1.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/AUTHORS.md` & `iocbio.gel-1.0.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/CHANGELOG.md` & `iocbio.gel-1.0.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
+## [1.0.1] - 2023-05-29
+- Bugfix: save cached background image only if needed
+
 ## [1.0.0] - 2023-04-05
 - Update documentation
 
 ## [0.10.0] - 2023-03-29
 
 ### Added
 - Allow to synchronize measurement region for all lanes
```

### Comparing `iocbio.gel-1.0.0/CONTRIBUTING.md` & `iocbio.gel-1.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/LICENSE.md` & `iocbio.gel-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/PKG-INFO` & `iocbio.gel-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iocbio.gel
-Version: 1.0.0
+Version: 1.0.1
 Summary: IOCBio Gel
 Home-page: https://iocbio.gitlab.io/gel
 Author: IOCBio team
 Author-email: iocbio@sysbio.ioc.ee
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `iocbio.gel-1.0.0/README.md` & `iocbio.gel-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/RELEASING.md` & `iocbio.gel-1.0.1/RELEASING.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 ## Making packages
 
 ### Adjust version number
 
+```
 emacs setup.py iocbio/gel/const.py
+```
 
 ### Adjust Changelog
 
 Create a section for new version. Move Unreleased section to the new version 
 section as appropriate.
 
 ### Commit the changes
 
+```
 git status
 git add setup.py iocbio/gel/const.py CHANGELOG.md
 git commit -m "bump version"
 git push origin main
+```
 
 ### Creating requirements file for automatic installation
 
 To create `requirements.txt` first install Gel software in a new
 virtual environment and make sure that the software works as it
 should.  Then use `pip` to create `requirements.txt`:
```

### Comparing `iocbio.gel-1.0.0/docs/development.md` & `iocbio.gel-1.0.1/docs/development.md`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/docs/img/curved_lane.png` & `iocbio.gel-1.0.1/docs/img/curved_lane.png`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/docs/img/lanes.png` & `iocbio.gel-1.0.1/docs/img/lanes.png`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/docs/img/measurement_lanes.png` & `iocbio.gel-1.0.1/docs/img/measurement_lanes.png`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/docs/img/projects.png` & `iocbio.gel-1.0.1/docs/img/projects.png`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/docs/img/types_and_edit_mode.png` & `iocbio.gel-1.0.1/docs/img/types_and_edit_mode.png`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/docs/index.md` & `iocbio.gel-1.0.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/docs/install.md` & `iocbio.gel-1.0.1/docs/install.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,21 @@
 python3 -m pip install --user --upgrade pip
 ```
 
 Then, open a terminal and go to the folder where you would like to install the program.
 Then, run the following command:
 
 ```
-curl https://gitlab.com/iocbio/gel/-/raw/master/install.sh | bash
+curl https://gitlab.com/iocbio/gel/-/raw/main/install.sh | bash
 ```
 
 or
 
 ```
-wget -qO - https://gitlab.com/iocbio/gel/-/raw/master/install.sh | bash
+wget -qO - https://gitlab.com/iocbio/gel/-/raw/main/install.sh | bash
 ```
 and run by
 ```
 iocbio-gel/bin/iocbio-gel
 ```
 
 ## Windows
@@ -73,15 +73,15 @@
 get things installed or `AllSigned` for quite a bit more
 security. First, run `Get-ExecutionPolicy` in PowerShell. In case, it
 returns `Restricted`, then run `Set-ExecutionPolicy AllSigned` or
 `Set-ExecutionPolicy Bypass -Scope Process`.  When this is all set you
 can install the program by running following command:
 
 ```
-Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://gitlab.com/iocbio/gel/-/raw/master/install.ps1'))
+Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://gitlab.com/iocbio/gel/-/raw/main/install.ps1'))
 ```
 
 
 ## pip with virtual environment
 
 Sometimes packages for different applications can cause
 incompatibilities. To avoid it, you could use virtual environment for
```

### Comparing `iocbio.gel-1.0.0/docs/users.md` & `iocbio.gel-1.0.1/docs/users.md`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/install.ps1` & `iocbio.gel-1.0.1/install.ps1`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 #
 # This script installs IOCBio gel program to python virtual environment iocbio-gel
 #
 
 $rname = 'iocbio-gel_requirements.txt'
-Invoke-WebRequest -Uri 'https://gitlab.com/iocbio/gel/-/raw/master/requirements.txt' -OutFile $rname
+Invoke-WebRequest -Uri 'https://gitlab.com/iocbio/gel/-/raw/main/requirements.txt' -OutFile $rname
 
 python.exe -m venv iocbio-gel
 Write-Output "Python virtual environment for iocbio-gel created"
 Write-Output ""
 
 # Upgrading pip
 .\iocbio-gel\Scripts\python.exe -m pip install --upgrade pip
```

### Comparing `iocbio.gel-1.0.0/install.sh` & `iocbio.gel-1.0.1/install.sh`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 #
 
 set -e
 RNAME=iocbio-gel_requirements.txt
 python3 -m venv iocbio-gel
 if command -v wget &> /dev/null
 then
-  wget -q -O $RNAME https://gitlab.com/iocbio/gel/-/raw/master/requirements.txt
+  wget -q -O $RNAME https://gitlab.com/iocbio/gel/-/raw/main/requirements.txt
 else
-  curl https://gitlab.com/iocbio/gel/-/raw/master/requirements.txt --output $RNAME
+  curl https://gitlab.com/iocbio/gel/-/raw/main/requirements.txt --output $RNAME
 fi
 iocbio-gel/bin/pip3 install -r $RNAME
 rm $RNAME
 # iocbio-gel/bin/pip3 install git+https://gitlab.com/iocbio/gel
 iocbio-gel/bin/pip3 install iocbio.gel
 
 echo Start the program by running iocbio-gel/bin/iocbio-gel
```

### Comparing `iocbio.gel-1.0.0/iocbio/gel/app.py` & `iocbio.gel-1.0.1/iocbio/gel/app.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/application_state/context.py` & `iocbio.gel-1.0.1/iocbio/gel/application/application_state/context.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/application_state/state.py` & `iocbio.gel-1.0.1/iocbio/gel/application/application_state/state.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/container.py` & `iocbio.gel-1.0.1/iocbio/gel/application/container.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/event_consumer.py` & `iocbio.gel-1.0.1/iocbio/gel/application/event_consumer.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/event_registry.py` & `iocbio.gel-1.0.1/iocbio/gel/application/event_registry.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/file_digest.py` & `iocbio.gel-1.0.1/iocbio/gel/application/file_digest.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/image/background_method.py` & `iocbio.gel-1.0.1/iocbio/gel/application/image/background_method.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/image/image.py` & `iocbio.gel-1.0.1/iocbio/gel/application/image/image.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/image/image_source_setup.py` & `iocbio.gel-1.0.1/iocbio/gel/application/image/image_source_setup.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/image/omero_client.py` & `iocbio.gel-1.0.1/iocbio/gel/application/image/omero_client.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/image/processing_cache.py` & `iocbio.gel-1.0.1/iocbio/gel/application/image/processing_cache.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/image/region.py` & `iocbio.gel-1.0.1/iocbio/gel/application/image/region.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/image/repository_backend.py` & `iocbio.gel-1.0.1/iocbio/gel/application/image/repository_backend.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/image/repository_backend_local.py` & `iocbio.gel-1.0.1/iocbio/gel/application/image/repository_backend_local.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/image/repository_backend_omero.py` & `iocbio.gel-1.0.1/iocbio/gel/application/image/repository_backend_omero.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/number_list.py` & `iocbio.gel-1.0.1/iocbio/gel/application/number_list.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/settings_proxy.py` & `iocbio.gel-1.0.1/iocbio/gel/application/settings_proxy.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/thread/fetch_image_from_omero.py` & `iocbio.gel-1.0.1/iocbio/gel/application/thread/fetch_image_from_omero.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/thread/job.py` & `iocbio.gel-1.0.1/iocbio/gel/application/thread/job.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/thread/load_image_preview.py` & `iocbio.gel-1.0.1/iocbio/gel/application/thread/load_image_preview.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/thread/pool_worker.py` & `iocbio.gel-1.0.1/iocbio/gel/application/thread/pool_worker.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/thread/rolling_ball.py` & `iocbio.gel-1.0.1/iocbio/gel/application/thread/rolling_ball.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,42 +13,46 @@
 from skimage.transform import rescale, resize
 
 from iocbio.gel.application.image.background_method import BackgroundMethod
 from iocbio.gel.application.thread.job import Job
 
 
 class Signals(QObject):
-    ready: SignalInstance = Signal(int, np.ndarray, np.ndarray)
+    ready: SignalInstance = Signal(int, np.ndarray, np.ndarray, str)
 
 
 class RollingBall(Job):
     METHODS = [BackgroundMethod.BALL, BackgroundMethod.ELLIPSOID]
 
     def __init__(
         self,
         image_id,
         source_image,
         method,
         is_light,
         radius_x,
         radius_y,
-        should_scale: bool = True,
+        should_scale,
+        cache_key: str,
     ):
-        super().__init__(image_id, method, radius_x, radius_y, is_light, str(should_scale))
+        super().__init__(
+            image_id, method, radius_x, radius_y, is_light, str(should_scale), cache_key
+        )
         if method not in self.METHODS:
             raise ValueError(f'Unexpected method="{method}" provided for {self.__class__.__name__}')
 
         self.signals = Signals()
         self.image_id = image_id
         self.source_image = source_image
         self.method = method
         self.is_light = is_light
         self.radius_x = radius_x
         self.radius_y = radius_y if radius_y else radius_x
         self.should_scale = should_scale
+        self.cache_key = cache_key
 
     def run_job(self) -> None:
         pool = QThreadPool.globalInstance()
         thread_count = max(round(pool.maxThreadCount() - pool.activeThreadCount() / 2), 1)
         scale_factor = 1 if not self.should_scale else self._get_scale_factor()
 
         background, result = self._subtract_background(
@@ -57,15 +61,15 @@
             self.is_light,
             self.radius_x,
             self.radius_y,
             scale_factor=scale_factor,
             thread_count=thread_count,
         )
 
-        self.signals.ready.emit(self.image_id, background, result)
+        self.signals.ready.emit(self.image_id, background, result, self.cache_key)
 
     def supersedes(self, job: "Job") -> bool:
         return isinstance(job, self.__class__) and self.image_id == job.image_id
 
     def _get_scale_factor(self) -> int:
         radius = max(self.radius_x, self.radius_y)
         thresholds = [10, 30, 100, 400, 1200]
```

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/thread/sequential_worker.py` & `iocbio.gel-1.0.1/iocbio/gel/application/thread/sequential_worker.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/thread/thread_pool.py` & `iocbio.gel-1.0.1/iocbio/gel/application/thread/thread_pool.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/application/thread/worker.py` & `iocbio.gel-1.0.1/iocbio/gel/application/thread/worker.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/command/command_set.py` & `iocbio.gel-1.0.1/iocbio/gel/command/command_set.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/command/create_entity.py` & `iocbio.gel-1.0.1/iocbio/gel/command/create_entity.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/command/delete_collector.py` & `iocbio.gel-1.0.1/iocbio/gel/command/delete_collector.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/command/delete_entity.py` & `iocbio.gel-1.0.1/iocbio/gel/command/delete_entity.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/command/history_manager.py` & `iocbio.gel-1.0.1/iocbio/gel/command/history_manager.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/command/project_delete_collector.py` & `iocbio.gel-1.0.1/iocbio/gel/command/project_delete_collector.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/command/transaction_set.py` & `iocbio.gel-1.0.1/iocbio/gel/command/transaction_set.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/command/update_entity.py` & `iocbio.gel-1.0.1/iocbio/gel/command/update_entity.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/command/update_many_relationship.py` & `iocbio.gel-1.0.1/iocbio/gel/command/update_many_relationship.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/command/update_project.py` & `iocbio.gel-1.0.1/iocbio/gel/command/update_project.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/db/alembic/alembic.ini` & `iocbio.gel-1.0.1/iocbio/gel/db/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/db/alembic/env.py` & `iocbio.gel-1.0.1/iocbio/gel/db/alembic/env.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/db/alembic/versions/8b8ae59755af_synced_lane_widths.py` & `iocbio.gel-1.0.1/iocbio/gel/db/alembic/versions/8b8ae59755af_synced_lane_widths.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/db/alembic/versions/create_views_set_1.sql` & `iocbio.gel-1.0.1/iocbio/gel/db/alembic/versions/create_views_set_1.sql`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/db/alembic/versions/d8d292a431fe_allow_to_sync_measurement_rois.py` & `iocbio.gel-1.0.1/iocbio/gel/db/alembic/versions/d8d292a431fe_allow_to_sync_measurement_rois.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/db/alembic/versions/e78898a9c9f1_change_transfer_to_ref_time.py` & `iocbio.gel-1.0.1/iocbio/gel/db/alembic/versions/e78898a9c9f1_change_transfer_to_ref_time.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/db/alembic/versions/fbf8b6944c61_limit_protein_to_non_negative_value.py` & `iocbio.gel-1.0.1/iocbio/gel/db/alembic/versions/fbf8b6944c61_limit_protein_to_non_negative_value.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/db/alembic/versions/fd339f2a6eb4_projects.py` & `iocbio.gel-1.0.1/iocbio/gel/db/alembic/versions/fd339f2a6eb4_projects.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/db/alembic/versions/nrobvvzilln3_create_views.py` & `iocbio.gel-1.0.1/iocbio/gel/db/alembic/versions/nrobvvzilln3_create_views.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/db/alembic/versions/wrsc7ffn1q95_revised_initial_version.py` & `iocbio.gel-1.0.1/iocbio/gel/db/alembic/versions/wrsc7ffn1q95_revised_initial_version.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/db/base.py` & `iocbio.gel-1.0.1/iocbio/gel/db/base.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/db/connection_parameters/postgresql_parameters.py` & `iocbio.gel-1.0.1/iocbio/gel/db/connection_parameters/postgresql_parameters.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/db/connection_parameters/sqlite_parameters.py` & `iocbio.gel-1.0.1/iocbio/gel/db/connection_parameters/sqlite_parameters.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/db/database_client.py` & `iocbio.gel-1.0.1/iocbio/gel/db/database_client.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/db/database_setup.py` & `iocbio.gel-1.0.1/iocbio/gel/db/database_setup.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/db/database_type.py` & `iocbio.gel-1.0.1/iocbio/gel/db/database_type.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/domain/curved_lane_region.py` & `iocbio.gel-1.0.1/iocbio/gel/domain/curved_lane_region.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/domain/detect_analysis_region.py` & `iocbio.gel-1.0.1/iocbio/gel/domain/detect_analysis_region.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/domain/gel.py` & `iocbio.gel-1.0.1/iocbio/gel/domain/gel.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/domain/gel_image.py` & `iocbio.gel-1.0.1/iocbio/gel/domain/gel_image.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/domain/gel_image_lane.py` & `iocbio.gel-1.0.1/iocbio/gel/domain/gel_image_lane.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/domain/gel_lane.py` & `iocbio.gel-1.0.1/iocbio/gel/domain/gel_lane.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/domain/measurement.py` & `iocbio.gel-1.0.1/iocbio/gel/domain/measurement.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/domain/measurement_lane.py` & `iocbio.gel-1.0.1/iocbio/gel/domain/measurement_lane.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/domain/measurement_type.py` & `iocbio.gel-1.0.1/iocbio/gel/domain/measurement_type.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/domain/plot.py` & `iocbio.gel-1.0.1/iocbio/gel/domain/plot.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/domain/plot_region.py` & `iocbio.gel-1.0.1/iocbio/gel/domain/plot_region.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/domain/project.py` & `iocbio.gel-1.0.1/iocbio/gel/domain/project.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/domain/xls_writer.py` & `iocbio.gel-1.0.1/iocbio/gel/domain/xls_writer.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/contexts/analysis.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/contexts/analysis.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/contexts/gels.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/contexts/gels.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/contexts/measurement_types.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/contexts/measurement_types.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/contexts/projects.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/contexts/projects.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/contexts/settings.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/contexts/settings.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/contexts/single_gel.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/contexts/single_gel.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/database_connection_settings/db_selection_form.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/database_connection_settings/db_selection_form.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/database_connection_settings/postgresql_connection_settings.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/database_connection_settings/postgresql_connection_settings.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/database_connection_settings/sqlite_connection_settings.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/database_connection_settings/sqlite_connection_settings.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/db_selection.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/db_selection.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/image_source_settings/image_source_form.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/image_source_settings/image_source_form.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/image_source_settings/image_source_settings.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/image_source_settings/image_source_settings.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/image_source_settings/local_settings.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/image_source_settings/local_settings.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/image_source_settings/omero_settings.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/image_source_settings/omero_settings.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/select_image_factory.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/select_image_factory.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/select_image_local.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/select_image_local.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/dialogs/select_image_omero.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/dialogs/select_image_omero.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/icons.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/icons.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/models/checkbox_proxy.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/models/checkbox_proxy.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/models/gel_images_model.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/models/gel_images_model.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/models/gel_lanes_model.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/models/gel_lanes_model.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/models/gels_model.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/models/gels_model.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/models/items/tree_item.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/models/items/tree_item.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/models/measurement_lanes_model.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/models/measurement_lanes_model.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/models/measurement_types_model.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/models/measurement_types_model.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/models/measurements_model.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/models/measurements_model.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/models/projects_gels_model.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/models/projects_gels_model.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/models/projects_tree_model.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/models/projects_tree_model.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/models/proxy_table_model.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/models/proxy_table_model.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/models/table_model.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/models/table_model.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/models/tracking_model.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/models/tracking_model.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/models/tree_model.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/models/tree_model.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/resources/rc_icons.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/resources/rc_icons.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/user_resized.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/user_resized.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/views/delegates/combobox_delegate.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/views/delegates/combobox_delegate.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/views/delegates/datetime_delegate.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/views/delegates/datetime_delegate.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/views/delegates/multiselect_delegate.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/views/delegates/multiselect_delegate.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/views/delegates/nobackground_delegate.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/views/delegates/nobackground_delegate.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/views/delegates/non_negative_double.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/views/delegates/non_negative_double.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/views/delegates/selectable_row_delegate.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/views/delegates/selectable_row_delegate.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/views/gel_images_view.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/views/gel_images_view.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/views/table_view.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/views/table_view.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/views/tree_view.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/views/tree_view.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/active_lanes.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/active_lanes.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/adjust.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/adjust.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/adjust_roi.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/adjust_roi.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/background/ball_layout.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/background/ball_layout.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/background/bg_color_box.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/background/bg_color_box.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/background/bg_subtraction_box.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/background/bg_subtraction_box.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/background/ellipsoid_layout.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/background/ellipsoid_layout.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/background_subtraction.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/background_subtraction.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/curved_line_roi.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/curved_line_roi.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/intensity/intensity_plot.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/intensity/intensity_plot.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/intensity/lane_intensity_plot.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/intensity/lane_intensity_plot.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/intensity/lane_plot_list.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/intensity/lane_plot_list.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/intensity/measurement_intensity_plot.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/intensity/measurement_intensity_plot.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/intensity/measurement_plot_list.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/intensity/measurement_plot_list.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/intensity/plot_list.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/intensity/plot_list.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/intensity/zero_line.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/intensity/zero_line.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/passive_lanes.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/passive_lanes.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/analysis_steps/raw.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/analysis_steps/raw.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/confirm_popup.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/confirm_popup.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/control_slider.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/control_slider.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/gel_form.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/gel_form.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/gel_image_form.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/gel_image_form.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/gel_measurements.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/gel_measurements.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/mandatory_line_edit.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/mandatory_line_edit.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/measurement_lanes.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/measurement_lanes.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/multiple_project_selection.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/multiple_project_selection.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/project_selection.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/project_selection.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/sidebar.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/sidebar.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/status_bar.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/status_bar.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/toolbars/add_gel.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/toolbars/add_gel.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/toolbars/main.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/toolbars/main.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/widgets/viewbox_empty_contextmenu.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/widgets/viewbox_empty_contextmenu.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/gui/windows/main.py` & `iocbio.gel-1.0.1/iocbio/gel/gui/windows/main.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/logging.ini` & `iocbio.gel-1.0.1/iocbio/gel/logging.ini`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/repository/entity_repository.py` & `iocbio.gel-1.0.1/iocbio/gel/repository/entity_repository.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/repository/export_repository.py` & `iocbio.gel-1.0.1/iocbio/gel/repository/export_repository.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/repository/gel_image_lane_repository.py` & `iocbio.gel-1.0.1/iocbio/gel/repository/gel_image_lane_repository.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/repository/gel_image_repository.py` & `iocbio.gel-1.0.1/iocbio/gel/repository/gel_image_repository.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/repository/gel_lane_repository.py` & `iocbio.gel-1.0.1/iocbio/gel/repository/gel_lane_repository.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/repository/gel_repository.py` & `iocbio.gel-1.0.1/iocbio/gel/repository/gel_repository.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/repository/image_repository.py` & `iocbio.gel-1.0.1/iocbio/gel/repository/image_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,29 +130,35 @@
             result = Region.crop(gel_image, image.raw)
             image.region = result
             self.processing_cache.set(cache_key, result)
 
         return image
 
     def _attach_background(self, gel_image: GelImage, image: Image) -> Image:
+        if gel_image.background_method == BackgroundMethod.FLAT:
+            background_value = np.percentile(image.region, self.FLAT_PERCENTILE)
+            image.background = np.full(image.region.shape, background_value)
+            image.subtracted = image.region - background_value
+            image.state = ImageState.READY
+            return image
+
+        if gel_image.background_method == BackgroundMethod.NONE:
+            image.state = ImageState.READY
+            return image
+
         cached = self.processing_cache.get(ProcessingCache.background_key(gel_image))
         if cached is not None:
             image.background = cached[0]
             image.subtracted = cached[1]
             image.state = ImageState.READY
             return image
 
         if self._can_defer_background_job(gel_image):
             return self._defer_bg_subtraction(gel_image, image)
 
-        if gel_image.background_method == BackgroundMethod.FLAT:
-            background_value = np.percentile(image.region, self.FLAT_PERCENTILE)
-            image.background = np.full(image.region.shape, background_value)
-            image.subtracted = image.region - background_value
-
         image.state = ImageState.READY
         return image
 
     def _defer_preview_loading(self, gel_image: GelImage, image: Image) -> Image:
         self.images[gel_image.id] = image
 
         job = LoadImagePreview(gel_image.id, image)
@@ -168,14 +174,15 @@
             gel_image.id,
             image.region,
             gel_image.background_method,
             not gel_image.background_is_dark,
             gel_image.background_radius_x,
             gel_image.background_radius_y,
             gel_image.background_scale,
+            ProcessingCache.background_key(gel_image),
         )
 
         job.signals.ready.connect(self._handle_subtraction_result)
         self.thread_pool.start(job)
 
         return image
 
@@ -203,18 +210,22 @@
     @Slot(int, Image)
     def _handle_preview_loading(self, gel_image_id: int, image: Image):
         gel_image = self.gel_image_repository.get(gel_image_id)
         self.set(gel_image.id, image)
         image = self.get(gel_image)
         self._emit_image_ready(gel_image, image)
 
-    @Slot(int, np.ndarray, np.ndarray)
-    def _handle_subtraction_result(self, image_id, background, subtracted):
+    @Slot(int, np.ndarray, np.ndarray, str)
+    def _handle_subtraction_result(self, image_id, background, subtracted, cache_key):
         gel_image = self.gel_image_repository.get(image_id)
 
+        if ProcessingCache.background_key(gel_image) != cache_key:
+            self.event_registry.set_status_message("Dropping expired subtraction")
+            return
+
         self.processing_cache.set(
             ProcessingCache.background_key(gel_image), [background, subtracted]
         )
 
         image = self.images.get(image_id)
         image.background = background
         image.subtracted = subtracted
```

### Comparing `iocbio.gel-1.0.0/iocbio/gel/repository/measurement_lane_repository.py` & `iocbio.gel-1.0.1/iocbio/gel/repository/measurement_lane_repository.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/repository/measurement_repository.py` & `iocbio.gel-1.0.1/iocbio/gel/repository/measurement_repository.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/repository/measurement_type_repository.py` & `iocbio.gel-1.0.1/iocbio/gel/repository/measurement_type_repository.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio/gel/repository/project_repository.py` & `iocbio.gel-1.0.1/iocbio/gel/repository/project_repository.py`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/iocbio.gel.egg-info/PKG-INFO` & `iocbio.gel-1.0.1/iocbio.gel.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iocbio.gel
-Version: 1.0.0
+Version: 1.0.1
 Summary: IOCBio Gel
 Home-page: https://iocbio.gitlab.io/gel
 Author: IOCBio team
 Author-email: iocbio@sysbio.ioc.ee
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `iocbio.gel-1.0.0/iocbio.gel.egg-info/SOURCES.txt` & `iocbio.gel-1.0.1/iocbio.gel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/packaging/pyinstaller/app.spec` & `iocbio.gel-1.0.1/packaging/pyinstaller/app.spec`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/requirements.txt` & `iocbio.gel-1.0.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/resources/icons/feather/readme-and-license.md` & `iocbio.gel-1.0.1/resources/icons/feather/readme-and-license.md`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/resources/icons/gel.svg` & `iocbio.gel-1.0.1/resources/icons/gel.svg`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/setup.py` & `iocbio.gel-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="iocbio.gel",
-    version="1.0.0",
+    version="1.0.1",
     description="IOCBio Gel",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="IOCBio team",
     author_email="iocbio@sysbio.ioc.ee",
     license="GPLv3",
     url="https://iocbio.gitlab.io/gel",
```

### Comparing `iocbio.gel-1.0.0/sql/README.md` & `iocbio.gel-1.0.1/sql/README.md`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/sql/gel_raw_data.sql` & `iocbio.gel-1.0.1/sql/gel_raw_data.sql`

 * *Files identical despite different names*

### Comparing `iocbio.gel-1.0.0/sql/gel_relative_data.sql` & `iocbio.gel-1.0.1/sql/gel_relative_data.sql`

 * *Files identical despite different names*

