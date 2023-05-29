# Comparing `tmp/radarr-py-0.2.2.tar.gz` & `tmp/radarr-py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radarr-py-0.2.2.tar", last modified: Mon Mar 27 14:23:49 2023, max compression
+gzip compressed data, was "radarr-py-0.3.0.tar", last modified: Mon May 29 06:42:04 2023, max compression
```

## Comparing `radarr-py-0.2.2.tar` & `radarr-py-0.3.0.tar`

### file list

```diff
@@ -1,215 +1,217 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:23:49.704659 radarr-py-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-03-27 14:23:34.000000 radarr-py-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    37764 2023-03-27 14:23:49.704659 radarr-py-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37292 2023-03-27 14:23:34.000000 radarr-py-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-27 14:23:34.000000 radarr-py-0.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:23:49.656657 radarr-py-0.2.2/radarr/
--rw-r--r--   0 runner    (1001) docker     (123)    12247 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:23:49.672657 radarr-py-0.2.2/radarr/api/
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/alternative_title_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/api_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/authentication_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22482 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/backup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23725 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/blocklist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13076 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/calendar_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/calendar_feed_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25027 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/collection_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23471 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/command_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/credit_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30446 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/custom_filter_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    35514 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/custom_format_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30446 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/delay_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/disk_space_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53854 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/download_client_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19137 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/download_client_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/extra_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/file_system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/health_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25831 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/history_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18582 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/host_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36645 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/import_exclusions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53182 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/import_list_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/import_list_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12560 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/import_list_movies_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52557 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/indexer_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18694 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/indexer_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/indexer_flag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/initialize_js_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/language_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/localization_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/log_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/manual_import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/media_cover_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19195 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/media_management_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52725 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/metadata_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30062 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/movie_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/movie_editor_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36977 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/movie_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/movie_import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23012 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/movie_lookup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29122 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/naming_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53397 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/notification_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/parse_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/ping_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25228 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/quality_definition_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30638 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/quality_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/quality_profile_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/queue_action_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26150 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/queue_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/queue_details_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/queue_status_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18200 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/release_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/release_push_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30991 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/remote_path_mapping_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/rename_movie_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30285 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/restriction_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23717 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/root_folder_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21832 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/static_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26845 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29517 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/tag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/tag_details_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/task_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/ui_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/update_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api/update_log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29525 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:23:49.700658 radarr-py-0.2.2/radarr/models/
--rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/add_movie_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/add_movie_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/alternative_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/alternative_title_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/api_info_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/apply_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/authentication_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/backup_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/backup_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/blocklist_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/blocklist_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/blocklist_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/certificate_validation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/collection_movie_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/collection_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/collection_update_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/colon_replacement_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/command_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/command_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/command_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/command_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/credit_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/credit_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/custom_filter_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/custom_format_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/custom_format_specification_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/database_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/delay_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/disk_space_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/download_client_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/download_client_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/download_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/extra_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/extra_file_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/field.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/file_date_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/health_check_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/health_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/history_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/history_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/host_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/import_exclusions_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/import_list_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/import_list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/import_list_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/indexer_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/indexer_flag_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/indexer_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/language_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/log_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/log_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/log_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/manual_import_reprocess_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/manual_import_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/media_cover.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/media_cover_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/media_info_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/media_management_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/metadata_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/metadata_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/modifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/monitor_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/movie_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/movie_editor_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/movie_file_list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/movie_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/movie_history_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    10213 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/movie_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    12205 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/movie_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/movie_runtime_format_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/movie_status_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/movie_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/naming_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/notification_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/paging_resource_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/parse_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/parsed_movie_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/ping_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/profile_format_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/proper_download_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/provider_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/provider_message_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/proxy_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/quality_definition_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/quality_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/quality_profile_quality_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/quality_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/queue_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/queue_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/queue_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/queue_status_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/rating_child.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/rating_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/ratings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/rejection.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/rejection_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/release_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/remote_path_mapping_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/rename_movie_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/rescan_after_refresh_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/restriction_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/root_folder_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/runtime_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/select_option.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/source.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/source_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/system_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/tag_details_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/tag_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/task_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/tmdb_country_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/tracked_download_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/tracked_download_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/tracked_download_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/ui_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/unmapped_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/update_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/update_mechanism.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/models/update_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-03-27 14:23:34.000000 radarr-py-0.2.2/radarr/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:23:49.704659 radarr-py-0.2.2/radarr_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37764 2023-03-27 14:23:49.000000 radarr-py-0.2.2/radarr_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-03-27 14:23:49.000000 radarr-py-0.2.2/radarr_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 14:23:49.000000 radarr-py-0.2.2/radarr_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-27 14:23:49.000000 radarr-py-0.2.2/radarr_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-27 14:23:49.000000 radarr-py-0.2.2/radarr_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 14:23:49.704659 radarr-py-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-27 14:23:34.000000 radarr-py-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:42:04.660362 radarr-py-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-29 06:41:42.000000 radarr-py-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    37806 2023-05-29 06:42:04.660362 radarr-py-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37334 2023-05-29 06:41:42.000000 radarr-py-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-29 06:41:42.000000 radarr-py-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:42:04.620361 radarr-py-0.3.0/radarr/
+-rw-r--r--   0 runner    (1001) docker     (123)    12302 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:42:04.632362 radarr-py-0.3.0/radarr/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/alternative_title_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/api_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/authentication_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22482 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/backup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23725 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/blocklist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13076 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/calendar_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/calendar_feed_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25027 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/collection_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23471 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/command_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/credit_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30446 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/custom_filter_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35514 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/custom_format_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30446 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/delay_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/disk_space_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54263 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/download_client_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19137 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/download_client_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/extra_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/file_system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/health_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25831 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/history_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18582 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/host_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36645 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/import_exclusions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53591 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/import_list_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/import_list_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12560 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/import_list_movies_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52966 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/indexer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18694 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/indexer_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/indexer_flag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/initialize_js_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/language_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/localization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/log_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/manual_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/media_cover_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19195 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/media_management_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53134 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/metadata_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31420 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/movie_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/movie_editor_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36977 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/movie_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/movie_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23012 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/movie_lookup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29122 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/naming_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53806 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/parse_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/ping_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25228 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/quality_definition_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30638 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/quality_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/quality_profile_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/queue_action_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26150 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/queue_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/queue_details_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/queue_status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18200 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/release_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/release_push_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30991 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/remote_path_mapping_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/rename_movie_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30285 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/restriction_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23717 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/root_folder_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21832 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/static_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26845 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29517 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/tag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/tag_details_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/task_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/ui_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/update_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/update_log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29639 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:42:04.656362 radarr-py-0.3.0/radarr/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/add_movie_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/add_movie_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/alternative_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/alternative_title_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/api_info_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/apply_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/authentication_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/backup_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/backup_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/blocklist_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/blocklist_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/blocklist_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/certificate_validation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/collection_movie_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/collection_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/collection_update_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/colon_replacement_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/command_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/command_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/command_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/command_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/command_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/credit_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/credit_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/custom_filter_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/custom_format_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/custom_format_specification_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/database_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/delay_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/disk_space_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/download_client_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/download_client_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/download_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/extra_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/extra_file_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/file_date_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/health_check_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/health_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/history_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/history_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/host_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/import_exclusions_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/import_list_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/import_list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/import_list_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/indexer_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/indexer_flag_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/indexer_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/language_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/log_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/log_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/log_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/manual_import_reprocess_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/manual_import_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/media_cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/media_cover_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/media_info_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/media_management_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/metadata_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/metadata_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/monitor_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/movie_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/movie_editor_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/movie_file_list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/movie_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/movie_history_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/movie_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/movie_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/movie_runtime_format_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/movie_status_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/movie_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/naming_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/notification_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/paging_resource_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/parse_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/parsed_movie_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/ping_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/profile_format_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/proper_download_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/provider_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/provider_message_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/proxy_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/quality_definition_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/quality_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/quality_profile_quality_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/quality_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/queue_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/queue_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/queue_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/queue_status_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/rating_child.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/rating_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/ratings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/rejection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/rejection_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9436 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/release_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/remote_path_mapping_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/rename_movie_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/rescan_after_refresh_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/restriction_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/root_folder_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/runtime_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/select_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/source_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/system_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/tag_details_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/tag_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/task_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/tmdb_country_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/tracked_download_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/tracked_download_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/tracked_download_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/ui_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/unmapped_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/update_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/update_mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/update_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:42:04.660362 radarr-py-0.3.0/radarr_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37806 2023-05-29 06:42:04.000000 radarr-py-0.3.0/radarr_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-05-29 06:42:04.000000 radarr-py-0.3.0/radarr_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 06:42:04.000000 radarr-py-0.3.0/radarr_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 06:42:04.000000 radarr-py-0.3.0/radarr_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 06:42:04.000000 radarr-py-0.3.0/radarr_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 06:42:04.660362 radarr-py-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-29 06:41:42.000000 radarr-py-0.3.0/setup.py
```

### Comparing `radarr-py-0.2.2/LICENSE` & `radarr-py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/PKG-INFO` & `radarr-py-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radarr-py
-Version: 0.2.2
+Version: 0.3.0
 Summary: Radarr API wrapper
 Project-URL: Homepage, https://github.com/devopsarr/radarr-py
 Project-URL: Bug Tracker, https://github.com/devopsarr/radarr-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 
 # radarr-py
 Radarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.2.2
+- Package version: 0.3.0
 
 [comment]: # (x-release-please-end)
 - API version: 3.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -358,14 +358,15 @@
  - [CollectionMovieResource](docs/CollectionMovieResource.md)
  - [CollectionResource](docs/CollectionResource.md)
  - [CollectionUpdateResource](docs/CollectionUpdateResource.md)
  - [ColonReplacementFormat](docs/ColonReplacementFormat.md)
  - [Command](docs/Command.md)
  - [CommandPriority](docs/CommandPriority.md)
  - [CommandResource](docs/CommandResource.md)
+ - [CommandResult](docs/CommandResult.md)
  - [CommandStatus](docs/CommandStatus.md)
  - [CommandTrigger](docs/CommandTrigger.md)
  - [CreditResource](docs/CreditResource.md)
  - [CreditType](docs/CreditType.md)
  - [CustomFilterResource](docs/CustomFilterResource.md)
  - [CustomFormatResource](docs/CustomFormatResource.md)
  - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
```

### Comparing `radarr-py-0.2.2/README.md` & `radarr-py-0.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # radarr-py
 Radarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.2.2
+- Package version: 0.3.0
 
 [comment]: # (x-release-please-end)
 - API version: 3.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -345,14 +345,15 @@
  - [CollectionMovieResource](docs/CollectionMovieResource.md)
  - [CollectionResource](docs/CollectionResource.md)
  - [CollectionUpdateResource](docs/CollectionUpdateResource.md)
  - [ColonReplacementFormat](docs/ColonReplacementFormat.md)
  - [Command](docs/Command.md)
  - [CommandPriority](docs/CommandPriority.md)
  - [CommandResource](docs/CommandResource.md)
+ - [CommandResult](docs/CommandResult.md)
  - [CommandStatus](docs/CommandStatus.md)
  - [CommandTrigger](docs/CommandTrigger.md)
  - [CreditResource](docs/CreditResource.md)
  - [CreditType](docs/CreditType.md)
  - [CustomFilterResource](docs/CustomFilterResource.md)
  - [CustomFormatResource](docs/CustomFormatResource.md)
  - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
```

### Comparing `radarr-py-0.2.2/pyproject.toml` & `radarr-py-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 [project]
 name = "radarr-py"
-version = "0.2.2"
+version = "0.3.0"
 dependencies = [
     "urllib3 >= 1.25.3",
     "python-dateutil",
     "requests>=2.28.1",
     "pydantic>=1.10.2",
     "aenum"
 ]
```

### Comparing `radarr-py-0.2.2/radarr/__init__.py` & `radarr-py-0.3.0/radarr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # x-release-please-start-version
-__version__ = "0.2.2"
+__version__ = "0.3.0"
 # x-release-please-end
 
 # import apis into sdk package
 from radarr.api.alternative_title_api import AlternativeTitleApi
 from radarr.api.api_info_api import ApiInfoApi
 from radarr.api.authentication_api import AuthenticationApi
 from radarr.api.backup_api import BackupApi
@@ -114,14 +114,15 @@
 from radarr.models.collection_movie_resource import CollectionMovieResource
 from radarr.models.collection_resource import CollectionResource
 from radarr.models.collection_update_resource import CollectionUpdateResource
 from radarr.models.colon_replacement_format import ColonReplacementFormat
 from radarr.models.command import Command
 from radarr.models.command_priority import CommandPriority
 from radarr.models.command_resource import CommandResource
+from radarr.models.command_result import CommandResult
 from radarr.models.command_status import CommandStatus
 from radarr.models.command_trigger import CommandTrigger
 from radarr.models.credit_resource import CreditResource
 from radarr.models.credit_type import CreditType
 from radarr.models.custom_filter_resource import CustomFilterResource
 from radarr.models.custom_format_resource import CustomFormatResource
 from radarr.models.custom_format_specification_schema import CustomFormatSpecificationSchema
```

### Comparing `radarr-py-0.2.2/radarr/api/__init__.py` & `radarr-py-0.3.0/radarr/api/__init__.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/alternative_title_api.py` & `radarr-py-0.3.0/radarr/api/alternative_title_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/api_info_api.py` & `radarr-py-0.3.0/radarr/api/api_info_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/authentication_api.py` & `radarr-py-0.3.0/radarr/api/authentication_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/backup_api.py` & `radarr-py-0.3.0/radarr/api/backup_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/blocklist_api.py` & `radarr-py-0.3.0/radarr/api/blocklist_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/calendar_api.py` & `radarr-py-0.3.0/radarr/api/calendar_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/calendar_feed_api.py` & `radarr-py-0.3.0/radarr/api/calendar_feed_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,29 +38,29 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_feed_v3_calendar_radarr_ics(self, past_days : Optional[StrictInt] = None, future_days : Optional[StrictInt] = None, tag_list : Optional[StrictStr] = None, unmonitored : Optional[StrictBool] = None, **kwargs) -> None:  # noqa: E501
+    def get_feed_v3_calendar_radarr_ics(self, past_days : Optional[StrictInt] = None, future_days : Optional[StrictInt] = None, tags : Optional[StrictStr] = None, unmonitored : Optional[StrictBool] = None, **kwargs) -> None:  # noqa: E501
         """get_feed_v3_calendar_radarr_ics  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_feed_v3_calendar_radarr_ics(past_days, future_days, tag_list, unmonitored, async_req=True)
+        >>> thread = api.get_feed_v3_calendar_radarr_ics(past_days, future_days, tags, unmonitored, async_req=True)
         >>> result = thread.get()
 
         :param past_days:
         :type past_days: int
         :param future_days:
         :type future_days: int
-        :param tag_list:
-        :type tag_list: str
+        :param tags:
+        :type tags: str
         :param unmonitored:
         :type unmonitored: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -71,32 +71,32 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_feed_v3_calendar_radarr_ics_with_http_info(past_days, future_days, tag_list, unmonitored, **kwargs)  # noqa: E501
+        return self.get_feed_v3_calendar_radarr_ics_with_http_info(past_days, future_days, tags, unmonitored, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_feed_v3_calendar_radarr_ics_with_http_info(self, past_days : Optional[StrictInt] = None, future_days : Optional[StrictInt] = None, tag_list : Optional[StrictStr] = None, unmonitored : Optional[StrictBool] = None, **kwargs):  # noqa: E501
+    def get_feed_v3_calendar_radarr_ics_with_http_info(self, past_days : Optional[StrictInt] = None, future_days : Optional[StrictInt] = None, tags : Optional[StrictStr] = None, unmonitored : Optional[StrictBool] = None, **kwargs):  # noqa: E501
         """get_feed_v3_calendar_radarr_ics  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_feed_v3_calendar_radarr_ics_with_http_info(past_days, future_days, tag_list, unmonitored, async_req=True)
+        >>> thread = api.get_feed_v3_calendar_radarr_ics_with_http_info(past_days, future_days, tags, unmonitored, async_req=True)
         >>> result = thread.get()
 
         :param past_days:
         :type past_days: int
         :param future_days:
         :type future_days: int
-        :param tag_list:
-        :type tag_list: str
+        :param tags:
+        :type tags: str
         :param unmonitored:
         :type unmonitored: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -120,15 +120,15 @@
         """
 
         _params = locals()
 
         _all_params = [
             'past_days',
             'future_days',
-            'tag_list',
+            'tags',
             'unmonitored'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -156,16 +156,16 @@
 
         # process the query parameters
         _query_params = []
         if _params.get('past_days') is not None:  # noqa: E501
             _query_params.append(('pastDays', _params['past_days']))
         if _params.get('future_days') is not None:  # noqa: E501
             _query_params.append(('futureDays', _params['future_days']))
-        if _params.get('tag_list') is not None:  # noqa: E501
-            _query_params.append(('tagList', _params['tag_list']))
+        if _params.get('tags') is not None:  # noqa: E501
+            _query_params.append(('tags', _params['tags']))
         if _params.get('unmonitored') is not None:  # noqa: E501
             _query_params.append(('unmonitored', _params['unmonitored']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
```

### Comparing `radarr-py-0.2.2/radarr/api/collection_api.py` & `radarr-py-0.3.0/radarr/api/collection_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/command_api.py` & `radarr-py-0.3.0/radarr/api/command_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/credit_api.py` & `radarr-py-0.3.0/radarr/api/credit_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/custom_filter_api.py` & `radarr-py-0.3.0/radarr/api/custom_filter_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/custom_format_api.py` & `radarr-py-0.3.0/radarr/api/custom_format_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/delay_profile_api.py` & `radarr-py-0.3.0/radarr/api/delay_profile_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/disk_space_api.py` & `radarr-py-0.3.0/radarr/api/disk_space_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/download_client_api.py` & `radarr-py-0.3.0/radarr/api/download_client_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
 from radarr.models.download_client_resource import DownloadClientResource
 
 from radarr.api_client import ApiClient
 from radarr.exceptions import (  # noqa: F401
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

### Comparing `radarr-py-0.2.2/radarr/api/download_client_config_api.py` & `radarr-py-0.3.0/radarr/api/download_client_config_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/extra_file_api.py` & `radarr-py-0.3.0/radarr/api/extra_file_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/file_system_api.py` & `radarr-py-0.3.0/radarr/api/file_system_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/health_api.py` & `radarr-py-0.3.0/radarr/api/health_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/history_api.py` & `radarr-py-0.3.0/radarr/api/history_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/host_config_api.py` & `radarr-py-0.3.0/radarr/api/host_config_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/import_exclusions_api.py` & `radarr-py-0.3.0/radarr/api/import_exclusions_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/import_list_api.py` & `radarr-py-0.3.0/radarr/api/import_list_api.py`

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
 
 from radarr.models.import_list_resource import ImportListResource
 
 from radarr.api_client import ApiClient
 from radarr.exceptions import (  # noqa: F401
@@ -1150,25 +1150,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_import_list(self, id : StrictStr, import_list_resource : Optional[ImportListResource] = None, **kwargs) -> ImportListResource:  # noqa: E501
+    def update_import_list(self, id : StrictStr, force_save : Optional[StrictBool] = None, import_list_resource : Optional[ImportListResource] = None, **kwargs) -> ImportListResource:  # noqa: E501
         """update_import_list  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_import_list(id, import_list_resource, async_req=True)
+        >>> thread = api.update_import_list(id, force_save, import_list_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param import_list_resource:
         :type import_list_resource: ImportListResource
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
         :rtype: ImportListResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_import_list_with_http_info(id, import_list_resource, **kwargs)  # noqa: E501
+        return self.update_import_list_with_http_info(id, force_save, import_list_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_import_list_with_http_info(self, id : StrictStr, import_list_resource : Optional[ImportListResource] = None, **kwargs):  # noqa: E501
+    def update_import_list_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, import_list_resource : Optional[ImportListResource] = None, **kwargs):  # noqa: E501
         """update_import_list  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_import_list_with_http_info(id, import_list_resource, async_req=True)
+        >>> thread = api.update_import_list_with_http_info(id, force_save, import_list_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param import_list_resource:
         :type import_list_resource: ImportListResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1223,14 +1227,15 @@
         :rtype: tuple(ImportListResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'force_save',
             'import_list_resource'
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

### Comparing `radarr-py-0.2.2/radarr/api/import_list_config_api.py` & `radarr-py-0.3.0/radarr/api/import_list_config_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/import_list_movies_api.py` & `radarr-py-0.3.0/radarr/api/import_list_movies_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/indexer_api.py` & `radarr-py-0.3.0/radarr/api/indexer_api.py`

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
 
 from radarr.models.indexer_resource import IndexerResource
 
 from radarr.api_client import ApiClient
 from radarr.exceptions import (  # noqa: F401
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

### Comparing `radarr-py-0.2.2/radarr/api/indexer_config_api.py` & `radarr-py-0.3.0/radarr/api/indexer_config_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/indexer_flag_api.py` & `radarr-py-0.3.0/radarr/api/indexer_flag_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/initialize_js_api.py` & `radarr-py-0.3.0/radarr/api/initialize_js_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/language_api.py` & `radarr-py-0.3.0/radarr/api/language_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/localization_api.py` & `radarr-py-0.3.0/radarr/api/localization_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/log_api.py` & `radarr-py-0.3.0/radarr/api/log_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/log_file_api.py` & `radarr-py-0.3.0/radarr/api/log_file_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/manual_import_api.py` & `radarr-py-0.3.0/radarr/api/manual_import_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/media_cover_api.py` & `radarr-py-0.3.0/radarr/api/media_cover_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/media_management_config_api.py` & `radarr-py-0.3.0/radarr/api/media_management_config_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/metadata_api.py` & `radarr-py-0.3.0/radarr/api/metadata_api.py`

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
 
 from radarr.models.metadata_resource import MetadataResource
 
 from radarr.api_client import ApiClient
 from radarr.exceptions import (  # noqa: F401
@@ -1150,25 +1150,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_metadata(self, id : StrictStr, metadata_resource : Optional[MetadataResource] = None, **kwargs) -> MetadataResource:  # noqa: E501
+    def update_metadata(self, id : StrictStr, force_save : Optional[StrictBool] = None, metadata_resource : Optional[MetadataResource] = None, **kwargs) -> MetadataResource:  # noqa: E501
         """update_metadata  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_metadata(id, metadata_resource, async_req=True)
+        >>> thread = api.update_metadata(id, force_save, metadata_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param metadata_resource:
         :type metadata_resource: MetadataResource
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
         :rtype: MetadataResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_metadata_with_http_info(id, metadata_resource, **kwargs)  # noqa: E501
+        return self.update_metadata_with_http_info(id, force_save, metadata_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_metadata_with_http_info(self, id : StrictStr, metadata_resource : Optional[MetadataResource] = None, **kwargs):  # noqa: E501
+    def update_metadata_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, metadata_resource : Optional[MetadataResource] = None, **kwargs):  # noqa: E501
         """update_metadata  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_metadata_with_http_info(id, metadata_resource, async_req=True)
+        >>> thread = api.update_metadata_with_http_info(id, force_save, metadata_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param metadata_resource:
         :type metadata_resource: MetadataResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1223,14 +1227,15 @@
         :rtype: tuple(MetadataResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'force_save',
             'metadata_resource'
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

### Comparing `radarr-py-0.2.2/radarr/api/metadata_config_api.py` & `radarr-py-0.3.0/radarr/api/metadata_config_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/movie_api.py` & `radarr-py-0.3.0/radarr/api/movie_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
 from radarr.models.movie_resource import MovieResource
 
 from radarr.api_client import ApiClient
 from radarr.exceptions import (  # noqa: F401
@@ -187,25 +187,29 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_movie(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
+    def delete_movie(self, id : StrictInt, delete_files : Optional[StrictBool] = None, add_import_exclusion : Optional[StrictBool] = None, **kwargs) -> None:  # noqa: E501
         """delete_movie  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_movie(id, async_req=True)
+        >>> thread = api.delete_movie(id, delete_files, add_import_exclusion, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
+        :param delete_files:
+        :type delete_files: bool
+        :param add_import_exclusion:
+        :type add_import_exclusion: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -214,28 +218,32 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_movie_with_http_info(id, **kwargs)  # noqa: E501
+        return self.delete_movie_with_http_info(id, delete_files, add_import_exclusion, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_movie_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+    def delete_movie_with_http_info(self, id : StrictInt, delete_files : Optional[StrictBool] = None, add_import_exclusion : Optional[StrictBool] = None, **kwargs):  # noqa: E501
         """delete_movie  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_movie_with_http_info(id, async_req=True)
+        >>> thread = api.delete_movie_with_http_info(id, delete_files, add_import_exclusion, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
+        :param delete_files:
+        :type delete_files: bool
+        :param add_import_exclusion:
+        :type add_import_exclusion: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -255,15 +263,17 @@
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
+            'id',
+            'delete_files',
+            'add_import_exclusion'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -288,14 +298,18 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('delete_files') is not None:  # noqa: E501
+            _query_params.append(('deleteFiles', _params['delete_files']))
+        if _params.get('add_import_exclusion') is not None:  # noqa: E501
+            _query_params.append(('addImportExclusion', _params['add_import_exclusion']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -604,25 +618,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_movie(self, id : StrictStr, movie_resource : Optional[MovieResource] = None, **kwargs) -> MovieResource:  # noqa: E501
+    def update_movie(self, id : StrictStr, move_files : Optional[StrictBool] = None, movie_resource : Optional[MovieResource] = None, **kwargs) -> MovieResource:  # noqa: E501
         """update_movie  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_movie(id, movie_resource, async_req=True)
+        >>> thread = api.update_movie(id, move_files, movie_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param move_files:
+        :type move_files: bool
         :param movie_resource:
         :type movie_resource: MovieResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -633,28 +649,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: MovieResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_movie_with_http_info(id, movie_resource, **kwargs)  # noqa: E501
+        return self.update_movie_with_http_info(id, move_files, movie_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_movie_with_http_info(self, id : StrictStr, movie_resource : Optional[MovieResource] = None, **kwargs):  # noqa: E501
+    def update_movie_with_http_info(self, id : StrictStr, move_files : Optional[StrictBool] = None, movie_resource : Optional[MovieResource] = None, **kwargs):  # noqa: E501
         """update_movie  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_movie_with_http_info(id, movie_resource, async_req=True)
+        >>> thread = api.update_movie_with_http_info(id, move_files, movie_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param move_files:
+        :type move_files: bool
         :param movie_resource:
         :type movie_resource: MovieResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -677,14 +695,15 @@
         :rtype: tuple(MovieResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'move_files',
             'movie_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -710,14 +729,16 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('move_files') is not None:  # noqa: E501
+            _query_params.append(('moveFiles', _params['move_files']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
```

### Comparing `radarr-py-0.2.2/radarr/api/movie_editor_api.py` & `radarr-py-0.3.0/radarr/api/movie_editor_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/movie_file_api.py` & `radarr-py-0.3.0/radarr/api/movie_file_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/movie_import_api.py` & `radarr-py-0.3.0/radarr/api/movie_import_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/movie_lookup_api.py` & `radarr-py-0.3.0/radarr/api/movie_lookup_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/naming_config_api.py` & `radarr-py-0.3.0/radarr/api/naming_config_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/notification_api.py` & `radarr-py-0.3.0/radarr/api/notification_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
 from radarr.models.notification_resource import NotificationResource
 
 from radarr.api_client import ApiClient
 from radarr.exceptions import (  # noqa: F401
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

### Comparing `radarr-py-0.2.2/radarr/api/parse_api.py` & `radarr-py-0.3.0/radarr/api/parse_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/ping_api.py` & `radarr-py-0.3.0/radarr/api/ping_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/quality_definition_api.py` & `radarr-py-0.3.0/radarr/api/quality_definition_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/quality_profile_api.py` & `radarr-py-0.3.0/radarr/api/quality_profile_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/quality_profile_schema_api.py` & `radarr-py-0.3.0/radarr/api/quality_profile_schema_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/queue_action_api.py` & `radarr-py-0.3.0/radarr/api/queue_action_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/queue_api.py` & `radarr-py-0.3.0/radarr/api/queue_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/queue_details_api.py` & `radarr-py-0.3.0/radarr/api/queue_details_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/queue_status_api.py` & `radarr-py-0.3.0/radarr/api/queue_status_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/release_api.py` & `radarr-py-0.3.0/radarr/api/release_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/release_push_api.py` & `radarr-py-0.3.0/radarr/api/release_push_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/remote_path_mapping_api.py` & `radarr-py-0.3.0/radarr/api/remote_path_mapping_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/rename_movie_api.py` & `radarr-py-0.3.0/radarr/api/rename_movie_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/restriction_api.py` & `radarr-py-0.3.0/radarr/api/restriction_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/root_folder_api.py` & `radarr-py-0.3.0/radarr/api/root_folder_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/static_resource_api.py` & `radarr-py-0.3.0/radarr/api/static_resource_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/system_api.py` & `radarr-py-0.3.0/radarr/api/system_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/tag_api.py` & `radarr-py-0.3.0/radarr/api/tag_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/tag_details_api.py` & `radarr-py-0.3.0/radarr/api/tag_details_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/task_api.py` & `radarr-py-0.3.0/radarr/api/task_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/ui_config_api.py` & `radarr-py-0.3.0/radarr/api/ui_config_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/update_api.py` & `radarr-py-0.3.0/radarr/api/update_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api/update_log_file_api.py` & `radarr-py-0.3.0/radarr/api/update_log_file_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/api_client.py` & `radarr-py-0.3.0/radarr/api_client.py`

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
-        self.user_agent = 'radarr-py/v0.2.2'
+        self.user_agent = 'radarr-py/v0.3.0'
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

### Comparing `radarr-py-0.2.2/radarr/configuration.py` & `radarr-py-0.3.0/radarr/configuration.py`

 * *Files 1% similar despite different names*

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
         self._base_path = "http://localhost:7878" if host is None else host
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
         self.logger["package_logger"] = logging.getLogger("radarr")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
@@ -421,15 +426,15 @@
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         # x-release-please-start-version
-        sdkversion = '0.2.2'
+        sdkversion = '0.3.0'
         # x-release-please-end
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3.0.0\n"\
                "SDK Package Version: {sdkversion}".\
                format(env=sys.platform, pyversion=sys.version, sdkversion=sdkversion)
```

### Comparing `radarr-py-0.2.2/radarr/exceptions.py` & `radarr-py-0.3.0/radarr/exceptions.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/__init__.py` & `radarr-py-0.3.0/radarr/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from radarr.models.collection_movie_resource import CollectionMovieResource
 from radarr.models.collection_resource import CollectionResource
 from radarr.models.collection_update_resource import CollectionUpdateResource
 from radarr.models.colon_replacement_format import ColonReplacementFormat
 from radarr.models.command import Command
 from radarr.models.command_priority import CommandPriority
 from radarr.models.command_resource import CommandResource
+from radarr.models.command_result import CommandResult
 from radarr.models.command_status import CommandStatus
 from radarr.models.command_trigger import CommandTrigger
 from radarr.models.credit_resource import CreditResource
 from radarr.models.credit_type import CreditType
 from radarr.models.custom_filter_resource import CustomFilterResource
 from radarr.models.custom_format_resource import CustomFormatResource
 from radarr.models.custom_format_specification_schema import CustomFormatSpecificationSchema
```

### Comparing `radarr-py-0.2.2/radarr/models/add_movie_method.py` & `radarr-py-0.3.0/radarr/models/add_movie_method.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/add_movie_options.py` & `radarr-py-0.3.0/radarr/models/add_movie_options.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/alternative_title.py` & `radarr-py-0.3.0/radarr/models/alternative_title.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/alternative_title_resource.py` & `radarr-py-0.3.0/radarr/models/alternative_title_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/api_info_resource.py` & `radarr-py-0.3.0/radarr/models/api_info_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/apply_tags.py` & `radarr-py-0.3.0/radarr/models/apply_tags.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/authentication_type.py` & `radarr-py-0.3.0/radarr/models/authentication_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/backup_resource.py` & `radarr-py-0.3.0/radarr/models/backup_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/backup_type.py` & `radarr-py-0.3.0/radarr/models/backup_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/blocklist_bulk_resource.py` & `radarr-py-0.3.0/radarr/models/blocklist_bulk_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/blocklist_resource.py` & `radarr-py-0.3.0/radarr/models/blocklist_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/blocklist_resource_paging_resource.py` & `radarr-py-0.3.0/radarr/models/blocklist_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/certificate_validation_type.py` & `radarr-py-0.3.0/radarr/models/certificate_validation_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/collection_movie_resource.py` & `radarr-py-0.3.0/radarr/models/collection_movie_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/collection_resource.py` & `radarr-py-0.3.0/radarr/models/collection_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/collection_update_resource.py` & `radarr-py-0.3.0/radarr/models/collection_update_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/colon_replacement_format.py` & `radarr-py-0.3.0/radarr/models/colon_replacement_format.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/command.py` & `radarr-py-0.3.0/radarr/models/command.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/command_priority.py` & `radarr-py-0.3.0/radarr/models/command_priority.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/command_resource.py` & `radarr-py-0.3.0/radarr/models/command_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel
 from radarr.models.command import Command
 from radarr.models.command_priority import CommandPriority
+from radarr.models.command_result import CommandResult
 from radarr.models.command_status import CommandStatus
 from radarr.models.command_trigger import CommandTrigger
 
 class CommandResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -33,26 +34,27 @@
     id: Optional[int]
     name: Optional[str]
     command_name: Optional[str]
     message: Optional[str]
     body: Optional[Command]
     priority: Optional[CommandPriority]
     status: Optional[CommandStatus]
+    result: Optional[CommandResult]
     queued: Optional[datetime]
     started: Optional[datetime]
     ended: Optional[datetime]
     duration: Optional[str]
     exception: Optional[str]
     trigger: Optional[CommandTrigger]
     client_user_agent: Optional[str]
     state_change_time: Optional[datetime]
     send_updates_to_client: Optional[bool]
     update_scheduled_task: Optional[bool]
     last_execution_time: Optional[datetime]
-    __properties = ["id", "name", "commandName", "message", "body", "priority", "status", "queued", "started", "ended", "duration", "exception", "trigger", "clientUserAgent", "stateChangeTime", "sendUpdatesToClient", "updateScheduledTask", "lastExecutionTime"]
+    __properties = ["id", "name", "commandName", "message", "body", "priority", "status", "result", "queued", "started", "ended", "duration", "exception", "trigger", "clientUserAgent", "stateChangeTime", "sendUpdatesToClient", "updateScheduledTask", "lastExecutionTime"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -131,14 +133,15 @@
             "id": obj.get("id"),
             "name": obj.get("name"),
             "command_name": obj.get("commandName"),
             "message": obj.get("message"),
             "body": Command.from_dict(obj.get("body")) if obj.get("body") is not None else None,
             "priority": obj.get("priority"),
             "status": obj.get("status"),
+            "result": obj.get("result"),
             "queued": obj.get("queued"),
             "started": obj.get("started"),
             "ended": obj.get("ended"),
             "duration": obj.get("duration"),
             "exception": obj.get("exception"),
             "trigger": obj.get("trigger"),
             "client_user_agent": obj.get("clientUserAgent"),
```

### Comparing `radarr-py-0.2.2/radarr/models/command_status.py` & `radarr-py-0.3.0/radarr/models/command_status.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/command_trigger.py` & `radarr-py-0.3.0/radarr/models/command_trigger.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/credit_resource.py` & `radarr-py-0.3.0/radarr/models/credit_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/credit_type.py` & `radarr-py-0.3.0/radarr/models/credit_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/custom_filter_resource.py` & `radarr-py-0.3.0/radarr/models/custom_filter_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/custom_format_resource.py` & `radarr-py-0.3.0/radarr/models/custom_format_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/custom_format_specification_schema.py` & `radarr-py-0.3.0/radarr/models/custom_format_specification_schema.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/database_type.py` & `radarr-py-0.3.0/radarr/models/database_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/delay_profile_resource.py` & `radarr-py-0.3.0/radarr/models/delay_profile_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/disk_space_resource.py` & `radarr-py-0.3.0/radarr/models/disk_space_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/download_client_config_resource.py` & `radarr-py-0.3.0/radarr/models/download_client_config_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/download_client_resource.py` & `radarr-py-0.3.0/radarr/models/download_client_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/download_protocol.py` & `radarr-py-0.3.0/radarr/models/download_protocol.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/extra_file_resource.py` & `radarr-py-0.3.0/radarr/models/extra_file_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/extra_file_type.py` & `radarr-py-0.3.0/radarr/models/extra_file_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/field.py` & `radarr-py-0.3.0/radarr/models/field.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/file_date_type.py` & `radarr-py-0.3.0/radarr/models/file_date_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/health_check_result.py` & `radarr-py-0.3.0/radarr/models/health_check_result.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/health_resource.py` & `radarr-py-0.3.0/radarr/models/health_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/history_resource.py` & `radarr-py-0.3.0/radarr/models/history_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/history_resource_paging_resource.py` & `radarr-py-0.3.0/radarr/models/history_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/host_config_resource.py` & `radarr-py-0.3.0/radarr/models/host_config_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/import_exclusions_resource.py` & `radarr-py-0.3.0/radarr/models/import_exclusions_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/import_list_config_resource.py` & `radarr-py-0.3.0/radarr/models/import_list_config_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/import_list_resource.py` & `radarr-py-0.3.0/radarr/models/import_list_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/import_list_type.py` & `radarr-py-0.3.0/radarr/models/import_list_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/indexer_config_resource.py` & `radarr-py-0.3.0/radarr/models/indexer_config_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/indexer_flag_resource.py` & `radarr-py-0.3.0/radarr/models/indexer_flag_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/indexer_resource.py` & `radarr-py-0.3.0/radarr/models/indexer_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/language.py` & `radarr-py-0.3.0/radarr/models/language.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/language_resource.py` & `radarr-py-0.3.0/radarr/models/language_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/log_file_resource.py` & `radarr-py-0.3.0/radarr/models/log_file_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/log_resource.py` & `radarr-py-0.3.0/radarr/models/log_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/log_resource_paging_resource.py` & `radarr-py-0.3.0/radarr/models/log_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/manual_import_reprocess_resource.py` & `radarr-py-0.3.0/radarr/models/manual_import_reprocess_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/manual_import_resource.py` & `radarr-py-0.3.0/radarr/models/manual_import_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/media_cover.py` & `radarr-py-0.3.0/radarr/models/media_cover.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/media_cover_types.py` & `radarr-py-0.3.0/radarr/models/update_mechanism.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,25 +15,24 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class MediaCoverTypes(str, Enum):
+class UpdateMechanism(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    UNKNOWN = 'unknown'
-    POSTER = 'poster'
-    BANNER = 'banner'
-    FANART = 'fanart'
-    SCREENSHOT = 'screenshot'
-    HEADSHOT = 'headshot'
+    BUILTIN = 'builtIn'
+    SCRIPT = 'script'
+    EXTERNAL = 'external'
+    APT = 'apt'
+    DOCKER = 'docker'
```

### Comparing `radarr-py-0.2.2/radarr/models/media_info_resource.py` & `radarr-py-0.3.0/radarr/models/media_info_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import Optional, Union
 from pydantic import BaseModel
 
 class MediaInfoResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `radarr-py-0.2.2/radarr/models/media_management_config_resource.py` & `radarr-py-0.3.0/radarr/models/media_management_config_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/metadata_config_resource.py` & `radarr-py-0.3.0/radarr/models/metadata_config_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/metadata_resource.py` & `radarr-py-0.3.0/radarr/models/metadata_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/modifier.py` & `radarr-py-0.3.0/radarr/models/modifier.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/monitor_types.py` & `radarr-py-0.3.0/radarr/models/monitor_types.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/movie_collection.py` & `radarr-py-0.3.0/radarr/models/movie_collection.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/movie_editor_resource.py` & `radarr-py-0.3.0/radarr/models/movie_editor_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/movie_file_list_resource.py` & `radarr-py-0.3.0/radarr/models/movie_file_list_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/movie_file_resource.py` & `radarr-py-0.3.0/radarr/models/movie_file_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/movie_history_event_type.py` & `radarr-py-0.3.0/radarr/models/movie_history_event_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/movie_metadata.py` & `radarr-py-0.3.0/radarr/models/movie_metadata.py`

 * *Files 1% similar despite different names*

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
 from radarr.models.alternative_title import AlternativeTitle
 from radarr.models.language import Language
 from radarr.models.media_cover import MediaCover
 from radarr.models.movie_status_type import MovieStatusType
 from radarr.models.movie_translation import MovieTranslation
 from radarr.models.ratings import Ratings
```

### Comparing `radarr-py-0.2.2/radarr/models/movie_resource.py` & `radarr-py-0.3.0/radarr/models/movie_resource.py`

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
 from radarr.models.add_movie_options import AddMovieOptions
 from radarr.models.alternative_title_resource import AlternativeTitleResource
 from radarr.models.language import Language
 from radarr.models.media_cover import MediaCover
 from radarr.models.movie_collection import MovieCollection
 from radarr.models.movie_file_resource import MovieFileResource
```

### Comparing `radarr-py-0.2.2/radarr/models/movie_runtime_format_type.py` & `radarr-py-0.3.0/radarr/models/movie_runtime_format_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/movie_status_type.py` & `radarr-py-0.3.0/radarr/models/movie_status_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/movie_translation.py` & `radarr-py-0.3.0/radarr/models/movie_translation.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/naming_config_resource.py` & `radarr-py-0.3.0/radarr/models/naming_config_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/notification_resource.py` & `radarr-py-0.3.0/radarr/models/notification_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,28 +44,32 @@
     on_upgrade: Optional[bool]
     on_rename: Optional[bool]
     on_movie_added: Optional[bool]
     on_movie_delete: Optional[bool]
     on_movie_file_delete: Optional[bool]
     on_movie_file_delete_for_upgrade: Optional[bool]
     on_health_issue: Optional[bool]
+    on_health_restored: Optional[bool]
     on_application_update: Optional[bool]
+    on_manual_interaction_required: Optional[bool]
     supports_on_grab: Optional[bool]
     supports_on_download: Optional[bool]
     supports_on_upgrade: Optional[bool]
     supports_on_rename: Optional[bool]
     supports_on_movie_added: Optional[bool]
     supports_on_movie_delete: Optional[bool]
     supports_on_movie_file_delete: Optional[bool]
     supports_on_movie_file_delete_for_upgrade: Optional[bool]
     supports_on_health_issue: Optional[bool]
+    supports_on_health_restored: Optional[bool]
     supports_on_application_update: Optional[bool]
+    supports_on_manual_interaction_required: Optional[bool]
     include_health_warnings: Optional[bool]
     test_command: Optional[str]
-    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "link", "onGrab", "onDownload", "onUpgrade", "onRename", "onMovieAdded", "onMovieDelete", "onMovieFileDelete", "onMovieFileDeleteForUpgrade", "onHealthIssue", "onApplicationUpdate", "supportsOnGrab", "supportsOnDownload", "supportsOnUpgrade", "supportsOnRename", "supportsOnMovieAdded", "supportsOnMovieDelete", "supportsOnMovieFileDelete", "supportsOnMovieFileDeleteForUpgrade", "supportsOnHealthIssue", "supportsOnApplicationUpdate", "includeHealthWarnings", "testCommand"]
+    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "link", "onGrab", "onDownload", "onUpgrade", "onRename", "onMovieAdded", "onMovieDelete", "onMovieFileDelete", "onMovieFileDeleteForUpgrade", "onHealthIssue", "onHealthRestored", "onApplicationUpdate", "onManualInteractionRequired", "supportsOnGrab", "supportsOnDownload", "supportsOnUpgrade", "supportsOnRename", "supportsOnMovieAdded", "supportsOnMovieDelete", "supportsOnMovieFileDelete", "supportsOnMovieFileDeleteForUpgrade", "supportsOnHealthIssue", "supportsOnHealthRestored", "supportsOnApplicationUpdate", "supportsOnManualInteractionRequired", "includeHealthWarnings", "testCommand"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -175,23 +179,27 @@
             "on_upgrade": obj.get("onUpgrade"),
             "on_rename": obj.get("onRename"),
             "on_movie_added": obj.get("onMovieAdded"),
             "on_movie_delete": obj.get("onMovieDelete"),
             "on_movie_file_delete": obj.get("onMovieFileDelete"),
             "on_movie_file_delete_for_upgrade": obj.get("onMovieFileDeleteForUpgrade"),
             "on_health_issue": obj.get("onHealthIssue"),
+            "on_health_restored": obj.get("onHealthRestored"),
             "on_application_update": obj.get("onApplicationUpdate"),
+            "on_manual_interaction_required": obj.get("onManualInteractionRequired"),
             "supports_on_grab": obj.get("supportsOnGrab"),
             "supports_on_download": obj.get("supportsOnDownload"),
             "supports_on_upgrade": obj.get("supportsOnUpgrade"),
             "supports_on_rename": obj.get("supportsOnRename"),
             "supports_on_movie_added": obj.get("supportsOnMovieAdded"),
             "supports_on_movie_delete": obj.get("supportsOnMovieDelete"),
             "supports_on_movie_file_delete": obj.get("supportsOnMovieFileDelete"),
             "supports_on_movie_file_delete_for_upgrade": obj.get("supportsOnMovieFileDeleteForUpgrade"),
             "supports_on_health_issue": obj.get("supportsOnHealthIssue"),
+            "supports_on_health_restored": obj.get("supportsOnHealthRestored"),
             "supports_on_application_update": obj.get("supportsOnApplicationUpdate"),
+            "supports_on_manual_interaction_required": obj.get("supportsOnManualInteractionRequired"),
             "include_health_warnings": obj.get("includeHealthWarnings"),
             "test_command": obj.get("testCommand")
         })
         return _obj
```

### Comparing `radarr-py-0.2.2/radarr/models/paging_resource_filter.py` & `radarr-py-0.3.0/radarr/models/paging_resource_filter.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/parse_resource.py` & `radarr-py-0.3.0/radarr/models/parse_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/parsed_movie_info.py` & `radarr-py-0.3.0/radarr/models/parsed_movie_info.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/ping_resource.py` & `radarr-py-0.3.0/radarr/models/ping_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/profile_format_item_resource.py` & `radarr-py-0.3.0/radarr/models/profile_format_item_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/proper_download_types.py` & `radarr-py-0.3.0/radarr/models/proper_download_types.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/provider_message.py` & `radarr-py-0.3.0/radarr/models/provider_message.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/provider_message_type.py` & `radarr-py-0.3.0/radarr/models/provider_message_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/proxy_type.py` & `radarr-py-0.3.0/radarr/models/proxy_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/quality.py` & `radarr-py-0.3.0/radarr/models/quality.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/quality_definition_resource.py` & `radarr-py-0.3.0/radarr/models/quality_definition_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import Optional, Union
 from pydantic import BaseModel
 from radarr.models.quality import Quality
 
 class QualityDefinitionResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `radarr-py-0.2.2/radarr/models/quality_model.py` & `radarr-py-0.3.0/radarr/models/quality_model.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/quality_profile_quality_item_resource.py` & `radarr-py-0.3.0/radarr/models/quality_profile_quality_item_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/quality_profile_resource.py` & `radarr-py-0.3.0/radarr/models/quality_profile_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/queue_bulk_resource.py` & `radarr-py-0.3.0/radarr/models/queue_bulk_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/queue_resource.py` & `radarr-py-0.3.0/radarr/models/queue_resource.py`

 * *Files 1% similar despite different names*

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
 from radarr.models.custom_format_resource import CustomFormatResource
 from radarr.models.download_protocol import DownloadProtocol
 from radarr.models.language import Language
 from radarr.models.movie_resource import MovieResource
 from radarr.models.quality_model import QualityModel
 from radarr.models.tracked_download_state import TrackedDownloadState
```

### Comparing `radarr-py-0.2.2/radarr/models/queue_resource_paging_resource.py` & `radarr-py-0.3.0/radarr/models/queue_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/queue_status_resource.py` & `radarr-py-0.3.0/radarr/models/queue_status_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/rating_child.py` & `radarr-py-0.3.0/radarr/models/rating_child.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import Optional, Union
 from pydantic import BaseModel
 from radarr.models.rating_type import RatingType
 
 class RatingChild(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `radarr-py-0.2.2/radarr/models/rating_type.py` & `radarr-py-0.3.0/radarr/models/rating_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/ratings.py` & `radarr-py-0.3.0/radarr/models/ratings.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/rejection.py` & `radarr-py-0.3.0/radarr/models/rejection.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/rejection_type.py` & `radarr-py-0.3.0/radarr/models/rejection_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/release_resource.py` & `radarr-py-0.3.0/radarr/models/release_resource.py`

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
 from radarr.models.custom_format_resource import CustomFormatResource
 from radarr.models.download_protocol import DownloadProtocol
 from radarr.models.language import Language
 from radarr.models.quality_model import QualityModel
 
 class ReleaseResource(BaseModel):
```

### Comparing `radarr-py-0.2.2/radarr/models/remote_path_mapping_resource.py` & `radarr-py-0.3.0/radarr/models/remote_path_mapping_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/rename_movie_resource.py` & `radarr-py-0.3.0/radarr/models/rename_movie_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/rescan_after_refresh_type.py` & `radarr-py-0.3.0/radarr/models/rescan_after_refresh_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/restriction_resource.py` & `radarr-py-0.3.0/radarr/models/restriction_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/revision.py` & `radarr-py-0.3.0/radarr/models/revision.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/root_folder_resource.py` & `radarr-py-0.3.0/radarr/models/root_folder_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/runtime_mode.py` & `radarr-py-0.3.0/radarr/models/runtime_mode.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/select_option.py` & `radarr-py-0.3.0/radarr/models/select_option.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/sort_direction.py` & `radarr-py-0.3.0/radarr/models/sort_direction.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/source.py` & `radarr-py-0.3.0/radarr/models/source.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/source_type.py` & `radarr-py-0.3.0/radarr/models/source_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/system_resource.py` & `radarr-py-0.3.0/radarr/models/system_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/tag_details_resource.py` & `radarr-py-0.3.0/radarr/models/tag_details_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/tag_resource.py` & `radarr-py-0.3.0/radarr/models/tag_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/task_resource.py` & `radarr-py-0.3.0/radarr/models/task_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/tmdb_country_code.py` & `radarr-py-0.3.0/radarr/models/tmdb_country_code.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/tracked_download_state.py` & `radarr-py-0.3.0/radarr/models/tracked_download_state.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/tracked_download_status.py` & `radarr-py-0.3.0/radarr/models/tracked_download_status.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/tracked_download_status_message.py` & `radarr-py-0.3.0/radarr/models/tracked_download_status_message.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/ui_config_resource.py` & `radarr-py-0.3.0/radarr/models/ui_config_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/unmapped_folder.py` & `radarr-py-0.3.0/radarr/models/unmapped_folder.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/update_changes.py` & `radarr-py-0.3.0/radarr/models/update_changes.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/models/update_mechanism.py` & `radarr-py-0.3.0/radarr/models/media_cover_types.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,24 +15,26 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class UpdateMechanism(str, Enum):
+class MediaCoverTypes(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    BUILTIN = 'builtIn'
-    SCRIPT = 'script'
-    EXTERNAL = 'external'
-    APT = 'apt'
-    DOCKER = 'docker'
+    UNKNOWN = 'unknown'
+    POSTER = 'poster'
+    BANNER = 'banner'
+    FANART = 'fanart'
+    SCREENSHOT = 'screenshot'
+    HEADSHOT = 'headshot'
+    CLEARLOGO = 'clearlogo'
```

### Comparing `radarr-py-0.2.2/radarr/models/update_resource.py` & `radarr-py-0.3.0/radarr/models/update_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr/rest.py` & `radarr-py-0.3.0/radarr/rest.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.2.2/radarr_py.egg-info/PKG-INFO` & `radarr-py-0.3.0/radarr_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radarr-py
-Version: 0.2.2
+Version: 0.3.0
 Summary: Radarr API wrapper
 Project-URL: Homepage, https://github.com/devopsarr/radarr-py
 Project-URL: Bug Tracker, https://github.com/devopsarr/radarr-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 
 # radarr-py
 Radarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.2.2
+- Package version: 0.3.0
 
 [comment]: # (x-release-please-end)
 - API version: 3.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -358,14 +358,15 @@
  - [CollectionMovieResource](docs/CollectionMovieResource.md)
  - [CollectionResource](docs/CollectionResource.md)
  - [CollectionUpdateResource](docs/CollectionUpdateResource.md)
  - [ColonReplacementFormat](docs/ColonReplacementFormat.md)
  - [Command](docs/Command.md)
  - [CommandPriority](docs/CommandPriority.md)
  - [CommandResource](docs/CommandResource.md)
+ - [CommandResult](docs/CommandResult.md)
  - [CommandStatus](docs/CommandStatus.md)
  - [CommandTrigger](docs/CommandTrigger.md)
  - [CreditResource](docs/CreditResource.md)
  - [CreditType](docs/CreditType.md)
  - [CustomFilterResource](docs/CustomFilterResource.md)
  - [CustomFormatResource](docs/CustomFormatResource.md)
  - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
```

### Comparing `radarr-py-0.2.2/radarr_py.egg-info/SOURCES.txt` & `radarr-py-0.3.0/radarr_py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 radarr/__init__.py
 radarr/api_client.py
+radarr/api_response.py
 radarr/configuration.py
 radarr/exceptions.py
 radarr/rest.py
 radarr/api/__init__.py
 radarr/api/alternative_title_api.py
 radarr/api/api_info_api.py
 radarr/api/authentication_api.py
@@ -93,14 +94,15 @@
 radarr/models/collection_movie_resource.py
 radarr/models/collection_resource.py
 radarr/models/collection_update_resource.py
 radarr/models/colon_replacement_format.py
 radarr/models/command.py
 radarr/models/command_priority.py
 radarr/models/command_resource.py
+radarr/models/command_result.py
 radarr/models/command_status.py
 radarr/models/command_trigger.py
 radarr/models/credit_resource.py
 radarr/models/credit_type.py
 radarr/models/custom_filter_resource.py
 radarr/models/custom_format_resource.py
 radarr/models/custom_format_specification_schema.py
```

