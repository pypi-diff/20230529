# Comparing `tmp/mitzu-0.6.0rc9.tar.gz` & `tmp/mitzu-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitzu-0.6.0rc9.tar", max compression
+gzip compressed data, was "mitzu-0.6.1.tar", max compression
```

## Comparing `mitzu-0.6.0rc9.tar` & `mitzu-0.6.1.tar`

### file list

```diff
@@ -1,125 +1,136 @@
--rw-r--r--   0        0        0     1082 2023-05-15 19:57:09.432988 mitzu-0.6.0rc9/LICENSE.txt
--rw-r--r--   0        0        0     2235 2023-05-15 19:57:09.432988 mitzu-0.6.0rc9/README.md
--rw-r--r--   0        0        0     6148 2023-05-15 19:57:09.824990 mitzu-0.6.0rc9/mitzu/.DS_Store
--rw-r--r--   0        0        0      865 2023-05-15 19:58:06.717343 mitzu-0.6.0rc9/mitzu/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 19:57:09.824990 mitzu-0.6.0rc9/mitzu/adapters/__init__.py
--rw-r--r--   0        0        0     1918 2023-05-15 19:57:09.824990 mitzu-0.6.0rc9/mitzu/adapters/adapter_factory.py
--rw-r--r--   0        0        0     5148 2023-05-15 19:57:09.824990 mitzu-0.6.0rc9/mitzu/adapters/athena_adapter.py
--rw-r--r--   0        0        0     3390 2023-05-15 19:57:09.824990 mitzu-0.6.0rc9/mitzu/adapters/bigquery_adapter.py
--rw-r--r--   0        0        0     6026 2023-05-15 19:57:09.824990 mitzu-0.6.0rc9/mitzu/adapters/databricks_adapter.py
--rw-r--r--   0        0        0     2261 2023-05-15 19:57:09.824990 mitzu-0.6.0rc9/mitzu/adapters/file_adapter.py
--rw-r--r--   0        0        0     2533 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/generic_adapter.py
--rw-r--r--   0        0        0      898 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/helper.py
--rw-r--r--   0        0        0     3422 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/mysql_adapter.py
--rw-r--r--   0        0        0     2297 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/postgresql_adapter.py
--rw-r--r--   0        0        0     3733 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/redshift_adapter.py
--rw-r--r--   0        0        0     3298 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/snowflake_adapter.py
--rw-r--r--   0        0        0        0 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      660 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/__init__.py
--rw-r--r--   0        0        0      701 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5071 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6415 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
--rw-r--r--   0        0        0     9751 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1844 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
--rw-r--r--   0        0        0      672 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/databricks/__init__.py
--rw-r--r--   0        0        0      713 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5010 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6601 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
--rw-r--r--   0        0        0    10073 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1848 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
--rw-r--r--   0        0        0    39624 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy_adapter.py
--rw-r--r--   0        0        0     4963 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/sqlite_adapter.py
--rw-r--r--   0        0        0     6614 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/adapters/trino_adapter.py
--rw-r--r--   0        0        0     1835 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/helper.py
--rw-r--r--   0        0        0    53963 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/model.py
--rw-r--r--   0        0        0        0 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/notebook/__init__.py
--rw-r--r--   0        0        0     6818 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/notebook/model_loader.py
--rw-r--r--   0        0        0     3306 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/project_discovery.py
--rw-r--r--   0        0        0     2102 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/project_serialization.py
--rw-r--r--   0        0        0      785 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/samples/__init__.py
--rw-r--r--   0        0        0     3794 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/samples/data_ingestion.py
--rw-r--r--   0        0        0    10141 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/samples/sample_data_generator.py
--rw-r--r--   0        0        0    11926 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/serialization.py
--rw-r--r--   0        0        0        0 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/visualization/__init__.py
--rw-r--r--   0        0        0     7022 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/visualization/charts.py
--rw-r--r--   0        0        0     1866 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/visualization/common.py
--rw-r--r--   0        0        0      941 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/visualization/labels.py
--rw-r--r--   0        0        0     7802 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/visualization/plot.py
--rw-r--r--   0        0        0     5767 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/visualization/titles.py
--rw-r--r--   0        0        0     3181 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/visualization/tooltips.py
--rw-r--r--   0        0        0     3339 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/visualization/transform_conv.py
--rw-r--r--   0        0        0     1278 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/visualization/transform_retention.py
--rw-r--r--   0        0        0     6148 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/webapp/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/webapp/__init__.py
--rw-r--r--   0        0        0     5347 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/webapp/assets/explore_page.css
--rw-r--r--   0        0        0   147145 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/webapp/assets/favicon.ico
--rw-r--r--   0        0        0    46702 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/webapp/assets/logo.png
--rw-r--r--   0        0        0    43472 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/webapp/assets/mitzu-logo-light.svg
--rw-r--r--   0        0        0    49422 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/athena.png
--rw-r--r--   0        0        0    20802 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/bigquery.png
--rw-r--r--   0        0        0    10321 2023-05-15 19:57:09.828990 mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/clickhouse.png
--rw-r--r--   0        0        0   119554 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/databricks.png
--rw-r--r--   0        0        0     3008 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/mysql.png
--rw-r--r--   0        0        0     2446 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/pandas.png
--rw-r--r--   0        0        0     5338 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/postgresql.png
--rw-r--r--   0        0        0     8512 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/redshift.png
--rw-r--r--   0        0        0    93500 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/snowflake.png
--rw-r--r--   0        0        0    48681 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/sqlite.png
--rw-r--r--   0        0        0    34219 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/trino.png
--rw-r--r--   0        0        0    13716 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/auth/authorizer.py
--rw-r--r--   0        0        0     3557 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/auth/cognito.py
--rw-r--r--   0        0        0     1594 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/auth/decorator.py
--rw-r--r--   0        0        0     2777 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/auth/google.py
--rw-r--r--   0        0        0     7481 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/cache.py
--rw-r--r--   0        0        0     2920 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/caching_dataset_adapter.py
--rw-r--r--   0        0        0     1462 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/configs.py
--rw-r--r--   0        0        0     3088 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/dependencies.py
--rw-r--r--   0        0        0     4833 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/helper.py
--rw-r--r--   0        0        0     8375 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/model.py
--rw-r--r--   0        0        0      408 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/navbar.py
--rw-r--r--   0        0        0     5435 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/offcanvas.py
--rw-r--r--   0        0        0        0 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/connections/__init__.py
--rw-r--r--   0        0        0    16230 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/connections/manage_connections_component.py
--rw-r--r--   0        0        0     4527 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/connections_page.py
--rw-r--r--   0        0        0        0 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/dashboards/__init__.py
--rw-r--r--   0        0        0    20885 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
--rw-r--r--   0        0        0     9787 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/dashboards_page.py
--rw-r--r--   0        0        0    14654 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/edit_user.py
--rw-r--r--   0        0        0        0 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore/__init__.py
--rw-r--r--   0        0        0     5724 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore/complex_segment_handler.py
--rw-r--r--   0        0        0     6488 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore/dates_selector_handler.py
--rw-r--r--   0        0        0     5564 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore/event_segment_handler.py
--rw-r--r--   0        0        0    21781 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore/explore_page.py
--rw-r--r--   0        0        0     9604 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore/graph_handler.py
--rw-r--r--   0        0        0    10940 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore/metric_config_handler.py
--rw-r--r--   0        0        0     2375 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore/metric_segments_handler.py
--rw-r--r--   0        0        0     1565 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore/metric_type_handler.py
--rw-r--r--   0        0        0     9783 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore/simple_segment_handler.py
--rw-r--r--   0        0        0     4644 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore/toolbar_handler.py
--rw-r--r--   0        0        0     1347 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/explore_project.py
--rw-r--r--   0        0        0     1751 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/home.py
--rw-r--r--   0        0        0     4107 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/login.py
--rw-r--r--   0        0        0     5027 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/manage_connection.py
--rw-r--r--   0        0        0     1387 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/manage_dashboard.py
--rw-r--r--   0        0        0    10191 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/manage_event_defs.py
--rw-r--r--   0        0        0    11953 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/manage_project.py
--rw-r--r--   0        0        0     9629 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/manage_saved_metrics.py
--rw-r--r--   0        0        0     1738 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/paths.py
--rw-r--r--   0        0        0        0 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/projects/__init__.py
--rw-r--r--   0        0        0    36159 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/projects/event_tables_config.py
--rw-r--r--   0        0        0      587 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/projects/helper.py
--rw-r--r--   0        0        0     9400 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/projects/manage_project_component.py
--rw-r--r--   0        0        0     5155 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/projects_page.py
--rw-r--r--   0        0        0     3185 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/pages/users.py
--rw-r--r--   0        0        0        0 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/service/__init__.py
--rw-r--r--   0        0        0     2207 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/service/events_service.py
--rw-r--r--   0        0        0     5302 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/service/navbar_service.py
--rw-r--r--   0        0        0      670 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/service/notification_service.py
--rw-r--r--   0        0        0     2105 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/service/secret_service.py
--rw-r--r--   0        0        0     4719 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/service/user_service.py
--rw-r--r--   0        0        0    23896 2023-05-15 19:57:09.832990 mitzu-0.6.0rc9/mitzu/webapp/storage.py
--rw-r--r--   0        0        0    25781 2023-05-15 19:57:09.836990 mitzu-0.6.0rc9/mitzu/webapp/storage_model.py
--rw-r--r--   0        0        0     4744 2023-05-15 19:57:09.836990 mitzu-0.6.0rc9/mitzu/webapp/webapp.py
--rw-r--r--   0        0        0     3055 2023-05-15 19:58:06.717343 mitzu-0.6.0rc9/pyproject.toml
--rw-r--r--   0        0        0     4799 1970-01-01 00:00:00.000000 mitzu-0.6.0rc9/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-29 11:48:37.423694 mitzu-0.6.1/LICENSE.txt
+-rw-r--r--   0        0        0     2235 2023-05-29 11:48:37.423694 mitzu-0.6.1/README.md
+-rw-r--r--   0        0        0     6148 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/.DS_Store
+-rw-r--r--   0        0        0      860 2023-05-29 11:50:04.368327 mitzu-0.6.1/mitzu/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/__init__.py
+-rw-r--r--   0        0        0     1918 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/adapter_factory.py
+-rw-r--r--   0        0        0     5148 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/athena_adapter.py
+-rw-r--r--   0        0        0     6262 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/bigquery_adapter.py
+-rw-r--r--   0        0        0     6026 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/databricks_adapter.py
+-rw-r--r--   0        0        0     2261 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/file_adapter.py
+-rw-r--r--   0        0        0     2533 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/generic_adapter.py
+-rw-r--r--   0        0        0      898 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/helper.py
+-rw-r--r--   0        0        0     3422 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/mysql_adapter.py
+-rw-r--r--   0        0        0     2297 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/postgresql_adapter.py
+-rw-r--r--   0        0        0     3765 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/redshift_adapter.py
+-rw-r--r--   0        0        0     3298 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/snowflake_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/athena/__init__.py
+-rw-r--r--   0        0        0      701 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5071 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6415 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0     9751 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1844 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
+-rw-r--r--   0        0        0        0 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/__init__.py
+-rw-r--r--   0        0        0     2146 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2412 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_helpers.py
+-rw-r--r--   0        0        0     5071 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_struct.py
+-rw-r--r--   0        0        0     4770 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_types.py
+-rw-r--r--   0        0        0    38550 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     8638 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/geography.py
+-rw-r--r--   0        0        0     9854 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/parse_url.py
+-rw-r--r--   0        0        0     7361 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/requirements.py
+-rw-r--r--   0        0        0     1131 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/version.py
+-rw-r--r--   0        0        0        0 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/databricks/__init__.py
+-rw-r--r--   0        0        0      713 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5010 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6601 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0    10073 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1848 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
+-rw-r--r--   0        0        0    40105 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy_adapter.py
+-rw-r--r--   0        0        0     4963 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlite_adapter.py
+-rw-r--r--   0        0        0     7705 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/trino_adapter.py
+-rw-r--r--   0        0        0     1835 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/helper.py
+-rw-r--r--   0        0        0    53991 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/model.py
+-rw-r--r--   0        0        0        0 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/notebook/__init__.py
+-rw-r--r--   0        0        0     6845 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/notebook/model_loader.py
+-rw-r--r--   0        0        0     2550 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/project_discovery.py
+-rw-r--r--   0        0        0     2102 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/project_serialization.py
+-rw-r--r--   0        0        0      785 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/samples/__init__.py
+-rw-r--r--   0        0        0     3794 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/samples/data_ingestion.py
+-rw-r--r--   0        0        0    10141 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/samples/sample_data_generator.py
+-rw-r--r--   0        0        0    11933 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/serialization.py
+-rw-r--r--   0        0        0        0 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/visualization/__init__.py
+-rw-r--r--   0        0        0     7305 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/visualization/charts.py
+-rw-r--r--   0        0        0     1866 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/visualization/common.py
+-rw-r--r--   0        0        0      941 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/visualization/labels.py
+-rw-r--r--   0        0        0     7802 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/visualization/plot.py
+-rw-r--r--   0        0        0     5767 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/visualization/titles.py
+-rw-r--r--   0        0        0     3181 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/visualization/tooltips.py
+-rw-r--r--   0        0        0     3289 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/visualization/transform_conv.py
+-rw-r--r--   0        0        0     1222 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/visualization/transform_retention.py
+-rw-r--r--   0        0        0     6148 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/__init__.py
+-rw-r--r--   0        0        0     5347 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/explore_page.css
+-rw-r--r--   0        0        0   147145 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/favicon.ico
+-rw-r--r--   0        0        0    46702 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/logo.png
+-rw-r--r--   0        0        0    43472 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/mitzu-logo-light.svg
+-rw-r--r--   0        0        0    49422 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/warehouse/athena.png
+-rw-r--r--   0        0        0    20802 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/warehouse/bigquery.png
+-rw-r--r--   0        0        0    10321 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/warehouse/clickhouse.png
+-rw-r--r--   0        0        0   119554 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/warehouse/databricks.png
+-rw-r--r--   0        0        0     3008 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/warehouse/mysql.png
+-rw-r--r--   0        0        0     2446 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/warehouse/pandas.png
+-rw-r--r--   0        0        0     5338 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/warehouse/postgresql.png
+-rw-r--r--   0        0        0     8512 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/warehouse/redshift.png
+-rw-r--r--   0        0        0    93500 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/warehouse/snowflake.png
+-rw-r--r--   0        0        0    48681 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/warehouse/sqlite.png
+-rw-r--r--   0        0        0    34219 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/warehouse/trino.png
+-rw-r--r--   0        0        0    15436 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/auth/authorizer.py
+-rw-r--r--   0        0        0     3557 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/auth/cognito.py
+-rw-r--r--   0        0        0     1305 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/auth/decorator.py
+-rw-r--r--   0        0        0     2777 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/auth/google.py
+-rw-r--r--   0        0        0     7481 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/cache.py
+-rw-r--r--   0        0        0     2920 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/caching_dataset_adapter.py
+-rw-r--r--   0        0        0     1664 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/configs.py
+-rw-r--r--   0        0        0     3432 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/dependencies.py
+-rw-r--r--   0        0        0     4984 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/helper.py
+-rw-r--r--   0        0        0     8375 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/model.py
+-rw-r--r--   0        0        0      309 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/navbar.py
+-rw-r--r--   0        0        0     5435 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/offcanvas.py
+-rw-r--r--   0        0        0        0 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/connections/__init__.py
+-rw-r--r--   0        0        0    22633 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/connections/manage_connections_component.py
+-rw-r--r--   0        0        0     4428 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/connections_page.py
+-rw-r--r--   0        0        0        0 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/dashboards/__init__.py
+-rw-r--r--   0        0        0    20561 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
+-rw-r--r--   0        0        0     9628 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/dashboards_page.py
+-rw-r--r--   0        0        0    14456 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/edit_user.py
+-rw-r--r--   0        0        0        0 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore/__init__.py
+-rw-r--r--   0        0        0     5738 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore/complex_segment_handler.py
+-rw-r--r--   0        0        0     6488 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore/dates_selector_handler.py
+-rw-r--r--   0        0        0     5564 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore/event_segment_handler.py
+-rw-r--r--   0        0        0    21704 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore/explore_page.py
+-rw-r--r--   0        0        0    10100 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore/graph_handler.py
+-rw-r--r--   0        0        0    10940 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore/metric_config_handler.py
+-rw-r--r--   0        0        0     2375 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore/metric_segments_handler.py
+-rw-r--r--   0        0        0     1565 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore/metric_type_handler.py
+-rw-r--r--   0        0        0     9772 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore/simple_segment_handler.py
+-rw-r--r--   0        0        0     4644 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore/toolbar_handler.py
+-rw-r--r--   0        0        0     1221 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore_project.py
+-rw-r--r--   0        0        0     1751 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/home.py
+-rw-r--r--   0        0        0     3947 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/login.py
+-rw-r--r--   0        0        0     5023 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/manage_connection.py
+-rw-r--r--   0        0        0     1288 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/manage_dashboard.py
+-rw-r--r--   0        0        0    10104 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/manage_event_defs.py
+-rw-r--r--   0        0        0    11845 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/manage_project.py
+-rw-r--r--   0        0        0     9470 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/manage_saved_metrics.py
+-rw-r--r--   0        0        0     1738 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/paths.py
+-rw-r--r--   0        0        0        0 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/projects/__init__.py
+-rw-r--r--   0        0        0    35694 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/projects/event_tables_config.py
+-rw-r--r--   0        0        0      587 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/projects/helper.py
+-rw-r--r--   0        0        0     9400 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/projects/manage_project_component.py
+-rw-r--r--   0        0        0     5075 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/projects_page.py
+-rw-r--r--   0        0        0     3114 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/users.py
+-rw-r--r--   0        0        0        0 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/service/__init__.py
+-rw-r--r--   0        0        0     2156 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/service/events_service.py
+-rw-r--r--   0        0        0     5064 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/service/navbar_service.py
+-rw-r--r--   0        0        0      670 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/service/notification_service.py
+-rw-r--r--   0        0        0     2105 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/service/secret_service.py
+-rw-r--r--   0        0        0     6650 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/service/tracking_service.py
+-rw-r--r--   0        0        0     4719 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/service/user_service.py
+-rw-r--r--   0        0        0    23895 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/storage.py
+-rw-r--r--   0        0        0    25760 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/storage_model.py
+-rw-r--r--   0        0        0     4700 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/webapp.py
+-rw-r--r--   0        0        0     3422 2023-05-29 11:50:04.364327 mitzu-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     5152 1970-01-01 00:00:00.000000 mitzu-0.6.1/PKG-INFO
```

### Comparing `mitzu-0.6.0rc9/LICENSE.txt` & `mitzu-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/README.md` & `mitzu-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/.DS_Store` & `mitzu-0.6.1/mitzu/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/__init__.py` & `mitzu-0.6.1/mitzu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     TimeWindow,
     TimeGroup,
     DiscoverySettings,
     WebappSettings,
 )
 from mitzu.samples import get_sample_discovered_project
 
-__version__ = "0.6.0-rc.9"
+__version__ = "0.6.1"
 
 
 __all__ = [
     "Connection",
     "ConnectionType",
     "Project",
     "EventDataTable",
```

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/adapter_factory.py` & `mitzu-0.6.1/mitzu/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/athena_adapter.py` & `mitzu-0.6.1/mitzu/adapters/athena_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/bigquery_adapter.py` & `mitzu-0.6.1/mitzu/adapters/mysql_adapter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,100 +1,93 @@
 from __future__ import annotations
 
-from typing import Any, List, Union
+from typing import Any
 
+import mitzu.adapters.generic_adapter as GA
 import mitzu.model as M
 import pandas as pd
-from mitzu.adapters.sqlalchemy_adapter import SQLAlchemyAdapter, FieldReference
-import mitzu.adapters.generic_adapter as GA
-import sqlalchemy as SA
-from mitzu.adapters.helper import pdf_string_json_array_to_array
+from mitzu.adapters.sqlalchemy_adapter import FieldReference, SQLAlchemyAdapter
 
+import sqlalchemy as SA
 import sqlalchemy.sql.expression as EXP
 
+NULL_VALUE_KEY = "##NULL##"
+
 
-class BigQueryAdapter(SQLAlchemyAdapter):
+class MySQLAdapter(SQLAlchemyAdapter):
     def __init__(self, project: M.Project):
         super().__init__(project)
 
-    def get_engine(self) -> Any:
-        con = self.project.connection
-        if self._engine is None:
-            if con.url is None:
-                url = self._get_connection_url(con)
-            else:
-                url = con.url
-            credentials = con.extra_configs.get("credentials")
-            if not credentials:
-                raise Exception(
-                    "Connection extra_configs must contain credentials json."
-                )
-            self._engine = SA.create_engine(url, credentials_info=credentials)
-        return self._engine
-
-    def execute_query(self, query: Any) -> pd.DataFrame:
-        if type(query) != str:
-            query = str(query.compile(compile_kwargs={"literal_binds": True}))
-
-        res = super().execute_query(query=query)
-
-        return res
-
-    def get_field_reference(
-        self,
-        field: M.Field,
-        event_data_table: M.EventDataTable = None,
-        sa_table: Union[SA.Table, EXP.CTE] = None,
-    ):
-        field_ref = super().get_field_reference(
-            field=field, event_data_table=event_data_table, sa_table=sa_table
-        )
-        if field._type == M.DataType.DATETIME:
-            field_ref = SA.func.datetime(field_ref)
-        return field_ref
-
-    def _get_sample_function(self):
-        return SA.func.mod(SA.cast(self._get_random_function() * 1367, SA.Integer), 100)
-
-    def _get_random_function(self):
-        return SA.func.rand()
-
     def _get_distinct_array_agg_func(self, field_ref: FieldReference) -> Any:
-        return SA.func.to_json(SA.func.array_agg(SA.distinct(field_ref)))
+        return SA.func.cast(
+            SA.func.json_keys(
+                SA.func.json_objectagg(SA.func.coalesce(field_ref, NULL_VALUE_KEY), "")
+            ),
+            SA.JSON,
+        )
 
-    def _get_date_trunc(
-        self, time_group: M.TimeGroup, field_ref: FieldReference
+    def _get_datetime_interval(
+        self, field_ref: FieldReference, timewindow: M.TimeWindow
     ) -> Any:
-        return SA.func.date_trunc(field_ref, SA.literal_column(time_group.name))
-
-    def _get_column_values_df(
-        self,
-        event_data_table: M.EventDataTable,
-        fields: List[M.Field],
-    ) -> pd.DataFrame:
-        df = super()._get_column_values_df(
-            event_data_table=event_data_table,
-            fields=fields,
-        )
-        return pdf_string_json_array_to_array(df)
+        return field_ref + SA.text(f"interval {timewindow.value} {timewindow.period}")
 
     def _get_dynamic_datetime_interval(
         self,
         field_ref: FieldReference,
         value_field_ref: FieldReference,
         time_group: M.TimeGroup,
     ) -> Any:
-        return SA.func.datetime_add(
-            field_ref,
-            SA.literal_column(f"interval {value_field_ref} {time_group.name.lower()}"),
-        )
+        return field_ref + SA.text(f"interval {value_field_ref} {time_group}")
+
+    def _get_date_trunc(self, time_group: M.TimeGroup, field_ref: FieldReference):
+        if time_group == M.TimeGroup.WEEK:
+            return SA.func.date_add(
+                SA.func.date(field_ref),
+                EXP.text(f"interval -{SA.func.weekday(field_ref)} day"),
+            )
+
+        elif time_group == M.TimeGroup.SECOND:
+            fmt = "%Y-%m-%dT%H:%i:%S"
+        elif time_group == M.TimeGroup.MINUTE:
+            fmt = "%Y-%m-%dT%H:%i:00"
+        elif time_group == M.TimeGroup.HOUR:
+            fmt = "%Y-%m-%dT%H:00:00"
+        elif time_group == M.TimeGroup.DAY:
+            fmt = "%Y-%m-%d"
+        elif time_group == M.TimeGroup.MONTH:
+            fmt = "%Y-%m-01"
+        elif time_group == M.TimeGroup.QUARTER:
+            raise NotImplementedError(
+                "Timegroup Quarter is not supported for MySQL Adapter"
+            )
+        elif time_group == M.TimeGroup.YEAR:
+            fmt = "%Y-01-01"
+
+        return SA.func.timestamp(SA.func.date_format(field_ref, fmt))
 
     def _get_conv_aggregation(
         self, metric: M.Metric, cte: EXP.CTE, first_cte: EXP.CTE
     ) -> Any:
-
+        if metric._agg_type == M.AggType.PERCENTILE_TIME_TO_CONV:
+            raise NotImplementedError(
+                "Percentile calculation is not supported by MySQL Connections."
+            )
         if metric._agg_type == M.AggType.AVERAGE_TIME_TO_CONV:
             t1 = first_cte.columns.get(GA.CTE_DATETIME_COL)
             t2 = cte.columns.get(GA.CTE_DATETIME_COL)
-            return SA.func.avg(SA.func.date_diff(t2, t1, SA.literal_column("second")))
+            diff = SA.func.unix_timestamp(t2) - SA.func.unix_timestamp(t1)
+            return SA.func.avg(diff)
         else:
             return super()._get_conv_aggregation(metric, cte, first_cte)
+
+    def get_conversion_df(self, metric: M.ConversionMetric) -> pd.DataFrame:
+        df = super().get_conversion_df(metric)
+        for index in range(1, len(metric._conversion._segments) + 1):
+            df[f"{GA.AGG_VALUE_COL}_{index}"] = df[
+                f"{GA.AGG_VALUE_COL}_{index}"
+            ].astype(float)
+        return df
+
+    def get_segmentation_df(self, metric: M.SegmentationMetric) -> pd.DataFrame:
+        df = super().get_segmentation_df(metric)
+        df[GA.AGG_VALUE_COL] = df[GA.AGG_VALUE_COL].astype(float)
+        return df
```

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/databricks_adapter.py` & `mitzu-0.6.1/mitzu/adapters/databricks_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/file_adapter.py` & `mitzu-0.6.1/mitzu/adapters/file_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/generic_adapter.py` & `mitzu-0.6.1/mitzu/adapters/generic_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/helper.py` & `mitzu-0.6.1/mitzu/adapters/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/mysql_adapter.py` & `mitzu-0.6.1/mitzu/adapters/postgresql_adapter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,51 @@
 from __future__ import annotations
 
 from typing import Any
 
 import mitzu.adapters.generic_adapter as GA
 import mitzu.model as M
 import pandas as pd
-from mitzu.adapters.sqlalchemy_adapter import FieldReference, SQLAlchemyAdapter
+from mitzu.adapters.sqlalchemy_adapter import (
+    FieldReference,
+    SQLAlchemyAdapter,
+)
 
 import sqlalchemy as SA
 import sqlalchemy.sql.expression as EXP
 
-NULL_VALUE_KEY = "##NULL##"
 
-
-class MySQLAdapter(SQLAlchemyAdapter):
+class PostgresqlAdapter(SQLAlchemyAdapter):
     def __init__(self, project: M.Project):
         super().__init__(project)
 
-    def _get_distinct_array_agg_func(self, field_ref: FieldReference) -> Any:
-        return SA.func.cast(
-            SA.func.json_keys(
-                SA.func.json_objectagg(SA.func.coalesce(field_ref, NULL_VALUE_KEY), "")
-            ),
-            SA.JSON,
-        )
-
     def _get_datetime_interval(
         self, field_ref: FieldReference, timewindow: M.TimeWindow
     ) -> Any:
-        return field_ref + SA.text(f"interval {timewindow.value} {timewindow.period}")
+        return field_ref + SA.text(f"interval '{timewindow.value} {timewindow.period}'")
 
     def _get_dynamic_datetime_interval(
         self,
         field_ref: FieldReference,
         value_field_ref: FieldReference,
         time_group: M.TimeGroup,
     ) -> Any:
-        return field_ref + SA.text(f"interval {value_field_ref} {time_group}")
-
-    def _get_date_trunc(self, time_group: M.TimeGroup, field_ref: FieldReference):
-        if time_group == M.TimeGroup.WEEK:
-            return SA.func.date_add(
-                SA.func.date(field_ref),
-                EXP.text(f"interval -{SA.func.weekday(field_ref)} day"),
-            )
-
-        elif time_group == M.TimeGroup.SECOND:
-            fmt = "%Y-%m-%dT%H:%i:%S"
-        elif time_group == M.TimeGroup.MINUTE:
-            fmt = "%Y-%m-%dT%H:%i:00"
-        elif time_group == M.TimeGroup.HOUR:
-            fmt = "%Y-%m-%dT%H:00:00"
-        elif time_group == M.TimeGroup.DAY:
-            fmt = "%Y-%m-%d"
-        elif time_group == M.TimeGroup.MONTH:
-            fmt = "%Y-%m-01"
-        elif time_group == M.TimeGroup.QUARTER:
-            raise NotImplementedError(
-                "Timegroup Quarter is not supported for MySQL Adapter"
-            )
-        elif time_group == M.TimeGroup.YEAR:
-            fmt = "%Y-01-01"
-
-        return SA.func.timestamp(SA.func.date_format(field_ref, fmt))
+        return field_ref + (value_field_ref * SA.text(f"interval '1 {time_group}'"))
 
     def _get_conv_aggregation(
         self, metric: M.Metric, cte: EXP.CTE, first_cte: EXP.CTE
     ) -> Any:
         if metric._agg_type == M.AggType.PERCENTILE_TIME_TO_CONV:
             raise NotImplementedError(
-                "Percentile calculation is not supported by MySQL Connections."
+                "Percentile calculation is not supported by PostgreSQL Connections."
             )
         if metric._agg_type == M.AggType.AVERAGE_TIME_TO_CONV:
             t1 = first_cte.columns.get(GA.CTE_DATETIME_COL)
             t2 = cte.columns.get(GA.CTE_DATETIME_COL)
-            diff = SA.func.unix_timestamp(t2) - SA.func.unix_timestamp(t1)
+            diff = SA.func.extract("EPOCH", t2) - SA.func.extract("EPOCH", t1)
             return SA.func.avg(diff)
         else:
             return super()._get_conv_aggregation(metric, cte, first_cte)
 
     def get_conversion_df(self, metric: M.ConversionMetric) -> pd.DataFrame:
         df = super().get_conversion_df(metric)
         for index in range(1, len(metric._conversion._segments) + 1):
@@ -87,7 +54,10 @@
             ].astype(float)
         return df
 
     def get_segmentation_df(self, metric: M.SegmentationMetric) -> pd.DataFrame:
         df = super().get_segmentation_df(metric)
         df[GA.AGG_VALUE_COL] = df[GA.AGG_VALUE_COL].astype(float)
         return df
+
+    def _get_distinct_array_agg_func(self, field_ref: FieldReference) -> Any:
+        return SA.func.to_json(SA.func.array_agg(SA.distinct(field_ref)))
```

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/redshift_adapter.py` & `mitzu-0.6.1/mitzu/adapters/redshift_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import pandas as pd
 import mitzu.adapters.sqlalchemy_adapter as SA
 from mitzu.adapters.postgresql_adapter import PostgresqlAdapter
 import mitzu.adapters.generic_adapter as GA
 from typing import List, Optional
 from sqlalchemy import distinct, select
 import sqlalchemy.sql.expression as EXP
+from sqlalchemy.orm import aliased
 
 VALUES_COL_NAME = "values"
 
 
 class RedshiftAdapter(PostgresqlAdapter):
     def __init__(self, project: M.Project):
         super().__init__(project)
@@ -47,15 +48,15 @@
         # We iterate through all columns in a loop. Also we use a window function to
         # pick only a sample of rows. We can't use group by at all for
         # discovering event field values.
 
         if event_data_table.discovery_settings is None:
             raise ValueError("Missing discovery settings")
 
-        cte = SA.aliased(
+        cte = aliased(
             self._get_dataset_discovery_cte(event_data_table),
             alias=SA.SAMPLED_SOURCE_CTE_NAME,
             name=SA.SAMPLED_SOURCE_CTE_NAME,
         )
         event_name_select_field = self.get_event_name_field(
             event_data_table, cte
         ).label(GA.EVENT_NAME_ALIAS_COL)
```

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/snowflake_adapter.py` & `mitzu-0.6.1/mitzu/adapters/snowflake_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/__init__.py` & `mitzu-0.6.1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,8 +7,12 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from sqlalchemy.dialects import registry
 
-registry.register("athena", "athena.sqlalchemy.dialect", "AthenaDialect")
+registry.register(
+    "athena",
+    "mitzu.adapters.sqlalchemy.athena.sqlalchemy.dialect",
+    "AthenaDialect",
+)
```

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py` & `mitzu-0.6.1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from sqlalchemy.dialects import registry
 
 registry.register(
-    "athena",
-    "mitzu.adapters.sqlalchemy.athena.sqlalchemy.dialect",
-    "AthenaDialect",
+    "databricks",
+    "mitzu.adapters.sqlalchemy.databricks.sqlalchemy.dialect",
+    "DatabricksDialect",
 )
```

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py` & `mitzu-0.6.1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py` & `mitzu-0.6.1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py` & `mitzu-0.6.1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py` & `mitzu-0.6.1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py` & `mitzu-0.6.1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py` & `mitzu-0.6.1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py` & `mitzu-0.6.1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py` & `mitzu-0.6.1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/sqlalchemy_adapter.py` & `mitzu-0.6.1/mitzu/adapters/sqlalchemy_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,18 +29,21 @@
 SAMPLED_SOURCE_CTE_NAME = "sampled_source"
 
 
 SIMPLE_TYPE_MAPPINGS = {
     SA_T.Numeric: M.DataType.NUMBER,
     SA_T.Integer: M.DataType.NUMBER,
     SA_T.Boolean: M.DataType.BOOL,
+    SA_T.NullType: M.DataType.STRING,
     SA_T.DateTime: M.DataType.DATETIME,
     SA_T.Date: M.DataType.DATETIME,
     SA_T.Time: M.DataType.DATETIME,
     SA_T.String: M.DataType.STRING,
+    SA_T.ARRAY: M.DataType.ARRAY,
+    SA_T.JSON: M.DataType.MAP,
 }
 
 
 def format_query(raw_query: Any):
     if type(raw_query) != str:
         raw_query = str(raw_query.compile(compile_kwargs={"literal_binds": True}))
 
@@ -118,14 +121,15 @@
         raise ValueError(f"{sa_type}[{type(sa_type)}]: is not supported.")
 
     def keep_alive_connection(self) -> bool:
         return False
 
     def execute_query(self, query: Any) -> pd.DataFrame:
         engine = self.get_engine()
+
         try:
             if H.LOGGER.isEnabledFor(logging.DEBUG):
                 H.LOGGER.debug(f"Query:\n{format_query(query)}")
             if self._connection is None:
                 self._connection = engine.connect()
             cursor_result = self._connection.execute(query)
             columns = cursor_result.keys()
@@ -202,27 +206,30 @@
             return SA.literal_column(f"{sa_table.name}.{field._get_name()}")
 
     def _get_struct_type(self) -> TypeEngine:
         raise NotImplementedError(
             "Generic SQL Alchemy Adapter doesn't support complex types (struct, row)"
         )
 
+    def _get_struct_sub_types(self, struct_val: Any) -> Any:
+        return struct_val.attr_types
+
     def _parse_struct_type(self, sa_type: Any, name: str, path: str) -> M.Field:
         real_struct_type = self._get_struct_type()
         if isinstance(sa_type, real_struct_type):
             row: TypeEngine = sa_type
             sub_fields: List[M.Field] = []
-            for n, st in row.attr_types:
+            for n, st in self._get_struct_sub_types(row):
                 next_path = f"{path}.{n}"
                 sf = self._parse_struct_type(
                     sa_type=st,
                     name=n,
                     path=next_path,
                 )
-                if sf._type == M.DataType and (
+                if sf._type == M.DataType.STRUCT and (
                     sf._sub_fields is None or len(sf._sub_fields) == 0
                 ):
                     continue
                 sub_fields.append(sf)
             return M.Field(
                 _name=name, _type=M.DataType.STRUCT, _sub_fields=tuple(sub_fields)
             )
@@ -313,21 +320,25 @@
                 )
                 if map_field._sub_fields is None or len(map_field._sub_fields) == 0:
                     continue
                 res.append(map_field)
             else:
                 field = M.Field(_name=field_name, _type=data_type)
                 res.append(field)
+
         return self._flatten_fields(res)
 
     def list_all_table_columns(self, schema: str, table_name: str) -> List[M.Field]:
         table = self.get_table_by_name(schema, table_name)
         field_types = table.columns
         res = []
         for field_name, field_type in field_types.items():
+            if "." in field_name:
+                # Columns with periods are not supported
+                continue
             data_type = self.map_type(field_type.type)
             if data_type == M.DataType.STRUCT:
                 complex_field = self._parse_struct_type(
                     sa_type=field_type.type,
                     name=field_name,
                     path=field_name,
                 )
@@ -389,14 +400,15 @@
         url_params_str = "" if con.url_params is None else con.url_params
         if url_params_str != "" and url_params_str[0] != "?":
             url_params_str = "?" + url_params_str
         catalog_str = "" if con.catalog is None else f"/{con.catalog}"
 
         protocol = con.connection_type.get_protocol().lower()
         res = f"{protocol}://{user_name}{password}{host_str}{port_str}{catalog_str}{schema_str}{url_params_str}"
+
         return res
 
     def _get_distinct_array_agg_func(self, field_ref: FieldReference) -> Any:
         return SA.func.cast(SA.func.array_agg(SA.distinct(field_ref)), SA.JSON)
 
     def _column_index_support(self):
         return True
@@ -420,18 +432,18 @@
         )
         date_partition_filter = self._get_date_partition_filter(
             event_data_table,
             table,
             self.project.get_default_discovery_start_dt(),
             self.project.get_default_end_dt(),
         )
-
+        cols = [c for c in table.columns.values()]
         raw_cte: EXP.CTE = SA.select(
             columns=[
-                *table.columns.values(),
+                *cols,
                 self._get_sample_function().label("__sample"),
                 SA.func.row_number()
                 .over(
                     partition_by=event_name_field, order_by=self._get_random_function()
                 )
                 .label("rn"),
             ],
@@ -497,14 +509,15 @@
                         self._get_distinct_array_agg_func(
                             self.get_field_reference(f, sa_table=cte)
                         ),
                     ),
                     else_=SA.literal(None),
                 ).label(f._get_name().replace(".", COLUMN_NAME_REPLACE_STR))
                 for f in fields
+                if not f._sub_fields
             ],
         )
         df = self.execute_query(query)
         df = df.rename(
             # This is required for complext types, as aliasing with `.`
             # doesn't work. The `.` comes from the get _get_name()
             # This issue might appear elsewhere as well
@@ -518,32 +531,34 @@
         self,
         event_data_table: M.EventDataTable,
         fields: List[M.Field],
     ) -> Dict[str, M.EventDef]:
         enums = self._get_column_values_df(event_data_table, fields).to_dict("index")
         res: Dict[str, M.EventDef] = {}
         for evt, values in enums.items():
-            field_defs: Dict[M.Field, M.EventFieldDef] = {}
+            field_defs: List[M.EventFieldDef] = []
             for f in fields:
                 field_values = values[f._get_name()]
                 if (
                     (field_values is None)
                     or (len(field_values) == 1 and field_values[0])
                     or (len(field_values) > 1)
                 ):
                     vals = (
                         [v for v in field_values if v is not None]
                         if field_values
                         else None
                     )
-                    field_defs[f] = M.EventFieldDef(
-                        _event_name=evt,
-                        _field=f,
-                        _event_data_table=event_data_table,
-                        _enums=vals,
+                    field_defs.append(
+                        M.EventFieldDef(
+                            _event_name=evt,
+                            _field=f,
+                            _event_data_table=event_data_table,
+                            _enums=vals,
+                        )
                     )
 
             res[evt] = M.EventDef(
                 _event_name=evt,
                 _fields=field_defs,
                 _event_data_table=event_data_table,
             )
@@ -671,15 +686,15 @@
             raise Exception("No DiscoveredProject was provided to SQLAlchemy Adapter.")
         events = dd.definitions.get(ed_table)
         if events is not None:
             event_def_reference = events.get(event_name)
             if event_def_reference is not None:
                 event_def = event_def_reference.get_value_if_exists()
                 for edt_evt_field in event_def._fields:
-                    if edt_evt_field == field:
+                    if edt_evt_field._field == field:
                         return True
         return False
 
     def _find_group_by_field_ref(
         self,
         group_field: M.EventFieldDef,
         sa_table: SA.Table,
```

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/sqlite_adapter.py` & `mitzu-0.6.1/mitzu/adapters/sqlite_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/adapters/trino_adapter.py` & `mitzu-0.6.1/mitzu/adapters/bigquery_adapter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,173 +1,185 @@
 from __future__ import annotations
 
-from datetime import datetime
-from typing import Any, List, Union, cast
+from typing import Any, List, Union
+from mitzu.adapters.sqlalchemy.bigquery import sqlalchemy  # noqa: F401
 
-import mitzu.adapters.generic_adapter as GA
 import mitzu.model as M
 import pandas as pd
-import trino.sqlalchemy.datatype as SA_T
-from mitzu.adapters.helper import (
-    dataframe_str_to_datetime,
-    pdf_string_json_array_to_array,
+from mitzu.adapters.sqlalchemy_adapter import (
+    SQLAlchemyAdapter,
+    FieldReference,
 )
-from mitzu.adapters.sqlalchemy_adapter import FieldReference, SQLAlchemyAdapter
-from mitzu.helper import LOGGER
-from sqlalchemy.sql.type_api import TypeEngine
+import mitzu.adapters.generic_adapter as GA
 import sqlalchemy as SA
+from mitzu.adapters.helper import pdf_string_json_array_to_array
+
 import sqlalchemy.sql.expression as EXP
+from mitzu.adapters.sqlalchemy.bigquery.sqlalchemy import STRUCT
+from sqlalchemy.sql.type_api import TypeEngine
+import sqlalchemy.sql.sqltypes as SA_T
+from mitzu.helper import LOGGER
+
+
+JSON_LIST_KEY_VALS = '''
+    CREATE TEMP FUNCTION
+    json_object_list(input JSON)
+    RETURNS ARRAY<String>
+    LANGUAGE js AS """
+    return Object.keys(input);
+    """;    
+
+    with prop_keys as ( 
+        SELECT ARRAY_CONCAT_AGG(json_object_list({field_name}) ) list
+        FROM {table}
+    )
+
+    SELECT distinct l FROM prop_keys, UNNEST(list) AS l LIMIT {limit}
+'''
 
 
-class TrinoAdapter(SQLAlchemyAdapter):
+class BigQueryAdapter(SQLAlchemyAdapter):
     def __init__(self, project: M.Project):
         super().__init__(project)
 
-    def get_conversion_df(self, metric: M.ConversionMetric) -> pd.DataFrame:
-        df = super().get_conversion_df(metric)
-        df = dataframe_str_to_datetime(df, GA.DATETIME_COL)
-        for index in range(1, len(metric._conversion._segments) + 1):
-            df[f"{GA.AGG_VALUE_COL}_{index}"] = df[
-                f"{GA.AGG_VALUE_COL}_{index}"
-            ].astype(float)
-        return df
-
-    def get_segmentation_df(self, metric: M.SegmentationMetric) -> pd.DataFrame:
-        df = super().get_segmentation_df(metric)
-        df = dataframe_str_to_datetime(df, GA.DATETIME_COL)
-        df[GA.AGG_VALUE_COL] = df[GA.AGG_VALUE_COL].astype(float)
-        return df
-
-    def get_retention_df(self, metric: M.RetentionMetric) -> pd.DataFrame:
-        df = super().get_retention_df(metric)
-        df = dataframe_str_to_datetime(df, GA.GROUP_COL)
-        df = dataframe_str_to_datetime(df, GA.DATETIME_COL)
-        df[GA.AGG_VALUE_COL] = df[GA.AGG_VALUE_COL].astype(float)
-        return df
+    def get_engine(self) -> Any:
+        con = self.project.connection
+        if self._engine is None:
+            if con.url is None:
+                url = self._get_connection_url(con)
+            else:
+                url = con.url
+            credentials = con.extra_configs.get("credentials")
+            if not credentials:
+                raise Exception(
+                    "Connection extra_configs must contain credentials json."
+                )
+            self._engine = SA.create_engine(url, credentials_info=credentials)
+        return self._engine
 
     def execute_query(self, query: Any) -> pd.DataFrame:
         if type(query) != str:
             query = str(query.compile(compile_kwargs={"literal_binds": True}))
+            query = query.replace(
+                "%", "%%"
+            )  # bugfix for pyathena, which has string formatting
         return super().execute_query(query=query)
 
     def get_field_reference(
         self,
         field: M.Field,
         event_data_table: M.EventDataTable = None,
         sa_table: Union[SA.Table, EXP.CTE] = None,
-    ) -> FieldReference:
+    ):
         if sa_table is None and event_data_table is not None:
             sa_table = self.get_table(event_data_table)
         if sa_table is None:
             raise ValueError("Either sa_table or event_data_table has to be provided")
 
-        if field._parent is not None and field._parent._type == M.DataType.MAP:
-            map_key = field._name
-            property = SA.literal_column(f"{sa_table.name}.{field._parent._get_name()}")
-            return SA.func.element_at(property, map_key)
-
-        return super().get_field_reference(field, event_data_table, sa_table)
-
-    def map_type(self, sa_type: Any) -> M.DataType:
-        if isinstance(sa_type, SA_T.ROW):
-            return M.DataType.STRUCT
-        if isinstance(sa_type, SA_T.MAP):
-            return M.DataType.MAP
-        return super().map_type(sa_type)
-
-    def _parse_map_type(
-        self,
-        sa_type: Any,
-        name: str,
-        event_data_table: M.EventDataTable,
-    ) -> M.Field:
-        if event_data_table.discovery_settings is None:
-            raise ValueError("Missing discovery settings")
-
-        LOGGER.debug(f"Discovering map: {name}")
-        map: SA_T.MAP = cast(SA_T.MAP, sa_type)
-        if map.value_type in (SA_T.ROW, SA_T.MAP):
-            raise Exception(
-                f"Compounded map types are not supported: map<{map.key_type}, {map.value_type}>"
+        if field._parent is None:
+            res = sa_table.columns.get(field._name)
+        elif field._parent._type == M.DataType.MAP:
+            res = SA.literal_column(
+                f"json_value({sa_table.name}.{field._parent._get_name()}['{field._name}'])"
             )
-        cte = self._get_dataset_discovery_cte(event_data_table)
-        F = SA.func
-        map_keys_func = F.array_distinct(
-            F.flatten(F.array_agg(F.distinct(F.map_keys(cte.columns[name]))))
-        )
+        else:
+            res = SA.literal_column(f"{sa_table.name}.{field._get_name()}")
 
-        max_cardinality = event_data_table.discovery_settings.max_map_key_cardinality
-        q = SA.select(
-            columns=[
-                SA.case(
-                    [(F.cardinality(map_keys_func) < max_cardinality, map_keys_func)],
-                    else_=None,
-                ).label("sub_fields")
-            ]
-        )
-        df = self.execute_query(q)
-        if df.shape[0] == 0:
-            return M.Field(_name=name, _type=M.DataType.MAP)
-        keys = df.iat[0, 0]
-        sf_type = self.map_type(map.value_type)
-        sub_fields: List[M.Field] = [M.Field(key, sf_type) for key in keys]
-        return M.Field(_name=name, _type=M.DataType.MAP, _sub_fields=tuple(sub_fields))
+        if field._type == M.DataType.DATETIME:
+            res = SA.func.datetime(res)
+        return res
 
-    def _generate_time_series_column(self, dt: datetime) -> Any:
-        return SA.literal_column(f"timestamp '{dt}'")
+    def _get_sample_function(self):
+        return SA.func.mod(SA.cast(self._get_random_function() * 1367, SA.Integer), 100)
 
-    def _get_struct_type(self) -> TypeEngine:
-        return SA_T.ROW
+    def _get_random_function(self):
+        return SA.func.rand()
 
     def _get_distinct_array_agg_func(self, field_ref: FieldReference) -> Any:
-        return SA.func.array_agg(SA.distinct(field_ref))
+        return SA.func.to_json(SA.func.array_agg(SA.distinct(field_ref)))
+
+    def _get_date_trunc(
+        self, time_group: M.TimeGroup, field_ref: FieldReference
+    ) -> Any:
+        return SA.func.date_trunc(field_ref, SA.literal_column(time_group.name))
 
     def _get_column_values_df(
         self,
         event_data_table: M.EventDataTable,
         fields: List[M.Field],
     ) -> pd.DataFrame:
         df = super()._get_column_values_df(
             event_data_table=event_data_table,
             fields=fields,
         )
         return pdf_string_json_array_to_array(df)
 
-    def _correct_timestamp(self, dt: datetime) -> Any:
-        return SA.text(f"timestamp '{dt}'")
-
-    def _get_datetime_interval(
-        self, field_ref: FieldReference, timewindow: M.TimeWindow
-    ) -> Any:
-        return SA.func.date_add(
-            timewindow.period.name.lower(),
-            timewindow.value,
-            field_ref,
-        )
-
     def _get_dynamic_datetime_interval(
         self,
         field_ref: FieldReference,
         value_field_ref: FieldReference,
         time_group: M.TimeGroup,
     ) -> Any:
-        return SA.func.date_add(time_group.name.lower(), value_field_ref, field_ref)
+        return SA.func.datetime_add(
+            field_ref,
+            SA.literal_column(f"interval {value_field_ref} {time_group.name.lower()}"),
+        )
 
     def _get_conv_aggregation(
         self, metric: M.Metric, cte: EXP.CTE, first_cte: EXP.CTE
     ) -> Any:
-        if metric._agg_type == M.AggType.PERCENTILE_TIME_TO_CONV:
-            if metric._agg_param is None or 0 < metric._agg_param > 100:
-                raise ValueError(
-                    "Conversion percentile parameter must be between 0 and 100"
-                )
-            t1 = first_cte.columns.get(GA.CTE_DATETIME_COL)
-            t2 = cte.columns.get(GA.CTE_DATETIME_COL)
-            return SA.func.approx_percentile(
-                SA.func.date_diff("second", t1, t2), metric._agg_param / 100.0
-            )
+
         if metric._agg_type == M.AggType.AVERAGE_TIME_TO_CONV:
             t1 = first_cte.columns.get(GA.CTE_DATETIME_COL)
             t2 = cte.columns.get(GA.CTE_DATETIME_COL)
-            return SA.func.avg(SA.func.date_diff("second", t1, t2))
+            return SA.func.avg(SA.func.date_diff(t2, t1, SA.literal_column("second")))
         else:
             return super()._get_conv_aggregation(metric, cte, first_cte)
+
+    def map_type(self, sa_type: Any) -> M.DataType:
+        if isinstance(sa_type, STRUCT):
+            return M.DataType.STRUCT
+        if isinstance(sa_type, SA_T.JSON):
+            return M.DataType.MAP
+        return super().map_type(sa_type)
+
+    def _get_struct_sub_types(self, struct_val: Any) -> Any:
+        return struct_val._STRUCT_fields
+
+    def _parse_map_type(
+        self,
+        sa_type: Any,
+        name: str,
+        event_data_table: M.EventDataTable,
+    ) -> M.Field:
+        if event_data_table.discovery_settings is None:
+            raise ValueError("Missing discovery settings")
+
+        LOGGER.debug(f"Discovering JSON (Map): {name}")
+
+        max_cardinality = event_data_table.discovery_settings.max_map_key_cardinality
+        try:
+            query = JSON_LIST_KEY_VALS.format(
+                table=event_data_table.get_full_name(),
+                field_name=name,
+                limit=max_cardinality + 1,
+            )
+
+            df = self.execute_query(SA.text(query))
+        except Exception as exc:
+            if (
+                "Cannot convert undefined or null to object at json_object_list(JSON)"
+                not in str(exc)
+            ):
+                raise exc
+            df = pd.DataFrame()
+
+        if df.shape[0] == 0 or df.shape[0] > max_cardinality:
+            return M.Field(_name=name, _type=M.DataType.MAP)
+
+        keys = df.to_dict(orient="list")["l"]
+        sub_fields: List[M.Field] = [M.Field(key, M.DataType.STRING) for key in keys]
+
+        return M.Field(_name=name, _type=M.DataType.MAP, _sub_fields=tuple(sub_fields))
+
+    def _get_struct_type(self) -> TypeEngine:
+        return STRUCT
```

### Comparing `mitzu-0.6.0rc9/mitzu/helper.py` & `mitzu-0.6.1/mitzu/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/model.py` & `mitzu-0.6.1/mitzu/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,17 +227,18 @@
 class DataType(Enum):
     STRING = auto()
     NUMBER = auto()
     BOOL = auto()
     DATETIME = auto()
     MAP = auto()
     STRUCT = auto()
+    ARRAY = auto()
 
     def is_complex(self) -> bool:
-        return self in (DataType.MAP, DataType.STRUCT)
+        return self in (DataType.MAP, DataType.STRUCT, DataType.ARRAY)
 
     def from_string(self, string_value: str) -> Any:
         if self == DataType.BOOL:
             return bool(string_value)
         if self == DataType.NUMBER:
             return float(string_value)
         if self == DataType.STRING:
@@ -1141,15 +1142,15 @@
         return self._event_data_table.project
 
 
 @dataclass(frozen=True)
 class EventDef(Identifiable):
 
     _event_name: str
-    _fields: Dict[Field, EventFieldDef]
+    _fields: List[EventFieldDef]
     _event_data_table: EventDataTable
     _description: Optional[str] = ""
     _id: str = field(default_factory=helper.create_unique_id)
 
     @property
     def _project(self) -> Project:
         return self._event_data_table.project
```

### Comparing `mitzu-0.6.0rc9/mitzu/notebook/model_loader.py` & `mitzu-0.6.1/mitzu/notebook/model_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,16 +179,16 @@
             res.insert(0, curr._name)
         return res
 
     def _create_event_instance(self, event: M.EventDef):
         fields = event._fields
 
         class_def: Dict[str, Any] = {}
-        for event_field, event_field_def in fields.items():
-
+        for event_field_def in fields:
+            event_field = event_field_def._field
             field_class = self._create_event_field_class(
                 event._event_name, event_field_def
             )
             class_instance = field_class(
                 _event_name=event._event_name,
                 _field=event_field,
                 _event_data_table=event_field_def._event_data_table,
```

### Comparing `mitzu-0.6.0rc9/mitzu/project_discovery.py` & `mitzu-0.6.1/mitzu/project_discovery.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Dict, List, Optional, Callable
+from typing import Callable, Dict, Optional
 
 import mitzu.model as M
 from mitzu.helper import LOGGER
 import traceback
 
 
 class ProjectDiscoveryError(Exception):
@@ -12,34 +12,14 @@
 
 
 class ProjectDiscovery:
     def __init__(self, project: M.Project, callback: Optional[Callable] = None):
         self.project = project
         self.callback = callback
 
-    def _get_field_values(
-        self,
-        ed_table: M.EventDataTable,
-        specific_fields: List[M.Field],
-    ) -> Dict[str, M.EventDef]:
-        return self.project.get_adapter().get_field_enums(
-            event_data_table=ed_table,
-            fields=specific_fields,
-        )
-
-    def _copy_gen_field_def_to_spec(
-        self, spec_event_name: str, gen_evt_field_def: M.EventFieldDef
-    ):
-        return M.EventFieldDef(
-            _event_name=spec_event_name,
-            _field=gen_evt_field_def._field,
-            _event_data_table=gen_evt_field_def._event_data_table,
-            _enums=gen_evt_field_def._enums,
-        )
-
     def _create_event_field_def_references(
         self,
         event_data_table: M.EventDataTable,
         specific: Dict[str, M.EventDef],
     ) -> Dict[str, M.Reference[M.EventDef]]:
         res: Dict[str, M.Reference[M.EventDef]] = {}
         for evt_name, spec_evt_def in specific.items():
@@ -53,33 +33,29 @@
         return res
 
     def discover_project(self, progress_bar: bool = False) -> M.DiscoveredProject:
         definitions: Dict[M.EventDataTable, Dict[str, M.Reference[M.EventDef]]] = {}
 
         self.project.validate()
         tables = self.project.event_data_tables
-
+        adapter = self.project.get_adapter()
         errors = {}
         for ed_table in tables:
             defs = {}
             try:
                 LOGGER.debug(f"Discovering {ed_table.get_full_name()}")
-                fields = self.project.get_adapter().list_fields(
-                    event_data_table=ed_table
-                )
-
-                specific_fields = [
+                fields = adapter.list_fields(event_data_table=ed_table)
+                fields = [
                     f for f in fields if f._get_name() not in ed_table.ignored_fields
                 ]
-                event_specific_field_values = self._get_field_values(
-                    ed_table, specific_fields
-                )
+
+                field_enums = adapter.get_field_enums(ed_table, fields)
                 defs = self._create_event_field_def_references(
                     ed_table,
-                    event_specific_field_values,
+                    field_enums,
                 )
                 definitions[ed_table] = defs
             except Exception as exc:
                 LOGGER.error(f"{ed_table.table_name} failed to discover: {str(exc)}")
                 errors[ed_table.table_name] = exc
 
             if self.callback is not None:
```

### Comparing `mitzu-0.6.0rc9/mitzu/project_serialization.py` & `mitzu-0.6.1/mitzu/project_serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/samples/__init__.py` & `mitzu-0.6.1/mitzu/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/samples/data_ingestion.py` & `mitzu-0.6.1/mitzu/samples/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/samples/sample_data_generator.py` & `mitzu-0.6.1/mitzu/samples/sample_data_generator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/serialization.py` & `mitzu-0.6.1/mitzu/serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,15 +247,15 @@
             _event_data_table=edt,
         )
     if type_hint == M.EventDef:
         event_name = value.get("en")
         edt = find_edt(project, event_name)
         return M.EventDef(
             _event_name=_from_dict(event_name, project, str, path + ".en"),
-            _fields={},
+            _fields=[],
             _event_data_table=edt,
         )
     if type_hint == EFD_OR_ED_TYPE:
         if "f" in value:
             return _from_dict(value, project, M.EventFieldDef, path)
         else:
             return _from_dict(value, project, M.EventDef, path)
@@ -267,18 +267,18 @@
         event_name = other_hint
         edt = find_edt(project, event_name)
         dd = project._discovered_project.get_value()
         if dd is None:
             raise Exception(f"Couldn't find {event_name} in any of the datasources.")
 
         event_def: M.EventDef = dd.definitions[edt][event_name].get_value_if_exists()
-        fields = event_def._fields.keys()
+        fields = event_def._fields
         for f in fields:
-            if f._get_name() == value:
-                return f
+            if f._field._get_name() == value:
+                return f._field
         raise Exception(f"Couldn't find {value} among {event_name} fields.")
     if type_hint == M.TimeGroup:
         return M.TimeGroup.parse(value)
     if type_hint == M.Resolution:
         return M.Resolution.parse(value)
     if type_hint == M.AggType:
         return M.AggType.parse_agg_str(value)
```

### Comparing `mitzu-0.6.0rc9/mitzu/visualization/charts.py` & `mitzu-0.6.1/mitzu/visualization/charts.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,22 @@
     if g_users.shape[0] > 0:
         g_users = g_users.sort_values(order_by_col, ascending=False)
     g_users = g_users.head(max)
     top_groups = list(g_users[GA.GROUP_COL].values)
     return pdf[pdf[GA.GROUP_COL].isin(top_groups)]
 
 
+def fix_na_cols_group_col(pdf: pd.DataFrame) -> pd.DataFrame:
+    pdf[GA.GROUP_COL] = pdf[GA.GROUP_COL].fillna("<n/a>")
+    pdf[GA.GROUP_COL] = pdf[GA.GROUP_COL].apply(
+        lambda val: val if val != "" else "<no value>"
+    )
+    return pdf
+
+
 def get_color_label(metric: M.Metric):
     if (
         isinstance(metric, M.SegmentationMetric)
         and metric._segment._group_by is not None
     ):
         return value_to_label(metric._segment._group_by._field._get_name())
     elif (
@@ -68,15 +76,17 @@
         else:
             raise ValueError(f"No default chart type defined for {type(metric)}")
 
 
 def get_preprocessed_conversion_dataframe(
     pdf: pd.DataFrame, metric: M.ConversionMetric, suffix: str
 ) -> pd.DataFrame:
-    pdf = TC.fix_conversion_na_cols(pdf, metric)
+    pdf = fix_na_cols_group_col(pdf)
+
+    pdf = TC.fix_conversion_steps_na_cols(pdf, metric)
     if metric._agg_type in [
         M.AggType.AVERAGE_TIME_TO_CONV,
         M.AggType.PERCENTILE_TIME_TO_CONV,
     ]:
         pdf = TC.fix_conv_times_pdf(pdf, metric)
 
     pdf = filter_top_groups(pdf, metric, order_by_col=f"{GA.USER_COUNT_COL}_1")
@@ -98,15 +108,15 @@
     )
     return pdf
 
 
 def get_preprocessed_segmentation_dataframe(
     pdf: pd.DataFrame, metric: M.SegmentationMetric
 ):
-    pdf[GA.GROUP_COL] = pdf[GA.GROUP_COL].fillna("n/a").astype(str).fillna("n/a")
+    pdf = fix_na_cols_group_col(pdf)
     pdf = filter_top_groups(pdf, metric, order_by_col=GA.AGG_VALUE_COL)
     pdf = pdf.rename(
         columns={
             GA.DATETIME_COL: C.X_AXIS_COL,
             GA.AGG_VALUE_COL: C.Y_AXIS_COL,
             GA.GROUP_COL: C.COLOR_COL,
         }
@@ -121,14 +131,15 @@
     return pdf
 
 
 def get_preprocessed_retention_dataframe(
     pdf: pd.DataFrame, metric: M.RetentionMetric
 ) -> pd.DataFrame:
     size = pdf.shape[0]
+    pdf = fix_na_cols_group_col(pdf)
     pdf = TR.fix_retention(pdf, metric)
     pdf = filter_top_groups(pdf, metric, order_by_col=GA.USER_COUNT_COL + "_1")
     pdf = TR.get_retention_mapping(pdf, metric)
     pdf = T.get_retention_tooltip(pdf, metric)
     pdf[C.TEXT_COL] = pdf[C.Y_AXIS_COL].apply(
         lambda val: f"{val:.1f}%" if val > 0 and size <= 200 else ""
     )
```

### Comparing `mitzu-0.6.0rc9/mitzu/visualization/common.py` & `mitzu-0.6.1/mitzu/visualization/common.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/visualization/labels.py` & `mitzu-0.6.1/mitzu/visualization/labels.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/visualization/plot.py` & `mitzu-0.6.1/mitzu/visualization/plot.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/visualization/titles.py` & `mitzu-0.6.1/mitzu/visualization/titles.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/visualization/tooltips.py` & `mitzu-0.6.1/mitzu/visualization/tooltips.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/visualization/transform_conv.py` & `mitzu-0.6.1/mitzu/visualization/transform_conv.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,18 +28,17 @@
         elif C.TTC_RANGE_2_SEC < max_ttc <= C.TTC_RANGE_3_SEC:
             pdf[key] = pdf[key].div(3600).round(1)
         else:
             pdf[key] = pdf[key].div(86400).round(1)
     return pdf
 
 
-def fix_conversion_na_cols(
+def fix_conversion_steps_na_cols(
     pdf: pd.DataFrame, metric: M.ConversionMetric
 ) -> pd.DataFrame:
-    pdf[GA.GROUP_COL] = pdf[GA.GROUP_COL].fillna("n/a")
     funnel_length = len(metric._conversion._segments)
     cols = [f"{GA.AGG_VALUE_COL}_{i}" for i in range(1, funnel_length + 1)]
     pdf[cols] = pdf[cols].fillna(0)
     return pdf
 
 
 def get_melted_conv_column(
```

### Comparing `mitzu-0.6.0rc9/mitzu/visualization/transform_retention.py` & `mitzu-0.6.1/mitzu/visualization/transform_retention.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import mitzu.adapters.generic_adapter as GA
 import pandas as pd
 import mitzu.visualization.common as C
 
 
 def fix_retention(pdf: pd.DataFrame, metric: M.RetentionMetric) -> pd.DataFrame:
     pdf[GA.AGG_VALUE_COL] = round(pdf[GA.AGG_VALUE_COL], 2)
-    pdf[GA.GROUP_COL] = pdf[GA.GROUP_COL].fillna("n/a")
     if metric._time_group not in [
         M.TimeGroup.HOUR,
         M.TimeGroup.MINUTE,
         M.TimeGroup.SECOND,
         M.TimeGroup.TOTAL,
     ]:
         pdf[GA.DATETIME_COL] = pdf[GA.DATETIME_COL].dt.date
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/.DS_Store` & `mitzu-0.6.1/mitzu/webapp/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/assets/explore_page.css` & `mitzu-0.6.1/mitzu/webapp/assets/explore_page.css`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/assets/favicon.ico` & `mitzu-0.6.1/mitzu/webapp/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/assets/logo.png` & `mitzu-0.6.1/mitzu/webapp/assets/logo.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/assets/mitzu-logo-light.svg` & `mitzu-0.6.1/mitzu/webapp/assets/mitzu-logo-light.svg`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/athena.png` & `mitzu-0.6.1/mitzu/webapp/assets/warehouse/athena.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/bigquery.png` & `mitzu-0.6.1/mitzu/webapp/assets/warehouse/bigquery.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/clickhouse.png` & `mitzu-0.6.1/mitzu/webapp/assets/warehouse/clickhouse.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/databricks.png` & `mitzu-0.6.1/mitzu/webapp/assets/warehouse/databricks.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/mysql.png` & `mitzu-0.6.1/mitzu/webapp/assets/warehouse/mysql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/pandas.png` & `mitzu-0.6.1/mitzu/webapp/assets/warehouse/pandas.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/postgresql.png` & `mitzu-0.6.1/mitzu/webapp/assets/warehouse/postgresql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/redshift.png` & `mitzu-0.6.1/mitzu/webapp/assets/warehouse/redshift.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/snowflake.png` & `mitzu-0.6.1/mitzu/webapp/assets/warehouse/snowflake.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/sqlite.png` & `mitzu-0.6.1/mitzu/webapp/assets/warehouse/sqlite.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/assets/warehouse/trino.png` & `mitzu-0.6.1/mitzu/webapp/assets/warehouse/trino.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/auth/authorizer.py` & `mitzu-0.6.1/mitzu/webapp/auth/authorizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import time
 import traceback
 from abc import ABC, abstractmethod
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 import flask
 import werkzeug
 import jwt
 import requests
 import base64
 from typing import Any, Dict, List, Optional
 from urllib import parse
@@ -73,57 +73,58 @@
             oauth_config.jwt_algorithms,
             oauth_config.client_id,
         )
 
 
 @dataclass(frozen=True)
 class AuthConfig:
-    user_service: U.UserService
-
     token_cookie_name: str = "auth-token"
     redirect_cookie_name: str = "redirect-to"
 
     session_timeout: int = 7 * 24 * 60 * 60
     token_refresh_threshold: int = 60
     token_signing_key: str = configs.AUTH_JWT_SECRET
 
     oauth: Optional[OAuthConfig] = None
     token_validator: Optional[TokenValidator] = None
 
 
 @dataclass(frozen=True)
-class OAuthAuthorizer:
+class Authorizer:
     _config: AuthConfig
 
-    _authorized_url_prefixes: List[str] = field(
-        default_factory=lambda: [
+    @property
+    def _authorized_url_prefixes(self) -> List[str]:
+        return [
             P.UNAUTHORIZED_URL,
             P.HEALTHCHECK_PATH,
             "/assets/",
             "/_dash-update-component",
             "/_dash-component-suites/",
             "/_dash-layout",
             "/_dash-dependencies",
         ]
-    )
-    _ignore_token_refresh_prefixes: List[str] = field(
-        default_factory=lambda: [
+
+    @property
+    def _ignore_token_refresh_prefixes(self) -> List[str]:
+        return [
             P.UNAUTHORIZED_URL,
             P.SIGN_OUT_URL,
             P.HEALTHCHECK_PATH,
             "/assets/",
             "/_dash-component-suites/",
         ]
-    )
 
-    @classmethod
-    def create(cls, config: AuthConfig) -> OAuthAuthorizer:
-        return OAuthAuthorizer(
-            _config=config,
-        )
+    def get_home_url(self):
+        if configs.HOME_URL:
+            return configs.HOME_URL
+        return flask.request.url_root
+
+    def get_auth_token(self):
+        return flask.request.cookies.get(self._config.token_cookie_name)
 
     def _get_unauthenticated_response(
         self, redirect_url: Optional[str] = None
     ) -> werkzeug.wrappers.response.Response:
         resp = self._redirect(P.UNAUTHORIZED_URL)
         self.clear_cookie(resp, self._config.token_cookie_name)
         if redirect_url:
@@ -167,15 +168,15 @@
             "utf-8",
         )
         secret_hash = base64.b64encode(message).decode()
         payload = {
             "grant_type": "authorization_code",
             "client_id": self._config.oauth.client_id,
             "code": auth_code,
-            "redirect_uri": f"{configs.HOME_URL}{P.OAUTH_CODE_URL}",
+            "redirect_uri": f"{self.get_home_url()}{P.OAUTH_CODE_URL}",
         }
         headers = {
             "Content-Type": "application/x-www-form-urlencoded",
             "Authorization": f"Basic {secret_hash}",
         }
 
         resp = requests.post(
@@ -203,19 +204,18 @@
 
     def _validate_token(self, token: str) -> Optional[Dict]:
         try:
             claims = jwt.decode(
                 token, self._config.token_signing_key, algorithms=[JWT_ALGORITHM]
             )
 
-            token_subject = claims["sub"]
-            user = self._config.user_service.get_user_by_id(token_subject)
-            if user is None:
-                raise Exception("User not found")
-            claims[JWT_CLAIM_ROLE] = user.role.value
+            user_id = claims["sub"]
+            expected_claims = self._get_token_claims_for_user_id(user_id)
+            # apply the recent user role changes in the current auth session
+            claims[JWT_CLAIM_ROLE] = expected_claims[JWT_CLAIM_ROLE]
             return claims
         except Exception as e:
             LOGGER.warning(f"Failed to validate token: {str(e)}")
             return None
 
     def _validate_foreign_token(self, token) -> Optional[str]:
         if not self._config.token_validator:
@@ -231,42 +231,63 @@
                 return None
 
             return user_email
         except Exception as e:
             LOGGER.warning(f"Failed to validate token: {str(e)}")
             return None
 
+    def _get_token_claims_for_email(self, user_email: str) -> Dict[str, Any]:
+        raise NotImplementedError()
+
+    def _get_token_claims_for_user_id(self, user_id: str) -> Dict[str, Any]:
+        raise NotImplementedError()
+
+    def _get_token_claims_for_email_and_password(
+        self, email: str, password: str
+    ) -> Dict[str, Any]:
+        raise NotImplementedError()
+
     def authorize_request(
         self, request: flask.Request
     ) -> Optional[werkzeug.wrappers.response.Response]:
-        if self._config.oauth and request.path == P.REDIRECT_TO_LOGIN_URL:
-            resp = self._redirect(self._config.oauth.sign_in_url)
-            return resp
+
+        if request.path == P.REDIRECT_TO_LOGIN_URL:
+            if self._config.oauth:
+                resp = self._redirect(self._config.oauth.sign_in_url)
+                return resp
+            else:
+                resp = self._redirect(P.REDIRECT_TO_LOGIN_URL)
+
+        if request.path == P.SIGN_OUT_URL:
+            if self._config.oauth and self._config.oauth.sign_out_url:
+                resp = self._redirect(self._config.oauth.sign_out_url)
+                self.clear_cookie(resp, self._config.token_cookie_name)
+                return resp
+            else:
+                return self._get_unauthenticated_response()
+
+        for prefix in self._authorized_url_prefixes:
+            if request.path.startswith(prefix):
+                return None
 
         if self._config.oauth and request.path == P.OAUTH_CODE_URL:
             code = self._get_oauth_code()
             if code is not None:
                 LOGGER.debug(f"Redirected with code={code}")
                 try:
                     id_token = self._get_identity_token(code)
                     redirect_url = flask.request.cookies.get(
-                        self._config.redirect_cookie_name, request.host_url
+                        self._config.redirect_cookie_name, self.get_home_url()
                     )
 
                     user_email = self._validate_foreign_token(id_token)
                     if not user_email:
                         raise Exception("Unauthorized (Invalid jwt token)")
 
-                    user = self._config.user_service.get_user_by_email(user_email)
-                    if user is None:
-                        raise Exception(
-                            f"User tried to login without having a local user: {user_email}"
-                        )
-
-                    token_claims = {"sub": user.id, JWT_CLAIM_ROLE: user.role.value}
+                    token_claims = self._get_token_claims_for_email(user_email)
                     token = self._generate_new_token_with_claims(token_claims)
 
                     resp = self._redirect(redirect_url)
                     self.set_cookie(resp, self._config.token_cookie_name, token)
                     self.clear_cookie(resp, self._config.redirect_cookie_name)
                     return resp
                 except Exception as exc:
@@ -274,40 +295,35 @@
                     LOGGER.warning(f"Failed to authenticate: {str(exc)}")
                     if self._config.oauth and self._config.oauth.sign_out_url:
                         resp = self._redirect(self._config.oauth.sign_out_url)
                         self.clear_cookie(resp, self._config.token_cookie_name)
                         return resp
                     return self._get_unauthenticated_response()
 
-        auth_token = flask.request.cookies.get(self._config.token_cookie_name)
-
-        if request.path == P.SIGN_OUT_URL:
-            if self._config.oauth and self._config.oauth.sign_out_url:
-                resp = self._redirect(self._config.oauth.sign_out_url)
-                self.clear_cookie(resp, self._config.token_cookie_name)
-                return resp
-            return self._get_unauthenticated_response()
+        auth_token = self.get_auth_token()
+        if auth_token:
+            return self._authorize_request_with_token(request, auth_token)
 
-        for prefix in self._authorized_url_prefixes:
-            if request.path.startswith(prefix):
-                return None
+        return self._get_unauthenticated_response(request.url)
 
-        if auth_token and self._validate_token(auth_token) is not None:
+    def _authorize_request_with_token(
+        self, request: flask.Request, auth_token: str
+    ) -> Optional[werkzeug.wrappers.response.Response]:
+        if self._validate_token(auth_token) is not None:
             return None
-
         return self._get_unauthenticated_response(request.url)
 
     def refresh_auth_token(
         self, request: flask.Request, resp: flask.Response
     ) -> werkzeug.wrappers.response.Response:
         for prefix in self._ignore_token_refresh_prefixes:
             if request.path.startswith(prefix):
                 return resp
 
-        auth_token = flask.request.cookies.get(self._config.token_cookie_name)
+        auth_token = self.get_auth_token()
         if auth_token is not None:
             token_claims = self._validate_token(auth_token)
             if token_claims is not None:
 
                 if (
                     token_claims["iat"]
                     >= int(time.time()) - self._config.token_refresh_threshold
@@ -336,31 +352,33 @@
 
     def login_local_user(
         self, email: str, password: str, response: Optional[flask.Response] = None
     ) -> Optional[str]:
         if self._config.oauth:
             raise ValueError("Password login is not enabled, need to use SSO")
 
-        user = self._config.user_service.get_user_by_email_and_password(email, password)
-        if user is None:
+        try:
+            token_claims = self._get_token_claims_for_email_and_password(
+                email, password
+            )
+        except Exception as e:
+            LOGGER.warning(e)
             return None
-
-        token_claims = {"sub": user.id, JWT_CLAIM_ROLE: user.role.value}
         token = self._generate_new_token_with_claims(token_claims)
 
         if response:
             self.set_cookie(response, self._config.token_cookie_name, token)
             self.clear_cookie(response, self._config.redirect_cookie_name)
 
         return flask.request.cookies.get(
-            self._config.redirect_cookie_name, configs.HOME_URL
+            self._config.redirect_cookie_name, self.get_home_url()
         )
 
     def get_current_user_id(self) -> Optional[str]:
-        auth_token = flask.request.cookies.get(self._config.token_cookie_name)
+        auth_token = self.get_auth_token()
         if auth_token is None:
             return None
         token_claims = self._validate_token(auth_token)
         if token_claims is None:
             return None
         return token_claims.get("sub")
 
@@ -373,7 +391,42 @@
     ):
         response.set_cookie(cookie_name, value, path="/", httponly=True, **params)
 
     def clear_cookie(
         self, response: werkzeug.wrappers.response.Response, cookie_name: str
     ):
         self.set_cookie(response, cookie_name, "", expires=0)
+
+
+@dataclass(frozen=True)
+class OAuthAuthorizer(Authorizer):
+    _user_service: U.UserService
+
+    @classmethod
+    def create(cls, config: AuthConfig, user_service: U.UserService) -> OAuthAuthorizer:
+        return OAuthAuthorizer(
+            _config=config,
+            _user_service=user_service,
+        )
+
+    def _get_token_claims_for_email(self, user_email: str) -> Dict[str, Any]:
+        user = self._user_service.get_user_by_email(user_email)
+        if user is None:
+            raise Exception(f"Local user not found with email: {user_email}")
+
+        return {"sub": user.id, JWT_CLAIM_ROLE: user.role.value}
+
+    def _get_token_claims_for_user_id(self, user_id: str) -> Dict[str, Any]:
+        user = self._user_service.get_user_by_id(user_id)
+        if user is None:
+            raise Exception(f"Local user not found with id: {user_id}")
+
+        return {"sub": user.id, JWT_CLAIM_ROLE: user.role.value}
+
+    def _get_token_claims_for_email_and_password(
+        self, email: str, password: str
+    ) -> Dict[str, Any]:
+        user = self._user_service.get_user_by_email_and_password(email, password)
+        if user is None:
+            raise Exception("Bad credentials")
+
+        return {"sub": user.id, JWT_CLAIM_ROLE: user.role.value}
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/auth/cognito.py` & `mitzu-0.6.1/mitzu/webapp/auth/cognito.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/auth/decorator.py` & `mitzu-0.6.1/mitzu/webapp/auth/decorator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 import flask
-from typing import cast
 import functools
 from dash.exceptions import PreventUpdate
 from dash.dcc import Location
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.pages.paths as P
 import mitzu.webapp.model as WM
 
 
 def restricted(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
-        dependencies: DEPS.Dependencies = cast(
-            DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-        )
-
+        dependencies = DEPS.Dependencies.get()
         if dependencies.authorizer.is_request_authorized(flask.request):
             return func(*args, **kwargs)
         else:
             raise PreventUpdate
 
     return wrapper
 
 
 def restricted_for_admin(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
-        dependencies: DEPS.Dependencies = cast(
-            DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-        )
+        dependencies = DEPS.Dependencies.get()
 
         user_role = dependencies.authorizer.get_current_user_role(flask.request)
         if user_role is None:
             raise PreventUpdate
 
         if user_role != WM.Role.ADMIN:
             raise PreventUpdate
@@ -41,17 +35,15 @@
 
     return wrapper
 
 
 def restricted_layout(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
-        dependencies: DEPS.Dependencies = cast(
-            DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-        )
+        dependencies = DEPS.Dependencies.get()
 
         if dependencies.authorizer.is_request_authorized(flask.request):
             return func(*args, **kwargs)
         else:
             return Location("url", href=P.UNAUTHORIZED_URL)
 
     return wrapper
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/auth/google.py` & `mitzu-0.6.1/mitzu/webapp/auth/google.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/cache.py` & `mitzu-0.6.1/mitzu/webapp/cache.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/caching_dataset_adapter.py` & `mitzu-0.6.1/mitzu/webapp/caching_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/configs.py` & `mitzu-0.6.1/mitzu/webapp/configs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from typing import Tuple, Optional
 
-HOME_URL = os.getenv("HOME_URL", "http://localhost:8082")
-
+HOME_URL = os.getenv("HOME_URL")
+ENVIRONMENT = os.getenv("ENVIRONMENT", "dev")
 # dash
 GRAPH_POLL_INTERVAL_MS = int(os.getenv("GRAPH_POLL_INTERVAL_MS", 300))
 DASH_TITLE = os.getenv("DASH_TITLE", "Mitzu")
 DASH_FAVICON_PATH = os.getenv("DASH_FAVICON_PATH", "assets/favicon.ico")
 DASH_LOGO_PATH = os.getenv("DASH_LOGO_PATH", "/assets/mitzu-logo-light.svg")
 
 
@@ -30,14 +30,17 @@
 
 SECRET_ENCRYPTION_KEY = os.getenv("SECRET_ENCRYPTION_KEY", None)
 STORAGE_CONNECTION_STRING = os.getenv(
     "STORAGE_CONNECTION_STRING",
     "sqlite:///storage.db?cache=shared&check_same_thread=False",
 )
 
+ENABLE_USAGE_TRACKING = os.getenv("ENABLE_USAGE_TRACKING", "true").lower() != "false"
+TRACKING_API_KEY = os.getenv("TRACKING_API_KEY", "")
+TRACKING_HOST = os.getenv("TRACKING_HOST")
 
 KALEIDO_CONFIGS = os.getenv("KALEIDO_CONFIGS", "--disable-gpu-*,--single-process")
 
 
 def get_kaleido_configs() -> Optional[Tuple[str, ...]]:
     if KALEIDO_CONFIGS:
         return tuple(KALEIDO_CONFIGS.split(","))
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/dependencies.py` & `mitzu-0.6.1/mitzu/webapp/dependencies.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
+import flask
 from dataclasses import dataclass
-from typing import Optional
+from typing import cast, Optional
 
 import mitzu.webapp.auth.authorizer as A
 import mitzu.webapp.cache as C
 import mitzu.webapp.configs as configs
 import mitzu.webapp.storage as S
 import mitzu.webapp.service.user_service as U
 import mitzu.webapp.service.navbar_service as NB
+import mitzu.webapp.service.tracking_service as TS
 import mitzu.webapp.service.events_service as E
 import mitzu.webapp.service.secret_service as SS
 import mitzu.webapp.service.notification_service as NS
 
 CONFIG_KEY = "dependencies"
 
 
@@ -24,14 +26,15 @@
     queue: C.MitzuCache
     cache: C.MitzuCache
     events_service: E.EventsService
     navbar_service: NB.NavbarService
     secret_service: SS.SecretService
     user_service: U.UserService
     notification_service: NS.NotificationService
+    tracking_service: TS.TrackingService
 
     @classmethod
     def from_configs(
         cls,
         notification_service: Optional[NS.NotificationService] = None,
     ) -> Dependencies:
         if notification_service is None:
@@ -69,27 +72,34 @@
             token_validator=(
                 A.JWTTokenValidator.create_from_oauth_config(oauth_config)
                 if oauth_config is not None
                 else None
             ),
             token_signing_key=configs.AUTH_JWT_SECRET,
             session_timeout=configs.AUTH_SESSION_TIMEOUT,
-            user_service=user_service,
         )
-        authorizer = A.OAuthAuthorizer.create(auth_config)
+        authorizer = A.OAuthAuthorizer.create(auth_config, user_service)
         queue = C.DiskMitzuCache("queue")
 
         # Adding cache layer over storage
         events_service = E.EventsService(storage)
         secret_service = SS.SecretService()
+        tracking_service = TS.AuthorizedTrackingService(authorizer)
 
         return Dependencies(
             authorizer=authorizer,
             cache=cache,
             storage=storage,
             queue=queue,
             user_service=user_service,
             navbar_service=NB.NavbarService(),
             events_service=events_service,
             secret_service=secret_service,
             notification_service=notification_service,
+            tracking_service=tracking_service,
         )
+
+    @classmethod
+    def get(
+        cls,
+    ) -> Dependencies:
+        return cast(Dependencies, flask.current_app.config.get(CONFIG_KEY))
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/helper.py` & `mitzu-0.6.1/mitzu/webapp/helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,16 @@
     path: str, discovered_project: M.DiscoveredProject
 ) -> M.EventFieldDef:
     path_parts = path.split(".")
     event_name = path_parts[0]
     event_def = discovered_project.get_event_def(event_name)
     field_name = ".".join(path_parts[1:])
 
-    for field, event_field_def in event_def._fields.items():
+    for event_field_def in event_def._fields:
+        field = event_field_def._field
         if field._get_name() == field_name:
             return event_field_def
     raise Exception(f"Invalid property path: {path}")
 
 
 def get_event_names(segment: Optional[M.Segment]) -> List[str]:
     if segment is None:
@@ -100,28 +101,30 @@
     input_lg: int = 3,
     input_sm: int = 12,
     label_lg: int = 3,
     label_sm: int = 12,
     justify: Optional[str] = None,
     read_only: bool = False,
     hidden: bool = False,
+    label: Optional[str] = None,
     **kwargs,
 ):
     if "size" not in kwargs and component_type not in [dbc.Checkbox, dcc.Dropdown]:
         kwargs["size"] = "sm"
     if (
         component_type in [dbc.Input, dbc.Textarea]
         and kwargs.get("placeholder") is None
     ):
-        kwargs["placeholder"] = value_to_label(property)
+        placeholder = label if label is not None else value_to_label(property)
+        kwargs["placeholder"] = placeholder
 
     if icon_cls is not None:
         label_children = [
             html.B(className=f"{icon_cls} me-1"),
-            value_to_label(property),
+            value_to_label(property) if label is None else label,
             "*" if kwargs.get("required") and not read_only else "",
         ]
     else:
         label_children = [value_to_label(property)]
     if read_only:
         component_type = dbc.Input
         kwargs["readonly"] = True
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/model.py` & `mitzu-0.6.1/mitzu/webapp/model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/offcanvas.py` & `mitzu-0.6.1/mitzu/webapp/offcanvas.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/connections_page.py` & `mitzu-0.6.1/mitzu/webapp/pages/connections_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import traceback
-from typing import List, cast
+from typing import List
 
 import dash.development.base_component as bc
 import dash_bootstrap_components as dbc
-import flask
 from dash import html, register_page
 
 import mitzu.helper as H
 import mitzu.model as M
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.navbar as NB
 import mitzu.webapp.pages.paths as P
@@ -15,17 +14,15 @@
 
 CONNECTIONS_CONTAINER = "connections_container"
 CONNECTION_TITLE = "connection_title"
 
 
 @restricted_layout
 def layout() -> bc.Component:
-    depenednecies: DEPS.Dependencies = cast(
-        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-    )
+    depenednecies = DEPS.Dependencies.get()
     connection_ids = depenednecies.storage.list_connections()
 
     connections: List[M.Connection] = []
     for con_id in connection_ids:
         con = depenednecies.storage.get_connection(con_id)
         connections.append(con)
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/dashboards/manage_dashboards_component.py` & `mitzu-0.6.1/mitzu/webapp/pages/dashboards/manage_dashboards_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from typing import Dict, List, cast
+from typing import Dict, List
 
 import dash.development.base_component as bc
 import dash_bootstrap_components as dbc
 import dash_draggable as dd
 from dash import ALL, Input, Output, callback, ctx, html, State, no_update, dcc
 import mitzu.webapp.model as WM
 import mitzu.webapp.dependencies as DEPS
-import flask
 import dash_mantine_components as dmc
 import mitzu.visualization.plot as PLT
 import mitzu.visualization.charts as CHRT
 from dash_iconify import DashIconify
 import mitzu.serialization as SE
 import mitzu.webapp.pages.paths as P
 from mitzu.webapp.auth.decorator import restricted
@@ -347,17 +346,15 @@
     Output(SAVED_METRICS_CONTAINER, "children"),
     Input(ADD_DASHBOARD_METRIC_BUTTON, "n_clicks"),
     Input(SAVED_METRICS_SEARCH, "value"),
     prevent_initial_call=True,
 )
 @restricted
 def manage_saved_metrics_off_canvas(button: int, search_value: str):
-    storage = cast(
-        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-    ).storage
+    storage = DEPS.Dependencies.get().storage
     sm_ids = storage.list_saved_metrics()
     saved_metrics = [storage.get_saved_metric(sm_id) for sm_id in sm_ids]
     if search_value:
         saved_metrics = [
             sm
             for sm in saved_metrics
             if (not search_value or (search_value.lower() in sm.name.lower()))
@@ -387,17 +384,15 @@
     delete_clicks: List[int],
     dashboard_name: int,
     dashboard_id: str,
 ):
     if ctx.triggered_id is None:
         return no_update, no_update, no_update
 
-    storage = cast(
-        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-    ).storage
+    storage = DEPS.Dependencies.get().storage
 
     if ctx.triggered_id.get("type") == DELETE_SAVED_METRICS_TYPE:
         delete_metric_id = ctx.triggered_id.get("index")
         if (
             delete_clicks is None
             or all([c is None for c in delete_clicks])
             or delete_clicks is None
@@ -460,17 +455,15 @@
     State(DASHBOARD_ID, "children"),
     prevent_initial_call=True,
 )
 @restricted
 def dashboard_name_changed(name: str, dashboard_id: str) -> str:
     if name is None:
         return no_update
-    storage = cast(
-        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-    ).storage
+    storage = DEPS.Dependencies.get().storage
 
     dashboard = storage.get_dashboard(dashboard_id)
     if dashboard is not None:
         d_name = name if name else "Unnamed dashboard"
         dashboard = dashboard.rename(d_name)
         dashboard = storage.set_dashboard(dashboard_id, dashboard)
     return name
@@ -483,17 +476,15 @@
     prevent_initial_call=True,
 )
 @restricted
 def manage_layout_change(layouts: Dict[str, Dict], dashboard_id: str) -> str:
     if dashboard_id is None:
         return no_update
 
-    storage = cast(
-        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-    ).storage
+    storage = DEPS.Dependencies.get().storage
 
     dashboard = storage.get_dashboard(dashboard_id)
     if dashboard is None:
         return no_update
 
     for lt in layouts["lg"]:
         prefix = len(DASHBOARD_ITEM_PREFIX) + 1
@@ -524,17 +515,15 @@
     background=True,
 )
 @restricted
 def refresh_dashboards(set_progress, refresh_button_click: int, dashboard_id: str):
     if dashboard_id is None or refresh_button_click is None:
         return no_update, 0
 
-    storage = cast(
-        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-    ).storage
+    storage = DEPS.Dependencies.get().storage
 
     dashboard = storage.get_dashboard(dashboard_id)
     figures = []
     total = len(dashboard.dashboard_metrics)
     for index, dm in enumerate(dashboard.dashboard_metrics):
         if dm.saved_metric is not None:
             metric = dm.saved_metric.metric
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/dashboards_page.py` & `mitzu-0.6.1/mitzu/webapp/pages/dashboards_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 from dash import html, register_page, callback, Input, Output, ctx, State, ALL, dcc
 
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.model as WM
 import mitzu.webapp.navbar as NB
 import mitzu.webapp.pages.paths as P
 from mitzu.webapp.auth.decorator import restricted, restricted_layout
-from typing import cast
-import flask
 from dash_iconify import DashIconify
 
 register_page(__name__, path_template=P.DASHBOARDS_PATH, title="Mitzu - Dashboards")
 
 
 CREATE_NEW_DASHBOARD_BTN = "create_new_dashboard"
 DASHBOARD_DELETE = "dashboard_delete"
@@ -31,17 +29,15 @@
 
 DASHBOARD_CONTAINER = "dashboard_container"
 DASHBOARDS_INFO = "dashboard_info"
 
 
 @restricted_layout
 def layout(**query_params) -> bc.Component:
-    storage = cast(
-        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-    ).storage
+    storage = DEPS.Dependencies.get().storage
     d_ids = storage.list_dashboards()
     dashboards = [storage.get_dashboard(d_id) for d_id in d_ids]
 
     return html.Div(
         [
             NB.create_mitzu_navbar("dashboard-navbar"),
             dbc.Container(
@@ -260,16 +256,14 @@
         )
     ],
     interval=200,
     prevent_initial_call=True,
 )
 @restricted
 def confirm_button_clicked(accept_button: int, dashboard_id: str) -> List:
-    storage = cast(
-        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-    ).storage
+    storage = DEPS.Dependencies.get().storage
     if ctx.triggered_id is not None:
         storage.clear_dashboard(dashboard_id)
 
     d_ids = storage.list_dashboards()
     dashboards = [storage.get_dashboard(d_id) for d_id in d_ids]
     return list_dashboards(dashboards)
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/edit_user.py` & `mitzu-0.6.1/mitzu/webapp/pages/edit_user.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import flask
-from typing import cast
 from dash import (
     Input,
     Output,
     State,
     callback,
     html,
     register_page,
@@ -44,15 +43,15 @@
 DELETE_RESPONSE_CONTAINER = "user_delete_response_container"
 CHANGE_PASSWORD_RESPONSE_CONTAINER = "user_change_password_response_container"
 CHANGE_ROLE_RESPONSE_CONTAINER = "user_change_role_response_container"
 
 
 @restricted_layout
 def layout(user_id: str, **query_params) -> bc.Component:
-    deps = cast(DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY))
+    deps = DEPS.Dependencies.get()
     user_service = deps.user_service
 
     is_sso = deps.authorizer._config.oauth is not None
 
     logged_in_user_id = deps.authorizer.get_current_user_id()
     if logged_in_user_id is None:
         raise ValueError("Cannot determine logged in user id")
@@ -280,27 +279,28 @@
         "role": State({"type": INDEX_TYPE, "index": PROP_ROLE}, "value"),
         "all_inputs": State({"type": INDEX_TYPE, "index": ALL}, "value"),
     },
     prevent_initial_call=True,
 )
 @restricted_for_admin
 def create_new_user(n_clicks: int, email="", role="", all_inputs=[]):
-    deps = cast(DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY))
+    deps = DEPS.Dependencies.get()
     user_service = deps.user_service
 
     if deps.authorizer._config.oauth:
         # SSO users don't have passwords
         password = None
         confirm_password = None
     else:
         password = all_inputs[2]
         confirm_password = all_inputs[3]
 
     try:
         user_service.new_user(email, password, confirm_password, role=WM.Role(role))
+        deps.tracking_service.register_new_user(email, role)
         return {
             SAVE_RESPONSE_CONTAINER: "User created!",
         }
     except Exception as e:
         return {
             SAVE_RESPONSE_CONTAINER: str(e),
         }
@@ -324,15 +324,15 @@
     },
     prevent_initial_call=True,
 )
 @restricted
 def update_password(
     n_clicks: int, password="", confirm_password="", pathname: str = ""
 ):
-    deps = cast(DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY))
+    deps = DEPS.Dependencies.get()
 
     user_service = deps.user_service
 
     try:
         logged_in_user_id = deps.authorizer.get_current_user_id()
         logged_in_user = user_service.get_user_by_id(logged_in_user_id)
 
@@ -364,15 +364,15 @@
         "role": State({"type": INDEX_TYPE, "index": PROP_ROLE}, "value"),
         "pathname": State(MITZU_LOCATION, "pathname"),
     },
     prevent_initial_call=True,
 )
 @restricted_for_admin
 def update_role(n_clicks: int, role="", pathname: str = ""):
-    deps = cast(DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY))
+    deps = DEPS.Dependencies.get()
 
     user_service = deps.user_service
 
     try:
         logged_in_user_id = deps.authorizer.get_current_user_id()
 
         user_id = P.get_path_value(P.USERS_HOME_PATH, pathname, P.USER_PATH_PART)
@@ -398,15 +398,15 @@
         "pathname": State(MITZU_LOCATION, "pathname"),
     },
     prevent_initial_call=True,
 )
 @restricted_for_admin
 def delete_user(n_clicks: int, pathname: str = ""):
     user_id = P.get_path_value(P.USERS_HOME_PATH, pathname, P.USER_PATH_PART)
-    deps = cast(DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY))
+    deps = DEPS.Dependencies.get()
     user_service = deps.user_service
 
     try:
         user_service.delete_user(user_id)
         return {
             DELETE_RESPONSE_CONTAINER: "User deleted",
         }
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/explore/complex_segment_handler.py` & `mitzu-0.6.1/mitzu/webapp/pages/explore/complex_segment_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,25 +25,25 @@
 
 def get_group_by_options(
     discovered_project: M.DiscoveredProject, event_names: List[str]
 ):
     options: List[Dict[str, str]] = []
     for event_name in event_names:
         for field in discovered_project.get_event_def(event_name)._fields:
-            field_value = field._get_name()
+            field_value = field._field._get_name()
             should_break = False
             final_field_value = f"{event_name}.{field_value}"
             for op in options:
                 if ".".join(op["value"].split(".")[1:]) == field_value:
                     should_break = True
                     break
             if not should_break:
                 options.append(
                     {
-                        "label": get_property_name_label(field._get_name()),
+                        "label": get_property_name_label(field._field._get_name()),
                         "value": final_field_value,
                     }
                 )
     options.sort(key=lambda v: ".".join(v["value"].split(".")[1:]))
     return options
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/explore/dates_selector_handler.py` & `mitzu-0.6.1/mitzu/webapp/pages/explore/dates_selector_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/explore/event_segment_handler.py` & `mitzu-0.6.1/mitzu/webapp/pages/explore/event_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/explore/explore_page.py` & `mitzu-0.6.1/mitzu/webapp/pages/explore/explore_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any, Dict, Optional, Tuple, cast
+from typing import Any, Dict, Optional, Tuple
 from urllib.parse import quote, urlparse, parse_qs
 
 import dash_bootstrap_components as dbc
 import dash.development.base_component as bc
 
 import mitzu.model as M
 import mitzu.webapp.model as WM
@@ -22,15 +22,14 @@
 import mitzu.webapp.pages.explore.toolbar_handler as TH
 import mitzu.webapp.navbar as NB
 import mitzu.visualization.charts as CHRT
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.storage as S
 from mitzu.webapp.helper import MITZU_LOCATION, find_event_field_def, CHILDREN
 import mitzu.webapp.pages.paths as P
-import flask
 import traceback
 from dash import ctx, html, callback, no_update, dcc
 from dash.dependencies import ALL, Input, Output, State
 from mitzu.webapp.auth.decorator import restricted
 
 
 from mitzu.webapp.helper import (
@@ -452,17 +451,15 @@
                 # page layout load and everything should be already rendered
                 return no_update_response
 
             url = urlparse(href)
             project_id = P.get_path_value(
                 P.PROJECTS_EXPLORE_PATH, url.path, P.PROJECT_ID_PATH_PART
             )
-            depenedencies: DEPS.Dependencies = cast(
-                DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-            )
+            depenedencies = DEPS.Dependencies.get()
             project = depenedencies.storage.get_project(project_id)
             if project is None:
                 return no_update_response
             all_inputs = get_final_all_inputs(all_inputs, ctx.inputs_list)
             all_inputs[METRIC_NAME_INPUT] = metric_name
             all_inputs[METRIC_ID_VALUE] = metric_id
             all_inputs[MITZU_LOCATION] = href
@@ -496,17 +493,18 @@
     save_new_nclicks: int,
     replace_nclicks: int,
     close_nclicks: int,
     metric_id: str,
     metric_name: str,
     href: str,
 ) -> Dict[str, Any]:
-    deps = cast(DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY))
+    deps = DEPS.Dependencies.get()
     storage = deps.storage
     mitzu_cache = deps.cache
+    tracking_service = deps.tracking_service
     if ctx.triggered_id == METRIC_SAVE_NAVBAR_BUTTON:
         original_name = None
         if metric_id is not None:
             try:
                 sm = storage.get_saved_metric(metric_id)
                 if sm is not None:
                     original_name = sm.name
@@ -578,15 +576,17 @@
         else:
             return {
                 METRIC_SAVE_DIALOG: True,
                 METRIC_NAME_INPUT: no_update,
                 METRIC_SAVE_DIALOG_INFO: "Couldn't save metric. Invalid state.",
             }
         hash_key = GH.create_metric_hash_key(metric)
-        result_df = GH.get_metric_result_df(hash_key, metric, mitzu_cache)
+        result_df = GH.get_metric_result_df(
+            hash_key, metric, mitzu_cache, tracking_service
+        )
         simple_chart = CHRT.get_simple_chart(metric, result_df)
 
         if ctx.triggered_id == METRIC_SAVE_DIALOG_SAVE_NEW_BUTTON:
             metric_id = H.create_unique_id()
 
         GH.store_rendered_saved_metric(
             metric_name=metric_name,
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/explore/graph_handler.py` & `mitzu-0.6.1/mitzu/webapp/pages/explore/graph_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from __future__ import annotations
 
 import traceback
-from typing import Any, Dict, Optional, cast
+from typing import Any, Dict, Optional
 import dash.development.base_component as bc
 import dash_bootstrap_components as dbc
 import mitzu.model as M
 import mitzu.webapp.pages.explore.toolbar_handler as TH
 import mitzu.webapp.pages.explore.explore_page as EXP
 import mitzu.webapp.configs as configs
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.storage as S
 import mitzu.webapp.cache as C
 import mitzu.visualization.common as CO
-import flask
 import mitzu.webapp.pages.paths as P
 import mitzu.webapp.model as WM
 import mitzu.serialization as SE
 from mitzu.webapp.helper import MITZU_LOCATION
 
 import pandas as pd
 from dash import Input, Output, State, ctx, dcc, html, callback, no_update, dash_table
 from mitzu.webapp.helper import get_final_all_inputs
 from mitzu.webapp.auth.decorator import restricted
 import mitzu.visualization.plot as PLT
 import mitzu.visualization.charts as CHRT
 import json
 import hashlib
 from urllib.parse import urlparse
+from datetime import datetime
+import mitzu.webapp.service.tracking_service as TS
 
 GRAPH = "graph"
 MESSAGE = "lead fw-normal text-center h-100 w-100"
 TABLE = "explore_results_table"
 SQL_AREA = "sql_area"
 
 
@@ -72,20 +73,30 @@
     # However we need to use the ID as well for caching, some project may contain the same events.
     metric_dict["prj"] = metric.get_project().get_id()
 
     return hashlib.md5(json.dumps(metric_dict).encode("ascii")).hexdigest()
 
 
 def get_metric_result_df(
-    hash_key: str, metric: M.Metric, mitzu_cache: C.MitzuCache
+    hash_key: str,
+    metric: M.Metric,
+    mitzu_cache: C.MitzuCache,
+    tracking_service: TS.TrackingService,
 ) -> pd.DataFrame:
+    start_time = datetime.now().timestamp()
     result_df = mitzu_cache.get(hash_key)
+    from_cache = True
     if result_df is None:
+        from_cache = False
         result_df = metric.get_df()
         mitzu_cache.put(hash_key, result_df, expire=configs.CACHE_EXPIRATION)
+    duration = datetime.now().timestamp() - start_time
+    tracking_service.track_explore_finished(
+        metric, duration_seconds=duration, from_cache=from_cache
+    )
     return result_df
 
 
 def create_graph(
     metric: Optional[M.Metric],
     simple_chart: CO.SimpleChart,
 ) -> Optional[dcc.Graph]:
@@ -105,20 +116,23 @@
     fig = PLT.plot_chart(simple_chart, metric)
     return dcc.Graph(
         id=GRAPH, className="w-100", figure=fig, config={"displayModeBar": False}
     )
 
 
 def create_table(
-    metric: Optional[M.Metric], hash_key: str, mitzu_cache: C.MitzuCache
+    metric: Optional[M.Metric],
+    hash_key: str,
+    mitzu_cache: C.MitzuCache,
+    tracking_service: TS.TrackingService,
 ) -> Optional[dbc.Table]:
     if metric is None:
         return None
 
-    result_df = get_metric_result_df(hash_key, metric, mitzu_cache)
+    result_df = get_metric_result_df(hash_key, metric, mitzu_cache, tracking_service)
     result_df = result_df.sort_values(by=[result_df.columns[0], result_df.columns[1]])
     result_df.columns = [col[1:].replace("_", " ").title() for col in result_df.columns]
     table = dash_table.DataTable(
         id=TABLE,
         columns=[
             {"name": i, "id": i, "deletable": False, "selectable": False}
             for i in result_df.columns
@@ -212,19 +226,18 @@
         metric_id: str,
     ) -> bc.Component:
         try:
             parse_result = urlparse(href)
             project_id = P.get_path_value(
                 P.PROJECTS_EXPLORE_PATH, parse_result.path, P.PROJECT_ID_PATH_PART
             )
-            deps = cast(
-                DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-            )
+            deps = DEPS.Dependencies.get()
             storage = deps.storage
             mitzu_cache = deps.cache
+            tracking_service = deps.tracking_service
 
             project = storage.get_project(project_id)
             if project is None:
                 return no_update
             all_inputs = get_final_all_inputs(all_inputs, ctx.inputs_list)
             all_inputs[EXP.METRIC_ID_VALUE] = metric_id
             all_inputs[EXP.METRIC_NAME_INPUT] = metric_name
@@ -264,21 +277,23 @@
                 and mitzu_cache.get(hash_key) is None
             ):
                 return html.Div(
                     "Click run to execute the query", id=GRAPH, className=MESSAGE
                 )
 
             if graph_content_type == TH.CHART_VAL:
-                result_df = get_metric_result_df(hash_key, metric, mitzu_cache)
+                result_df = get_metric_result_df(
+                    hash_key, metric, mitzu_cache, tracking_service
+                )
                 simple_chart = CHRT.get_simple_chart(metric, result_df)
 
             if graph_content_type == TH.CHART_VAL:
                 res = create_graph(metric, simple_chart)  # noqa
             if graph_content_type == TH.TABLE_VAL:
-                res = create_table(metric, hash_key, mitzu_cache)
+                res = create_table(metric, hash_key, mitzu_cache, tracking_service)
             elif graph_content_type == TH.SQL_VAL:
                 res = create_sql_area(metric)
 
             return res
         except Exception as exc:
             traceback.print_exc()
             return html.Div(
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/explore/metric_config_handler.py` & `mitzu-0.6.1/mitzu/webapp/pages/explore/metric_config_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/explore/metric_segments_handler.py` & `mitzu-0.6.1/mitzu/webapp/pages/explore/metric_segments_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/explore/metric_type_handler.py` & `mitzu-0.6.1/mitzu/webapp/pages/explore/metric_type_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/explore/simple_segment_handler.py` & `mitzu-0.6.1/mitzu/webapp/pages/explore/simple_segment_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,22 +49,22 @@
     event_name = simple_segment._left._event_name
     field_name: Optional[str] = None
     if type(simple_segment._left) == M.EventFieldDef:
         field_name = simple_segment._left._field._get_name()
 
     event = discovered_project.get_event_def(event_name)
     placeholder = "+ Where" if simple_segment_index == 0 else "+ And"
-    fields_names = list(event._fields.keys())
-    fields_names.sort(key=lambda f: f._get_name())
+    fields = [f._field for f in event._fields]
+    fields.sort(key=lambda f: f._get_name())
     options = [
         {
             "label": get_property_name_label(f._get_name()),
             "value": f"{event_name}.{f._get_name()}",
         }
-        for f in fields_names
+        for f in fields
     ]
 
     return dmc.Select(
         data=options,
         value=None if field_name is None else f"{event_name}.{field_name}",
         placeholder=placeholder,
         searchable=True,
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/explore/toolbar_handler.py` & `mitzu-0.6.1/mitzu/webapp/pages/explore/toolbar_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/explore_project.py` & `mitzu-0.6.1/mitzu/webapp/pages/explore_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from typing import cast
-
 import dash.development.base_component as bc
-import flask
 from dash import html, register_page
 
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.pages.explore.explore_page as EXP
 import mitzu.webapp.pages.paths as P
 from mitzu.webapp.auth.decorator import restricted_layout
 import traceback
@@ -17,17 +14,15 @@
     title="Mitzu - Explore",
 )
 
 
 @restricted_layout
 def layout(project_id: str, **query_params) -> bc.Component:
     try:
-        depenednecies: DEPS.Dependencies = cast(
-            DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-        )
+        depenednecies = DEPS.Dependencies.get()
         project = depenednecies.storage.get_project(project_id)
 
         if project is None:
             return html.Div("Project not found", className="d-flex text-center lead")
 
         discovered_project = project._discovered_project.get_value()
         if discovered_project is None:
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/home.py` & `mitzu-0.6.1/mitzu/webapp/pages/home.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/login.py` & `mitzu-0.6.1/mitzu/webapp/pages/login.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from typing import List, cast
-import flask
+from typing import List
 from dash import (
     register_page,
     dcc,
     callback,
     Input,
     Output,
     State,
@@ -24,17 +23,15 @@
 INPUT_PASSWORD = "password"
 BUTTON_LOGIN = "login"
 LOGIN_ERROR = "login_error"
 LOCATION = "login_location"
 
 
 def layout(**query_params):
-    depenednecies: DEPS.Dependencies = cast(
-        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-    )
+    depenednecies = DEPS.Dependencies.get()
     return dbc.Container(
         children=[
             dbc.Row(
                 [
                     html.Img(
                         src=configs.DASH_LOGO_PATH,
                         height="100px",
@@ -138,17 +135,15 @@
         Output(LOGIN_ERROR, "children"),
     ],
     Input(BUTTON_LOGIN, "n_clicks"),
     State({"type": INDEX_TYPE, "index": ALL}, "value"),
     prevent_initial_call=True,
 )
 def login(n_click: int, inputs: List[str]):
-    authorizer = cast(
-        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-    ).authorizer
+    authorizer = DEPS.Dependencies.get().authorizer
 
     redirect_when_authorized = authorizer.login_local_user(
         inputs[0], inputs[1], callback_context.response
     )
     if redirect_when_authorized:
         return (redirect_when_authorized, "")
     return (
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/manage_connection.py` & `mitzu-0.6.1/mitzu/webapp/pages/manage_connection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-from typing import Any, List, Optional, cast
+from typing import Any, List, Optional
 
 import dash.development.base_component as bc
 import dash_bootstrap_components as dbc
-import flask
 from dash import (
     ALL,
     Input,
     Output,
     State,
     callback,
     ctx,
     html,
     no_update,
     register_page,
     dcc,
 )
 
-import mitzu.helper as H
 import mitzu.model as M
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.navbar as NB
 import mitzu.webapp.pages.connections.manage_connections_component as MCC
 import mitzu.webapp.pages.paths as P
 from mitzu.webapp.auth.decorator import restricted, restricted_layout
 
@@ -36,17 +34,15 @@
     return layout(None)
 
 
 @restricted_layout
 def layout(connection_id: Optional[str] = None, **query_params) -> bc.Component:
     connection: Optional[M.Connection] = None
     if connection_id is not None:
-        depenednecies: DEPS.Dependencies = cast(
-            DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-        )
+        depenednecies = DEPS.Dependencies.get()
         connection = depenednecies.storage.get_connection(connection_id)
 
     title = "Create new connection" if connection is None else "Manage connection"
 
     return dbc.Form(
         [
             NB.create_mitzu_navbar("create-connection-navbar"),
@@ -129,22 +125,29 @@
         return no_update
 
     vals = {}
     for prop in ctx.args_grouping[2]:
         id_val = prop["id"]
         if id_val.get("type") == MCC.INDEX_TYPE:
             vals[id_val.get("index")] = prop["value"]
-
-    connection = MCC.create_connection_from_values(vals)
-    depenednecies: DEPS.Dependencies = cast(
-        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-    )
-
-    invalid = MCC.validate_input_values(values=vals)
-    if invalid is not None:
-        return html.P(f"Invalid {H.value_to_label(invalid)}", className="lead")
-    depenednecies.storage.set_connection(connection.id, connection)
-
-    if ctx.triggered_id == CONNECTION_SAVE_BUTTON:
-        return [html.P("Connection saved", className="lead"), no_update]
-    else:
-        return [no_update, f"{P.PROJECTS_CREATE_PATH}?connection_id={connection.id}"]
+    try:
+        connection = MCC.create_connection_from_values(vals)
+        depenednecies = DEPS.Dependencies.get()
+
+        depenednecies.storage.set_connection(connection.id, connection)
+        depenednecies.tracking_service.track_connection_saved(connection)
+
+        if ctx.triggered_id == CONNECTION_SAVE_BUTTON:
+            return [html.P("Connection saved", className="lead"), no_update]
+        else:
+            return [
+                no_update,
+                f"{P.PROJECTS_CREATE_PATH}?connection_id={connection.id}",
+            ]
+    except Exception as exc:
+        return [
+            html.P(
+                f"Saving failed: {str(exc)[:100]}",
+                className="lead text-danger",
+            ),
+            no_update,
+        ]
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/manage_dashboard.py` & `mitzu-0.6.1/mitzu/webapp/pages/manage_dashboard.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from typing import Optional, cast
+from typing import Optional
 
 import dash.development.base_component as bc
-import flask
 from dash import html, register_page
 
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.model as WM
 import mitzu.webapp.navbar as NB
 import mitzu.webapp.pages.dashboards.manage_dashboards_component as MDC
 import mitzu.webapp.pages.paths as P
@@ -15,17 +14,15 @@
 @restricted_layout
 def no_connection_layout():
     return layout(None)
 
 
 @restricted_layout
 def layout(dashboard_id: Optional[str] = None, **query_params) -> bc.Component:
-    depenednecies: DEPS.Dependencies = cast(
-        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-    )
+    depenednecies = DEPS.Dependencies.get()
     if dashboard_id is not None:
         dashboard = depenednecies.storage.get_dashboard(dashboard_id)
     else:
         dashboard = WM.Dashboard("New dashboard")
         depenednecies.storage.set_dashboard(dashboard.id, dashboard)
 
     return html.Div(
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/manage_event_defs.py` & `mitzu-0.6.1/mitzu/webapp/pages/manage_event_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 import dash.development.base_component as bc
 import mitzu.webapp.navbar as NB
 import mitzu.webapp.pages.paths as P
 from typing import Dict, List, Tuple, Optional
 from mitzu.webapp.auth.decorator import restricted, restricted_layout
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.helper as H
-import flask
 import mitzu.model as M
-from typing import cast, Callable
+from typing import Callable
 import traceback
 import dash_mantine_components as dmc
 
 SELECT_PROJECT_DD = "events_select_project"
 DISCOVER_INFO = "events_discovered_info"
 DISCOVER_PROJECT_BUTTON = "events_discover_button"
 DISCOVER_CANCEL_BUTTON = "cancel_discovery_button"
@@ -37,16 +36,16 @@
     )
 
 
 def create_table_row(
     edt: M.EventDataTable, event_def: M.Reference[M.EventDef]
 ) -> html.Tr:
     all_fields: List[str] = []
-    for field in event_def.get_value_if_exists()._fields.keys():
-        all_fields.extend(sf._get_name() for sf in field.get_all_subfields())
+    for field in event_def.get_value_if_exists()._fields:
+        all_fields.extend(sf._get_name() for sf in field._field.get_all_subfields())
     properties = f"{len(all_fields)} properties"
 
     return html.Tr(
         [
             html.Td(edt.get_full_name(), H.TBL_CLS),
             html.Td(event_def.get_value_if_exists()._event_name, className=H.TBL_CLS),
             html.Td(properties, className=H.TBL_CLS + " w-50"),
@@ -56,17 +55,15 @@
 
 def create_event_table_component(project: Optional[M.Project]) -> bc.Component:
     rows = []
     if project is not None:
         dp = project._discovered_project.get_value()
         if dp is None:
             dp = M.DiscoveredProject({}, project)
-        events_service = cast(
-            DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-        ).events_service
+        events_service = DEPS.Dependencies.get().events_service
         events_service.populate_discovered_project(dp)
 
         if dp is not None:
             for edt, df in dp.definitions.items():
                 for evt_df in df.values():
                     rows.append(create_table_row(edt, evt_df))
 
@@ -93,17 +90,15 @@
 
 def no_project_layout():
     return layout(None)
 
 
 @restricted_layout
 def layout(project_id: Optional[str], **query_params) -> bc.Component:
-    events_service = cast(
-        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-    ).events_service
+    events_service = DEPS.Dependencies.get().events_service
 
     projects = events_service.list_all_projects()
     selected_project: Optional[M.Project] = None
     for p in projects:
         if p.id == project_id:
             selected_project = p
             break
@@ -231,17 +226,17 @@
     cancel=Input(DISCOVER_CANCEL_BUTTON, "n_clicks"),
 )
 @restricted
 def handle_project_discovery(
     set_progress: Callable, discovery_clicks: int, project_id: str
 ):
     rows: List[bc.Component] = []
-    events_service = cast(
-        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-    ).events_service
+    deps = DEPS.Dependencies.get()
+    events_service = deps.events_service
+    tracking_service = deps.tracking_service
 
     try:
         if ctx.triggered_id == SELECT_PROJECT_DD:
             set_progress(([], ""))
             defs = events_service.get_project_definition(project_id)
             for edt, df in defs.items():
                 for evt_df in df.values():
@@ -263,16 +258,16 @@
                 set_progress(
                     (
                         rows,
                         f"Discovering tables {processed_count*100/total_count:.0f}%",
                     )
                 )
 
-            events_service.discover_project(project_id, callback=edt_callback)
-
+            dp = events_service.discover_project(project_id, callback=edt_callback)
+            tracking_service.track_project_discovered(dp)
         return (rows, "")
 
     except Exception as exc:
         traceback.print_exc()
         return ([], f"Something went wrong: {exc}")
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/manage_project.py` & `mitzu-0.6.1/mitzu/webapp/pages/manage_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import traceback
 from typing import Any, Dict, List, Optional, cast
 
 import dash.development.base_component as bc
 import dash_bootstrap_components as dbc
-import flask
 from dash import (
     ALL,
     Input,
     Output,
     State,
     callback,
     ctx,
@@ -134,17 +133,15 @@
 def layout_create(**query_params) -> bc.Component:
     return layout(None, **query_params)
 
 
 @restricted_layout
 def layout(project_id: Optional[str] = None, **query_params) -> bc.Component:
     project: Optional[M.Project] = None
-    dependencies: DEPS.Dependencies = cast(
-        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-    )
+    dependencies = DEPS.Dependencies.get()
     if project_id is not None:
         project = dependencies.storage.get_project(project_id)
 
     title = (
         "Create new project"
         if project is None
         else f"{H.value_to_label(project.project_name)}"
@@ -222,17 +219,15 @@
 )
 @restricted
 def delete_confirm_button_clicked(n_clicks: int, pathname: str) -> int:
     if n_clicks:
         project_id = P.get_path_value(
             P.PROJECTS_MANAGE_PATH, pathname, P.PROJECT_ID_PATH_PART
         )
-        depenednecies = cast(
-            DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-        )
+        depenednecies = DEPS.Dependencies.get()
         try:
             depenednecies.storage.delete_project(project_id)
         except Exception:
             # TBD: Toaster
             traceback.print_exc()
 
     return no_update
@@ -267,17 +262,18 @@
     save_clicks: int,
     save_and_discover_clicks: int,
     edt_table_rows: List,
     prop_values: List,
     pathname: str,
 ):
     try:
-        storage = cast(
-            DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-        ).storage
+
+        deps = DEPS.Dependencies.get()
+        storage = deps.storage
+        tracking_service = deps.tracking_service
 
         project_props: Dict[str, Any] = {}
 
         for prop in ctx.args_grouping[3]:
             id_val = prop["id"]
             if id_val.get("type") == MPH.PROJECT_INDEX_TYPE:
                 project_props[id_val.get("index")] = prop["value"]
@@ -333,15 +329,15 @@
                 min_property_sample_size=min_sample_size,
                 lookback_days=disc_lookback_days,
             ),
             event_data_tables=event_data_tables,
         )
 
         storage.set_project(project_id, project)
-
+        tracking_service.track_project_saved(project)
         if ctx.triggered_id == SAVE_BUTTON:
             return ["Project succesfully saved", no_update]
         else:
             return [
                 no_update,
                 P.create_path(
                     P.EVENTS_AND_PROPERTIES_PROJECT_PATH,
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/manage_saved_metrics.py` & `mitzu-0.6.1/mitzu/webapp/pages/manage_saved_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 import mitzu.webapp.navbar as NB
 import mitzu.webapp.pages.paths as P
 import mitzu.webapp.storage as S
 import mitzu.webapp.model as WM
 from typing import List
 import mitzu.webapp.dependencies as DEPS
 from mitzu.webapp.auth.decorator import restricted, restricted_layout
-import flask
-from typing import cast
 import datetime
 from mitzu.webapp.helper import MISSING_RESOURCE_CSS
 from urllib.parse import quote
 
 CREATE_PROJECT_DOCS_LINK = "https://github.com/mitzu-io/mitzu/blob/main/DOCS.md"
 SAVE_BUTTON = "project_save_button"
 CLOSE_BUTTON = "project_close_button"
@@ -199,17 +197,15 @@
         )
         for sm in saved_metrics
     ]
 
 
 @restricted_layout
 def layout(**query_params) -> bc.Component:
-    storage = cast(
-        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-    ).storage
+    storage = DEPS.Dependencies.get().storage
 
     return html.Div(
         [
             NB.create_mitzu_navbar("saved_metrics_navbar", storage=storage),
             dbc.Container(
                 [
                     html.H4("Saved metrics"),
@@ -266,14 +262,12 @@
     Output(SAVED_METRICS_CONTAINER, "children"),
     Input(CONFIRM_DIALOG_ACCEPT, "n_clicks"),
     State(CONFIRM_METRIC_ID, "children"),
     prevent_initial_call=True,
 )
 @restricted
 def confirm_button_clicked(close_button: int, metric_id: str) -> List:
-    storage = cast(
-        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-    ).storage
+    storage = DEPS.Dependencies.get().storage
     if ctx.triggered_id is not None:
         storage.clear_saved_metric(metric_id)
 
     return list_saved_metrics(storage)
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/paths.py` & `mitzu-0.6.1/mitzu/webapp/pages/paths.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/projects/event_tables_config.py` & `mitzu-0.6.1/mitzu/webapp/pages/projects/event_tables_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import dash_bootstrap_components as dbc
 from dash import ALL, Input, Output, State, callback, ctx, html, no_update
 import dash.development.base_component as bc
-from typing import Callable, Dict, List, Optional, Tuple, cast, Set
+from typing import Callable, Dict, List, Optional, Set, Tuple
 import mitzu.model as M
 from mitzu.webapp.pages.projects.helper import (
     PROP_CONNECTION,
     PROJECT_INDEX_TYPE,
     EDT_TBL_BODY,
     MISSING_FIELD,
     create_empty_edt,
     get_value_from_row,
 )
 from mitzu.webapp.auth.decorator import restricted
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.helper as H
-import flask
 import traceback
 import dash_mantine_components as dmc
 
 
 TBL_ID = "add_tables_id"
 TBL_SEARCH_INPUT = "table_search_box"
 TBL_PROGRESS_INFO = "table_progress_info"
@@ -587,17 +586,15 @@
 def manage_choose_schema_dropdown(
     add_tables: int, close: int, confirm: int, connection_id: Optional[str]
 ) -> Tuple:
     if ctx.triggered_id in [ADD_TABLES_MODAL_CLOSE, ADD_TABLES_MODAL_CONFIRM]:
         return ([], None, "Select schema")
     if connection_id is not None:
         try:
-            dependencies: DEPS.Dependencies = cast(
-                DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-            )
+            dependencies = DEPS.Dependencies.get()
             connection = dependencies.storage.get_connection(connection_id)
             dummy_project = M.Project(
                 connection=connection,
                 event_data_tables=[],
                 project_name="dummy_project",
             )
             adapter = dummy_project.get_adapter()
@@ -663,17 +660,15 @@
             return (options, [], "Choose tables to add")
         else:
             vals = [o.get("value") for o in options]
             return (options, vals, "Choose tables to add")
 
     if connection_id is not None:
         try:
-            dependencies: DEPS.Dependencies = cast(
-                DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-            )
+            dependencies = DEPS.Dependencies.get()
             connection = dependencies.storage.get_connection(connection_id)
             dummy_project = M.Project(
                 connection=connection,
                 event_data_tables=[],
                 project_name="dummy_project",
             )
             adapter = dummy_project.get_adapter()
@@ -721,17 +716,15 @@
             [None for _ in range(0, 5)],
             ["Loading..." for _ in range(0, 5)],
             "Loading table column",
         )
 
     if connection_id is not None:
         try:
-            dependencies: DEPS.Dependencies = cast(
-                DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-            )
+            dependencies = DEPS.Dependencies.get()
             connection = dependencies.storage.get_connection(connection_id)
             dummy_project = M.Project(
                 connection=connection,
                 event_data_tables=[],
                 project_name="dummy_project",
             )
             all_selected_count = 0
@@ -777,17 +770,15 @@
 
 def handle_configure_modal_confirm(
     set_progress,
     connection_id: str,
     tbl_body_children: List[bc.Component],
     edt_properties: List[bc.Component],
 ) -> List[bc.Component]:
-    dependencies: DEPS.Dependencies = cast(
-        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-    )
+    dependencies = DEPS.Dependencies.get()
     connection = dependencies.storage.get_connection(connection_id)
     dummy_project = M.Project(
         connection=connection,
         event_data_tables=[],
         project_name="dummy_project",
     )
     adapter = dummy_project.get_adapter()
@@ -806,15 +797,17 @@
             set_progress(f"Validating {count}/{sel_count} tables")
             full_table_name = get_value_from_row(tr, 1)
             schema, table_name = tuple(full_table_name.split("."))
             fields = adapter.list_all_table_columns(
                 table_name=table_name, schema=schema
             )
             field_names: Dict[str, M.Field] = {}
+
             for field in fields:
+
                 for f in field.get_all_subfields():
                     field_names[f._get_name()] = f
 
             user_id_fields = edt_properties[0]
             evnet_time_fields = edt_properties[1]
             event_name_fields = edt_properties[2]
             date_partition_fields = edt_properties[3]
@@ -845,17 +838,15 @@
 
 
 def handle_validate_button_clicked(
     set_progress,
     connection_id: str,
     tbl_body_children: List[bc.Component],
 ) -> List[bc.Component]:
-    dependencies: DEPS.Dependencies = cast(
-        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-    )
+    dependencies = DEPS.Dependencies.get()
     connection = dependencies.storage.get_connection(connection_id)
     dummy_project = M.Project(
         connection=connection,
         event_data_tables=[],
         project_name="dummy_project",
     )
     adapter = dummy_project.get_adapter()
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/projects/helper.py` & `mitzu-0.6.1/mitzu/webapp/pages/projects/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/projects/manage_project_component.py` & `mitzu-0.6.1/mitzu/webapp/pages/projects/manage_project_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/projects_page.py` & `mitzu-0.6.1/mitzu/webapp/pages/projects_page.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from dash import register_page
 import dash_bootstrap_components as dbc
 from dash import html
 import dash.development.base_component as bc
-import flask
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.navbar as NB
 from mitzu.webapp.auth.decorator import restricted_layout
 import mitzu.webapp.pages.paths as P
-from typing import List, cast
+from typing import List
 import traceback
 
 
 PROJECTS_CONTAINER = "projects_container"
 PROJECTS_ROW = "projects_row"
 PROJECT_CARD_TITLE = "project_card_title"
 
@@ -60,17 +59,15 @@
                 ]
             ),
         ]
     )
 
 
 def create_projects_children() -> List[bc.Component]:
-    depenednecies = cast(
-        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-    )
+    depenednecies = DEPS.Dependencies.get()
     project_ids = depenednecies.storage.list_projects()
 
     projects = []
     if len(project_ids) > 0:
         for p in project_ids:
             try:
                 projects.append(create_project_selector(p, depenednecies))
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/pages/users.py` & `mitzu-0.6.1/mitzu/webapp/pages/users.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import flask
-from typing import cast
 from dash import (
     html,
     register_page,
 )
 import dash_bootstrap_components as dbc
 import dash.development.base_component as bc
 import mitzu.webapp.dependencies as DEPS
@@ -66,15 +65,15 @@
         size="sm",
         id=USERS_TABLE_ID,
     )
 
 
 @restricted_layout
 def layout(**query_params) -> bc.Component:
-    deps = cast(DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY))
+    deps = DEPS.Dependencies.get()
     user_service = deps.user_service
 
     authorizer = deps.authorizer
 
     is_admin = authorizer.get_current_user_role(flask.request) == WM.Role.ADMIN
 
     table = create_users_table(user_service)
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/service/events_service.py` & `mitzu-0.6.1/mitzu/webapp/service/events_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                 Dict[str, M.Reference[M.EventDef]],
                 Optional[Exception],
                 int,
                 int,
             ],
             None,
         ],
-    ) -> Dict[M.EventDataTable, Dict[str, M.Reference[M.EventDef]]]:
+    ) -> M.DiscoveredProject:
         project = self.storage.get_project(project_id)
         edt_count = len(project.event_data_tables)
         edts = []
 
         def edt_callback(
             edt: M.EventDataTable,
             defs: Dict[str, M.Reference[M.EventDef]],
@@ -64,8 +64,8 @@
 
         discovered_project = project.discover_project(False, edt_callback)
         self.storage.set_project(
             project_id=discovered_project.project.id,
             project=discovered_project.project,
         )
 
-        return discovered_project.definitions
+        return discovered_project
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/service/navbar_service.py` & `mitzu-0.6.1/mitzu/webapp/service/navbar_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
 import dash.development.base_component as bc
 
 import dash_bootstrap_components as dbc
 from dash import html
-from typing import Optional, cast, Callable, List, Tuple
+from typing import Callable, List, Optional, Tuple
 import mitzu.webapp.pages.paths as P
-import flask
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.storage as S
 
 
 OFF_CANVAS_TOGGLER = "off-canvas-toggler"
 EXPLORE_DROPDOWN = "explore-dropdown"
 SIGNED_IN_AS_DIV = "signed-in-as"
@@ -43,17 +42,15 @@
             create_explore_button: bool = True,
             project_name: Optional[str] = None,
             storage: Optional[S.MitzuStorage] = None,
             **kwargs,
         ) -> Optional[bc.Component]:
             if create_explore_button:
                 if storage is None:
-                    storage = cast(
-                        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-                    ).storage
+                    storage = DEPS.Dependencies.get().storage
 
                 project_ids = storage.list_projects()
                 projects = [storage.get_project(p_id) for p_id in project_ids]
                 return dbc.DropdownMenu(
                     children=[
                         dbc.DropdownMenuItem(
                             children=p.project_name,
@@ -73,21 +70,17 @@
 
         self._left_navbar_providers = [
             (0, off_canvas_toggle),
             (10, explore_button),
         ]
 
         def signed_in_as(id: str, **kwargs) -> Optional[bc.Component]:
-            authorizer = cast(
-                DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-            ).authorizer
-
-            storage = cast(
-                DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-            ).storage
+            dependencies = DEPS.Dependencies.get()
+            authorizer = dependencies.authorizer
+            storage = dependencies.storage
 
             user_id = authorizer.get_current_user_id()
             if user_id is None:
                 return None
 
             email = None
             if storage:
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/service/notification_service.py` & `mitzu-0.6.1/mitzu/webapp/service/notification_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/service/secret_service.py` & `mitzu-0.6.1/mitzu/webapp/service/secret_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/service/user_service.py` & `mitzu-0.6.1/mitzu/webapp/service/user_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/storage.py` & `mitzu-0.6.1/mitzu/webapp/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,14 @@
                 self._set_event_data_table(project.id, edt, session)
 
             discovered_project = project._discovered_project.get_value()
             if discovered_project:
                 self._populate_discovered_project(discovered_project, session)
                 for edt, vals in discovered_project.definitions.items():
                     self._set_event_data_table_definition(edt, vals, session)
-
             session.commit()
 
     def project_exists(self, project_id: str) -> bool:
         with self._new_db_session() as session:
             return (
                 session.query(SM.ProjectStorageRecord)
                 .filter(SM.ProjectStorageRecord.project_id == project_id)
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/storage_model.py` & `mitzu-0.6.1/mitzu/webapp/storage_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,32 +10,29 @@
 import mitzu.webapp.model as WM
 import mitzu.visualization.common as VC
 import sqlalchemy as SA
 
 Base: SA.orm.DeclarativeMeta = SA.orm.declarative_base()
 
 
-def serialize_field(field: M.Field) -> str:
-    return json.dumps(
-        {
-            "_name": field._name,
-            "_type": field._type.value,
-            "_sub_fields": [serialize_field(f) for f in field._sub_fields]
-            if field._sub_fields
-            else None,
-        }
-    )
+def serialize_field(field: M.Field) -> Dict:
+    return {
+        "_name": field._name,
+        "_type": field._type.value,
+        "_parent": serialize_field(field._parent)
+        if field._parent is not None
+        else None,
+    }
 
 
-def deserialize_field(serialized: str) -> M.Field:
-    data = json.loads(serialized)
+def deserialize_field(data: Dict[str, Any]) -> M.Field:
     return M.Field(
         _name=data["_name"],
         _type=M.DataType(data["_type"]),
-        _sub_fields=data["_sub_fields"],
+        _parent=deserialize_field(data["_parent"]) if data["_parent"] else None,
     )
 
 
 class UserStorageRecord(Base):
     __tablename__ = "users"
 
     user_id = SA.Column(SA.String, primary_key=True)
@@ -464,22 +461,24 @@
     description = SA.Column(SA.String, nullable=True)
 
     def as_model_instance(
         self,
         edt: M.EventDataTable,
     ) -> M.EventDef:
         fields_dict = json.loads(self.fields)
-        fields: Dict[M.Field, M.EventFieldDef] = {}
+        fields: List[M.EventFieldDef] = []
         for field_def in fields_dict:
-            fields[deserialize_field(field_def["_key"])] = M.EventFieldDef(
-                _event_name=field_def["_event_name"],
-                _field=deserialize_field(field_def["_field"]),
-                _event_data_table=edt,
-                _description=field_def["_description"],
-                _enums=field_def["_enums"],
+            fields.append(
+                M.EventFieldDef(
+                    _event_name=field_def["_event_name"],
+                    _field=deserialize_field(field_def["_field"]),
+                    _event_data_table=edt,
+                    _description=field_def["_description"],
+                    _enums=field_def["_enums"],
+                )
             )
 
         return M.EventDef(
             _id=self.id,
             _event_name=self.event_name,
             _fields=fields,
             _event_data_table=edt,
@@ -487,30 +486,31 @@
         )
 
     @classmethod
     def from_model_instance(
         self, event_data_table_id: str, event_def: M.EventDef
     ) -> EventDefStorageRecord:
         fields = []
-        for field, field_def in event_def._fields.items():
+        for field_def in event_def._fields:
+            if field_def._field._sub_fields:
+                raise ValueError("Only leaf nodes can be serialized")
             fields.append(
                 {
-                    "_key": serialize_field(field),
                     "_event_name": field_def._event_name,
                     "_field": serialize_field(field_def._field),
                     "_event_data_table_id": field_def._event_data_table.id,
                     "_description": field_def._description,
                     "_enums": field_def._enums,
                 }
             )
         return EventDefStorageRecord(
             id=event_def.get_id(),
             event_data_table_id=event_data_table_id,
             event_name=event_def._event_name,
-            fields=json.dumps(fields),  # FIXME: double serialization
+            fields=json.dumps(fields),
             description=event_def._description,
         )
 
 
 class SavedMetricStorageRecord(Base):
     __tablename__ = "saved_metrics"
```

### Comparing `mitzu-0.6.0rc9/mitzu/webapp/webapp.py` & `mitzu-0.6.1/mitzu/webapp/webapp.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,26 +50,28 @@
     server = flask.Flask(__name__)
     if dependencies is None:
         dependencies = DEPS.Dependencies.from_configs()
 
     @server.before_request
     def before_request():
         request = flask.request
-        deps: DEPS.Dependencies = cast(
-            DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-        )
-        return deps.authorizer.authorize_request(request)
+        deps = DEPS.Dependencies.get()
+        res = deps.authorizer.authorize_request(request)
+        if res is not None:
+            deps.tracking_service.track_page_view(request, res)
+        return res
 
     @server.after_request
     def after_request(response: flask.Response):
         request = flask.request
-        deps: DEPS.Dependencies = cast(
-            DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-        )
-        return deps.authorizer.refresh_auth_token(request, response)
+        deps = DEPS.Dependencies.get()
+        res = deps.authorizer.refresh_auth_token(request, response)
+        if res is not None:
+            deps.tracking_service.track_page_view(request, res)
+        return res
 
     with server.app_context():
         dependencies.storage.init_db_schema()
         try:
             if configs.AUTH_ROOT_USER_EMAIL:
                 dependencies.user_service.new_user(
                     configs.AUTH_ROOT_USER_EMAIL,
@@ -117,17 +119,15 @@
         background_callback_manager=get_callback_manager(dependencies),
     )
     app._favicon = configs.DASH_FAVICON_PATH
     app.layout = create_webapp_layout()
 
     @server.route(P.HEALTHCHECK_PATH)
     def healthcheck():
-        dependencies: DEPS.Dependencies = cast(
-            DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-        )
+        dependencies = DEPS.Dependencies.get()
         try:
             # These will fail with exception if there is an underlying issue
             dependencies.queue.health_check()
             dependencies.cache.health_check()
             dependencies.storage.health_check()
         except Exception as exc:
             traceback.print_exc()
```

### Comparing `mitzu-0.6.0rc9/pyproject.toml` & `mitzu-0.6.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mitzu"
-version = "0.6.0-rc.9"
+version = "0.6.1"
 description = "Product analytics over your data warehouse"
 authors = ["Istvan Meszaros <istvan.meszaros.88@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mitzu.io"
 repository = "https://github.com/mitzu-io/mitzu"
 documentation = "https://mitzu.io/documentation/"
@@ -26,48 +26,54 @@
 psycopg2 = {version = "~2.9.3", optional=true}
 mysql-connector-python = {version = "~8.0.28", optional=true}
 trino = { version = "~0.313.0", optional=true, extras=["sqlalchemy"] }
 databricks-sql-connector = { version = "^2.0.2", optional=true}
 PyAthena = { version="^2.13.0", optional=true}
 snowflake-sqlalchemy = {version = "^1.4.3", optional=true}
 snowflake-connector-python = {version = "~=2.8.3", optional=true}
-sqlalchemy-bigquery = {version="^1.6.1", optional=true, extras=["bqstorage"]}
+google-cloud-bigquery = {version="^3.10.0", optional=true}
+google-cloud-core = {version="^2.3.2", optional=true}
+geoalchemy2 = {version= "^0.13.2", optional=true}
+shapely =  {version="^2.0.1", optional=true}
+google-cloud-bigquery-storage = {version="^2.19.1", optional=true}
 
 # Webapp Extras
 dash = {version="~2.8.1", optional=true, extras=["diskcache", "celery", "compress"]}
 dash-bootstrap-components = { version="^1.2.0", optional=true}
 dash-mantine-components =  { version= "^0.11.1", optional=true}
 orjson = {version="^3.7.11", optional=true}
 PyJWT = { version="^2.4.0", extras=["crypto"], optional=true}
 gunicorn = {version= "^20.1.0", optional=true}
 redis =  { version= "^4.4.0", optional=true}
 kaleido = {version = "==0.2.1", optional=true}
 dash-iconify = {version ="^0.1.2", optional=true}
 dash-draggable = {version="^0.1.2", optional=true}
+segment-analytics-python = {version="^2.2.2", optional=true}
 
 [tool.poetry.extras]
 postgres = ["psycopg2"]
 redshift= ["psycopg2"]
 mysql = ["mysql-connector-python"]
 trinodwh = ["trino"]
 databricks = ["databricks-sql-connector"]
 athena = ["PyAthena"]
 snowflake = ["snowflake-sqlalchemy","snowflake-connector-python"]
-bigquery= ["sqlalchemy-bigquery"]
+bigquery= ["google-cloud-bigquery", "google-cloud-core", "shapely", "geoalchemy2","google-cloud-bigquery-storage"]
 webapp = [
     "orjson", 
     "PyJWT", 
     "dash-bootstrap-components",
     "dash-mantine-components", 
     "dash", 
     "dash-iconify", 
     "gunicorn", 
     "redis", 
     "kaleido", 
     "dash-draggable", 
+    "segment-analytics-python",
     ]
 doc = ["sphinx", "sphinx-autodoc-typehints"]
 
 
 [tool.poetry.dev-dependencies]
 mypy = "^0.982"
 pytest = "^6.2.5"
@@ -90,15 +96,15 @@
 [tool.poetry.group.dev.dependencies]
 types-redis = "^4.3.21.6"
 vulture = "^2.6"
 black = {extras = ["jupyter"], version = "^22.12.0"}
 pylint = "^2.15.9"
 
 [tool.poetry-dynamic-versioning]
-enable = true
+enable = false
 vcs = "git"
 style = "semver"
 
 [tool.poetry-dynamic-versioning.substitution]
 folders = [{ path = "mitzu" }]
```

### Comparing `mitzu-0.6.0rc9/PKG-INFO` & `mitzu-0.6.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitzu
-Version: 0.6.0rc9
+Version: 0.6.1
 Summary: Product analytics over your data warehouse
 Home-page: https://mitzu.io
 License: MIT
 Author: Istvan Meszaros
 Author-email: istvan.meszaros.88@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -28,27 +28,32 @@
 Requires-Dist: dash-bootstrap-components (>=1.2.0,<2.0.0) ; extra == "webapp"
 Requires-Dist: dash-draggable (>=0.1.2,<0.2.0) ; extra == "webapp"
 Requires-Dist: dash-iconify (>=0.1.2,<0.2.0) ; extra == "webapp"
 Requires-Dist: dash-mantine-components (>=0.11.1,<0.12.0) ; extra == "webapp"
 Requires-Dist: dash[celery,compress,diskcache] (>=2.8.1,<2.9.0) ; extra == "webapp"
 Requires-Dist: databricks-sql-connector (>=2.0.2,<3.0.0) ; extra == "databricks"
 Requires-Dist: fastparquet (>=0.8.0,<0.9.0)
+Requires-Dist: geoalchemy2 (>=0.13.2,<0.14.0) ; extra == "bigquery"
+Requires-Dist: google-cloud-bigquery (>=3.10.0,<4.0.0) ; extra == "bigquery"
+Requires-Dist: google-cloud-bigquery-storage (>=2.19.1,<3.0.0) ; extra == "bigquery"
+Requires-Dist: google-cloud-core (>=2.3.2,<3.0.0) ; extra == "bigquery"
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0) ; extra == "webapp"
 Requires-Dist: kaleido (==0.2.1) ; extra == "webapp"
 Requires-Dist: mysql-connector-python (>=8.0.28,<8.1.0) ; extra == "mysql"
 Requires-Dist: orjson (>=3.7.11,<4.0.0) ; extra == "webapp"
 Requires-Dist: pandas (>=1.3.5,<1.4.0)
 Requires-Dist: plotly (>=5.5.0,<5.6.0)
 Requires-Dist: psycopg2 (>=2.9.3,<2.10.0) ; extra == "postgres" or extra == "redshift"
 Requires-Dist: pyarrow (>=8.0.0,<8.1.0)
 Requires-Dist: redis (>=4.4.0,<5.0.0) ; extra == "webapp"
 Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: segment-analytics-python (>=2.2.2,<3.0.0) ; extra == "webapp"
+Requires-Dist: shapely (>=2.0.1,<3.0.0) ; extra == "bigquery"
 Requires-Dist: snowflake-connector-python (>=2.8.3,<2.9.0) ; extra == "snowflake"
 Requires-Dist: snowflake-sqlalchemy (>=1.4.3,<2.0.0) ; extra == "snowflake"
-Requires-Dist: sqlalchemy-bigquery[bqstorage] (>=1.6.1,<2.0.0) ; extra == "bigquery"
 Requires-Dist: sqlalchemy[asyncio] (>=1.4.31,<1.5.0)
 Requires-Dist: sqlparse (>=0.4.2,<0.5.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: trino[sqlalchemy] (>=0.313.0,<0.314.0) ; extra == "trinodwh"
 Project-URL: Documentation, https://mitzu.io/documentation/
 Project-URL: Repository, https://github.com/mitzu-io/mitzu
 Description-Content-Type: text/markdown
```

