# Comparing `tmp/readarr-py-0.2.2.tar.gz` & `tmp/readarr-py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readarr-py-0.2.2.tar", last modified: Mon Mar 27 14:23:13 2023, max compression
+gzip compressed data, was "readarr-py-0.3.0.tar", last modified: Mon May 29 06:41:07 2023, max compression
```

## Comparing `readarr-py-0.2.2.tar` & `readarr-py-0.3.0.tar`

### file list

```diff
@@ -1,230 +1,249 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:23:13.089244 readarr-py-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-03-27 14:22:59.000000 readarr-py-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    37877 2023-03-27 14:23:13.089244 readarr-py-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37401 2023-03-27 14:22:59.000000 readarr-py-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-27 14:22:59.000000 readarr-py-0.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:23:13.041241 readarr-py-0.2.2/readarr/
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:23:13.057242 readarr-py-0.2.2/readarr/api/
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12650 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/authentication_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29705 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/author_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/author_editor_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/author_lookup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22403 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/backup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17781 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/blacklist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37389 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/book_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37557 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/book_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/book_lookup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/bookshelf_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13478 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/calendar_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/calendar_feed_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23392 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/command_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30346 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/custom_filter_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/cutoff_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36133 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/delay_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18930 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/development_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/disk_space_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53670 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/download_client_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19141 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/download_client_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18345 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/file_system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/health_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27700 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/history_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18524 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/host_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52998 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/import_list_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    31083 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/import_list_exclusion_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52373 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/indexer_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18698 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/indexer_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/initialize_js_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/language_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/localization_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/log_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14628 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/manual_import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/media_cover_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19199 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/media_management_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52541 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30634 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/metadata_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/metadata_profile_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/metadata_provider_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/missing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29331 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/naming_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53213 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/notification_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/parse_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25149 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/quality_definition_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30538 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/quality_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/quality_profile_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12251 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/queue_action_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27470 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/queue_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/queue_details_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12007 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/queue_status_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18827 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/release_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30538 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/release_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12804 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/release_push_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30891 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/remote_path_mapping_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/rename_book_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/retag_book_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30154 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/root_folder_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/series_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21693 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/static_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26373 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29417 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/tag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12017 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/tag_details_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/task_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/ui_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/update_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api/update_log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29533 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16302 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:23:13.089244 readarr-py-0.2.2/readarr/models/
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/add_author_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/add_book_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/allow_fingerprinting.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/apply_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/authentication_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/author.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/author_editor_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/author_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/author_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/author_metadata_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     9257 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/author_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/author_statistics_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/author_status_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/author_title_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/backup_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/backup_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/blacklist_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/blacklist_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/blacklist_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/book.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/book_add_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/book_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/book_file_list_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/book_file_list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/book_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/book_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/book_list_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/book_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/book_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/book_statistics_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/books_monitored_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/bookshelf_author_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/bookshelf_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/certificate_validation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/command_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/command_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/command_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/command_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/custom_filter_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/delay_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/development_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/disk_space_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/download_client_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/download_client_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/download_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/edition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/edition_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/edition_list_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/edition_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/field.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/file_date_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/health_check_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/health_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/history_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/history_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/history_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/host_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/import_list_exclusion_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/import_list_monitor_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/import_list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/import_list_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/indexer_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/indexer_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/iso_country.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/language_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/log_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/log_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/log_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/manual_import_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/media_cover.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/media_cover_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/media_info_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/media_info_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/media_management_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/metadata_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/metadata_profile_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/metadata_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/metadata_provider_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/metadata_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/monitor_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/monitoring_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/naming_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/notification_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/paging_resource_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/parse_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/parsed_book_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/parsed_track_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/proper_download_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/provider_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/provider_message_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/proxy_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/quality_definition_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/quality_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/quality_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/quality_profile_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/quality_profile_quality_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/quality_profile_quality_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/quality_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/queue_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/queue_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/queue_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/queue_status_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/ratings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/rejection.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/rejection_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/release_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/release_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/remote_path_mapping_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/rename_book_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/rescan_after_refresh_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/retag_book_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/root_folder_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/select_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/series_book_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/series_book_link_list_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/series_book_link_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/series_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/series_list_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/series_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/string_int32_key_value_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/tag_details_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/tag_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/tag_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/task_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/tracked_download_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/tracked_download_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/tracked_download_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/ui_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/update_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/update_mechanism.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/update_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/write_audio_tags_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/models/write_book_tags_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-03-27 14:22:59.000000 readarr-py-0.2.2/readarr/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:23:13.089244 readarr-py-0.2.2/readarr_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37877 2023-03-27 14:23:13.000000 readarr-py-0.2.2/readarr_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-03-27 14:23:13.000000 readarr-py-0.2.2/readarr_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 14:23:13.000000 readarr-py-0.2.2/readarr_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-27 14:23:13.000000 readarr-py-0.2.2/readarr_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-27 14:23:13.000000 readarr-py-0.2.2/readarr_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 14:23:13.089244 readarr-py-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-27 14:22:59.000000 readarr-py-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:07.296209 readarr-py-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-29 06:40:53.000000 readarr-py-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    40629 2023-05-29 06:41:07.296209 readarr-py-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40153 2023-05-29 06:40:53.000000 readarr-py-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-29 06:40:53.000000 readarr-py-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:07.244208 readarr-py-0.3.0/readarr/
+-rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:07.272209 readarr-py-0.3.0/readarr/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/api_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/authentication_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29810 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/author_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/author_editor_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/author_lookup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22487 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/backup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17844 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/blocklist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42877 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/book_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/book_editor_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37683 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/book_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/book_lookup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/bookshelf_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/calendar_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/calendar_feed_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23476 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/command_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30451 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/custom_filter_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35519 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/custom_format_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/cutoff_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36259 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/delay_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18993 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/development_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/disk_space_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53859 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/download_client_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19204 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/download_client_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/edition_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/file_system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/health_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27532 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/history_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/host_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53187 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/import_list_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31188 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/import_list_exclusion_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52562 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/indexer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/indexer_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/initialize_js_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/language_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/localization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/log_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14887 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/manual_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/media_cover_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/media_management_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52730 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30739 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/metadata_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/metadata_profile_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19320 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/metadata_provider_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/missing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29415 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/naming_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53402 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/parse_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/ping_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25233 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/quality_definition_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30643 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/quality_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/quality_profile_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/queue_action_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27554 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/queue_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13796 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/queue_details_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/queue_status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/release_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30643 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/release_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12846 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/release_push_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30996 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/remote_path_mapping_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/rename_book_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/retag_book_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30259 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/root_folder_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/series_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21836 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/static_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26850 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29522 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/tag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/tag_details_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/task_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18471 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/ui_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/update_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/update_log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29647 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:07.296209 readarr-py-0.3.0/readarr/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    10175 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/add_author_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/add_book_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/allow_fingerprinting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/api_info_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/apply_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/authentication_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/author.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/author_editor_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/author_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/author_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/author_metadata_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/author_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/author_statistics_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/author_status_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/author_title_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/backup_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/backup_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/blocklist_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/blocklist_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/blocklist_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book_add_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book_editor_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book_file_list_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book_file_list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book_list_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book_statistics_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/books_monitored_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/bookshelf_author_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/bookshelf_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/certificate_validation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/command_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/command_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/command_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/command_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/custom_filter_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/custom_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/custom_format_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/custom_format_specification_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/database_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/delay_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/development_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/disk_space_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/download_client_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/download_client_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/download_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/edition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/edition_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/edition_list_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/edition_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/entity_history_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/file_date_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/health_check_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/health_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/history_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/history_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/host_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/i_custom_format_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/import_list_exclusion_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/import_list_monitor_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/import_list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/import_list_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/indexer_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/indexer_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/iso_country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/language_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/log_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/log_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/log_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/manual_import_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/manual_import_update_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/media_cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/media_cover_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/media_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/media_info_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/media_management_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/metadata_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/metadata_profile_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/metadata_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/metadata_provider_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/metadata_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/monitor_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/monitoring_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/naming_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/new_item_monitor_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/notification_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/paging_resource_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/parse_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/parsed_book_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/parsed_track_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/ping_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/profile_format_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/profile_format_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/proper_download_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/provider_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/provider_message_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/proxy_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/quality_definition_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/quality_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/quality_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/quality_profile_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/quality_profile_quality_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/quality_profile_quality_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/quality_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/queue_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/queue_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/queue_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/queue_status_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/ratings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/rejection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/rejection_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/release_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/release_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/remote_path_mapping_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/rename_book_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/rescan_after_refresh_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/retag_book_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/root_folder_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/runtime_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/select_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/series_book_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/series_book_link_list_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/series_book_link_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/series_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/series_list_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/series_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/system_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/tag_details_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/tag_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/tag_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/task_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/tracked_download_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/tracked_download_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/tracked_download_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/ui_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/update_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/update_mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/update_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/write_audio_tags_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/write_book_tags_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:07.296209 readarr-py-0.3.0/readarr_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40629 2023-05-29 06:41:07.000000 readarr-py-0.3.0/readarr_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-05-29 06:41:07.000000 readarr-py-0.3.0/readarr_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 06:41:07.000000 readarr-py-0.3.0/readarr_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 06:41:07.000000 readarr-py-0.3.0/readarr_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 06:41:07.000000 readarr-py-0.3.0/readarr_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 06:41:07.296209 readarr-py-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-29 06:40:53.000000 readarr-py-0.3.0/setup.py
```

### Comparing `readarr-py-0.2.2/LICENSE` & `readarr-py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `readarr-py-0.2.2/PKG-INFO` & `readarr-py-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readarr-py
-Version: 0.2.2
+Version: 0.3.0
 Summary: Readarr API wrapper
 Project-URL: Homepage, https://github.com/devopsarr/readarr-py
 Project-URL: Bug Tracker, https://github.com/devopsarr/readarr-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,18 +13,18 @@
 
 # readarr-py
 Readarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.2.2
+- Package version: 0.3.0
 
 [comment]: # (x-release-please-end)
-- API version: 0.1.0
+- API version: 1.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
@@ -65,87 +65,111 @@
 from __future__ import print_function
 
 import time
 import readarr
 from readarr.rest import ApiException
 from pprint import pprint
 
-# Defining the host is optional and defaults to http://localhost
+# Defining the host is optional and defaults to http://localhost:8787
 # See configuration.py for a list of all supported configuration parameters.
 configuration = readarr.Configuration(
-    host = "http://localhost"
+    host = "http://localhost:8787"
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure API key authorization: apikey
+configuration.api_key['apikey'] = os.environ["API_KEY"]
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['apikey'] = 'Bearer'
+
+# Configure API key authorization: X-Api-Key
+configuration.api_key['X-Api-Key'] = os.environ["API_KEY"]
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['X-Api-Key'] = 'Bearer'
 
 
 # Enter a context with an instance of the API client
 with readarr.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = readarr.AuthenticationApi(api_client)
-    return_url = 'return_url_example' # str |  (optional)
-    username = 'username_example' # str |  (optional)
-    password = 'password_example' # str |  (optional)
-    remember_me = 'remember_me_example' # str |  (optional)
+    api_instance = readarr.ApiInfoApi(api_client)
 
     try:
-        api_instance.create_login(return_url=return_url, username=username, password=password, remember_me=remember_me)
+        api_response = api_instance.get_api()
+        print("The response of ApiInfoApi->get_api:\n")
+        pprint(api_response)
     except ApiException as e:
-        print("Exception when calling AuthenticationApi->create_login: %s\n" % e)
+        print("Exception when calling ApiInfoApi->get_api: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
-All URIs are relative to *http://localhost*
+All URIs are relative to *http://localhost:8787*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
+*ApiInfoApi* | [**get_api**](docs/ApiInfoApi.md#get_api) | **GET** /api | 
 *AuthenticationApi* | [**create_login**](docs/AuthenticationApi.md#create_login) | **POST** /login | 
 *AuthenticationApi* | [**get_logout**](docs/AuthenticationApi.md#get_logout) | **GET** /logout | 
 *AuthorApi* | [**create_author**](docs/AuthorApi.md#create_author) | **POST** /api/v1/author | 
 *AuthorApi* | [**delete_author**](docs/AuthorApi.md#delete_author) | **DELETE** /api/v1/author/{id} | 
 *AuthorApi* | [**get_author_by_id**](docs/AuthorApi.md#get_author_by_id) | **GET** /api/v1/author/{id} | 
 *AuthorApi* | [**list_author**](docs/AuthorApi.md#list_author) | **GET** /api/v1/author | 
 *AuthorApi* | [**update_author**](docs/AuthorApi.md#update_author) | **PUT** /api/v1/author/{id} | 
 *AuthorEditorApi* | [**delete_author_editor**](docs/AuthorEditorApi.md#delete_author_editor) | **DELETE** /api/v1/author/editor | 
 *AuthorEditorApi* | [**put_author_editor**](docs/AuthorEditorApi.md#put_author_editor) | **PUT** /api/v1/author/editor | 
 *AuthorLookupApi* | [**get_author_lookup**](docs/AuthorLookupApi.md#get_author_lookup) | **GET** /api/v1/author/lookup | 
 *BackupApi* | [**create_system_backup_restore_by_id**](docs/BackupApi.md#create_system_backup_restore_by_id) | **POST** /api/v1/system/backup/restore/{id} | 
 *BackupApi* | [**create_system_backup_restore_upload**](docs/BackupApi.md#create_system_backup_restore_upload) | **POST** /api/v1/system/backup/restore/upload | 
 *BackupApi* | [**delete_system_backup**](docs/BackupApi.md#delete_system_backup) | **DELETE** /api/v1/system/backup/{id} | 
 *BackupApi* | [**list_system_backup**](docs/BackupApi.md#list_system_backup) | **GET** /api/v1/system/backup | 
-*BlacklistApi* | [**delete_blacklist**](docs/BlacklistApi.md#delete_blacklist) | **DELETE** /api/v1/blacklist/{id} | 
-*BlacklistApi* | [**delete_blacklist_bulk**](docs/BlacklistApi.md#delete_blacklist_bulk) | **DELETE** /api/v1/blacklist/bulk | 
-*BlacklistApi* | [**get_blacklist**](docs/BlacklistApi.md#get_blacklist) | **GET** /api/v1/blacklist | 
+*BlocklistApi* | [**delete_blocklist**](docs/BlocklistApi.md#delete_blocklist) | **DELETE** /api/v1/blocklist/{id} | 
+*BlocklistApi* | [**delete_blocklist_bulk**](docs/BlocklistApi.md#delete_blocklist_bulk) | **DELETE** /api/v1/blocklist/bulk | 
+*BlocklistApi* | [**get_blocklist**](docs/BlocklistApi.md#get_blocklist) | **GET** /api/v1/blocklist | 
 *BookApi* | [**create_book**](docs/BookApi.md#create_book) | **POST** /api/v1/book | 
 *BookApi* | [**delete_book**](docs/BookApi.md#delete_book) | **DELETE** /api/v1/book/{id} | 
 *BookApi* | [**get_book_by_id**](docs/BookApi.md#get_book_by_id) | **GET** /api/v1/book/{id} | 
+*BookApi* | [**get_bookid_overview**](docs/BookApi.md#get_bookid_overview) | **GET** /api/v1/book/{id}/overview | 
 *BookApi* | [**list_book**](docs/BookApi.md#list_book) | **GET** /api/v1/book | 
 *BookApi* | [**put_book_monitor**](docs/BookApi.md#put_book_monitor) | **PUT** /api/v1/book/monitor | 
 *BookApi* | [**update_book**](docs/BookApi.md#update_book) | **PUT** /api/v1/book/{id} | 
+*BookEditorApi* | [**delete_book_editor**](docs/BookEditorApi.md#delete_book_editor) | **DELETE** /api/v1/book/editor | 
+*BookEditorApi* | [**put_book_editor**](docs/BookEditorApi.md#put_book_editor) | **PUT** /api/v1/book/editor | 
 *BookFileApi* | [**delete_book_file**](docs/BookFileApi.md#delete_book_file) | **DELETE** /api/v1/bookfile/{id} | 
 *BookFileApi* | [**delete_book_file_bulk**](docs/BookFileApi.md#delete_book_file_bulk) | **DELETE** /api/v1/bookfile/bulk | 
 *BookFileApi* | [**get_book_file_by_id**](docs/BookFileApi.md#get_book_file_by_id) | **GET** /api/v1/bookfile/{id} | 
 *BookFileApi* | [**list_book_file**](docs/BookFileApi.md#list_book_file) | **GET** /api/v1/bookfile | 
 *BookFileApi* | [**put_book_file_editor**](docs/BookFileApi.md#put_book_file_editor) | **PUT** /api/v1/bookfile/editor | 
 *BookFileApi* | [**update_book_file**](docs/BookFileApi.md#update_book_file) | **PUT** /api/v1/bookfile/{id} | 
 *BookLookupApi* | [**get_book_lookup**](docs/BookLookupApi.md#get_book_lookup) | **GET** /api/v1/book/lookup | 
 *BookshelfApi* | [**create_bookshelf**](docs/BookshelfApi.md#create_bookshelf) | **POST** /api/v1/bookshelf | 
 *CalendarApi* | [**get_calendar_by_id**](docs/CalendarApi.md#get_calendar_by_id) | **GET** /api/v1/calendar/{id} | 
 *CalendarApi* | [**list_calendar**](docs/CalendarApi.md#list_calendar) | **GET** /api/v1/calendar | 
-*CalendarFeedApi* | [**get_calendar_readarr_ics**](docs/CalendarFeedApi.md#get_calendar_readarr_ics) | **GET** /api/v1/calendar/readarr.ics | 
+*CalendarFeedApi* | [**get_feed_v1_calendar_readarr_ics**](docs/CalendarFeedApi.md#get_feed_v1_calendar_readarr_ics) | **GET** /feed/v1/calendar/readarr.ics | 
 *CommandApi* | [**create_command**](docs/CommandApi.md#create_command) | **POST** /api/v1/command | 
 *CommandApi* | [**delete_command**](docs/CommandApi.md#delete_command) | **DELETE** /api/v1/command/{id} | 
 *CommandApi* | [**get_command_by_id**](docs/CommandApi.md#get_command_by_id) | **GET** /api/v1/command/{id} | 
 *CommandApi* | [**list_command**](docs/CommandApi.md#list_command) | **GET** /api/v1/command | 
 *CustomFilterApi* | [**create_custom_filter**](docs/CustomFilterApi.md#create_custom_filter) | **POST** /api/v1/customfilter | 
 *CustomFilterApi* | [**delete_custom_filter**](docs/CustomFilterApi.md#delete_custom_filter) | **DELETE** /api/v1/customfilter/{id} | 
 *CustomFilterApi* | [**get_custom_filter_by_id**](docs/CustomFilterApi.md#get_custom_filter_by_id) | **GET** /api/v1/customfilter/{id} | 
 *CustomFilterApi* | [**list_custom_filter**](docs/CustomFilterApi.md#list_custom_filter) | **GET** /api/v1/customfilter | 
 *CustomFilterApi* | [**update_custom_filter**](docs/CustomFilterApi.md#update_custom_filter) | **PUT** /api/v1/customfilter/{id} | 
+*CustomFormatApi* | [**create_custom_format**](docs/CustomFormatApi.md#create_custom_format) | **POST** /api/v1/customformat | 
+*CustomFormatApi* | [**delete_custom_format**](docs/CustomFormatApi.md#delete_custom_format) | **DELETE** /api/v1/customformat/{id} | 
+*CustomFormatApi* | [**get_custom_format_by_id**](docs/CustomFormatApi.md#get_custom_format_by_id) | **GET** /api/v1/customformat/{id} | 
+*CustomFormatApi* | [**get_custom_format_schema**](docs/CustomFormatApi.md#get_custom_format_schema) | **GET** /api/v1/customformat/schema | 
+*CustomFormatApi* | [**list_custom_format**](docs/CustomFormatApi.md#list_custom_format) | **GET** /api/v1/customformat | 
+*CustomFormatApi* | [**update_custom_format**](docs/CustomFormatApi.md#update_custom_format) | **PUT** /api/v1/customformat/{id} | 
 *CutoffApi* | [**get_wanted_cutoff**](docs/CutoffApi.md#get_wanted_cutoff) | **GET** /api/v1/wanted/cutoff | 
 *CutoffApi* | [**get_wanted_cutoff_by_id**](docs/CutoffApi.md#get_wanted_cutoff_by_id) | **GET** /api/v1/wanted/cutoff/{id} | 
 *DelayProfileApi* | [**create_delay_profile**](docs/DelayProfileApi.md#create_delay_profile) | **POST** /api/v1/delayprofile | 
 *DelayProfileApi* | [**delete_delay_profile**](docs/DelayProfileApi.md#delete_delay_profile) | **DELETE** /api/v1/delayprofile/{id} | 
 *DelayProfileApi* | [**get_delay_profile_by_id**](docs/DelayProfileApi.md#get_delay_profile_by_id) | **GET** /api/v1/delayprofile/{id} | 
 *DelayProfileApi* | [**list_delay_profile**](docs/DelayProfileApi.md#list_delay_profile) | **GET** /api/v1/delayprofile | 
 *DelayProfileApi* | [**update_delay_profile**](docs/DelayProfileApi.md#update_delay_profile) | **PUT** /api/v1/delayprofile/{id} | 
@@ -162,20 +186,21 @@
 *DownloadClientApi* | [**list_download_client_schema**](docs/DownloadClientApi.md#list_download_client_schema) | **GET** /api/v1/downloadclient/schema | 
 *DownloadClientApi* | [**test_download_client**](docs/DownloadClientApi.md#test_download_client) | **POST** /api/v1/downloadclient/test | 
 *DownloadClientApi* | [**testall_download_client**](docs/DownloadClientApi.md#testall_download_client) | **POST** /api/v1/downloadclient/testall | 
 *DownloadClientApi* | [**update_download_client**](docs/DownloadClientApi.md#update_download_client) | **PUT** /api/v1/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**get_download_client_config**](docs/DownloadClientConfigApi.md#get_download_client_config) | **GET** /api/v1/config/downloadclient | 
 *DownloadClientConfigApi* | [**get_download_client_config_by_id**](docs/DownloadClientConfigApi.md#get_download_client_config_by_id) | **GET** /api/v1/config/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**update_download_client_config**](docs/DownloadClientConfigApi.md#update_download_client_config) | **PUT** /api/v1/config/downloadclient/{id} | 
+*EditionApi* | [**list_edition**](docs/EditionApi.md#list_edition) | **GET** /api/v1/edition | 
 *FileSystemApi* | [**get_file_system**](docs/FileSystemApi.md#get_file_system) | **GET** /api/v1/filesystem | 
 *FileSystemApi* | [**get_file_system_mediafiles**](docs/FileSystemApi.md#get_file_system_mediafiles) | **GET** /api/v1/filesystem/mediafiles | 
 *FileSystemApi* | [**get_file_system_type**](docs/FileSystemApi.md#get_file_system_type) | **GET** /api/v1/filesystem/type | 
 *HealthApi* | [**get_health_by_id**](docs/HealthApi.md#get_health_by_id) | **GET** /api/v1/health/{id} | 
 *HealthApi* | [**list_health**](docs/HealthApi.md#list_health) | **GET** /api/v1/health | 
-*HistoryApi* | [**create_history_failed**](docs/HistoryApi.md#create_history_failed) | **POST** /api/v1/history/failed | 
+*HistoryApi* | [**create_history_failed_by_id**](docs/HistoryApi.md#create_history_failed_by_id) | **POST** /api/v1/history/failed/{id} | 
 *HistoryApi* | [**get_history**](docs/HistoryApi.md#get_history) | **GET** /api/v1/history | 
 *HistoryApi* | [**list_history_author**](docs/HistoryApi.md#list_history_author) | **GET** /api/v1/history/author | 
 *HistoryApi* | [**list_history_since**](docs/HistoryApi.md#list_history_since) | **GET** /api/v1/history/since | 
 *HostConfigApi* | [**get_host_config**](docs/HostConfigApi.md#get_host_config) | **GET** /api/v1/config/host | 
 *HostConfigApi* | [**get_host_config_by_id**](docs/HostConfigApi.md#get_host_config_by_id) | **GET** /api/v1/config/host/{id} | 
 *HostConfigApi* | [**update_host_config**](docs/HostConfigApi.md#update_host_config) | **PUT** /api/v1/config/host/{id} | 
 *ImportListApi* | [**create_import_list**](docs/ImportListApi.md#create_import_list) | **POST** /api/v1/importlist | 
@@ -207,16 +232,16 @@
 *InitializeJsApi* | [**get_initialize_js**](docs/InitializeJsApi.md#get_initialize_js) | **GET** /initialize.js | 
 *LanguageApi* | [**get_language_by_id**](docs/LanguageApi.md#get_language_by_id) | **GET** /api/v1/language/{id} | 
 *LanguageApi* | [**list_language**](docs/LanguageApi.md#list_language) | **GET** /api/v1/language | 
 *LocalizationApi* | [**get_localization**](docs/LocalizationApi.md#get_localization) | **GET** /api/v1/localization | 
 *LogApi* | [**get_log**](docs/LogApi.md#get_log) | **GET** /api/v1/log | 
 *LogFileApi* | [**get_log_file_by_filename**](docs/LogFileApi.md#get_log_file_by_filename) | **GET** /api/v1/log/file/{filename} | 
 *LogFileApi* | [**list_log_file**](docs/LogFileApi.md#list_log_file) | **GET** /api/v1/log/file | 
+*ManualImportApi* | [**create_manual_import**](docs/ManualImportApi.md#create_manual_import) | **POST** /api/v1/manualimport | 
 *ManualImportApi* | [**list_manual_import**](docs/ManualImportApi.md#list_manual_import) | **GET** /api/v1/manualimport | 
-*ManualImportApi* | [**put_manual_import**](docs/ManualImportApi.md#put_manual_import) | **PUT** /api/v1/manualimport | 
 *MediaCoverApi* | [**get_media_cover_authorauthor_id_by_filename**](docs/MediaCoverApi.md#get_media_cover_authorauthor_id_by_filename) | **GET** /api/v1/mediacover/author/{authorId}/{filename} | 
 *MediaCoverApi* | [**get_media_cover_bookbook_id_by_filename**](docs/MediaCoverApi.md#get_media_cover_bookbook_id_by_filename) | **GET** /api/v1/mediacover/book/{bookId}/{filename} | 
 *MediaManagementConfigApi* | [**get_media_management_config**](docs/MediaManagementConfigApi.md#get_media_management_config) | **GET** /api/v1/config/mediamanagement | 
 *MediaManagementConfigApi* | [**get_media_management_config_by_id**](docs/MediaManagementConfigApi.md#get_media_management_config_by_id) | **GET** /api/v1/config/mediamanagement/{id} | 
 *MediaManagementConfigApi* | [**update_media_management_config**](docs/MediaManagementConfigApi.md#update_media_management_config) | **PUT** /api/v1/config/mediamanagement/{id} | 
 *MetadataApi* | [**create_metadata**](docs/MetadataApi.md#create_metadata) | **POST** /api/v1/metadata | 
 *MetadataApi* | [**create_metadata_action_by_name**](docs/MetadataApi.md#create_metadata_action_by_name) | **POST** /api/v1/metadata/action/{name} | 
@@ -248,14 +273,15 @@
 *NotificationApi* | [**get_notification_by_id**](docs/NotificationApi.md#get_notification_by_id) | **GET** /api/v1/notification/{id} | 
 *NotificationApi* | [**list_notification**](docs/NotificationApi.md#list_notification) | **GET** /api/v1/notification | 
 *NotificationApi* | [**list_notification_schema**](docs/NotificationApi.md#list_notification_schema) | **GET** /api/v1/notification/schema | 
 *NotificationApi* | [**test_notification**](docs/NotificationApi.md#test_notification) | **POST** /api/v1/notification/test | 
 *NotificationApi* | [**testall_notification**](docs/NotificationApi.md#testall_notification) | **POST** /api/v1/notification/testall | 
 *NotificationApi* | [**update_notification**](docs/NotificationApi.md#update_notification) | **PUT** /api/v1/notification/{id} | 
 *ParseApi* | [**get_parse**](docs/ParseApi.md#get_parse) | **GET** /api/v1/parse | 
+*PingApi* | [**get_ping**](docs/PingApi.md#get_ping) | **GET** /ping | 
 *QualityDefinitionApi* | [**get_quality_definition_by_id**](docs/QualityDefinitionApi.md#get_quality_definition_by_id) | **GET** /api/v1/qualitydefinition/{id} | 
 *QualityDefinitionApi* | [**list_quality_definition**](docs/QualityDefinitionApi.md#list_quality_definition) | **GET** /api/v1/qualitydefinition | 
 *QualityDefinitionApi* | [**put_quality_definition_update**](docs/QualityDefinitionApi.md#put_quality_definition_update) | **PUT** /api/v1/qualitydefinition/update | 
 *QualityDefinitionApi* | [**update_quality_definition**](docs/QualityDefinitionApi.md#update_quality_definition) | **PUT** /api/v1/qualitydefinition/{id} | 
 *QualityProfileApi* | [**create_quality_profile**](docs/QualityProfileApi.md#create_quality_profile) | **POST** /api/v1/qualityprofile | 
 *QualityProfileApi* | [**delete_quality_profile**](docs/QualityProfileApi.md#delete_quality_profile) | **DELETE** /api/v1/qualityprofile/{id} | 
 *QualityProfileApi* | [**get_quality_profile_by_id**](docs/QualityProfileApi.md#get_quality_profile_by_id) | **GET** /api/v1/qualityprofile/{id} | 
@@ -323,32 +349,34 @@
 
 
 ## Documentation For Models
 
  - [AddAuthorOptions](docs/AddAuthorOptions.md)
  - [AddBookOptions](docs/AddBookOptions.md)
  - [AllowFingerprinting](docs/AllowFingerprinting.md)
+ - [ApiInfoResource](docs/ApiInfoResource.md)
  - [ApplyTags](docs/ApplyTags.md)
  - [AuthenticationType](docs/AuthenticationType.md)
  - [Author](docs/Author.md)
  - [AuthorEditorResource](docs/AuthorEditorResource.md)
  - [AuthorLazyLoaded](docs/AuthorLazyLoaded.md)
  - [AuthorMetadata](docs/AuthorMetadata.md)
  - [AuthorMetadataLazyLoaded](docs/AuthorMetadataLazyLoaded.md)
  - [AuthorResource](docs/AuthorResource.md)
  - [AuthorStatisticsResource](docs/AuthorStatisticsResource.md)
  - [AuthorStatusType](docs/AuthorStatusType.md)
  - [AuthorTitleInfo](docs/AuthorTitleInfo.md)
  - [BackupResource](docs/BackupResource.md)
  - [BackupType](docs/BackupType.md)
- - [BlacklistBulkResource](docs/BlacklistBulkResource.md)
- - [BlacklistResource](docs/BlacklistResource.md)
- - [BlacklistResourcePagingResource](docs/BlacklistResourcePagingResource.md)
+ - [BlocklistBulkResource](docs/BlocklistBulkResource.md)
+ - [BlocklistResource](docs/BlocklistResource.md)
+ - [BlocklistResourcePagingResource](docs/BlocklistResourcePagingResource.md)
  - [Book](docs/Book.md)
  - [BookAddType](docs/BookAddType.md)
+ - [BookEditorResource](docs/BookEditorResource.md)
  - [BookFile](docs/BookFile.md)
  - [BookFileListLazyLoaded](docs/BookFileListLazyLoaded.md)
  - [BookFileListResource](docs/BookFileListResource.md)
  - [BookFileResource](docs/BookFileResource.md)
  - [BookLazyLoaded](docs/BookLazyLoaded.md)
  - [BookListLazyLoaded](docs/BookListLazyLoaded.md)
  - [BookResource](docs/BookResource.md)
@@ -360,63 +388,73 @@
  - [CertificateValidationType](docs/CertificateValidationType.md)
  - [Command](docs/Command.md)
  - [CommandPriority](docs/CommandPriority.md)
  - [CommandResource](docs/CommandResource.md)
  - [CommandStatus](docs/CommandStatus.md)
  - [CommandTrigger](docs/CommandTrigger.md)
  - [CustomFilterResource](docs/CustomFilterResource.md)
+ - [CustomFormat](docs/CustomFormat.md)
+ - [CustomFormatResource](docs/CustomFormatResource.md)
+ - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
+ - [DatabaseType](docs/DatabaseType.md)
  - [DelayProfileResource](docs/DelayProfileResource.md)
  - [DevelopmentConfigResource](docs/DevelopmentConfigResource.md)
  - [DiskSpaceResource](docs/DiskSpaceResource.md)
  - [DownloadClientConfigResource](docs/DownloadClientConfigResource.md)
  - [DownloadClientResource](docs/DownloadClientResource.md)
  - [DownloadProtocol](docs/DownloadProtocol.md)
  - [Edition](docs/Edition.md)
  - [EditionLazyLoaded](docs/EditionLazyLoaded.md)
  - [EditionListLazyLoaded](docs/EditionListLazyLoaded.md)
  - [EditionResource](docs/EditionResource.md)
+ - [EntityHistoryEventType](docs/EntityHistoryEventType.md)
  - [Field](docs/Field.md)
  - [FileDateType](docs/FileDateType.md)
  - [HealthCheckResult](docs/HealthCheckResult.md)
  - [HealthResource](docs/HealthResource.md)
- - [HistoryEventType](docs/HistoryEventType.md)
  - [HistoryResource](docs/HistoryResource.md)
  - [HistoryResourcePagingResource](docs/HistoryResourcePagingResource.md)
  - [HostConfigResource](docs/HostConfigResource.md)
+ - [ICustomFormatSpecification](docs/ICustomFormatSpecification.md)
  - [ImportListExclusionResource](docs/ImportListExclusionResource.md)
  - [ImportListMonitorType](docs/ImportListMonitorType.md)
  - [ImportListResource](docs/ImportListResource.md)
  - [ImportListType](docs/ImportListType.md)
  - [IndexerConfigResource](docs/IndexerConfigResource.md)
  - [IndexerResource](docs/IndexerResource.md)
  - [IsoCountry](docs/IsoCountry.md)
  - [LanguageResource](docs/LanguageResource.md)
  - [Links](docs/Links.md)
  - [LogFileResource](docs/LogFileResource.md)
  - [LogResource](docs/LogResource.md)
  - [LogResourcePagingResource](docs/LogResourcePagingResource.md)
  - [ManualImportResource](docs/ManualImportResource.md)
+ - [ManualImportUpdateResource](docs/ManualImportUpdateResource.md)
  - [MediaCover](docs/MediaCover.md)
  - [MediaCoverTypes](docs/MediaCoverTypes.md)
  - [MediaInfoModel](docs/MediaInfoModel.md)
  - [MediaInfoResource](docs/MediaInfoResource.md)
  - [MediaManagementConfigResource](docs/MediaManagementConfigResource.md)
  - [MetadataProfile](docs/MetadataProfile.md)
  - [MetadataProfileLazyLoaded](docs/MetadataProfileLazyLoaded.md)
  - [MetadataProfileResource](docs/MetadataProfileResource.md)
  - [MetadataProviderConfigResource](docs/MetadataProviderConfigResource.md)
  - [MetadataResource](docs/MetadataResource.md)
  - [MonitorTypes](docs/MonitorTypes.md)
  - [MonitoringOptions](docs/MonitoringOptions.md)
  - [NamingConfigResource](docs/NamingConfigResource.md)
+ - [NewItemMonitorTypes](docs/NewItemMonitorTypes.md)
  - [NotificationResource](docs/NotificationResource.md)
  - [PagingResourceFilter](docs/PagingResourceFilter.md)
  - [ParseResource](docs/ParseResource.md)
  - [ParsedBookInfo](docs/ParsedBookInfo.md)
  - [ParsedTrackInfo](docs/ParsedTrackInfo.md)
+ - [PingResource](docs/PingResource.md)
+ - [ProfileFormatItem](docs/ProfileFormatItem.md)
+ - [ProfileFormatItemResource](docs/ProfileFormatItemResource.md)
  - [ProperDownloadTypes](docs/ProperDownloadTypes.md)
  - [ProviderMessage](docs/ProviderMessage.md)
  - [ProviderMessageType](docs/ProviderMessageType.md)
  - [ProxyType](docs/ProxyType.md)
  - [Quality](docs/Quality.md)
  - [QualityDefinitionResource](docs/QualityDefinitionResource.md)
  - [QualityModel](docs/QualityModel.md)
@@ -436,24 +474,25 @@
  - [ReleaseResource](docs/ReleaseResource.md)
  - [RemotePathMappingResource](docs/RemotePathMappingResource.md)
  - [RenameBookResource](docs/RenameBookResource.md)
  - [RescanAfterRefreshType](docs/RescanAfterRefreshType.md)
  - [RetagBookResource](docs/RetagBookResource.md)
  - [Revision](docs/Revision.md)
  - [RootFolderResource](docs/RootFolderResource.md)
+ - [RuntimeMode](docs/RuntimeMode.md)
  - [SelectOption](docs/SelectOption.md)
  - [Series](docs/Series.md)
  - [SeriesBookLink](docs/SeriesBookLink.md)
  - [SeriesBookLinkListLazyLoaded](docs/SeriesBookLinkListLazyLoaded.md)
  - [SeriesBookLinkResource](docs/SeriesBookLinkResource.md)
  - [SeriesLazyLoaded](docs/SeriesLazyLoaded.md)
  - [SeriesListLazyLoaded](docs/SeriesListLazyLoaded.md)
  - [SeriesResource](docs/SeriesResource.md)
  - [SortDirection](docs/SortDirection.md)
- - [StringInt32KeyValuePair](docs/StringInt32KeyValuePair.md)
+ - [SystemResource](docs/SystemResource.md)
  - [TagDetailsResource](docs/TagDetailsResource.md)
  - [TagDifference](docs/TagDifference.md)
  - [TagResource](docs/TagResource.md)
  - [TaskResource](docs/TaskResource.md)
  - [TrackedDownloadState](docs/TrackedDownloadState.md)
  - [TrackedDownloadStatus](docs/TrackedDownloadStatus.md)
  - [TrackedDownloadStatusMessage](docs/TrackedDownloadStatusMessage.md)
@@ -463,14 +502,27 @@
  - [UpdateResource](docs/UpdateResource.md)
  - [WriteAudioTagsType](docs/WriteAudioTagsType.md)
  - [WriteBookTagsType](docs/WriteBookTagsType.md)
 
 
 ## Documentation For Authorization
 
- All endpoints do not require authorization.
+
+## X-Api-Key
+
+- **Type**: API key
+- **API key parameter name**: X-Api-Key
+- **Location**: HTTP header
+
+
+## apikey
+
+- **Type**: API key
+- **API key parameter name**: apikey
+- **Location**: URL query string
+
 
 ## Author
```

### Comparing `readarr-py-0.2.2/README.md` & `readarr-py-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # readarr-py
 Readarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.2.2
+- Package version: 0.3.0
 
 [comment]: # (x-release-please-end)
-- API version: 0.1.0
+- API version: 1.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
@@ -52,87 +52,111 @@
 from __future__ import print_function
 
 import time
 import readarr
 from readarr.rest import ApiException
 from pprint import pprint
 
-# Defining the host is optional and defaults to http://localhost
+# Defining the host is optional and defaults to http://localhost:8787
 # See configuration.py for a list of all supported configuration parameters.
 configuration = readarr.Configuration(
-    host = "http://localhost"
+    host = "http://localhost:8787"
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure API key authorization: apikey
+configuration.api_key['apikey'] = os.environ["API_KEY"]
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['apikey'] = 'Bearer'
+
+# Configure API key authorization: X-Api-Key
+configuration.api_key['X-Api-Key'] = os.environ["API_KEY"]
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['X-Api-Key'] = 'Bearer'
 
 
 # Enter a context with an instance of the API client
 with readarr.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = readarr.AuthenticationApi(api_client)
-    return_url = 'return_url_example' # str |  (optional)
-    username = 'username_example' # str |  (optional)
-    password = 'password_example' # str |  (optional)
-    remember_me = 'remember_me_example' # str |  (optional)
+    api_instance = readarr.ApiInfoApi(api_client)
 
     try:
-        api_instance.create_login(return_url=return_url, username=username, password=password, remember_me=remember_me)
+        api_response = api_instance.get_api()
+        print("The response of ApiInfoApi->get_api:\n")
+        pprint(api_response)
     except ApiException as e:
-        print("Exception when calling AuthenticationApi->create_login: %s\n" % e)
+        print("Exception when calling ApiInfoApi->get_api: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
-All URIs are relative to *http://localhost*
+All URIs are relative to *http://localhost:8787*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
+*ApiInfoApi* | [**get_api**](docs/ApiInfoApi.md#get_api) | **GET** /api | 
 *AuthenticationApi* | [**create_login**](docs/AuthenticationApi.md#create_login) | **POST** /login | 
 *AuthenticationApi* | [**get_logout**](docs/AuthenticationApi.md#get_logout) | **GET** /logout | 
 *AuthorApi* | [**create_author**](docs/AuthorApi.md#create_author) | **POST** /api/v1/author | 
 *AuthorApi* | [**delete_author**](docs/AuthorApi.md#delete_author) | **DELETE** /api/v1/author/{id} | 
 *AuthorApi* | [**get_author_by_id**](docs/AuthorApi.md#get_author_by_id) | **GET** /api/v1/author/{id} | 
 *AuthorApi* | [**list_author**](docs/AuthorApi.md#list_author) | **GET** /api/v1/author | 
 *AuthorApi* | [**update_author**](docs/AuthorApi.md#update_author) | **PUT** /api/v1/author/{id} | 
 *AuthorEditorApi* | [**delete_author_editor**](docs/AuthorEditorApi.md#delete_author_editor) | **DELETE** /api/v1/author/editor | 
 *AuthorEditorApi* | [**put_author_editor**](docs/AuthorEditorApi.md#put_author_editor) | **PUT** /api/v1/author/editor | 
 *AuthorLookupApi* | [**get_author_lookup**](docs/AuthorLookupApi.md#get_author_lookup) | **GET** /api/v1/author/lookup | 
 *BackupApi* | [**create_system_backup_restore_by_id**](docs/BackupApi.md#create_system_backup_restore_by_id) | **POST** /api/v1/system/backup/restore/{id} | 
 *BackupApi* | [**create_system_backup_restore_upload**](docs/BackupApi.md#create_system_backup_restore_upload) | **POST** /api/v1/system/backup/restore/upload | 
 *BackupApi* | [**delete_system_backup**](docs/BackupApi.md#delete_system_backup) | **DELETE** /api/v1/system/backup/{id} | 
 *BackupApi* | [**list_system_backup**](docs/BackupApi.md#list_system_backup) | **GET** /api/v1/system/backup | 
-*BlacklistApi* | [**delete_blacklist**](docs/BlacklistApi.md#delete_blacklist) | **DELETE** /api/v1/blacklist/{id} | 
-*BlacklistApi* | [**delete_blacklist_bulk**](docs/BlacklistApi.md#delete_blacklist_bulk) | **DELETE** /api/v1/blacklist/bulk | 
-*BlacklistApi* | [**get_blacklist**](docs/BlacklistApi.md#get_blacklist) | **GET** /api/v1/blacklist | 
+*BlocklistApi* | [**delete_blocklist**](docs/BlocklistApi.md#delete_blocklist) | **DELETE** /api/v1/blocklist/{id} | 
+*BlocklistApi* | [**delete_blocklist_bulk**](docs/BlocklistApi.md#delete_blocklist_bulk) | **DELETE** /api/v1/blocklist/bulk | 
+*BlocklistApi* | [**get_blocklist**](docs/BlocklistApi.md#get_blocklist) | **GET** /api/v1/blocklist | 
 *BookApi* | [**create_book**](docs/BookApi.md#create_book) | **POST** /api/v1/book | 
 *BookApi* | [**delete_book**](docs/BookApi.md#delete_book) | **DELETE** /api/v1/book/{id} | 
 *BookApi* | [**get_book_by_id**](docs/BookApi.md#get_book_by_id) | **GET** /api/v1/book/{id} | 
+*BookApi* | [**get_bookid_overview**](docs/BookApi.md#get_bookid_overview) | **GET** /api/v1/book/{id}/overview | 
 *BookApi* | [**list_book**](docs/BookApi.md#list_book) | **GET** /api/v1/book | 
 *BookApi* | [**put_book_monitor**](docs/BookApi.md#put_book_monitor) | **PUT** /api/v1/book/monitor | 
 *BookApi* | [**update_book**](docs/BookApi.md#update_book) | **PUT** /api/v1/book/{id} | 
+*BookEditorApi* | [**delete_book_editor**](docs/BookEditorApi.md#delete_book_editor) | **DELETE** /api/v1/book/editor | 
+*BookEditorApi* | [**put_book_editor**](docs/BookEditorApi.md#put_book_editor) | **PUT** /api/v1/book/editor | 
 *BookFileApi* | [**delete_book_file**](docs/BookFileApi.md#delete_book_file) | **DELETE** /api/v1/bookfile/{id} | 
 *BookFileApi* | [**delete_book_file_bulk**](docs/BookFileApi.md#delete_book_file_bulk) | **DELETE** /api/v1/bookfile/bulk | 
 *BookFileApi* | [**get_book_file_by_id**](docs/BookFileApi.md#get_book_file_by_id) | **GET** /api/v1/bookfile/{id} | 
 *BookFileApi* | [**list_book_file**](docs/BookFileApi.md#list_book_file) | **GET** /api/v1/bookfile | 
 *BookFileApi* | [**put_book_file_editor**](docs/BookFileApi.md#put_book_file_editor) | **PUT** /api/v1/bookfile/editor | 
 *BookFileApi* | [**update_book_file**](docs/BookFileApi.md#update_book_file) | **PUT** /api/v1/bookfile/{id} | 
 *BookLookupApi* | [**get_book_lookup**](docs/BookLookupApi.md#get_book_lookup) | **GET** /api/v1/book/lookup | 
 *BookshelfApi* | [**create_bookshelf**](docs/BookshelfApi.md#create_bookshelf) | **POST** /api/v1/bookshelf | 
 *CalendarApi* | [**get_calendar_by_id**](docs/CalendarApi.md#get_calendar_by_id) | **GET** /api/v1/calendar/{id} | 
 *CalendarApi* | [**list_calendar**](docs/CalendarApi.md#list_calendar) | **GET** /api/v1/calendar | 
-*CalendarFeedApi* | [**get_calendar_readarr_ics**](docs/CalendarFeedApi.md#get_calendar_readarr_ics) | **GET** /api/v1/calendar/readarr.ics | 
+*CalendarFeedApi* | [**get_feed_v1_calendar_readarr_ics**](docs/CalendarFeedApi.md#get_feed_v1_calendar_readarr_ics) | **GET** /feed/v1/calendar/readarr.ics | 
 *CommandApi* | [**create_command**](docs/CommandApi.md#create_command) | **POST** /api/v1/command | 
 *CommandApi* | [**delete_command**](docs/CommandApi.md#delete_command) | **DELETE** /api/v1/command/{id} | 
 *CommandApi* | [**get_command_by_id**](docs/CommandApi.md#get_command_by_id) | **GET** /api/v1/command/{id} | 
 *CommandApi* | [**list_command**](docs/CommandApi.md#list_command) | **GET** /api/v1/command | 
 *CustomFilterApi* | [**create_custom_filter**](docs/CustomFilterApi.md#create_custom_filter) | **POST** /api/v1/customfilter | 
 *CustomFilterApi* | [**delete_custom_filter**](docs/CustomFilterApi.md#delete_custom_filter) | **DELETE** /api/v1/customfilter/{id} | 
 *CustomFilterApi* | [**get_custom_filter_by_id**](docs/CustomFilterApi.md#get_custom_filter_by_id) | **GET** /api/v1/customfilter/{id} | 
 *CustomFilterApi* | [**list_custom_filter**](docs/CustomFilterApi.md#list_custom_filter) | **GET** /api/v1/customfilter | 
 *CustomFilterApi* | [**update_custom_filter**](docs/CustomFilterApi.md#update_custom_filter) | **PUT** /api/v1/customfilter/{id} | 
+*CustomFormatApi* | [**create_custom_format**](docs/CustomFormatApi.md#create_custom_format) | **POST** /api/v1/customformat | 
+*CustomFormatApi* | [**delete_custom_format**](docs/CustomFormatApi.md#delete_custom_format) | **DELETE** /api/v1/customformat/{id} | 
+*CustomFormatApi* | [**get_custom_format_by_id**](docs/CustomFormatApi.md#get_custom_format_by_id) | **GET** /api/v1/customformat/{id} | 
+*CustomFormatApi* | [**get_custom_format_schema**](docs/CustomFormatApi.md#get_custom_format_schema) | **GET** /api/v1/customformat/schema | 
+*CustomFormatApi* | [**list_custom_format**](docs/CustomFormatApi.md#list_custom_format) | **GET** /api/v1/customformat | 
+*CustomFormatApi* | [**update_custom_format**](docs/CustomFormatApi.md#update_custom_format) | **PUT** /api/v1/customformat/{id} | 
 *CutoffApi* | [**get_wanted_cutoff**](docs/CutoffApi.md#get_wanted_cutoff) | **GET** /api/v1/wanted/cutoff | 
 *CutoffApi* | [**get_wanted_cutoff_by_id**](docs/CutoffApi.md#get_wanted_cutoff_by_id) | **GET** /api/v1/wanted/cutoff/{id} | 
 *DelayProfileApi* | [**create_delay_profile**](docs/DelayProfileApi.md#create_delay_profile) | **POST** /api/v1/delayprofile | 
 *DelayProfileApi* | [**delete_delay_profile**](docs/DelayProfileApi.md#delete_delay_profile) | **DELETE** /api/v1/delayprofile/{id} | 
 *DelayProfileApi* | [**get_delay_profile_by_id**](docs/DelayProfileApi.md#get_delay_profile_by_id) | **GET** /api/v1/delayprofile/{id} | 
 *DelayProfileApi* | [**list_delay_profile**](docs/DelayProfileApi.md#list_delay_profile) | **GET** /api/v1/delayprofile | 
 *DelayProfileApi* | [**update_delay_profile**](docs/DelayProfileApi.md#update_delay_profile) | **PUT** /api/v1/delayprofile/{id} | 
@@ -149,20 +173,21 @@
 *DownloadClientApi* | [**list_download_client_schema**](docs/DownloadClientApi.md#list_download_client_schema) | **GET** /api/v1/downloadclient/schema | 
 *DownloadClientApi* | [**test_download_client**](docs/DownloadClientApi.md#test_download_client) | **POST** /api/v1/downloadclient/test | 
 *DownloadClientApi* | [**testall_download_client**](docs/DownloadClientApi.md#testall_download_client) | **POST** /api/v1/downloadclient/testall | 
 *DownloadClientApi* | [**update_download_client**](docs/DownloadClientApi.md#update_download_client) | **PUT** /api/v1/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**get_download_client_config**](docs/DownloadClientConfigApi.md#get_download_client_config) | **GET** /api/v1/config/downloadclient | 
 *DownloadClientConfigApi* | [**get_download_client_config_by_id**](docs/DownloadClientConfigApi.md#get_download_client_config_by_id) | **GET** /api/v1/config/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**update_download_client_config**](docs/DownloadClientConfigApi.md#update_download_client_config) | **PUT** /api/v1/config/downloadclient/{id} | 
+*EditionApi* | [**list_edition**](docs/EditionApi.md#list_edition) | **GET** /api/v1/edition | 
 *FileSystemApi* | [**get_file_system**](docs/FileSystemApi.md#get_file_system) | **GET** /api/v1/filesystem | 
 *FileSystemApi* | [**get_file_system_mediafiles**](docs/FileSystemApi.md#get_file_system_mediafiles) | **GET** /api/v1/filesystem/mediafiles | 
 *FileSystemApi* | [**get_file_system_type**](docs/FileSystemApi.md#get_file_system_type) | **GET** /api/v1/filesystem/type | 
 *HealthApi* | [**get_health_by_id**](docs/HealthApi.md#get_health_by_id) | **GET** /api/v1/health/{id} | 
 *HealthApi* | [**list_health**](docs/HealthApi.md#list_health) | **GET** /api/v1/health | 
-*HistoryApi* | [**create_history_failed**](docs/HistoryApi.md#create_history_failed) | **POST** /api/v1/history/failed | 
+*HistoryApi* | [**create_history_failed_by_id**](docs/HistoryApi.md#create_history_failed_by_id) | **POST** /api/v1/history/failed/{id} | 
 *HistoryApi* | [**get_history**](docs/HistoryApi.md#get_history) | **GET** /api/v1/history | 
 *HistoryApi* | [**list_history_author**](docs/HistoryApi.md#list_history_author) | **GET** /api/v1/history/author | 
 *HistoryApi* | [**list_history_since**](docs/HistoryApi.md#list_history_since) | **GET** /api/v1/history/since | 
 *HostConfigApi* | [**get_host_config**](docs/HostConfigApi.md#get_host_config) | **GET** /api/v1/config/host | 
 *HostConfigApi* | [**get_host_config_by_id**](docs/HostConfigApi.md#get_host_config_by_id) | **GET** /api/v1/config/host/{id} | 
 *HostConfigApi* | [**update_host_config**](docs/HostConfigApi.md#update_host_config) | **PUT** /api/v1/config/host/{id} | 
 *ImportListApi* | [**create_import_list**](docs/ImportListApi.md#create_import_list) | **POST** /api/v1/importlist | 
@@ -194,16 +219,16 @@
 *InitializeJsApi* | [**get_initialize_js**](docs/InitializeJsApi.md#get_initialize_js) | **GET** /initialize.js | 
 *LanguageApi* | [**get_language_by_id**](docs/LanguageApi.md#get_language_by_id) | **GET** /api/v1/language/{id} | 
 *LanguageApi* | [**list_language**](docs/LanguageApi.md#list_language) | **GET** /api/v1/language | 
 *LocalizationApi* | [**get_localization**](docs/LocalizationApi.md#get_localization) | **GET** /api/v1/localization | 
 *LogApi* | [**get_log**](docs/LogApi.md#get_log) | **GET** /api/v1/log | 
 *LogFileApi* | [**get_log_file_by_filename**](docs/LogFileApi.md#get_log_file_by_filename) | **GET** /api/v1/log/file/{filename} | 
 *LogFileApi* | [**list_log_file**](docs/LogFileApi.md#list_log_file) | **GET** /api/v1/log/file | 
+*ManualImportApi* | [**create_manual_import**](docs/ManualImportApi.md#create_manual_import) | **POST** /api/v1/manualimport | 
 *ManualImportApi* | [**list_manual_import**](docs/ManualImportApi.md#list_manual_import) | **GET** /api/v1/manualimport | 
-*ManualImportApi* | [**put_manual_import**](docs/ManualImportApi.md#put_manual_import) | **PUT** /api/v1/manualimport | 
 *MediaCoverApi* | [**get_media_cover_authorauthor_id_by_filename**](docs/MediaCoverApi.md#get_media_cover_authorauthor_id_by_filename) | **GET** /api/v1/mediacover/author/{authorId}/{filename} | 
 *MediaCoverApi* | [**get_media_cover_bookbook_id_by_filename**](docs/MediaCoverApi.md#get_media_cover_bookbook_id_by_filename) | **GET** /api/v1/mediacover/book/{bookId}/{filename} | 
 *MediaManagementConfigApi* | [**get_media_management_config**](docs/MediaManagementConfigApi.md#get_media_management_config) | **GET** /api/v1/config/mediamanagement | 
 *MediaManagementConfigApi* | [**get_media_management_config_by_id**](docs/MediaManagementConfigApi.md#get_media_management_config_by_id) | **GET** /api/v1/config/mediamanagement/{id} | 
 *MediaManagementConfigApi* | [**update_media_management_config**](docs/MediaManagementConfigApi.md#update_media_management_config) | **PUT** /api/v1/config/mediamanagement/{id} | 
 *MetadataApi* | [**create_metadata**](docs/MetadataApi.md#create_metadata) | **POST** /api/v1/metadata | 
 *MetadataApi* | [**create_metadata_action_by_name**](docs/MetadataApi.md#create_metadata_action_by_name) | **POST** /api/v1/metadata/action/{name} | 
@@ -235,14 +260,15 @@
 *NotificationApi* | [**get_notification_by_id**](docs/NotificationApi.md#get_notification_by_id) | **GET** /api/v1/notification/{id} | 
 *NotificationApi* | [**list_notification**](docs/NotificationApi.md#list_notification) | **GET** /api/v1/notification | 
 *NotificationApi* | [**list_notification_schema**](docs/NotificationApi.md#list_notification_schema) | **GET** /api/v1/notification/schema | 
 *NotificationApi* | [**test_notification**](docs/NotificationApi.md#test_notification) | **POST** /api/v1/notification/test | 
 *NotificationApi* | [**testall_notification**](docs/NotificationApi.md#testall_notification) | **POST** /api/v1/notification/testall | 
 *NotificationApi* | [**update_notification**](docs/NotificationApi.md#update_notification) | **PUT** /api/v1/notification/{id} | 
 *ParseApi* | [**get_parse**](docs/ParseApi.md#get_parse) | **GET** /api/v1/parse | 
+*PingApi* | [**get_ping**](docs/PingApi.md#get_ping) | **GET** /ping | 
 *QualityDefinitionApi* | [**get_quality_definition_by_id**](docs/QualityDefinitionApi.md#get_quality_definition_by_id) | **GET** /api/v1/qualitydefinition/{id} | 
 *QualityDefinitionApi* | [**list_quality_definition**](docs/QualityDefinitionApi.md#list_quality_definition) | **GET** /api/v1/qualitydefinition | 
 *QualityDefinitionApi* | [**put_quality_definition_update**](docs/QualityDefinitionApi.md#put_quality_definition_update) | **PUT** /api/v1/qualitydefinition/update | 
 *QualityDefinitionApi* | [**update_quality_definition**](docs/QualityDefinitionApi.md#update_quality_definition) | **PUT** /api/v1/qualitydefinition/{id} | 
 *QualityProfileApi* | [**create_quality_profile**](docs/QualityProfileApi.md#create_quality_profile) | **POST** /api/v1/qualityprofile | 
 *QualityProfileApi* | [**delete_quality_profile**](docs/QualityProfileApi.md#delete_quality_profile) | **DELETE** /api/v1/qualityprofile/{id} | 
 *QualityProfileApi* | [**get_quality_profile_by_id**](docs/QualityProfileApi.md#get_quality_profile_by_id) | **GET** /api/v1/qualityprofile/{id} | 
@@ -310,32 +336,34 @@
 
 
 ## Documentation For Models
 
  - [AddAuthorOptions](docs/AddAuthorOptions.md)
  - [AddBookOptions](docs/AddBookOptions.md)
  - [AllowFingerprinting](docs/AllowFingerprinting.md)
+ - [ApiInfoResource](docs/ApiInfoResource.md)
  - [ApplyTags](docs/ApplyTags.md)
  - [AuthenticationType](docs/AuthenticationType.md)
  - [Author](docs/Author.md)
  - [AuthorEditorResource](docs/AuthorEditorResource.md)
  - [AuthorLazyLoaded](docs/AuthorLazyLoaded.md)
  - [AuthorMetadata](docs/AuthorMetadata.md)
  - [AuthorMetadataLazyLoaded](docs/AuthorMetadataLazyLoaded.md)
  - [AuthorResource](docs/AuthorResource.md)
  - [AuthorStatisticsResource](docs/AuthorStatisticsResource.md)
  - [AuthorStatusType](docs/AuthorStatusType.md)
  - [AuthorTitleInfo](docs/AuthorTitleInfo.md)
  - [BackupResource](docs/BackupResource.md)
  - [BackupType](docs/BackupType.md)
- - [BlacklistBulkResource](docs/BlacklistBulkResource.md)
- - [BlacklistResource](docs/BlacklistResource.md)
- - [BlacklistResourcePagingResource](docs/BlacklistResourcePagingResource.md)
+ - [BlocklistBulkResource](docs/BlocklistBulkResource.md)
+ - [BlocklistResource](docs/BlocklistResource.md)
+ - [BlocklistResourcePagingResource](docs/BlocklistResourcePagingResource.md)
  - [Book](docs/Book.md)
  - [BookAddType](docs/BookAddType.md)
+ - [BookEditorResource](docs/BookEditorResource.md)
  - [BookFile](docs/BookFile.md)
  - [BookFileListLazyLoaded](docs/BookFileListLazyLoaded.md)
  - [BookFileListResource](docs/BookFileListResource.md)
  - [BookFileResource](docs/BookFileResource.md)
  - [BookLazyLoaded](docs/BookLazyLoaded.md)
  - [BookListLazyLoaded](docs/BookListLazyLoaded.md)
  - [BookResource](docs/BookResource.md)
@@ -347,63 +375,73 @@
  - [CertificateValidationType](docs/CertificateValidationType.md)
  - [Command](docs/Command.md)
  - [CommandPriority](docs/CommandPriority.md)
  - [CommandResource](docs/CommandResource.md)
  - [CommandStatus](docs/CommandStatus.md)
  - [CommandTrigger](docs/CommandTrigger.md)
  - [CustomFilterResource](docs/CustomFilterResource.md)
+ - [CustomFormat](docs/CustomFormat.md)
+ - [CustomFormatResource](docs/CustomFormatResource.md)
+ - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
+ - [DatabaseType](docs/DatabaseType.md)
  - [DelayProfileResource](docs/DelayProfileResource.md)
  - [DevelopmentConfigResource](docs/DevelopmentConfigResource.md)
  - [DiskSpaceResource](docs/DiskSpaceResource.md)
  - [DownloadClientConfigResource](docs/DownloadClientConfigResource.md)
  - [DownloadClientResource](docs/DownloadClientResource.md)
  - [DownloadProtocol](docs/DownloadProtocol.md)
  - [Edition](docs/Edition.md)
  - [EditionLazyLoaded](docs/EditionLazyLoaded.md)
  - [EditionListLazyLoaded](docs/EditionListLazyLoaded.md)
  - [EditionResource](docs/EditionResource.md)
+ - [EntityHistoryEventType](docs/EntityHistoryEventType.md)
  - [Field](docs/Field.md)
  - [FileDateType](docs/FileDateType.md)
  - [HealthCheckResult](docs/HealthCheckResult.md)
  - [HealthResource](docs/HealthResource.md)
- - [HistoryEventType](docs/HistoryEventType.md)
  - [HistoryResource](docs/HistoryResource.md)
  - [HistoryResourcePagingResource](docs/HistoryResourcePagingResource.md)
  - [HostConfigResource](docs/HostConfigResource.md)
+ - [ICustomFormatSpecification](docs/ICustomFormatSpecification.md)
  - [ImportListExclusionResource](docs/ImportListExclusionResource.md)
  - [ImportListMonitorType](docs/ImportListMonitorType.md)
  - [ImportListResource](docs/ImportListResource.md)
  - [ImportListType](docs/ImportListType.md)
  - [IndexerConfigResource](docs/IndexerConfigResource.md)
  - [IndexerResource](docs/IndexerResource.md)
  - [IsoCountry](docs/IsoCountry.md)
  - [LanguageResource](docs/LanguageResource.md)
  - [Links](docs/Links.md)
  - [LogFileResource](docs/LogFileResource.md)
  - [LogResource](docs/LogResource.md)
  - [LogResourcePagingResource](docs/LogResourcePagingResource.md)
  - [ManualImportResource](docs/ManualImportResource.md)
+ - [ManualImportUpdateResource](docs/ManualImportUpdateResource.md)
  - [MediaCover](docs/MediaCover.md)
  - [MediaCoverTypes](docs/MediaCoverTypes.md)
  - [MediaInfoModel](docs/MediaInfoModel.md)
  - [MediaInfoResource](docs/MediaInfoResource.md)
  - [MediaManagementConfigResource](docs/MediaManagementConfigResource.md)
  - [MetadataProfile](docs/MetadataProfile.md)
  - [MetadataProfileLazyLoaded](docs/MetadataProfileLazyLoaded.md)
  - [MetadataProfileResource](docs/MetadataProfileResource.md)
  - [MetadataProviderConfigResource](docs/MetadataProviderConfigResource.md)
  - [MetadataResource](docs/MetadataResource.md)
  - [MonitorTypes](docs/MonitorTypes.md)
  - [MonitoringOptions](docs/MonitoringOptions.md)
  - [NamingConfigResource](docs/NamingConfigResource.md)
+ - [NewItemMonitorTypes](docs/NewItemMonitorTypes.md)
  - [NotificationResource](docs/NotificationResource.md)
  - [PagingResourceFilter](docs/PagingResourceFilter.md)
  - [ParseResource](docs/ParseResource.md)
  - [ParsedBookInfo](docs/ParsedBookInfo.md)
  - [ParsedTrackInfo](docs/ParsedTrackInfo.md)
+ - [PingResource](docs/PingResource.md)
+ - [ProfileFormatItem](docs/ProfileFormatItem.md)
+ - [ProfileFormatItemResource](docs/ProfileFormatItemResource.md)
  - [ProperDownloadTypes](docs/ProperDownloadTypes.md)
  - [ProviderMessage](docs/ProviderMessage.md)
  - [ProviderMessageType](docs/ProviderMessageType.md)
  - [ProxyType](docs/ProxyType.md)
  - [Quality](docs/Quality.md)
  - [QualityDefinitionResource](docs/QualityDefinitionResource.md)
  - [QualityModel](docs/QualityModel.md)
@@ -423,24 +461,25 @@
  - [ReleaseResource](docs/ReleaseResource.md)
  - [RemotePathMappingResource](docs/RemotePathMappingResource.md)
  - [RenameBookResource](docs/RenameBookResource.md)
  - [RescanAfterRefreshType](docs/RescanAfterRefreshType.md)
  - [RetagBookResource](docs/RetagBookResource.md)
  - [Revision](docs/Revision.md)
  - [RootFolderResource](docs/RootFolderResource.md)
+ - [RuntimeMode](docs/RuntimeMode.md)
  - [SelectOption](docs/SelectOption.md)
  - [Series](docs/Series.md)
  - [SeriesBookLink](docs/SeriesBookLink.md)
  - [SeriesBookLinkListLazyLoaded](docs/SeriesBookLinkListLazyLoaded.md)
  - [SeriesBookLinkResource](docs/SeriesBookLinkResource.md)
  - [SeriesLazyLoaded](docs/SeriesLazyLoaded.md)
  - [SeriesListLazyLoaded](docs/SeriesListLazyLoaded.md)
  - [SeriesResource](docs/SeriesResource.md)
  - [SortDirection](docs/SortDirection.md)
- - [StringInt32KeyValuePair](docs/StringInt32KeyValuePair.md)
+ - [SystemResource](docs/SystemResource.md)
  - [TagDetailsResource](docs/TagDetailsResource.md)
  - [TagDifference](docs/TagDifference.md)
  - [TagResource](docs/TagResource.md)
  - [TaskResource](docs/TaskResource.md)
  - [TrackedDownloadState](docs/TrackedDownloadState.md)
  - [TrackedDownloadStatus](docs/TrackedDownloadStatus.md)
  - [TrackedDownloadStatusMessage](docs/TrackedDownloadStatusMessage.md)
@@ -450,14 +489,27 @@
  - [UpdateResource](docs/UpdateResource.md)
  - [WriteAudioTagsType](docs/WriteAudioTagsType.md)
  - [WriteBookTagsType](docs/WriteBookTagsType.md)
 
 
 ## Documentation For Authorization
 
- All endpoints do not require authorization.
+
+## X-Api-Key
+
+- **Type**: API key
+- **API key parameter name**: X-Api-Key
+- **Location**: HTTP header
+
+
+## apikey
+
+- **Type**: API key
+- **API key parameter name**: apikey
+- **Location**: URL query string
+
 
 ## Author
```

### Comparing `readarr-py-0.2.2/pyproject.toml` & `readarr-py-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 [project]
 name = "readarr-py"
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

### Comparing `readarr-py-0.2.2/readarr/__init__.py` & `readarr-py-0.3.0/readarr/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,46 +3,50 @@
 # flake8: noqa
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # x-release-please-start-version
-__version__ = "0.2.2"
+__version__ = "0.3.0"
 # x-release-please-end
 
 # import apis into sdk package
+from readarr.api.api_info_api import ApiInfoApi
 from readarr.api.authentication_api import AuthenticationApi
 from readarr.api.author_api import AuthorApi
 from readarr.api.author_editor_api import AuthorEditorApi
 from readarr.api.author_lookup_api import AuthorLookupApi
 from readarr.api.backup_api import BackupApi
-from readarr.api.blacklist_api import BlacklistApi
+from readarr.api.blocklist_api import BlocklistApi
 from readarr.api.book_api import BookApi
+from readarr.api.book_editor_api import BookEditorApi
 from readarr.api.book_file_api import BookFileApi
 from readarr.api.book_lookup_api import BookLookupApi
 from readarr.api.bookshelf_api import BookshelfApi
 from readarr.api.calendar_api import CalendarApi
 from readarr.api.calendar_feed_api import CalendarFeedApi
 from readarr.api.command_api import CommandApi
 from readarr.api.custom_filter_api import CustomFilterApi
+from readarr.api.custom_format_api import CustomFormatApi
 from readarr.api.cutoff_api import CutoffApi
 from readarr.api.delay_profile_api import DelayProfileApi
 from readarr.api.development_config_api import DevelopmentConfigApi
 from readarr.api.disk_space_api import DiskSpaceApi
 from readarr.api.download_client_api import DownloadClientApi
 from readarr.api.download_client_config_api import DownloadClientConfigApi
+from readarr.api.edition_api import EditionApi
 from readarr.api.file_system_api import FileSystemApi
 from readarr.api.health_api import HealthApi
 from readarr.api.history_api import HistoryApi
 from readarr.api.host_config_api import HostConfigApi
 from readarr.api.import_list_api import ImportListApi
 from readarr.api.import_list_exclusion_api import ImportListExclusionApi
 from readarr.api.indexer_api import IndexerApi
@@ -59,14 +63,15 @@
 from readarr.api.metadata_profile_api import MetadataProfileApi
 from readarr.api.metadata_profile_schema_api import MetadataProfileSchemaApi
 from readarr.api.metadata_provider_config_api import MetadataProviderConfigApi
 from readarr.api.missing_api import MissingApi
 from readarr.api.naming_config_api import NamingConfigApi
 from readarr.api.notification_api import NotificationApi
 from readarr.api.parse_api import ParseApi
+from readarr.api.ping_api import PingApi
 from readarr.api.quality_definition_api import QualityDefinitionApi
 from readarr.api.quality_profile_api import QualityProfileApi
 from readarr.api.quality_profile_schema_api import QualityProfileSchemaApi
 from readarr.api.queue_api import QueueApi
 from readarr.api.queue_action_api import QueueActionApi
 from readarr.api.queue_details_api import QueueDetailsApi
 from readarr.api.queue_status_api import QueueStatusApi
@@ -97,32 +102,34 @@
 from readarr.exceptions import ApiKeyError
 from readarr.exceptions import ApiAttributeError
 from readarr.exceptions import ApiException
 # import models into sdk package
 from readarr.models.add_author_options import AddAuthorOptions
 from readarr.models.add_book_options import AddBookOptions
 from readarr.models.allow_fingerprinting import AllowFingerprinting
+from readarr.models.api_info_resource import ApiInfoResource
 from readarr.models.apply_tags import ApplyTags
 from readarr.models.authentication_type import AuthenticationType
 from readarr.models.author import Author
 from readarr.models.author_editor_resource import AuthorEditorResource
 from readarr.models.author_lazy_loaded import AuthorLazyLoaded
 from readarr.models.author_metadata import AuthorMetadata
 from readarr.models.author_metadata_lazy_loaded import AuthorMetadataLazyLoaded
 from readarr.models.author_resource import AuthorResource
 from readarr.models.author_statistics_resource import AuthorStatisticsResource
 from readarr.models.author_status_type import AuthorStatusType
 from readarr.models.author_title_info import AuthorTitleInfo
 from readarr.models.backup_resource import BackupResource
 from readarr.models.backup_type import BackupType
-from readarr.models.blacklist_bulk_resource import BlacklistBulkResource
-from readarr.models.blacklist_resource import BlacklistResource
-from readarr.models.blacklist_resource_paging_resource import BlacklistResourcePagingResource
+from readarr.models.blocklist_bulk_resource import BlocklistBulkResource
+from readarr.models.blocklist_resource import BlocklistResource
+from readarr.models.blocklist_resource_paging_resource import BlocklistResourcePagingResource
 from readarr.models.book import Book
 from readarr.models.book_add_type import BookAddType
+from readarr.models.book_editor_resource import BookEditorResource
 from readarr.models.book_file import BookFile
 from readarr.models.book_file_list_lazy_loaded import BookFileListLazyLoaded
 from readarr.models.book_file_list_resource import BookFileListResource
 from readarr.models.book_file_resource import BookFileResource
 from readarr.models.book_lazy_loaded import BookLazyLoaded
 from readarr.models.book_list_lazy_loaded import BookListLazyLoaded
 from readarr.models.book_resource import BookResource
@@ -134,63 +141,73 @@
 from readarr.models.certificate_validation_type import CertificateValidationType
 from readarr.models.command import Command
 from readarr.models.command_priority import CommandPriority
 from readarr.models.command_resource import CommandResource
 from readarr.models.command_status import CommandStatus
 from readarr.models.command_trigger import CommandTrigger
 from readarr.models.custom_filter_resource import CustomFilterResource
+from readarr.models.custom_format import CustomFormat
+from readarr.models.custom_format_resource import CustomFormatResource
+from readarr.models.custom_format_specification_schema import CustomFormatSpecificationSchema
+from readarr.models.database_type import DatabaseType
 from readarr.models.delay_profile_resource import DelayProfileResource
 from readarr.models.development_config_resource import DevelopmentConfigResource
 from readarr.models.disk_space_resource import DiskSpaceResource
 from readarr.models.download_client_config_resource import DownloadClientConfigResource
 from readarr.models.download_client_resource import DownloadClientResource
 from readarr.models.download_protocol import DownloadProtocol
 from readarr.models.edition import Edition
 from readarr.models.edition_lazy_loaded import EditionLazyLoaded
 from readarr.models.edition_list_lazy_loaded import EditionListLazyLoaded
 from readarr.models.edition_resource import EditionResource
+from readarr.models.entity_history_event_type import EntityHistoryEventType
 from readarr.models.field import Field
 from readarr.models.file_date_type import FileDateType
 from readarr.models.health_check_result import HealthCheckResult
 from readarr.models.health_resource import HealthResource
-from readarr.models.history_event_type import HistoryEventType
 from readarr.models.history_resource import HistoryResource
 from readarr.models.history_resource_paging_resource import HistoryResourcePagingResource
 from readarr.models.host_config_resource import HostConfigResource
+from readarr.models.i_custom_format_specification import ICustomFormatSpecification
 from readarr.models.import_list_exclusion_resource import ImportListExclusionResource
 from readarr.models.import_list_monitor_type import ImportListMonitorType
 from readarr.models.import_list_resource import ImportListResource
 from readarr.models.import_list_type import ImportListType
 from readarr.models.indexer_config_resource import IndexerConfigResource
 from readarr.models.indexer_resource import IndexerResource
 from readarr.models.iso_country import IsoCountry
 from readarr.models.language_resource import LanguageResource
 from readarr.models.links import Links
 from readarr.models.log_file_resource import LogFileResource
 from readarr.models.log_resource import LogResource
 from readarr.models.log_resource_paging_resource import LogResourcePagingResource
 from readarr.models.manual_import_resource import ManualImportResource
+from readarr.models.manual_import_update_resource import ManualImportUpdateResource
 from readarr.models.media_cover import MediaCover
 from readarr.models.media_cover_types import MediaCoverTypes
 from readarr.models.media_info_model import MediaInfoModel
 from readarr.models.media_info_resource import MediaInfoResource
 from readarr.models.media_management_config_resource import MediaManagementConfigResource
 from readarr.models.metadata_profile import MetadataProfile
 from readarr.models.metadata_profile_lazy_loaded import MetadataProfileLazyLoaded
 from readarr.models.metadata_profile_resource import MetadataProfileResource
 from readarr.models.metadata_provider_config_resource import MetadataProviderConfigResource
 from readarr.models.metadata_resource import MetadataResource
 from readarr.models.monitor_types import MonitorTypes
 from readarr.models.monitoring_options import MonitoringOptions
 from readarr.models.naming_config_resource import NamingConfigResource
+from readarr.models.new_item_monitor_types import NewItemMonitorTypes
 from readarr.models.notification_resource import NotificationResource
 from readarr.models.paging_resource_filter import PagingResourceFilter
 from readarr.models.parse_resource import ParseResource
 from readarr.models.parsed_book_info import ParsedBookInfo
 from readarr.models.parsed_track_info import ParsedTrackInfo
+from readarr.models.ping_resource import PingResource
+from readarr.models.profile_format_item import ProfileFormatItem
+from readarr.models.profile_format_item_resource import ProfileFormatItemResource
 from readarr.models.proper_download_types import ProperDownloadTypes
 from readarr.models.provider_message import ProviderMessage
 from readarr.models.provider_message_type import ProviderMessageType
 from readarr.models.proxy_type import ProxyType
 from readarr.models.quality import Quality
 from readarr.models.quality_definition_resource import QualityDefinitionResource
 from readarr.models.quality_model import QualityModel
@@ -210,24 +227,25 @@
 from readarr.models.release_resource import ReleaseResource
 from readarr.models.remote_path_mapping_resource import RemotePathMappingResource
 from readarr.models.rename_book_resource import RenameBookResource
 from readarr.models.rescan_after_refresh_type import RescanAfterRefreshType
 from readarr.models.retag_book_resource import RetagBookResource
 from readarr.models.revision import Revision
 from readarr.models.root_folder_resource import RootFolderResource
+from readarr.models.runtime_mode import RuntimeMode
 from readarr.models.select_option import SelectOption
 from readarr.models.series import Series
 from readarr.models.series_book_link import SeriesBookLink
 from readarr.models.series_book_link_list_lazy_loaded import SeriesBookLinkListLazyLoaded
 from readarr.models.series_book_link_resource import SeriesBookLinkResource
 from readarr.models.series_lazy_loaded import SeriesLazyLoaded
 from readarr.models.series_list_lazy_loaded import SeriesListLazyLoaded
 from readarr.models.series_resource import SeriesResource
 from readarr.models.sort_direction import SortDirection
-from readarr.models.string_int32_key_value_pair import StringInt32KeyValuePair
+from readarr.models.system_resource import SystemResource
 from readarr.models.tag_details_resource import TagDetailsResource
 from readarr.models.tag_difference import TagDifference
 from readarr.models.tag_resource import TagResource
 from readarr.models.task_resource import TaskResource
 from readarr.models.tracked_download_state import TrackedDownloadState
 from readarr.models.tracked_download_status import TrackedDownloadStatus
 from readarr.models.tracked_download_status_message import TrackedDownloadStatusMessage
```

### Comparing `readarr-py-0.2.2/readarr/api/__init__.py` & `readarr-py-0.3.0/readarr/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,40 +3,44 @@
 # flake8: noqa
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 # import apis into api package
+from readarr.api.api_info_api import ApiInfoApi
 from readarr.api.authentication_api import AuthenticationApi
 from readarr.api.author_api import AuthorApi
 from readarr.api.author_editor_api import AuthorEditorApi
 from readarr.api.author_lookup_api import AuthorLookupApi
 from readarr.api.backup_api import BackupApi
-from readarr.api.blacklist_api import BlacklistApi
+from readarr.api.blocklist_api import BlocklistApi
 from readarr.api.book_api import BookApi
+from readarr.api.book_editor_api import BookEditorApi
 from readarr.api.book_file_api import BookFileApi
 from readarr.api.book_lookup_api import BookLookupApi
 from readarr.api.bookshelf_api import BookshelfApi
 from readarr.api.calendar_api import CalendarApi
 from readarr.api.calendar_feed_api import CalendarFeedApi
 from readarr.api.command_api import CommandApi
 from readarr.api.custom_filter_api import CustomFilterApi
+from readarr.api.custom_format_api import CustomFormatApi
 from readarr.api.cutoff_api import CutoffApi
 from readarr.api.delay_profile_api import DelayProfileApi
 from readarr.api.development_config_api import DevelopmentConfigApi
 from readarr.api.disk_space_api import DiskSpaceApi
 from readarr.api.download_client_api import DownloadClientApi
 from readarr.api.download_client_config_api import DownloadClientConfigApi
+from readarr.api.edition_api import EditionApi
 from readarr.api.file_system_api import FileSystemApi
 from readarr.api.health_api import HealthApi
 from readarr.api.history_api import HistoryApi
 from readarr.api.host_config_api import HostConfigApi
 from readarr.api.import_list_api import ImportListApi
 from readarr.api.import_list_exclusion_api import ImportListExclusionApi
 from readarr.api.indexer_api import IndexerApi
@@ -53,14 +57,15 @@
 from readarr.api.metadata_profile_api import MetadataProfileApi
 from readarr.api.metadata_profile_schema_api import MetadataProfileSchemaApi
 from readarr.api.metadata_provider_config_api import MetadataProviderConfigApi
 from readarr.api.missing_api import MissingApi
 from readarr.api.naming_config_api import NamingConfigApi
 from readarr.api.notification_api import NotificationApi
 from readarr.api.parse_api import ParseApi
+from readarr.api.ping_api import PingApi
 from readarr.api.quality_definition_api import QualityDefinitionApi
 from readarr.api.quality_profile_api import QualityProfileApi
 from readarr.api.quality_profile_schema_api import QualityProfileSchemaApi
 from readarr.api.queue_api import QueueApi
 from readarr.api.queue_action_api import QueueActionApi
 from readarr.api.queue_details_api import QueueDetailsApi
 from readarr.api.queue_status_api import QueueStatusApi
```

### Comparing `readarr-py-0.2.2/readarr/api/authentication_api.py` & `readarr-py-0.3.0/readarr/api/authentication_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -179,15 +179,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['multipart/form-data']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/login', 'POST',
             _path_params,
             _query_params,
@@ -307,15 +307,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/logout', 'GET',
             _path_params,
             _query_params,
```

### Comparing `readarr-py-0.2.2/readarr/api/author_api.py` & `readarr-py-0.3.0/readarr/api/author_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -163,15 +163,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "AuthorResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/author', 'POST',
@@ -300,15 +300,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/author/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -439,15 +439,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "AuthorResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/author/{id}', 'GET',
@@ -573,15 +573,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[AuthorResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/author', 'GET',
@@ -728,15 +728,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "AuthorResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/author/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/author_editor_api.py` & `readarr-py-0.3.0/readarr/api/author_editor_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -157,15 +157,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/author/editor', 'DELETE',
             _path_params,
             _query_params,
@@ -299,15 +299,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/author/editor', 'PUT',
             _path_params,
             _query_params,
```

### Comparing `readarr-py-0.2.2/readarr/api/author_lookup_api.py` & `readarr-py-0.3.0/readarr/api/author_lookup_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -151,15 +151,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/author/lookup', 'GET',
             _path_params,
             _query_params,
```

### Comparing `readarr-py-0.2.2/readarr/api/backup_api.py` & `readarr-py-0.3.0/readarr/api/backup_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -152,15 +152,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/system/backup/restore/{id}', 'POST',
             _path_params,
             _query_params,
@@ -280,15 +280,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/system/backup/restore/upload', 'POST',
             _path_params,
             _query_params,
@@ -415,15 +415,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/system/backup/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -547,15 +547,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[BackupResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/system/backup', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/blacklist_api.py` & `readarr-py-0.3.0/readarr/api/blocklist_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -17,44 +17,44 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictInt
 
 from typing import Optional
 
-from readarr.models.blacklist_bulk_resource import BlacklistBulkResource
-from readarr.models.blacklist_resource_paging_resource import BlacklistResourcePagingResource
+from readarr.models.blocklist_bulk_resource import BlocklistBulkResource
+from readarr.models.blocklist_resource_paging_resource import BlocklistResourcePagingResource
 
 from readarr.api_client import ApiClient
 from readarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class BlacklistApi(object):
+class BlocklistApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def delete_blacklist(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
-        """delete_blacklist  # noqa: E501
+    def delete_blocklist(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
+        """delete_blocklist  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_blacklist(id, async_req=True)
+        >>> thread = api.delete_blocklist(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -67,24 +67,24 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_blacklist_with_http_info(id, **kwargs)  # noqa: E501
+        return self.delete_blocklist_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_blacklist_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """delete_blacklist  # noqa: E501
+    def delete_blocklist_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """delete_blocklist  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_blacklist_with_http_info(id, async_req=True)
+        >>> thread = api.delete_blocklist_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -127,15 +127,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_blacklist" % _key
+                    " to method delete_blocklist" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -153,20 +153,20 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/blacklist/{id}', 'DELETE',
+            '/api/v1/blocklist/{id}', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -175,25 +175,25 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_blacklist_bulk(self, blacklist_bulk_resource : Optional[BlacklistBulkResource] = None, **kwargs) -> None:  # noqa: E501
-        """delete_blacklist_bulk  # noqa: E501
+    def delete_blocklist_bulk(self, blocklist_bulk_resource : Optional[BlocklistBulkResource] = None, **kwargs) -> None:  # noqa: E501
+        """delete_blocklist_bulk  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_blacklist_bulk(blacklist_bulk_resource, async_req=True)
+        >>> thread = api.delete_blocklist_bulk(blocklist_bulk_resource, async_req=True)
         >>> result = thread.get()
 
-        :param blacklist_bulk_resource:
-        :type blacklist_bulk_resource: BlacklistBulkResource
+        :param blocklist_bulk_resource:
+        :type blocklist_bulk_resource: BlocklistBulkResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -202,28 +202,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_blacklist_bulk_with_http_info(blacklist_bulk_resource, **kwargs)  # noqa: E501
+        return self.delete_blocklist_bulk_with_http_info(blocklist_bulk_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_blacklist_bulk_with_http_info(self, blacklist_bulk_resource : Optional[BlacklistBulkResource] = None, **kwargs):  # noqa: E501
-        """delete_blacklist_bulk  # noqa: E501
+    def delete_blocklist_bulk_with_http_info(self, blocklist_bulk_resource : Optional[BlocklistBulkResource] = None, **kwargs):  # noqa: E501
+        """delete_blocklist_bulk  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_blacklist_bulk_with_http_info(blacklist_bulk_resource, async_req=True)
+        >>> thread = api.delete_blocklist_bulk_with_http_info(blocklist_bulk_resource, async_req=True)
         >>> result = thread.get()
 
-        :param blacklist_bulk_resource:
-        :type blacklist_bulk_resource: BlacklistBulkResource
+        :param blocklist_bulk_resource:
+        :type blocklist_bulk_resource: BlocklistBulkResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -243,15 +243,15 @@
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'blacklist_bulk_resource'
+            'blocklist_bulk_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -262,15 +262,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_blacklist_bulk" % _key
+                    " to method delete_blocklist_bulk" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -284,31 +284,31 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['blacklist_bulk_resource']:
-            _body_params = _params['blacklist_bulk_resource']
+        if _params['blocklist_bulk_resource']:
+            _body_params = _params['blocklist_bulk_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/blacklist/bulk', 'DELETE',
+            '/api/v1/blocklist/bulk', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -317,21 +317,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_blacklist(self, **kwargs) -> BlacklistResourcePagingResource:  # noqa: E501
-        """get_blacklist  # noqa: E501
+    def get_blocklist(self, **kwargs) -> BlocklistResourcePagingResource:  # noqa: E501
+        """get_blocklist  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_blacklist(async_req=True)
+        >>> thread = api.get_blocklist(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -339,27 +339,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: BlacklistResourcePagingResource
+        :rtype: BlocklistResourcePagingResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_blacklist_with_http_info(**kwargs)  # noqa: E501
+        return self.get_blocklist_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_blacklist_with_http_info(self, **kwargs):  # noqa: E501
-        """get_blacklist  # noqa: E501
+    def get_blocklist_with_http_info(self, **kwargs):  # noqa: E501
+        """get_blocklist  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_blacklist_with_http_info(async_req=True)
+        >>> thread = api.get_blocklist_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -375,15 +375,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(BlacklistResourcePagingResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(BlocklistResourcePagingResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
@@ -399,15 +399,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_blacklist" % _key
+                    " to method get_blocklist" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -427,22 +427,22 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "BlacklistResourcePagingResource",
+            '200': "BlocklistResourcePagingResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/blacklist', 'GET',
+            '/api/v1/blocklist', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `readarr-py-0.2.2/readarr/api/book_api.py` & `readarr-py-0.3.0/readarr/api/book_file_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -17,78 +17,78 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictBool, StrictInt, StrictStr, conlist
 
 from typing import List, Optional
 
-from readarr.models.book_resource import BookResource
-from readarr.models.books_monitored_resource import BooksMonitoredResource
+from readarr.models.book_file_list_resource import BookFileListResource
+from readarr.models.book_file_resource import BookFileResource
 
 from readarr.api_client import ApiClient
 from readarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class BookApi(object):
+class BookFileApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_book(self, book_resource : Optional[BookResource] = None, **kwargs) -> BookResource:  # noqa: E501
-        """create_book  # noqa: E501
+    def delete_book_file(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
+        """delete_book_file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_book(book_resource, async_req=True)
+        >>> thread = api.delete_book_file(id, async_req=True)
         >>> result = thread.get()
 
-        :param book_resource:
-        :type book_resource: BookResource
+        :param id: (required)
+        :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: BookResource
+        :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_book_with_http_info(book_resource, **kwargs)  # noqa: E501
+        return self.delete_book_file_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_book_with_http_info(self, book_resource : Optional[BookResource] = None, **kwargs):  # noqa: E501
-        """create_book  # noqa: E501
+    def delete_book_file_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """delete_book_file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_book_with_http_info(book_resource, async_req=True)
+        >>> thread = api.delete_book_file_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
-        :param book_resource:
-        :type book_resource: BookResource
+        :param id: (required)
+        :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -102,21 +102,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(BookResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'book_resource'
+            'id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -127,59 +127,46 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_book" % _key
+                    " to method delete_book_file" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
+        if _params['id']:
+            _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['book_resource']:
-            _body_params = _params['book_resource']
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
-
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {
-            '200': "BookResource",
-        }
+        _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/book', 'POST',
+            '/api/v1/bookfile/{id}', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -188,25 +175,25 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_book(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
-        """delete_book  # noqa: E501
+    def delete_book_file_bulk(self, book_file_list_resource : Optional[BookFileListResource] = None, **kwargs) -> None:  # noqa: E501
+        """delete_book_file_bulk  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_book(id, async_req=True)
+        >>> thread = api.delete_book_file_bulk(book_file_list_resource, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
+        :param book_file_list_resource:
+        :type book_file_list_resource: BookFileListResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -215,28 +202,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_book_with_http_info(id, **kwargs)  # noqa: E501
+        return self.delete_book_file_bulk_with_http_info(book_file_list_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_book_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """delete_book  # noqa: E501
+    def delete_book_file_bulk_with_http_info(self, book_file_list_resource : Optional[BookFileListResource] = None, **kwargs):  # noqa: E501
+        """delete_book_file_bulk  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_book_with_http_info(id, async_req=True)
+        >>> thread = api.delete_book_file_bulk_with_http_info(book_file_list_resource, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
+        :param book_file_list_resource:
+        :type book_file_list_resource: BookFileListResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -256,15 +243,15 @@
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
+            'book_file_list_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -275,46 +262,53 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_book" % _key
+                    " to method delete_book_file_bulk" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
+        if _params['book_file_list_resource']:
+            _body_params = _params['book_file_list_resource']
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json', 'text/json', 'application/*+json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/book/{id}', 'DELETE',
+            '/api/v1/bookfile/bulk', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -323,21 +317,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_book_by_id(self, id : StrictInt, **kwargs) -> BookResource:  # noqa: E501
-        """get_book_by_id  # noqa: E501
+    def get_book_file_by_id(self, id : StrictInt, **kwargs) -> BookFileResource:  # noqa: E501
+        """get_book_file_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_book_by_id(id, async_req=True)
+        >>> thread = api.get_book_file_by_id(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -347,27 +341,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: BookResource
+        :rtype: BookFileResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_book_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_book_file_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_book_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_book_by_id  # noqa: E501
+    def get_book_file_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_book_file_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_book_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.get_book_file_by_id_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -385,15 +379,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(BookResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(BookFileResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id'
         ]
@@ -410,15 +404,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_book_by_id" % _key
+                    " to method get_book_file_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -440,22 +434,22 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "BookResource",
+            '200': "BookFileResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/book/{id}', 'GET',
+            '/api/v1/bookfile/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -464,67 +458,67 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_book(self, author_id : Optional[StrictInt] = None, book_ids : Optional[conlist(StrictInt)] = None, title_slug : Optional[StrictStr] = None, include_all_author_books : Optional[StrictBool] = None, **kwargs) -> List[BookResource]:  # noqa: E501
-        """list_book  # noqa: E501
+    def list_book_file(self, author_id : Optional[StrictInt] = None, book_file_ids : Optional[conlist(StrictInt)] = None, book_id : Optional[conlist(StrictInt)] = None, unmapped : Optional[StrictBool] = None, **kwargs) -> List[BookFileResource]:  # noqa: E501
+        """list_book_file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_book(author_id, book_ids, title_slug, include_all_author_books, async_req=True)
+        >>> thread = api.list_book_file(author_id, book_file_ids, book_id, unmapped, async_req=True)
         >>> result = thread.get()
 
         :param author_id:
         :type author_id: int
-        :param book_ids:
-        :type book_ids: List[int]
-        :param title_slug:
-        :type title_slug: str
-        :param include_all_author_books:
-        :type include_all_author_books: bool
+        :param book_file_ids:
+        :type book_file_ids: List[int]
+        :param book_id:
+        :type book_id: List[int]
+        :param unmapped:
+        :type unmapped: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: List[BookResource]
+        :rtype: List[BookFileResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_book_with_http_info(author_id, book_ids, title_slug, include_all_author_books, **kwargs)  # noqa: E501
+        return self.list_book_file_with_http_info(author_id, book_file_ids, book_id, unmapped, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_book_with_http_info(self, author_id : Optional[StrictInt] = None, book_ids : Optional[conlist(StrictInt)] = None, title_slug : Optional[StrictStr] = None, include_all_author_books : Optional[StrictBool] = None, **kwargs):  # noqa: E501
-        """list_book  # noqa: E501
+    def list_book_file_with_http_info(self, author_id : Optional[StrictInt] = None, book_file_ids : Optional[conlist(StrictInt)] = None, book_id : Optional[conlist(StrictInt)] = None, unmapped : Optional[StrictBool] = None, **kwargs):  # noqa: E501
+        """list_book_file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_book_with_http_info(author_id, book_ids, title_slug, include_all_author_books, async_req=True)
+        >>> thread = api.list_book_file_with_http_info(author_id, book_file_ids, book_id, unmapped, async_req=True)
         >>> result = thread.get()
 
         :param author_id:
         :type author_id: int
-        :param book_ids:
-        :type book_ids: List[int]
-        :param title_slug:
-        :type title_slug: str
-        :param include_all_author_books:
-        :type include_all_author_books: bool
+        :param book_file_ids:
+        :type book_file_ids: List[int]
+        :param book_id:
+        :type book_id: List[int]
+        :param unmapped:
+        :type unmapped: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -538,24 +532,24 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[BookResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[BookFileResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'author_id',
-            'book_ids',
-            'title_slug',
-            'include_all_author_books'
+            'book_file_ids',
+            'book_id',
+            'unmapped'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -566,35 +560,36 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_book" % _key
+                    " to method list_book_file" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
         if _params.get('author_id') is not None:  # noqa: E501
             _query_params.append(('authorId', _params['author_id']))
-        if _params.get('book_ids') is not None:  # noqa: E501
-            _query_params.append(('bookIds', _params['book_ids']))
-            _collection_formats['bookIds'] = 'multi'
-        if _params.get('title_slug') is not None:  # noqa: E501
-            _query_params.append(('titleSlug', _params['title_slug']))
-        if _params.get('include_all_author_books') is not None:  # noqa: E501
-            _query_params.append(('includeAllAuthorBooks', _params['include_all_author_books']))
+        if _params.get('book_file_ids') is not None:  # noqa: E501
+            _query_params.append(('bookFileIds', _params['book_file_ids']))
+            _collection_formats['bookFileIds'] = 'multi'
+        if _params.get('book_id') is not None:  # noqa: E501
+            _query_params.append(('bookId', _params['book_id']))
+            _collection_formats['bookId'] = 'multi'
+        if _params.get('unmapped') is not None:  # noqa: E501
+            _query_params.append(('unmapped', _params['unmapped']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -603,22 +598,22 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[BookResource]",
+            '200': "List[BookFileResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/book', 'GET',
+            '/api/v1/bookfile', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -627,25 +622,25 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def put_book_monitor(self, books_monitored_resource : Optional[BooksMonitoredResource] = None, **kwargs) -> None:  # noqa: E501
-        """put_book_monitor  # noqa: E501
+    def put_book_file_editor(self, book_file_list_resource : Optional[BookFileListResource] = None, **kwargs) -> None:  # noqa: E501
+        """put_book_file_editor  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.put_book_monitor(books_monitored_resource, async_req=True)
+        >>> thread = api.put_book_file_editor(book_file_list_resource, async_req=True)
         >>> result = thread.get()
 
-        :param books_monitored_resource:
-        :type books_monitored_resource: BooksMonitoredResource
+        :param book_file_list_resource:
+        :type book_file_list_resource: BookFileListResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -654,28 +649,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.put_book_monitor_with_http_info(books_monitored_resource, **kwargs)  # noqa: E501
+        return self.put_book_file_editor_with_http_info(book_file_list_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def put_book_monitor_with_http_info(self, books_monitored_resource : Optional[BooksMonitoredResource] = None, **kwargs):  # noqa: E501
-        """put_book_monitor  # noqa: E501
+    def put_book_file_editor_with_http_info(self, book_file_list_resource : Optional[BookFileListResource] = None, **kwargs):  # noqa: E501
+        """put_book_file_editor  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.put_book_monitor_with_http_info(books_monitored_resource, async_req=True)
+        >>> thread = api.put_book_file_editor_with_http_info(book_file_list_resource, async_req=True)
         >>> result = thread.get()
 
-        :param books_monitored_resource:
-        :type books_monitored_resource: BooksMonitoredResource
+        :param book_file_list_resource:
+        :type book_file_list_resource: BookFileListResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -695,15 +690,15 @@
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'books_monitored_resource'
+            'book_file_list_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -714,15 +709,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method put_book_monitor" % _key
+                    " to method put_book_file_editor" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -736,31 +731,31 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['books_monitored_resource']:
-            _body_params = _params['books_monitored_resource']
+        if _params['book_file_list_resource']:
+            _body_params = _params['book_file_list_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/book/monitor', 'PUT',
+            '/api/v1/bookfile/editor', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -769,59 +764,59 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_book(self, id : StrictStr, book_resource : Optional[BookResource] = None, **kwargs) -> BookResource:  # noqa: E501
-        """update_book  # noqa: E501
+    def update_book_file(self, id : StrictStr, book_file_resource : Optional[BookFileResource] = None, **kwargs) -> BookFileResource:  # noqa: E501
+        """update_book_file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_book(id, book_resource, async_req=True)
+        >>> thread = api.update_book_file(id, book_file_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
-        :param book_resource:
-        :type book_resource: BookResource
+        :param book_file_resource:
+        :type book_file_resource: BookFileResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: BookResource
+        :rtype: BookFileResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_book_with_http_info(id, book_resource, **kwargs)  # noqa: E501
+        return self.update_book_file_with_http_info(id, book_file_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_book_with_http_info(self, id : StrictStr, book_resource : Optional[BookResource] = None, **kwargs):  # noqa: E501
-        """update_book  # noqa: E501
+    def update_book_file_with_http_info(self, id : StrictStr, book_file_resource : Optional[BookFileResource] = None, **kwargs):  # noqa: E501
+        """update_book_file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_book_with_http_info(id, book_resource, async_req=True)
+        >>> thread = api.update_book_file_with_http_info(id, book_file_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
-        :param book_resource:
-        :type book_resource: BookResource
+        :param book_file_resource:
+        :type book_file_resource: BookFileResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -835,22 +830,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(BookResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(BookFileResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
-            'book_resource'
+            'book_file_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -861,15 +856,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_book" % _key
+                    " to method update_book_file" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -885,37 +880,37 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['book_resource']:
-            _body_params = _params['book_resource']
+        if _params['book_file_resource']:
+            _body_params = _params['book_file_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "BookResource",
+            '200': "BookFileResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/book/{id}', 'PUT',
+            '/api/v1/bookfile/{id}', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `readarr-py-0.2.2/readarr/api/book_file_api.py` & `readarr-py-0.3.0/readarr/api/custom_format_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,94 +1,93 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictBool, StrictInt, StrictStr, conlist
+from pydantic import StrictInt, StrictStr
 
 from typing import List, Optional
 
-from readarr.models.book_file_list_resource import BookFileListResource
-from readarr.models.book_file_resource import BookFileResource
+from readarr.models.custom_format_resource import CustomFormatResource
 
 from readarr.api_client import ApiClient
 from readarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class BookFileApi(object):
+class CustomFormatApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def delete_book_file(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
-        """delete_book_file  # noqa: E501
+    def create_custom_format(self, custom_format_resource : Optional[CustomFormatResource] = None, **kwargs) -> CustomFormatResource:  # noqa: E501
+        """create_custom_format  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_book_file(id, async_req=True)
+        >>> thread = api.create_custom_format(custom_format_resource, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
+        :param custom_format_resource:
+        :type custom_format_resource: CustomFormatResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: CustomFormatResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_book_file_with_http_info(id, **kwargs)  # noqa: E501
+        return self.create_custom_format_with_http_info(custom_format_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_book_file_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """delete_book_file  # noqa: E501
+    def create_custom_format_with_http_info(self, custom_format_resource : Optional[CustomFormatResource] = None, **kwargs):  # noqa: E501
+        """create_custom_format  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_book_file_with_http_info(id, async_req=True)
+        >>> thread = api.create_custom_format_with_http_info(custom_format_resource, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
+        :param custom_format_resource:
+        :type custom_format_resource: CustomFormatResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -102,21 +101,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: tuple(CustomFormatResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
+            'custom_format_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -127,46 +126,59 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_book_file" % _key
+                    " to method create_custom_format" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
+        if _params['custom_format_resource']:
+            _body_params = _params['custom_format_resource']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {}
+        _response_types_map = {
+            '200': "CustomFormatResource",
+        }
 
         return self.api_client.call_api(
-            '/api/v1/bookfile/{id}', 'DELETE',
+            '/api/v1/customformat', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -175,25 +187,25 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_book_file_bulk(self, book_file_list_resource : Optional[BookFileListResource] = None, **kwargs) -> None:  # noqa: E501
-        """delete_book_file_bulk  # noqa: E501
+    def delete_custom_format(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
+        """delete_custom_format  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_book_file_bulk(book_file_list_resource, async_req=True)
+        >>> thread = api.delete_custom_format(id, async_req=True)
         >>> result = thread.get()
 
-        :param book_file_list_resource:
-        :type book_file_list_resource: BookFileListResource
+        :param id: (required)
+        :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -202,28 +214,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_book_file_bulk_with_http_info(book_file_list_resource, **kwargs)  # noqa: E501
+        return self.delete_custom_format_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_book_file_bulk_with_http_info(self, book_file_list_resource : Optional[BookFileListResource] = None, **kwargs):  # noqa: E501
-        """delete_book_file_bulk  # noqa: E501
+    def delete_custom_format_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """delete_custom_format  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_book_file_bulk_with_http_info(book_file_list_resource, async_req=True)
+        >>> thread = api.delete_custom_format_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
-        :param book_file_list_resource:
-        :type book_file_list_resource: BookFileListResource
+        :param id: (required)
+        :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -243,15 +255,15 @@
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'book_file_list_resource'
+            'id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -262,53 +274,46 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_book_file_bulk" % _key
+                    " to method delete_custom_format" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
+        if _params['id']:
+            _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['book_file_list_resource']:
-            _body_params = _params['book_file_list_resource']
-
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/bookfile/bulk', 'DELETE',
+            '/api/v1/customformat/{id}', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -317,21 +322,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_book_file_by_id(self, id : StrictInt, **kwargs) -> BookFileResource:  # noqa: E501
-        """get_book_file_by_id  # noqa: E501
+    def get_custom_format_by_id(self, id : StrictInt, **kwargs) -> CustomFormatResource:  # noqa: E501
+        """get_custom_format_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_book_file_by_id(id, async_req=True)
+        >>> thread = api.get_custom_format_by_id(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -341,27 +346,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: BookFileResource
+        :rtype: CustomFormatResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_book_file_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_custom_format_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_book_file_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_book_file_by_id  # noqa: E501
+    def get_custom_format_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_custom_format_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_book_file_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.get_custom_format_by_id_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -379,15 +384,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(BookFileResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(CustomFormatResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id'
         ]
@@ -404,15 +409,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_book_file_by_id" % _key
+                    " to method get_custom_format_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -434,22 +439,22 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "BookFileResource",
+            '200': "CustomFormatResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/bookfile/{id}', 'GET',
+            '/api/v1/customformat/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -458,67 +463,51 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_book_file(self, author_id : Optional[StrictInt] = None, book_file_ids : Optional[conlist(StrictInt)] = None, book_id : Optional[conlist(StrictInt)] = None, unmapped : Optional[StrictBool] = None, **kwargs) -> List[BookFileResource]:  # noqa: E501
-        """list_book_file  # noqa: E501
+    def get_custom_format_schema(self, **kwargs) -> None:  # noqa: E501
+        """get_custom_format_schema  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_book_file(author_id, book_file_ids, book_id, unmapped, async_req=True)
+        >>> thread = api.get_custom_format_schema(async_req=True)
         >>> result = thread.get()
 
-        :param author_id:
-        :type author_id: int
-        :param book_file_ids:
-        :type book_file_ids: List[int]
-        :param book_id:
-        :type book_id: List[int]
-        :param unmapped:
-        :type unmapped: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: List[BookFileResource]
+        :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_book_file_with_http_info(author_id, book_file_ids, book_id, unmapped, **kwargs)  # noqa: E501
+        return self.get_custom_format_schema_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_book_file_with_http_info(self, author_id : Optional[StrictInt] = None, book_file_ids : Optional[conlist(StrictInt)] = None, book_id : Optional[conlist(StrictInt)] = None, unmapped : Optional[StrictBool] = None, **kwargs):  # noqa: E501
-        """list_book_file  # noqa: E501
+    def get_custom_format_schema_with_http_info(self, **kwargs):  # noqa: E501
+        """get_custom_format_schema  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_book_file_with_http_info(author_id, book_file_ids, book_id, unmapped, async_req=True)
+        >>> thread = api.get_custom_format_schema_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param author_id:
-        :type author_id: int
-        :param book_file_ids:
-        :type book_file_ids: List[int]
-        :param book_id:
-        :type book_id: List[int]
-        :param unmapped:
-        :type unmapped: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -532,24 +521,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[BookFileResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'author_id',
-            'book_file_ids',
-            'book_id',
-            'unmapped'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -560,60 +545,44 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_book_file" % _key
+                    " to method get_custom_format_schema" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
-        if _params.get('author_id') is not None:  # noqa: E501
-            _query_params.append(('authorId', _params['author_id']))
-        if _params.get('book_file_ids') is not None:  # noqa: E501
-            _query_params.append(('bookFileIds', _params['book_file_ids']))
-            _collection_formats['bookFileIds'] = 'multi'
-        if _params.get('book_id') is not None:  # noqa: E501
-            _query_params.append(('bookId', _params['book_id']))
-            _collection_formats['bookId'] = 'multi'
-        if _params.get('unmapped') is not None:  # noqa: E501
-            _query_params.append(('unmapped', _params['unmapped']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
-
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {
-            '200': "List[BookFileResource]",
-        }
+        _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/bookfile', 'GET',
+            '/api/v1/customformat/schema', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -622,55 +591,51 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def put_book_file_editor(self, book_file_list_resource : Optional[BookFileListResource] = None, **kwargs) -> None:  # noqa: E501
-        """put_book_file_editor  # noqa: E501
+    def list_custom_format(self, **kwargs) -> List[CustomFormatResource]:  # noqa: E501
+        """list_custom_format  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.put_book_file_editor(book_file_list_resource, async_req=True)
+        >>> thread = api.list_custom_format(async_req=True)
         >>> result = thread.get()
 
-        :param book_file_list_resource:
-        :type book_file_list_resource: BookFileListResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: List[CustomFormatResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.put_book_file_editor_with_http_info(book_file_list_resource, **kwargs)  # noqa: E501
+        return self.list_custom_format_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def put_book_file_editor_with_http_info(self, book_file_list_resource : Optional[BookFileListResource] = None, **kwargs):  # noqa: E501
-        """put_book_file_editor  # noqa: E501
+    def list_custom_format_with_http_info(self, **kwargs):  # noqa: E501
+        """list_custom_format  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.put_book_file_editor_with_http_info(book_file_list_resource, async_req=True)
+        >>> thread = api.list_custom_format_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param book_file_list_resource:
-        :type book_file_list_resource: BookFileListResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -684,21 +649,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: tuple(List[CustomFormatResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'book_file_list_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -709,15 +673,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method put_book_file_editor" % _key
+                    " to method list_custom_format" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -731,31 +695,28 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['book_file_list_resource']:
-            _body_params = _params['book_file_list_resource']
 
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {}
+        _response_types_map = {
+            '200': "List[CustomFormatResource]",
+        }
 
         return self.api_client.call_api(
-            '/api/v1/bookfile/editor', 'PUT',
+            '/api/v1/customformat', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -764,59 +725,59 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_book_file(self, id : StrictStr, book_file_resource : Optional[BookFileResource] = None, **kwargs) -> BookFileResource:  # noqa: E501
-        """update_book_file  # noqa: E501
+    def update_custom_format(self, id : StrictStr, custom_format_resource : Optional[CustomFormatResource] = None, **kwargs) -> CustomFormatResource:  # noqa: E501
+        """update_custom_format  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_book_file(id, book_file_resource, async_req=True)
+        >>> thread = api.update_custom_format(id, custom_format_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
-        :param book_file_resource:
-        :type book_file_resource: BookFileResource
+        :param custom_format_resource:
+        :type custom_format_resource: CustomFormatResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: BookFileResource
+        :rtype: CustomFormatResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_book_file_with_http_info(id, book_file_resource, **kwargs)  # noqa: E501
+        return self.update_custom_format_with_http_info(id, custom_format_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_book_file_with_http_info(self, id : StrictStr, book_file_resource : Optional[BookFileResource] = None, **kwargs):  # noqa: E501
-        """update_book_file  # noqa: E501
+    def update_custom_format_with_http_info(self, id : StrictStr, custom_format_resource : Optional[CustomFormatResource] = None, **kwargs):  # noqa: E501
+        """update_custom_format  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_book_file_with_http_info(id, book_file_resource, async_req=True)
+        >>> thread = api.update_custom_format_with_http_info(id, custom_format_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
-        :param book_file_resource:
-        :type book_file_resource: BookFileResource
+        :param custom_format_resource:
+        :type custom_format_resource: CustomFormatResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -830,22 +791,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(BookFileResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(CustomFormatResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
-            'book_file_resource'
+            'custom_format_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -856,15 +817,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_book_file" % _key
+                    " to method update_custom_format" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -880,37 +841,37 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['book_file_resource']:
-            _body_params = _params['book_file_resource']
+        if _params['custom_format_resource']:
+            _body_params = _params['custom_format_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "BookFileResource",
+            '200': "CustomFormatResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/bookfile/{id}', 'PUT',
+            '/api/v1/customformat/{id}', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `readarr-py-0.2.2/readarr/api/book_lookup_api.py` & `readarr-py-0.3.0/readarr/api/book_lookup_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -151,15 +151,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/book/lookup', 'GET',
             _path_params,
             _query_params,
```

### Comparing `readarr-py-0.2.2/readarr/api/bookshelf_api.py` & `readarr-py-0.3.0/readarr/api/bookshelf_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -157,15 +157,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/bookshelf', 'POST',
             _path_params,
             _query_params,
```

### Comparing `readarr-py-0.2.2/readarr/api/calendar_api.py` & `readarr-py-0.3.0/readarr/api/calendar_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -158,15 +158,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "BookResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/calendar/{id}', 'GET',
@@ -320,15 +320,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[BookResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/calendar', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/calendar_feed_api.py` & `readarr-py-0.3.0/readarr/api/calendar_feed_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -38,21 +38,21 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_calendar_readarr_ics(self, past_days : Optional[StrictInt] = None, future_days : Optional[StrictInt] = None, tag_list : Optional[StrictStr] = None, unmonitored : Optional[StrictBool] = None, **kwargs) -> None:  # noqa: E501
-        """get_calendar_readarr_ics  # noqa: E501
+    def get_feed_v1_calendar_readarr_ics(self, past_days : Optional[StrictInt] = None, future_days : Optional[StrictInt] = None, tag_list : Optional[StrictStr] = None, unmonitored : Optional[StrictBool] = None, **kwargs) -> None:  # noqa: E501
+        """get_feed_v1_calendar_readarr_ics  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_calendar_readarr_ics(past_days, future_days, tag_list, unmonitored, async_req=True)
+        >>> thread = api.get_feed_v1_calendar_readarr_ics(past_days, future_days, tag_list, unmonitored, async_req=True)
         >>> result = thread.get()
 
         :param past_days:
         :type past_days: int
         :param future_days:
         :type future_days: int
         :param tag_list:
@@ -71,24 +71,24 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_calendar_readarr_ics_with_http_info(past_days, future_days, tag_list, unmonitored, **kwargs)  # noqa: E501
+        return self.get_feed_v1_calendar_readarr_ics_with_http_info(past_days, future_days, tag_list, unmonitored, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_calendar_readarr_ics_with_http_info(self, past_days : Optional[StrictInt] = None, future_days : Optional[StrictInt] = None, tag_list : Optional[StrictStr] = None, unmonitored : Optional[StrictBool] = None, **kwargs):  # noqa: E501
-        """get_calendar_readarr_ics  # noqa: E501
+    def get_feed_v1_calendar_readarr_ics_with_http_info(self, past_days : Optional[StrictInt] = None, future_days : Optional[StrictInt] = None, tag_list : Optional[StrictStr] = None, unmonitored : Optional[StrictBool] = None, **kwargs):  # noqa: E501
+        """get_feed_v1_calendar_readarr_ics  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_calendar_readarr_ics_with_http_info(past_days, future_days, tag_list, unmonitored, async_req=True)
+        >>> thread = api.get_feed_v1_calendar_readarr_ics_with_http_info(past_days, future_days, tag_list, unmonitored, async_req=True)
         >>> result = thread.get()
 
         :param past_days:
         :type past_days: int
         :param future_days:
         :type future_days: int
         :param tag_list:
@@ -140,15 +140,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_calendar_readarr_ics" % _key
+                    " to method get_feed_v1_calendar_readarr_ics" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -172,20 +172,20 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/calendar/readarr.ics', 'GET',
+            '/feed/v1/calendar/readarr.ics', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `readarr-py-0.2.2/readarr/api/command_api.py` & `readarr-py-0.3.0/readarr/api/command_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -163,15 +163,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "CommandResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/command', 'POST',
@@ -300,15 +300,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/command/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -439,15 +439,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "CommandResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/command/{id}', 'GET',
@@ -573,15 +573,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[CommandResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/command', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/custom_filter_api.py` & `readarr-py-0.3.0/readarr/api/custom_filter_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -163,15 +163,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "CustomFilterResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/customfilter', 'POST',
@@ -300,15 +300,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/customfilter/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -439,15 +439,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "CustomFilterResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/customfilter/{id}', 'GET',
@@ -573,15 +573,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[CustomFilterResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/customfilter', 'GET',
@@ -728,15 +728,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "CustomFilterResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/customfilter/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/cutoff_api.py` & `readarr-py-0.3.0/readarr/api/cutoff_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -157,15 +157,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "BookResourcePagingResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/wanted/cutoff', 'GET',
@@ -298,15 +298,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "BookResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/wanted/cutoff/{id}', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/delay_profile_api.py` & `readarr-py-0.3.0/readarr/api/delay_profile_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -163,15 +163,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "DelayProfileResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/delayprofile', 'POST',
@@ -300,15 +300,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/delayprofile/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -439,15 +439,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "DelayProfileResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/delayprofile/{id}', 'GET',
@@ -573,15 +573,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[DelayProfileResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/delayprofile', 'GET',
@@ -728,15 +728,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "DelayProfileResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/delayprofile/{id}', 'PUT',
@@ -872,15 +872,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/delayprofile/reorder/{id}', 'PUT',
             _path_params,
             _query_params,
```

### Comparing `readarr-py-0.2.2/readarr/api/development_config_api.py` & `readarr-py-0.3.0/readarr/api/development_config_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -149,15 +149,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "DevelopmentConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/development', 'GET',
@@ -290,15 +290,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "DevelopmentConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/development/{id}', 'GET',
@@ -445,15 +445,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "DevelopmentConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/development/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/disk_space_api.py` & `readarr-py-0.3.0/readarr/api/disk_space_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -147,15 +147,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[DiskSpaceResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/diskspace', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/download_client_api.py` & `readarr-py-0.3.0/readarr/api/download_client_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -163,15 +163,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "DownloadClientResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/downloadclient', 'POST',
@@ -314,15 +314,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/downloadclient/action/{name}', 'POST',
             _path_params,
             _query_params,
@@ -449,15 +449,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/downloadclient/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -588,15 +588,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "DownloadClientResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/downloadclient/{id}', 'GET',
@@ -722,15 +722,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[DownloadClientResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/downloadclient', 'GET',
@@ -856,15 +856,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[DownloadClientResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/downloadclient/schema', 'GET',
@@ -1000,15 +1000,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/downloadclient/test', 'POST',
             _path_params,
             _query_params,
@@ -1128,15 +1128,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/downloadclient/testall', 'POST',
             _path_params,
             _query_params,
@@ -1281,15 +1281,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "DownloadClientResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/downloadclient/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/download_client_config_api.py` & `readarr-py-0.3.0/readarr/api/download_client_config_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -149,15 +149,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "DownloadClientConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/downloadclient', 'GET',
@@ -290,15 +290,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "DownloadClientConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/downloadclient/{id}', 'GET',
@@ -445,15 +445,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "DownloadClientConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/downloadclient/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/file_system_api.py` & `readarr-py-0.3.0/readarr/api/file_system_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -165,15 +165,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/filesystem', 'GET',
             _path_params,
             _query_params,
@@ -300,15 +300,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/filesystem/mediafiles', 'GET',
             _path_params,
             _query_params,
@@ -435,15 +435,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/filesystem/type', 'GET',
             _path_params,
             _query_params,
```

### Comparing `readarr-py-0.2.2/readarr/api/health_api.py` & `readarr-py-0.3.0/readarr/api/health_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -156,15 +156,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "HealthResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/health/{id}', 'GET',
@@ -290,15 +290,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[HealthResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/health', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/history_api.py` & `readarr-py-0.3.0/readarr/api/history_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -19,15 +19,15 @@
 
 from datetime import datetime
 
 from pydantic import StrictBool, StrictInt
 
 from typing import List, Optional
 
-from readarr.models.history_event_type import HistoryEventType
+from readarr.models.entity_history_event_type import EntityHistoryEventType
 from readarr.models.history_resource import HistoryResource
 from readarr.models.history_resource_paging_resource import HistoryResourcePagingResource
 
 from readarr.api_client import ApiClient
 from readarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
@@ -43,25 +43,25 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_history_failed(self, body : Optional[StrictInt] = None, **kwargs) -> None:  # noqa: E501
-        """create_history_failed  # noqa: E501
+    def create_history_failed_by_id(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
+        """create_history_failed_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_history_failed(body, async_req=True)
+        >>> thread = api.create_history_failed_by_id(id, async_req=True)
         >>> result = thread.get()
 
-        :param body:
-        :type body: int
+        :param id: (required)
+        :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -70,28 +70,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_history_failed_with_http_info(body, **kwargs)  # noqa: E501
+        return self.create_history_failed_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_history_failed_with_http_info(self, body : Optional[StrictInt] = None, **kwargs):  # noqa: E501
-        """create_history_failed  # noqa: E501
+    def create_history_failed_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """create_history_failed_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_history_failed_with_http_info(body, async_req=True)
+        >>> thread = api.create_history_failed_by_id_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
-        :param body:
-        :type body: int
+        :param id: (required)
+        :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -111,15 +111,15 @@
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'body'
+            'id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -130,53 +130,46 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_history_failed" % _key
+                    " to method create_history_failed_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
+        if _params['id']:
+            _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['body']:
-            _body_params = _params['body']
-
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/history/failed', 'POST',
+            '/api/v1/history/failed/{id}', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -309,15 +302,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "HistoryResourcePagingResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/history', 'GET',
@@ -333,29 +326,29 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_history_author(self, author_id : Optional[StrictInt] = None, book_id : Optional[StrictInt] = None, event_type : Optional[HistoryEventType] = None, include_author : Optional[StrictBool] = None, include_book : Optional[StrictBool] = None, **kwargs) -> List[HistoryResource]:  # noqa: E501
+    def list_history_author(self, author_id : Optional[StrictInt] = None, book_id : Optional[StrictInt] = None, event_type : Optional[EntityHistoryEventType] = None, include_author : Optional[StrictBool] = None, include_book : Optional[StrictBool] = None, **kwargs) -> List[HistoryResource]:  # noqa: E501
         """list_history_author  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_history_author(author_id, book_id, event_type, include_author, include_book, async_req=True)
         >>> result = thread.get()
 
         :param author_id:
         :type author_id: int
         :param book_id:
         :type book_id: int
         :param event_type:
-        :type event_type: HistoryEventType
+        :type event_type: EntityHistoryEventType
         :param include_author:
         :type include_author: bool
         :param include_book:
         :type include_book: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -371,29 +364,29 @@
                  returns the request thread.
         :rtype: List[HistoryResource]
         """
         kwargs['_return_http_data_only'] = True
         return self.list_history_author_with_http_info(author_id, book_id, event_type, include_author, include_book, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_history_author_with_http_info(self, author_id : Optional[StrictInt] = None, book_id : Optional[StrictInt] = None, event_type : Optional[HistoryEventType] = None, include_author : Optional[StrictBool] = None, include_book : Optional[StrictBool] = None, **kwargs):  # noqa: E501
+    def list_history_author_with_http_info(self, author_id : Optional[StrictInt] = None, book_id : Optional[StrictInt] = None, event_type : Optional[EntityHistoryEventType] = None, include_author : Optional[StrictBool] = None, include_book : Optional[StrictBool] = None, **kwargs):  # noqa: E501
         """list_history_author  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_history_author_with_http_info(author_id, book_id, event_type, include_author, include_book, async_req=True)
         >>> result = thread.get()
 
         :param author_id:
         :type author_id: int
         :param book_id:
         :type book_id: int
         :param event_type:
-        :type event_type: HistoryEventType
+        :type event_type: EntityHistoryEventType
         :param include_author:
         :type include_author: bool
         :param include_book:
         :type include_book: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -478,15 +471,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[HistoryResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/history/author', 'GET',
@@ -502,27 +495,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_history_since(self, var_date : Optional[datetime] = None, event_type : Optional[HistoryEventType] = None, include_author : Optional[StrictBool] = None, include_book : Optional[StrictBool] = None, **kwargs) -> List[HistoryResource]:  # noqa: E501
+    def list_history_since(self, var_date : Optional[datetime] = None, event_type : Optional[EntityHistoryEventType] = None, include_author : Optional[StrictBool] = None, include_book : Optional[StrictBool] = None, **kwargs) -> List[HistoryResource]:  # noqa: E501
         """list_history_since  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_history_since(var_date, event_type, include_author, include_book, async_req=True)
         >>> result = thread.get()
 
         :param var_date:
         :type var_date: datetime
         :param event_type:
-        :type event_type: HistoryEventType
+        :type event_type: EntityHistoryEventType
         :param include_author:
         :type include_author: bool
         :param include_book:
         :type include_book: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -538,27 +531,27 @@
                  returns the request thread.
         :rtype: List[HistoryResource]
         """
         kwargs['_return_http_data_only'] = True
         return self.list_history_since_with_http_info(var_date, event_type, include_author, include_book, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_history_since_with_http_info(self, var_date : Optional[datetime] = None, event_type : Optional[HistoryEventType] = None, include_author : Optional[StrictBool] = None, include_book : Optional[StrictBool] = None, **kwargs):  # noqa: E501
+    def list_history_since_with_http_info(self, var_date : Optional[datetime] = None, event_type : Optional[EntityHistoryEventType] = None, include_author : Optional[StrictBool] = None, include_book : Optional[StrictBool] = None, **kwargs):  # noqa: E501
         """list_history_since  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_history_since_with_http_info(var_date, event_type, include_author, include_book, async_req=True)
         >>> result = thread.get()
 
         :param var_date:
         :type var_date: datetime
         :param event_type:
-        :type event_type: HistoryEventType
+        :type event_type: EntityHistoryEventType
         :param include_author:
         :type include_author: bool
         :param include_book:
         :type include_book: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -640,15 +633,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[HistoryResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/history/since', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/host_config_api.py` & `readarr-py-0.3.0/readarr/api/host_config_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -149,15 +149,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "HostConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/host', 'GET',
@@ -290,15 +290,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "HostConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/host/{id}', 'GET',
@@ -445,15 +445,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "HostConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/host/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/import_list_api.py` & `readarr-py-0.3.0/readarr/api/import_list_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -163,15 +163,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "ImportListResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/importlist', 'POST',
@@ -314,15 +314,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/importlist/action/{name}', 'POST',
             _path_params,
             _query_params,
@@ -449,15 +449,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/importlist/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -588,15 +588,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "ImportListResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/importlist/{id}', 'GET',
@@ -722,15 +722,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[ImportListResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/importlist', 'GET',
@@ -856,15 +856,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[ImportListResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/importlist/schema', 'GET',
@@ -1000,15 +1000,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/importlist/test', 'POST',
             _path_params,
             _query_params,
@@ -1128,15 +1128,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/importlist/testall', 'POST',
             _path_params,
             _query_params,
@@ -1281,15 +1281,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "ImportListResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/importlist/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/import_list_exclusion_api.py` & `readarr-py-0.3.0/readarr/api/import_list_exclusion_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -163,15 +163,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "ImportListExclusionResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/importlistexclusion', 'POST',
@@ -300,15 +300,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/importlistexclusion/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -439,15 +439,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "ImportListExclusionResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/importlistexclusion/{id}', 'GET',
@@ -573,15 +573,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[ImportListExclusionResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/importlistexclusion', 'GET',
@@ -728,15 +728,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "ImportListExclusionResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/importlistexclusion/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/indexer_api.py` & `readarr-py-0.3.0/readarr/api/indexer_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -163,15 +163,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "IndexerResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/indexer', 'POST',
@@ -314,15 +314,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/indexer/action/{name}', 'POST',
             _path_params,
             _query_params,
@@ -449,15 +449,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/indexer/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -588,15 +588,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "IndexerResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/indexer/{id}', 'GET',
@@ -722,15 +722,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[IndexerResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/indexer', 'GET',
@@ -856,15 +856,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[IndexerResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/indexer/schema', 'GET',
@@ -1000,15 +1000,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/indexer/test', 'POST',
             _path_params,
             _query_params,
@@ -1128,15 +1128,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/indexer/testall', 'POST',
             _path_params,
             _query_params,
@@ -1281,15 +1281,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "IndexerResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/indexer/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/indexer_config_api.py` & `readarr-py-0.3.0/readarr/api/indexer_config_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -149,15 +149,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "IndexerConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/indexer', 'GET',
@@ -290,15 +290,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "IndexerConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/indexer/{id}', 'GET',
@@ -445,15 +445,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "IndexerConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/indexer/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/initialize_js_api.py` & `readarr-py-0.3.0/readarr/api/initialize_js_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -140,15 +140,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/initialize.js', 'GET',
             _path_params,
             _query_params,
```

### Comparing `readarr-py-0.2.2/readarr/api/language_api.py` & `readarr-py-0.3.0/readarr/api/language_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -156,15 +156,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "LanguageResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/language/{id}', 'GET',
@@ -290,15 +290,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[LanguageResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/language', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/localization_api.py` & `readarr-py-0.3.0/readarr/api/localization_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -144,15 +144,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "str",
         }
 
         return self.api_client.call_api(
             '/api/v1/localization', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/log_api.py` & `readarr-py-0.3.0/readarr/api/log_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -145,15 +145,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "LogResourcePagingResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/log', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/log_file_api.py` & `readarr-py-0.3.0/readarr/api/log_file_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictStr
+from pydantic import constr, validator
 
 from typing import List
 
 from readarr.models.log_file_resource import LogFileResource
 
 from readarr.api_client import ApiClient
 from readarr.exceptions import (  # noqa: F401
@@ -39,15 +39,15 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_log_file_by_filename(self, filename : StrictStr, **kwargs) -> None:  # noqa: E501
+    def get_log_file_by_filename(self, filename : constr(strict=True), **kwargs) -> None:  # noqa: E501
         """get_log_file_by_filename  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_log_file_by_filename(filename, async_req=True)
         >>> result = thread.get()
@@ -69,15 +69,15 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.get_log_file_by_filename_with_http_info(filename, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_log_file_by_filename_with_http_info(self, filename : StrictStr, **kwargs):  # noqa: E501
+    def get_log_file_by_filename_with_http_info(self, filename : constr(strict=True), **kwargs):  # noqa: E501
         """get_log_file_by_filename  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_log_file_by_filename_with_http_info(filename, async_req=True)
         >>> result = thread.get()
@@ -152,15 +152,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/log/file/{filename}', 'GET',
             _path_params,
             _query_params,
@@ -284,15 +284,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[LogFileResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/log/file', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/manual_import_api.py` & `readarr-py-0.3.0/readarr/api/manual_import_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -18,14 +18,15 @@
 from typing_extensions import Annotated
 
 from pydantic import StrictBool, StrictInt, StrictStr, conlist
 
 from typing import List, Optional
 
 from readarr.models.manual_import_resource import ManualImportResource
+from readarr.models.manual_import_update_resource import ManualImportUpdateResource
 
 from readarr.api_client import ApiClient
 from readarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
@@ -39,71 +40,55 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def list_manual_import(self, folder : Optional[StrictStr] = None, download_id : Optional[StrictStr] = None, author_id : Optional[StrictInt] = None, filter_existing_files : Optional[StrictBool] = None, replace_existing_files : Optional[StrictBool] = None, **kwargs) -> List[ManualImportResource]:  # noqa: E501
-        """list_manual_import  # noqa: E501
+    def create_manual_import(self, manual_import_update_resource : Optional[conlist(ManualImportUpdateResource)] = None, **kwargs) -> None:  # noqa: E501
+        """create_manual_import  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_manual_import(folder, download_id, author_id, filter_existing_files, replace_existing_files, async_req=True)
+        >>> thread = api.create_manual_import(manual_import_update_resource, async_req=True)
         >>> result = thread.get()
 
-        :param folder:
-        :type folder: str
-        :param download_id:
-        :type download_id: str
-        :param author_id:
-        :type author_id: int
-        :param filter_existing_files:
-        :type filter_existing_files: bool
-        :param replace_existing_files:
-        :type replace_existing_files: bool
+        :param manual_import_update_resource:
+        :type manual_import_update_resource: List[ManualImportUpdateResource]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: List[ManualImportResource]
+        :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_manual_import_with_http_info(folder, download_id, author_id, filter_existing_files, replace_existing_files, **kwargs)  # noqa: E501
+        return self.create_manual_import_with_http_info(manual_import_update_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_manual_import_with_http_info(self, folder : Optional[StrictStr] = None, download_id : Optional[StrictStr] = None, author_id : Optional[StrictInt] = None, filter_existing_files : Optional[StrictBool] = None, replace_existing_files : Optional[StrictBool] = None, **kwargs):  # noqa: E501
-        """list_manual_import  # noqa: E501
+    def create_manual_import_with_http_info(self, manual_import_update_resource : Optional[conlist(ManualImportUpdateResource)] = None, **kwargs):  # noqa: E501
+        """create_manual_import  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_manual_import_with_http_info(folder, download_id, author_id, filter_existing_files, replace_existing_files, async_req=True)
+        >>> thread = api.create_manual_import_with_http_info(manual_import_update_resource, async_req=True)
         >>> result = thread.get()
 
-        :param folder:
-        :type folder: str
-        :param download_id:
-        :type download_id: str
-        :param author_id:
-        :type author_id: int
-        :param filter_existing_files:
-        :type filter_existing_files: bool
-        :param replace_existing_files:
-        :type replace_existing_files: bool
+        :param manual_import_update_resource:
+        :type manual_import_update_resource: List[ManualImportUpdateResource]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -117,25 +102,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[ManualImportResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'folder',
-            'download_id',
-            'author_id',
-            'filter_existing_files',
-            'replace_existing_files'
+            'manual_import_update_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -146,60 +127,53 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_manual_import" % _key
+                    " to method create_manual_import" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
-        if _params.get('folder') is not None:  # noqa: E501
-            _query_params.append(('folder', _params['folder']))
-        if _params.get('download_id') is not None:  # noqa: E501
-            _query_params.append(('downloadId', _params['download_id']))
-        if _params.get('author_id') is not None:  # noqa: E501
-            _query_params.append(('authorId', _params['author_id']))
-        if _params.get('filter_existing_files') is not None:  # noqa: E501
-            _query_params.append(('filterExistingFiles', _params['filter_existing_files']))
-        if _params.get('replace_existing_files') is not None:  # noqa: E501
-            _query_params.append(('replaceExistingFiles', _params['replace_existing_files']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
+        if _params['manual_import_update_resource']:
+            _body_params = _params['manual_import_update_resource']
 
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json', 'text/json', 'application/*+json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {
-            '200': "List[ManualImportResource]",
-        }
+        _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/manualimport', 'GET',
+            '/api/v1/manualimport', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -208,55 +182,71 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def put_manual_import(self, manual_import_resource : Optional[conlist(ManualImportResource)] = None, **kwargs) -> None:  # noqa: E501
-        """put_manual_import  # noqa: E501
+    def list_manual_import(self, folder : Optional[StrictStr] = None, download_id : Optional[StrictStr] = None, author_id : Optional[StrictInt] = None, filter_existing_files : Optional[StrictBool] = None, replace_existing_files : Optional[StrictBool] = None, **kwargs) -> List[ManualImportResource]:  # noqa: E501
+        """list_manual_import  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.put_manual_import(manual_import_resource, async_req=True)
+        >>> thread = api.list_manual_import(folder, download_id, author_id, filter_existing_files, replace_existing_files, async_req=True)
         >>> result = thread.get()
 
-        :param manual_import_resource:
-        :type manual_import_resource: List[ManualImportResource]
+        :param folder:
+        :type folder: str
+        :param download_id:
+        :type download_id: str
+        :param author_id:
+        :type author_id: int
+        :param filter_existing_files:
+        :type filter_existing_files: bool
+        :param replace_existing_files:
+        :type replace_existing_files: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: List[ManualImportResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.put_manual_import_with_http_info(manual_import_resource, **kwargs)  # noqa: E501
+        return self.list_manual_import_with_http_info(folder, download_id, author_id, filter_existing_files, replace_existing_files, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def put_manual_import_with_http_info(self, manual_import_resource : Optional[conlist(ManualImportResource)] = None, **kwargs):  # noqa: E501
-        """put_manual_import  # noqa: E501
+    def list_manual_import_with_http_info(self, folder : Optional[StrictStr] = None, download_id : Optional[StrictStr] = None, author_id : Optional[StrictInt] = None, filter_existing_files : Optional[StrictBool] = None, replace_existing_files : Optional[StrictBool] = None, **kwargs):  # noqa: E501
+        """list_manual_import  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.put_manual_import_with_http_info(manual_import_resource, async_req=True)
+        >>> thread = api.list_manual_import_with_http_info(folder, download_id, author_id, filter_existing_files, replace_existing_files, async_req=True)
         >>> result = thread.get()
 
-        :param manual_import_resource:
-        :type manual_import_resource: List[ManualImportResource]
+        :param folder:
+        :type folder: str
+        :param download_id:
+        :type download_id: str
+        :param author_id:
+        :type author_id: int
+        :param filter_existing_files:
+        :type filter_existing_files: bool
+        :param replace_existing_files:
+        :type replace_existing_files: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -270,21 +260,25 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: tuple(List[ManualImportResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'manual_import_resource'
+            'folder',
+            'download_id',
+            'author_id',
+            'filter_existing_files',
+            'replace_existing_files'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -295,53 +289,60 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method put_manual_import" % _key
+                    " to method list_manual_import" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
+        if _params.get('folder') is not None:  # noqa: E501
+            _query_params.append(('folder', _params['folder']))
+        if _params.get('download_id') is not None:  # noqa: E501
+            _query_params.append(('downloadId', _params['download_id']))
+        if _params.get('author_id') is not None:  # noqa: E501
+            _query_params.append(('authorId', _params['author_id']))
+        if _params.get('filter_existing_files') is not None:  # noqa: E501
+            _query_params.append(('filterExistingFiles', _params['filter_existing_files']))
+        if _params.get('replace_existing_files') is not None:  # noqa: E501
+            _query_params.append(('replaceExistingFiles', _params['replace_existing_files']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['manual_import_resource']:
-            _body_params = _params['manual_import_resource']
 
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {}
+        _response_types_map = {
+            '200': "List[ManualImportResource]",
+        }
 
         return self.api_client.call_api(
-            '/api/v1/manualimport', 'PUT',
+            '/api/v1/manualimport', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `readarr-py-0.2.2/readarr/api/media_cover_api.py` & `readarr-py-0.3.0/readarr/api/media_cover_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictInt, constr, validator
 
 
 from readarr.api_client import ApiClient
 from readarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
@@ -36,15 +36,15 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_media_cover_authorauthor_id_by_filename(self, author_id : StrictInt, filename : StrictStr, **kwargs) -> None:  # noqa: E501
+    def get_media_cover_authorauthor_id_by_filename(self, author_id : StrictInt, filename : constr(strict=True), **kwargs) -> None:  # noqa: E501
         """get_media_cover_authorauthor_id_by_filename  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_media_cover_authorauthor_id_by_filename(author_id, filename, async_req=True)
         >>> result = thread.get()
@@ -68,15 +68,15 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.get_media_cover_authorauthor_id_by_filename_with_http_info(author_id, filename, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_media_cover_authorauthor_id_by_filename_with_http_info(self, author_id : StrictInt, filename : StrictStr, **kwargs):  # noqa: E501
+    def get_media_cover_authorauthor_id_by_filename_with_http_info(self, author_id : StrictInt, filename : constr(strict=True), **kwargs):  # noqa: E501
         """get_media_cover_authorauthor_id_by_filename  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_media_cover_authorauthor_id_by_filename_with_http_info(author_id, filename, async_req=True)
         >>> result = thread.get()
@@ -156,15 +156,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/mediacover/author/{authorId}/{filename}', 'GET',
             _path_params,
             _query_params,
@@ -178,15 +178,15 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_media_cover_bookbook_id_by_filename(self, book_id : StrictInt, filename : StrictStr, **kwargs) -> None:  # noqa: E501
+    def get_media_cover_bookbook_id_by_filename(self, book_id : StrictInt, filename : constr(strict=True), **kwargs) -> None:  # noqa: E501
         """get_media_cover_bookbook_id_by_filename  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_media_cover_bookbook_id_by_filename(book_id, filename, async_req=True)
         >>> result = thread.get()
@@ -210,15 +210,15 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.get_media_cover_bookbook_id_by_filename_with_http_info(book_id, filename, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_media_cover_bookbook_id_by_filename_with_http_info(self, book_id : StrictInt, filename : StrictStr, **kwargs):  # noqa: E501
+    def get_media_cover_bookbook_id_by_filename_with_http_info(self, book_id : StrictInt, filename : constr(strict=True), **kwargs):  # noqa: E501
         """get_media_cover_bookbook_id_by_filename  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_media_cover_bookbook_id_by_filename_with_http_info(book_id, filename, async_req=True)
         >>> result = thread.get()
@@ -298,15 +298,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/mediacover/book/{bookId}/{filename}', 'GET',
             _path_params,
             _query_params,
```

### Comparing `readarr-py-0.2.2/readarr/api/media_management_config_api.py` & `readarr-py-0.3.0/readarr/api/media_management_config_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -149,15 +149,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "MediaManagementConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/mediamanagement', 'GET',
@@ -290,15 +290,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "MediaManagementConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/mediamanagement/{id}', 'GET',
@@ -445,15 +445,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "MediaManagementConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/mediamanagement/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/metadata_api.py` & `readarr-py-0.3.0/readarr/api/metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -163,15 +163,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "MetadataResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/metadata', 'POST',
@@ -314,15 +314,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/metadata/action/{name}', 'POST',
             _path_params,
             _query_params,
@@ -449,15 +449,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/metadata/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -588,15 +588,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "MetadataResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/metadata/{id}', 'GET',
@@ -722,15 +722,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[MetadataResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/metadata', 'GET',
@@ -856,15 +856,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[MetadataResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/metadata/schema', 'GET',
@@ -1000,15 +1000,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/metadata/test', 'POST',
             _path_params,
             _query_params,
@@ -1128,15 +1128,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/metadata/testall', 'POST',
             _path_params,
             _query_params,
@@ -1281,15 +1281,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "MetadataResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/metadata/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/metadata_profile_api.py` & `readarr-py-0.3.0/readarr/api/metadata_profile_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -163,15 +163,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "MetadataProfileResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/metadataprofile', 'POST',
@@ -300,15 +300,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/metadataprofile/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -439,15 +439,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "MetadataProfileResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/metadataprofile/{id}', 'GET',
@@ -573,15 +573,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[MetadataProfileResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/metadataprofile', 'GET',
@@ -728,15 +728,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "MetadataProfileResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/metadataprofile/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/metadata_profile_schema_api.py` & `readarr-py-0.3.0/readarr/api/metadata_profile_schema_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -145,15 +145,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "MetadataProfileResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/metadataprofile/schema', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/metadata_provider_config_api.py` & `readarr-py-0.3.0/readarr/api/metadata_provider_config_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -149,15 +149,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "MetadataProviderConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/metadataprovider', 'GET',
@@ -290,15 +290,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "MetadataProviderConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/metadataprovider/{id}', 'GET',
@@ -445,15 +445,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "MetadataProviderConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/metadataprovider/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/missing_api.py` & `readarr-py-0.3.0/readarr/api/missing_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -157,15 +157,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "BookResourcePagingResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/wanted/missing', 'GET',
@@ -298,15 +298,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "BookResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/wanted/missing/{id}', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/naming_config_api.py` & `readarr-py-0.3.0/readarr/api/naming_config_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -149,15 +149,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "NamingConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/naming', 'GET',
@@ -290,15 +290,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "NamingConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/naming/{id}', 'GET',
@@ -504,15 +504,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/config/naming/examples', 'GET',
             _path_params,
             _query_params,
@@ -657,15 +657,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "NamingConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/naming/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/notification_api.py` & `readarr-py-0.3.0/readarr/api/notification_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -163,15 +163,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "NotificationResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/notification', 'POST',
@@ -314,15 +314,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/notification/action/{name}', 'POST',
             _path_params,
             _query_params,
@@ -449,15 +449,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/notification/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -588,15 +588,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "NotificationResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/notification/{id}', 'GET',
@@ -722,15 +722,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[NotificationResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/notification', 'GET',
@@ -856,15 +856,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[NotificationResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/notification/schema', 'GET',
@@ -1000,15 +1000,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/notification/test', 'POST',
             _path_params,
             _query_params,
@@ -1128,15 +1128,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/notification/testall', 'POST',
             _path_params,
             _query_params,
@@ -1281,15 +1281,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "NotificationResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/notification/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/parse_api.py` & `readarr-py-0.3.0/readarr/api/parse_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -156,15 +156,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "ParseResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/parse', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/quality_definition_api.py` & `readarr-py-0.3.0/readarr/api/quality_definition_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -156,15 +156,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "QualityDefinitionResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/qualitydefinition/{id}', 'GET',
@@ -290,15 +290,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[QualityDefinitionResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/qualitydefinition', 'GET',
@@ -434,15 +434,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/qualitydefinition/update', 'PUT',
             _path_params,
             _query_params,
@@ -587,15 +587,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "QualityDefinitionResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/qualitydefinition/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/quality_profile_api.py` & `readarr-py-0.3.0/readarr/api/quality_profile_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -163,15 +163,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "QualityProfileResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/qualityprofile', 'POST',
@@ -300,15 +300,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/qualityprofile/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -439,15 +439,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "QualityProfileResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/qualityprofile/{id}', 'GET',
@@ -573,15 +573,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[QualityProfileResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/qualityprofile', 'GET',
@@ -728,15 +728,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "QualityProfileResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/qualityprofile/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/quality_profile_schema_api.py` & `readarr-py-0.3.0/readarr/api/quality_profile_schema_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -145,15 +145,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "QualityProfileResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/qualityprofile/schema', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/queue_action_api.py` & `readarr-py-0.3.0/readarr/api/queue_action_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -159,15 +159,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/queue/grab/bulk', 'POST',
             _path_params,
             _query_params,
@@ -294,15 +294,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/queue/grab/{id}', 'POST',
             _path_params,
             _query_params,
```

### Comparing `readarr-py-0.2.2/readarr/api/queue_api.py` & `readarr-py-0.3.0/readarr/api/queue_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -41,29 +41,29 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def delete_queue(self, id : StrictInt, remove_from_client : Optional[StrictBool] = None, blacklist : Optional[StrictBool] = None, skip_re_download : Optional[StrictBool] = None, **kwargs) -> None:  # noqa: E501
+    def delete_queue(self, id : StrictInt, remove_from_client : Optional[StrictBool] = None, blocklist : Optional[StrictBool] = None, skip_re_download : Optional[StrictBool] = None, **kwargs) -> None:  # noqa: E501
         """delete_queue  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_queue(id, remove_from_client, blacklist, skip_re_download, async_req=True)
+        >>> thread = api.delete_queue(id, remove_from_client, blocklist, skip_re_download, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param remove_from_client:
         :type remove_from_client: bool
-        :param blacklist:
-        :type blacklist: bool
+        :param blocklist:
+        :type blocklist: bool
         :param skip_re_download:
         :type skip_re_download: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -74,32 +74,32 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_queue_with_http_info(id, remove_from_client, blacklist, skip_re_download, **kwargs)  # noqa: E501
+        return self.delete_queue_with_http_info(id, remove_from_client, blocklist, skip_re_download, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_queue_with_http_info(self, id : StrictInt, remove_from_client : Optional[StrictBool] = None, blacklist : Optional[StrictBool] = None, skip_re_download : Optional[StrictBool] = None, **kwargs):  # noqa: E501
+    def delete_queue_with_http_info(self, id : StrictInt, remove_from_client : Optional[StrictBool] = None, blocklist : Optional[StrictBool] = None, skip_re_download : Optional[StrictBool] = None, **kwargs):  # noqa: E501
         """delete_queue  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_queue_with_http_info(id, remove_from_client, blacklist, skip_re_download, async_req=True)
+        >>> thread = api.delete_queue_with_http_info(id, remove_from_client, blocklist, skip_re_download, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param remove_from_client:
         :type remove_from_client: bool
-        :param blacklist:
-        :type blacklist: bool
+        :param blocklist:
+        :type blocklist: bool
         :param skip_re_download:
         :type skip_re_download: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -123,15 +123,15 @@
         """
 
         _params = locals()
 
         _all_params = [
             'id',
             'remove_from_client',
-            'blacklist',
+            'blocklist',
             'skip_re_download'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -159,31 +159,31 @@
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
         if _params.get('remove_from_client') is not None:  # noqa: E501
             _query_params.append(('removeFromClient', _params['remove_from_client']))
-        if _params.get('blacklist') is not None:  # noqa: E501
-            _query_params.append(('blacklist', _params['blacklist']))
+        if _params.get('blocklist') is not None:  # noqa: E501
+            _query_params.append(('blocklist', _params['blocklist']))
         if _params.get('skip_re_download') is not None:  # noqa: E501
             _query_params.append(('skipReDownload', _params['skip_re_download']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/queue/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -197,27 +197,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_queue_bulk(self, remove_from_client : Optional[StrictBool] = None, blacklist : Optional[StrictBool] = None, skip_re_download : Optional[StrictBool] = None, queue_bulk_resource : Optional[QueueBulkResource] = None, **kwargs) -> None:  # noqa: E501
+    def delete_queue_bulk(self, remove_from_client : Optional[StrictBool] = None, blocklist : Optional[StrictBool] = None, skip_re_download : Optional[StrictBool] = None, queue_bulk_resource : Optional[QueueBulkResource] = None, **kwargs) -> None:  # noqa: E501
         """delete_queue_bulk  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_queue_bulk(remove_from_client, blacklist, skip_re_download, queue_bulk_resource, async_req=True)
+        >>> thread = api.delete_queue_bulk(remove_from_client, blocklist, skip_re_download, queue_bulk_resource, async_req=True)
         >>> result = thread.get()
 
         :param remove_from_client:
         :type remove_from_client: bool
-        :param blacklist:
-        :type blacklist: bool
+        :param blocklist:
+        :type blocklist: bool
         :param skip_re_download:
         :type skip_re_download: bool
         :param queue_bulk_resource:
         :type queue_bulk_resource: QueueBulkResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -230,30 +230,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_queue_bulk_with_http_info(remove_from_client, blacklist, skip_re_download, queue_bulk_resource, **kwargs)  # noqa: E501
+        return self.delete_queue_bulk_with_http_info(remove_from_client, blocklist, skip_re_download, queue_bulk_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_queue_bulk_with_http_info(self, remove_from_client : Optional[StrictBool] = None, blacklist : Optional[StrictBool] = None, skip_re_download : Optional[StrictBool] = None, queue_bulk_resource : Optional[QueueBulkResource] = None, **kwargs):  # noqa: E501
+    def delete_queue_bulk_with_http_info(self, remove_from_client : Optional[StrictBool] = None, blocklist : Optional[StrictBool] = None, skip_re_download : Optional[StrictBool] = None, queue_bulk_resource : Optional[QueueBulkResource] = None, **kwargs):  # noqa: E501
         """delete_queue_bulk  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_queue_bulk_with_http_info(remove_from_client, blacklist, skip_re_download, queue_bulk_resource, async_req=True)
+        >>> thread = api.delete_queue_bulk_with_http_info(remove_from_client, blocklist, skip_re_download, queue_bulk_resource, async_req=True)
         >>> result = thread.get()
 
         :param remove_from_client:
         :type remove_from_client: bool
-        :param blacklist:
-        :type blacklist: bool
+        :param blocklist:
+        :type blocklist: bool
         :param skip_re_download:
         :type skip_re_download: bool
         :param queue_bulk_resource:
         :type queue_bulk_resource: QueueBulkResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -278,15 +278,15 @@
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
             'remove_from_client',
-            'blacklist',
+            'blocklist',
             'skip_re_download',
             'queue_bulk_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -313,16 +313,16 @@
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
         if _params.get('remove_from_client') is not None:  # noqa: E501
             _query_params.append(('removeFromClient', _params['remove_from_client']))
-        if _params.get('blacklist') is not None:  # noqa: E501
-            _query_params.append(('blacklist', _params['blacklist']))
+        if _params.get('blocklist') is not None:  # noqa: E501
+            _query_params.append(('blocklist', _params['blocklist']))
         if _params.get('skip_re_download') is not None:  # noqa: E501
             _query_params.append(('skipReDownload', _params['skip_re_download']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
@@ -338,15 +338,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/queue/bulk', 'DELETE',
             _path_params,
             _query_params,
@@ -491,15 +491,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "QueueResourcePagingResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/queue', 'GET',
@@ -632,15 +632,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "QueueResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/queue/{id}', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/queue_details_api.py` & `readarr-py-0.3.0/readarr/api/queue_details_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -156,15 +156,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "QueueResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/queue/details/{id}', 'GET',
@@ -319,15 +319,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[QueueResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/queue/details', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/queue_status_api.py` & `readarr-py-0.3.0/readarr/api/queue_status_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -147,15 +147,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "QueueStatusResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/queue/status', 'GET',
@@ -288,15 +288,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "QueueStatusResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/queue/status/{id}', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/release_api.py` & `readarr-py-0.3.0/readarr/api/release_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -163,15 +163,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "ReleaseResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/release', 'POST',
@@ -304,15 +304,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "ReleaseResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/release/{id}', 'GET',
@@ -452,15 +452,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[ReleaseResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/release', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/release_profile_api.py` & `readarr-py-0.3.0/readarr/api/release_profile_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -163,15 +163,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "ReleaseProfileResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/releaseprofile', 'POST',
@@ -300,15 +300,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/releaseprofile/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -439,15 +439,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "ReleaseProfileResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/releaseprofile/{id}', 'GET',
@@ -573,15 +573,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[ReleaseProfileResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/releaseprofile', 'GET',
@@ -728,15 +728,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "ReleaseProfileResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/releaseprofile/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/release_push_api.py` & `readarr-py-0.3.0/readarr/api/release_push_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -163,15 +163,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "ReleaseResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/release/push', 'POST',
@@ -304,15 +304,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "ReleaseResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/release/push/{id}', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/remote_path_mapping_api.py` & `readarr-py-0.3.0/readarr/api/remote_path_mapping_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -163,15 +163,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "RemotePathMappingResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/remotepathmapping', 'POST',
@@ -300,15 +300,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/remotepathmapping/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -439,15 +439,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "RemotePathMappingResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/remotepathmapping/{id}', 'GET',
@@ -573,15 +573,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[RemotePathMappingResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/remotepathmapping', 'GET',
@@ -728,15 +728,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "RemotePathMappingResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/remotepathmapping/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/rename_book_api.py` & `readarr-py-0.3.0/readarr/api/rename_book_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -163,15 +163,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[RenameBookResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/rename', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/retag_book_api.py` & `readarr-py-0.3.0/readarr/api/retag_book_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -163,15 +163,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[RetagBookResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/retag', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/root_folder_api.py` & `readarr-py-0.3.0/readarr/api/root_folder_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -163,15 +163,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "RootFolderResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/rootfolder', 'POST',
@@ -300,15 +300,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/rootfolder/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -439,15 +439,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "RootFolderResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/rootfolder/{id}', 'GET',
@@ -573,15 +573,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[RootFolderResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/rootfolder', 'GET',
@@ -728,15 +728,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "RootFolderResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/rootfolder/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/search_api.py` & `readarr-py-0.3.0/readarr/api/search_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -151,15 +151,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/search', 'GET',
             _path_params,
             _query_params,
```

### Comparing `readarr-py-0.2.2/readarr/api/series_api.py` & `readarr-py-0.3.0/readarr/api/series_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -156,15 +156,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[SeriesResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/series', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/static_resource_api.py` & `readarr-py-0.3.0/readarr/api/static_resource_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictStr
+from pydantic import StrictStr, constr, validator
 
 
 from readarr.api_client import ApiClient
 from readarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
@@ -149,15 +149,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/', 'GET',
             _path_params,
             _query_params,
@@ -171,15 +171,15 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_by_path(self, path : StrictStr, **kwargs) -> None:  # noqa: E501
+    def get_by_path(self, path : constr(strict=True), **kwargs) -> None:  # noqa: E501
         """get_by_path  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_by_path(path, async_req=True)
         >>> result = thread.get()
@@ -201,15 +201,15 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.get_by_path_with_http_info(path, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_by_path_with_http_info(self, path : StrictStr, **kwargs):  # noqa: E501
+    def get_by_path_with_http_info(self, path : constr(strict=True), **kwargs):  # noqa: E501
         """get_by_path  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_by_path_with_http_info(path, async_req=True)
         >>> result = thread.get()
@@ -284,15 +284,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/{path}', 'GET',
             _path_params,
             _query_params,
@@ -306,15 +306,15 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_content_by_path(self, path : StrictStr, **kwargs) -> None:  # noqa: E501
+    def get_content_by_path(self, path : constr(strict=True), **kwargs) -> None:  # noqa: E501
         """get_content_by_path  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_content_by_path(path, async_req=True)
         >>> result = thread.get()
@@ -336,15 +336,15 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.get_content_by_path_with_http_info(path, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_content_by_path_with_http_info(self, path : StrictStr, **kwargs):  # noqa: E501
+    def get_content_by_path_with_http_info(self, path : constr(strict=True), **kwargs):  # noqa: E501
         """get_content_by_path  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_content_by_path_with_http_info(path, async_req=True)
         >>> result = thread.get()
@@ -419,15 +419,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/content/{path}', 'GET',
             _path_params,
             _query_params,
@@ -547,15 +547,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/login', 'GET',
             _path_params,
             _query_params,
```

### Comparing `readarr-py-0.2.2/readarr/api/system_api.py` & `readarr-py-0.3.0/readarr/api/system_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
+from readarr.models.system_resource import SystemResource
 
 from readarr.api_client import ApiClient
 from readarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
@@ -140,15 +141,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/system/restart', 'POST',
             _path_params,
             _query_params,
@@ -268,15 +269,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/system/shutdown', 'POST',
             _path_params,
             _query_params,
@@ -396,15 +397,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/system/routes', 'GET',
             _path_params,
             _query_params,
@@ -524,15 +525,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/system/routes/duplicate', 'GET',
             _path_params,
             _query_params,
@@ -546,15 +547,15 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_system_status(self, **kwargs) -> None:  # noqa: E501
+    def get_system_status(self, **kwargs) -> SystemResource:  # noqa: E501
         """get_system_status  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_system_status(async_req=True)
         >>> result = thread.get()
@@ -568,15 +569,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: SystemResource
         """
         kwargs['_return_http_data_only'] = True
         return self.get_system_status_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
     def get_system_status_with_http_info(self, **kwargs):  # noqa: E501
         """get_system_status  # noqa: E501
@@ -604,15 +605,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: tuple(SystemResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
@@ -651,18 +652,24 @@
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {}
+        _response_types_map = {
+            '200': "SystemResource",
+        }
 
         return self.api_client.call_api(
             '/api/v1/system/status', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
```

### Comparing `readarr-py-0.2.2/readarr/api/tag_api.py` & `readarr-py-0.3.0/readarr/api/tag_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -163,15 +163,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "TagResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/tag', 'POST',
@@ -300,15 +300,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/tag/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -439,15 +439,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "TagResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/tag/{id}', 'GET',
@@ -573,15 +573,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[TagResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/tag', 'GET',
@@ -728,15 +728,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "TagResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/tag/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/tag_details_api.py` & `readarr-py-0.3.0/readarr/api/tag_details_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -156,15 +156,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "TagDetailsResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/tag/detail/{id}', 'GET',
@@ -290,15 +290,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[TagDetailsResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/tag/detail', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/task_api.py` & `readarr-py-0.3.0/readarr/api/task_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -156,15 +156,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "TaskResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/system/task/{id}', 'GET',
@@ -290,15 +290,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[TaskResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/system/task', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/ui_config_api.py` & `readarr-py-0.3.0/readarr/api/ui_config_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -149,15 +149,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "UiConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/ui', 'GET',
@@ -290,15 +290,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "UiConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/ui/{id}', 'GET',
@@ -445,15 +445,15 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "UiConfigResource",
         }
 
         return self.api_client.call_api(
             '/api/v1/config/ui/{id}', 'PUT',
```

### Comparing `readarr-py-0.2.2/readarr/api/update_api.py` & `readarr-py-0.3.0/readarr/api/update_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -147,15 +147,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[UpdateResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/update', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api/update_log_file_api.py` & `readarr-py-0.3.0/readarr/api/update_log_file_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictStr
+from pydantic import constr, validator
 
 from typing import List
 
 from readarr.models.log_file_resource import LogFileResource
 
 from readarr.api_client import ApiClient
 from readarr.exceptions import (  # noqa: F401
@@ -39,15 +39,15 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_log_file_update_by_filename(self, filename : StrictStr, **kwargs) -> None:  # noqa: E501
+    def get_log_file_update_by_filename(self, filename : constr(strict=True), **kwargs) -> None:  # noqa: E501
         """get_log_file_update_by_filename  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_log_file_update_by_filename(filename, async_req=True)
         >>> result = thread.get()
@@ -69,15 +69,15 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.get_log_file_update_by_filename_with_http_info(filename, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_log_file_update_by_filename_with_http_info(self, filename : StrictStr, **kwargs):  # noqa: E501
+    def get_log_file_update_by_filename_with_http_info(self, filename : constr(strict=True), **kwargs):  # noqa: E501
         """get_log_file_update_by_filename  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_log_file_update_by_filename_with_http_info(filename, async_req=True)
         >>> result = thread.get()
@@ -152,15 +152,15 @@
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/api/v1/log/file/update/{filename}', 'GET',
             _path_params,
             _query_params,
@@ -284,15 +284,15 @@
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = []  # noqa: E501
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[LogFileResource]",
         }
 
         return self.api_client.call_api(
             '/api/v1/log/file/update', 'GET',
```

### Comparing `readarr-py-0.2.2/readarr/api_client.py` & `readarr-py-0.3.0/readarr/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
 import datetime
@@ -74,15 +74,15 @@
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
         # x-release-please-start-version
-        self.user_agent = 'readarr-py/v0.2.2'
+        self.user_agent = 'readarr-py/v0.3.0'
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

### Comparing `readarr-py-0.2.2/readarr/configuration.py` & `readarr-py-0.3.0/readarr/configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import copy
@@ -64,42 +64,64 @@
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
       string values to replace variables in templated server configuration.
       The validation of enums is performed for variables with defined enum values before.
     :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
       in PEM format.
 
+    :Example:
+
+    API Key Authentication Example.
+    Given the following security scheme in the OpenAPI specification:
+      components:
+        securitySchemes:
+          cookieAuth:         # name for the security scheme
+            type: apiKey
+            in: cookie
+            name: JSESSIONID  # cookie name
+
+    You can programmatically set the cookie:
+
+conf = readarr.Configuration(
+    api_key={'cookieAuth': 'abc123'}
+    api_key_prefix={'cookieAuth': 'JSESSIONID'}
+)
+
+    The following cookie will be added to the HTTP request:
+       Cookie: JSESSIONID abc123
     """
 
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
-        self._base_path = "http://localhost" if host is None else host
+        self._base_path = "http://localhost:8787" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
         """Default server index
         """
         self.server_variables = server_variables or {}
@@ -127,14 +149,17 @@
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
         self.logger["package_logger"] = logging.getLogger("readarr")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
@@ -375,40 +400,72 @@
 
     def auth_settings(self):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
         auth = {}
+        if 'X-Api-Key' in self.api_key:
+            auth['X-Api-Key'] = {
+                'type': 'api_key',
+                'in': 'header',
+                'key': 'X-Api-Key',
+                'value': self.get_api_key_with_prefix(
+                    'X-Api-Key',
+                ),
+            }
+        if 'apikey' in self.api_key:
+            auth['apikey'] = {
+                'type': 'api_key',
+                'in': 'query',
+                'key': 'apikey',
+                'value': self.get_api_key_with_prefix(
+                    'apikey',
+                ),
+            }
         return auth
 
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
-               "Version of the API: 0.1.0\n"\
+               "Version of the API: 1.0.0\n"\
                "SDK Package Version: {sdkversion}".\
                format(env=sys.platform, pyversion=sys.version, sdkversion=sdkversion)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
         return [
             {
-                'url': "",
+                'url': "{protocol}://{hostpath}",
                 'description': "No description provided",
+                'variables': {
+                    'protocol': {
+                        'description': "No description provided",
+                        'default_value': "http",
+                        'enum_values': [
+                            "http",
+                            "https"
+                        ]
+                        },
+                    'hostpath': {
+                        'description': "No description provided",
+                        'default_value': "localhost:8787",
+                        }
+                    }
             }
         ]
 
     def get_host_from_settings(self, index, variables=None, servers=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
         :param variables: hash of variable and the corresponding value
```

### Comparing `readarr-py-0.2.2/readarr/exceptions.py` & `readarr-py-0.3.0/readarr/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `readarr-py-0.2.2/readarr/models/__init__.py` & `readarr-py-0.3.0/readarr/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,43 +3,45 @@
 # flake8: noqa
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
 from readarr.models.add_author_options import AddAuthorOptions
 from readarr.models.add_book_options import AddBookOptions
 from readarr.models.allow_fingerprinting import AllowFingerprinting
+from readarr.models.api_info_resource import ApiInfoResource
 from readarr.models.apply_tags import ApplyTags
 from readarr.models.authentication_type import AuthenticationType
 from readarr.models.author import Author
 from readarr.models.author_editor_resource import AuthorEditorResource
 from readarr.models.author_lazy_loaded import AuthorLazyLoaded
 from readarr.models.author_metadata import AuthorMetadata
 from readarr.models.author_metadata_lazy_loaded import AuthorMetadataLazyLoaded
 from readarr.models.author_resource import AuthorResource
 from readarr.models.author_statistics_resource import AuthorStatisticsResource
 from readarr.models.author_status_type import AuthorStatusType
 from readarr.models.author_title_info import AuthorTitleInfo
 from readarr.models.backup_resource import BackupResource
 from readarr.models.backup_type import BackupType
-from readarr.models.blacklist_bulk_resource import BlacklistBulkResource
-from readarr.models.blacklist_resource import BlacklistResource
-from readarr.models.blacklist_resource_paging_resource import BlacklistResourcePagingResource
+from readarr.models.blocklist_bulk_resource import BlocklistBulkResource
+from readarr.models.blocklist_resource import BlocklistResource
+from readarr.models.blocklist_resource_paging_resource import BlocklistResourcePagingResource
 from readarr.models.book import Book
 from readarr.models.book_add_type import BookAddType
+from readarr.models.book_editor_resource import BookEditorResource
 from readarr.models.book_file import BookFile
 from readarr.models.book_file_list_lazy_loaded import BookFileListLazyLoaded
 from readarr.models.book_file_list_resource import BookFileListResource
 from readarr.models.book_file_resource import BookFileResource
 from readarr.models.book_lazy_loaded import BookLazyLoaded
 from readarr.models.book_list_lazy_loaded import BookListLazyLoaded
 from readarr.models.book_resource import BookResource
@@ -51,63 +53,73 @@
 from readarr.models.certificate_validation_type import CertificateValidationType
 from readarr.models.command import Command
 from readarr.models.command_priority import CommandPriority
 from readarr.models.command_resource import CommandResource
 from readarr.models.command_status import CommandStatus
 from readarr.models.command_trigger import CommandTrigger
 from readarr.models.custom_filter_resource import CustomFilterResource
+from readarr.models.custom_format import CustomFormat
+from readarr.models.custom_format_resource import CustomFormatResource
+from readarr.models.custom_format_specification_schema import CustomFormatSpecificationSchema
+from readarr.models.database_type import DatabaseType
 from readarr.models.delay_profile_resource import DelayProfileResource
 from readarr.models.development_config_resource import DevelopmentConfigResource
 from readarr.models.disk_space_resource import DiskSpaceResource
 from readarr.models.download_client_config_resource import DownloadClientConfigResource
 from readarr.models.download_client_resource import DownloadClientResource
 from readarr.models.download_protocol import DownloadProtocol
 from readarr.models.edition import Edition
 from readarr.models.edition_lazy_loaded import EditionLazyLoaded
 from readarr.models.edition_list_lazy_loaded import EditionListLazyLoaded
 from readarr.models.edition_resource import EditionResource
+from readarr.models.entity_history_event_type import EntityHistoryEventType
 from readarr.models.field import Field
 from readarr.models.file_date_type import FileDateType
 from readarr.models.health_check_result import HealthCheckResult
 from readarr.models.health_resource import HealthResource
-from readarr.models.history_event_type import HistoryEventType
 from readarr.models.history_resource import HistoryResource
 from readarr.models.history_resource_paging_resource import HistoryResourcePagingResource
 from readarr.models.host_config_resource import HostConfigResource
+from readarr.models.i_custom_format_specification import ICustomFormatSpecification
 from readarr.models.import_list_exclusion_resource import ImportListExclusionResource
 from readarr.models.import_list_monitor_type import ImportListMonitorType
 from readarr.models.import_list_resource import ImportListResource
 from readarr.models.import_list_type import ImportListType
 from readarr.models.indexer_config_resource import IndexerConfigResource
 from readarr.models.indexer_resource import IndexerResource
 from readarr.models.iso_country import IsoCountry
 from readarr.models.language_resource import LanguageResource
 from readarr.models.links import Links
 from readarr.models.log_file_resource import LogFileResource
 from readarr.models.log_resource import LogResource
 from readarr.models.log_resource_paging_resource import LogResourcePagingResource
 from readarr.models.manual_import_resource import ManualImportResource
+from readarr.models.manual_import_update_resource import ManualImportUpdateResource
 from readarr.models.media_cover import MediaCover
 from readarr.models.media_cover_types import MediaCoverTypes
 from readarr.models.media_info_model import MediaInfoModel
 from readarr.models.media_info_resource import MediaInfoResource
 from readarr.models.media_management_config_resource import MediaManagementConfigResource
 from readarr.models.metadata_profile import MetadataProfile
 from readarr.models.metadata_profile_lazy_loaded import MetadataProfileLazyLoaded
 from readarr.models.metadata_profile_resource import MetadataProfileResource
 from readarr.models.metadata_provider_config_resource import MetadataProviderConfigResource
 from readarr.models.metadata_resource import MetadataResource
 from readarr.models.monitor_types import MonitorTypes
 from readarr.models.monitoring_options import MonitoringOptions
 from readarr.models.naming_config_resource import NamingConfigResource
+from readarr.models.new_item_monitor_types import NewItemMonitorTypes
 from readarr.models.notification_resource import NotificationResource
 from readarr.models.paging_resource_filter import PagingResourceFilter
 from readarr.models.parse_resource import ParseResource
 from readarr.models.parsed_book_info import ParsedBookInfo
 from readarr.models.parsed_track_info import ParsedTrackInfo
+from readarr.models.ping_resource import PingResource
+from readarr.models.profile_format_item import ProfileFormatItem
+from readarr.models.profile_format_item_resource import ProfileFormatItemResource
 from readarr.models.proper_download_types import ProperDownloadTypes
 from readarr.models.provider_message import ProviderMessage
 from readarr.models.provider_message_type import ProviderMessageType
 from readarr.models.proxy_type import ProxyType
 from readarr.models.quality import Quality
 from readarr.models.quality_definition_resource import QualityDefinitionResource
 from readarr.models.quality_model import QualityModel
@@ -127,24 +139,25 @@
 from readarr.models.release_resource import ReleaseResource
 from readarr.models.remote_path_mapping_resource import RemotePathMappingResource
 from readarr.models.rename_book_resource import RenameBookResource
 from readarr.models.rescan_after_refresh_type import RescanAfterRefreshType
 from readarr.models.retag_book_resource import RetagBookResource
 from readarr.models.revision import Revision
 from readarr.models.root_folder_resource import RootFolderResource
+from readarr.models.runtime_mode import RuntimeMode
 from readarr.models.select_option import SelectOption
 from readarr.models.series import Series
 from readarr.models.series_book_link import SeriesBookLink
 from readarr.models.series_book_link_list_lazy_loaded import SeriesBookLinkListLazyLoaded
 from readarr.models.series_book_link_resource import SeriesBookLinkResource
 from readarr.models.series_lazy_loaded import SeriesLazyLoaded
 from readarr.models.series_list_lazy_loaded import SeriesListLazyLoaded
 from readarr.models.series_resource import SeriesResource
 from readarr.models.sort_direction import SortDirection
-from readarr.models.string_int32_key_value_pair import StringInt32KeyValuePair
+from readarr.models.system_resource import SystemResource
 from readarr.models.tag_details_resource import TagDetailsResource
 from readarr.models.tag_difference import TagDifference
 from readarr.models.tag_resource import TagResource
 from readarr.models.task_resource import TaskResource
 from readarr.models.tracked_download_state import TrackedDownloadState
 from readarr.models.tracked_download_status import TrackedDownloadStatus
 from readarr.models.tracked_download_status_message import TrackedDownloadStatusMessage
```

### Comparing `readarr-py-0.2.2/readarr/models/add_author_options.py` & `readarr-py-0.3.0/readarr/models/add_author_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/add_book_options.py` & `readarr-py-0.3.0/readarr/models/add_book_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/allow_fingerprinting.py` & `readarr-py-0.3.0/readarr/models/rescan_after_refresh_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class AllowFingerprinting(str, Enum):
+class RescanAfterRefreshType(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
+    ALWAYS = 'always'
+    AFTERMANUAL = 'afterManual'
     NEVER = 'never'
-    NEWFILES = 'newFiles'
-    ALLFILES = 'allFiles'
```

### Comparing `readarr-py-0.2.2/readarr/models/apply_tags.py` & `readarr-py-0.3.0/readarr/models/apply_tags.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
```

### Comparing `readarr-py-0.2.2/readarr/models/authentication_type.py` & `readarr-py-0.3.0/readarr/models/authentication_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
```

### Comparing `readarr-py-0.2.2/readarr/models/author.py` & `readarr-py-0.3.0/readarr/models/author.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
@@ -18,26 +18,28 @@
 
 from datetime import datetime
 from typing import List, Optional
 from pydantic import BaseModel
 from readarr.models.add_author_options import AddAuthorOptions
 from readarr.models.author_metadata_lazy_loaded import AuthorMetadataLazyLoaded
 from readarr.models.metadata_profile_lazy_loaded import MetadataProfileLazyLoaded
+from readarr.models.new_item_monitor_types import NewItemMonitorTypes
 from readarr.models.quality_profile_lazy_loaded import QualityProfileLazyLoaded
 
 class Author(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     id: Optional[int]
     author_metadata_id: Optional[int]
     clean_name: Optional[str]
     monitored: Optional[bool]
+    monitor_new_items: Optional[NewItemMonitorTypes]
     last_info_sync: Optional[datetime]
     path: Optional[str]
     root_folder_path: Optional[str]
     added: Optional[datetime]
     quality_profile_id: Optional[int]
     metadata_profile_id: Optional[int]
     tags: Optional[List]
@@ -45,15 +47,15 @@
     metadata: Optional[AuthorMetadataLazyLoaded]
     quality_profile: Optional[QualityProfileLazyLoaded]
     metadata_profile: Optional[MetadataProfileLazyLoaded]
     books: Optional[BookListLazyLoaded]
     series: Optional[SeriesListLazyLoaded]
     name: Optional[str]
     foreign_author_id: Optional[str]
-    __properties = ["id", "authorMetadataId", "cleanName", "monitored", "lastInfoSync", "path", "rootFolderPath", "added", "qualityProfileId", "metadataProfileId", "tags", "addOptions", "metadata", "qualityProfile", "metadataProfile", "books", "series", "name", "foreignAuthorId"]
+    __properties = ["id", "authorMetadataId", "cleanName", "monitored", "monitorNewItems", "lastInfoSync", "path", "rootFolderPath", "added", "qualityProfileId", "metadataProfileId", "tags", "addOptions", "metadata", "qualityProfile", "metadataProfile", "books", "series", "name", "foreignAuthorId"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -136,14 +138,15 @@
             return Author.parse_obj(obj)
 
         _obj = Author.parse_obj({
             "id": obj.get("id"),
             "author_metadata_id": obj.get("authorMetadataId"),
             "clean_name": obj.get("cleanName"),
             "monitored": obj.get("monitored"),
+            "monitor_new_items": obj.get("monitorNewItems"),
             "last_info_sync": obj.get("lastInfoSync"),
             "path": obj.get("path"),
             "root_folder_path": obj.get("rootFolderPath"),
             "added": obj.get("added"),
             "quality_profile_id": obj.get("qualityProfileId"),
             "metadata_profile_id": obj.get("metadataProfileId"),
             "tags": obj.get("tags"),
```

### Comparing `readarr-py-0.2.2/readarr/models/author_editor_resource.py` & `readarr-py-0.3.0/readarr/models/author_editor_resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel
 from readarr.models.apply_tags import ApplyTags
+from readarr.models.new_item_monitor_types import NewItemMonitorTypes
 
 class AuthorEditorResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     author_ids: Optional[List]
     monitored: Optional[bool]
+    monitor_new_items: Optional[NewItemMonitorTypes]
     quality_profile_id: Optional[int]
     metadata_profile_id: Optional[int]
     root_folder_path: Optional[str]
     tags: Optional[List]
     apply_tags: Optional[ApplyTags]
     move_files: Optional[bool]
     delete_files: Optional[bool]
-    __properties = ["authorIds", "monitored", "qualityProfileId", "metadataProfileId", "rootFolderPath", "tags", "applyTags", "moveFiles", "deleteFiles"]
+    __properties = ["authorIds", "monitored", "monitorNewItems", "qualityProfileId", "metadataProfileId", "rootFolderPath", "tags", "applyTags", "moveFiles", "deleteFiles"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -99,14 +101,15 @@
 
         if type(obj) is not dict:
             return AuthorEditorResource.parse_obj(obj)
 
         _obj = AuthorEditorResource.parse_obj({
             "author_ids": obj.get("authorIds"),
             "monitored": obj.get("monitored"),
+            "monitor_new_items": obj.get("monitorNewItems"),
             "quality_profile_id": obj.get("qualityProfileId"),
             "metadata_profile_id": obj.get("metadataProfileId"),
             "root_folder_path": obj.get("rootFolderPath"),
             "tags": obj.get("tags"),
             "apply_tags": obj.get("applyTags"),
             "move_files": obj.get("moveFiles"),
             "delete_files": obj.get("deleteFiles")
```

### Comparing `readarr-py-0.2.2/readarr/models/author_lazy_loaded.py` & `readarr-py-0.3.0/readarr/models/author_lazy_loaded.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/author_metadata.py` & `readarr-py-0.3.0/readarr/models/author_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/author_metadata_lazy_loaded.py` & `readarr-py-0.3.0/readarr/models/author_metadata_lazy_loaded.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/author_resource.py` & `readarr-py-0.3.0/readarr/models/author_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
@@ -21,14 +21,15 @@
 from pydantic import BaseModel
 from readarr.models.add_author_options import AddAuthorOptions
 from readarr.models.author_statistics_resource import AuthorStatisticsResource
 from readarr.models.author_status_type import AuthorStatusType
 from readarr.models.book import Book
 from readarr.models.links import Links
 from readarr.models.media_cover import MediaCover
+from readarr.models.new_item_monitor_types import NewItemMonitorTypes
 from readarr.models.ratings import Ratings
 
 class AuthorResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -48,25 +49,26 @@
     last_book: Optional[Book]
     images: Optional[List]
     remote_poster: Optional[str]
     path: Optional[str]
     quality_profile_id: Optional[int]
     metadata_profile_id: Optional[int]
     monitored: Optional[bool]
+    monitor_new_items: Optional[NewItemMonitorTypes]
     root_folder_path: Optional[str]
     genres: Optional[List]
     clean_name: Optional[str]
     sort_name: Optional[str]
     sort_name_last_first: Optional[str]
     tags: Optional[List]
     added: Optional[datetime]
     add_options: Optional[AddAuthorOptions]
     ratings: Optional[Ratings]
     statistics: Optional[AuthorStatisticsResource]
-    __properties = ["id", "authorMetadataId", "status", "ended", "authorName", "authorNameLastFirst", "foreignAuthorId", "titleSlug", "overview", "disambiguation", "links", "nextBook", "lastBook", "images", "remotePoster", "path", "qualityProfileId", "metadataProfileId", "monitored", "rootFolderPath", "genres", "cleanName", "sortName", "sortNameLastFirst", "tags", "added", "addOptions", "ratings", "statistics"]
+    __properties = ["id", "authorMetadataId", "status", "ended", "authorName", "authorNameLastFirst", "foreignAuthorId", "titleSlug", "overview", "disambiguation", "links", "nextBook", "lastBook", "images", "remotePoster", "path", "qualityProfileId", "metadataProfileId", "monitored", "monitorNewItems", "rootFolderPath", "genres", "cleanName", "sortName", "sortNameLastFirst", "tags", "added", "addOptions", "ratings", "statistics"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -212,14 +214,15 @@
             "last_book": Book.from_dict(obj.get("lastBook")) if obj.get("lastBook") is not None else None,
             "images": [MediaCover.from_dict(_item) for _item in obj.get("images")] if obj.get("images") is not None else None,
             "remote_poster": obj.get("remotePoster"),
             "path": obj.get("path"),
             "quality_profile_id": obj.get("qualityProfileId"),
             "metadata_profile_id": obj.get("metadataProfileId"),
             "monitored": obj.get("monitored"),
+            "monitor_new_items": obj.get("monitorNewItems"),
             "root_folder_path": obj.get("rootFolderPath"),
             "genres": obj.get("genres"),
             "clean_name": obj.get("cleanName"),
             "sort_name": obj.get("sortName"),
             "sort_name_last_first": obj.get("sortNameLastFirst"),
             "tags": obj.get("tags"),
             "added": obj.get("added"),
```

### Comparing `readarr-py-0.2.2/readarr/models/author_statistics_resource.py` & `readarr-py-0.3.0/readarr/models/author_statistics_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import Optional, Union
 from pydantic import BaseModel
 
 class AuthorStatisticsResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `readarr-py-0.2.2/readarr/models/author_status_type.py` & `readarr-py-0.3.0/readarr/models/author_status_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
```

### Comparing `readarr-py-0.2.2/readarr/models/author_title_info.py` & `readarr-py-0.3.0/readarr/models/author_title_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/backup_resource.py` & `readarr-py-0.3.0/readarr/models/backup_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
@@ -27,16 +27,17 @@
 
     Do not edit the class manually.
     """
     id: Optional[int]
     name: Optional[str]
     path: Optional[str]
     type: Optional[BackupType]
+    size: Optional[int]
     time: Optional[datetime]
-    __properties = ["id", "name", "path", "type", "time"]
+    __properties = ["id", "name", "path", "type", "size", "time"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -81,11 +82,12 @@
             return BackupResource.parse_obj(obj)
 
         _obj = BackupResource.parse_obj({
             "id": obj.get("id"),
             "name": obj.get("name"),
             "path": obj.get("path"),
             "type": obj.get("type"),
+            "size": obj.get("size"),
             "time": obj.get("time")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/backup_type.py` & `readarr-py-0.3.0/readarr/models/command_trigger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class BackupType(str, Enum):
+class CommandTrigger(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    SCHEDULED = 'scheduled'
+    UNSPECIFIED = 'unspecified'
     MANUAL = 'manual'
-    UPDATE = 'update'
+    SCHEDULED = 'scheduled'
```

### Comparing `readarr-py-0.2.2/readarr/models/blacklist_bulk_resource.py` & `readarr-py-0.3.0/readarr/models/blocklist_bulk_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel
 
-class BlacklistBulkResource(BaseModel):
+class BlocklistBulkResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     ids: Optional[List]
     __properties = ["ids"]
@@ -42,16 +42,16 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> BlacklistBulkResource:
-        """Create an instance of BlacklistBulkResource from a JSON string"""
+    def from_json(cls, json_str: str) -> BlocklistBulkResource:
+        """Create an instance of BlocklistBulkResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -59,20 +59,20 @@
         # set to None if ids (nullable) is None
         if self.ids is None:
             _dict['ids'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> BlacklistBulkResource:
-        """Create an instance of BlacklistBulkResource from a dict"""
+    def from_dict(cls, obj: dict) -> BlocklistBulkResource:
+        """Create an instance of BlocklistBulkResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return BlacklistBulkResource.parse_obj(obj)
+            return BlocklistBulkResource.parse_obj(obj)
 
-        _obj = BlacklistBulkResource.parse_obj({
+        _obj = BlocklistBulkResource.parse_obj({
             "ids": obj.get("ids")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/blacklist_resource.py` & `readarr-py-0.3.0/readarr/models/delay_profile_resource.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
+
 from typing import List, Optional
 from pydantic import BaseModel
-from readarr.models.author_resource import AuthorResource
 from readarr.models.download_protocol import DownloadProtocol
-from readarr.models.quality_model import QualityModel
 
-class BlacklistResource(BaseModel):
+class DelayProfileResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     id: Optional[int]
-    author_id: Optional[int]
-    book_ids: Optional[List]
-    source_title: Optional[str]
-    quality: Optional[QualityModel]
-    var_date: Optional[datetime]
-    protocol: Optional[DownloadProtocol]
-    indexer: Optional[str]
-    message: Optional[str]
-    author: Optional[AuthorResource]
-    __properties = ["id", "authorId", "bookIds", "sourceTitle", "quality", "date", "protocol", "indexer", "message", "author"]
+    enable_usenet: Optional[bool]
+    enable_torrent: Optional[bool]
+    preferred_protocol: Optional[DownloadProtocol]
+    usenet_delay: Optional[int]
+    torrent_delay: Optional[int]
+    bypass_if_highest_quality: Optional[bool]
+    bypass_if_above_custom_format_score: Optional[bool]
+    minimum_custom_format_score: Optional[int]
+    order: Optional[int]
+    tags: Optional[List]
+    __properties = ["id", "enableUsenet", "enableTorrent", "preferredProtocol", "usenetDelay", "torrentDelay", "bypassIfHighestQuality", "bypassIfAboveCustomFormatScore", "minimumCustomFormatScore", "order", "tags"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -54,64 +53,47 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> BlacklistResource:
-        """Create an instance of BlacklistResource from a JSON string"""
+    def from_json(cls, json_str: str) -> DelayProfileResource:
+        """Create an instance of DelayProfileResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of quality
-        if self.quality:
-            _dict['quality'] = self.quality.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of author
-        if self.author:
-            _dict['author'] = self.author.to_dict()
-        # set to None if book_ids (nullable) is None
-        if self.book_ids is None:
-            _dict['bookIds'] = None
-
-        # set to None if source_title (nullable) is None
-        if self.source_title is None:
-            _dict['sourceTitle'] = None
-
-        # set to None if indexer (nullable) is None
-        if self.indexer is None:
-            _dict['indexer'] = None
-
-        # set to None if message (nullable) is None
-        if self.message is None:
-            _dict['message'] = None
+        # set to None if tags (nullable) is None
+        if self.tags is None:
+            _dict['tags'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> BlacklistResource:
-        """Create an instance of BlacklistResource from a dict"""
+    def from_dict(cls, obj: dict) -> DelayProfileResource:
+        """Create an instance of DelayProfileResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return BlacklistResource.parse_obj(obj)
+            return DelayProfileResource.parse_obj(obj)
 
-        _obj = BlacklistResource.parse_obj({
+        _obj = DelayProfileResource.parse_obj({
             "id": obj.get("id"),
-            "author_id": obj.get("authorId"),
-            "book_ids": obj.get("bookIds"),
-            "source_title": obj.get("sourceTitle"),
-            "quality": QualityModel.from_dict(obj.get("quality")) if obj.get("quality") is not None else None,
-            "var_date": obj.get("date"),
-            "protocol": obj.get("protocol"),
-            "indexer": obj.get("indexer"),
-            "message": obj.get("message"),
-            "author": AuthorResource.from_dict(obj.get("author")) if obj.get("author") is not None else None
+            "enable_usenet": obj.get("enableUsenet"),
+            "enable_torrent": obj.get("enableTorrent"),
+            "preferred_protocol": obj.get("preferredProtocol"),
+            "usenet_delay": obj.get("usenetDelay"),
+            "torrent_delay": obj.get("torrentDelay"),
+            "bypass_if_highest_quality": obj.get("bypassIfHighestQuality"),
+            "bypass_if_above_custom_format_score": obj.get("bypassIfAboveCustomFormatScore"),
+            "minimum_custom_format_score": obj.get("minimumCustomFormatScore"),
+            "order": obj.get("order"),
+            "tags": obj.get("tags")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/blacklist_resource_paging_resource.py` & `readarr-py-0.3.0/readarr/models/book_resource_paging_resource.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel
-from readarr.models.blacklist_resource import BlacklistResource
+from readarr.models.book_resource import BookResource
 from readarr.models.paging_resource_filter import PagingResourceFilter
 from readarr.models.sort_direction import SortDirection
 
-class BlacklistResourcePagingResource(BaseModel):
+class BookResourcePagingResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     page: Optional[int]
     page_size: Optional[int]
@@ -51,16 +51,16 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> BlacklistResourcePagingResource:
-        """Create an instance of BlacklistResourcePagingResource from a JSON string"""
+    def from_json(cls, json_str: str) -> BookResourcePagingResource:
+        """Create an instance of BookResourcePagingResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -90,26 +90,26 @@
         # set to None if records (nullable) is None
         if self.records is None:
             _dict['records'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> BlacklistResourcePagingResource:
-        """Create an instance of BlacklistResourcePagingResource from a dict"""
+    def from_dict(cls, obj: dict) -> BookResourcePagingResource:
+        """Create an instance of BookResourcePagingResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return BlacklistResourcePagingResource.parse_obj(obj)
+            return BookResourcePagingResource.parse_obj(obj)
 
-        _obj = BlacklistResourcePagingResource.parse_obj({
+        _obj = BookResourcePagingResource.parse_obj({
             "page": obj.get("page"),
             "page_size": obj.get("pageSize"),
             "sort_key": obj.get("sortKey"),
             "sort_direction": obj.get("sortDirection"),
             "filters": [PagingResourceFilter.from_dict(_item) for _item in obj.get("filters")] if obj.get("filters") is not None else None,
             "total_records": obj.get("totalRecords"),
-            "records": [BlacklistResource.from_dict(_item) for _item in obj.get("records")] if obj.get("records") is not None else None
+            "records": [BookResource.from_dict(_item) for _item in obj.get("records")] if obj.get("records") is not None else None
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/book.py` & `readarr-py-0.3.0/readarr/models/book.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
@@ -34,27 +34,28 @@
     author_metadata_id: Optional[int]
     foreign_book_id: Optional[str]
     title_slug: Optional[str]
     title: Optional[str]
     release_date: Optional[datetime]
     links: Optional[List]
     genres: Optional[List]
+    related_books: Optional[List]
     ratings: Optional[Ratings]
     clean_title: Optional[str]
     monitored: Optional[bool]
     any_edition_ok: Optional[bool]
     last_info_sync: Optional[datetime]
     added: Optional[datetime]
     add_options: Optional[AddBookOptions]
     author_metadata: Optional[AuthorMetadataLazyLoaded]
     author: Optional[AuthorLazyLoaded]
     editions: Optional[EditionListLazyLoaded]
     book_files: Optional[BookFileListLazyLoaded]
     series_links: Optional[SeriesBookLinkListLazyLoaded]
-    __properties = ["id", "authorMetadataId", "foreignBookId", "titleSlug", "title", "releaseDate", "links", "genres", "ratings", "cleanTitle", "monitored", "anyEditionOk", "lastInfoSync", "added", "addOptions", "authorMetadata", "author", "editions", "bookFiles", "seriesLinks"]
+    __properties = ["id", "authorMetadataId", "foreignBookId", "titleSlug", "title", "releaseDate", "links", "genres", "relatedBooks", "ratings", "cleanTitle", "monitored", "anyEditionOk", "lastInfoSync", "added", "addOptions", "authorMetadata", "author", "editions", "bookFiles", "seriesLinks"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -127,14 +128,18 @@
         if self.links is None:
             _dict['links'] = None
 
         # set to None if genres (nullable) is None
         if self.genres is None:
             _dict['genres'] = None
 
+        # set to None if related_books (nullable) is None
+        if self.related_books is None:
+            _dict['relatedBooks'] = None
+
         # set to None if clean_title (nullable) is None
         if self.clean_title is None:
             _dict['cleanTitle'] = None
 
         # set to None if last_info_sync (nullable) is None
         if self.last_info_sync is None:
             _dict['lastInfoSync'] = None
@@ -155,14 +160,15 @@
             "author_metadata_id": obj.get("authorMetadataId"),
             "foreign_book_id": obj.get("foreignBookId"),
             "title_slug": obj.get("titleSlug"),
             "title": obj.get("title"),
             "release_date": obj.get("releaseDate"),
             "links": [Links.from_dict(_item) for _item in obj.get("links")] if obj.get("links") is not None else None,
             "genres": obj.get("genres"),
+            "related_books": obj.get("relatedBooks"),
             "ratings": Ratings.from_dict(obj.get("ratings")) if obj.get("ratings") is not None else None,
             "clean_title": obj.get("cleanTitle"),
             "monitored": obj.get("monitored"),
             "any_edition_ok": obj.get("anyEditionOk"),
             "last_info_sync": obj.get("lastInfoSync"),
             "added": obj.get("added"),
             "add_options": AddBookOptions.from_dict(obj.get("addOptions")) if obj.get("addOptions") is not None else None,
```

### Comparing `readarr-py-0.2.2/readarr/models/book_add_type.py` & `readarr-py-0.3.0/readarr/models/book_add_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
```

### Comparing `readarr-py-0.2.2/readarr/models/book_file.py` & `readarr-py-0.3.0/readarr/models/book_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
@@ -29,25 +29,26 @@
     Do not edit the class manually.
     """
     id: Optional[int]
     path: Optional[str]
     size: Optional[int]
     modified: Optional[datetime]
     date_added: Optional[datetime]
+    original_file_path: Optional[str]
     scene_name: Optional[str]
     release_group: Optional[str]
     quality: Optional[QualityModel]
     media_info: Optional[MediaInfoModel]
     edition_id: Optional[int]
     calibre_id: Optional[int]
     part: Optional[int]
     author: Optional[AuthorLazyLoaded]
     edition: Optional[EditionLazyLoaded]
     part_count: Optional[int]
-    __properties = ["id", "path", "size", "modified", "dateAdded", "sceneName", "releaseGroup", "quality", "mediaInfo", "editionId", "calibreId", "part", "author", "edition", "partCount"]
+    __properties = ["id", "path", "size", "modified", "dateAdded", "originalFilePath", "sceneName", "releaseGroup", "quality", "mediaInfo", "editionId", "calibreId", "part", "author", "edition", "partCount"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -84,14 +85,18 @@
         # override the default output from pydantic by calling `to_dict()` of edition
         if self.edition:
             _dict['edition'] = self.edition.to_dict()
         # set to None if path (nullable) is None
         if self.path is None:
             _dict['path'] = None
 
+        # set to None if original_file_path (nullable) is None
+        if self.original_file_path is None:
+            _dict['originalFilePath'] = None
+
         # set to None if scene_name (nullable) is None
         if self.scene_name is None:
             _dict['sceneName'] = None
 
         # set to None if release_group (nullable) is None
         if self.release_group is None:
             _dict['releaseGroup'] = None
@@ -109,14 +114,15 @@
 
         _obj = BookFile.parse_obj({
             "id": obj.get("id"),
             "path": obj.get("path"),
             "size": obj.get("size"),
             "modified": obj.get("modified"),
             "date_added": obj.get("dateAdded"),
+            "original_file_path": obj.get("originalFilePath"),
             "scene_name": obj.get("sceneName"),
             "release_group": obj.get("releaseGroup"),
             "quality": QualityModel.from_dict(obj.get("quality")) if obj.get("quality") is not None else None,
             "media_info": MediaInfoModel.from_dict(obj.get("mediaInfo")) if obj.get("mediaInfo") is not None else None,
             "edition_id": obj.get("editionId"),
             "calibre_id": obj.get("calibreId"),
             "part": obj.get("part"),
```

### Comparing `readarr-py-0.2.2/readarr/models/book_file_list_lazy_loaded.py` & `readarr-py-0.3.0/readarr/models/book_file_list_lazy_loaded.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel
-from readarr.models.book_file import BookFile
 
 class BookFileListLazyLoaded(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
```

### Comparing `readarr-py-0.2.2/readarr/models/book_file_list_resource.py` & `readarr-py-0.3.0/readarr/models/book_file_list_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/book_file_resource.py` & `readarr-py-0.3.0/readarr/models/book_file_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/book_lazy_loaded.py` & `readarr-py-0.3.0/readarr/models/book_lazy_loaded.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/book_list_lazy_loaded.py` & `readarr-py-0.3.0/readarr/models/book_list_lazy_loaded.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel
-from readarr.models.book import Book
 
 class BookListLazyLoaded(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
```

### Comparing `readarr-py-0.2.2/readarr/models/book_resource.py` & `readarr-py-0.3.0/readarr/models/book_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/book_resource_paging_resource.py` & `readarr-py-0.3.0/readarr/models/queue_resource_paging_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel
-from readarr.models.book_resource import BookResource
 from readarr.models.paging_resource_filter import PagingResourceFilter
+from readarr.models.queue_resource import QueueResource
 from readarr.models.sort_direction import SortDirection
 
-class BookResourcePagingResource(BaseModel):
+class QueueResourcePagingResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     page: Optional[int]
     page_size: Optional[int]
@@ -51,16 +51,16 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> BookResourcePagingResource:
-        """Create an instance of BookResourcePagingResource from a JSON string"""
+    def from_json(cls, json_str: str) -> QueueResourcePagingResource:
+        """Create an instance of QueueResourcePagingResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -90,26 +90,26 @@
         # set to None if records (nullable) is None
         if self.records is None:
             _dict['records'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> BookResourcePagingResource:
-        """Create an instance of BookResourcePagingResource from a dict"""
+    def from_dict(cls, obj: dict) -> QueueResourcePagingResource:
+        """Create an instance of QueueResourcePagingResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return BookResourcePagingResource.parse_obj(obj)
+            return QueueResourcePagingResource.parse_obj(obj)
 
-        _obj = BookResourcePagingResource.parse_obj({
+        _obj = QueueResourcePagingResource.parse_obj({
             "page": obj.get("page"),
             "page_size": obj.get("pageSize"),
             "sort_key": obj.get("sortKey"),
             "sort_direction": obj.get("sortDirection"),
             "filters": [PagingResourceFilter.from_dict(_item) for _item in obj.get("filters")] if obj.get("filters") is not None else None,
             "total_records": obj.get("totalRecords"),
-            "records": [BookResource.from_dict(_item) for _item in obj.get("records")] if obj.get("records") is not None else None
+            "records": [QueueResource.from_dict(_item) for _item in obj.get("records")] if obj.get("records") is not None else None
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/book_statistics_resource.py` & `readarr-py-0.3.0/readarr/models/book_statistics_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import Optional, Union
 from pydantic import BaseModel
 
 class BookStatisticsResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `readarr-py-0.2.2/readarr/models/books_monitored_resource.py` & `readarr-py-0.3.0/readarr/models/books_monitored_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/bookshelf_author_resource.py` & `readarr-py-0.3.0/readarr/models/bookshelf_author_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/bookshelf_resource.py` & `readarr-py-0.3.0/readarr/models/bookshelf_resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
@@ -17,24 +17,26 @@
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel
 from readarr.models.bookshelf_author_resource import BookshelfAuthorResource
 from readarr.models.monitoring_options import MonitoringOptions
+from readarr.models.new_item_monitor_types import NewItemMonitorTypes
 
 class BookshelfResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     authors: Optional[List]
     monitoring_options: Optional[MonitoringOptions]
-    __properties = ["authors", "monitoringOptions"]
+    monitor_new_items: Optional[NewItemMonitorTypes]
+    __properties = ["authors", "monitoringOptions", "monitorNewItems"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -82,11 +84,12 @@
             return None
 
         if type(obj) is not dict:
             return BookshelfResource.parse_obj(obj)
 
         _obj = BookshelfResource.parse_obj({
             "authors": [BookshelfAuthorResource.from_dict(_item) for _item in obj.get("authors")] if obj.get("authors") is not None else None,
-            "monitoring_options": MonitoringOptions.from_dict(obj.get("monitoringOptions")) if obj.get("monitoringOptions") is not None else None
+            "monitoring_options": MonitoringOptions.from_dict(obj.get("monitoringOptions")) if obj.get("monitoringOptions") is not None else None,
+            "monitor_new_items": obj.get("monitorNewItems")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/certificate_validation_type.py` & `readarr-py-0.3.0/readarr/models/import_list_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class CertificateValidationType(str, Enum):
+class ImportListType(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    ENABLED = 'enabled'
-    DISABLEDFORLOCALADDRESSES = 'disabledForLocalAddresses'
-    DISABLED = 'disabled'
+    PROGRAM = 'program'
+    GOODREADS = 'goodreads'
+    OTHER = 'other'
```

### Comparing `readarr-py-0.2.2/readarr/models/command.py` & `readarr-py-0.3.0/readarr/models/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
@@ -29,21 +29,22 @@
     """
     send_updates_to_client: Optional[bool]
     update_scheduled_task: Optional[bool]
     completion_message: Optional[str]
     requires_disk_access: Optional[bool]
     is_exclusive: Optional[bool]
     is_type_exclusive: Optional[bool]
+    is_long_running: Optional[bool]
     name: Optional[str]
     last_execution_time: Optional[datetime]
     last_start_time: Optional[datetime]
     trigger: Optional[CommandTrigger]
     suppress_messages: Optional[bool]
     client_user_agent: Optional[str]
-    __properties = ["sendUpdatesToClient", "updateScheduledTask", "completionMessage", "requiresDiskAccess", "isExclusive", "isTypeExclusive", "name", "lastExecutionTime", "lastStartTime", "trigger", "suppressMessages", "clientUserAgent"]
+    __properties = ["sendUpdatesToClient", "updateScheduledTask", "completionMessage", "requiresDiskAccess", "isExclusive", "isTypeExclusive", "isLongRunning", "name", "lastExecutionTime", "lastStartTime", "trigger", "suppressMessages", "clientUserAgent"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -67,14 +68,15 @@
         _dict = self.dict(by_alias=True,
                           exclude={
                             "update_scheduled_task",
                             "completion_message",
                             "requires_disk_access",
                             "is_exclusive",
                             "is_type_exclusive",
+                            "is_long_running",
                             "name",
                           },
                           exclude_none=True)
         # set to None if completion_message (nullable) is None
         if self.completion_message is None:
             _dict['completionMessage'] = None
 
@@ -108,14 +110,15 @@
         _obj = Command.parse_obj({
             "send_updates_to_client": obj.get("sendUpdatesToClient"),
             "update_scheduled_task": obj.get("updateScheduledTask"),
             "completion_message": obj.get("completionMessage"),
             "requires_disk_access": obj.get("requiresDiskAccess"),
             "is_exclusive": obj.get("isExclusive"),
             "is_type_exclusive": obj.get("isTypeExclusive"),
+            "is_long_running": obj.get("isLongRunning"),
             "name": obj.get("name"),
             "last_execution_time": obj.get("lastExecutionTime"),
             "last_start_time": obj.get("lastStartTime"),
             "trigger": obj.get("trigger"),
             "suppress_messages": obj.get("suppressMessages"),
             "client_user_agent": obj.get("clientUserAgent")
         })
```

### Comparing `readarr-py-0.2.2/readarr/models/command_priority.py` & `readarr-py-0.3.0/readarr/models/rejection_type.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class CommandPriority(str, Enum):
+class RejectionType(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    NORMAL = 'normal'
-    HIGH = 'high'
-    LOW = 'low'
+    PERMANENT = 'permanent'
+    TEMPORARY = 'temporary'
```

### Comparing `readarr-py-0.2.2/readarr/models/command_resource.py` & `readarr-py-0.3.0/readarr/models/command_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/command_status.py` & `readarr-py-0.3.0/readarr/models/command_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
```

### Comparing `readarr-py-0.2.2/readarr/models/command_trigger.py` & `readarr-py-0.3.0/readarr/models/download_protocol.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class CommandTrigger(str, Enum):
+class DownloadProtocol(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    UNSPECIFIED = 'unspecified'
-    MANUAL = 'manual'
-    SCHEDULED = 'scheduled'
+    UNKNOWN = 'unknown'
+    USENET = 'usenet'
+    TORRENT = 'torrent'
```

### Comparing `readarr-py-0.2.2/readarr/models/custom_filter_resource.py` & `readarr-py-0.3.0/readarr/models/custom_filter_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/delay_profile_resource.py` & `readarr-py-0.3.0/readarr/models/release_profile_resource.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel
-from readarr.models.download_protocol import DownloadProtocol
 
-class DelayProfileResource(BaseModel):
+class ReleaseProfileResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     id: Optional[int]
-    enable_usenet: Optional[bool]
-    enable_torrent: Optional[bool]
-    preferred_protocol: Optional[DownloadProtocol]
-    usenet_delay: Optional[int]
-    torrent_delay: Optional[int]
-    order: Optional[int]
+    enabled: Optional[bool]
+    required: Optional[List]
+    ignored: Optional[List]
+    indexer_id: Optional[int]
     tags: Optional[List]
-    __properties = ["id", "enableUsenet", "enableTorrent", "preferredProtocol", "usenetDelay", "torrentDelay", "order", "tags"]
+    __properties = ["id", "enabled", "required", "ignored", "indexerId", "tags"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -50,44 +47,50 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> DelayProfileResource:
-        """Create an instance of DelayProfileResource from a JSON string"""
+    def from_json(cls, json_str: str) -> ReleaseProfileResource:
+        """Create an instance of ReleaseProfileResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # set to None if required (nullable) is None
+        if self.required is None:
+            _dict['required'] = None
+
+        # set to None if ignored (nullable) is None
+        if self.ignored is None:
+            _dict['ignored'] = None
+
         # set to None if tags (nullable) is None
         if self.tags is None:
             _dict['tags'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> DelayProfileResource:
-        """Create an instance of DelayProfileResource from a dict"""
+    def from_dict(cls, obj: dict) -> ReleaseProfileResource:
+        """Create an instance of ReleaseProfileResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return DelayProfileResource.parse_obj(obj)
+            return ReleaseProfileResource.parse_obj(obj)
 
-        _obj = DelayProfileResource.parse_obj({
+        _obj = ReleaseProfileResource.parse_obj({
             "id": obj.get("id"),
-            "enable_usenet": obj.get("enableUsenet"),
-            "enable_torrent": obj.get("enableTorrent"),
-            "preferred_protocol": obj.get("preferredProtocol"),
-            "usenet_delay": obj.get("usenetDelay"),
-            "torrent_delay": obj.get("torrentDelay"),
-            "order": obj.get("order"),
+            "enabled": obj.get("enabled"),
+            "required": obj.get("required"),
+            "ignored": obj.get("ignored"),
+            "indexer_id": obj.get("indexerId"),
             "tags": obj.get("tags")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/development_config_resource.py` & `readarr-py-0.3.0/readarr/models/development_config_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/disk_space_resource.py` & `readarr-py-0.3.0/readarr/models/disk_space_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/download_client_config_resource.py` & `readarr-py-0.3.0/readarr/models/download_client_config_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/download_client_resource.py` & `readarr-py-0.3.0/readarr/models/download_client_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/download_protocol.py` & `readarr-py-0.3.0/readarr/models/provider_message_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class DownloadProtocol(str, Enum):
+class ProviderMessageType(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    UNKNOWN = 'unknown'
-    USENET = 'usenet'
-    TORRENT = 'torrent'
+    INFO = 'info'
+    WARNING = 'warning'
+    ERROR = 'error'
```

### Comparing `readarr-py-0.2.2/readarr/models/edition.py` & `readarr-py-0.3.0/readarr/models/edition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/edition_lazy_loaded.py` & `readarr-py-0.3.0/readarr/models/edition_lazy_loaded.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/edition_list_lazy_loaded.py` & `readarr-py-0.3.0/readarr/models/edition_list_lazy_loaded.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel
-from readarr.models.edition import Edition
 
 class EditionListLazyLoaded(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
```

### Comparing `readarr-py-0.2.2/readarr/models/edition_resource.py` & `readarr-py-0.3.0/readarr/models/edition_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/field.py` & `readarr-py-0.3.0/readarr/models/field.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
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

### Comparing `readarr-py-0.2.2/readarr/models/file_date_type.py` & `readarr-py-0.3.0/readarr/models/file_date_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
```

### Comparing `readarr-py-0.2.2/readarr/models/health_check_result.py` & `readarr-py-0.3.0/readarr/models/backup_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class HealthCheckResult(str, Enum):
+class BackupType(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    OK = 'ok'
-    NOTICE = 'notice'
-    WARNING = 'warning'
-    ERROR = 'error'
+    SCHEDULED = 'scheduled'
+    MANUAL = 'manual'
+    UPDATE = 'update'
```

### Comparing `readarr-py-0.2.2/readarr/models/health_resource.py` & `readarr-py-0.3.0/readarr/models/health_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/history_resource.py` & `readarr-py-0.3.0/readarr/models/blocklist_resource.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import Dict, Optional
+from typing import List, Optional
 from pydantic import BaseModel
 from readarr.models.author_resource import AuthorResource
-from readarr.models.book_resource import BookResource
-from readarr.models.history_event_type import HistoryEventType
+from readarr.models.custom_format_resource import CustomFormatResource
+from readarr.models.download_protocol import DownloadProtocol
 from readarr.models.quality_model import QualityModel
 
-class HistoryResource(BaseModel):
+class BlocklistResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     id: Optional[int]
-    book_id: Optional[int]
     author_id: Optional[int]
+    book_ids: Optional[List]
     source_title: Optional[str]
     quality: Optional[QualityModel]
-    quality_cutoff_not_met: Optional[bool]
+    custom_formats: Optional[List]
     var_date: Optional[datetime]
-    download_id: Optional[str]
-    event_type: Optional[HistoryEventType]
-    data: Optional[Dict]
-    book: Optional[BookResource]
+    protocol: Optional[DownloadProtocol]
+    indexer: Optional[str]
+    message: Optional[str]
     author: Optional[AuthorResource]
-    __properties = ["id", "bookId", "authorId", "sourceTitle", "quality", "qualityCutoffNotMet", "date", "downloadId", "eventType", "data", "book", "author"]
+    __properties = ["id", "authorId", "bookIds", "sourceTitle", "quality", "customFormats", "date", "protocol", "indexer", "message", "author"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -57,65 +56,76 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> HistoryResource:
-        """Create an instance of HistoryResource from a JSON string"""
+    def from_json(cls, json_str: str) -> BlocklistResource:
+        """Create an instance of BlocklistResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of quality
         if self.quality:
             _dict['quality'] = self.quality.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of book
-        if self.book:
-            _dict['book'] = self.book.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in custom_formats (list)
+        _items = []
+        if self.custom_formats:
+            for _item in self.custom_formats:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['customFormats'] = _items
         # override the default output from pydantic by calling `to_dict()` of author
         if self.author:
             _dict['author'] = self.author.to_dict()
+        # set to None if book_ids (nullable) is None
+        if self.book_ids is None:
+            _dict['bookIds'] = None
+
         # set to None if source_title (nullable) is None
         if self.source_title is None:
             _dict['sourceTitle'] = None
 
-        # set to None if download_id (nullable) is None
-        if self.download_id is None:
-            _dict['downloadId'] = None
-
-        # set to None if data (nullable) is None
-        if self.data is None:
-            _dict['data'] = None
+        # set to None if custom_formats (nullable) is None
+        if self.custom_formats is None:
+            _dict['customFormats'] = None
+
+        # set to None if indexer (nullable) is None
+        if self.indexer is None:
+            _dict['indexer'] = None
+
+        # set to None if message (nullable) is None
+        if self.message is None:
+            _dict['message'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> HistoryResource:
-        """Create an instance of HistoryResource from a dict"""
+    def from_dict(cls, obj: dict) -> BlocklistResource:
+        """Create an instance of BlocklistResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return HistoryResource.parse_obj(obj)
+            return BlocklistResource.parse_obj(obj)
 
-        _obj = HistoryResource.parse_obj({
+        _obj = BlocklistResource.parse_obj({
             "id": obj.get("id"),
-            "book_id": obj.get("bookId"),
             "author_id": obj.get("authorId"),
+            "book_ids": obj.get("bookIds"),
             "source_title": obj.get("sourceTitle"),
             "quality": QualityModel.from_dict(obj.get("quality")) if obj.get("quality") is not None else None,
-            "quality_cutoff_not_met": obj.get("qualityCutoffNotMet"),
+            "custom_formats": [CustomFormatResource.from_dict(_item) for _item in obj.get("customFormats")] if obj.get("customFormats") is not None else None,
             "var_date": obj.get("date"),
-            "download_id": obj.get("downloadId"),
-            "event_type": obj.get("eventType"),
-            "data": obj.get("data"),
-            "book": BookResource.from_dict(obj.get("book")) if obj.get("book") is not None else None,
+            "protocol": obj.get("protocol"),
+            "indexer": obj.get("indexer"),
+            "message": obj.get("message"),
             "author": AuthorResource.from_dict(obj.get("author")) if obj.get("author") is not None else None
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/history_resource_paging_resource.py` & `readarr-py-0.3.0/readarr/models/history_resource_paging_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/host_config_resource.py` & `readarr-py-0.3.0/readarr/models/host_config_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
@@ -43,14 +43,16 @@
     log_level: Optional[str]
     console_log_level: Optional[str]
     branch: Optional[str]
     api_key: Optional[str]
     ssl_cert_path: Optional[str]
     ssl_cert_password: Optional[str]
     url_base: Optional[str]
+    instance_name: Optional[str]
+    application_url: Optional[str]
     update_automatically: Optional[bool]
     update_mechanism: Optional[UpdateMechanism]
     update_script_path: Optional[str]
     proxy_enabled: Optional[bool]
     proxy_type: Optional[ProxyType]
     proxy_hostname: Optional[str]
     proxy_port: Optional[int]
@@ -58,15 +60,15 @@
     proxy_password: Optional[str]
     proxy_bypass_filter: Optional[str]
     proxy_bypass_local_addresses: Optional[bool]
     certificate_validation: Optional[CertificateValidationType]
     backup_folder: Optional[str]
     backup_interval: Optional[int]
     backup_retention: Optional[int]
-    __properties = ["id", "bindAddress", "port", "sslPort", "enableSsl", "launchBrowser", "authenticationMethod", "analyticsEnabled", "username", "password", "logLevel", "consoleLogLevel", "branch", "apiKey", "sslCertPath", "sslCertPassword", "urlBase", "updateAutomatically", "updateMechanism", "updateScriptPath", "proxyEnabled", "proxyType", "proxyHostname", "proxyPort", "proxyUsername", "proxyPassword", "proxyBypassFilter", "proxyBypassLocalAddresses", "certificateValidation", "backupFolder", "backupInterval", "backupRetention"]
+    __properties = ["id", "bindAddress", "port", "sslPort", "enableSsl", "launchBrowser", "authenticationMethod", "analyticsEnabled", "username", "password", "logLevel", "consoleLogLevel", "branch", "apiKey", "sslCertPath", "sslCertPassword", "urlBase", "instanceName", "applicationUrl", "updateAutomatically", "updateMechanism", "updateScriptPath", "proxyEnabled", "proxyType", "proxyHostname", "proxyPort", "proxyUsername", "proxyPassword", "proxyBypassFilter", "proxyBypassLocalAddresses", "certificateValidation", "backupFolder", "backupInterval", "backupRetention"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -127,14 +129,22 @@
         if self.ssl_cert_password is None:
             _dict['sslCertPassword'] = None
 
         # set to None if url_base (nullable) is None
         if self.url_base is None:
             _dict['urlBase'] = None
 
+        # set to None if instance_name (nullable) is None
+        if self.instance_name is None:
+            _dict['instanceName'] = None
+
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
@@ -180,14 +190,16 @@
             "log_level": obj.get("logLevel"),
             "console_log_level": obj.get("consoleLogLevel"),
             "branch": obj.get("branch"),
             "api_key": obj.get("apiKey"),
             "ssl_cert_path": obj.get("sslCertPath"),
             "ssl_cert_password": obj.get("sslCertPassword"),
             "url_base": obj.get("urlBase"),
+            "instance_name": obj.get("instanceName"),
+            "application_url": obj.get("applicationUrl"),
             "update_automatically": obj.get("updateAutomatically"),
             "update_mechanism": obj.get("updateMechanism"),
             "update_script_path": obj.get("updateScriptPath"),
             "proxy_enabled": obj.get("proxyEnabled"),
             "proxy_type": obj.get("proxyType"),
             "proxy_hostname": obj.get("proxyHostname"),
             "proxy_port": obj.get("proxyPort"),
```

### Comparing `readarr-py-0.2.2/readarr/models/import_list_exclusion_resource.py` & `readarr-py-0.3.0/readarr/models/import_list_exclusion_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/import_list_monitor_type.py` & `readarr-py-0.3.0/readarr/models/import_list_monitor_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
```

### Comparing `readarr-py-0.2.2/readarr/models/import_list_resource.py` & `readarr-py-0.3.0/readarr/models/import_list_resource.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
@@ -18,14 +18,15 @@
 
 
 from typing import List, Optional
 from pydantic import BaseModel
 from readarr.models.field import Field
 from readarr.models.import_list_monitor_type import ImportListMonitorType
 from readarr.models.import_list_type import ImportListType
+from readarr.models.new_item_monitor_types import NewItemMonitorTypes
 from readarr.models.provider_message import ProviderMessage
 
 class ImportListResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -38,21 +39,24 @@
     config_contract: Optional[str]
     info_link: Optional[str]
     message: Optional[ProviderMessage]
     tags: Optional[List]
     presets: Optional[List]
     enable_automatic_add: Optional[bool]
     should_monitor: Optional[ImportListMonitorType]
+    should_monitor_existing: Optional[bool]
     should_search: Optional[bool]
     root_folder_path: Optional[str]
+    monitor_new_items: Optional[NewItemMonitorTypes]
     quality_profile_id: Optional[int]
     metadata_profile_id: Optional[int]
     list_type: Optional[ImportListType]
     list_order: Optional[int]
-    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "enableAutomaticAdd", "shouldMonitor", "shouldSearch", "rootFolderPath", "qualityProfileId", "metadataProfileId", "listType", "listOrder"]
+    min_refresh_interval: Optional[str]
+    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "enableAutomaticAdd", "shouldMonitor", "shouldMonitorExisting", "shouldSearch", "rootFolderPath", "monitorNewItems", "qualityProfileId", "metadataProfileId", "listType", "listOrder", "minRefreshInterval"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -150,16 +154,19 @@
             "config_contract": obj.get("configContract"),
             "info_link": obj.get("infoLink"),
             "message": ProviderMessage.from_dict(obj.get("message")) if obj.get("message") is not None else None,
             "tags": obj.get("tags"),
             "presets": [ImportListResource.from_dict(_item) for _item in obj.get("presets")] if obj.get("presets") is not None else None,
             "enable_automatic_add": obj.get("enableAutomaticAdd"),
             "should_monitor": obj.get("shouldMonitor"),
+            "should_monitor_existing": obj.get("shouldMonitorExisting"),
             "should_search": obj.get("shouldSearch"),
             "root_folder_path": obj.get("rootFolderPath"),
+            "monitor_new_items": obj.get("monitorNewItems"),
             "quality_profile_id": obj.get("qualityProfileId"),
             "metadata_profile_id": obj.get("metadataProfileId"),
             "list_type": obj.get("listType"),
-            "list_order": obj.get("listOrder")
+            "list_order": obj.get("listOrder"),
+            "min_refresh_interval": obj.get("minRefreshInterval")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/import_list_type.py` & `readarr-py-0.3.0/readarr/models/update_mechanism.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class ImportListType(str, Enum):
+class UpdateMechanism(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    PROGRAM = 'program'
-    GOODREADS = 'goodreads'
-    OTHER = 'other'
+    BUILTIN = 'builtIn'
+    SCRIPT = 'script'
+    EXTERNAL = 'external'
+    APT = 'apt'
+    DOCKER = 'docker'
```

### Comparing `readarr-py-0.2.2/readarr/models/indexer_config_resource.py` & `readarr-py-0.3.0/readarr/models/indexer_config_resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/indexer_resource.py` & `readarr-py-0.3.0/readarr/models/indexer_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
@@ -42,15 +42,16 @@
     enable_rss: Optional[bool]
     enable_automatic_search: Optional[bool]
     enable_interactive_search: Optional[bool]
     supports_rss: Optional[bool]
     supports_search: Optional[bool]
     protocol: Optional[DownloadProtocol]
     priority: Optional[int]
-    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "enableRss", "enableAutomaticSearch", "enableInteractiveSearch", "supportsRss", "supportsSearch", "protocol", "priority"]
+    download_client_id: Optional[int]
+    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "enableRss", "enableAutomaticSearch", "enableInteractiveSearch", "supportsRss", "supportsSearch", "protocol", "priority", "downloadClientId"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -148,11 +149,12 @@
             "presets": [IndexerResource.from_dict(_item) for _item in obj.get("presets")] if obj.get("presets") is not None else None,
             "enable_rss": obj.get("enableRss"),
             "enable_automatic_search": obj.get("enableAutomaticSearch"),
             "enable_interactive_search": obj.get("enableInteractiveSearch"),
             "supports_rss": obj.get("supportsRss"),
             "supports_search": obj.get("supportsSearch"),
             "protocol": obj.get("protocol"),
-            "priority": obj.get("priority")
+            "priority": obj.get("priority"),
+            "download_client_id": obj.get("downloadClientId")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/iso_country.py` & `readarr-py-0.3.0/readarr/models/iso_country.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/language_resource.py` & `readarr-py-0.3.0/readarr/models/language_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/links.py` & `readarr-py-0.3.0/readarr/models/links.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/log_file_resource.py` & `readarr-py-0.3.0/readarr/models/log_file_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/log_resource.py` & `readarr-py-0.3.0/readarr/models/log_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/log_resource_paging_resource.py` & `readarr-py-0.3.0/readarr/models/log_resource_paging_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/manual_import_resource.py` & `readarr-py-0.3.0/readarr/models/manual_import_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
@@ -35,22 +35,23 @@
     path: Optional[str]
     name: Optional[str]
     size: Optional[int]
     author: Optional[AuthorResource]
     book: Optional[BookResource]
     foreign_edition_id: Optional[str]
     quality: Optional[QualityModel]
+    release_group: Optional[str]
     quality_weight: Optional[int]
     download_id: Optional[str]
     rejections: Optional[List]
     audio_tags: Optional[ParsedTrackInfo]
     additional_file: Optional[bool]
     replace_existing_files: Optional[bool]
     disable_release_switching: Optional[bool]
-    __properties = ["id", "path", "name", "size", "author", "book", "foreignEditionId", "quality", "qualityWeight", "downloadId", "rejections", "audioTags", "additionalFile", "replaceExistingFiles", "disableReleaseSwitching"]
+    __properties = ["id", "path", "name", "size", "author", "book", "foreignEditionId", "quality", "releaseGroup", "qualityWeight", "downloadId", "rejections", "audioTags", "additionalFile", "replaceExistingFiles", "disableReleaseSwitching"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -102,14 +103,18 @@
         if self.name is None:
             _dict['name'] = None
 
         # set to None if foreign_edition_id (nullable) is None
         if self.foreign_edition_id is None:
             _dict['foreignEditionId'] = None
 
+        # set to None if release_group (nullable) is None
+        if self.release_group is None:
+            _dict['releaseGroup'] = None
+
         # set to None if download_id (nullable) is None
         if self.download_id is None:
             _dict['downloadId'] = None
 
         # set to None if rejections (nullable) is None
         if self.rejections is None:
             _dict['rejections'] = None
@@ -130,14 +135,15 @@
             "path": obj.get("path"),
             "name": obj.get("name"),
             "size": obj.get("size"),
             "author": AuthorResource.from_dict(obj.get("author")) if obj.get("author") is not None else None,
             "book": BookResource.from_dict(obj.get("book")) if obj.get("book") is not None else None,
             "foreign_edition_id": obj.get("foreignEditionId"),
             "quality": QualityModel.from_dict(obj.get("quality")) if obj.get("quality") is not None else None,
+            "release_group": obj.get("releaseGroup"),
             "quality_weight": obj.get("qualityWeight"),
             "download_id": obj.get("downloadId"),
             "rejections": [Rejection.from_dict(_item) for _item in obj.get("rejections")] if obj.get("rejections") is not None else None,
             "audio_tags": ParsedTrackInfo.from_dict(obj.get("audioTags")) if obj.get("audioTags") is not None else None,
             "additional_file": obj.get("additionalFile"),
             "replace_existing_files": obj.get("replaceExistingFiles"),
             "disable_release_switching": obj.get("disableReleaseSwitching")
```

### Comparing `readarr-py-0.2.2/readarr/models/media_cover.py` & `readarr-py-0.3.0/readarr/models/media_cover.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/media_cover_types.py` & `readarr-py-0.3.0/readarr/models/command_priority.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class MediaCoverTypes(str, Enum):
+class CommandPriority(str, Enum):
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
-    COVER = 'cover'
-    DISC = 'disc'
-    LOGO = 'logo'
+    NORMAL = 'normal'
+    HIGH = 'high'
+    LOW = 'low'
```

### Comparing `readarr-py-0.2.2/readarr/models/media_info_model.py` & `readarr-py-0.3.0/readarr/models/media_info_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/media_info_resource.py` & `readarr-py-0.3.0/readarr/models/media_info_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
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

### Comparing `readarr-py-0.2.2/readarr/models/media_management_config_resource.py` & `readarr-py-0.3.0/readarr/models/media_management_config_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/metadata_profile.py` & `readarr-py-0.3.0/readarr/models/metadata_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import Optional, Union
 from pydantic import BaseModel
 
 class MetadataProfile(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `readarr-py-0.2.2/readarr/models/metadata_profile_lazy_loaded.py` & `readarr-py-0.3.0/readarr/models/metadata_profile_lazy_loaded.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/metadata_profile_resource.py` & `readarr-py-0.3.0/readarr/models/metadata_profile_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import Optional, Union
 from pydantic import BaseModel
 
 class MetadataProfileResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `readarr-py-0.2.2/readarr/models/metadata_provider_config_resource.py` & `readarr-py-0.3.0/readarr/models/metadata_provider_config_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/metadata_resource.py` & `readarr-py-0.3.0/readarr/models/metadata_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/monitor_types.py` & `readarr-py-0.3.0/readarr/models/database_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class MonitorTypes(str, Enum):
+class DatabaseType(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    ALL = 'all'
-    FUTURE = 'future'
-    MISSING = 'missing'
-    EXISTING = 'existing'
-    LATEST = 'latest'
-    FIRST = 'first'
-    NONE = 'none'
-    UNKNOWN = 'unknown'
+    SQLITE = 'sqLite'
+    POSTGRESQL = 'postgreSQL'
```

### Comparing `readarr-py-0.2.2/readarr/models/monitoring_options.py` & `readarr-py-0.3.0/readarr/models/monitoring_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/naming_config_resource.py` & `readarr-py-0.3.0/readarr/models/naming_config_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/notification_resource.py` & `readarr-py-0.3.0/readarr/models/notification_resource.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
@@ -39,33 +39,39 @@
     tags: Optional[List]
     presets: Optional[List]
     link: Optional[str]
     on_grab: Optional[bool]
     on_release_import: Optional[bool]
     on_upgrade: Optional[bool]
     on_rename: Optional[bool]
+    on_author_delete: Optional[bool]
+    on_book_delete: Optional[bool]
+    on_book_file_delete: Optional[bool]
+    on_book_file_delete_for_upgrade: Optional[bool]
     on_health_issue: Optional[bool]
     on_download_failure: Optional[bool]
     on_import_failure: Optional[bool]
     on_book_retag: Optional[bool]
+    on_application_update: Optional[bool]
     supports_on_grab: Optional[bool]
     supports_on_release_import: Optional[bool]
     supports_on_upgrade: Optional[bool]
     supports_on_rename: Optional[bool]
+    supports_on_author_delete: Optional[bool]
+    supports_on_book_delete: Optional[bool]
+    supports_on_book_file_delete: Optional[bool]
+    supports_on_book_file_delete_for_upgrade: Optional[bool]
     supports_on_health_issue: Optional[bool]
     include_health_warnings: Optional[bool]
     supports_on_download_failure: Optional[bool]
     supports_on_import_failure: Optional[bool]
     supports_on_book_retag: Optional[bool]
+    supports_on_application_update: Optional[bool]
     test_command: Optional[str]
-    on_author_delete: Optional[bool]
-    on_book_delete: Optional[bool]
-    on_book_file_delete: Optional[bool]
-    on_book_file_delete_for_upgrade: Optional[bool]
-    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "link", "onGrab", "onReleaseImport", "onUpgrade", "onRename", "onHealthIssue", "onDownloadFailure", "onImportFailure", "onBookRetag", "supportsOnGrab", "supportsOnReleaseImport", "supportsOnUpgrade", "supportsOnRename", "supportsOnHealthIssue", "includeHealthWarnings", "supportsOnDownloadFailure", "supportsOnImportFailure", "supportsOnBookRetag", "testCommand", "onAuthorDelete", "onBookDelete", "onBookFileDelete", "onBookFileDeleteForUpgrade"]
+    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "link", "onGrab", "onReleaseImport", "onUpgrade", "onRename", "onAuthorDelete", "onBookDelete", "onBookFileDelete", "onBookFileDeleteForUpgrade", "onHealthIssue", "onDownloadFailure", "onImportFailure", "onBookRetag", "onApplicationUpdate", "supportsOnGrab", "supportsOnReleaseImport", "supportsOnUpgrade", "supportsOnRename", "supportsOnAuthorDelete", "supportsOnBookDelete", "supportsOnBookFileDelete", "supportsOnBookFileDeleteForUpgrade", "supportsOnHealthIssue", "includeHealthWarnings", "supportsOnDownloadFailure", "supportsOnImportFailure", "supportsOnBookRetag", "supportsOnApplicationUpdate", "testCommand"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -170,28 +176,34 @@
             "tags": obj.get("tags"),
             "presets": [NotificationResource.from_dict(_item) for _item in obj.get("presets")] if obj.get("presets") is not None else None,
             "link": obj.get("link"),
             "on_grab": obj.get("onGrab"),
             "on_release_import": obj.get("onReleaseImport"),
             "on_upgrade": obj.get("onUpgrade"),
             "on_rename": obj.get("onRename"),
+            "on_author_delete": obj.get("onAuthorDelete"),
+            "on_book_delete": obj.get("onBookDelete"),
+            "on_book_file_delete": obj.get("onBookFileDelete"),
+            "on_book_file_delete_for_upgrade": obj.get("onBookFileDeleteForUpgrade"),
             "on_health_issue": obj.get("onHealthIssue"),
             "on_download_failure": obj.get("onDownloadFailure"),
             "on_import_failure": obj.get("onImportFailure"),
             "on_book_retag": obj.get("onBookRetag"),
+            "on_application_update": obj.get("onApplicationUpdate"),
             "supports_on_grab": obj.get("supportsOnGrab"),
             "supports_on_release_import": obj.get("supportsOnReleaseImport"),
             "supports_on_upgrade": obj.get("supportsOnUpgrade"),
             "supports_on_rename": obj.get("supportsOnRename"),
+            "supports_on_author_delete": obj.get("supportsOnAuthorDelete"),
+            "supports_on_book_delete": obj.get("supportsOnBookDelete"),
+            "supports_on_book_file_delete": obj.get("supportsOnBookFileDelete"),
+            "supports_on_book_file_delete_for_upgrade": obj.get("supportsOnBookFileDeleteForUpgrade"),
             "supports_on_health_issue": obj.get("supportsOnHealthIssue"),
             "include_health_warnings": obj.get("includeHealthWarnings"),
             "supports_on_download_failure": obj.get("supportsOnDownloadFailure"),
             "supports_on_import_failure": obj.get("supportsOnImportFailure"),
             "supports_on_book_retag": obj.get("supportsOnBookRetag"),
-            "test_command": obj.get("testCommand"),
-            "on_author_delete": obj.get("onAuthorDelete"),
-            "on_book_delete": obj.get("onBookDelete"),
-            "on_book_file_delete": obj.get("onBookFileDelete"),
-            "on_book_file_delete_for_upgrade": obj.get("onBookFileDeleteForUpgrade")
+            "supports_on_application_update": obj.get("supportsOnApplicationUpdate"),
+            "test_command": obj.get("testCommand")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/paging_resource_filter.py` & `readarr-py-0.3.0/readarr/models/paging_resource_filter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/parse_resource.py` & `readarr-py-0.3.0/readarr/models/parse_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/parsed_book_info.py` & `readarr-py-0.3.0/readarr/models/parsed_book_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
@@ -35,15 +35,16 @@
     release_date: Optional[str]
     discography: Optional[bool]
     discography_start: Optional[int]
     discography_end: Optional[int]
     release_group: Optional[str]
     release_hash: Optional[str]
     release_version: Optional[str]
-    __properties = ["bookTitle", "authorName", "authorTitleInfo", "quality", "releaseDate", "discography", "discographyStart", "discographyEnd", "releaseGroup", "releaseHash", "releaseVersion"]
+    release_title: Optional[str]
+    __properties = ["bookTitle", "authorName", "authorTitleInfo", "quality", "releaseDate", "discography", "discographyStart", "discographyEnd", "releaseGroup", "releaseHash", "releaseVersion", "releaseTitle"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -94,14 +95,18 @@
         if self.release_hash is None:
             _dict['releaseHash'] = None
 
         # set to None if release_version (nullable) is None
         if self.release_version is None:
             _dict['releaseVersion'] = None
 
+        # set to None if release_title (nullable) is None
+        if self.release_title is None:
+            _dict['releaseTitle'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> ParsedBookInfo:
         """Create an instance of ParsedBookInfo from a dict"""
         if obj is None:
             return None
@@ -116,11 +121,12 @@
             "quality": QualityModel.from_dict(obj.get("quality")) if obj.get("quality") is not None else None,
             "release_date": obj.get("releaseDate"),
             "discography": obj.get("discography"),
             "discography_start": obj.get("discographyStart"),
             "discography_end": obj.get("discographyEnd"),
             "release_group": obj.get("releaseGroup"),
             "release_hash": obj.get("releaseHash"),
-            "release_version": obj.get("releaseVersion")
+            "release_version": obj.get("releaseVersion"),
+            "release_title": obj.get("releaseTitle")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/parsed_track_info.py` & `readarr-py-0.3.0/readarr/models/parsed_track_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/proper_download_types.py` & `readarr-py-0.3.0/readarr/models/proper_download_types.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
```

### Comparing `readarr-py-0.2.2/readarr/models/provider_message.py` & `readarr-py-0.3.0/readarr/models/provider_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/provider_message_type.py` & `readarr-py-0.3.0/readarr/models/runtime_mode.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class ProviderMessageType(str, Enum):
+class RuntimeMode(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    INFO = 'info'
-    WARNING = 'warning'
-    ERROR = 'error'
+    CONSOLE = 'console'
+    SERVICE = 'service'
+    TRAY = 'tray'
```

### Comparing `readarr-py-0.2.2/readarr/models/proxy_type.py` & `readarr-py-0.3.0/readarr/models/health_check_result.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class ProxyType(str, Enum):
+class HealthCheckResult(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    HTTP = 'http'
-    SOCKS4 = 'socks4'
-    SOCKS5 = 'socks5'
+    OK = 'ok'
+    NOTICE = 'notice'
+    WARNING = 'warning'
+    ERROR = 'error'
```

### Comparing `readarr-py-0.2.2/readarr/models/quality.py` & `readarr-py-0.3.0/readarr/models/quality.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/quality_definition_resource.py` & `readarr-py-0.3.0/readarr/models/quality_definition_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import Optional, Union
 from pydantic import BaseModel
 from readarr.models.quality import Quality
 
 class QualityDefinitionResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `readarr-py-0.2.2/readarr/models/quality_model.py` & `readarr-py-0.3.0/readarr/models/quality_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/quality_profile.py` & `readarr-py-0.3.0/readarr/models/quality_profile_quality_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel
-from readarr.models.quality_profile_quality_item import QualityProfileQualityItem
+from readarr.models.quality import Quality
 
-class QualityProfile(BaseModel):
+class QualityProfileQualityItem(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     id: Optional[int]
     name: Optional[str]
-    upgrade_allowed: Optional[bool]
-    cutoff: Optional[int]
+    quality: Optional[Quality]
     items: Optional[List]
-    __properties = ["id", "name", "upgradeAllowed", "cutoff", "items"]
+    allowed: Optional[bool]
+    __properties = ["id", "name", "quality", "items", "allowed"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -47,24 +47,27 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> QualityProfile:
-        """Create an instance of QualityProfile from a JSON string"""
+    def from_json(cls, json_str: str) -> QualityProfileQualityItem:
+        """Create an instance of QualityProfileQualityItem from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of quality
+        if self.quality:
+            _dict['quality'] = self.quality.to_dict()
         # override the default output from pydantic by calling `to_dict()` of each item in items (list)
         _items = []
         if self.items:
             for _item in self.items:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['items'] = _items
@@ -75,24 +78,24 @@
         # set to None if items (nullable) is None
         if self.items is None:
             _dict['items'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> QualityProfile:
-        """Create an instance of QualityProfile from a dict"""
+    def from_dict(cls, obj: dict) -> QualityProfileQualityItem:
+        """Create an instance of QualityProfileQualityItem from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return QualityProfile.parse_obj(obj)
+            return QualityProfileQualityItem.parse_obj(obj)
 
-        _obj = QualityProfile.parse_obj({
+        _obj = QualityProfileQualityItem.parse_obj({
             "id": obj.get("id"),
             "name": obj.get("name"),
-            "upgrade_allowed": obj.get("upgradeAllowed"),
-            "cutoff": obj.get("cutoff"),
-            "items": [QualityProfileQualityItem.from_dict(_item) for _item in obj.get("items")] if obj.get("items") is not None else None
+            "quality": Quality.from_dict(obj.get("quality")) if obj.get("quality") is not None else None,
+            "items": [QualityProfileQualityItem.from_dict(_item) for _item in obj.get("items")] if obj.get("items") is not None else None,
+            "allowed": obj.get("allowed")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/quality_profile_lazy_loaded.py` & `readarr-py-0.3.0/readarr/models/quality_profile_lazy_loaded.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/quality_profile_quality_item.py` & `readarr-py-0.3.0/readarr/models/quality_profile_quality_item_resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
@@ -17,15 +17,15 @@
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel
 from readarr.models.quality import Quality
 
-class QualityProfileQualityItem(BaseModel):
+class QualityProfileQualityItemResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     id: Optional[int]
     name: Optional[str]
@@ -47,16 +47,16 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> QualityProfileQualityItem:
-        """Create an instance of QualityProfileQualityItem from a JSON string"""
+    def from_json(cls, json_str: str) -> QualityProfileQualityItemResource:
+        """Create an instance of QualityProfileQualityItemResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -78,24 +78,24 @@
         # set to None if items (nullable) is None
         if self.items is None:
             _dict['items'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> QualityProfileQualityItem:
-        """Create an instance of QualityProfileQualityItem from a dict"""
+    def from_dict(cls, obj: dict) -> QualityProfileQualityItemResource:
+        """Create an instance of QualityProfileQualityItemResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return QualityProfileQualityItem.parse_obj(obj)
+            return QualityProfileQualityItemResource.parse_obj(obj)
 
-        _obj = QualityProfileQualityItem.parse_obj({
+        _obj = QualityProfileQualityItemResource.parse_obj({
             "id": obj.get("id"),
             "name": obj.get("name"),
             "quality": Quality.from_dict(obj.get("quality")) if obj.get("quality") is not None else None,
-            "items": [QualityProfileQualityItem.from_dict(_item) for _item in obj.get("items")] if obj.get("items") is not None else None,
+            "items": [QualityProfileQualityItemResource.from_dict(_item) for _item in obj.get("items")] if obj.get("items") is not None else None,
             "allowed": obj.get("allowed")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/quality_profile_quality_item_resource.py` & `readarr-py-0.3.0/readarr/models/book_editor_resource.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel
-from readarr.models.quality import Quality
 
-class QualityProfileQualityItemResource(BaseModel):
+class BookEditorResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    id: Optional[int]
-    name: Optional[str]
-    quality: Optional[Quality]
-    items: Optional[List]
-    allowed: Optional[bool]
-    __properties = ["id", "name", "quality", "items", "allowed"]
+    book_ids: Optional[List]
+    monitored: Optional[bool]
+    delete_files: Optional[bool]
+    add_import_list_exclusion: Optional[bool]
+    __properties = ["bookIds", "monitored", "deleteFiles", "addImportListExclusion"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -47,55 +45,52 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> QualityProfileQualityItemResource:
-        """Create an instance of QualityProfileQualityItemResource from a JSON string"""
+    def from_json(cls, json_str: str) -> BookEditorResource:
+        """Create an instance of BookEditorResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of quality
-        if self.quality:
-            _dict['quality'] = self.quality.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in items (list)
-        _items = []
-        if self.items:
-            for _item in self.items:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['items'] = _items
-        # set to None if name (nullable) is None
-        if self.name is None:
-            _dict['name'] = None
-
-        # set to None if items (nullable) is None
-        if self.items is None:
-            _dict['items'] = None
+        # set to None if book_ids (nullable) is None
+        if self.book_ids is None:
+            _dict['bookIds'] = None
+
+        # set to None if monitored (nullable) is None
+        if self.monitored is None:
+            _dict['monitored'] = None
+
+        # set to None if delete_files (nullable) is None
+        if self.delete_files is None:
+            _dict['deleteFiles'] = None
+
+        # set to None if add_import_list_exclusion (nullable) is None
+        if self.add_import_list_exclusion is None:
+            _dict['addImportListExclusion'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> QualityProfileQualityItemResource:
-        """Create an instance of QualityProfileQualityItemResource from a dict"""
+    def from_dict(cls, obj: dict) -> BookEditorResource:
+        """Create an instance of BookEditorResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return QualityProfileQualityItemResource.parse_obj(obj)
+            return BookEditorResource.parse_obj(obj)
 
-        _obj = QualityProfileQualityItemResource.parse_obj({
-            "id": obj.get("id"),
-            "name": obj.get("name"),
-            "quality": Quality.from_dict(obj.get("quality")) if obj.get("quality") is not None else None,
-            "items": [QualityProfileQualityItemResource.from_dict(_item) for _item in obj.get("items")] if obj.get("items") is not None else None,
-            "allowed": obj.get("allowed")
+        _obj = BookEditorResource.parse_obj({
+            "book_ids": obj.get("bookIds"),
+            "monitored": obj.get("monitored"),
+            "delete_files": obj.get("deleteFiles"),
+            "add_import_list_exclusion": obj.get("addImportListExclusion")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/quality_profile_resource.py` & `readarr-py-0.3.0/readarr/models/rename_book_resource.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
+from typing import Optional
 from pydantic import BaseModel
-from readarr.models.quality_profile_quality_item_resource import QualityProfileQualityItemResource
 
-class QualityProfileResource(BaseModel):
+class RenameBookResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     id: Optional[int]
-    name: Optional[str]
-    upgrade_allowed: Optional[bool]
-    cutoff: Optional[int]
-    items: Optional[List]
-    __properties = ["id", "name", "upgradeAllowed", "cutoff", "items"]
+    author_id: Optional[int]
+    book_id: Optional[int]
+    book_file_id: Optional[int]
+    existing_path: Optional[str]
+    new_path: Optional[str]
+    __properties = ["id", "authorId", "bookId", "bookFileId", "existingPath", "newPath"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -47,52 +47,46 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> QualityProfileResource:
-        """Create an instance of QualityProfileResource from a JSON string"""
+    def from_json(cls, json_str: str) -> RenameBookResource:
+        """Create an instance of RenameBookResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in items (list)
-        _items = []
-        if self.items:
-            for _item in self.items:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['items'] = _items
-        # set to None if name (nullable) is None
-        if self.name is None:
-            _dict['name'] = None
-
-        # set to None if items (nullable) is None
-        if self.items is None:
-            _dict['items'] = None
+        # set to None if existing_path (nullable) is None
+        if self.existing_path is None:
+            _dict['existingPath'] = None
+
+        # set to None if new_path (nullable) is None
+        if self.new_path is None:
+            _dict['newPath'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> QualityProfileResource:
-        """Create an instance of QualityProfileResource from a dict"""
+    def from_dict(cls, obj: dict) -> RenameBookResource:
+        """Create an instance of RenameBookResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return QualityProfileResource.parse_obj(obj)
+            return RenameBookResource.parse_obj(obj)
 
-        _obj = QualityProfileResource.parse_obj({
+        _obj = RenameBookResource.parse_obj({
             "id": obj.get("id"),
-            "name": obj.get("name"),
-            "upgrade_allowed": obj.get("upgradeAllowed"),
-            "cutoff": obj.get("cutoff"),
-            "items": [QualityProfileQualityItemResource.from_dict(_item) for _item in obj.get("items")] if obj.get("items") is not None else None
+            "author_id": obj.get("authorId"),
+            "book_id": obj.get("bookId"),
+            "book_file_id": obj.get("bookFileId"),
+            "existing_path": obj.get("existingPath"),
+            "new_path": obj.get("newPath")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/queue_bulk_resource.py` & `readarr-py-0.3.0/readarr/models/queue_bulk_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/queue_resource.py` & `readarr-py-0.3.0/readarr/models/queue_resource.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import List, Optional
+from typing import List, Optional, Union
 from pydantic import BaseModel
 from readarr.models.author_resource import AuthorResource
 from readarr.models.book_resource import BookResource
+from readarr.models.custom_format_resource import CustomFormatResource
 from readarr.models.download_protocol import DownloadProtocol
 from readarr.models.quality_model import QualityModel
 from readarr.models.tracked_download_state import TrackedDownloadState
 from readarr.models.tracked_download_status import TrackedDownloadStatus
 from readarr.models.tracked_download_status_message import TrackedDownloadStatusMessage
 
 class QueueResource(BaseModel):
@@ -35,14 +36,15 @@
     """
     id: Optional[int]
     author_id: Optional[int]
     book_id: Optional[int]
     author: Optional[AuthorResource]
     book: Optional[BookResource]
     quality: Optional[QualityModel]
+    custom_formats: Optional[List]
     size: Optional[float]
     title: Optional[str]
     sizeleft: Optional[float]
     timeleft: Optional[str]
     estimated_completion_time: Optional[datetime]
     status: Optional[str]
     tracked_download_status: Optional[TrackedDownloadStatus]
@@ -51,15 +53,15 @@
     error_message: Optional[str]
     download_id: Optional[str]
     protocol: Optional[DownloadProtocol]
     download_client: Optional[str]
     indexer: Optional[str]
     output_path: Optional[str]
     download_forced: Optional[bool]
-    __properties = ["id", "authorId", "bookId", "author", "book", "quality", "size", "title", "sizeleft", "timeleft", "estimatedCompletionTime", "status", "trackedDownloadStatus", "trackedDownloadState", "statusMessages", "errorMessage", "downloadId", "protocol", "downloadClient", "indexer", "outputPath", "downloadForced"]
+    __properties = ["id", "authorId", "bookId", "author", "book", "quality", "customFormats", "size", "title", "sizeleft", "timeleft", "estimatedCompletionTime", "status", "trackedDownloadStatus", "trackedDownloadState", "statusMessages", "errorMessage", "downloadId", "protocol", "downloadClient", "indexer", "outputPath", "downloadForced"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -89,14 +91,21 @@
             _dict['author'] = self.author.to_dict()
         # override the default output from pydantic by calling `to_dict()` of book
         if self.book:
             _dict['book'] = self.book.to_dict()
         # override the default output from pydantic by calling `to_dict()` of quality
         if self.quality:
             _dict['quality'] = self.quality.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in custom_formats (list)
+        _items = []
+        if self.custom_formats:
+            for _item in self.custom_formats:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['customFormats'] = _items
         # override the default output from pydantic by calling `to_dict()` of each item in status_messages (list)
         _items = []
         if self.status_messages:
             for _item in self.status_messages:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['statusMessages'] = _items
@@ -104,14 +113,18 @@
         if self.author_id is None:
             _dict['authorId'] = None
 
         # set to None if book_id (nullable) is None
         if self.book_id is None:
             _dict['bookId'] = None
 
+        # set to None if custom_formats (nullable) is None
+        if self.custom_formats is None:
+            _dict['customFormats'] = None
+
         # set to None if title (nullable) is None
         if self.title is None:
             _dict['title'] = None
 
         # set to None if estimated_completion_time (nullable) is None
         if self.estimated_completion_time is None:
             _dict['estimatedCompletionTime'] = None
@@ -158,14 +171,15 @@
         _obj = QueueResource.parse_obj({
             "id": obj.get("id"),
             "author_id": obj.get("authorId"),
             "book_id": obj.get("bookId"),
             "author": AuthorResource.from_dict(obj.get("author")) if obj.get("author") is not None else None,
             "book": BookResource.from_dict(obj.get("book")) if obj.get("book") is not None else None,
             "quality": QualityModel.from_dict(obj.get("quality")) if obj.get("quality") is not None else None,
+            "custom_formats": [CustomFormatResource.from_dict(_item) for _item in obj.get("customFormats")] if obj.get("customFormats") is not None else None,
             "size": obj.get("size"),
             "title": obj.get("title"),
             "sizeleft": obj.get("sizeleft"),
             "timeleft": obj.get("timeleft"),
             "estimated_completion_time": obj.get("estimatedCompletionTime"),
             "status": obj.get("status"),
             "tracked_download_status": obj.get("trackedDownloadStatus"),
```

### Comparing `readarr-py-0.2.2/readarr/models/queue_resource_paging_resource.py` & `readarr-py-0.3.0/readarr/models/blocklist_resource_paging_resource.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel
+from readarr.models.blocklist_resource import BlocklistResource
 from readarr.models.paging_resource_filter import PagingResourceFilter
-from readarr.models.queue_resource import QueueResource
 from readarr.models.sort_direction import SortDirection
 
-class QueueResourcePagingResource(BaseModel):
+class BlocklistResourcePagingResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     page: Optional[int]
     page_size: Optional[int]
@@ -51,16 +51,16 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> QueueResourcePagingResource:
-        """Create an instance of QueueResourcePagingResource from a JSON string"""
+    def from_json(cls, json_str: str) -> BlocklistResourcePagingResource:
+        """Create an instance of BlocklistResourcePagingResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -90,26 +90,26 @@
         # set to None if records (nullable) is None
         if self.records is None:
             _dict['records'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> QueueResourcePagingResource:
-        """Create an instance of QueueResourcePagingResource from a dict"""
+    def from_dict(cls, obj: dict) -> BlocklistResourcePagingResource:
+        """Create an instance of BlocklistResourcePagingResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return QueueResourcePagingResource.parse_obj(obj)
+            return BlocklistResourcePagingResource.parse_obj(obj)
 
-        _obj = QueueResourcePagingResource.parse_obj({
+        _obj = BlocklistResourcePagingResource.parse_obj({
             "page": obj.get("page"),
             "page_size": obj.get("pageSize"),
             "sort_key": obj.get("sortKey"),
             "sort_direction": obj.get("sortDirection"),
             "filters": [PagingResourceFilter.from_dict(_item) for _item in obj.get("filters")] if obj.get("filters") is not None else None,
             "total_records": obj.get("totalRecords"),
-            "records": [QueueResource.from_dict(_item) for _item in obj.get("records")] if obj.get("records") is not None else None
+            "records": [BlocklistResource.from_dict(_item) for _item in obj.get("records")] if obj.get("records") is not None else None
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/queue_status_resource.py` & `readarr-py-0.3.0/readarr/models/queue_status_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/ratings.py` & `readarr-py-0.3.0/readarr/models/ratings.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
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

### Comparing `readarr-py-0.2.2/readarr/models/rejection.py` & `readarr-py-0.3.0/readarr/models/rejection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/rejection_type.py` & `readarr-py-0.3.0/readarr/models/sort_direction.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class RejectionType(str, Enum):
+class SortDirection(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    PERMANENT = 'permanent'
-    TEMPORARY = 'temporary'
+    DEFAULT = 'default'
+    ASCENDING = 'ascending'
+    DESCENDING = 'descending'
```

### Comparing `readarr-py-0.2.2/readarr/models/release_profile_resource.py` & `readarr-py-0.3.0/readarr/models/retag_book_resource.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel
-from readarr.models.string_int32_key_value_pair import StringInt32KeyValuePair
+from readarr.models.tag_difference import TagDifference
 
-class ReleaseProfileResource(BaseModel):
+class RetagBookResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     id: Optional[int]
-    enabled: Optional[bool]
-    required: Optional[str]
-    ignored: Optional[str]
-    preferred: Optional[List]
-    include_preferred_when_renaming: Optional[bool]
-    indexer_id: Optional[int]
-    tags: Optional[List]
-    __properties = ["id", "enabled", "required", "ignored", "preferred", "includePreferredWhenRenaming", "indexerId", "tags"]
+    author_id: Optional[int]
+    book_id: Optional[int]
+    track_numbers: Optional[List]
+    book_file_id: Optional[int]
+    path: Optional[str]
+    changes: Optional[List]
+    __properties = ["id", "authorId", "bookId", "trackNumbers", "bookFileId", "path", "changes"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -50,63 +49,58 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ReleaseProfileResource:
-        """Create an instance of ReleaseProfileResource from a JSON string"""
+    def from_json(cls, json_str: str) -> RetagBookResource:
+        """Create an instance of RetagBookResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in preferred (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in changes (list)
         _items = []
-        if self.preferred:
-            for _item in self.preferred:
+        if self.changes:
+            for _item in self.changes:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['preferred'] = _items
-        # set to None if required (nullable) is None
-        if self.required is None:
-            _dict['required'] = None
-
-        # set to None if ignored (nullable) is None
-        if self.ignored is None:
-            _dict['ignored'] = None
-
-        # set to None if preferred (nullable) is None
-        if self.preferred is None:
-            _dict['preferred'] = None
-
-        # set to None if tags (nullable) is None
-        if self.tags is None:
-            _dict['tags'] = None
+            _dict['changes'] = _items
+        # set to None if track_numbers (nullable) is None
+        if self.track_numbers is None:
+            _dict['trackNumbers'] = None
+
+        # set to None if path (nullable) is None
+        if self.path is None:
+            _dict['path'] = None
+
+        # set to None if changes (nullable) is None
+        if self.changes is None:
+            _dict['changes'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ReleaseProfileResource:
-        """Create an instance of ReleaseProfileResource from a dict"""
+    def from_dict(cls, obj: dict) -> RetagBookResource:
+        """Create an instance of RetagBookResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return ReleaseProfileResource.parse_obj(obj)
+            return RetagBookResource.parse_obj(obj)
 
-        _obj = ReleaseProfileResource.parse_obj({
+        _obj = RetagBookResource.parse_obj({
             "id": obj.get("id"),
-            "enabled": obj.get("enabled"),
-            "required": obj.get("required"),
-            "ignored": obj.get("ignored"),
-            "preferred": [StringInt32KeyValuePair.from_dict(_item) for _item in obj.get("preferred")] if obj.get("preferred") is not None else None,
-            "include_preferred_when_renaming": obj.get("includePreferredWhenRenaming"),
-            "indexer_id": obj.get("indexerId"),
-            "tags": obj.get("tags")
+            "author_id": obj.get("authorId"),
+            "book_id": obj.get("bookId"),
+            "track_numbers": obj.get("trackNumbers"),
+            "book_file_id": obj.get("bookFileId"),
+            "path": obj.get("path"),
+            "changes": [TagDifference.from_dict(_item) for _item in obj.get("changes")] if obj.get("changes") is not None else None
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/release_resource.py` & `readarr-py-0.3.0/readarr/models/release_resource.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import List, Optional
+from typing import List, Optional, Union
 from pydantic import BaseModel
+from readarr.models.custom_format_resource import CustomFormatResource
 from readarr.models.download_protocol import DownloadProtocol
 from readarr.models.quality_model import QualityModel
 
 class ReleaseResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -53,23 +54,24 @@
     rejections: Optional[List]
     publish_date: Optional[datetime]
     comment_url: Optional[str]
     download_url: Optional[str]
     info_url: Optional[str]
     download_allowed: Optional[bool]
     release_weight: Optional[int]
-    preferred_word_score: Optional[int]
+    custom_formats: Optional[List]
+    custom_format_score: Optional[int]
     magnet_url: Optional[str]
     info_hash: Optional[str]
     seeders: Optional[int]
     leechers: Optional[int]
     protocol: Optional[DownloadProtocol]
     author_id: Optional[int]
     book_id: Optional[int]
-    __properties = ["id", "guid", "quality", "qualityWeight", "age", "ageHours", "ageMinutes", "size", "indexerId", "indexer", "releaseGroup", "subGroup", "releaseHash", "title", "discography", "sceneSource", "airDate", "authorName", "bookTitle", "approved", "temporarilyRejected", "rejected", "rejections", "publishDate", "commentUrl", "downloadUrl", "infoUrl", "downloadAllowed", "releaseWeight", "preferredWordScore", "magnetUrl", "infoHash", "seeders", "leechers", "protocol", "authorId", "bookId"]
+    __properties = ["id", "guid", "quality", "qualityWeight", "age", "ageHours", "ageMinutes", "size", "indexerId", "indexer", "releaseGroup", "subGroup", "releaseHash", "title", "discography", "sceneSource", "airDate", "authorName", "bookTitle", "approved", "temporarilyRejected", "rejected", "rejections", "publishDate", "commentUrl", "downloadUrl", "infoUrl", "downloadAllowed", "releaseWeight", "customFormats", "customFormatScore", "magnetUrl", "infoHash", "seeders", "leechers", "protocol", "authorId", "bookId"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -93,14 +95,21 @@
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of quality
         if self.quality:
             _dict['quality'] = self.quality.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in custom_formats (list)
+        _items = []
+        if self.custom_formats:
+            for _item in self.custom_formats:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['customFormats'] = _items
         # set to None if guid (nullable) is None
         if self.guid is None:
             _dict['guid'] = None
 
         # set to None if indexer (nullable) is None
         if self.indexer is None:
             _dict['indexer'] = None
@@ -145,14 +154,18 @@
         if self.download_url is None:
             _dict['downloadUrl'] = None
 
         # set to None if info_url (nullable) is None
         if self.info_url is None:
             _dict['infoUrl'] = None
 
+        # set to None if custom_formats (nullable) is None
+        if self.custom_formats is None:
+            _dict['customFormats'] = None
+
         # set to None if magnet_url (nullable) is None
         if self.magnet_url is None:
             _dict['magnetUrl'] = None
 
         # set to None if info_hash (nullable) is None
         if self.info_hash is None:
             _dict['infoHash'] = None
@@ -210,15 +223,16 @@
             "rejections": obj.get("rejections"),
             "publish_date": obj.get("publishDate"),
             "comment_url": obj.get("commentUrl"),
             "download_url": obj.get("downloadUrl"),
             "info_url": obj.get("infoUrl"),
             "download_allowed": obj.get("downloadAllowed"),
             "release_weight": obj.get("releaseWeight"),
-            "preferred_word_score": obj.get("preferredWordScore"),
+            "custom_formats": [CustomFormatResource.from_dict(_item) for _item in obj.get("customFormats")] if obj.get("customFormats") is not None else None,
+            "custom_format_score": obj.get("customFormatScore"),
             "magnet_url": obj.get("magnetUrl"),
             "info_hash": obj.get("infoHash"),
             "seeders": obj.get("seeders"),
             "leechers": obj.get("leechers"),
             "protocol": obj.get("protocol"),
             "author_id": obj.get("authorId"),
             "book_id": obj.get("bookId")
```

### Comparing `readarr-py-0.2.2/readarr/models/remote_path_mapping_resource.py` & `readarr-py-0.3.0/readarr/models/remote_path_mapping_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/rename_book_resource.py` & `readarr-py-0.3.0/readarr/models/series_book_link_resource.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel
 
-class RenameBookResource(BaseModel):
+class SeriesBookLinkResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     id: Optional[int]
-    author_id: Optional[int]
+    position: Optional[str]
+    series_position: Optional[int]
+    series_id: Optional[int]
     book_id: Optional[int]
-    book_file_id: Optional[int]
-    existing_path: Optional[str]
-    new_path: Optional[str]
-    __properties = ["id", "authorId", "bookId", "bookFileId", "existingPath", "newPath"]
+    __properties = ["id", "position", "seriesPosition", "seriesId", "bookId"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -47,46 +46,41 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> RenameBookResource:
-        """Create an instance of RenameBookResource from a JSON string"""
+    def from_json(cls, json_str: str) -> SeriesBookLinkResource:
+        """Create an instance of SeriesBookLinkResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if existing_path (nullable) is None
-        if self.existing_path is None:
-            _dict['existingPath'] = None
-
-        # set to None if new_path (nullable) is None
-        if self.new_path is None:
-            _dict['newPath'] = None
+        # set to None if position (nullable) is None
+        if self.position is None:
+            _dict['position'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> RenameBookResource:
-        """Create an instance of RenameBookResource from a dict"""
+    def from_dict(cls, obj: dict) -> SeriesBookLinkResource:
+        """Create an instance of SeriesBookLinkResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return RenameBookResource.parse_obj(obj)
+            return SeriesBookLinkResource.parse_obj(obj)
 
-        _obj = RenameBookResource.parse_obj({
+        _obj = SeriesBookLinkResource.parse_obj({
             "id": obj.get("id"),
-            "author_id": obj.get("authorId"),
-            "book_id": obj.get("bookId"),
-            "book_file_id": obj.get("bookFileId"),
-            "existing_path": obj.get("existingPath"),
-            "new_path": obj.get("newPath")
+            "position": obj.get("position"),
+            "series_position": obj.get("seriesPosition"),
+            "series_id": obj.get("seriesId"),
+            "book_id": obj.get("bookId")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/rescan_after_refresh_type.py` & `readarr-py-0.3.0/readarr/models/proxy_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class RescanAfterRefreshType(str, Enum):
+class ProxyType(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    ALWAYS = 'always'
-    AFTERMANUAL = 'afterManual'
-    NEVER = 'never'
+    HTTP = 'http'
+    SOCKS4 = 'socks4'
+    SOCKS5 = 'socks5'
```

### Comparing `readarr-py-0.2.2/readarr/models/retag_book_resource.py` & `readarr-py-0.3.0/readarr/models/series_book_link.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
+from typing import Optional
 from pydantic import BaseModel
-from readarr.models.tag_difference import TagDifference
 
-class RetagBookResource(BaseModel):
+class SeriesBookLink(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     id: Optional[int]
-    author_id: Optional[int]
+    position: Optional[str]
+    series_position: Optional[int]
+    series_id: Optional[int]
     book_id: Optional[int]
-    track_numbers: Optional[List]
-    book_file_id: Optional[int]
-    path: Optional[str]
-    changes: Optional[List]
-    __properties = ["id", "authorId", "bookId", "trackNumbers", "bookFileId", "path", "changes"]
+    is_primary: Optional[bool]
+    series: Optional[SeriesLazyLoaded]
+    book: Optional[BookLazyLoaded]
+    __properties = ["id", "position", "seriesPosition", "seriesId", "bookId", "isPrimary", "series", "book"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -49,58 +49,50 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> RetagBookResource:
-        """Create an instance of RetagBookResource from a JSON string"""
+    def from_json(cls, json_str: str) -> SeriesBookLink:
+        """Create an instance of SeriesBookLink from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in changes (list)
-        _items = []
-        if self.changes:
-            for _item in self.changes:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['changes'] = _items
-        # set to None if track_numbers (nullable) is None
-        if self.track_numbers is None:
-            _dict['trackNumbers'] = None
-
-        # set to None if path (nullable) is None
-        if self.path is None:
-            _dict['path'] = None
-
-        # set to None if changes (nullable) is None
-        if self.changes is None:
-            _dict['changes'] = None
+        # override the default output from pydantic by calling `to_dict()` of series
+        if self.series:
+            _dict['series'] = self.series.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of book
+        if self.book:
+            _dict['book'] = self.book.to_dict()
+        # set to None if position (nullable) is None
+        if self.position is None:
+            _dict['position'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> RetagBookResource:
-        """Create an instance of RetagBookResource from a dict"""
+    def from_dict(cls, obj: dict) -> SeriesBookLink:
+        """Create an instance of SeriesBookLink from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return RetagBookResource.parse_obj(obj)
+            return SeriesBookLink.parse_obj(obj)
 
-        _obj = RetagBookResource.parse_obj({
+        _obj = SeriesBookLink.parse_obj({
             "id": obj.get("id"),
-            "author_id": obj.get("authorId"),
+            "position": obj.get("position"),
+            "series_position": obj.get("seriesPosition"),
+            "series_id": obj.get("seriesId"),
             "book_id": obj.get("bookId"),
-            "track_numbers": obj.get("trackNumbers"),
-            "book_file_id": obj.get("bookFileId"),
-            "path": obj.get("path"),
-            "changes": [TagDifference.from_dict(_item) for _item in obj.get("changes")] if obj.get("changes") is not None else None
+            "is_primary": obj.get("isPrimary"),
+            "series": SeriesLazyLoaded.from_dict(obj.get("series")) if obj.get("series") is not None else None,
+            "book": BookLazyLoaded.from_dict(obj.get("book")) if obj.get("book") is not None else None
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/revision.py` & `readarr-py-0.3.0/readarr/models/revision.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/root_folder_resource.py` & `readarr-py-0.3.0/readarr/models/root_folder_resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel
 from readarr.models.monitor_types import MonitorTypes
+from readarr.models.new_item_monitor_types import NewItemMonitorTypes
 
 class RootFolderResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     id: Optional[int]
     name: Optional[str]
     path: Optional[str]
     default_metadata_profile_id: Optional[int]
     default_quality_profile_id: Optional[int]
     default_monitor_option: Optional[MonitorTypes]
+    default_new_item_monitor_option: Optional[NewItemMonitorTypes]
     default_tags: Optional[List]
     is_calibre_library: Optional[bool]
     host: Optional[str]
     port: Optional[int]
     url_base: Optional[str]
     username: Optional[str]
     password: Optional[str]
     library: Optional[str]
     output_format: Optional[str]
     output_profile: Optional[str]
     use_ssl: Optional[bool]
     accessible: Optional[bool]
     free_space: Optional[int]
     total_space: Optional[int]
-    __properties = ["id", "name", "path", "defaultMetadataProfileId", "defaultQualityProfileId", "defaultMonitorOption", "defaultTags", "isCalibreLibrary", "host", "port", "urlBase", "username", "password", "library", "outputFormat", "outputProfile", "useSsl", "accessible", "freeSpace", "totalSpace"]
+    __properties = ["id", "name", "path", "defaultMetadataProfileId", "defaultQualityProfileId", "defaultMonitorOption", "defaultNewItemMonitorOption", "defaultTags", "isCalibreLibrary", "host", "port", "urlBase", "username", "password", "library", "outputFormat", "outputProfile", "useSsl", "accessible", "freeSpace", "totalSpace"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -138,14 +140,15 @@
         _obj = RootFolderResource.parse_obj({
             "id": obj.get("id"),
             "name": obj.get("name"),
             "path": obj.get("path"),
             "default_metadata_profile_id": obj.get("defaultMetadataProfileId"),
             "default_quality_profile_id": obj.get("defaultQualityProfileId"),
             "default_monitor_option": obj.get("defaultMonitorOption"),
+            "default_new_item_monitor_option": obj.get("defaultNewItemMonitorOption"),
             "default_tags": obj.get("defaultTags"),
             "is_calibre_library": obj.get("isCalibreLibrary"),
             "host": obj.get("host"),
             "port": obj.get("port"),
             "url_base": obj.get("urlBase"),
             "username": obj.get("username"),
             "password": obj.get("password"),
```

### Comparing `readarr-py-0.2.2/readarr/models/select_option.py` & `readarr-py-0.3.0/readarr/models/select_option.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/series.py` & `readarr-py-0.3.0/readarr/models/series.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/series_book_link.py` & `readarr-py-0.3.0/readarr/models/series_lazy_loaded.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel
 
-class SeriesBookLink(BaseModel):
+class SeriesLazyLoaded(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    id: Optional[int]
-    position: Optional[str]
-    series_id: Optional[int]
-    book_id: Optional[int]
-    is_primary: Optional[bool]
-    series: Optional[SeriesLazyLoaded]
-    book: Optional[BookLazyLoaded]
-    __properties = ["id", "position", "seriesId", "bookId", "isPrimary", "series", "book"]
+    value: Optional[Series]
+    is_loaded: Optional[bool]
+    __properties = ["value", "isLoaded"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -48,49 +43,38 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SeriesBookLink:
-        """Create an instance of SeriesBookLink from a JSON string"""
+    def from_json(cls, json_str: str) -> SeriesLazyLoaded:
+        """Create an instance of SeriesLazyLoaded from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
+                            "is_loaded",
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of series
-        if self.series:
-            _dict['series'] = self.series.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of book
-        if self.book:
-            _dict['book'] = self.book.to_dict()
-        # set to None if position (nullable) is None
-        if self.position is None:
-            _dict['position'] = None
-
+        # override the default output from pydantic by calling `to_dict()` of value
+        if self.value:
+            _dict['value'] = self.value.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SeriesBookLink:
-        """Create an instance of SeriesBookLink from a dict"""
+    def from_dict(cls, obj: dict) -> SeriesLazyLoaded:
+        """Create an instance of SeriesLazyLoaded from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return SeriesBookLink.parse_obj(obj)
+            return SeriesLazyLoaded.parse_obj(obj)
 
-        _obj = SeriesBookLink.parse_obj({
-            "id": obj.get("id"),
-            "position": obj.get("position"),
-            "series_id": obj.get("seriesId"),
-            "book_id": obj.get("bookId"),
-            "is_primary": obj.get("isPrimary"),
-            "series": SeriesLazyLoaded.from_dict(obj.get("series")) if obj.get("series") is not None else None,
-            "book": BookLazyLoaded.from_dict(obj.get("book")) if obj.get("book") is not None else None
+        _obj = SeriesLazyLoaded.parse_obj({
+            "value": Series.from_dict(obj.get("value")) if obj.get("value") is not None else None,
+            "is_loaded": obj.get("isLoaded")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/series_book_link_list_lazy_loaded.py` & `readarr-py-0.3.0/readarr/models/series_book_link_list_lazy_loaded.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel
-from readarr.models.series_book_link import SeriesBookLink
 
 class SeriesBookLinkListLazyLoaded(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
```

### Comparing `readarr-py-0.2.2/readarr/models/series_book_link_resource.py` & `readarr-py-0.3.0/readarr/models/update_changes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import List, Optional
 from pydantic import BaseModel
 
-class SeriesBookLinkResource(BaseModel):
+class UpdateChanges(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    id: Optional[int]
-    position: Optional[str]
-    series_id: Optional[int]
-    book_id: Optional[int]
-    __properties = ["id", "position", "seriesId", "bookId"]
+    new: Optional[List]
+    fixed: Optional[List]
+    __properties = ["new", "fixed"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -45,40 +43,42 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SeriesBookLinkResource:
-        """Create an instance of SeriesBookLinkResource from a JSON string"""
+    def from_json(cls, json_str: str) -> UpdateChanges:
+        """Create an instance of UpdateChanges from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if position (nullable) is None
-        if self.position is None:
-            _dict['position'] = None
+        # set to None if new (nullable) is None
+        if self.new is None:
+            _dict['new'] = None
+
+        # set to None if fixed (nullable) is None
+        if self.fixed is None:
+            _dict['fixed'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SeriesBookLinkResource:
-        """Create an instance of SeriesBookLinkResource from a dict"""
+    def from_dict(cls, obj: dict) -> UpdateChanges:
+        """Create an instance of UpdateChanges from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return SeriesBookLinkResource.parse_obj(obj)
+            return UpdateChanges.parse_obj(obj)
 
-        _obj = SeriesBookLinkResource.parse_obj({
-            "id": obj.get("id"),
-            "position": obj.get("position"),
-            "series_id": obj.get("seriesId"),
-            "book_id": obj.get("bookId")
+        _obj = UpdateChanges.parse_obj({
+            "new": obj.get("new"),
+            "fixed": obj.get("fixed")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/series_lazy_loaded.py` & `readarr-py-0.3.0/readarr/models/series_list_lazy_loaded.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import List, Optional
 from pydantic import BaseModel
 
-class SeriesLazyLoaded(BaseModel):
+class SeriesListLazyLoaded(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    value: Optional[Series]
+    value: Optional[List]
     is_loaded: Optional[bool]
     __properties = ["value", "isLoaded"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
@@ -43,38 +43,47 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SeriesLazyLoaded:
-        """Create an instance of SeriesLazyLoaded from a JSON string"""
+    def from_json(cls, json_str: str) -> SeriesListLazyLoaded:
+        """Create an instance of SeriesListLazyLoaded from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
+                            "value",
                             "is_loaded",
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of value
+        # override the default output from pydantic by calling `to_dict()` of each item in value (list)
+        _items = []
         if self.value:
-            _dict['value'] = self.value.to_dict()
+            for _item in self.value:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['value'] = _items
+        # set to None if value (nullable) is None
+        if self.value is None:
+            _dict['value'] = None
+
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SeriesLazyLoaded:
-        """Create an instance of SeriesLazyLoaded from a dict"""
+    def from_dict(cls, obj: dict) -> SeriesListLazyLoaded:
+        """Create an instance of SeriesListLazyLoaded from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return SeriesLazyLoaded.parse_obj(obj)
+            return SeriesListLazyLoaded.parse_obj(obj)
 
-        _obj = SeriesLazyLoaded.parse_obj({
-            "value": Series.from_dict(obj.get("value")) if obj.get("value") is not None else None,
+        _obj = SeriesListLazyLoaded.parse_obj({
+            "value": [Series.from_dict(_item) for _item in obj.get("value")] if obj.get("value") is not None else None,
             "is_loaded": obj.get("isLoaded")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/series_list_lazy_loaded.py` & `readarr-py-0.3.0/readarr/models/tag_resource.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
+from typing import Optional
 from pydantic import BaseModel
-from readarr.models.series import Series
 
-class SeriesListLazyLoaded(BaseModel):
+class TagResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    value: Optional[List]
-    is_loaded: Optional[bool]
-    __properties = ["value", "isLoaded"]
+    id: Optional[int]
+    label: Optional[str]
+    __properties = ["id", "label"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -44,47 +43,38 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SeriesListLazyLoaded:
-        """Create an instance of SeriesListLazyLoaded from a JSON string"""
+    def from_json(cls, json_str: str) -> TagResource:
+        """Create an instance of TagResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
-                            "value",
-                            "is_loaded",
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in value (list)
-        _items = []
-        if self.value:
-            for _item in self.value:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['value'] = _items
-        # set to None if value (nullable) is None
-        if self.value is None:
-            _dict['value'] = None
+        # set to None if label (nullable) is None
+        if self.label is None:
+            _dict['label'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SeriesListLazyLoaded:
-        """Create an instance of SeriesListLazyLoaded from a dict"""
+    def from_dict(cls, obj: dict) -> TagResource:
+        """Create an instance of TagResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return SeriesListLazyLoaded.parse_obj(obj)
+            return TagResource.parse_obj(obj)
 
-        _obj = SeriesListLazyLoaded.parse_obj({
-            "value": [Series.from_dict(_item) for _item in obj.get("value")] if obj.get("value") is not None else None,
-            "is_loaded": obj.get("isLoaded")
+        _obj = TagResource.parse_obj({
+            "id": obj.get("id"),
+            "label": obj.get("label")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/series_resource.py` & `readarr-py-0.3.0/readarr/models/series_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/sort_direction.py` & `readarr-py-0.3.0/readarr/models/tracked_download_state.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class SortDirection(str, Enum):
+class TrackedDownloadState(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    DEFAULT = 'default'
-    ASCENDING = 'ascending'
-    DESCENDING = 'descending'
+    DOWNLOADING = 'downloading'
+    DOWNLOADFAILED = 'downloadFailed'
+    DOWNLOADFAILEDPENDING = 'downloadFailedPending'
+    IMPORTPENDING = 'importPending'
+    IMPORTING = 'importing'
+    IMPORTFAILED = 'importFailed'
+    IMPORTED = 'imported'
+    IGNORED = 'ignored'
```

### Comparing `readarr-py-0.2.2/readarr/models/string_int32_key_value_pair.py` & `readarr-py-0.3.0/readarr/models/api_info_resource.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import List, Optional
 from pydantic import BaseModel
 
-class StringInt32KeyValuePair(BaseModel):
+class ApiInfoResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    key: Optional[str]
-    value: Optional[int]
-    __properties = ["key", "value"]
+    current: Optional[str]
+    deprecated: Optional[List]
+    __properties = ["current", "deprecated"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -43,40 +43,42 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> StringInt32KeyValuePair:
-        """Create an instance of StringInt32KeyValuePair from a JSON string"""
+    def from_json(cls, json_str: str) -> ApiInfoResource:
+        """Create an instance of ApiInfoResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
-                            "key",
-                            "value",
                           },
                           exclude_none=True)
-        # set to None if key (nullable) is None
-        if self.key is None:
-            _dict['key'] = None
+        # set to None if current (nullable) is None
+        if self.current is None:
+            _dict['current'] = None
+
+        # set to None if deprecated (nullable) is None
+        if self.deprecated is None:
+            _dict['deprecated'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> StringInt32KeyValuePair:
-        """Create an instance of StringInt32KeyValuePair from a dict"""
+    def from_dict(cls, obj: dict) -> ApiInfoResource:
+        """Create an instance of ApiInfoResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return StringInt32KeyValuePair.parse_obj(obj)
+            return ApiInfoResource.parse_obj(obj)
 
-        _obj = StringInt32KeyValuePair.parse_obj({
-            "key": obj.get("key"),
-            "value": obj.get("value")
+        _obj = ApiInfoResource.parse_obj({
+            "current": obj.get("current"),
+            "deprecated": obj.get("deprecated")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/tag_details_resource.py` & `readarr-py-0.3.0/readarr/models/tag_details_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
@@ -28,16 +28,17 @@
     """
     id: Optional[int]
     label: Optional[str]
     delay_profile_ids: Optional[List]
     import_list_ids: Optional[List]
     notification_ids: Optional[List]
     restriction_ids: Optional[List]
+    indexer_ids: Optional[List]
     author_ids: Optional[List]
-    __properties = ["id", "label", "delayProfileIds", "importListIds", "notificationIds", "restrictionIds", "authorIds"]
+    __properties = ["id", "label", "delayProfileIds", "importListIds", "notificationIds", "restrictionIds", "indexerIds", "authorIds"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -78,14 +79,18 @@
         if self.notification_ids is None:
             _dict['notificationIds'] = None
 
         # set to None if restriction_ids (nullable) is None
         if self.restriction_ids is None:
             _dict['restrictionIds'] = None
 
+        # set to None if indexer_ids (nullable) is None
+        if self.indexer_ids is None:
+            _dict['indexerIds'] = None
+
         # set to None if author_ids (nullable) is None
         if self.author_ids is None:
             _dict['authorIds'] = None
 
         return _dict
 
     @classmethod
@@ -100,11 +105,12 @@
         _obj = TagDetailsResource.parse_obj({
             "id": obj.get("id"),
             "label": obj.get("label"),
             "delay_profile_ids": obj.get("delayProfileIds"),
             "import_list_ids": obj.get("importListIds"),
             "notification_ids": obj.get("notificationIds"),
             "restriction_ids": obj.get("restrictionIds"),
+            "indexer_ids": obj.get("indexerIds"),
             "author_ids": obj.get("authorIds")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/tag_difference.py` & `readarr-py-0.3.0/readarr/models/tag_difference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/tag_resource.py` & `readarr-py-0.3.0/readarr/models/ping_resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel
 
-class TagResource(BaseModel):
+class PingResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    id: Optional[int]
-    label: Optional[str]
-    __properties = ["id", "label"]
+    status: Optional[str]
+    __properties = ["status"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -43,38 +42,37 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> TagResource:
-        """Create an instance of TagResource from a JSON string"""
+    def from_json(cls, json_str: str) -> PingResource:
+        """Create an instance of PingResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if label (nullable) is None
-        if self.label is None:
-            _dict['label'] = None
+        # set to None if status (nullable) is None
+        if self.status is None:
+            _dict['status'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> TagResource:
-        """Create an instance of TagResource from a dict"""
+    def from_dict(cls, obj: dict) -> PingResource:
+        """Create an instance of PingResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return TagResource.parse_obj(obj)
+            return PingResource.parse_obj(obj)
 
-        _obj = TagResource.parse_obj({
-            "id": obj.get("id"),
-            "label": obj.get("label")
+        _obj = PingResource.parse_obj({
+            "status": obj.get("status")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/task_resource.py` & `readarr-py-0.3.0/readarr/models/task_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/tracked_download_state.py` & `readarr-py-0.3.0/readarr/models/entity_history_event_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class TrackedDownloadState(str, Enum):
+class EntityHistoryEventType(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    DOWNLOADING = 'downloading'
+    UNKNOWN = 'unknown'
+    GRABBED = 'grabbed'
+    BOOKFILEIMPORTED = 'bookFileImported'
     DOWNLOADFAILED = 'downloadFailed'
-    DOWNLOADFAILEDPENDING = 'downloadFailedPending'
-    IMPORTPENDING = 'importPending'
-    IMPORTING = 'importing'
-    IMPORTFAILED = 'importFailed'
-    IMPORTED = 'imported'
-    IGNORED = 'ignored'
+    BOOKFILEDELETED = 'bookFileDeleted'
+    BOOKFILERENAMED = 'bookFileRenamed'
+    BOOKIMPORTINCOMPLETE = 'bookImportIncomplete'
+    DOWNLOADIMPORTED = 'downloadImported'
+    BOOKFILERETAGGED = 'bookFileRetagged'
+    DOWNLOADIGNORED = 'downloadIgnored'
```

### Comparing `readarr-py-0.2.2/readarr/models/tracked_download_status.py` & `readarr-py-0.3.0/readarr/models/tracked_download_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
```

### Comparing `readarr-py-0.2.2/readarr/models/tracked_download_status_message.py` & `readarr-py-0.3.0/readarr/models/tracked_download_status_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
```

### Comparing `readarr-py-0.2.2/readarr/models/ui_config_resource.py` & `readarr-py-0.3.0/readarr/models/ui_config_resource.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
@@ -31,15 +31,16 @@
     calendar_week_column_header: Optional[str]
     short_date_format: Optional[str]
     long_date_format: Optional[str]
     time_format: Optional[str]
     show_relative_dates: Optional[bool]
     enable_color_impaired_mode: Optional[bool]
     ui_language: Optional[int]
-    __properties = ["id", "firstDayOfWeek", "calendarWeekColumnHeader", "shortDateFormat", "longDateFormat", "timeFormat", "showRelativeDates", "enableColorImpairedMode", "uiLanguage"]
+    theme: Optional[str]
+    __properties = ["id", "firstDayOfWeek", "calendarWeekColumnHeader", "shortDateFormat", "longDateFormat", "timeFormat", "showRelativeDates", "enableColorImpairedMode", "uiLanguage", "theme"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -76,14 +77,18 @@
         if self.long_date_format is None:
             _dict['longDateFormat'] = None
 
         # set to None if time_format (nullable) is None
         if self.time_format is None:
             _dict['timeFormat'] = None
 
+        # set to None if theme (nullable) is None
+        if self.theme is None:
+            _dict['theme'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> UiConfigResource:
         """Create an instance of UiConfigResource from a dict"""
         if obj is None:
             return None
@@ -96,11 +101,12 @@
             "first_day_of_week": obj.get("firstDayOfWeek"),
             "calendar_week_column_header": obj.get("calendarWeekColumnHeader"),
             "short_date_format": obj.get("shortDateFormat"),
             "long_date_format": obj.get("longDateFormat"),
             "time_format": obj.get("timeFormat"),
             "show_relative_dates": obj.get("showRelativeDates"),
             "enable_color_impaired_mode": obj.get("enableColorImpairedMode"),
-            "ui_language": obj.get("uiLanguage")
+            "ui_language": obj.get("uiLanguage"),
+            "theme": obj.get("theme")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/update_changes.py` & `readarr-py-0.3.0/readarr/models/profile_format_item_resource.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
+from typing import Optional
 from pydantic import BaseModel
 
-class UpdateChanges(BaseModel):
+class ProfileFormatItemResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    new: Optional[List]
-    fixed: Optional[List]
-    __properties = ["new", "fixed"]
+    id: Optional[int]
+    format: Optional[int]
+    name: Optional[str]
+    score: Optional[int]
+    __properties = ["id", "format", "name", "score"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -43,42 +45,40 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UpdateChanges:
-        """Create an instance of UpdateChanges from a JSON string"""
+    def from_json(cls, json_str: str) -> ProfileFormatItemResource:
+        """Create an instance of ProfileFormatItemResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if new (nullable) is None
-        if self.new is None:
-            _dict['new'] = None
-
-        # set to None if fixed (nullable) is None
-        if self.fixed is None:
-            _dict['fixed'] = None
+        # set to None if name (nullable) is None
+        if self.name is None:
+            _dict['name'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UpdateChanges:
-        """Create an instance of UpdateChanges from a dict"""
+    def from_dict(cls, obj: dict) -> ProfileFormatItemResource:
+        """Create an instance of ProfileFormatItemResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UpdateChanges.parse_obj(obj)
+            return ProfileFormatItemResource.parse_obj(obj)
 
-        _obj = UpdateChanges.parse_obj({
-            "new": obj.get("new"),
-            "fixed": obj.get("fixed")
+        _obj = ProfileFormatItemResource.parse_obj({
+            "id": obj.get("id"),
+            "format": obj.get("format"),
+            "name": obj.get("name"),
+            "score": obj.get("score")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/update_mechanism.py` & `readarr-py-0.3.0/readarr/models/write_audio_tags_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class UpdateMechanism(str, Enum):
+class WriteAudioTagsType(str, Enum):
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
+    NO = 'no'
+    NEWFILES = 'newFiles'
+    ALLFILES = 'allFiles'
+    SYNC = 'sync'
```

### Comparing `readarr-py-0.2.2/readarr/models/update_resource.py` & `readarr-py-0.3.0/readarr/models/update_resource.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
@@ -30,19 +30,20 @@
     id: Optional[int]
     version: Optional[str]
     branch: Optional[str]
     release_date: Optional[datetime]
     file_name: Optional[str]
     url: Optional[str]
     installed: Optional[bool]
+    installed_on: Optional[datetime]
     installable: Optional[bool]
     latest: Optional[bool]
     changes: Optional[UpdateChanges]
     hash: Optional[str]
-    __properties = ["id", "version", "branch", "releaseDate", "fileName", "url", "installed", "installable", "latest", "changes", "hash"]
+    __properties = ["id", "version", "branch", "releaseDate", "fileName", "url", "installed", "installedOn", "installable", "latest", "changes", "hash"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -78,14 +79,18 @@
         if self.file_name is None:
             _dict['fileName'] = None
 
         # set to None if url (nullable) is None
         if self.url is None:
             _dict['url'] = None
 
+        # set to None if installed_on (nullable) is None
+        if self.installed_on is None:
+            _dict['installedOn'] = None
+
         # set to None if hash (nullable) is None
         if self.hash is None:
             _dict['hash'] = None
 
         return _dict
 
     @classmethod
@@ -101,14 +106,15 @@
             "id": obj.get("id"),
             "version": obj.get("version"),
             "branch": obj.get("branch"),
             "release_date": obj.get("releaseDate"),
             "file_name": obj.get("fileName"),
             "url": obj.get("url"),
             "installed": obj.get("installed"),
+            "installed_on": obj.get("installedOn"),
             "installable": obj.get("installable"),
             "latest": obj.get("latest"),
             "changes": UpdateChanges.from_dict(obj.get("changes")) if obj.get("changes") is not None else None,
             "hash": obj.get("hash")
         })
         return _obj
```

### Comparing `readarr-py-0.2.2/readarr/models/write_audio_tags_type.py` & `readarr-py-0.3.0/readarr/models/write_book_tags_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class WriteAudioTagsType(str, Enum):
+class WriteBookTagsType(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    NO = 'no'
     NEWFILES = 'newFiles'
     ALLFILES = 'allFiles'
     SYNC = 'sync'
```

### Comparing `readarr-py-0.2.2/readarr/models/write_book_tags_type.py` & `readarr-py-0.3.0/readarr/models/media_cover_types.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class WriteBookTagsType(str, Enum):
+class MediaCoverTypes(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    NEWFILES = 'newFiles'
-    ALLFILES = 'allFiles'
-    SYNC = 'sync'
+    UNKNOWN = 'unknown'
+    POSTER = 'poster'
+    BANNER = 'banner'
+    FANART = 'fanart'
+    SCREENSHOT = 'screenshot'
+    HEADSHOT = 'headshot'
+    COVER = 'cover'
+    DISC = 'disc'
+    LOGO = 'logo'
```

### Comparing `readarr-py-0.2.2/readarr/rest.py` & `readarr-py-0.3.0/readarr/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Readarr
 
     Readarr API docs  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import io
```

### Comparing `readarr-py-0.2.2/readarr_py.egg-info/PKG-INFO` & `readarr-py-0.3.0/readarr_py.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readarr-py
-Version: 0.2.2
+Version: 0.3.0
 Summary: Readarr API wrapper
 Project-URL: Homepage, https://github.com/devopsarr/readarr-py
 Project-URL: Bug Tracker, https://github.com/devopsarr/readarr-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,18 +13,18 @@
 
 # readarr-py
 Readarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.2.2
+- Package version: 0.3.0
 
 [comment]: # (x-release-please-end)
-- API version: 0.1.0
+- API version: 1.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
@@ -65,87 +65,111 @@
 from __future__ import print_function
 
 import time
 import readarr
 from readarr.rest import ApiException
 from pprint import pprint
 
-# Defining the host is optional and defaults to http://localhost
+# Defining the host is optional and defaults to http://localhost:8787
 # See configuration.py for a list of all supported configuration parameters.
 configuration = readarr.Configuration(
-    host = "http://localhost"
+    host = "http://localhost:8787"
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure API key authorization: apikey
+configuration.api_key['apikey'] = os.environ["API_KEY"]
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['apikey'] = 'Bearer'
+
+# Configure API key authorization: X-Api-Key
+configuration.api_key['X-Api-Key'] = os.environ["API_KEY"]
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['X-Api-Key'] = 'Bearer'
 
 
 # Enter a context with an instance of the API client
 with readarr.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = readarr.AuthenticationApi(api_client)
-    return_url = 'return_url_example' # str |  (optional)
-    username = 'username_example' # str |  (optional)
-    password = 'password_example' # str |  (optional)
-    remember_me = 'remember_me_example' # str |  (optional)
+    api_instance = readarr.ApiInfoApi(api_client)
 
     try:
-        api_instance.create_login(return_url=return_url, username=username, password=password, remember_me=remember_me)
+        api_response = api_instance.get_api()
+        print("The response of ApiInfoApi->get_api:\n")
+        pprint(api_response)
     except ApiException as e:
-        print("Exception when calling AuthenticationApi->create_login: %s\n" % e)
+        print("Exception when calling ApiInfoApi->get_api: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
-All URIs are relative to *http://localhost*
+All URIs are relative to *http://localhost:8787*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
+*ApiInfoApi* | [**get_api**](docs/ApiInfoApi.md#get_api) | **GET** /api | 
 *AuthenticationApi* | [**create_login**](docs/AuthenticationApi.md#create_login) | **POST** /login | 
 *AuthenticationApi* | [**get_logout**](docs/AuthenticationApi.md#get_logout) | **GET** /logout | 
 *AuthorApi* | [**create_author**](docs/AuthorApi.md#create_author) | **POST** /api/v1/author | 
 *AuthorApi* | [**delete_author**](docs/AuthorApi.md#delete_author) | **DELETE** /api/v1/author/{id} | 
 *AuthorApi* | [**get_author_by_id**](docs/AuthorApi.md#get_author_by_id) | **GET** /api/v1/author/{id} | 
 *AuthorApi* | [**list_author**](docs/AuthorApi.md#list_author) | **GET** /api/v1/author | 
 *AuthorApi* | [**update_author**](docs/AuthorApi.md#update_author) | **PUT** /api/v1/author/{id} | 
 *AuthorEditorApi* | [**delete_author_editor**](docs/AuthorEditorApi.md#delete_author_editor) | **DELETE** /api/v1/author/editor | 
 *AuthorEditorApi* | [**put_author_editor**](docs/AuthorEditorApi.md#put_author_editor) | **PUT** /api/v1/author/editor | 
 *AuthorLookupApi* | [**get_author_lookup**](docs/AuthorLookupApi.md#get_author_lookup) | **GET** /api/v1/author/lookup | 
 *BackupApi* | [**create_system_backup_restore_by_id**](docs/BackupApi.md#create_system_backup_restore_by_id) | **POST** /api/v1/system/backup/restore/{id} | 
 *BackupApi* | [**create_system_backup_restore_upload**](docs/BackupApi.md#create_system_backup_restore_upload) | **POST** /api/v1/system/backup/restore/upload | 
 *BackupApi* | [**delete_system_backup**](docs/BackupApi.md#delete_system_backup) | **DELETE** /api/v1/system/backup/{id} | 
 *BackupApi* | [**list_system_backup**](docs/BackupApi.md#list_system_backup) | **GET** /api/v1/system/backup | 
-*BlacklistApi* | [**delete_blacklist**](docs/BlacklistApi.md#delete_blacklist) | **DELETE** /api/v1/blacklist/{id} | 
-*BlacklistApi* | [**delete_blacklist_bulk**](docs/BlacklistApi.md#delete_blacklist_bulk) | **DELETE** /api/v1/blacklist/bulk | 
-*BlacklistApi* | [**get_blacklist**](docs/BlacklistApi.md#get_blacklist) | **GET** /api/v1/blacklist | 
+*BlocklistApi* | [**delete_blocklist**](docs/BlocklistApi.md#delete_blocklist) | **DELETE** /api/v1/blocklist/{id} | 
+*BlocklistApi* | [**delete_blocklist_bulk**](docs/BlocklistApi.md#delete_blocklist_bulk) | **DELETE** /api/v1/blocklist/bulk | 
+*BlocklistApi* | [**get_blocklist**](docs/BlocklistApi.md#get_blocklist) | **GET** /api/v1/blocklist | 
 *BookApi* | [**create_book**](docs/BookApi.md#create_book) | **POST** /api/v1/book | 
 *BookApi* | [**delete_book**](docs/BookApi.md#delete_book) | **DELETE** /api/v1/book/{id} | 
 *BookApi* | [**get_book_by_id**](docs/BookApi.md#get_book_by_id) | **GET** /api/v1/book/{id} | 
+*BookApi* | [**get_bookid_overview**](docs/BookApi.md#get_bookid_overview) | **GET** /api/v1/book/{id}/overview | 
 *BookApi* | [**list_book**](docs/BookApi.md#list_book) | **GET** /api/v1/book | 
 *BookApi* | [**put_book_monitor**](docs/BookApi.md#put_book_monitor) | **PUT** /api/v1/book/monitor | 
 *BookApi* | [**update_book**](docs/BookApi.md#update_book) | **PUT** /api/v1/book/{id} | 
+*BookEditorApi* | [**delete_book_editor**](docs/BookEditorApi.md#delete_book_editor) | **DELETE** /api/v1/book/editor | 
+*BookEditorApi* | [**put_book_editor**](docs/BookEditorApi.md#put_book_editor) | **PUT** /api/v1/book/editor | 
 *BookFileApi* | [**delete_book_file**](docs/BookFileApi.md#delete_book_file) | **DELETE** /api/v1/bookfile/{id} | 
 *BookFileApi* | [**delete_book_file_bulk**](docs/BookFileApi.md#delete_book_file_bulk) | **DELETE** /api/v1/bookfile/bulk | 
 *BookFileApi* | [**get_book_file_by_id**](docs/BookFileApi.md#get_book_file_by_id) | **GET** /api/v1/bookfile/{id} | 
 *BookFileApi* | [**list_book_file**](docs/BookFileApi.md#list_book_file) | **GET** /api/v1/bookfile | 
 *BookFileApi* | [**put_book_file_editor**](docs/BookFileApi.md#put_book_file_editor) | **PUT** /api/v1/bookfile/editor | 
 *BookFileApi* | [**update_book_file**](docs/BookFileApi.md#update_book_file) | **PUT** /api/v1/bookfile/{id} | 
 *BookLookupApi* | [**get_book_lookup**](docs/BookLookupApi.md#get_book_lookup) | **GET** /api/v1/book/lookup | 
 *BookshelfApi* | [**create_bookshelf**](docs/BookshelfApi.md#create_bookshelf) | **POST** /api/v1/bookshelf | 
 *CalendarApi* | [**get_calendar_by_id**](docs/CalendarApi.md#get_calendar_by_id) | **GET** /api/v1/calendar/{id} | 
 *CalendarApi* | [**list_calendar**](docs/CalendarApi.md#list_calendar) | **GET** /api/v1/calendar | 
-*CalendarFeedApi* | [**get_calendar_readarr_ics**](docs/CalendarFeedApi.md#get_calendar_readarr_ics) | **GET** /api/v1/calendar/readarr.ics | 
+*CalendarFeedApi* | [**get_feed_v1_calendar_readarr_ics**](docs/CalendarFeedApi.md#get_feed_v1_calendar_readarr_ics) | **GET** /feed/v1/calendar/readarr.ics | 
 *CommandApi* | [**create_command**](docs/CommandApi.md#create_command) | **POST** /api/v1/command | 
 *CommandApi* | [**delete_command**](docs/CommandApi.md#delete_command) | **DELETE** /api/v1/command/{id} | 
 *CommandApi* | [**get_command_by_id**](docs/CommandApi.md#get_command_by_id) | **GET** /api/v1/command/{id} | 
 *CommandApi* | [**list_command**](docs/CommandApi.md#list_command) | **GET** /api/v1/command | 
 *CustomFilterApi* | [**create_custom_filter**](docs/CustomFilterApi.md#create_custom_filter) | **POST** /api/v1/customfilter | 
 *CustomFilterApi* | [**delete_custom_filter**](docs/CustomFilterApi.md#delete_custom_filter) | **DELETE** /api/v1/customfilter/{id} | 
 *CustomFilterApi* | [**get_custom_filter_by_id**](docs/CustomFilterApi.md#get_custom_filter_by_id) | **GET** /api/v1/customfilter/{id} | 
 *CustomFilterApi* | [**list_custom_filter**](docs/CustomFilterApi.md#list_custom_filter) | **GET** /api/v1/customfilter | 
 *CustomFilterApi* | [**update_custom_filter**](docs/CustomFilterApi.md#update_custom_filter) | **PUT** /api/v1/customfilter/{id} | 
+*CustomFormatApi* | [**create_custom_format**](docs/CustomFormatApi.md#create_custom_format) | **POST** /api/v1/customformat | 
+*CustomFormatApi* | [**delete_custom_format**](docs/CustomFormatApi.md#delete_custom_format) | **DELETE** /api/v1/customformat/{id} | 
+*CustomFormatApi* | [**get_custom_format_by_id**](docs/CustomFormatApi.md#get_custom_format_by_id) | **GET** /api/v1/customformat/{id} | 
+*CustomFormatApi* | [**get_custom_format_schema**](docs/CustomFormatApi.md#get_custom_format_schema) | **GET** /api/v1/customformat/schema | 
+*CustomFormatApi* | [**list_custom_format**](docs/CustomFormatApi.md#list_custom_format) | **GET** /api/v1/customformat | 
+*CustomFormatApi* | [**update_custom_format**](docs/CustomFormatApi.md#update_custom_format) | **PUT** /api/v1/customformat/{id} | 
 *CutoffApi* | [**get_wanted_cutoff**](docs/CutoffApi.md#get_wanted_cutoff) | **GET** /api/v1/wanted/cutoff | 
 *CutoffApi* | [**get_wanted_cutoff_by_id**](docs/CutoffApi.md#get_wanted_cutoff_by_id) | **GET** /api/v1/wanted/cutoff/{id} | 
 *DelayProfileApi* | [**create_delay_profile**](docs/DelayProfileApi.md#create_delay_profile) | **POST** /api/v1/delayprofile | 
 *DelayProfileApi* | [**delete_delay_profile**](docs/DelayProfileApi.md#delete_delay_profile) | **DELETE** /api/v1/delayprofile/{id} | 
 *DelayProfileApi* | [**get_delay_profile_by_id**](docs/DelayProfileApi.md#get_delay_profile_by_id) | **GET** /api/v1/delayprofile/{id} | 
 *DelayProfileApi* | [**list_delay_profile**](docs/DelayProfileApi.md#list_delay_profile) | **GET** /api/v1/delayprofile | 
 *DelayProfileApi* | [**update_delay_profile**](docs/DelayProfileApi.md#update_delay_profile) | **PUT** /api/v1/delayprofile/{id} | 
@@ -162,20 +186,21 @@
 *DownloadClientApi* | [**list_download_client_schema**](docs/DownloadClientApi.md#list_download_client_schema) | **GET** /api/v1/downloadclient/schema | 
 *DownloadClientApi* | [**test_download_client**](docs/DownloadClientApi.md#test_download_client) | **POST** /api/v1/downloadclient/test | 
 *DownloadClientApi* | [**testall_download_client**](docs/DownloadClientApi.md#testall_download_client) | **POST** /api/v1/downloadclient/testall | 
 *DownloadClientApi* | [**update_download_client**](docs/DownloadClientApi.md#update_download_client) | **PUT** /api/v1/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**get_download_client_config**](docs/DownloadClientConfigApi.md#get_download_client_config) | **GET** /api/v1/config/downloadclient | 
 *DownloadClientConfigApi* | [**get_download_client_config_by_id**](docs/DownloadClientConfigApi.md#get_download_client_config_by_id) | **GET** /api/v1/config/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**update_download_client_config**](docs/DownloadClientConfigApi.md#update_download_client_config) | **PUT** /api/v1/config/downloadclient/{id} | 
+*EditionApi* | [**list_edition**](docs/EditionApi.md#list_edition) | **GET** /api/v1/edition | 
 *FileSystemApi* | [**get_file_system**](docs/FileSystemApi.md#get_file_system) | **GET** /api/v1/filesystem | 
 *FileSystemApi* | [**get_file_system_mediafiles**](docs/FileSystemApi.md#get_file_system_mediafiles) | **GET** /api/v1/filesystem/mediafiles | 
 *FileSystemApi* | [**get_file_system_type**](docs/FileSystemApi.md#get_file_system_type) | **GET** /api/v1/filesystem/type | 
 *HealthApi* | [**get_health_by_id**](docs/HealthApi.md#get_health_by_id) | **GET** /api/v1/health/{id} | 
 *HealthApi* | [**list_health**](docs/HealthApi.md#list_health) | **GET** /api/v1/health | 
-*HistoryApi* | [**create_history_failed**](docs/HistoryApi.md#create_history_failed) | **POST** /api/v1/history/failed | 
+*HistoryApi* | [**create_history_failed_by_id**](docs/HistoryApi.md#create_history_failed_by_id) | **POST** /api/v1/history/failed/{id} | 
 *HistoryApi* | [**get_history**](docs/HistoryApi.md#get_history) | **GET** /api/v1/history | 
 *HistoryApi* | [**list_history_author**](docs/HistoryApi.md#list_history_author) | **GET** /api/v1/history/author | 
 *HistoryApi* | [**list_history_since**](docs/HistoryApi.md#list_history_since) | **GET** /api/v1/history/since | 
 *HostConfigApi* | [**get_host_config**](docs/HostConfigApi.md#get_host_config) | **GET** /api/v1/config/host | 
 *HostConfigApi* | [**get_host_config_by_id**](docs/HostConfigApi.md#get_host_config_by_id) | **GET** /api/v1/config/host/{id} | 
 *HostConfigApi* | [**update_host_config**](docs/HostConfigApi.md#update_host_config) | **PUT** /api/v1/config/host/{id} | 
 *ImportListApi* | [**create_import_list**](docs/ImportListApi.md#create_import_list) | **POST** /api/v1/importlist | 
@@ -207,16 +232,16 @@
 *InitializeJsApi* | [**get_initialize_js**](docs/InitializeJsApi.md#get_initialize_js) | **GET** /initialize.js | 
 *LanguageApi* | [**get_language_by_id**](docs/LanguageApi.md#get_language_by_id) | **GET** /api/v1/language/{id} | 
 *LanguageApi* | [**list_language**](docs/LanguageApi.md#list_language) | **GET** /api/v1/language | 
 *LocalizationApi* | [**get_localization**](docs/LocalizationApi.md#get_localization) | **GET** /api/v1/localization | 
 *LogApi* | [**get_log**](docs/LogApi.md#get_log) | **GET** /api/v1/log | 
 *LogFileApi* | [**get_log_file_by_filename**](docs/LogFileApi.md#get_log_file_by_filename) | **GET** /api/v1/log/file/{filename} | 
 *LogFileApi* | [**list_log_file**](docs/LogFileApi.md#list_log_file) | **GET** /api/v1/log/file | 
+*ManualImportApi* | [**create_manual_import**](docs/ManualImportApi.md#create_manual_import) | **POST** /api/v1/manualimport | 
 *ManualImportApi* | [**list_manual_import**](docs/ManualImportApi.md#list_manual_import) | **GET** /api/v1/manualimport | 
-*ManualImportApi* | [**put_manual_import**](docs/ManualImportApi.md#put_manual_import) | **PUT** /api/v1/manualimport | 
 *MediaCoverApi* | [**get_media_cover_authorauthor_id_by_filename**](docs/MediaCoverApi.md#get_media_cover_authorauthor_id_by_filename) | **GET** /api/v1/mediacover/author/{authorId}/{filename} | 
 *MediaCoverApi* | [**get_media_cover_bookbook_id_by_filename**](docs/MediaCoverApi.md#get_media_cover_bookbook_id_by_filename) | **GET** /api/v1/mediacover/book/{bookId}/{filename} | 
 *MediaManagementConfigApi* | [**get_media_management_config**](docs/MediaManagementConfigApi.md#get_media_management_config) | **GET** /api/v1/config/mediamanagement | 
 *MediaManagementConfigApi* | [**get_media_management_config_by_id**](docs/MediaManagementConfigApi.md#get_media_management_config_by_id) | **GET** /api/v1/config/mediamanagement/{id} | 
 *MediaManagementConfigApi* | [**update_media_management_config**](docs/MediaManagementConfigApi.md#update_media_management_config) | **PUT** /api/v1/config/mediamanagement/{id} | 
 *MetadataApi* | [**create_metadata**](docs/MetadataApi.md#create_metadata) | **POST** /api/v1/metadata | 
 *MetadataApi* | [**create_metadata_action_by_name**](docs/MetadataApi.md#create_metadata_action_by_name) | **POST** /api/v1/metadata/action/{name} | 
@@ -248,14 +273,15 @@
 *NotificationApi* | [**get_notification_by_id**](docs/NotificationApi.md#get_notification_by_id) | **GET** /api/v1/notification/{id} | 
 *NotificationApi* | [**list_notification**](docs/NotificationApi.md#list_notification) | **GET** /api/v1/notification | 
 *NotificationApi* | [**list_notification_schema**](docs/NotificationApi.md#list_notification_schema) | **GET** /api/v1/notification/schema | 
 *NotificationApi* | [**test_notification**](docs/NotificationApi.md#test_notification) | **POST** /api/v1/notification/test | 
 *NotificationApi* | [**testall_notification**](docs/NotificationApi.md#testall_notification) | **POST** /api/v1/notification/testall | 
 *NotificationApi* | [**update_notification**](docs/NotificationApi.md#update_notification) | **PUT** /api/v1/notification/{id} | 
 *ParseApi* | [**get_parse**](docs/ParseApi.md#get_parse) | **GET** /api/v1/parse | 
+*PingApi* | [**get_ping**](docs/PingApi.md#get_ping) | **GET** /ping | 
 *QualityDefinitionApi* | [**get_quality_definition_by_id**](docs/QualityDefinitionApi.md#get_quality_definition_by_id) | **GET** /api/v1/qualitydefinition/{id} | 
 *QualityDefinitionApi* | [**list_quality_definition**](docs/QualityDefinitionApi.md#list_quality_definition) | **GET** /api/v1/qualitydefinition | 
 *QualityDefinitionApi* | [**put_quality_definition_update**](docs/QualityDefinitionApi.md#put_quality_definition_update) | **PUT** /api/v1/qualitydefinition/update | 
 *QualityDefinitionApi* | [**update_quality_definition**](docs/QualityDefinitionApi.md#update_quality_definition) | **PUT** /api/v1/qualitydefinition/{id} | 
 *QualityProfileApi* | [**create_quality_profile**](docs/QualityProfileApi.md#create_quality_profile) | **POST** /api/v1/qualityprofile | 
 *QualityProfileApi* | [**delete_quality_profile**](docs/QualityProfileApi.md#delete_quality_profile) | **DELETE** /api/v1/qualityprofile/{id} | 
 *QualityProfileApi* | [**get_quality_profile_by_id**](docs/QualityProfileApi.md#get_quality_profile_by_id) | **GET** /api/v1/qualityprofile/{id} | 
@@ -323,32 +349,34 @@
 
 
 ## Documentation For Models
 
  - [AddAuthorOptions](docs/AddAuthorOptions.md)
  - [AddBookOptions](docs/AddBookOptions.md)
  - [AllowFingerprinting](docs/AllowFingerprinting.md)
+ - [ApiInfoResource](docs/ApiInfoResource.md)
  - [ApplyTags](docs/ApplyTags.md)
  - [AuthenticationType](docs/AuthenticationType.md)
  - [Author](docs/Author.md)
  - [AuthorEditorResource](docs/AuthorEditorResource.md)
  - [AuthorLazyLoaded](docs/AuthorLazyLoaded.md)
  - [AuthorMetadata](docs/AuthorMetadata.md)
  - [AuthorMetadataLazyLoaded](docs/AuthorMetadataLazyLoaded.md)
  - [AuthorResource](docs/AuthorResource.md)
  - [AuthorStatisticsResource](docs/AuthorStatisticsResource.md)
  - [AuthorStatusType](docs/AuthorStatusType.md)
  - [AuthorTitleInfo](docs/AuthorTitleInfo.md)
  - [BackupResource](docs/BackupResource.md)
  - [BackupType](docs/BackupType.md)
- - [BlacklistBulkResource](docs/BlacklistBulkResource.md)
- - [BlacklistResource](docs/BlacklistResource.md)
- - [BlacklistResourcePagingResource](docs/BlacklistResourcePagingResource.md)
+ - [BlocklistBulkResource](docs/BlocklistBulkResource.md)
+ - [BlocklistResource](docs/BlocklistResource.md)
+ - [BlocklistResourcePagingResource](docs/BlocklistResourcePagingResource.md)
  - [Book](docs/Book.md)
  - [BookAddType](docs/BookAddType.md)
+ - [BookEditorResource](docs/BookEditorResource.md)
  - [BookFile](docs/BookFile.md)
  - [BookFileListLazyLoaded](docs/BookFileListLazyLoaded.md)
  - [BookFileListResource](docs/BookFileListResource.md)
  - [BookFileResource](docs/BookFileResource.md)
  - [BookLazyLoaded](docs/BookLazyLoaded.md)
  - [BookListLazyLoaded](docs/BookListLazyLoaded.md)
  - [BookResource](docs/BookResource.md)
@@ -360,63 +388,73 @@
  - [CertificateValidationType](docs/CertificateValidationType.md)
  - [Command](docs/Command.md)
  - [CommandPriority](docs/CommandPriority.md)
  - [CommandResource](docs/CommandResource.md)
  - [CommandStatus](docs/CommandStatus.md)
  - [CommandTrigger](docs/CommandTrigger.md)
  - [CustomFilterResource](docs/CustomFilterResource.md)
+ - [CustomFormat](docs/CustomFormat.md)
+ - [CustomFormatResource](docs/CustomFormatResource.md)
+ - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
+ - [DatabaseType](docs/DatabaseType.md)
  - [DelayProfileResource](docs/DelayProfileResource.md)
  - [DevelopmentConfigResource](docs/DevelopmentConfigResource.md)
  - [DiskSpaceResource](docs/DiskSpaceResource.md)
  - [DownloadClientConfigResource](docs/DownloadClientConfigResource.md)
  - [DownloadClientResource](docs/DownloadClientResource.md)
  - [DownloadProtocol](docs/DownloadProtocol.md)
  - [Edition](docs/Edition.md)
  - [EditionLazyLoaded](docs/EditionLazyLoaded.md)
  - [EditionListLazyLoaded](docs/EditionListLazyLoaded.md)
  - [EditionResource](docs/EditionResource.md)
+ - [EntityHistoryEventType](docs/EntityHistoryEventType.md)
  - [Field](docs/Field.md)
  - [FileDateType](docs/FileDateType.md)
  - [HealthCheckResult](docs/HealthCheckResult.md)
  - [HealthResource](docs/HealthResource.md)
- - [HistoryEventType](docs/HistoryEventType.md)
  - [HistoryResource](docs/HistoryResource.md)
  - [HistoryResourcePagingResource](docs/HistoryResourcePagingResource.md)
  - [HostConfigResource](docs/HostConfigResource.md)
+ - [ICustomFormatSpecification](docs/ICustomFormatSpecification.md)
  - [ImportListExclusionResource](docs/ImportListExclusionResource.md)
  - [ImportListMonitorType](docs/ImportListMonitorType.md)
  - [ImportListResource](docs/ImportListResource.md)
  - [ImportListType](docs/ImportListType.md)
  - [IndexerConfigResource](docs/IndexerConfigResource.md)
  - [IndexerResource](docs/IndexerResource.md)
  - [IsoCountry](docs/IsoCountry.md)
  - [LanguageResource](docs/LanguageResource.md)
  - [Links](docs/Links.md)
  - [LogFileResource](docs/LogFileResource.md)
  - [LogResource](docs/LogResource.md)
  - [LogResourcePagingResource](docs/LogResourcePagingResource.md)
  - [ManualImportResource](docs/ManualImportResource.md)
+ - [ManualImportUpdateResource](docs/ManualImportUpdateResource.md)
  - [MediaCover](docs/MediaCover.md)
  - [MediaCoverTypes](docs/MediaCoverTypes.md)
  - [MediaInfoModel](docs/MediaInfoModel.md)
  - [MediaInfoResource](docs/MediaInfoResource.md)
  - [MediaManagementConfigResource](docs/MediaManagementConfigResource.md)
  - [MetadataProfile](docs/MetadataProfile.md)
  - [MetadataProfileLazyLoaded](docs/MetadataProfileLazyLoaded.md)
  - [MetadataProfileResource](docs/MetadataProfileResource.md)
  - [MetadataProviderConfigResource](docs/MetadataProviderConfigResource.md)
  - [MetadataResource](docs/MetadataResource.md)
  - [MonitorTypes](docs/MonitorTypes.md)
  - [MonitoringOptions](docs/MonitoringOptions.md)
  - [NamingConfigResource](docs/NamingConfigResource.md)
+ - [NewItemMonitorTypes](docs/NewItemMonitorTypes.md)
  - [NotificationResource](docs/NotificationResource.md)
  - [PagingResourceFilter](docs/PagingResourceFilter.md)
  - [ParseResource](docs/ParseResource.md)
  - [ParsedBookInfo](docs/ParsedBookInfo.md)
  - [ParsedTrackInfo](docs/ParsedTrackInfo.md)
+ - [PingResource](docs/PingResource.md)
+ - [ProfileFormatItem](docs/ProfileFormatItem.md)
+ - [ProfileFormatItemResource](docs/ProfileFormatItemResource.md)
  - [ProperDownloadTypes](docs/ProperDownloadTypes.md)
  - [ProviderMessage](docs/ProviderMessage.md)
  - [ProviderMessageType](docs/ProviderMessageType.md)
  - [ProxyType](docs/ProxyType.md)
  - [Quality](docs/Quality.md)
  - [QualityDefinitionResource](docs/QualityDefinitionResource.md)
  - [QualityModel](docs/QualityModel.md)
@@ -436,24 +474,25 @@
  - [ReleaseResource](docs/ReleaseResource.md)
  - [RemotePathMappingResource](docs/RemotePathMappingResource.md)
  - [RenameBookResource](docs/RenameBookResource.md)
  - [RescanAfterRefreshType](docs/RescanAfterRefreshType.md)
  - [RetagBookResource](docs/RetagBookResource.md)
  - [Revision](docs/Revision.md)
  - [RootFolderResource](docs/RootFolderResource.md)
+ - [RuntimeMode](docs/RuntimeMode.md)
  - [SelectOption](docs/SelectOption.md)
  - [Series](docs/Series.md)
  - [SeriesBookLink](docs/SeriesBookLink.md)
  - [SeriesBookLinkListLazyLoaded](docs/SeriesBookLinkListLazyLoaded.md)
  - [SeriesBookLinkResource](docs/SeriesBookLinkResource.md)
  - [SeriesLazyLoaded](docs/SeriesLazyLoaded.md)
  - [SeriesListLazyLoaded](docs/SeriesListLazyLoaded.md)
  - [SeriesResource](docs/SeriesResource.md)
  - [SortDirection](docs/SortDirection.md)
- - [StringInt32KeyValuePair](docs/StringInt32KeyValuePair.md)
+ - [SystemResource](docs/SystemResource.md)
  - [TagDetailsResource](docs/TagDetailsResource.md)
  - [TagDifference](docs/TagDifference.md)
  - [TagResource](docs/TagResource.md)
  - [TaskResource](docs/TaskResource.md)
  - [TrackedDownloadState](docs/TrackedDownloadState.md)
  - [TrackedDownloadStatus](docs/TrackedDownloadStatus.md)
  - [TrackedDownloadStatusMessage](docs/TrackedDownloadStatusMessage.md)
@@ -463,14 +502,27 @@
  - [UpdateResource](docs/UpdateResource.md)
  - [WriteAudioTagsType](docs/WriteAudioTagsType.md)
  - [WriteBookTagsType](docs/WriteBookTagsType.md)
 
 
 ## Documentation For Authorization
 
- All endpoints do not require authorization.
+
+## X-Api-Key
+
+- **Type**: API key
+- **API key parameter name**: X-Api-Key
+- **Location**: HTTP header
+
+
+## apikey
+
+- **Type**: API key
+- **API key parameter name**: apikey
+- **Location**: URL query string
+
 
 ## Author
```

### Comparing `readarr-py-0.2.2/readarr_py.egg-info/SOURCES.txt` & `readarr-py-0.3.0/readarr_py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 readarr/__init__.py
 readarr/api_client.py
+readarr/api_response.py
 readarr/configuration.py
 readarr/exceptions.py
 readarr/rest.py
 readarr/api/__init__.py
+readarr/api/api_info_api.py
 readarr/api/authentication_api.py
 readarr/api/author_api.py
 readarr/api/author_editor_api.py
 readarr/api/author_lookup_api.py
 readarr/api/backup_api.py
-readarr/api/blacklist_api.py
+readarr/api/blocklist_api.py
 readarr/api/book_api.py
+readarr/api/book_editor_api.py
 readarr/api/book_file_api.py
 readarr/api/book_lookup_api.py
 readarr/api/bookshelf_api.py
 readarr/api/calendar_api.py
 readarr/api/calendar_feed_api.py
 readarr/api/command_api.py
 readarr/api/custom_filter_api.py
+readarr/api/custom_format_api.py
 readarr/api/cutoff_api.py
 readarr/api/delay_profile_api.py
 readarr/api/development_config_api.py
 readarr/api/disk_space_api.py
 readarr/api/download_client_api.py
 readarr/api/download_client_config_api.py
+readarr/api/edition_api.py
 readarr/api/file_system_api.py
 readarr/api/health_api.py
 readarr/api/history_api.py
 readarr/api/host_config_api.py
 readarr/api/import_list_api.py
 readarr/api/import_list_exclusion_api.py
 readarr/api/indexer_api.py
@@ -48,14 +53,15 @@
 readarr/api/metadata_profile_api.py
 readarr/api/metadata_profile_schema_api.py
 readarr/api/metadata_provider_config_api.py
 readarr/api/missing_api.py
 readarr/api/naming_config_api.py
 readarr/api/notification_api.py
 readarr/api/parse_api.py
+readarr/api/ping_api.py
 readarr/api/quality_definition_api.py
 readarr/api/quality_profile_api.py
 readarr/api/quality_profile_schema_api.py
 readarr/api/queue_action_api.py
 readarr/api/queue_api.py
 readarr/api/queue_details_api.py
 readarr/api/queue_status_api.py
@@ -76,32 +82,34 @@
 readarr/api/ui_config_api.py
 readarr/api/update_api.py
 readarr/api/update_log_file_api.py
 readarr/models/__init__.py
 readarr/models/add_author_options.py
 readarr/models/add_book_options.py
 readarr/models/allow_fingerprinting.py
+readarr/models/api_info_resource.py
 readarr/models/apply_tags.py
 readarr/models/authentication_type.py
 readarr/models/author.py
 readarr/models/author_editor_resource.py
 readarr/models/author_lazy_loaded.py
 readarr/models/author_metadata.py
 readarr/models/author_metadata_lazy_loaded.py
 readarr/models/author_resource.py
 readarr/models/author_statistics_resource.py
 readarr/models/author_status_type.py
 readarr/models/author_title_info.py
 readarr/models/backup_resource.py
 readarr/models/backup_type.py
-readarr/models/blacklist_bulk_resource.py
-readarr/models/blacklist_resource.py
-readarr/models/blacklist_resource_paging_resource.py
+readarr/models/blocklist_bulk_resource.py
+readarr/models/blocklist_resource.py
+readarr/models/blocklist_resource_paging_resource.py
 readarr/models/book.py
 readarr/models/book_add_type.py
+readarr/models/book_editor_resource.py
 readarr/models/book_file.py
 readarr/models/book_file_list_lazy_loaded.py
 readarr/models/book_file_list_resource.py
 readarr/models/book_file_resource.py
 readarr/models/book_lazy_loaded.py
 readarr/models/book_list_lazy_loaded.py
 readarr/models/book_resource.py
@@ -113,63 +121,73 @@
 readarr/models/certificate_validation_type.py
 readarr/models/command.py
 readarr/models/command_priority.py
 readarr/models/command_resource.py
 readarr/models/command_status.py
 readarr/models/command_trigger.py
 readarr/models/custom_filter_resource.py
+readarr/models/custom_format.py
+readarr/models/custom_format_resource.py
+readarr/models/custom_format_specification_schema.py
+readarr/models/database_type.py
 readarr/models/delay_profile_resource.py
 readarr/models/development_config_resource.py
 readarr/models/disk_space_resource.py
 readarr/models/download_client_config_resource.py
 readarr/models/download_client_resource.py
 readarr/models/download_protocol.py
 readarr/models/edition.py
 readarr/models/edition_lazy_loaded.py
 readarr/models/edition_list_lazy_loaded.py
 readarr/models/edition_resource.py
+readarr/models/entity_history_event_type.py
 readarr/models/field.py
 readarr/models/file_date_type.py
 readarr/models/health_check_result.py
 readarr/models/health_resource.py
-readarr/models/history_event_type.py
 readarr/models/history_resource.py
 readarr/models/history_resource_paging_resource.py
 readarr/models/host_config_resource.py
+readarr/models/i_custom_format_specification.py
 readarr/models/import_list_exclusion_resource.py
 readarr/models/import_list_monitor_type.py
 readarr/models/import_list_resource.py
 readarr/models/import_list_type.py
 readarr/models/indexer_config_resource.py
 readarr/models/indexer_resource.py
 readarr/models/iso_country.py
 readarr/models/language_resource.py
 readarr/models/links.py
 readarr/models/log_file_resource.py
 readarr/models/log_resource.py
 readarr/models/log_resource_paging_resource.py
 readarr/models/manual_import_resource.py
+readarr/models/manual_import_update_resource.py
 readarr/models/media_cover.py
 readarr/models/media_cover_types.py
 readarr/models/media_info_model.py
 readarr/models/media_info_resource.py
 readarr/models/media_management_config_resource.py
 readarr/models/metadata_profile.py
 readarr/models/metadata_profile_lazy_loaded.py
 readarr/models/metadata_profile_resource.py
 readarr/models/metadata_provider_config_resource.py
 readarr/models/metadata_resource.py
 readarr/models/monitor_types.py
 readarr/models/monitoring_options.py
 readarr/models/naming_config_resource.py
+readarr/models/new_item_monitor_types.py
 readarr/models/notification_resource.py
 readarr/models/paging_resource_filter.py
 readarr/models/parse_resource.py
 readarr/models/parsed_book_info.py
 readarr/models/parsed_track_info.py
+readarr/models/ping_resource.py
+readarr/models/profile_format_item.py
+readarr/models/profile_format_item_resource.py
 readarr/models/proper_download_types.py
 readarr/models/provider_message.py
 readarr/models/provider_message_type.py
 readarr/models/proxy_type.py
 readarr/models/quality.py
 readarr/models/quality_definition_resource.py
 readarr/models/quality_model.py
@@ -189,24 +207,25 @@
 readarr/models/release_resource.py
 readarr/models/remote_path_mapping_resource.py
 readarr/models/rename_book_resource.py
 readarr/models/rescan_after_refresh_type.py
 readarr/models/retag_book_resource.py
 readarr/models/revision.py
 readarr/models/root_folder_resource.py
+readarr/models/runtime_mode.py
 readarr/models/select_option.py
 readarr/models/series.py
 readarr/models/series_book_link.py
 readarr/models/series_book_link_list_lazy_loaded.py
 readarr/models/series_book_link_resource.py
 readarr/models/series_lazy_loaded.py
 readarr/models/series_list_lazy_loaded.py
 readarr/models/series_resource.py
 readarr/models/sort_direction.py
-readarr/models/string_int32_key_value_pair.py
+readarr/models/system_resource.py
 readarr/models/tag_details_resource.py
 readarr/models/tag_difference.py
 readarr/models/tag_resource.py
 readarr/models/task_resource.py
 readarr/models/tracked_download_state.py
 readarr/models/tracked_download_status.py
 readarr/models/tracked_download_status_message.py
```

