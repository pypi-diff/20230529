# Comparing `tmp/lidarr-py-0.2.2.tar.gz` & `tmp/lidarr-py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lidarr-py-0.2.2.tar", last modified: Mon Mar 27 14:23:35 2023, max compression
+gzip compressed data, was "lidarr-py-0.3.0.tar", last modified: Mon May 29 06:41:55 2023, max compression
```

## Comparing `lidarr-py-0.2.2.tar` & `lidarr-py-0.3.0.tar`

### file list

```diff
@@ -1,249 +1,251 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:23:35.950342 lidarr-py-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40327 2023-03-27 14:23:35.950342 lidarr-py-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39855 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:23:35.918341 lidarr-py-0.2.2/lidarr/
--rw-r--r--   0 runner    (1001) docker     (123)    14655 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:23:35.926341 lidarr-py-0.2.2/lidarr/api/
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37736 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/album_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/album_lookup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/album_studio_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/api_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/artist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/artist_editor_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/artist_lookup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/authentication_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22482 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/backup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17838 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/blocklist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13525 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/calendar_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/calendar_feed_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23471 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/command_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30446 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/custom_filter_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    35514 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/custom_format_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/cutoff_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36254 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/delay_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/disk_space_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53854 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/download_client_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19199 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/download_client_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/file_system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/health_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28885 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/history_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18582 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/host_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53182 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/import_list_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    31183 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/import_list_exclusion_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52557 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/indexer_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18756 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/indexer_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/initialize_js_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/language_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/localization_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/log_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/manual_import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/media_cover_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/media_management_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52725 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30734 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/metadata_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/metadata_profile_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19315 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/metadata_provider_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/missing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30009 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/naming_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53397 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/notification_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/parse_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/ping_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25228 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/quality_definition_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30638 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/quality_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/quality_profile_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/queue_action_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27560 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/queue_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13818 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/queue_details_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/queue_status_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/release_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30638 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/release_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12841 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/release_push_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30991 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/remote_path_mapping_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/rename_track_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/retag_track_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30254 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/root_folder_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21832 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/static_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26845 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29517 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/tag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/tag_details_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/task_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/track_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37824 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/track_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/ui_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/update_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api/update_log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29525 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:23:35.946341 lidarr-py-0.2.2/lidarr/models/
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/add_album_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/add_artist_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/album.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/album_add_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/album_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/album_list_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/album_release.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/album_release_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/album_release_list_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/album_release_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/album_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/album_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/album_statistics_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/album_studio_artist_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/album_studio_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/albums_monitored_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/allow_fingerprinting.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/apply_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/artist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/artist_editor_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/artist_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/artist_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/artist_metadata_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/artist_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/artist_statistics_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/artist_status_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/artist_title_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/authentication_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/backup_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/backup_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/blocklist_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/blocklist_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/blocklist_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/certificate_validation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/command_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/command_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/command_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/command_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/custom_filter_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/custom_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/custom_format_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/custom_format_specification_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/database_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/delay_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/disk_space_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/download_client_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/download_client_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/download_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/entity_history_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/field.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/file_date_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/health_check_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/health_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/history_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/history_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/host_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/i_custom_format_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/import_list_exclusion_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/import_list_monitor_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/import_list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/import_list_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/indexer_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/indexer_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/iso_country.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/language_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/log_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/log_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/log_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/manual_import_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/manual_import_update_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/media_cover.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/media_cover_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/media_info_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/media_info_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/media_management_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/medium_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/metadata_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/metadata_profile_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/metadata_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/metadata_provider_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/metadata_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/monitor_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/monitoring_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/naming_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/new_item_monitor_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/notification_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/paging_resource_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/parse_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/parsed_album_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/parsed_track_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/ping_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/primary_album_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/profile_format_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/profile_format_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/profile_primary_album_type_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/profile_primary_album_type_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/profile_release_status_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/profile_release_status_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/profile_secondary_album_type_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/profile_secondary_album_type_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/proper_download_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/provider_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/provider_message_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/proxy_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/quality_definition_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/quality_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/quality_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/quality_profile_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/quality_profile_quality_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/quality_profile_quality_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/quality_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/queue_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/queue_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/queue_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/queue_status_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/ratings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/rejection.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/rejection_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/release_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/release_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/release_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/remote_path_mapping_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/rename_track_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/rescan_after_refresh_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/retag_track_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/root_folder_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/runtime_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/secondary_album_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/select_option.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/system_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/tag_details_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/tag_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/tag_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/task_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/track.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/track_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/track_file_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/track_file_list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/track_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/track_list_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/track_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/tracked_download_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/tracked_download_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/tracked_download_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/ui_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/update_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/update_mechanism.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/update_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/models/write_audio_tags_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/lidarr/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:23:35.950342 lidarr-py-0.2.2/lidarr_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40327 2023-03-27 14:23:35.000000 lidarr-py-0.2.2/lidarr_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-03-27 14:23:35.000000 lidarr-py-0.2.2/lidarr_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 14:23:35.000000 lidarr-py-0.2.2/lidarr_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-27 14:23:35.000000 lidarr-py-0.2.2/lidarr_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-27 14:23:35.000000 lidarr-py-0.2.2/lidarr_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 14:23:35.950342 lidarr-py-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-27 14:23:21.000000 lidarr-py-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:55.320011 lidarr-py-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    40369 2023-05-29 06:41:55.320011 lidarr-py-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39897 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:55.272012 lidarr-py-0.3.0/lidarr/
+-rw-r--r--   0 runner    (1001) docker     (123)    14710 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:55.288012 lidarr-py-0.3.0/lidarr/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38749 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/album_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/album_lookup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/album_studio_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/api_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31554 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/artist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/artist_editor_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/artist_lookup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/authentication_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22482 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/backup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17838 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/blocklist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13525 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/calendar_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/calendar_feed_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23471 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/command_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30446 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/custom_filter_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35514 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/custom_format_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/cutoff_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36254 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/delay_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/disk_space_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54263 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/download_client_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19199 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/download_client_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/file_system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/health_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28885 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/history_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18582 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/host_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53591 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/import_list_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31183 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/import_list_exclusion_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52966 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/indexer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18756 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/indexer_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/initialize_js_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/language_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/localization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/log_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/manual_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/media_cover_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/media_management_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53134 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30734 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/metadata_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/metadata_profile_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19315 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/metadata_provider_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/missing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30583 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/naming_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53806 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/parse_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/ping_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25228 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/quality_definition_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30638 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/quality_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/quality_profile_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/queue_action_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27560 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/queue_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13818 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/queue_details_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/queue_status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/release_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30638 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/release_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12841 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/release_push_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30991 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/remote_path_mapping_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/rename_track_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/retag_track_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30254 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/root_folder_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21832 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/static_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26845 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29517 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/tag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/tag_details_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/task_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/track_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37824 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/track_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/ui_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/update_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/update_log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29639 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:55.320011 lidarr-py-0.3.0/lidarr/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/add_album_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/add_artist_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_add_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_list_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_release_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_release_list_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_release_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_statistics_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_studio_artist_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_studio_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/albums_monitored_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/allow_fingerprinting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/apply_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/artist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/artist_editor_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/artist_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/artist_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/artist_metadata_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/artist_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/artist_statistics_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/artist_status_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/artist_title_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/authentication_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/backup_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/backup_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/blocklist_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/blocklist_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/blocklist_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/certificate_validation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/command_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/command_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/command_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/command_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/command_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/custom_filter_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/custom_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/custom_format_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/custom_format_specification_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/database_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/delay_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/disk_space_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/download_client_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/download_client_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/download_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/entity_history_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/file_date_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/health_check_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/health_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/history_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/history_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/host_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/i_custom_format_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/import_list_exclusion_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/import_list_monitor_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/import_list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/import_list_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/indexer_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/indexer_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/iso_country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/language_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/log_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/log_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/log_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/manual_import_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/manual_import_update_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/media_cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/media_cover_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/media_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/media_info_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/media_management_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/medium_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/metadata_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/metadata_profile_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/metadata_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/metadata_provider_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/metadata_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/monitor_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/monitoring_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/naming_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/new_item_monitor_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/notification_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/paging_resource_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/parse_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/parsed_album_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/parsed_track_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/ping_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/primary_album_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/profile_format_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/profile_format_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/profile_primary_album_type_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/profile_primary_album_type_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/profile_release_status_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/profile_release_status_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/profile_secondary_album_type_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/profile_secondary_album_type_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/proper_download_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/provider_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/provider_message_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/proxy_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/quality_definition_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/quality_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/quality_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/quality_profile_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/quality_profile_quality_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/quality_profile_quality_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/quality_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/queue_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/queue_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/queue_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/queue_status_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/ratings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/rejection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/rejection_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/release_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/release_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/release_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/remote_path_mapping_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/rename_track_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/rescan_after_refresh_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/retag_track_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/root_folder_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/runtime_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/secondary_album_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/select_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/system_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/tag_details_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/tag_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/tag_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/task_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/track_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/track_file_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/track_file_list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/track_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/track_list_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/track_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/tracked_download_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/tracked_download_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/tracked_download_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/ui_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/update_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/update_mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/update_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/write_audio_tags_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:55.320011 lidarr-py-0.3.0/lidarr_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40369 2023-05-29 06:41:55.000000 lidarr-py-0.3.0/lidarr_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-05-29 06:41:55.000000 lidarr-py-0.3.0/lidarr_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 06:41:55.000000 lidarr-py-0.3.0/lidarr_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 06:41:55.000000 lidarr-py-0.3.0/lidarr_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 06:41:55.000000 lidarr-py-0.3.0/lidarr_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 06:41:55.320011 lidarr-py-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/setup.py
```

### Comparing `lidarr-py-0.2.2/LICENSE` & `lidarr-py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/PKG-INFO` & `lidarr-py-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lidarr-py
-Version: 0.2.2
+Version: 0.3.0
 Summary: Lidarr API wrapper
 Project-URL: Homepage, https://github.com/devopsarr/lidarr-py
 Project-URL: Bug Tracker, https://github.com/devopsarr/lidarr-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 
 # lidarr-py
 Lidarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.2.2
+- Package version: 0.3.0
 
 [comment]: # (x-release-please-end)
 - API version: 1.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -378,14 +378,15 @@
  - [BlocklistBulkResource](docs/BlocklistBulkResource.md)
  - [BlocklistResource](docs/BlocklistResource.md)
  - [BlocklistResourcePagingResource](docs/BlocklistResourcePagingResource.md)
  - [CertificateValidationType](docs/CertificateValidationType.md)
  - [Command](docs/Command.md)
  - [CommandPriority](docs/CommandPriority.md)
  - [CommandResource](docs/CommandResource.md)
+ - [CommandResult](docs/CommandResult.md)
  - [CommandStatus](docs/CommandStatus.md)
  - [CommandTrigger](docs/CommandTrigger.md)
  - [CustomFilterResource](docs/CustomFilterResource.md)
  - [CustomFormat](docs/CustomFormat.md)
  - [CustomFormatResource](docs/CustomFormatResource.md)
  - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
  - [DatabaseType](docs/DatabaseType.md)
```

### Comparing `lidarr-py-0.2.2/README.md` & `lidarr-py-0.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lidarr-py
 Lidarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.2.2
+- Package version: 0.3.0
 
 [comment]: # (x-release-please-end)
 - API version: 1.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -365,14 +365,15 @@
  - [BlocklistBulkResource](docs/BlocklistBulkResource.md)
  - [BlocklistResource](docs/BlocklistResource.md)
  - [BlocklistResourcePagingResource](docs/BlocklistResourcePagingResource.md)
  - [CertificateValidationType](docs/CertificateValidationType.md)
  - [Command](docs/Command.md)
  - [CommandPriority](docs/CommandPriority.md)
  - [CommandResource](docs/CommandResource.md)
+ - [CommandResult](docs/CommandResult.md)
  - [CommandStatus](docs/CommandStatus.md)
  - [CommandTrigger](docs/CommandTrigger.md)
  - [CustomFilterResource](docs/CustomFilterResource.md)
  - [CustomFormat](docs/CustomFormat.md)
  - [CustomFormatResource](docs/CustomFormatResource.md)
  - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
  - [DatabaseType](docs/DatabaseType.md)
```

### Comparing `lidarr-py-0.2.2/lidarr/__init__.py` & `lidarr-py-0.3.0/lidarr/__init__.py`

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
 from lidarr.api.album_api import AlbumApi
 from lidarr.api.album_lookup_api import AlbumLookupApi
 from lidarr.api.album_studio_api import AlbumStudioApi
 from lidarr.api.api_info_api import ApiInfoApi
@@ -133,14 +133,15 @@
 from lidarr.models.blocklist_bulk_resource import BlocklistBulkResource
 from lidarr.models.blocklist_resource import BlocklistResource
 from lidarr.models.blocklist_resource_paging_resource import BlocklistResourcePagingResource
 from lidarr.models.certificate_validation_type import CertificateValidationType
 from lidarr.models.command import Command
 from lidarr.models.command_priority import CommandPriority
 from lidarr.models.command_resource import CommandResource
+from lidarr.models.command_result import CommandResult
 from lidarr.models.command_status import CommandStatus
 from lidarr.models.command_trigger import CommandTrigger
 from lidarr.models.custom_filter_resource import CustomFilterResource
 from lidarr.models.custom_format import CustomFormat
 from lidarr.models.custom_format_resource import CustomFormatResource
 from lidarr.models.custom_format_specification_schema import CustomFormatSpecificationSchema
 from lidarr.models.database_type import DatabaseType
```

### Comparing `lidarr-py-0.2.2/lidarr/api/__init__.py` & `lidarr-py-0.3.0/lidarr/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/album_api.py` & `lidarr-py-0.3.0/lidarr/api/album_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,25 +188,29 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_album(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
+    def delete_album(self, id : StrictInt, delete_files : Optional[StrictBool] = None, add_import_list_exclusion : Optional[StrictBool] = None, **kwargs) -> None:  # noqa: E501
         """delete_album  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_album(id, async_req=True)
+        >>> thread = api.delete_album(id, delete_files, add_import_list_exclusion, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
+        :param delete_files:
+        :type delete_files: bool
+        :param add_import_list_exclusion:
+        :type add_import_list_exclusion: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -215,28 +219,32 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_album_with_http_info(id, **kwargs)  # noqa: E501
+        return self.delete_album_with_http_info(id, delete_files, add_import_list_exclusion, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_album_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+    def delete_album_with_http_info(self, id : StrictInt, delete_files : Optional[StrictBool] = None, add_import_list_exclusion : Optional[StrictBool] = None, **kwargs):  # noqa: E501
         """delete_album  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_album_with_http_info(id, async_req=True)
+        >>> thread = api.delete_album_with_http_info(id, delete_files, add_import_list_exclusion, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
+        :param delete_files:
+        :type delete_files: bool
+        :param add_import_list_exclusion:
+        :type add_import_list_exclusion: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -256,15 +264,17 @@
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
+            'id',
+            'delete_files',
+            'add_import_list_exclusion'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -289,14 +299,18 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('delete_files') is not None:  # noqa: E501
+            _query_params.append(('deleteFiles', _params['delete_files']))
+        if _params.get('add_import_list_exclusion') is not None:  # noqa: E501
+            _query_params.append(('addImportListExclusion', _params['add_import_list_exclusion']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
```

### Comparing `lidarr-py-0.2.2/lidarr/api/album_lookup_api.py` & `lidarr-py-0.3.0/lidarr/api/album_lookup_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/album_studio_api.py` & `lidarr-py-0.3.0/lidarr/api/album_studio_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/api_info_api.py` & `lidarr-py-0.3.0/lidarr/api/api_info_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/artist_api.py` & `lidarr-py-0.3.0/lidarr/api/artist_api.py`

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
 
 from lidarr.models.artist_resource import ArtistResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
@@ -187,25 +187,29 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_artist(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
+    def delete_artist(self, id : StrictInt, delete_files : Optional[StrictBool] = None, add_import_list_exclusion : Optional[StrictBool] = None, **kwargs) -> None:  # noqa: E501
         """delete_artist  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_artist(id, async_req=True)
+        >>> thread = api.delete_artist(id, delete_files, add_import_list_exclusion, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
+        :param delete_files:
+        :type delete_files: bool
+        :param add_import_list_exclusion:
+        :type add_import_list_exclusion: bool
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
-        return self.delete_artist_with_http_info(id, **kwargs)  # noqa: E501
+        return self.delete_artist_with_http_info(id, delete_files, add_import_list_exclusion, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_artist_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+    def delete_artist_with_http_info(self, id : StrictInt, delete_files : Optional[StrictBool] = None, add_import_list_exclusion : Optional[StrictBool] = None, **kwargs):  # noqa: E501
         """delete_artist  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_artist_with_http_info(id, async_req=True)
+        >>> thread = api.delete_artist_with_http_info(id, delete_files, add_import_list_exclusion, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
+        :param delete_files:
+        :type delete_files: bool
+        :param add_import_list_exclusion:
+        :type add_import_list_exclusion: bool
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
+            'add_import_list_exclusion'
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
+        if _params.get('add_import_list_exclusion') is not None:  # noqa: E501
+            _query_params.append(('addImportListExclusion', _params['add_import_list_exclusion']))
 
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
-    def update_artist(self, id : StrictStr, artist_resource : Optional[ArtistResource] = None, **kwargs) -> ArtistResource:  # noqa: E501
+    def update_artist(self, id : StrictStr, move_files : Optional[StrictBool] = None, artist_resource : Optional[ArtistResource] = None, **kwargs) -> ArtistResource:  # noqa: E501
         """update_artist  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_artist(id, artist_resource, async_req=True)
+        >>> thread = api.update_artist(id, move_files, artist_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param move_files:
+        :type move_files: bool
         :param artist_resource:
         :type artist_resource: ArtistResource
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
         :rtype: ArtistResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_artist_with_http_info(id, artist_resource, **kwargs)  # noqa: E501
+        return self.update_artist_with_http_info(id, move_files, artist_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_artist_with_http_info(self, id : StrictStr, artist_resource : Optional[ArtistResource] = None, **kwargs):  # noqa: E501
+    def update_artist_with_http_info(self, id : StrictStr, move_files : Optional[StrictBool] = None, artist_resource : Optional[ArtistResource] = None, **kwargs):  # noqa: E501
         """update_artist  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_artist_with_http_info(id, artist_resource, async_req=True)
+        >>> thread = api.update_artist_with_http_info(id, move_files, artist_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param move_files:
+        :type move_files: bool
         :param artist_resource:
         :type artist_resource: ArtistResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -677,14 +695,15 @@
         :rtype: tuple(ArtistResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'move_files',
             'artist_resource'
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

### Comparing `lidarr-py-0.2.2/lidarr/api/artist_editor_api.py` & `lidarr-py-0.3.0/lidarr/api/artist_editor_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/artist_lookup_api.py` & `lidarr-py-0.3.0/lidarr/api/artist_lookup_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/authentication_api.py` & `lidarr-py-0.3.0/lidarr/api/authentication_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/backup_api.py` & `lidarr-py-0.3.0/lidarr/api/backup_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/blocklist_api.py` & `lidarr-py-0.3.0/lidarr/api/blocklist_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/calendar_api.py` & `lidarr-py-0.3.0/lidarr/api/calendar_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/calendar_feed_api.py` & `lidarr-py-0.3.0/lidarr/api/calendar_feed_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/command_api.py` & `lidarr-py-0.3.0/lidarr/api/command_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/custom_filter_api.py` & `lidarr-py-0.3.0/lidarr/api/custom_filter_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/custom_format_api.py` & `lidarr-py-0.3.0/lidarr/api/custom_format_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/cutoff_api.py` & `lidarr-py-0.3.0/lidarr/api/cutoff_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/delay_profile_api.py` & `lidarr-py-0.3.0/lidarr/api/delay_profile_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/disk_space_api.py` & `lidarr-py-0.3.0/lidarr/api/disk_space_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/download_client_api.py` & `lidarr-py-0.3.0/lidarr/api/download_client_api.py`

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
 
 from lidarr.models.download_client_resource import DownloadClientResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
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

### Comparing `lidarr-py-0.2.2/lidarr/api/download_client_config_api.py` & `lidarr-py-0.3.0/lidarr/api/download_client_config_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/file_system_api.py` & `lidarr-py-0.3.0/lidarr/api/file_system_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/health_api.py` & `lidarr-py-0.3.0/lidarr/api/health_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/history_api.py` & `lidarr-py-0.3.0/lidarr/api/history_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/host_config_api.py` & `lidarr-py-0.3.0/lidarr/api/host_config_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/import_list_api.py` & `lidarr-py-0.3.0/lidarr/api/import_list_api.py`

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
 
 from lidarr.models.import_list_resource import ImportListResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
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

### Comparing `lidarr-py-0.2.2/lidarr/api/import_list_exclusion_api.py` & `lidarr-py-0.3.0/lidarr/api/import_list_exclusion_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/indexer_api.py` & `lidarr-py-0.3.0/lidarr/api/indexer_api.py`

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
 
 from lidarr.models.indexer_resource import IndexerResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
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

### Comparing `lidarr-py-0.2.2/lidarr/api/indexer_config_api.py` & `lidarr-py-0.3.0/lidarr/api/indexer_config_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/initialize_js_api.py` & `lidarr-py-0.3.0/lidarr/api/initialize_js_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/language_api.py` & `lidarr-py-0.3.0/lidarr/api/language_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/localization_api.py` & `lidarr-py-0.3.0/lidarr/api/localization_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/log_api.py` & `lidarr-py-0.3.0/lidarr/api/log_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/log_file_api.py` & `lidarr-py-0.3.0/lidarr/api/log_file_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/manual_import_api.py` & `lidarr-py-0.3.0/lidarr/api/manual_import_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/media_cover_api.py` & `lidarr-py-0.3.0/lidarr/api/media_cover_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/media_management_config_api.py` & `lidarr-py-0.3.0/lidarr/api/media_management_config_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/metadata_api.py` & `lidarr-py-0.3.0/lidarr/api/metadata_api.py`

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
 
 from lidarr.models.metadata_resource import MetadataResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
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

### Comparing `lidarr-py-0.2.2/lidarr/api/metadata_profile_api.py` & `lidarr-py-0.3.0/lidarr/api/metadata_profile_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/metadata_profile_schema_api.py` & `lidarr-py-0.3.0/lidarr/api/metadata_profile_schema_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/metadata_provider_config_api.py` & `lidarr-py-0.3.0/lidarr/api/metadata_provider_config_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/missing_api.py` & `lidarr-py-0.3.0/lidarr/api/missing_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/naming_config_api.py` & `lidarr-py-0.3.0/lidarr/api/naming_config_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,27 +314,29 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_naming_config_examples(self, rename_tracks : Optional[StrictBool] = None, replace_illegal_characters : Optional[StrictBool] = None, standard_track_format : Optional[StrictStr] = None, multi_disc_track_format : Optional[StrictStr] = None, artist_folder_format : Optional[StrictStr] = None, include_artist_name : Optional[StrictBool] = None, include_album_title : Optional[StrictBool] = None, include_quality : Optional[StrictBool] = None, replace_spaces : Optional[StrictBool] = None, separator : Optional[StrictStr] = None, number_style : Optional[StrictStr] = None, id : Optional[StrictInt] = None, resource_name : Optional[StrictStr] = None, **kwargs) -> None:  # noqa: E501
+    def get_naming_config_examples(self, rename_tracks : Optional[StrictBool] = None, replace_illegal_characters : Optional[StrictBool] = None, colon_replacement_format : Optional[StrictInt] = None, standard_track_format : Optional[StrictStr] = None, multi_disc_track_format : Optional[StrictStr] = None, artist_folder_format : Optional[StrictStr] = None, include_artist_name : Optional[StrictBool] = None, include_album_title : Optional[StrictBool] = None, include_quality : Optional[StrictBool] = None, replace_spaces : Optional[StrictBool] = None, separator : Optional[StrictStr] = None, number_style : Optional[StrictStr] = None, id : Optional[StrictInt] = None, resource_name : Optional[StrictStr] = None, **kwargs) -> None:  # noqa: E501
         """get_naming_config_examples  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_naming_config_examples(rename_tracks, replace_illegal_characters, standard_track_format, multi_disc_track_format, artist_folder_format, include_artist_name, include_album_title, include_quality, replace_spaces, separator, number_style, id, resource_name, async_req=True)
+        >>> thread = api.get_naming_config_examples(rename_tracks, replace_illegal_characters, colon_replacement_format, standard_track_format, multi_disc_track_format, artist_folder_format, include_artist_name, include_album_title, include_quality, replace_spaces, separator, number_style, id, resource_name, async_req=True)
         >>> result = thread.get()
 
         :param rename_tracks:
         :type rename_tracks: bool
         :param replace_illegal_characters:
         :type replace_illegal_characters: bool
+        :param colon_replacement_format:
+        :type colon_replacement_format: int
         :param standard_track_format:
         :type standard_track_format: str
         :param multi_disc_track_format:
         :type multi_disc_track_format: str
         :param artist_folder_format:
         :type artist_folder_format: str
         :param include_artist_name:
@@ -365,30 +367,32 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_naming_config_examples_with_http_info(rename_tracks, replace_illegal_characters, standard_track_format, multi_disc_track_format, artist_folder_format, include_artist_name, include_album_title, include_quality, replace_spaces, separator, number_style, id, resource_name, **kwargs)  # noqa: E501
+        return self.get_naming_config_examples_with_http_info(rename_tracks, replace_illegal_characters, colon_replacement_format, standard_track_format, multi_disc_track_format, artist_folder_format, include_artist_name, include_album_title, include_quality, replace_spaces, separator, number_style, id, resource_name, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_naming_config_examples_with_http_info(self, rename_tracks : Optional[StrictBool] = None, replace_illegal_characters : Optional[StrictBool] = None, standard_track_format : Optional[StrictStr] = None, multi_disc_track_format : Optional[StrictStr] = None, artist_folder_format : Optional[StrictStr] = None, include_artist_name : Optional[StrictBool] = None, include_album_title : Optional[StrictBool] = None, include_quality : Optional[StrictBool] = None, replace_spaces : Optional[StrictBool] = None, separator : Optional[StrictStr] = None, number_style : Optional[StrictStr] = None, id : Optional[StrictInt] = None, resource_name : Optional[StrictStr] = None, **kwargs):  # noqa: E501
+    def get_naming_config_examples_with_http_info(self, rename_tracks : Optional[StrictBool] = None, replace_illegal_characters : Optional[StrictBool] = None, colon_replacement_format : Optional[StrictInt] = None, standard_track_format : Optional[StrictStr] = None, multi_disc_track_format : Optional[StrictStr] = None, artist_folder_format : Optional[StrictStr] = None, include_artist_name : Optional[StrictBool] = None, include_album_title : Optional[StrictBool] = None, include_quality : Optional[StrictBool] = None, replace_spaces : Optional[StrictBool] = None, separator : Optional[StrictStr] = None, number_style : Optional[StrictStr] = None, id : Optional[StrictInt] = None, resource_name : Optional[StrictStr] = None, **kwargs):  # noqa: E501
         """get_naming_config_examples  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_naming_config_examples_with_http_info(rename_tracks, replace_illegal_characters, standard_track_format, multi_disc_track_format, artist_folder_format, include_artist_name, include_album_title, include_quality, replace_spaces, separator, number_style, id, resource_name, async_req=True)
+        >>> thread = api.get_naming_config_examples_with_http_info(rename_tracks, replace_illegal_characters, colon_replacement_format, standard_track_format, multi_disc_track_format, artist_folder_format, include_artist_name, include_album_title, include_quality, replace_spaces, separator, number_style, id, resource_name, async_req=True)
         >>> result = thread.get()
 
         :param rename_tracks:
         :type rename_tracks: bool
         :param replace_illegal_characters:
         :type replace_illegal_characters: bool
+        :param colon_replacement_format:
+        :type colon_replacement_format: int
         :param standard_track_format:
         :type standard_track_format: str
         :param multi_disc_track_format:
         :type multi_disc_track_format: str
         :param artist_folder_format:
         :type artist_folder_format: str
         :param include_artist_name:
@@ -432,14 +436,15 @@
         """
 
         _params = locals()
 
         _all_params = [
             'rename_tracks',
             'replace_illegal_characters',
+            'colon_replacement_format',
             'standard_track_format',
             'multi_disc_track_format',
             'artist_folder_format',
             'include_artist_name',
             'include_album_title',
             'include_quality',
             'replace_spaces',
@@ -477,14 +482,16 @@
 
         # process the query parameters
         _query_params = []
         if _params.get('rename_tracks') is not None:  # noqa: E501
             _query_params.append(('RenameTracks', _params['rename_tracks']))
         if _params.get('replace_illegal_characters') is not None:  # noqa: E501
             _query_params.append(('ReplaceIllegalCharacters', _params['replace_illegal_characters']))
+        if _params.get('colon_replacement_format') is not None:  # noqa: E501
+            _query_params.append(('ColonReplacementFormat', _params['colon_replacement_format']))
         if _params.get('standard_track_format') is not None:  # noqa: E501
             _query_params.append(('StandardTrackFormat', _params['standard_track_format']))
         if _params.get('multi_disc_track_format') is not None:  # noqa: E501
             _query_params.append(('MultiDiscTrackFormat', _params['multi_disc_track_format']))
         if _params.get('artist_folder_format') is not None:  # noqa: E501
             _query_params.append(('ArtistFolderFormat', _params['artist_folder_format']))
         if _params.get('include_artist_name') is not None:  # noqa: E501
```

### Comparing `lidarr-py-0.2.2/lidarr/api/notification_api.py` & `lidarr-py-0.3.0/lidarr/api/notification_api.py`

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
 
 from lidarr.models.notification_resource import NotificationResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
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

### Comparing `lidarr-py-0.2.2/lidarr/api/parse_api.py` & `lidarr-py-0.3.0/lidarr/api/parse_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/ping_api.py` & `lidarr-py-0.3.0/lidarr/api/ping_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/quality_definition_api.py` & `lidarr-py-0.3.0/lidarr/api/quality_definition_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/quality_profile_api.py` & `lidarr-py-0.3.0/lidarr/api/quality_profile_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/quality_profile_schema_api.py` & `lidarr-py-0.3.0/lidarr/api/quality_profile_schema_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/queue_action_api.py` & `lidarr-py-0.3.0/lidarr/api/queue_action_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/queue_api.py` & `lidarr-py-0.3.0/lidarr/api/queue_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/queue_details_api.py` & `lidarr-py-0.3.0/lidarr/api/queue_details_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/queue_status_api.py` & `lidarr-py-0.3.0/lidarr/api/queue_status_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/release_api.py` & `lidarr-py-0.3.0/lidarr/api/release_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/release_profile_api.py` & `lidarr-py-0.3.0/lidarr/api/release_profile_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/release_push_api.py` & `lidarr-py-0.3.0/lidarr/api/release_push_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/remote_path_mapping_api.py` & `lidarr-py-0.3.0/lidarr/api/remote_path_mapping_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/rename_track_api.py` & `lidarr-py-0.3.0/lidarr/api/rename_track_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/retag_track_api.py` & `lidarr-py-0.3.0/lidarr/api/retag_track_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/root_folder_api.py` & `lidarr-py-0.3.0/lidarr/api/root_folder_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/search_api.py` & `lidarr-py-0.3.0/lidarr/api/search_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/static_resource_api.py` & `lidarr-py-0.3.0/lidarr/api/static_resource_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/system_api.py` & `lidarr-py-0.3.0/lidarr/api/system_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/tag_api.py` & `lidarr-py-0.3.0/lidarr/api/tag_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/tag_details_api.py` & `lidarr-py-0.3.0/lidarr/api/tag_details_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/task_api.py` & `lidarr-py-0.3.0/lidarr/api/task_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/track_api.py` & `lidarr-py-0.3.0/lidarr/api/track_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/track_file_api.py` & `lidarr-py-0.3.0/lidarr/api/track_file_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/ui_config_api.py` & `lidarr-py-0.3.0/lidarr/api/ui_config_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/update_api.py` & `lidarr-py-0.3.0/lidarr/api/update_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api/update_log_file_api.py` & `lidarr-py-0.3.0/lidarr/api/update_log_file_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/api_client.py` & `lidarr-py-0.3.0/lidarr/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
         # x-release-please-start-version
-        self.user_agent = 'lidarr-py/v0.2.2'
+        self.user_agent = 'lidarr-py/v0.3.0'
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

### Comparing `lidarr-py-0.2.2/lidarr/configuration.py` & `lidarr-py-0.3.0/lidarr/configuration.py`

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
         self._base_path = "http://localhost:8686" if host is None else host
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
         self.logger["package_logger"] = logging.getLogger("lidarr")
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
                "Version of the API: 1.0.0\n"\
                "SDK Package Version: {sdkversion}".\
                format(env=sys.platform, pyversion=sys.version, sdkversion=sdkversion)
```

### Comparing `lidarr-py-0.2.2/lidarr/exceptions.py` & `lidarr-py-0.3.0/lidarr/exceptions.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/__init__.py` & `lidarr-py-0.3.0/lidarr/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 from lidarr.models.blocklist_bulk_resource import BlocklistBulkResource
 from lidarr.models.blocklist_resource import BlocklistResource
 from lidarr.models.blocklist_resource_paging_resource import BlocklistResourcePagingResource
 from lidarr.models.certificate_validation_type import CertificateValidationType
 from lidarr.models.command import Command
 from lidarr.models.command_priority import CommandPriority
 from lidarr.models.command_resource import CommandResource
+from lidarr.models.command_result import CommandResult
 from lidarr.models.command_status import CommandStatus
 from lidarr.models.command_trigger import CommandTrigger
 from lidarr.models.custom_filter_resource import CustomFilterResource
 from lidarr.models.custom_format import CustomFormat
 from lidarr.models.custom_format_resource import CustomFormatResource
 from lidarr.models.custom_format_specification_schema import CustomFormatSpecificationSchema
 from lidarr.models.database_type import DatabaseType
```

### Comparing `lidarr-py-0.2.2/lidarr/models/add_album_options.py` & `lidarr-py-0.3.0/lidarr/models/add_album_options.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/add_artist_options.py` & `lidarr-py-0.3.0/lidarr/models/add_artist_options.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/album.py` & `lidarr-py-0.3.0/lidarr/models/album.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/album_add_type.py` & `lidarr-py-0.3.0/lidarr/models/album_add_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/album_lazy_loaded.py` & `lidarr-py-0.3.0/lidarr/models/album_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/album_list_lazy_loaded.py` & `lidarr-py-0.3.0/lidarr/models/album_list_lazy_loaded.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel
-from lidarr.models.album import Album
 
 class AlbumListLazyLoaded(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
```

### Comparing `lidarr-py-0.2.2/lidarr/models/album_release.py` & `lidarr-py-0.3.0/lidarr/models/album_release.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/album_release_lazy_loaded.py` & `lidarr-py-0.3.0/lidarr/models/album_release_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/album_release_list_lazy_loaded.py` & `lidarr-py-0.3.0/lidarr/models/album_release_list_lazy_loaded.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel
-from lidarr.models.album_release import AlbumRelease
 
 class AlbumReleaseListLazyLoaded(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
```

### Comparing `lidarr-py-0.2.2/lidarr/models/album_release_resource.py` & `lidarr-py-0.3.0/lidarr/models/album_release_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/album_resource.py` & `lidarr-py-0.3.0/lidarr/models/album_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/album_resource_paging_resource.py` & `lidarr-py-0.3.0/lidarr/models/album_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/album_statistics_resource.py` & `lidarr-py-0.3.0/lidarr/models/album_statistics_resource.py`

 * *Files 3% similar despite different names*

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
 
 class AlbumStatisticsResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `lidarr-py-0.2.2/lidarr/models/album_studio_artist_resource.py` & `lidarr-py-0.3.0/lidarr/models/album_studio_artist_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/album_studio_resource.py` & `lidarr-py-0.3.0/lidarr/models/album_studio_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/albums_monitored_resource.py` & `lidarr-py-0.3.0/lidarr/models/albums_monitored_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/allow_fingerprinting.py` & `lidarr-py-0.3.0/lidarr/models/allow_fingerprinting.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/apply_tags.py` & `lidarr-py-0.3.0/lidarr/models/apply_tags.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/artist.py` & `lidarr-py-0.3.0/lidarr/models/artist.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/artist_editor_resource.py` & `lidarr-py-0.3.0/lidarr/models/artist_editor_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/artist_lazy_loaded.py` & `lidarr-py-0.3.0/lidarr/models/artist_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/artist_metadata.py` & `lidarr-py-0.3.0/lidarr/models/artist_metadata.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/artist_metadata_lazy_loaded.py` & `lidarr-py-0.3.0/lidarr/models/artist_metadata_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/artist_resource.py` & `lidarr-py-0.3.0/lidarr/models/artist_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/artist_statistics_resource.py` & `lidarr-py-0.3.0/lidarr/models/artist_statistics_resource.py`

 * *Files 4% similar despite different names*

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
 
 class ArtistStatisticsResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `lidarr-py-0.2.2/lidarr/models/artist_status_type.py` & `lidarr-py-0.3.0/lidarr/models/artist_status_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/artist_title_info.py` & `lidarr-py-0.3.0/lidarr/models/artist_title_info.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/authentication_type.py` & `lidarr-py-0.3.0/lidarr/models/authentication_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/backup_resource.py` & `lidarr-py-0.3.0/lidarr/models/backup_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/backup_type.py` & `lidarr-py-0.3.0/lidarr/models/backup_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/blocklist_bulk_resource.py` & `lidarr-py-0.3.0/lidarr/models/blocklist_bulk_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/blocklist_resource.py` & `lidarr-py-0.3.0/lidarr/models/blocklist_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/blocklist_resource_paging_resource.py` & `lidarr-py-0.3.0/lidarr/models/blocklist_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/certificate_validation_type.py` & `lidarr-py-0.3.0/lidarr/models/certificate_validation_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/command.py` & `lidarr-py-0.3.0/lidarr/models/command.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/command_priority.py` & `lidarr-py-0.3.0/lidarr/models/command_priority.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/command_resource.py` & `lidarr-py-0.3.0/lidarr/models/command_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel
 from lidarr.models.command import Command
 from lidarr.models.command_priority import CommandPriority
+from lidarr.models.command_result import CommandResult
 from lidarr.models.command_status import CommandStatus
 from lidarr.models.command_trigger import CommandTrigger
 
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

### Comparing `lidarr-py-0.2.2/lidarr/models/command_status.py` & `lidarr-py-0.3.0/lidarr/models/command_status.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/command_trigger.py` & `lidarr-py-0.3.0/lidarr/models/command_trigger.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/custom_filter_resource.py` & `lidarr-py-0.3.0/lidarr/models/custom_filter_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/custom_format.py` & `lidarr-py-0.3.0/lidarr/models/custom_format.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/custom_format_resource.py` & `lidarr-py-0.3.0/lidarr/models/custom_format_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/custom_format_specification_schema.py` & `lidarr-py-0.3.0/lidarr/models/custom_format_specification_schema.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/database_type.py` & `lidarr-py-0.3.0/lidarr/models/database_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/delay_profile_resource.py` & `lidarr-py-0.3.0/lidarr/models/delay_profile_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/disk_space_resource.py` & `lidarr-py-0.3.0/lidarr/models/disk_space_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/download_client_config_resource.py` & `lidarr-py-0.3.0/lidarr/models/download_client_config_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/download_client_resource.py` & `lidarr-py-0.3.0/lidarr/models/download_client_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/download_protocol.py` & `lidarr-py-0.3.0/lidarr/models/download_protocol.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/entity_history_event_type.py` & `lidarr-py-0.3.0/lidarr/models/entity_history_event_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/field.py` & `lidarr-py-0.3.0/lidarr/models/field.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,16 @@
     value: Optional[object]
     type: Optional[str]
     advanced: Optional[bool]
     select_options: Optional[List]
     select_options_provider_action: Optional[str]
     section: Optional[str]
     hidden: Optional[str]
-    __properties = ["order", "name", "label", "unit", "helpText", "helpLink", "value", "type", "advanced", "selectOptions", "selectOptionsProviderAction", "section", "hidden"]
+    placeholder: Optional[str]
+    __properties = ["order", "name", "label", "unit", "helpText", "helpLink", "value", "type", "advanced", "selectOptions", "selectOptionsProviderAction", "section", "hidden", "placeholder"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -116,14 +117,18 @@
         if self.section is None:
             _dict['section'] = None
 
         # set to None if hidden (nullable) is None
         if self.hidden is None:
             _dict['hidden'] = None
 
+        # set to None if placeholder (nullable) is None
+        if self.placeholder is None:
+            _dict['placeholder'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Field:
         """Create an instance of Field from a dict"""
         if obj is None:
             return None
@@ -140,11 +145,12 @@
             "help_link": obj.get("helpLink"),
             "value": obj.get("value"),
             "type": obj.get("type"),
             "advanced": obj.get("advanced"),
             "select_options": [SelectOption.from_dict(_item) for _item in obj.get("selectOptions")] if obj.get("selectOptions") is not None else None,
             "select_options_provider_action": obj.get("selectOptionsProviderAction"),
             "section": obj.get("section"),
-            "hidden": obj.get("hidden")
+            "hidden": obj.get("hidden"),
+            "placeholder": obj.get("placeholder")
         })
         return _obj
```

### Comparing `lidarr-py-0.2.2/lidarr/models/file_date_type.py` & `lidarr-py-0.3.0/lidarr/models/file_date_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/health_check_result.py` & `lidarr-py-0.3.0/lidarr/models/health_check_result.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/health_resource.py` & `lidarr-py-0.3.0/lidarr/models/health_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/history_resource.py` & `lidarr-py-0.3.0/lidarr/models/history_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/history_resource_paging_resource.py` & `lidarr-py-0.3.0/lidarr/models/history_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/host_config_resource.py` & `lidarr-py-0.3.0/lidarr/models/host_config_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/i_custom_format_specification.py` & `lidarr-py-0.3.0/lidarr/models/i_custom_format_specification.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/import_list_exclusion_resource.py` & `lidarr-py-0.3.0/lidarr/models/import_list_exclusion_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/import_list_monitor_type.py` & `lidarr-py-0.3.0/lidarr/models/import_list_monitor_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/import_list_resource.py` & `lidarr-py-0.3.0/lidarr/models/import_list_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/import_list_type.py` & `lidarr-py-0.3.0/lidarr/models/import_list_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/indexer_config_resource.py` & `lidarr-py-0.3.0/lidarr/models/indexer_config_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/indexer_resource.py` & `lidarr-py-0.3.0/lidarr/models/indexer_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/iso_country.py` & `lidarr-py-0.3.0/lidarr/models/iso_country.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/language_resource.py` & `lidarr-py-0.3.0/lidarr/models/language_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/links.py` & `lidarr-py-0.3.0/lidarr/models/links.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/log_file_resource.py` & `lidarr-py-0.3.0/lidarr/models/log_file_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/log_resource.py` & `lidarr-py-0.3.0/lidarr/models/log_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/log_resource_paging_resource.py` & `lidarr-py-0.3.0/lidarr/models/log_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/manual_import_resource.py` & `lidarr-py-0.3.0/lidarr/models/manual_import_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/manual_import_update_resource.py` & `lidarr-py-0.3.0/lidarr/models/manual_import_update_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/media_cover.py` & `lidarr-py-0.3.0/lidarr/models/media_cover.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/media_cover_types.py` & `lidarr-py-0.3.0/lidarr/models/media_cover_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,8 +35,9 @@
     BANNER = 'banner'
     FANART = 'fanart'
     SCREENSHOT = 'screenshot'
     HEADSHOT = 'headshot'
     COVER = 'cover'
     DISC = 'disc'
     LOGO = 'logo'
+    CLEARLOGO = 'clearlogo'
```

### Comparing `lidarr-py-0.2.2/lidarr/models/media_info_model.py` & `lidarr-py-0.3.0/lidarr/models/media_info_model.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/media_info_resource.py` & `lidarr-py-0.3.0/lidarr/models/media_info_resource.py`

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

### Comparing `lidarr-py-0.2.2/lidarr/models/media_management_config_resource.py` & `lidarr-py-0.3.0/lidarr/models/media_management_config_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/medium.py` & `lidarr-py-0.3.0/lidarr/models/medium.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/medium_resource.py` & `lidarr-py-0.3.0/lidarr/models/medium_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/member.py` & `lidarr-py-0.3.0/lidarr/models/member.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/metadata_profile.py` & `lidarr-py-0.3.0/lidarr/models/metadata_profile.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/metadata_profile_lazy_loaded.py` & `lidarr-py-0.3.0/lidarr/models/metadata_profile_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/metadata_profile_resource.py` & `lidarr-py-0.3.0/lidarr/models/metadata_profile_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/metadata_provider_config_resource.py` & `lidarr-py-0.3.0/lidarr/models/metadata_provider_config_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/metadata_resource.py` & `lidarr-py-0.3.0/lidarr/models/metadata_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/monitor_types.py` & `lidarr-py-0.3.0/lidarr/models/monitor_types.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/monitoring_options.py` & `lidarr-py-0.3.0/lidarr/models/monitoring_options.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/naming_config_resource.py` & `lidarr-py-0.3.0/lidarr/models/naming_config_resource.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,24 +25,25 @@
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     id: Optional[int]
     rename_tracks: Optional[bool]
     replace_illegal_characters: Optional[bool]
+    colon_replacement_format: Optional[int]
     standard_track_format: Optional[str]
     multi_disc_track_format: Optional[str]
     artist_folder_format: Optional[str]
     include_artist_name: Optional[bool]
     include_album_title: Optional[bool]
     include_quality: Optional[bool]
     replace_spaces: Optional[bool]
     separator: Optional[str]
     number_style: Optional[str]
-    __properties = ["id", "renameTracks", "replaceIllegalCharacters", "standardTrackFormat", "multiDiscTrackFormat", "artistFolderFormat", "includeArtistName", "includeAlbumTitle", "includeQuality", "replaceSpaces", "separator", "numberStyle"]
+    __properties = ["id", "renameTracks", "replaceIllegalCharacters", "colonReplacementFormat", "standardTrackFormat", "multiDiscTrackFormat", "artistFolderFormat", "includeArtistName", "includeAlbumTitle", "includeQuality", "replaceSpaces", "separator", "numberStyle"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -98,14 +99,15 @@
         if type(obj) is not dict:
             return NamingConfigResource.parse_obj(obj)
 
         _obj = NamingConfigResource.parse_obj({
             "id": obj.get("id"),
             "rename_tracks": obj.get("renameTracks"),
             "replace_illegal_characters": obj.get("replaceIllegalCharacters"),
+            "colon_replacement_format": obj.get("colonReplacementFormat"),
             "standard_track_format": obj.get("standardTrackFormat"),
             "multi_disc_track_format": obj.get("multiDiscTrackFormat"),
             "artist_folder_format": obj.get("artistFolderFormat"),
             "include_artist_name": obj.get("includeArtistName"),
             "include_album_title": obj.get("includeAlbumTitle"),
             "include_quality": obj.get("includeQuality"),
             "replace_spaces": obj.get("replaceSpaces"),
```

### Comparing `lidarr-py-0.2.2/lidarr/models/new_item_monitor_types.py` & `lidarr-py-0.3.0/lidarr/models/new_item_monitor_types.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/notification_resource.py` & `lidarr-py-0.3.0/lidarr/models/notification_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,32 +42,34 @@
     on_grab: Optional[bool]
     on_release_import: Optional[bool]
     on_upgrade: Optional[bool]
     on_rename: Optional[bool]
     on_album_delete: Optional[bool]
     on_artist_delete: Optional[bool]
     on_health_issue: Optional[bool]
+    on_health_restored: Optional[bool]
     on_download_failure: Optional[bool]
     on_import_failure: Optional[bool]
     on_track_retag: Optional[bool]
     on_application_update: Optional[bool]
     supports_on_grab: Optional[bool]
     supports_on_release_import: Optional[bool]
     supports_on_upgrade: Optional[bool]
     supports_on_rename: Optional[bool]
     supports_on_album_delete: Optional[bool]
     supports_on_artist_delete: Optional[bool]
     supports_on_health_issue: Optional[bool]
+    supports_on_health_restored: Optional[bool]
     include_health_warnings: Optional[bool]
     supports_on_download_failure: Optional[bool]
     supports_on_import_failure: Optional[bool]
     supports_on_track_retag: Optional[bool]
     supports_on_application_update: Optional[bool]
     test_command: Optional[str]
-    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "link", "onGrab", "onReleaseImport", "onUpgrade", "onRename", "onAlbumDelete", "onArtistDelete", "onHealthIssue", "onDownloadFailure", "onImportFailure", "onTrackRetag", "onApplicationUpdate", "supportsOnGrab", "supportsOnReleaseImport", "supportsOnUpgrade", "supportsOnRename", "supportsOnAlbumDelete", "supportsOnArtistDelete", "supportsOnHealthIssue", "includeHealthWarnings", "supportsOnDownloadFailure", "supportsOnImportFailure", "supportsOnTrackRetag", "supportsOnApplicationUpdate", "testCommand"]
+    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "link", "onGrab", "onReleaseImport", "onUpgrade", "onRename", "onAlbumDelete", "onArtistDelete", "onHealthIssue", "onHealthRestored", "onDownloadFailure", "onImportFailure", "onTrackRetag", "onApplicationUpdate", "supportsOnGrab", "supportsOnReleaseImport", "supportsOnUpgrade", "supportsOnRename", "supportsOnAlbumDelete", "supportsOnArtistDelete", "supportsOnHealthIssue", "supportsOnHealthRestored", "includeHealthWarnings", "supportsOnDownloadFailure", "supportsOnImportFailure", "supportsOnTrackRetag", "supportsOnApplicationUpdate", "testCommand"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -175,25 +177,27 @@
             "on_grab": obj.get("onGrab"),
             "on_release_import": obj.get("onReleaseImport"),
             "on_upgrade": obj.get("onUpgrade"),
             "on_rename": obj.get("onRename"),
             "on_album_delete": obj.get("onAlbumDelete"),
             "on_artist_delete": obj.get("onArtistDelete"),
             "on_health_issue": obj.get("onHealthIssue"),
+            "on_health_restored": obj.get("onHealthRestored"),
             "on_download_failure": obj.get("onDownloadFailure"),
             "on_import_failure": obj.get("onImportFailure"),
             "on_track_retag": obj.get("onTrackRetag"),
             "on_application_update": obj.get("onApplicationUpdate"),
             "supports_on_grab": obj.get("supportsOnGrab"),
             "supports_on_release_import": obj.get("supportsOnReleaseImport"),
             "supports_on_upgrade": obj.get("supportsOnUpgrade"),
             "supports_on_rename": obj.get("supportsOnRename"),
             "supports_on_album_delete": obj.get("supportsOnAlbumDelete"),
             "supports_on_artist_delete": obj.get("supportsOnArtistDelete"),
             "supports_on_health_issue": obj.get("supportsOnHealthIssue"),
+            "supports_on_health_restored": obj.get("supportsOnHealthRestored"),
             "include_health_warnings": obj.get("includeHealthWarnings"),
             "supports_on_download_failure": obj.get("supportsOnDownloadFailure"),
             "supports_on_import_failure": obj.get("supportsOnImportFailure"),
             "supports_on_track_retag": obj.get("supportsOnTrackRetag"),
             "supports_on_application_update": obj.get("supportsOnApplicationUpdate"),
             "test_command": obj.get("testCommand")
         })
```

### Comparing `lidarr-py-0.2.2/lidarr/models/paging_resource_filter.py` & `lidarr-py-0.3.0/lidarr/models/paging_resource_filter.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/parse_resource.py` & `lidarr-py-0.3.0/lidarr/models/parse_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/parsed_album_info.py` & `lidarr-py-0.3.0/lidarr/models/parsed_album_info.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/parsed_track_info.py` & `lidarr-py-0.3.0/lidarr/models/parsed_track_info.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/ping_resource.py` & `lidarr-py-0.3.0/lidarr/models/ping_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/primary_album_type.py` & `lidarr-py-0.3.0/lidarr/models/primary_album_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/profile_format_item.py` & `lidarr-py-0.3.0/lidarr/models/profile_format_item.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/profile_format_item_resource.py` & `lidarr-py-0.3.0/lidarr/models/profile_format_item_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/profile_primary_album_type_item.py` & `lidarr-py-0.3.0/lidarr/models/profile_primary_album_type_item.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/profile_primary_album_type_item_resource.py` & `lidarr-py-0.3.0/lidarr/models/profile_primary_album_type_item_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/profile_release_status_item.py` & `lidarr-py-0.3.0/lidarr/models/profile_release_status_item.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/profile_release_status_item_resource.py` & `lidarr-py-0.3.0/lidarr/models/profile_release_status_item_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/profile_secondary_album_type_item.py` & `lidarr-py-0.3.0/lidarr/models/profile_secondary_album_type_item.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/profile_secondary_album_type_item_resource.py` & `lidarr-py-0.3.0/lidarr/models/profile_secondary_album_type_item_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/proper_download_types.py` & `lidarr-py-0.3.0/lidarr/models/proper_download_types.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/provider_message.py` & `lidarr-py-0.3.0/lidarr/models/provider_message.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/provider_message_type.py` & `lidarr-py-0.3.0/lidarr/models/provider_message_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/proxy_type.py` & `lidarr-py-0.3.0/lidarr/models/proxy_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/quality.py` & `lidarr-py-0.3.0/lidarr/models/quality.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/quality_definition_resource.py` & `lidarr-py-0.3.0/lidarr/models/quality_definition_resource.py`

 * *Files 2% similar despite different names*

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
 from lidarr.models.quality import Quality
 
 class QualityDefinitionResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `lidarr-py-0.2.2/lidarr/models/quality_model.py` & `lidarr-py-0.3.0/lidarr/models/quality_model.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/quality_profile.py` & `lidarr-py-0.3.0/lidarr/models/quality_profile.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/quality_profile_lazy_loaded.py` & `lidarr-py-0.3.0/lidarr/models/quality_profile_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/quality_profile_quality_item.py` & `lidarr-py-0.3.0/lidarr/models/quality_profile_quality_item.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/quality_profile_quality_item_resource.py` & `lidarr-py-0.3.0/lidarr/models/quality_profile_quality_item_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/quality_profile_resource.py` & `lidarr-py-0.3.0/lidarr/models/quality_profile_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/queue_bulk_resource.py` & `lidarr-py-0.3.0/lidarr/models/queue_bulk_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/queue_resource.py` & `lidarr-py-0.3.0/lidarr/models/queue_resource.py`

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
 from lidarr.models.album_resource import AlbumResource
 from lidarr.models.artist_resource import ArtistResource
 from lidarr.models.custom_format_resource import CustomFormatResource
 from lidarr.models.download_protocol import DownloadProtocol
 from lidarr.models.quality_model import QualityModel
 from lidarr.models.tracked_download_state import TrackedDownloadState
```

### Comparing `lidarr-py-0.2.2/lidarr/models/queue_resource_paging_resource.py` & `lidarr-py-0.3.0/lidarr/models/queue_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/queue_status_resource.py` & `lidarr-py-0.3.0/lidarr/models/queue_status_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/ratings.py` & `lidarr-py-0.3.0/lidarr/models/ratings.py`

 * *Files 4% similar despite different names*

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
 
 class Ratings(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `lidarr-py-0.2.2/lidarr/models/rejection.py` & `lidarr-py-0.3.0/lidarr/models/rejection.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/rejection_type.py` & `lidarr-py-0.3.0/lidarr/models/rejection_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/release_profile_resource.py` & `lidarr-py-0.3.0/lidarr/models/release_profile_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/release_resource.py` & `lidarr-py-0.3.0/lidarr/models/release_resource.py`

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
 from lidarr.models.custom_format_resource import CustomFormatResource
 from lidarr.models.download_protocol import DownloadProtocol
 from lidarr.models.quality_model import QualityModel
 
 class ReleaseResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `lidarr-py-0.2.2/lidarr/models/release_status.py` & `lidarr-py-0.3.0/lidarr/models/release_status.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/remote_path_mapping_resource.py` & `lidarr-py-0.3.0/lidarr/models/remote_path_mapping_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/rename_track_resource.py` & `lidarr-py-0.3.0/lidarr/models/rename_track_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/rescan_after_refresh_type.py` & `lidarr-py-0.3.0/lidarr/models/rescan_after_refresh_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/retag_track_resource.py` & `lidarr-py-0.3.0/lidarr/models/retag_track_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/revision.py` & `lidarr-py-0.3.0/lidarr/models/revision.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/root_folder_resource.py` & `lidarr-py-0.3.0/lidarr/models/root_folder_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/runtime_mode.py` & `lidarr-py-0.3.0/lidarr/models/runtime_mode.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/secondary_album_type.py` & `lidarr-py-0.3.0/lidarr/models/secondary_album_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/select_option.py` & `lidarr-py-0.3.0/lidarr/models/select_option.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/sort_direction.py` & `lidarr-py-0.3.0/lidarr/models/sort_direction.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/system_resource.py` & `lidarr-py-0.3.0/lidarr/models/system_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/tag_details_resource.py` & `lidarr-py-0.3.0/lidarr/models/tag_details_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/tag_difference.py` & `lidarr-py-0.3.0/lidarr/models/tag_difference.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/tag_resource.py` & `lidarr-py-0.3.0/lidarr/models/tag_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/task_resource.py` & `lidarr-py-0.3.0/lidarr/models/task_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/track.py` & `lidarr-py-0.3.0/lidarr/models/track.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/track_file.py` & `lidarr-py-0.3.0/lidarr/models/track_file.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/track_file_lazy_loaded.py` & `lidarr-py-0.3.0/lidarr/models/track_file_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/track_file_list_resource.py` & `lidarr-py-0.3.0/lidarr/models/track_file_list_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/track_file_resource.py` & `lidarr-py-0.3.0/lidarr/models/track_file_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/track_list_lazy_loaded.py` & `lidarr-py-0.3.0/lidarr/models/track_list_lazy_loaded.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel
-from lidarr.models.track import Track
 
 class TrackListLazyLoaded(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
```

### Comparing `lidarr-py-0.2.2/lidarr/models/track_resource.py` & `lidarr-py-0.3.0/lidarr/models/track_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/tracked_download_state.py` & `lidarr-py-0.3.0/lidarr/models/tracked_download_state.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/tracked_download_status.py` & `lidarr-py-0.3.0/lidarr/models/tracked_download_status.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/tracked_download_status_message.py` & `lidarr-py-0.3.0/lidarr/models/tracked_download_status_message.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/ui_config_resource.py` & `lidarr-py-0.3.0/lidarr/models/ui_config_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/update_changes.py` & `lidarr-py-0.3.0/lidarr/models/update_changes.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/update_mechanism.py` & `lidarr-py-0.3.0/lidarr/models/update_mechanism.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/update_resource.py` & `lidarr-py-0.3.0/lidarr/models/update_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/models/write_audio_tags_type.py` & `lidarr-py-0.3.0/lidarr/models/write_audio_tags_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr/rest.py` & `lidarr-py-0.3.0/lidarr/rest.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.2.2/lidarr_py.egg-info/PKG-INFO` & `lidarr-py-0.3.0/lidarr_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lidarr-py
-Version: 0.2.2
+Version: 0.3.0
 Summary: Lidarr API wrapper
 Project-URL: Homepage, https://github.com/devopsarr/lidarr-py
 Project-URL: Bug Tracker, https://github.com/devopsarr/lidarr-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 
 # lidarr-py
 Lidarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.2.2
+- Package version: 0.3.0
 
 [comment]: # (x-release-please-end)
 - API version: 1.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -378,14 +378,15 @@
  - [BlocklistBulkResource](docs/BlocklistBulkResource.md)
  - [BlocklistResource](docs/BlocklistResource.md)
  - [BlocklistResourcePagingResource](docs/BlocklistResourcePagingResource.md)
  - [CertificateValidationType](docs/CertificateValidationType.md)
  - [Command](docs/Command.md)
  - [CommandPriority](docs/CommandPriority.md)
  - [CommandResource](docs/CommandResource.md)
+ - [CommandResult](docs/CommandResult.md)
  - [CommandStatus](docs/CommandStatus.md)
  - [CommandTrigger](docs/CommandTrigger.md)
  - [CustomFilterResource](docs/CustomFilterResource.md)
  - [CustomFormat](docs/CustomFormat.md)
  - [CustomFormatResource](docs/CustomFormatResource.md)
  - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
  - [DatabaseType](docs/DatabaseType.md)
```

### Comparing `lidarr-py-0.2.2/lidarr_py.egg-info/SOURCES.txt` & `lidarr-py-0.3.0/lidarr_py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 lidarr/__init__.py
 lidarr/api_client.py
+lidarr/api_response.py
 lidarr/configuration.py
 lidarr/exceptions.py
 lidarr/rest.py
 lidarr/api/__init__.py
 lidarr/api/album_api.py
 lidarr/api/album_lookup_api.py
 lidarr/api/album_studio_api.py
@@ -112,14 +113,15 @@
 lidarr/models/blocklist_bulk_resource.py
 lidarr/models/blocklist_resource.py
 lidarr/models/blocklist_resource_paging_resource.py
 lidarr/models/certificate_validation_type.py
 lidarr/models/command.py
 lidarr/models/command_priority.py
 lidarr/models/command_resource.py
+lidarr/models/command_result.py
 lidarr/models/command_status.py
 lidarr/models/command_trigger.py
 lidarr/models/custom_filter_resource.py
 lidarr/models/custom_format.py
 lidarr/models/custom_format_resource.py
 lidarr/models/custom_format_specification_schema.py
 lidarr/models/database_type.py
```

### Comparing `lidarr-py-0.2.2/pyproject.toml` & `lidarr-py-0.3.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 [project]
 name = "lidarr-py"
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

