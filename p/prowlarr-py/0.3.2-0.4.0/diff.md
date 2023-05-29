# Comparing `tmp/prowlarr-py-0.3.2.tar.gz` & `tmp/prowlarr-py-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prowlarr-py-0.3.2.tar", last modified: Mon Mar 27 14:24:37 2023, max compression
+gzip compressed data, was "prowlarr-py-0.4.0.tar", last modified: Mon May 29 06:41:16 2023, max compression
```

## Comparing `prowlarr-py-0.3.2.tar` & `prowlarr-py-0.4.0.tar`

### file list

```diff
@@ -1,127 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:24:37.672810 prowlarr-py-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22640 2023-03-27 14:24:37.672810 prowlarr-py-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22160 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:24:37.660810 prowlarr-py-0.3.2/prowlarr/
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:24:37.664811 prowlarr-py-0.3.2/prowlarr/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/api_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30218 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/app_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53212 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/application_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/authentication_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22492 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/backup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23427 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/command_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30375 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/custom_filter_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/development_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53756 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/download_client_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/download_client_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/file_system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/health_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/history_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18592 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/host_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52459 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/indexer_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/indexer_default_categories_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/indexer_editor_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53420 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/indexer_proxy_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/indexer_stats_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12167 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/indexer_status_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/initialize_js_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/localization_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/log_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    42217 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/newznab_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53299 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/notification_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/ping_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/quality_profile_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26683 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21840 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/static_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26855 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29527 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/tag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/tag_details_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/task_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18422 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/ui_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/update_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api/update_log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29541 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:24:37.672810 prowlarr-py-0.3.2/prowlarr/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/api_info_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/app_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/application_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/application_sync_level.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/apply_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/authentication_required_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/authentication_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/backup_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/backup_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/book_search_param.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/certificate_validation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/command_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/command_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/command_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/command_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/custom_filter_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/database_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/development_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/download_client_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/download_client_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/download_client_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/download_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/field.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/health_check_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/health_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/history_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/history_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/history_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/host_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/host_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/indexer_capability_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/indexer_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/indexer_editor_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/indexer_privacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/indexer_proxy_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/indexer_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/indexer_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/indexer_stats_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/indexer_status_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/localization_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/log_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/log_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/log_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/movie_search_param.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/music_search_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/notification_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/paging_resource_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/ping_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/provider_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/provider_message_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/proxy_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/release_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/runtime_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/search_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/select_option.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/system_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/tag_details_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/tag_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/task_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/tv_search_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/ui_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/update_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/update_mechanism.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/update_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/models/user_agent_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/prowlarr/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:24:37.672810 prowlarr-py-0.3.2/prowlarr_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22640 2023-03-27 14:24:37.000000 prowlarr-py-0.3.2/prowlarr_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-03-27 14:24:37.000000 prowlarr-py-0.3.2/prowlarr_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 14:24:37.000000 prowlarr-py-0.3.2/prowlarr_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-27 14:24:37.000000 prowlarr-py-0.3.2/prowlarr_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-27 14:24:37.000000 prowlarr-py-0.3.2/prowlarr_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 14:24:37.672810 prowlarr-py-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-27 14:24:24.000000 prowlarr-py-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:16.270099 prowlarr-py-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22640 2023-05-29 06:41:16.270099 prowlarr-py-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22160 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:16.258098 prowlarr-py-0.4.0/prowlarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:16.262098 prowlarr-py-0.4.0/prowlarr/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/api_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30218 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/app_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53621 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/application_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/authentication_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22492 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/backup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23427 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/command_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30375 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/custom_filter_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/development_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54165 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/download_client_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/download_client_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/file_system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/health_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/history_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18592 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/host_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52868 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/indexer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/indexer_default_categories_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/indexer_editor_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53829 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/indexer_proxy_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/indexer_stats_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12167 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/indexer_status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/initialize_js_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/localization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/log_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42217 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/newznab_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53708 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/ping_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/quality_profile_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26683 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21840 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/static_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26855 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29527 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/tag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/tag_details_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/task_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18422 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/ui_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/update_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/update_log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29655 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18224 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:16.270099 prowlarr-py-0.4.0/prowlarr/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/api_info_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/app_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/application_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/application_sync_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/apply_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/authentication_required_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/authentication_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/backup_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/backup_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/book_search_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/certificate_validation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/command_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/command_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/command_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/command_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/custom_filter_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/database_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/development_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/download_client_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/download_client_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/download_client_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/download_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/health_check_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/health_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/history_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/history_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/history_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/host_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/host_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/indexer_capability_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/indexer_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/indexer_editor_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/indexer_privacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/indexer_proxy_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/indexer_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/indexer_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/indexer_stats_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/indexer_status_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/localization_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/log_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/log_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/log_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/movie_search_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/music_search_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/notification_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/paging_resource_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/ping_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/provider_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/provider_message_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/proxy_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/release_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/runtime_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/search_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/select_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/system_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/tag_details_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/tag_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/task_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/tv_search_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/ui_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/update_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/update_mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/update_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/user_agent_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:16.270099 prowlarr-py-0.4.0/prowlarr_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22640 2023-05-29 06:41:16.000000 prowlarr-py-0.4.0/prowlarr_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-29 06:41:16.000000 prowlarr-py-0.4.0/prowlarr_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 06:41:16.000000 prowlarr-py-0.4.0/prowlarr_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 06:41:16.000000 prowlarr-py-0.4.0/prowlarr_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 06:41:16.000000 prowlarr-py-0.4.0/prowlarr_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 06:41:16.270099 prowlarr-py-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/setup.py
```

### Comparing `prowlarr-py-0.3.2/LICENSE` & `prowlarr-py-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/PKG-INFO` & `prowlarr-py-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prowlarr-py
-Version: 0.3.2
+Version: 0.4.0
 Summary: Prowlarr API wrapper
 Project-URL: Homepage, https://github.com/devopsarr/prowlarr-py
 Project-URL: Bug Tracker, https://github.com/devopsarr/prowlarr-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 
 # prowlarr-py
 Prowlarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.3.2
+- Package version: 0.4.0
 
 [comment]: # (x-release-please-end)
 - API version: 1.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
```

### Comparing `prowlarr-py-0.3.2/README.md` & `prowlarr-py-0.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # prowlarr-py
 Prowlarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.3.2
+- Package version: 0.4.0
 
 [comment]: # (x-release-please-end)
 - API version: 1.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
```

### Comparing `prowlarr-py-0.3.2/prowlarr/__init__.py` & `prowlarr-py-0.4.0/prowlarr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # x-release-please-start-version
-__version__ = "0.3.2"
+__version__ = "0.4.0"
 # x-release-please-end
 
 # import apis into sdk package
 from prowlarr.api.api_info_api import ApiInfoApi
 from prowlarr.api.app_profile_api import AppProfileApi
 from prowlarr.api.application_api import ApplicationApi
 from prowlarr.api.authentication_api import AuthenticationApi
```

### Comparing `prowlarr-py-0.3.2/prowlarr/api/__init__.py` & `prowlarr-py-0.4.0/prowlarr/api/__init__.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/api_info_api.py` & `prowlarr-py-0.4.0/prowlarr/api/api_info_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/app_profile_api.py` & `prowlarr-py-0.4.0/prowlarr/api/app_profile_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/application_api.py` & `prowlarr-py-0.4.0/prowlarr/api/application_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
 from prowlarr.models.application_resource import ApplicationResource
 
 from prowlarr.api_client import ApiClient
 from prowlarr.exceptions import (  # noqa: F401
@@ -1150,25 +1150,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_applications(self, id : StrictStr, application_resource : Optional[ApplicationResource] = None, **kwargs) -> ApplicationResource:  # noqa: E501
+    def update_applications(self, id : StrictStr, force_save : Optional[StrictBool] = None, application_resource : Optional[ApplicationResource] = None, **kwargs) -> ApplicationResource:  # noqa: E501
         """update_applications  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_applications(id, application_resource, async_req=True)
+        >>> thread = api.update_applications(id, force_save, application_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param application_resource:
         :type application_resource: ApplicationResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1179,28 +1181,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: ApplicationResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_applications_with_http_info(id, application_resource, **kwargs)  # noqa: E501
+        return self.update_applications_with_http_info(id, force_save, application_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_applications_with_http_info(self, id : StrictStr, application_resource : Optional[ApplicationResource] = None, **kwargs):  # noqa: E501
+    def update_applications_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, application_resource : Optional[ApplicationResource] = None, **kwargs):  # noqa: E501
         """update_applications  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_applications_with_http_info(id, application_resource, async_req=True)
+        >>> thread = api.update_applications_with_http_info(id, force_save, application_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param application_resource:
         :type application_resource: ApplicationResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1223,14 +1227,15 @@
         :rtype: tuple(ApplicationResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'force_save',
             'application_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1256,14 +1261,16 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
```

### Comparing `prowlarr-py-0.3.2/prowlarr/api/authentication_api.py` & `prowlarr-py-0.4.0/prowlarr/api/authentication_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/backup_api.py` & `prowlarr-py-0.4.0/prowlarr/api/backup_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/command_api.py` & `prowlarr-py-0.4.0/prowlarr/api/command_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/custom_filter_api.py` & `prowlarr-py-0.4.0/prowlarr/api/custom_filter_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/development_config_api.py` & `prowlarr-py-0.4.0/prowlarr/api/development_config_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/download_client_api.py` & `prowlarr-py-0.4.0/prowlarr/api/download_client_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
 from prowlarr.models.download_client_resource import DownloadClientResource
 
 from prowlarr.api_client import ApiClient
 from prowlarr.exceptions import (  # noqa: F401
@@ -1150,25 +1150,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_download_client(self, id : StrictStr, download_client_resource : Optional[DownloadClientResource] = None, **kwargs) -> DownloadClientResource:  # noqa: E501
+    def update_download_client(self, id : StrictStr, force_save : Optional[StrictBool] = None, download_client_resource : Optional[DownloadClientResource] = None, **kwargs) -> DownloadClientResource:  # noqa: E501
         """update_download_client  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_download_client(id, download_client_resource, async_req=True)
+        >>> thread = api.update_download_client(id, force_save, download_client_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param download_client_resource:
         :type download_client_resource: DownloadClientResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1179,28 +1181,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: DownloadClientResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_download_client_with_http_info(id, download_client_resource, **kwargs)  # noqa: E501
+        return self.update_download_client_with_http_info(id, force_save, download_client_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_download_client_with_http_info(self, id : StrictStr, download_client_resource : Optional[DownloadClientResource] = None, **kwargs):  # noqa: E501
+    def update_download_client_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, download_client_resource : Optional[DownloadClientResource] = None, **kwargs):  # noqa: E501
         """update_download_client  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_download_client_with_http_info(id, download_client_resource, async_req=True)
+        >>> thread = api.update_download_client_with_http_info(id, force_save, download_client_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param download_client_resource:
         :type download_client_resource: DownloadClientResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1223,14 +1227,15 @@
         :rtype: tuple(DownloadClientResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'force_save',
             'download_client_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1256,14 +1261,16 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
```

### Comparing `prowlarr-py-0.3.2/prowlarr/api/download_client_config_api.py` & `prowlarr-py-0.4.0/prowlarr/api/download_client_config_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/file_system_api.py` & `prowlarr-py-0.4.0/prowlarr/api/file_system_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/health_api.py` & `prowlarr-py-0.4.0/prowlarr/api/health_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/history_api.py` & `prowlarr-py-0.4.0/prowlarr/api/history_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/host_config_api.py` & `prowlarr-py-0.4.0/prowlarr/api/host_config_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/indexer_api.py` & `prowlarr-py-0.4.0/prowlarr/api/indexer_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
 from prowlarr.models.indexer_resource import IndexerResource
 
 from prowlarr.api_client import ApiClient
 from prowlarr.exceptions import (  # noqa: F401
@@ -1150,25 +1150,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_indexer(self, id : StrictStr, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> IndexerResource:  # noqa: E501
+    def update_indexer(self, id : StrictStr, force_save : Optional[StrictBool] = None, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> IndexerResource:  # noqa: E501
         """update_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_indexer(id, indexer_resource, async_req=True)
+        >>> thread = api.update_indexer(id, force_save, indexer_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param indexer_resource:
         :type indexer_resource: IndexerResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1179,28 +1181,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: IndexerResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_indexer_with_http_info(id, indexer_resource, **kwargs)  # noqa: E501
+        return self.update_indexer_with_http_info(id, force_save, indexer_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_indexer_with_http_info(self, id : StrictStr, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
+    def update_indexer_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
         """update_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_indexer_with_http_info(id, indexer_resource, async_req=True)
+        >>> thread = api.update_indexer_with_http_info(id, force_save, indexer_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param indexer_resource:
         :type indexer_resource: IndexerResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1223,14 +1227,15 @@
         :rtype: tuple(IndexerResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'force_save',
             'indexer_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1256,14 +1261,16 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
```

### Comparing `prowlarr-py-0.3.2/prowlarr/api/indexer_default_categories_api.py` & `prowlarr-py-0.4.0/prowlarr/api/indexer_default_categories_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/indexer_editor_api.py` & `prowlarr-py-0.4.0/prowlarr/api/indexer_editor_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/indexer_proxy_api.py` & `prowlarr-py-0.4.0/prowlarr/api/indexer_proxy_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
 from prowlarr.models.indexer_proxy_resource import IndexerProxyResource
 
 from prowlarr.api_client import ApiClient
 from prowlarr.exceptions import (  # noqa: F401
@@ -1150,25 +1150,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_indexer_proxy(self, id : StrictStr, indexer_proxy_resource : Optional[IndexerProxyResource] = None, **kwargs) -> IndexerProxyResource:  # noqa: E501
+    def update_indexer_proxy(self, id : StrictStr, force_save : Optional[StrictBool] = None, indexer_proxy_resource : Optional[IndexerProxyResource] = None, **kwargs) -> IndexerProxyResource:  # noqa: E501
         """update_indexer_proxy  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_indexer_proxy(id, indexer_proxy_resource, async_req=True)
+        >>> thread = api.update_indexer_proxy(id, force_save, indexer_proxy_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param indexer_proxy_resource:
         :type indexer_proxy_resource: IndexerProxyResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1179,28 +1181,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: IndexerProxyResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_indexer_proxy_with_http_info(id, indexer_proxy_resource, **kwargs)  # noqa: E501
+        return self.update_indexer_proxy_with_http_info(id, force_save, indexer_proxy_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_indexer_proxy_with_http_info(self, id : StrictStr, indexer_proxy_resource : Optional[IndexerProxyResource] = None, **kwargs):  # noqa: E501
+    def update_indexer_proxy_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, indexer_proxy_resource : Optional[IndexerProxyResource] = None, **kwargs):  # noqa: E501
         """update_indexer_proxy  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_indexer_proxy_with_http_info(id, indexer_proxy_resource, async_req=True)
+        >>> thread = api.update_indexer_proxy_with_http_info(id, force_save, indexer_proxy_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param indexer_proxy_resource:
         :type indexer_proxy_resource: IndexerProxyResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1223,14 +1227,15 @@
         :rtype: tuple(IndexerProxyResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'force_save',
             'indexer_proxy_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1256,14 +1261,16 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
```

### Comparing `prowlarr-py-0.3.2/prowlarr/api/indexer_stats_api.py` & `prowlarr-py-0.4.0/prowlarr/api/indexer_stats_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/indexer_status_api.py` & `prowlarr-py-0.4.0/prowlarr/api/indexer_status_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/initialize_js_api.py` & `prowlarr-py-0.4.0/prowlarr/api/initialize_js_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/localization_api.py` & `prowlarr-py-0.4.0/prowlarr/api/localization_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/log_api.py` & `prowlarr-py-0.4.0/prowlarr/api/log_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/log_file_api.py` & `prowlarr-py-0.4.0/prowlarr/api/log_file_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/newznab_api.py` & `prowlarr-py-0.4.0/prowlarr/api/newznab_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/notification_api.py` & `prowlarr-py-0.4.0/prowlarr/api/notification_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
 from prowlarr.models.notification_resource import NotificationResource
 
 from prowlarr.api_client import ApiClient
 from prowlarr.exceptions import (  # noqa: F401
@@ -1150,25 +1150,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_notification(self, id : StrictStr, notification_resource : Optional[NotificationResource] = None, **kwargs) -> NotificationResource:  # noqa: E501
+    def update_notification(self, id : StrictStr, force_save : Optional[StrictBool] = None, notification_resource : Optional[NotificationResource] = None, **kwargs) -> NotificationResource:  # noqa: E501
         """update_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_notification(id, notification_resource, async_req=True)
+        >>> thread = api.update_notification(id, force_save, notification_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param notification_resource:
         :type notification_resource: NotificationResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1179,28 +1181,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: NotificationResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_notification_with_http_info(id, notification_resource, **kwargs)  # noqa: E501
+        return self.update_notification_with_http_info(id, force_save, notification_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_notification_with_http_info(self, id : StrictStr, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
+    def update_notification_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
         """update_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_notification_with_http_info(id, notification_resource, async_req=True)
+        >>> thread = api.update_notification_with_http_info(id, force_save, notification_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param notification_resource:
         :type notification_resource: NotificationResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1223,14 +1227,15 @@
         :rtype: tuple(NotificationResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'force_save',
             'notification_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1256,14 +1261,16 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
```

### Comparing `prowlarr-py-0.3.2/prowlarr/api/ping_api.py` & `prowlarr-py-0.4.0/prowlarr/api/ping_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/quality_profile_schema_api.py` & `prowlarr-py-0.4.0/prowlarr/api/quality_profile_schema_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/search_api.py` & `prowlarr-py-0.4.0/prowlarr/api/search_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/static_resource_api.py` & `prowlarr-py-0.4.0/prowlarr/api/static_resource_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/system_api.py` & `prowlarr-py-0.4.0/prowlarr/api/system_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/tag_api.py` & `prowlarr-py-0.4.0/prowlarr/api/tag_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/tag_details_api.py` & `prowlarr-py-0.4.0/prowlarr/api/tag_details_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/task_api.py` & `prowlarr-py-0.4.0/prowlarr/api/task_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/ui_config_api.py` & `prowlarr-py-0.4.0/prowlarr/api/ui_config_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/update_api.py` & `prowlarr-py-0.4.0/prowlarr/api/update_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api/update_log_file_api.py` & `prowlarr-py-0.4.0/prowlarr/api/update_log_file_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/api_client.py` & `prowlarr-py-0.4.0/prowlarr/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
         # x-release-please-start-version
-        self.user_agent = 'prowlarr-py/v0.3.2'
+        self.user_agent = 'prowlarr-py/v0.4.0'
         # x-release-please-end
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
@@ -187,14 +187,18 @@
 
         # auth setting
         self.update_params_for_auth(
             header_params, query_params, auth_settings,
             resource_path, method, body,
             request_auth=_request_auth)
 
+        # request timeout
+        if not _request_timeout:
+            _request_timeout = config.request_timeout
+
         # body
         if body:
             body = self.sanitize_for_serialization(body)
 
         # request url
         if _host is None:
             url = self.configuration.host + resource_path
```

### Comparing `prowlarr-py-0.3.2/prowlarr/configuration.py` & `prowlarr-py-0.4.0/prowlarr/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
       and data received from the server, independent of any validation performed by
       the server side. If the input data does not satisfy the JSON schema validation
       rules specified in the OpenAPI document, an exception is raised.
       If disabled_client_side_validations is set, structural validation is
       disabled. This can be useful to troubleshoot data validation problem, such as
       when the OpenAPI document validation rules do not match the actual API data
       received by the server.
+    :param request_timeout: Default request timeout.
     :param server_index: Index to servers configuration.
     :param server_variables: Mapping with string values to replace variables in
       templated server configuration. The validation of enums is performed for
       variables with defined enum values before.
     :param server_operation_index: Mapping from operation ID to an index to server
       configuration.
     :param server_operation_variables: Mapping from operation ID to a mapping with
@@ -105,14 +106,15 @@
     _default = None
 
     def __init__(self, host=None,
                  api_key=None, api_key_prefix=None,
                  username=None, password=None,
                  discard_unknown_keys=False,
                  disabled_client_side_validations="",
+                 request_timeout=None,
                  server_index=None, server_variables=None,
                  server_operation_index=None, server_operation_variables=None,
                  ssl_ca_cert=None,
                  ):
         """Constructor
         """
         self._base_path = "http://localhost:9696" if host is None else host
@@ -147,14 +149,17 @@
         """Username for HTTP basic authentication
         """
         self.password = password
         """Password for HTTP basic authentication
         """
         self.discard_unknown_keys = discard_unknown_keys
         self.disabled_client_side_validations = disabled_client_side_validations
+        self.request_timeout = request_timeout
+        """Request Timeout
+        """
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("prowlarr")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
@@ -421,15 +426,15 @@
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         # x-release-please-start-version
-        sdkversion = '0.3.2'
+        sdkversion = '0.4.0'
         # x-release-please-end
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
                "SDK Package Version: {sdkversion}".\
                format(env=sys.platform, pyversion=sys.version, sdkversion=sdkversion)
```

### Comparing `prowlarr-py-0.3.2/prowlarr/exceptions.py` & `prowlarr-py-0.4.0/prowlarr/exceptions.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/__init__.py` & `prowlarr-py-0.4.0/prowlarr/models/__init__.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/api_info_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/api_info_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/app_profile_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/app_profile_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/application_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/application_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/application_sync_level.py` & `prowlarr-py-0.4.0/prowlarr/models/application_sync_level.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/apply_tags.py` & `prowlarr-py-0.4.0/prowlarr/models/apply_tags.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/authentication_required_type.py` & `prowlarr-py-0.4.0/prowlarr/models/authentication_required_type.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/authentication_type.py` & `prowlarr-py-0.4.0/prowlarr/models/authentication_type.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/backup_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/backup_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/backup_type.py` & `prowlarr-py-0.4.0/prowlarr/models/backup_type.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/book_search_param.py` & `prowlarr-py-0.4.0/prowlarr/models/book_search_param.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/certificate_validation_type.py` & `prowlarr-py-0.4.0/prowlarr/models/certificate_validation_type.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/command.py` & `prowlarr-py-0.4.0/prowlarr/models/command.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/command_priority.py` & `prowlarr-py-0.4.0/prowlarr/models/command_priority.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/command_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/command_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/command_status.py` & `prowlarr-py-0.4.0/prowlarr/models/command_status.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/command_trigger.py` & `prowlarr-py-0.4.0/prowlarr/models/command_trigger.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/custom_filter_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/custom_filter_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/database_type.py` & `prowlarr-py-0.4.0/prowlarr/models/database_type.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/development_config_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/development_config_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/download_client_category.py` & `prowlarr-py-0.4.0/prowlarr/models/download_client_category.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/download_client_config_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/download_client_config_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/download_client_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/download_client_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/download_protocol.py` & `prowlarr-py-0.4.0/prowlarr/models/download_protocol.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/field.py` & `prowlarr-py-0.4.0/prowlarr/models/field.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/health_check_result.py` & `prowlarr-py-0.4.0/prowlarr/models/health_check_result.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/health_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/health_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/history_event_type.py` & `prowlarr-py-0.4.0/prowlarr/models/history_event_type.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/history_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/history_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/history_resource_paging_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/history_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/host_config_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/host_config_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     console_log_level: Optional[str]
     branch: Optional[str]
     api_key: Optional[str]
     ssl_cert_path: Optional[str]
     ssl_cert_password: Optional[str]
     url_base: Optional[str]
     instance_name: Optional[str]
+    application_url: Optional[str]
     update_automatically: Optional[bool]
     update_mechanism: Optional[UpdateMechanism]
     update_script_path: Optional[str]
     proxy_enabled: Optional[bool]
     proxy_type: Optional[ProxyType]
     proxy_hostname: Optional[str]
     proxy_port: Optional[int]
@@ -62,15 +63,15 @@
     proxy_bypass_filter: Optional[str]
     proxy_bypass_local_addresses: Optional[bool]
     certificate_validation: Optional[CertificateValidationType]
     backup_folder: Optional[str]
     backup_interval: Optional[int]
     backup_retention: Optional[int]
     history_cleanup_days: Optional[int]
-    __properties = ["id", "bindAddress", "port", "sslPort", "enableSsl", "launchBrowser", "authenticationMethod", "authenticationRequired", "analyticsEnabled", "username", "password", "logLevel", "consoleLogLevel", "branch", "apiKey", "sslCertPath", "sslCertPassword", "urlBase", "instanceName", "updateAutomatically", "updateMechanism", "updateScriptPath", "proxyEnabled", "proxyType", "proxyHostname", "proxyPort", "proxyUsername", "proxyPassword", "proxyBypassFilter", "proxyBypassLocalAddresses", "certificateValidation", "backupFolder", "backupInterval", "backupRetention", "historyCleanupDays"]
+    __properties = ["id", "bindAddress", "port", "sslPort", "enableSsl", "launchBrowser", "authenticationMethod", "authenticationRequired", "analyticsEnabled", "username", "password", "logLevel", "consoleLogLevel", "branch", "apiKey", "sslCertPath", "sslCertPassword", "urlBase", "instanceName", "applicationUrl", "updateAutomatically", "updateMechanism", "updateScriptPath", "proxyEnabled", "proxyType", "proxyHostname", "proxyPort", "proxyUsername", "proxyPassword", "proxyBypassFilter", "proxyBypassLocalAddresses", "certificateValidation", "backupFolder", "backupInterval", "backupRetention", "historyCleanupDays"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -135,14 +136,18 @@
         if self.url_base is None:
             _dict['urlBase'] = None
 
         # set to None if instance_name (nullable) is None
         if self.instance_name is None:
             _dict['instanceName'] = None
 
+        # set to None if application_url (nullable) is None
+        if self.application_url is None:
+            _dict['applicationUrl'] = None
+
         # set to None if update_script_path (nullable) is None
         if self.update_script_path is None:
             _dict['updateScriptPath'] = None
 
         # set to None if proxy_hostname (nullable) is None
         if self.proxy_hostname is None:
             _dict['proxyHostname'] = None
@@ -190,14 +195,15 @@
             "console_log_level": obj.get("consoleLogLevel"),
             "branch": obj.get("branch"),
             "api_key": obj.get("apiKey"),
             "ssl_cert_path": obj.get("sslCertPath"),
             "ssl_cert_password": obj.get("sslCertPassword"),
             "url_base": obj.get("urlBase"),
             "instance_name": obj.get("instanceName"),
+            "application_url": obj.get("applicationUrl"),
             "update_automatically": obj.get("updateAutomatically"),
             "update_mechanism": obj.get("updateMechanism"),
             "update_script_path": obj.get("updateScriptPath"),
             "proxy_enabled": obj.get("proxyEnabled"),
             "proxy_type": obj.get("proxyType"),
             "proxy_hostname": obj.get("proxyHostname"),
             "proxy_port": obj.get("proxyPort"),
```

### Comparing `prowlarr-py-0.3.2/prowlarr/models/host_statistics.py` & `prowlarr-py-0.4.0/prowlarr/models/host_statistics.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/indexer_capability_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/indexer_capability_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/indexer_category.py` & `prowlarr-py-0.4.0/prowlarr/models/indexer_category.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/indexer_editor_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/indexer_editor_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/indexer_privacy.py` & `prowlarr-py-0.4.0/prowlarr/models/indexer_privacy.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/indexer_proxy_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/indexer_proxy_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/indexer_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/indexer_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/indexer_statistics.py` & `prowlarr-py-0.4.0/prowlarr/models/indexer_statistics.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/indexer_stats_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/indexer_stats_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/indexer_status_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/indexer_status_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/localization_option.py` & `prowlarr-py-0.4.0/prowlarr/models/localization_option.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/log_file_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/log_file_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/log_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/log_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/log_resource_paging_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/log_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/movie_search_param.py` & `prowlarr-py-0.4.0/prowlarr/models/movie_search_param.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/music_search_param.py` & `prowlarr-py-0.4.0/prowlarr/models/music_search_param.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/notification_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/notification_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,22 +37,24 @@
     info_link: Optional[str]
     message: Optional[ProviderMessage]
     tags: Optional[List]
     presets: Optional[List]
     link: Optional[str]
     on_grab: Optional[bool]
     on_health_issue: Optional[bool]
+    on_health_restored: Optional[bool]
     on_application_update: Optional[bool]
     supports_on_grab: Optional[bool]
     include_manual_grabs: Optional[bool]
     supports_on_health_issue: Optional[bool]
+    supports_on_health_restored: Optional[bool]
     include_health_warnings: Optional[bool]
     supports_on_application_update: Optional[bool]
     test_command: Optional[str]
-    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "link", "onGrab", "onHealthIssue", "onApplicationUpdate", "supportsOnGrab", "includeManualGrabs", "supportsOnHealthIssue", "includeHealthWarnings", "supportsOnApplicationUpdate", "testCommand"]
+    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "link", "onGrab", "onHealthIssue", "onHealthRestored", "onApplicationUpdate", "supportsOnGrab", "includeManualGrabs", "supportsOnHealthIssue", "supportsOnHealthRestored", "includeHealthWarnings", "supportsOnApplicationUpdate", "testCommand"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -155,17 +157,19 @@
             "info_link": obj.get("infoLink"),
             "message": ProviderMessage.from_dict(obj.get("message")) if obj.get("message") is not None else None,
             "tags": obj.get("tags"),
             "presets": [NotificationResource.from_dict(_item) for _item in obj.get("presets")] if obj.get("presets") is not None else None,
             "link": obj.get("link"),
             "on_grab": obj.get("onGrab"),
             "on_health_issue": obj.get("onHealthIssue"),
+            "on_health_restored": obj.get("onHealthRestored"),
             "on_application_update": obj.get("onApplicationUpdate"),
             "supports_on_grab": obj.get("supportsOnGrab"),
             "include_manual_grabs": obj.get("includeManualGrabs"),
             "supports_on_health_issue": obj.get("supportsOnHealthIssue"),
+            "supports_on_health_restored": obj.get("supportsOnHealthRestored"),
             "include_health_warnings": obj.get("includeHealthWarnings"),
             "supports_on_application_update": obj.get("supportsOnApplicationUpdate"),
             "test_command": obj.get("testCommand")
         })
         return _obj
```

### Comparing `prowlarr-py-0.3.2/prowlarr/models/paging_resource_filter.py` & `prowlarr-py-0.4.0/prowlarr/models/paging_resource_filter.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/ping_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/ping_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/provider_message.py` & `prowlarr-py-0.4.0/prowlarr/models/provider_message.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/provider_message_type.py` & `prowlarr-py-0.4.0/prowlarr/models/provider_message_type.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/proxy_type.py` & `prowlarr-py-0.4.0/prowlarr/models/proxy_type.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/release_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/release_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import List, Optional
+from typing import List, Optional, Union
 from pydantic import BaseModel
 from prowlarr.models.download_protocol import DownloadProtocol
 from prowlarr.models.indexer_category import IndexerCategory
 
 class ReleaseResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `prowlarr-py-0.3.2/prowlarr/models/runtime_mode.py` & `prowlarr-py-0.4.0/prowlarr/models/runtime_mode.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/search_param.py` & `prowlarr-py-0.4.0/prowlarr/models/search_param.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/select_option.py` & `prowlarr-py-0.4.0/prowlarr/models/select_option.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/sort_direction.py` & `prowlarr-py-0.4.0/prowlarr/models/sort_direction.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/system_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/system_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/tag_details_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/tag_details_resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     Do not edit the class manually.
     """
     id: Optional[int]
     label: Optional[str]
     notification_ids: Optional[List]
     indexer_ids: Optional[List]
     indexer_proxy_ids: Optional[List]
-    __properties = ["id", "label", "notificationIds", "indexerIds", "indexerProxyIds"]
+    application_ids: Optional[List]
+    __properties = ["id", "label", "notificationIds", "indexerIds", "indexerProxyIds", "applicationIds"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -72,14 +73,18 @@
         if self.indexer_ids is None:
             _dict['indexerIds'] = None
 
         # set to None if indexer_proxy_ids (nullable) is None
         if self.indexer_proxy_ids is None:
             _dict['indexerProxyIds'] = None
 
+        # set to None if application_ids (nullable) is None
+        if self.application_ids is None:
+            _dict['applicationIds'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> TagDetailsResource:
         """Create an instance of TagDetailsResource from a dict"""
         if obj is None:
             return None
@@ -88,11 +93,12 @@
             return TagDetailsResource.parse_obj(obj)
 
         _obj = TagDetailsResource.parse_obj({
             "id": obj.get("id"),
             "label": obj.get("label"),
             "notification_ids": obj.get("notificationIds"),
             "indexer_ids": obj.get("indexerIds"),
-            "indexer_proxy_ids": obj.get("indexerProxyIds")
+            "indexer_proxy_ids": obj.get("indexerProxyIds"),
+            "application_ids": obj.get("applicationIds")
         })
         return _obj
```

### Comparing `prowlarr-py-0.3.2/prowlarr/models/tag_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/tag_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/task_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/task_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/tv_search_param.py` & `prowlarr-py-0.4.0/prowlarr/models/tv_search_param.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/ui_config_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/ui_config_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/update_changes.py` & `prowlarr-py-0.4.0/prowlarr/models/update_changes.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/update_mechanism.py` & `prowlarr-py-0.4.0/prowlarr/models/update_mechanism.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/update_resource.py` & `prowlarr-py-0.4.0/prowlarr/models/update_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/models/user_agent_statistics.py` & `prowlarr-py-0.4.0/prowlarr/models/user_agent_statistics.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr/rest.py` & `prowlarr-py-0.4.0/prowlarr/rest.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.3.2/prowlarr_py.egg-info/PKG-INFO` & `prowlarr-py-0.4.0/prowlarr_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prowlarr-py
-Version: 0.3.2
+Version: 0.4.0
 Summary: Prowlarr API wrapper
 Project-URL: Homepage, https://github.com/devopsarr/prowlarr-py
 Project-URL: Bug Tracker, https://github.com/devopsarr/prowlarr-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 
 # prowlarr-py
 Prowlarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.3.2
+- Package version: 0.4.0
 
 [comment]: # (x-release-please-end)
 - API version: 1.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
```

### Comparing `prowlarr-py-0.3.2/prowlarr_py.egg-info/SOURCES.txt` & `prowlarr-py-0.4.0/prowlarr_py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 prowlarr/__init__.py
 prowlarr/api_client.py
+prowlarr/api_response.py
 prowlarr/configuration.py
 prowlarr/exceptions.py
 prowlarr/rest.py
 prowlarr/api/__init__.py
 prowlarr/api/api_info_api.py
 prowlarr/api/app_profile_api.py
 prowlarr/api/application_api.py
```

### Comparing `prowlarr-py-0.3.2/pyproject.toml` & `prowlarr-py-0.4.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 [project]
 name = "prowlarr-py"
-version = "0.3.2"
+version = "0.4.0"
 dependencies = [
     "urllib3 >= 1.25.3",
     "python-dateutil",
     "requests>=2.28.1",
     "pydantic>=1.10.2",
     "aenum"
 ]
```

