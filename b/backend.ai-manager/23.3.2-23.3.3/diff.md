# Comparing `tmp/backend.ai-manager-23.3.2.tar.gz` & `tmp/backend.ai-manager-23.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-manager-23.3.2.tar", last modified: Fri May  5 07:08:25 2023, max compression
+gzip compressed data, was "backend.ai-manager-23.3.3.tar", last modified: Thu May 25 17:30:38 2023, max compression
```

## Comparing `backend.ai-manager-23.3.2.tar` & `backend.ai-manager-23.3.3.tar`

### file list

```diff
@@ -1,240 +1,244 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:25.834619 backend.ai-manager-23.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-05-05 07:08:25.834619 backend.ai-manager-23.3.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:25.786618 backend.ai-manager-23.3.2/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:25.786618 backend.ai-manager-23.3.2/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:25.790618 backend.ai-manager-23.3.2/ai/backend/manager/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:25.798618 backend.ai-manager-23.3.2/ai/backend/manager/api/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    37001 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/domainconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    15041 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/groupconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (123)    36500 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    21340 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/service.py
--rw-r--r--   0 runner    (1001) docker     (123)   112264 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/session_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    32921 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/userconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   117914 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/api/wsproxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:25.798618 backend.ai-manager-23.3.2/ai/backend/manager/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/cli/dbschema.py
--rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/cli/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/cli/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/cli/gql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/cli/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/cli/image_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    25517 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:25.798618 backend.ai-manager-23.3.2/ai/backend/manager/container_registry/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/container_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/container_registry/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/container_registry/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/container_registry/harbor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/container_registry/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    39619 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/idle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:25.806618 backend.ai-manager-23.3.2/ai/backend/manager/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    21710 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:25.810618 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:25.830619 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/06184d82a211_add_session_creation_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/0e558d06e0e3_add_service_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/0f7a4b643940_.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/1e673659b283_add_clusterized_column_to_agents_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/213a04e90ecf_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/360af8f33d4e_merge_f83d_and_1f55.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/36b69ddee76e_.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/3cf19d906e71_.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/3f1dafab60b2_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9112 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/51dddd79aa21_add_logs_column_on_kernel_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/57e717103287_rename_clone_allowed_to_cloneable.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/5e88398bc340_add_unmanaged_path_column_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/65c4a109bbc7_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/95f51fc6ffdb_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/97f6c80c8aa5_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/a7ca9f175d5f_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py
--rw-r--r--   0 runner    (1001) docker     (123)    23603 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/bf4bae8f942e_add_kernel_host.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/c1409ad0e8da_.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/c3e74dcf1808_add_environ_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/d643752544de_.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/dc9b66466e43_remove_clusterized.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/eec98e65902a_merge_with_vfolder_clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/ff4bfca66bf8_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33845 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/dotfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/error_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    48343 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/gql.py
--rw-r--r--   0 runner    (1001) docker     (123)    24553 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    31774 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)    20630 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/keypair.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:25.830619 backend.ai-manager-23.3.2/ai/backend/manager/models/minilang/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/minilang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/minilang/ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/minilang/queryfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/resource_preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)    23731 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    54071 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/session_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    41915 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    45109 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/models/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/pglock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:25.834619 backend.ai-manager-23.3.2/ai/backend/manager/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/plugin/error_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/plugin/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/plugin/webapp.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   113474 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:25.834619 backend.ai-manager-23.3.2/ai/backend/manager/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52451 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/scheduler/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/scheduler/drf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/scheduler/fifo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/scheduler/mof.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/scheduler/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/scheduler/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    29977 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/ai/backend/manager/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:25.834619 backend.ai-manager-23.3.2/backend.ai_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/backend.ai_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13894 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/backend.ai_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/backend.ai_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/backend.ai_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/backend.ai_manager.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/backend.ai_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/backend.ai_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/backend.ai_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:08:25.834619 backend.ai-manager-23.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-05-05 07:08:25.000000 backend.ai-manager-23.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:38.481117 backend.ai-manager-23.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-25 17:30:38.481117 backend.ai-manager-23.3.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:38.425116 backend.ai-manager-23.3.3/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:38.425116 backend.ai-manager-23.3.3/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:38.429117 backend.ai-manager-23.3.3/ai/backend/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:38.437116 backend.ai-manager-23.3.3/ai/backend/manager/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40846 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/domainconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/groupconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36500 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21340 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111747 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32921 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/userconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117914 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/api/wsproxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:38.437116 backend.ai-manager-23.3.3/ai/backend/manager/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/cli/dbschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/cli/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/cli/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/cli/gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/cli/image_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25764 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:38.441117 backend.ai-manager-23.3.3/ai/backend/manager/container_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/container_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/container_registry/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/container_registry/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/container_registry/harbor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/container_registry/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39619 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/idle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:38.445117 backend.ai-manager-23.3.3/ai/backend/manager/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21947 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:38.445117 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:38.473117 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/06184d82a211_add_session_creation_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/0e558d06e0e3_add_service_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/0f7a4b643940_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/1e673659b283_add_clusterized_column_to_agents_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/213a04e90ecf_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/360af8f33d4e_merge_f83d_and_1f55.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/36b69ddee76e_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/3cf19d906e71_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/3f1dafab60b2_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9112 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/51dddd79aa21_add_logs_column_on_kernel_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/57e717103287_rename_clone_allowed_to_cloneable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/5e88398bc340_add_unmanaged_path_column_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/65c4a109bbc7_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/95f51fc6ffdb_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/97f6c80c8aa5_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/a7ca9f175d5f_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29414 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/bf4bae8f942e_add_kernel_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/c1409ad0e8da_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/c3e74dcf1808_add_environ_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/d643752544de_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/dc9b66466e43_remove_clusterized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/eec98e65902a_merge_with_vfolder_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/ff4bfca66bf8_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33845 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/dotfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/error_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48343 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24553 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31774 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51030 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20630 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/keypair.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:38.477117 backend.ai-manager-23.3.3/ai/backend/manager/models/minilang/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/minilang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/minilang/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/minilang/queryfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/resource_preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23731 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54702 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42526 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45109 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/models/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/pglock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:38.477117 backend.ai-manager-23.3.3/ai/backend/manager/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/plugin/error_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/plugin/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/plugin/webapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   115135 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:38.477117 backend.ai-manager-23.3.3/ai/backend/manager/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52978 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/scheduler/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/scheduler/drf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/scheduler/fifo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/scheduler/mof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/scheduler/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/scheduler/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29977 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/ai/backend/manager/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:38.481117 backend.ai-manager-23.3.3/backend.ai_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-25 17:30:38.000000 backend.ai-manager-23.3.3/backend.ai_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-05-25 17:30:38.000000 backend.ai-manager-23.3.3/backend.ai_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:38.000000 backend.ai-manager-23.3.3/backend.ai_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-25 17:30:38.000000 backend.ai-manager-23.3.3/backend.ai_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:38.000000 backend.ai-manager-23.3.3/backend.ai_manager.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:38.000000 backend.ai-manager-23.3.3/backend.ai_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-25 17:30:38.000000 backend.ai-manager-23.3.3/backend.ai_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-25 17:30:38.000000 backend.ai-manager-23.3.3/backend.ai_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:30:38.481117 backend.ai-manager-23.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    11630 2023-05-25 17:30:37.000000 backend.ai-manager-23.3.3/setup.py
```

### Comparing `backend.ai-manager-23.3.2/PKG-INFO` & `backend.ai-manager-23.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-manager
-Version: 23.3.2
+Version: 23.3.3
 Summary: Backend.AI Manager
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Requires-Python: >=3.11,<3.12
 Description-Content-Type: text/markdown
 
 Backend.AI Manager with API Gateway
 ===================================
```

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/acl.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/admin.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/admin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/auth.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import functools
 import hashlib
 import hmac
 import logging
 import secrets
 from collections import ChainMap
 from datetime import datetime, timedelta
@@ -23,30 +25,40 @@
 from ai.backend.common.plugin.hook import ALL_COMPLETED, FIRST_COMPLETED, PASSED
 from ai.backend.common.types import ReadableCIDR
 
 from ..models import keypair_resource_policies, keypairs, users
 from ..models.group import association_groups_users, groups
 from ..models.keypair import generate_keypair as _gen_keypair
 from ..models.keypair import generate_ssh_keypair as _gen_ssh_keypair
-from ..models.user import INACTIVE_USER_STATUSES, UserRole, UserStatus, check_credential
+from ..models.user import (
+    INACTIVE_USER_STATUSES,
+    UserRole,
+    UserStatus,
+    check_credential,
+    compare_to_hashed_password,
+)
 from ..models.utils import execute_with_retry
 from .exceptions import (
     AuthorizationFailed,
     GenericBadRequest,
     GenericForbidden,
     InternalServerError,
     InvalidAPIParameters,
     InvalidAuthParameters,
     ObjectNotFound,
+    PasswordExpired,
     RejectedByHook,
 )
 from .types import CORSOptions, WebMiddleware
 from .utils import check_api_params, get_handler_attr, set_handler_attr
 
 if TYPE_CHECKING:
+    from sqlalchemy.engine.row import Row
+
+    from ..models.utils import ExtendedAsyncSAEngine
     from .context import RootContext
 
 log: Final = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
 
 _whois_timezone_info: Final = {
     "A": 1 * 3600,
     "ACDT": 10.5 * 3600,
@@ -388,14 +400,32 @@
     except InvalidIpAddressValue:
         raise InvalidAuthParameters(f"{raw_client_addr} is invalid IP address value")
     if any(client_addr.address in allowed_ip_cand.address for allowed_ip_cand in allowed_client_ip):
         return
     raise AuthorizationFailed(f"'{client_addr}' is not allowed IP address")
 
 
+async def check_password_age(
+    db: ExtendedAsyncSAEngine, user: Row, auth_config: Mapping[str, Any] | None
+) -> None:
+    if (
+        auth_config is not None
+        and (max_password_age := auth_config["max_password_age"]) is not None
+    ):
+        password_changed_at: datetime = user.users_password_changed_at
+
+        async with db.begin_readonly() as db_conn:
+            current_dt: datetime = await db_conn.scalar(sa.select(sa.func.now()))
+            if password_changed_at + max_password_age < current_dt:
+                # Force user to update password
+                raise PasswordExpired(
+                    extra_msg=f"Password expired on {password_changed_at + max_password_age}."
+                )
+
+
 @web.middleware
 async def auth_middleware(request: web.Request, handler) -> web.StreamResponse:
     """
     Fetches user information and sets up keypair, uesr, and is_authorized
     attributes.
     """
     # This is a global middleware: request.app is the root app.
@@ -680,14 +710,15 @@
             )
             .order_by(sa.desc(keypairs.c.is_admin))
         )
         result = await conn.execute(query)
         keypair = result.first()
     if keypair is None:
         raise AuthorizationFailed("No API keypairs found.")
+    await check_password_age(root_ctx.db, user, root_ctx.shared_config["auth"])
     # [Hooking point for POST_AUTHORIZE]
     # The hook handlers should accept a tuple of the request, user, and keypair objects.
     hook_result = await root_ctx.hook_plugin_ctx.dispatch(
         "POST_AUTHORIZE",
         (request, params, user, keypair),
         return_when=FIRST_COMPLETED,
     )
@@ -927,15 +958,15 @@
 
     user = await check_credential(root_ctx.db, domain_name, email, params["old_password"])
     if user is None:
         log.info(log_fmt + ": old password mismtach", *log_args)
         raise AuthorizationFailed("Old password mismatch")
     if params["new_password"] != params["new_password2"]:
         log.info(log_fmt + ": new password mismtach", *log_args)
-        return web.json_response({"error_msg": "new password mismitch"}, status=400)
+        return web.json_response({"error_msg": "new password mismatch"}, status=400)
 
     # [Hooking point for VERIFY_PASSWORD_FORMAT with the ALL_COMPLETED requirement]
     # The hook handlers should accept the request and whole ``params` dict.
     # They should return None if the validation is successful and raise the
     # Reject error otherwise.
     hook_result = await root_ctx.hook_plugin_ctx.dispatch(
         "VERIFY_PASSWORD_FORMAT",
@@ -947,20 +978,91 @@
         raise RejectedByHook.from_hook_result(hook_result)
 
     async with root_ctx.db.begin() as conn:
         # Update user password.
         data = {
             "password": params["new_password"],
             "need_password_change": False,
+            "password_changed_at": sa.func.now(),
         }
         query = users.update().values(data).where(users.c.email == email)
         await conn.execute(query)
     return web.json_response({}, status=200)
 
 
+@check_api_params(
+    t.Dict(
+        {
+            t.Key("domain"): t.String,
+            t.Key("username"): t.String,
+            t.Key("current_password"): t.String,
+            t.Key("new_password"): t.String,
+        }
+    )
+)
+async def update_password_no_auth(request: web.Request, params: Any) -> web.Response:
+    """
+    Update user's password without any authorization
+    to allows users to update passwords that have expired
+    because it's been too long since a user changed the password.
+    """
+
+    root_ctx: RootContext = request.app["_root.context"]
+    log_fmt = "AUTH.UPDATE_PASSWORD_NO_AUTH(d:{}, u:{}, passwd:****)"
+    log_args = (params["domain"], params["username"])
+    log.info(log_fmt, *log_args)
+
+    if (auth_config := root_ctx.shared_config["auth"]) is None or auth_config[
+        "max_password_age"
+    ] is None:
+        raise GenericBadRequest("Unsupported function.")
+
+    checked_user = await check_credential(
+        root_ctx.db, params["domain"], params["username"], params["current_password"]
+    )
+    if checked_user is None:
+        raise AuthorizationFailed("User credential mismatch.")
+    new_password = params["new_password"]
+    if compare_to_hashed_password(new_password, checked_user["password"]):
+        raise AuthorizationFailed("Cannot update to the same password as an existing password.")
+
+    # [Hooking point for VERIFY_PASSWORD_FORMAT with the ALL_COMPLETED requirement]
+    # The hook handlers should accept the request and whole ``params` dict.
+    # They should return None if the validation is successful and raise the
+    # Reject error otherwise.
+    hook_result = await root_ctx.hook_plugin_ctx.dispatch(
+        "VERIFY_PASSWORD_FORMAT",
+        (request, params),
+        return_when=ALL_COMPLETED,
+    )
+    if hook_result.status != PASSED:
+        hook_result.reason = hook_result.reason or "invalid password format"
+        raise RejectedByHook.from_hook_result(hook_result)
+
+    async def _update() -> datetime:
+        async with root_ctx.db.begin() as conn:
+            # Update user password.
+            data = {
+                "password": new_password,
+                "need_password_change": False,
+                "password_changed_at": sa.func.now(),
+            }
+            query = (
+                sa.update(users)
+                .values(data)
+                .where(users.c.uuid == checked_user["uuid"])
+                .returning(users.c.password_changed_at)
+            )
+            result = await conn.execute(query)
+            return result.scalar()
+
+    changed_at = await execute_with_retry(_update)
+    return web.json_response({"password_changed_at": changed_at.isoformat()}, status=201)
+
+
 @auth_required
 async def get_ssh_keypair(request: web.Request) -> web.Response:
     root_ctx: RootContext = request.app["_root.context"]
     domain_name = request["user"]["domain_name"]
     access_key = request["keypair"]["access_key"]
     log_fmt = "AUTH.GET_SSH_KEYPAIR(d:{}, ak:{})"
     log_args = (domain_name, access_key)
@@ -1032,13 +1134,14 @@
     test_resource = cors.add(app.router.add_resource("/test"))
     cors.add(test_resource.add_route("GET", test))
     cors.add(test_resource.add_route("POST", test))
     cors.add(app.router.add_route("POST", "/authorize", authorize))
     cors.add(app.router.add_route("GET", "/role", get_role))
     cors.add(app.router.add_route("POST", "/signup", signup))
     cors.add(app.router.add_route("POST", "/signout", signout))
+    cors.add(app.router.add_route("POST", "/update-password-no-auth", update_password_no_auth))
     cors.add(app.router.add_route("POST", "/update-password", update_password))
     cors.add(app.router.add_route("POST", "/update-full-name", update_full_name))
     cors.add(app.router.add_route("GET", "/ssh-keypair", get_ssh_keypair))
     cors.add(app.router.add_route("PATCH", "/ssh-keypair", generate_ssh_keypair))
     cors.add(app.router.add_route("POST", "/ssh-keypair", upload_ssh_keypair))
     return app, [auth_middleware]
```

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/cluster_template.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/cluster_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/context.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/domainconfig.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/domainconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/etcd.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/events.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/events.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/exceptions.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,19 @@
 
 
 class AuthorizationFailed(BackendError, web.HTTPUnauthorized):
     error_type = "https://api.backend.ai/probs/auth-failed"
     error_title = "Credential/signature mismatch."
 
 
+class PasswordExpired(BackendError, web.HTTPUnauthorized):
+    error_type = "https://api.backend.ai/probs/password-expired"
+    error_title = "Password has expired."
+
+
 class InvalidAPIParameters(BackendError, web.HTTPBadRequest):
     error_type = "https://api.backend.ai/probs/invalid-api-params"
     error_title = "Missing or invalid API parameters."
 
 
 class GraphQLError(BackendError, web.HTTPBadRequest):
     error_type = "https://api.backend.ai/probs/graphql-error"
```

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/groupconfig.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/groupconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/image.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/logs.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/logs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/manager.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/ratelimit.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/ratelimit.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/resource.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/resource.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/scaling_group.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/service.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/service.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/session.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,28 +78,25 @@
     SessionStartedEvent,
     SessionSuccessEvent,
     SessionTerminatedEvent,
     SessionTerminatingEvent,
 )
 from ai.backend.common.exception import AliasResolutionFailed, UnknownImageReference
 from ai.backend.common.logging import BraceStyleAdapter
-from ai.backend.common.plugin.hook import HookResults
 from ai.backend.common.plugin.monitor import GAUGE
 from ai.backend.common.types import (
     AccessKey,
     AgentId,
     ClusterMode,
-    EtcdRedisConfig,
     KernelEnqueueingConfig,
     KernelId,
     SessionTypes,
     check_typed_dict,
 )
 from ai.backend.common.utils import cancel_tasks, str_to_timedelta
-from ai.backend.manager.defs import PluginDatabaseID
 
 from ..config import DEFAULT_CHUNK_SIZE
 from ..defs import DEFAULT_IMAGE_ARCH, DEFAULT_ROLE, REDIS_STREAM_DB
 from ..models import (
     AGENT_RESOURCE_OCCUPYING_KERNEL_STATUSES,
     DEAD_SESSION_STATUSES,
     PRIVATE_KERNEL_ROLES,
@@ -136,15 +133,14 @@
     BackendError,
     GenericForbidden,
     ImageNotFound,
     InsufficientPrivilege,
     InternalServerError,
     InvalidAPIParameters,
     ObjectNotFound,
-    RejectedByHook,
     ServiceUnavailable,
     SessionAlreadyExists,
     SessionNotFound,
     StorageProxyError,
     TaskTemplateNotFound,
     TooManySessionsMatched,
     UnknownImageReferenceError,
@@ -1416,23 +1412,19 @@
     )
     try:
         async with root_ctx.db.begin_readonly_session() as db_sess:
             session = await SessionRow.get_session_with_main_kernel(
                 session_name, owner_access_key, db_session=db_sess
             )
         kernel = session.main_kernel
-        report = await root_ctx.registry.get_abusing_report(
-            kernel.id, kernel.agent, kernel.agent_addr
-        )
+        report = await root_ctx.registry.get_abusing_report(kernel.id)
     except BackendError:
         log.exception("GET_ABUSING_REPORT: exception")
         raise
-    if report is None:
-        report = {}
-    return web.json_response(report, status=200)
+    return web.json_response(report or {}, status=200)
 
 
 @server_status_required(ALL_ALLOWED)
 @auth_required
 @check_api_params(
     t.Dict(
         {
@@ -1641,46 +1633,39 @@
     | SessionCancelledEvent
     | SessionTerminatingEvent
     | SessionTerminatedEvent
     | SessionSuccessEvent
     | SessionFailureEvent,
 ) -> None:
     log.info("INVOKE_SESSION_CALLBACK (source:{}, event:{})", source, event)
+    app_ctx: PrivateContext = app["session.context"]
     root_ctx: RootContext = app["_root.context"]
+
     try:
         allow_stale = isinstance(event, (SessionCancelledEvent, SessionTerminatedEvent))
         async with root_ctx.db.begin_readonly_session() as db_sess:
             session = await SessionRow.get_session_with_main_kernel(
                 event.session_id, db_session=db_sess, allow_stale=allow_stale
             )
     except SessionNotFound:
         return
-    url = session.callback_url
-    if url is None:
-        return
-    if (addr := root_ctx.local_config.get("pipeline", {}).get("event-queue")) is None:
+
+    if (callback_url := session.callback_url) is None:
         return
-    etcd_redis_config: EtcdRedisConfig = {
-        "addr": addr,
-        "sentinel": None,
-        "service_name": None,
-        "password": None,
-    }
-    stream_key = "events"
-    token = url.query.get("token")
 
-    async def _dispatch() -> None:
-        hook_result = await root_ctx.hook_plugin_ctx.dispatch(
-            "PUBLISH_EVENT",
-            (event, etcd_redis_config, PluginDatabaseID.SESSION_EVENT, stream_key, token),
-        )
-        if hook_result.status != HookResults.PASSED:
-            raise RejectedByHook.from_hook_result(hook_result)
+    data = {
+        "type": "session_lifecycle",
+        "event": event.name.removeprefix("session_"),
+        "session_id": str(event.session_id),
+        "when": datetime.now(tzutc()).isoformat(),
+    }
 
-    await execute_with_retry(_dispatch)
+    app_ctx.webhook_ptask_group.create_task(
+        _make_session_callback(data, callback_url),
+    )
 
 
 async def handle_batch_result(
     app: web.Application,
     source: AgentId,
     event: SessionSuccessEvent | SessionFailureEvent,
 ) -> None:
@@ -2093,14 +2078,15 @@
         resp["occupiedSlots"] = str(sess.main_kernel.occupied_slots)  # legacy
         resp["occupyingSlots"] = str(sess.occupying_slots)
         resp["requestedSlots"] = str(sess.requested_slots)
         resp["occupiedShares"] = str(
             sess.main_kernel.occupied_shares
         )  # legacy, only caculate main kernel's occupying resource
         resp["environ"] = str(sess.environ)
+        resp["resourceOpts"] = str(sess.resource_opts)
 
         # Lifecycle
         resp["status"] = sess.status.name  # "e.g. 'SessionStatus.RUNNING' -> 'RUNNING' "
         resp["statusInfo"] = str(sess.status_info)
         resp["statusData"] = sess.status_data
         age = datetime.now(tzutc()) - sess.created_at
         resp["age"] = int(age.total_seconds() * 1000)  # age in milliseconds
```

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/session_template.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/stream.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/stream.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/types.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/userconfig.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/userconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/utils.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/vfolder.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/api/wsproxy.py` & `backend.ai-manager-23.3.3/ai/backend/manager/api/wsproxy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/cli/__main__.py` & `backend.ai-manager-23.3.3/ai/backend/manager/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/cli/context.py` & `backend.ai-manager-23.3.3/ai/backend/manager/cli/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/cli/dbschema.py` & `backend.ai-manager-23.3.3/ai/backend/manager/cli/dbschema.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/cli/etcd.py` & `backend.ai-manager-23.3.3/ai/backend/manager/cli/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/cli/fixture.py` & `backend.ai-manager-23.3.3/ai/backend/manager/cli/fixture.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/cli/gql.py` & `backend.ai-manager-23.3.3/ai/backend/manager/cli/gql.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/cli/image.py` & `backend.ai-manager-23.3.3/ai/backend/manager/cli/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/cli/image_impl.py` & `backend.ai-manager-23.3.3/ai/backend/manager/cli/image_impl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/config.py` & `backend.ai-manager-23.3.3/ai/backend/manager/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,14 +396,22 @@
             }
         ).allow_extra("*"),
         t.Key("watcher", default=_shdefs["watcher"]): t.Dict(
             {
                 t.Key("token", default=_shdefs["watcher"]["token"]): t.Null | t.String,
             }
         ).allow_extra("*"),
+        t.Key("auth", default=None): (
+            t.Dict(
+                {
+                    t.Key("max_password_age", default=None): t.Null | tx.TimeDuration(),
+                }
+            ).allow_extra("*")
+            | t.Null
+        ),
     }
 ).allow_extra("*")
 
 volume_config_iv = t.Dict(
     {
         t.Key("default_host"): t.String,
         t.Key("proxies"): t.Mapping(
```

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/container_registry/__init__.py` & `backend.ai-manager-23.3.3/ai/backend/manager/container_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/container_registry/base.py` & `backend.ai-manager-23.3.3/ai/backend/manager/container_registry/base.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/container_registry/docker.py` & `backend.ai-manager-23.3.3/ai/backend/manager/container_registry/docker.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/container_registry/harbor.py` & `backend.ai-manager-23.3.3/ai/backend/manager/container_registry/harbor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/container_registry/local.py` & `backend.ai-manager-23.3.3/ai/backend/manager/container_registry/local.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/defs.py` & `backend.ai-manager-23.3.3/ai/backend/manager/defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -62,19 +62,14 @@
 REDIS_RLIM_DB: Final = 1
 REDIS_LIVE_DB: Final = 2
 REDIS_IMAGE_DB: Final = 3
 REDIS_STREAM_DB: Final = 4
 REDIS_STREAM_LOCK: Final = 5
 
 
-# Redis database IDs used for plugins
-class PluginDatabaseID(enum.IntEnum):
-    SESSION_EVENT = 1
-
-
 # The unique identifiers for distributed locks.
 # To be used with PostgreSQL advisory locks, the values are defined as integers.
 class LockID(enum.IntEnum):
     LOCKID_TEST = 42
     LOCKID_SCHEDULE = 91
     LOCKID_PREPARE = 92
     LOCKID_SCHEDULE_TIMER = 191
```

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/exceptions.py` & `backend.ai-manager-23.3.3/ai/backend/manager/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/idle.py` & `backend.ai-manager-23.3.3/ai/backend/manager/idle.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/__init__.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/acl.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/agent.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from dateutil.parser import parse as dtparse
 from graphene.types.datetime import DateTime as GQLDateTime
 from sqlalchemy.dialects import postgresql as pgsql
 from sqlalchemy.engine.row import Row
 from sqlalchemy.ext.asyncio import AsyncConnection as SAConnection
 from sqlalchemy.ext.asyncio import AsyncSession as SASession
 from sqlalchemy.orm import relationship
-from sqlalchemy.sql.expression import true
+from sqlalchemy.sql.expression import false, true
 
 from ai.backend.common import msgpack, redis_helper
 from ai.backend.common.types import AgentId, BinarySize, HardwareMetadata, ResourceSlot
 
 from .base import (
     Base,
     EnumType,
@@ -85,14 +85,21 @@
     sa.Column("addr", sa.String(length=128), nullable=False),
     sa.Column("public_host", sa.String(length=256), nullable=True),
     sa.Column("first_contact", sa.DateTime(timezone=True), server_default=sa.func.now()),
     sa.Column("lost_at", sa.DateTime(timezone=True), nullable=True),
     sa.Column("version", sa.String(length=64), nullable=False),
     sa.Column("architecture", sa.String(length=32), nullable=False),
     sa.Column("compute_plugins", pgsql.JSONB(), nullable=False, default={}),
+    sa.Column(
+        "auto_terminate_abusing_kernel",
+        sa.Boolean(),
+        nullable=False,
+        server_default=false(),
+        default=False,
+    ),
 )
 
 
 class AgentRow(Base):
     __table__ = agents
     kernels = relationship("KernelRow", back_populates="agent_row")
     scaling_group_row = relationship("ScalingGroupRow", back_populates="agents")
@@ -127,14 +134,15 @@
     architecture = graphene.String()
     first_contact = GQLDateTime()
     lost_at = GQLDateTime()
     live_stat = graphene.JSONString()
     version = graphene.String()
     compute_plugins = graphene.JSONString()
     hardware_metadata = graphene.JSONString()
+    auto_terminate_abusing_kernel = graphene.Boolean()
     local_config = graphene.JSONString()
 
     # Legacy fields
     mem_slots = graphene.Int()
     cpu_slots = graphene.Float()
     gpu_slots = graphene.Float()
     tpu_slots = graphene.Float()
@@ -167,14 +175,15 @@
             occupied_slots=row["occupied_slots"].to_json(),
             addr=row["addr"],
             architecture=row["architecture"],
             first_contact=row["first_contact"],
             lost_at=row["lost_at"],
             version=row["version"],
             compute_plugins=row["compute_plugins"],
+            auto_terminate_abusing_kernel=row["auto_terminate_abusing_kernel"],
             # legacy fields
             mem_slots=BinarySize.from_str(row["available_slots"]["mem"]) // mega,
             cpu_slots=row["available_slots"]["cpu"],
             gpu_slots=row["available_slots"].get("cuda.device", 0),
             tpu_slots=row["available_slots"].get("tpu.device", 0),
             used_mem_slots=BinarySize.from_str(row["occupied_slots"].get("mem", 0)) // mega,
             used_cpu_slots=float(row["occupied_slots"].get("cpu", 0)),
@@ -219,19 +228,20 @@
         info: graphene.ResolveInfo,
     ) -> Optional[Mapping[str, HardwareMetadata]]:
         if self.status != AgentStatus.ALIVE.name:
             return None
         graph_ctx: GraphQueryContext = info.context
         return await graph_ctx.registry.gather_agent_hwinfo(self.id)
 
-    async def resolve_local_config(self, info: graphene.ResolveInfo) -> Optional[Mapping[str, Any]]:
-        if self.status != AgentStatus.ALIVE.name:
-            return None
-        graph_ctx: GraphQueryContext = info.context
-        return await graph_ctx.registry.get_agent_local_config(self.id, self.addr)
+    async def resolve_local_config(self, info: graphene.ResolveInfo) -> Mapping[str, Any]:
+        return {
+            "agent": {
+                "auto_terminate_abusing_kernel": self.auto_terminate_abusing_kernel,
+            },
+        }
 
     _queryfilter_fieldspec = {
         "id": ("id", None),
         "status": ("status", lambda s: AgentStatus[s]),
         "status_changed": ("status_changed", dtparse),
         "region": ("region", None),
         "scaling_group": ("scaling_group", None),
```

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/env.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/env.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """add a new session type INFERENCE
 
 Revision ID: b5be363ab05c
-Revises: cace152eefac
+Revises: b6b884fbae1f
 Create Date: 2023-02-15 15:24:29.112938
 
 Reference: https://www.postgresql.org/message-id/CANu8FiwwBxZZGX23=Na_7bc4DZ-yzd_poKhaoPmN3+SHG08MAg@mail.gmail.com
 
 """
 import textwrap
 
 from alembic import op
 from sqlalchemy.sql import text
 
 from ai.backend.common.types import SessionTypes
 
 # revision identifiers, used by Alembic.
 revision = "b5be363ab05c"
-down_revision = "cace152eefac"
+down_revision = "b6b884fbae1f"
 branch_labels = None
 depends_on = None
 
 # select enum_range(null::sessiontypes);
 typename = SessionTypes.__name__.lower()
```

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,54 @@
 """add_session_table
 
 Revision ID: b6b884fbae1f
-Revises: 213a04e90ecf
+Revises: cace152eefac
 Create Date: 2022-12-05 16:12:53.275671
 
 """
 from collections import defaultdict
-from uuid import uuid4
+from typing import Any, Mapping, Sequence
+from uuid import UUID, uuid4
 
 import sqlalchemy as sa
 from alembic import op
 from sqlalchemy.dialects import postgresql as pgsql
 from sqlalchemy.orm import registry
 
+from ai.backend.manager.defs import DEFAULT_ROLE
 from ai.backend.manager.models import KernelStatus, SessionStatus
 from ai.backend.manager.models.base import GUID, KernelIDColumn, convention
+from ai.backend.manager.models.session import SessionDependencyRow
 
 # revision identifiers, used by Alembic.
 revision = "b6b884fbae1f"
-down_revision = "213a04e90ecf"
+down_revision = "cace152eefac"
 branch_labels = None
 depends_on = None
 
 
 kernel_status = tuple(s.name for s in KernelStatus)
 
 session_status = tuple(s.name for s in SessionStatus)
 
 metadata = sa.MetaData(naming_convention=convention)
 mapper_registry = registry(metadata=metadata)
 Base = mapper_registry.generate_base()
 
+PAGE_SIZE = 100
+
 
 def default_hostname(context) -> str:
     params = context.get_current_parameters()
     return f"{params['cluster_role']}{params['cluster_idx']}"
 
 
-def upgrade():
+def upgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
     connection = op.get_bind()
-    # db_session = Session(connection)
-
-    # class ImageRow(Base):
-    #     __tablename__ = "images"
-    #     id = sa.Column("id", GUID(), nullable=False, primary_key=True)
-    #     name = sa.Column("name", sa.String, nullable=False, index=True)
-
     kernels = sa.Table(
         "kernels",
         metadata,
         KernelIDColumn(),
         sa.Column("session_id", GUID, nullable=False),
         sa.Column("session_creation_id", sa.String(length=32), unique=False),
         sa.Column("session_name", sa.String(length=64), unique=False),
@@ -66,60 +64,86 @@
             "cluster_mode",
             sa.String(length=16),
             nullable=False,
             default="SINGLE_NODE",
             server_default="SINGLE_NODE",
         ),
         sa.Column("cluster_size", sa.Integer, nullable=False, default=1),
+        sa.Column("cluster_idx", sa.Integer, nullable=False, default=0),
+        sa.Column("local_rank", sa.Integer, nullable=False, default=0),
+        sa.Column(
+            "cluster_hostname", sa.String(length=64), nullable=False, default=default_hostname
+        ),
         # Resource ownership
+        sa.Column("agent", sa.String(length=64), sa.ForeignKey("agents.id"), nullable=True),
+        sa.Column("agent_addr", sa.String(length=128), nullable=True),
         sa.Column("scaling_group", sa.ForeignKey("scaling_groups.name"), nullable=True),
         sa.Column(
             "domain_name", sa.String(length=64), sa.ForeignKey("domains.name"), nullable=False
         ),
         sa.Column("group_id", GUID, sa.ForeignKey("groups.id"), nullable=False),
         sa.Column("user_uuid", GUID, sa.ForeignKey("users.uuid"), nullable=False),
         sa.Column("access_key", sa.String(length=20), sa.ForeignKey("keypairs.access_key")),
         sa.Column("image", sa.String(length=512)),
+        sa.Column("architecture", sa.String(length=32), default="x86_64"),
+        sa.Column("registry", sa.String(length=512)),
         sa.Column("tag", sa.String(length=64), nullable=True),
         # Resource occupation
+        sa.Column("container_id", sa.String(length=64)),
         sa.Column("occupied_slots", pgsql.JSONB(), nullable=False),
+        sa.Column("occupied_shares", pgsql.JSONB(), nullable=False, default={}),  # legacy
+        sa.Column("environ", sa.ARRAY(sa.String), nullable=True),
+        sa.Column("mounts", sa.ARRAY(sa.String), nullable=True),  # list of list; legacy since 22.03
+        sa.Column("mount_map", pgsql.JSONB(), nullable=True, default={}),  # legacy since 22.03
         sa.Column("vfolder_mounts", pgsql.JSONB(), nullable=True),
+        sa.Column("attached_devices", pgsql.JSONB(), nullable=True, default={}),
         sa.Column("resource_opts", pgsql.JSONB(), nullable=True, default={}),
         sa.Column("bootstrap_script", sa.String(length=16 * 1024), nullable=True),
+        # Port mappings
+        # If kernel_host is NULL, it is assumed to be same to the agent host or IP.
+        sa.Column("kernel_host", sa.String(length=128), nullable=True),
+        sa.Column("repl_in_port", sa.Integer(), nullable=False),
+        sa.Column("repl_out_port", sa.Integer(), nullable=False),
+        sa.Column("stdin_port", sa.Integer(), nullable=False),  # legacy for stream_pty
+        sa.Column("stdout_port", sa.Integer(), nullable=False),  # legacy for stream_pty
+        sa.Column("service_ports", pgsql.JSONB(), nullable=True),
+        sa.Column("preopen_ports", sa.ARRAY(sa.Integer), nullable=True),
         sa.Column("use_host_network", sa.Boolean(), default=False, nullable=False),
         # Lifecycle
         sa.Column("created_at", sa.DateTime(timezone=True), server_default=sa.func.now()),
         sa.Column("terminated_at", sa.DateTime(timezone=True), nullable=True, default=sa.null()),
         sa.Column("starts_at", sa.DateTime(timezone=True), nullable=True, default=sa.null()),
         sa.Column(
             "status",
             sa.Enum(*kernel_status),
             default="PENDING",
             server_default="PENDING",
             nullable=False,
         ),
-        # sa.Column("status_changed", sa.DateTime(timezone=True), nullable=True),
+        sa.Column("status_changed", sa.DateTime(timezone=True), nullable=True),
         sa.Column("status_history", pgsql.JSONB(), nullable=True, default=sa.null()),
         sa.Column("status_info", sa.Unicode(), nullable=True, default=sa.null()),
         sa.Column("status_data", pgsql.JSONB(), nullable=True, default=sa.null()),
         sa.Column("callback_url", sa.types.UnicodeText, nullable=True, default=sa.null()),
         sa.Column("startup_command", sa.Text, nullable=True),
         sa.Column(
             "result",
             sa.Enum("UNDEFINED", "SUCCESS", "FAILURE"),
             default="UNDEFINED",
             server_default="UNDEFINED",
             nullable=False,
         ),
+        sa.Column("internal_data", pgsql.JSONB(), nullable=True),
+        sa.Column("container_log", sa.LargeBinary(), nullable=True),
         # Resource metrics measured upon termination
         sa.Column("num_queries", sa.BigInteger(), default=0),
         sa.Column("last_stat", pgsql.JSONB(), nullable=True, default=sa.null()),
     )
 
-    class SessionRow(Base):
+    class SessionRow(Base):  # type: ignore[valid-type, misc]
         __tablename__ = "sessions"
         id = sa.Column(
             "id",
             GUID(),
             server_default=sa.text("uuid_generate_v4()"),
             nullable=False,
             primary_key=True,
@@ -242,122 +266,224 @@
     op.create_index(op.f("ix_sessions_session_type"), "sessions", ["session_type"], unique=False)
     # op.create_index(op.f("ix_sessions_status"), "sessions", ["status"], unique=False)
     # op.create_index(
     #     op.f("ix_sessions_status_changed"), "sessions", ["status_changed"], unique=False
     # )
     op.create_index(op.f("ix_sessions_terminated_at"), "sessions", ["terminated_at"], unique=False)
 
-    query = sa.select([kernels]).select_from(kernels).order_by(kernels.c.created_at)
-    kernel_rows = connection.execute(query).fetchall()
-
-    # imgs = db_session.query(ImageRow).all()
-    # img_map = {img.name: img.id for img in imgs}
+    op.drop_constraint(
+        "fk_session_dependencies_depends_on_kernels", "session_dependencies", type_="foreignkey"
+    )
+    op.drop_constraint(
+        "fk_session_dependencies_session_id_kernels", "session_dependencies", type_="foreignkey"
+    )
 
-    all_kernel_sessions = {}
-    # kernel_id and session_id are the same if it is a single kernel session.
-    # update kernel's session_id of single kernel session.
-    single_kernel_ids = {}
-    for row in kernel_rows:
-        sess_id = row["session_id"]
-        if sess_id not in all_kernel_sessions:
-            if sess_id == row["id"]:
-                # create session with new id if the kernel_id and session_id are the same.
-                sess_id = uuid4()
-                single_kernel_ids[row["id"]] = sess_id
-            sess = {
-                "id": sess_id,
-                "creation_id": row["session_creation_id"],
-                "name": row["session_name"],
-                "session_type": row["session_type"],
-                "cluster_mode": row["cluster_mode"],
-                "cluster_size": row["cluster_size"],
-                "scaling_group_name": row["scaling_group"],
-                "domain_name": row["domain_name"],
-                "group_id": row["group_id"],
-                "user_uuid": row["user_uuid"],
-                "access_key": row["access_key"],
+    def migrate_kernel_to_session(kernel_query: sa.sql.Select, is_single_kernel: bool) -> None:
+        session_map: dict[UUID, dict[str, Any]] = {}
+        main_kernel_rows: dict[UUID, dict[str, Any]] = {}
+        single_kernel_ids: dict[UUID, UUID] = {}
+        kernel_rows: Sequence[Mapping[str, Any]] = connection.execute(kernel_query).fetchall()
+
+        def _map_session(session_id: UUID, kernel_row: Mapping[str, Any]) -> dict[str, Any]:
+            return {
+                "id": session_id,
+                "creation_id": kernel_row["session_creation_id"],
+                "name": kernel_row["session_name"],
+                "session_type": kernel_row["session_type"],
+                "cluster_mode": kernel_row["cluster_mode"],
+                "cluster_size": kernel_row["cluster_size"],
+                "scaling_group_name": kernel_row["scaling_group"],
+                "domain_name": kernel_row["domain_name"],
+                "group_id": kernel_row["group_id"],
+                "user_uuid": kernel_row["user_uuid"],
+                "access_key": kernel_row["access_key"],
                 # "image_id": img_map[row["image"]],
                 # "image": row["image"],
-                "tag": row["tag"],
-                "occupying_slots": row["occupied_slots"],
-                "requested_slots": row["occupied_slots"],
-                "vfolder_mounts": row["vfolder_mounts"],
-                "resource_opts": row["resource_opts"],
-                "bootstrap_script": row["bootstrap_script"],
-                "use_host_network": row["use_host_network"],
-                "created_at": row["created_at"],
-                "terminated_at": row["terminated_at"],
-                "starts_at": row["starts_at"],
-                "status": row["status"],
+                "tag": kernel_row["tag"],
+                "occupying_slots": kernel_row["occupied_slots"],
+                "requested_slots": kernel_row["occupied_slots"],
+                "vfolder_mounts": kernel_row["vfolder_mounts"],
+                "resource_opts": kernel_row["resource_opts"],
+                "bootstrap_script": kernel_row["bootstrap_script"],
+                "use_host_network": kernel_row["use_host_network"],
+                "created_at": kernel_row["created_at"],
+                "terminated_at": kernel_row["terminated_at"],
+                "starts_at": kernel_row["starts_at"],
+                "status": kernel_row["status"],
                 # "status_changed": row["status_changed"],
-                "status_history": row["status_history"],
-                "status_info": row["status_info"],
-                "status_data": row["status_data"],
-                "callback_url": row["callback_url"],
-                "startup_command": row["startup_command"],
-                "result": row["result"],
-                "num_queries": row["num_queries"],
-                "last_stat": row["last_stat"],
+                "status_history": kernel_row["status_history"],
+                "status_info": kernel_row["status_info"],
+                "status_data": kernel_row["status_data"],
+                "callback_url": kernel_row["callback_url"],
+                "startup_command": kernel_row["startup_command"],
+                "result": kernel_row["result"],
+                "num_queries": kernel_row["num_queries"],
+                "last_stat": kernel_row["last_stat"],
             }
-            all_kernel_sessions[sess_id] = sess
-        else:
-            sess = all_kernel_sessions[sess_id]
 
-            # st_change = sess["status_changed"]
+        if is_single_kernel:
+            for row in kernel_rows:
+                sess_id = uuid4()
+                session_map[sess_id] = _map_session(sess_id, row)
+                single_kernel_ids[row["id"]] = sess_id
+        else:
+            for row in kernel_rows:
+                # Since main kernel of multi-kernel session has the same id with session_id
+                # insert new kernels to kernels have distinguished id with sessions.
+                if row["cluster_role"] == "main" or row["cluster_role"] == DEFAULT_ROLE:
+                    new_kern_id = uuid4()
+                    main_kernel_rows[row["id"]] = {
+                        **row,
+                        "id": new_kern_id,
+                    }
+
+                sess_id = row["session_id"]
+                if sess_id not in session_map:
+                    session_map[sess_id] = _map_session(sess_id, row)
+                else:
+                    sess = session_map[sess_id]
+                    try:
+                        if sess["created_at"] is not None and row["created_at"] is not None:
+                            if sess["created_at"] > row["created_at"]:
+                                sess["created_at"] = row["created_at"]
+                                # st_change = row["st_change"]
+                    except (TypeError, ValueError):
+                        pass
+
+                    try:
+                        if sess["starts_at"] is not None and row["starts_at"] is not None:
+                            if sess["starts_at"] > row["starts_at"]:
+                                sess["starts_at"] = row["starts_at"]
+                                # st_change = row["st_change"]
+                    except (TypeError, ValueError):
+                        pass
+
+                    # if str(sess["status"]) not in ("ERROR", "CANCELLED"):
+                    #     if KernelStatus.index(str(sess["status"])) > KernelStatus.index(str(row["status"])):
+                    #         sess["status"] = row["status"]
+                    sess["status"] = row["status"]
+
+                    try:
+                        if sess["terminated_at"] is not None and row["terminated_at"] is not None:
+                            if sess["terminated_at"] < row["terminated_at"]:
+                                sess["terminated_at"] = row["terminated_at"]
+                                # st_change = row["status_changed"]
+                        elif sess["terminated_at"] is None:
+                            pass
+                        elif row["terminated_at"] is None:
+                            sess["terminated_at"] = None
+                        # sess["status_changed"] = st_change
+                    except (TypeError, ValueError):
+                        pass
+
+                    if sess["status_info"] != row["status_info"]:
+                        if row["cluster_role"] == "main" or row["cluster_role"] == DEFAULT_ROLE:
+                            sess["status_info"] = row["status_info"]
+
+        if session_map:
+            creates = tuple(session_map.values())
+            connection.execute(SessionRow.__table__.insert(), creates)
+
+        if is_single_kernel and single_kernel_ids:
+            # Delete and insert session_dependencies
+            # Since session_id and depends_on columns have primary constraint, we should not `update` them.
+            kern_ids = list(single_kernel_ids.keys())
+            insert_values = []
+            sess_dep_query = sa.select(SessionDependencyRow).where(
+                SessionDependencyRow.session_id.in_(kern_ids)
+                | SessionDependencyRow.depends_on.in_(kern_ids)
+            )
+            for row in connection.execute(sess_dep_query).fetchall():
+                val = {}
+                if row["session_id"] in single_kernel_ids:
+                    val["session_id"] = single_kernel_ids[row["session_id"]]
+                else:
+                    val["session_id"] = row["session_id"]
+
+                if row["depends_on"] in single_kernel_ids:
+                    val["depends_on"] = single_kernel_ids[row["depends_on"]]
+                else:
+                    val["depends_on"] = row["depends_on"]
+                insert_values.append(val)
+            dep_delete_query = sa.delete(SessionDependencyRow).where(
+                SessionDependencyRow.session_id.in_(kern_ids)
+                | SessionDependencyRow.depends_on.in_(kern_ids)
+            )
+            connection.execute(dep_delete_query)
+            if insert_values:
+                connection.execute(sa.insert(SessionDependencyRow), insert_values)
+
+            # Update single-kernel session's kernel
+            sess_query = (
+                sa.update(kernels)
+                .where(kernels.c.id == sa.bindparam("kernel_id"))
+                .values(session_id=sa.bindparam("b_session_id"))
+            )
+            sess_update_params = [
+                {
+                    "kernel_id": kern_id,
+                    "b_session_id": sess_id,
+                }
+                for kern_id, sess_id in single_kernel_ids.items()
+            ]
+            if sess_update_params:
+                connection.execute(sess_query, sess_update_params)
+
+        # Insert and delete multi-kernel session's main kernel
+        if main_kernel_rows:
+            connection.execute(sa.insert(kernels), list(main_kernel_rows.values()))
+            delete_query = sa.delete(kernels).where(kernels.c.id.in_(list(main_kernel_rows.keys())))
+            connection.execute(delete_query)
+
+    # Drop the unique constraint before migration
+    op.drop_index("ix_kernels_unique_sess_token", table_name="kernels")
+
+    # Multi-kernel session migration
+    session_cnt = connection.execute(
+        sa.select([sa.func.count(sa.distinct(kernels.c.session_id))]).where(
+            kernels.c.cluster_size > 1
+        )
+    ).scalar()
+    for offset in range(0, session_cnt, PAGE_SIZE):
+        session_id_query = (
+            sa.select([sa.distinct(kernels.c.session_id)])
+            .where(kernels.c.cluster_size > 1)
+            .order_by(kernels.c.session_id)
+            .offset(offset)
+            .limit(PAGE_SIZE)
+        )
+        session_ids = connection.execute(session_id_query).scalars().all()
+        query = sa.select([kernels]).where(kernels.c.session_id.in_(session_ids))
+        migrate_kernel_to_session(query, is_single_kernel=False)
+
+    # Single-kernel session migration
+    kernel_cnt = connection.execute(
+        sa.select([sa.func.count()]).select_from(kernels).where(kernels.c.cluster_size == 1)
+    ).scalar()
+    for offset in range(0, kernel_cnt, PAGE_SIZE):
+        query = (
+            sa.select([kernels])
+            .where(kernels.c.cluster_size == 1)
+            .order_by(kernels.c.id)
+            .offset(offset)
+            .limit(PAGE_SIZE)
+        )
+        migrate_kernel_to_session(query, is_single_kernel=True)
 
-            try:
-                if sess["created_at"] is not None and row["created_at"] is not None:
-                    if sess["created_at"] > row["created_at"]:
-                        sess["created_at"] = row["created_at"]
-                        # st_change = row["st_change"]
-            except (TypeError, ValueError):
-                pass
-
-            try:
-                if sess["starts_at"] is not None and row["starts_at"] is not None:
-                    if sess["starts_at"] > row["starts_at"]:
-                        sess["starts_at"] = row["starts_at"]
-                        # st_change = row["st_change"]
-            except (TypeError, ValueError):
-                pass
-
-            # if str(sess["status"]) not in ("ERROR", "CANCELLED"):
-            #     if KernelStatus.index(str(sess["status"])) > KernelStatus.index(str(row["status"])):
-            #         sess["status"] = row["status"]
-            sess["status"] = row["status"]
-
-            try:
-                if sess["terminated_at"] is not None and row["terminated_at"] is not None:
-                    if sess["terminated_at"] < row["terminated_at"]:
-                        sess["terminated_at"] = row["terminated_at"]
-                        # st_change = row["status_changed"]
-                elif sess["terminated_at"] is None:
-                    pass
-                elif row["terminated_at"] is None:
-                    sess["terminated_at"] = None
-                # sess["status_changed"] = st_change
-            except (TypeError, ValueError):
-                pass
-
-            if sess["status_info"] != row["status_info"]:
-                import json
-
-                sinfo = sess["status_info"]
-                try:
-                    sinfo = json.loads(sinfo)
-                except json.decoder.JSONDecodeError:
-                    sinfo = {sess["id"]: sinfo}
-                sinfo = {**sinfo, row["id"]: row["status_info"]}
-                sess["status_info"] = json.dumps(sinfo)
-
-    if all_kernel_sessions:
-        creates = tuple(all_kernel_sessions.values())
-        connection.execute(SessionRow.__table__.insert(), creates)
+    # Restore the dropped constraint.
+    op.create_index(
+        "ix_kernels_unique_sess_token",
+        "kernels",
+        ["access_key", "session_name"],
+        unique=True,
+        postgresql_where=sa.text(
+            "status NOT IN ('TERMINATED', 'CANCELLED') and cluster_role = 'main'"
+        ),
+    )
 
-    # Session dependency table
     op.create_foreign_key(
         op.f("fk_session_dependencies_session_id_sessions"),
         "session_dependencies",
         "sessions",
         ["session_id"],
         ["id"],
         onupdate="CASCADE",
@@ -368,70 +494,18 @@
         "session_dependencies",
         "sessions",
         ["depends_on"],
         ["id"],
         onupdate="CASCADE",
         ondelete="CASCADE",
     )
-    op.drop_constraint(
-        "fk_session_dependencies_depends_on_kernels", "session_dependencies", type_="foreignkey"
-    )
-    op.drop_constraint(
-        "fk_session_dependencies_session_id_kernels", "session_dependencies", type_="foreignkey"
-    )
 
-    # Kernel table
-    sess_query = (
-        sa.update(kernels)
-        .where(kernels.c.id == sa.bindparam("kernel_id"))
-        .values(session_id=sa.bindparam("b_session_id"))
-    )
-    sess_update_params = []
-    for kern_id, sess_id in single_kernel_ids.items():
-        sess_update_params.append(
-            {
-                "kernel_id": kern_id,
-                "b_session_id": sess_id,
-            }
-        )
-    if sess_update_params:
-        connection.execute(sess_query, sess_update_params)
     op.create_foreign_key(
         op.f("fk_kernels_session_id_sessions"), "kernels", "sessions", ["session_id"], ["id"]
     )
-    # op.add_column("kernels", sa.Column("image_id", GUID(), nullable=True))
-    # kernels = sa.Table(
-    #     "kernels",
-    #     metadata,
-    #     KernelIDColumn(),
-    #     sa.Column("image_id", GUID(), nullable=True),
-    #     extend_existing=True,
-    # )
-    # img_query = (
-    #     sa.update(kernels)
-    #     .where(kernels.c.id == sa.bindparam("kernel_id"))
-    #     .values(image_id=sa.bindparam("b_image_id"))
-    # )
-    # img_update_params = []
-    # for kern in kernel_rows:
-    #     try:
-    #         img_update_params.append(
-    #             {
-    #                 "kernel_id": kern["id"],
-    #                 "b_image_id": img_map[kern["image"]],
-    #             }
-    #         )
-    #     except KeyError:
-    #         continue
-    # if img_update_params:
-    #     connection.execute(img_query, img_update_params)
-
-    # op.create_foreign_key(
-    #     op.f("fk_kernels_image_id_images"), "kernels", "images", ["image_id"], ["id"]
-    # )
     op.add_column("kernels", sa.Column("requested_slots", pgsql.JSONB(), nullable=True))
 
     ## Association tables
     # groups_users
     op.drop_constraint(
         "uq_association_user_id_group_id", "association_groups_users", type_="unique"
     )
@@ -445,88 +519,113 @@
     # scaling_groups_keypairs
     op.drop_constraint("uq_sgroup_akey", "sgroups_for_keypairs", type_="unique")
 
     # ### end Alembic commands ###
 
 
 def downgrade():
-    # ### commands auto generated by Alembic - please adjust! ###
-    # class ImageRow(Base):
-    #     __tablename__ = "images"
-    #     id = sa.Column("id", GUID(), nullable=False, primary_key=True)
-    #     name = sa.Column("name", sa.String, nullable=False, index=True)
-
     connection = op.get_bind()
-    # db_session = Session(connection)
-    # imgs = db_session.query(ImageRow).all()
-    # img_map = {img.id: img.name for img in imgs}
 
     # Kernel table
     op.drop_constraint(op.f("fk_kernels_session_id_sessions"), "kernels", type_="foreignkey")
-    # op.drop_constraint(op.f("fk_kernels_image_id_images"), "kernels", type_="foreignkey")
     kernels = sa.Table(
         "kernels",
         metadata,
         KernelIDColumn(),
         sa.Column("session_id", GUID, nullable=False),
-        # sa.Column("image_id", GUID(), nullable=True),
-        # sa.Column("image", sa.String(length=512), nullable=True),
         sa.Column("created_at", sa.DateTime(timezone=True), server_default=sa.func.now()),
     )
-    query = sa.select(kernels).select_from(kernels).order_by(kernels.c.created_at)
-    kernel_rows = connection.execute(query).fetchall()
+    op.drop_constraint(
+        op.f("fk_session_dependencies_depends_on_sessions"),
+        "session_dependencies",
+        type_="foreignkey",
+    )
+    op.drop_constraint(
+        op.f("fk_session_dependencies_session_id_sessions"),
+        "session_dependencies",
+        type_="foreignkey",
+    )
+
+    class SessionRow(Base):
+        __tablename__ = "sessions"
+        id = sa.Column(
+            "id",
+            GUID(),
+            server_default=sa.text("uuid_generate_v4()"),
+            nullable=False,
+            primary_key=True,
+        )
+
+    session_cnt = connection.execute(sa.select([sa.func.count()]).select_from(SessionRow)).scalar()
+    for page in range(0, session_cnt, PAGE_SIZE):
+        query = sa.select(SessionRow.id).order_by(SessionRow.id).offset(page).limit(PAGE_SIZE)
+        session_ids = [row["id"] for row in connection.execute(query).fetchall()]
+
+        query = sa.select([kernels]).where(kernels.c.session_id.in_(session_ids))
+        kernel_rows = connection.execute(query).fetchall()
+
+        num_kernel_sess: dict[UUID, int] = defaultdict(int)
+        sess_kern_map = {}
+        for kern in kernel_rows:
+            # restore kernel's session_id
+            sess_id = kern["session_id"]
+            num_kernel_sess[sess_id] += 1
+            if sess_id not in sess_kern_map:
+                sess_kern_map[sess_id] = kern["id"]
+        kern_update_query = (
+            sa.update(kernels)
+            .where(kernels.c.id == sa.bindparam("kernel_id"))
+            .values({kernels.c.session_id: sa.bindparam("session_id")})
+        )
+        sess_update_params = []
+        single_kern_sess = {}
+        for sess_id, num_kern in num_kernel_sess.items():
+            if num_kern == 1:
+                # it is single kernel session.
+                # session_id must be same with kernel_id.
+                kernel_id = sess_kern_map[sess_id]
+                single_kern_sess[sess_id] = kernel_id
+                sess_update_params.append(
+                    {
+                        "kernel_id": kernel_id,
+                        "session_id": kernel_id,
+                    }
+                )
+        if sess_update_params:
+            connection.execute(kern_update_query, sess_update_params)
+
+        # Session dependency table
+        sess_ids = list(single_kern_sess.keys())
+        sess_dep_query = sa.select(SessionDependencyRow).where(
+            SessionDependencyRow.session_id.in_(sess_ids)
+            | SessionDependencyRow.depends_on.in_(sess_ids)
+        )
+        insert_values = []
+        for row in connection.execute(sess_dep_query).fetchall():
+            val = {}
+            if row["session_id"] in single_kern_sess:
+                val["session_id"] = single_kern_sess[row["session_id"]]
+            else:
+                val["session_id"] = row["session_id"]
+
+            if row["depends_on"] in single_kern_sess:
+                val["depends_on"] = single_kern_sess[row["depends_on"]]
+            else:
+                val["depends_on"] = row["depends_on"]
+            insert_values.append(val)
+        dep_delete_query = sa.delete(SessionDependencyRow).where(
+            SessionDependencyRow.session_id.in_(sess_ids)
+            | SessionDependencyRow.depends_on.in_(sess_ids)
+        )
+        connection.execute(dep_delete_query)
+        if insert_values:
+            connection.execute(sa.insert(SessionDependencyRow), insert_values)
 
-    # img_update_query = (
-    #     sa.update(kernels)
-    #     .where(kernels.c.id == sa.bindparam("kernel_id"))
-    #     .values({kernels.c.image: sa.bindparam("image")})
-    # )
-    # img_params = []
-    num_kernel_sess = defaultdict(int)
-    sess_kern_map = {}
-    for kern in kernel_rows:
-        # restore kernel's session_id
-        sess_id = kern["session_id"]
-        num_kernel_sess[sess_id] += 1
-        if sess_id not in sess_kern_map:
-            sess_kern_map[sess_id] = kern["id"]
-    #     try:
-    #         img_params.append(
-    #             {
-    #                 "kernel_id": kern["id"],
-    #                 "image": img_map[kern["image_id"]],
-    #             }
-    #         )
-    #     except KeyError:
-    #         continue
-    # if img_params:
-    #     connection.execute(img_update_query, img_params)
-    kern_update_query = (
-        sa.update(kernels)
-        .where(kernels.c.id == sa.bindparam("kernel_id"))
-        .values({kernels.c.session_id: sa.bindparam("session_id")})
-    )
-    sess_update_params = []
-    for sess_id, num_kern in num_kernel_sess.items():
-        if num_kern == 1:
-            # it is single kernel session.
-            # session_id must be same with kernel_id.
-            kernel_id = sess_kern_map[sess_id]
-            sess_update_params.append(
-                {
-                    "kernel_id": kernel_id,
-                    "session_id": kernel_id,
-                }
-            )
-    if sess_update_params:
-        connection.execute(kern_update_query, sess_update_params)
     # op.drop_column("kernels", "image_id")
     op.drop_column("kernels", "requested_slots")
-
-    # Session dependency table
     op.create_foreign_key(
         "fk_session_dependencies_session_id_kernels",
         "session_dependencies",
         "kernels",
         ["session_id"],
         ["id"],
         onupdate="CASCADE",
@@ -537,24 +636,14 @@
         "session_dependencies",
         "kernels",
         ["depends_on"],
         ["id"],
         onupdate="CASCADE",
         ondelete="CASCADE",
     )
-    op.drop_constraint(
-        op.f("fk_session_dependencies_depends_on_sessions"),
-        "session_dependencies",
-        type_="foreignkey",
-    )
-    op.drop_constraint(
-        op.f("fk_session_dependencies_session_id_sessions"),
-        "session_dependencies",
-        type_="foreignkey",
-    )
 
     # Session table
     op.drop_index(op.f("ix_sessions_terminated_at"), table_name="sessions")
     # op.drop_index(op.f("ix_sessions_status_changed"), table_name="sessions")
     # op.drop_index(op.f("ix_sessions_status"), table_name="sessions")
     op.drop_index(op.f("ix_sessions_session_type"), table_name="sessions")
     op.drop_index(op.f("ix_sessions_scaling_group_name"), table_name="sessions")
```

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """add role column on kernels table
 
 Revision ID: bedd92de93af
-Revises: 10c58e701d87
+Revises: 3efd66393bd0, 10c58e701d87
 Create Date: 2023-04-24 11:57:53.111968
 
 """
 import sqlalchemy as sa
 from alembic import op
 from sqlalchemy import cast
 from sqlalchemy.dialects import postgresql
 from sqlalchemy.sql.functions import coalesce
 
 from ai.backend.manager.models import ImageRow, KernelRole, kernels
 from ai.backend.manager.models.base import EnumType
 
 # revision identifiers, used by Alembic.
 revision = "bedd92de93af"
-down_revision = "10c58e701d87"
+down_revision = ("3efd66393bd0", "10c58e701d87")
 branch_labels = None
 depends_on = None
 
 images = ImageRow.__table__
 kernelrole_choices = list(map(lambda v: v.name, KernelRole))
 kernelrole = postgresql.ENUM(*kernelrole_choices, name="kernelrole")
 
@@ -40,14 +40,16 @@
             .where(kernels.c.role == None)
             .order_by(kernels.c.id)
             .limit(batch_size)
         )
         result = connection.execute(query).fetchall()
         kernel_ids_to_update = [kid[0] for kid in result]
 
+        if not kernel_ids_to_update:
+            break
         query = (
             sa.update(kernels)
             .values(
                 {
                     "role": cast(
                         coalesce(
                             # `limit(1)` is introduced since it is possible (not prevented) for two
```

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """change keypair's ssh key column type
 
 Revision ID: cace152eefac
-Revises: b6b884fbae1f
+Revises: 213a04e90ecf
 Create Date: 2023-02-10 15:43:51.482204
 
 """
 import sqlalchemy as sa
 from alembic import op
 
 # revision identifiers, used by Alembic.
 revision = "cace152eefac"
-down_revision = "b6b884fbae1f"
+down_revision = "213a04e90ecf"
 branch_labels = None
 depends_on = None
 
 
 def upgrade():
     op.alter_column(
         "keypairs", "ssh_public_key", existing_type=sa.String(length=750), type_=sa.Text
```

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/base.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/base.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/domain.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/domain.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/dotfile.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/dotfile.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/endpoint.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/error_logs.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/error_logs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/gql.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/gql.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/group.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/image.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/kernel.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/kernel.py`

 * *Files 1% similar despite different names*

```diff
@@ -556,14 +556,18 @@
 
     @property
     def cluster_name(self) -> str:
         if self.cluster_role == DEFAULT_ROLE:
             return self.cluster_role
         return self.cluster_role + str(self.cluster_idx)
 
+    @property
+    def is_private(self) -> bool:
+        return self.role in PRIVATE_KERNEL_ROLES
+
     @staticmethod
     async def get_kernel(
         db: ExtendedAsyncSAEngine, kern_id: uuid.UUID, allow_stale: bool = False
     ) -> KernelRow:
         from .agent import AgentStatus
 
         async with db.begin_readonly_session() as db_sess:
@@ -855,15 +859,15 @@
         self,
         info: graphene.ResolveInfo,
         access_key: AccessKey | None,
     ) -> Optional[Mapping[str, Any]]:
         graph_ctx: GraphQueryContext = info.context
         if access_key is None:
             return None
-        return await graph_ctx.registry.get_abusing_report(self.id, self.agent, self.agent_addr)
+        return await graph_ctx.registry.get_abusing_report(self.id)
 
     _queryfilter_fieldspec = {
         "image": ("image", None),
         "architecture": ("architecture", None),
         "agent": ("agent", None),
         "agent_addr": ("agent_addr", None),
         "cluster_idx": ("cluster_idx", None),
@@ -1438,16 +1442,34 @@
             .where(
                 (KernelRow.access_key == access_key)
                 & (KernelRow.status.in_(USER_RESOURCE_OCCUPYING_KERNEL_STATUSES))
                 & (KernelRow.role.not_in(PRIVATE_KERNEL_ROLES)),
             ),
         )
         concurrency_used = result.scalar()
+        result = await db_sess.execute(
+            sa.select(sa.func.count())
+            .select_from(KernelRow)
+            .where(
+                (KernelRow.access_key == access_key)
+                & (KernelRow.status.in_(USER_RESOURCE_OCCUPYING_KERNEL_STATUSES))
+                & (KernelRow.role.in_(PRIVATE_KERNEL_ROLES)),
+            ),
+        )
+        sftp_concurrency_used = result.scalar()
         assert isinstance(concurrency_used, int)
+        assert isinstance(sftp_concurrency_used, int)
 
     await redis_helper.execute(
         redis_stat,
         lambda r: r.set(
             f"keypair.concurrency_used.{access_key}",
             concurrency_used,
         ),
     )
+    await redis_helper.execute(
+        redis_stat,
+        lambda r: r.set(
+            f"keypair.sftp_concurrency_used.{access_key}",
+            sftp_concurrency_used,
+        ),
+    )
```

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/keypair.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/minilang/ordering.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/minilang/ordering.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/minilang/queryfilter.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/minilang/queryfilter.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/resource_policy.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/resource_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,17 @@
         EnumType(DefaultForUnspecified),
         default=DefaultForUnspecified.LIMITED,
         nullable=False,
     ),
     sa.Column("total_resource_slots", ResourceSlotColumn(), nullable=False),
     sa.Column("max_session_lifetime", sa.Integer(), nullable=False, server_default=sa.text("0")),
     sa.Column("max_concurrent_sessions", sa.Integer(), nullable=False),
+    sa.Column(
+        "max_concurrent_sftp_sessions", sa.Integer(), nullable=False, server_default=sa.text("1")
+    ),
     sa.Column("max_containers_per_session", sa.Integer(), nullable=False),
     sa.Column("max_vfolder_count", sa.Integer(), nullable=False),
     sa.Column("max_vfolder_size", sa.BigInteger(), nullable=False),
     sa.Column("idle_timeout", sa.BigInteger(), nullable=False),
     sa.Column(
         "allowed_vfolder_hosts",
         VFolderHostPermissionColumn(),
```

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/resource_preset.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/resource_preset.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/routing.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/routing.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/scaling_group.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/session.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -587,15 +587,14 @@
     # Resource occupation
     # occupied_slots = sa.Column('occupied_slots', ResourceSlotColumn(), nullable=False)
     occupying_slots = sa.Column("occupying_slots", ResourceSlotColumn(), nullable=False)
     requested_slots = sa.Column("requested_slots", ResourceSlotColumn(), nullable=False)
     vfolder_mounts = sa.Column(
         "vfolder_mounts", StructuredJSONObjectListColumn(VFolderMount), nullable=True
     )
-    resource_opts = sa.Column("resource_opts", pgsql.JSONB(), nullable=True, default={})
     environ = sa.Column("environ", pgsql.JSONB(), nullable=True, default={})
     bootstrap_script = sa.Column("bootstrap_script", sa.String(length=16 * 1024), nullable=True)
     use_host_network = sa.Column("use_host_network", sa.Boolean(), default=False, nullable=False)
 
     # Lifecycle
     timeout = sa.Column("timeout", sa.BigInteger(), nullable=True)
     created_at = sa.Column(
@@ -690,16 +689,27 @@
         if len(kerns) == 0:
             raise MainKernelNotFound(
                 f"Session (id: {self.id}) has no main kernel.",
             )
         return kerns[0]
 
     @property
-    def status_changed(self) -> datetime:
-        return datetime.fromisoformat(self.status_history[self.status.name])
+    def status_changed(self) -> Optional[datetime]:
+        try:
+            return datetime.fromisoformat(self.status_history[self.status.name])
+        except KeyError:
+            return None
+
+    @property
+    def resource_opts(self) -> dict[str, Any]:
+        return {kern.cluster_hostname: kern.resource_opts for kern in self.kernels}
+
+    @property
+    def is_private(self) -> bool:
+        return any([kernel.is_private for kernel in self.kernels])
 
     def get_kernel_by_cluster_name(self, cluster_name: str) -> KernelRow:
         kerns = tuple(kern for kern in self.kernels if kern.cluster_name == cluster_name)
         if len(kerns) > 1:
             raise TooManyKernelsFound(
                 f"Session (id: {self.id}) has more than 1 kernel with {cluster_name = }",
             )
@@ -1132,15 +1142,14 @@
 
 
 DEFAULT_SESSION_ORDERING = [
     sa.desc(
         sa.func.greatest(
             SessionRow.created_at,
             SessionRow.terminated_at,
-            # SessionRow.status_changed,
         )
     ),
 ]
 
 
 class ComputeSession(graphene.ObjectType):
     class Meta:
@@ -1148,14 +1157,15 @@
 
     # identity
     session_id = graphene.UUID()  # identical to `id`
     main_kernel_id = graphene.UUID()
     tag = graphene.String()
     name = graphene.String()
     type = graphene.String()
+    main_kernel_role = graphene.String()
 
     # image
     image = graphene.String()  # image for the main container
     architecture = graphene.String()  # image architecture for the main container
     registry = graphene.String()  # image registry for the main container
     cluster_template = graphene.String()
     cluster_mode = graphene.String()
@@ -1218,14 +1228,15 @@
             # identity
             "id": row.id,
             "session_id": row.id,
             "main_kernel_id": row.main_kernel.id,
             "tag": row.tag,
             "name": row.name,
             "type": row.session_type.name,
+            "main_kernel_role": row.main_kernel.role.name,
             # image
             # "image": row.image_id,
             "image": row.main_kernel.image,
             "architecture": row.main_kernel.architecture,
             "registry": row.main_kernel.registry,
             "cluster_template": None,  # TODO: implement
             "cluster_mode": row.cluster_mode,
@@ -1248,15 +1259,14 @@
             "status_history": row.status_history or {},
             "created_at": row.created_at,
             "terminated_at": row.terminated_at,
             "starts_at": row.starts_at,
             "startup_command": row.startup_command,
             "result": row.result.name,
             # resources
-            "resource_opts": row.resource_opts,
             "scaling_group": row.scaling_group_name,
             "service_ports": row.main_kernel.service_ports,
             "mounts": [mount.name for mount in row.vfolder_mounts],
             "vfolder_mounts": row.vfolder_mounts,
             # statistics
             "num_queries": row.num_queries,
         }
@@ -1329,22 +1339,32 @@
         async with graph_ctx.db.begin_readonly_session() as db_sess:
             session: SessionRow = await SessionRow.get_session_with_main_kernel(
                 self.id, db_session=db_sess
             )
         commit_status = await graph_ctx.registry.get_commit_status(session)
         return commit_status["status"]
 
+    async def resolve_resource_opts(self, info: graphene.ResolveInfo) -> dict[str, Any]:
+        containers = self.containers
+        if containers is None:
+            containers = await self.resolve_containers(info)
+        if containers is None:
+            return {}
+        self.containers = containers
+        return {cntr.cluster_hostname: cntr.resource_opts for cntr in containers}
+
     async def resolve_abusing_reports(
         self, info: graphene.ResolveInfo
     ) -> Iterable[Optional[Mapping[str, Any]]]:
         containers = self.containers
         if containers is None:
             containers = await self.resolve_containers(info)
         if containers is None:
             return []
+        self.containers = containers
         return [(await con.resolve_abusing_report(info, self.access_key)) for con in containers]
 
     async def resolve_idle_checks(self, info: graphene.ResolveInfo) -> Mapping[str, Any]:
         graph_ctx: GraphQueryContext = info.context
         return await graph_ctx.idle_checker_host.get_idle_check_report(self.session_id)
 
     _queryfilter_fieldspec = {
@@ -1357,15 +1377,14 @@
         "full_name": ("users_full_name", None),
         "access_key": ("sessions_access_key", None),
         "scaling_group": ("sessions_scaling_group_name", None),
         "cluster_mode": ("sessions_cluster_mode", lambda s: ClusterMode[s]),
         "cluster_size": ("sessions_cluster_size", None),
         "status": ("sessions_status", lambda s: SessionStatus[s]),
         "status_info": ("sessions_status_info", None),
-        # "status_changed": ("status_changed", dtparse),
         "result": ("sessions_result", lambda s: SessionResult[s]),
         "created_at": ("sessions_created_at", dtparse),
         "terminated_at": ("sessions_terminated_at", dtparse),
         "starts_at": ("sessions_starts_at", dtparse),
         "startup_command": ("sessions_startup_command", None),
     }
```

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/session_template.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/storage.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/user.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,14 +110,19 @@
     "users",
     mapper_registry.metadata,
     IDColumn("uuid"),
     sa.Column("username", sa.String(length=64), unique=True),
     sa.Column("email", sa.String(length=64), index=True, nullable=False, unique=True),
     sa.Column("password", PasswordColumn()),
     sa.Column("need_password_change", sa.Boolean),
+    sa.Column(
+        "password_changed_at",
+        sa.DateTime(timezone=True),
+        server_default=sa.func.now(),
+    ),
     sa.Column("full_name", sa.String(length=64)),
     sa.Column("description", sa.String(length=500)),
     sa.Column("status", EnumValueType(UserStatus), default=UserStatus.ACTIVE, nullable=False),
     sa.Column("status_info", sa.Unicode(), nullable=True, default=sa.null()),
     sa.Column("created_at", sa.DateTime(timezone=True), server_default=sa.func.now()),
     sa.Column(
         "modified_at",
@@ -633,14 +638,17 @@
         set_if_set(props, data, "allowed_client_ip")
         set_if_set(props, data, "totp_activated")
         if not data and not props.group_ids:
             return cls(ok=False, msg="nothing to update", user=None)
         if data.get("status") is None and props.is_active is not None:
             data["status"] = UserStatus.ACTIVE if props.is_active else UserStatus.INACTIVE
 
+        if data.get("password") is not None:
+            data["password_changed_at"] = sa.func.now()
+
         user_update_data: Dict[str, Any]
         prev_domain_name: str
         prev_role: UserRole
 
         async def _pre_func(conn: SAConnection) -> None:
             nonlocal user_update_data, prev_domain_name, prev_role
             result = await conn.execute(
@@ -1114,14 +1122,18 @@
         )
         if (row := ak_rows.first()) and (access_key := row.access_key):
             # Log concurrency used only when there is at least one keypair.
             await redis_helper.execute(
                 redis_conn,
                 lambda r: r.delete(f"keypair.concurrency_used.{access_key}"),
             )
+            await redis_helper.execute(
+                redis_conn,
+                lambda r: r.delete(f"keypair.sftp_concurrency_used.{access_key}"),
+            )
         result = await conn.execute(
             sa.delete(keypairs).where(keypairs.c.user == user_uuid),
         )
         if result.rowcount > 0:
             log.info("deleted {0} user's keypairs ({1})", result.rowcount, user_uuid)
         return result.rowcount
 
@@ -1130,14 +1142,21 @@
     return bcrypt.using(rounds=12).hash(password)
 
 
 def _verify_password(guess, hashed):
     return bcrypt.verify(guess, hashed)
 
 
+def compare_to_hashed_password(raw_password: str, hashed_password: str) -> bool:
+    """
+    Compare a raw string password value to hased password.
+    """
+    return _verify_password(raw_password, hashed_password)
+
+
 async def check_credential(
     db: SAEngine,
     domain: str,
     email: str,
     password: str,
 ) -> Any:
     async with db.begin_readonly() as conn:
```

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/utils.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/models/vfolder.py` & `backend.ai-manager-23.3.3/ai/backend/manager/models/vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/pglock.py` & `backend.ai-manager-23.3.3/ai/backend/manager/pglock.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/plugin/error_monitor.py` & `backend.ai-manager-23.3.3/ai/backend/manager/plugin/error_monitor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/plugin/webapp.py` & `backend.ai-manager-23.3.3/ai/backend/manager/plugin/webapp.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/registry.py` & `backend.ai-manager-23.3.3/ai/backend/manager/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     SessionTerminatedEvent,
     SessionTerminatingEvent,
 )
 from ai.backend.common.logging import BraceStyleAdapter
 from ai.backend.common.plugin.hook import ALL_COMPLETED, PASSED, HookPluginContext
 from ai.backend.common.service_ports import parse_service_ports
 from ai.backend.common.types import (
+    AbuseReport,
     AccessKey,
     AgentId,
     BinarySize,
     ClusterInfo,
     ClusterMode,
     ClusterSSHKeyPair,
     ClusterSSHPortMapping,
@@ -1366,19 +1367,22 @@
 
                 await execute_with_retry(_update_agent_resource)
 
     async def recalc_resource_usage(self, do_fullscan: bool = False) -> None:
         concurrency_used_per_key: MutableMapping[str, set] = defaultdict(
             set
         )  # key: access_key, value: set of session_id
-        occupied_slots_per_agent: MutableMapping[str, ResourceSlot] = defaultdict(
-            lambda: ResourceSlot({"cpu": 0, "mem": 0})
-        )
+        sftp_concurrency_used_per_key: MutableMapping[str, set] = defaultdict(
+            set
+        )  # key: access_key, value: set of session_id
 
         async def _recalc() -> None:
+            occupied_slots_per_agent: MutableMapping[str, ResourceSlot] = defaultdict(
+                lambda: ResourceSlot({"cpu": 0, "mem": 0})
+            )
             async with self.db.begin() as conn:
                 # Query running containers and calculate concurrency_used per AK and
                 # occupied_slots per agent.
                 query = (
                     sa.select([kernels.c.access_key, kernels.c.agent, kernels.c.occupied_slots])
                     .where(kernels.c.status.in_(AGENT_RESOURCE_OCCUPYING_KERNEL_STATUSES))
                     .order_by(sa.asc(kernels.c.access_key))
@@ -1388,26 +1392,25 @@
                 query = (
                     sa.select(
                         [
                             kernels.c.access_key,
                             kernels.c.session_id,
                             kernels.c.agent,
                             kernels.c.occupied_slots,
+                            kernels.c.role,
                         ]
                     )
-                    .where(
-                        (
-                            kernels.c.status.in_(USER_RESOURCE_OCCUPYING_KERNEL_STATUSES)
-                            & kernels.c.role.not_in(PRIVATE_KERNEL_ROLES)
-                        )
-                    )
+                    .where(kernels.c.status.in_(USER_RESOURCE_OCCUPYING_KERNEL_STATUSES))
                     .order_by(sa.asc(kernels.c.access_key))
                 )
                 async for row in await conn.stream(query):
-                    concurrency_used_per_key[row.access_key].add(row.session_id)
+                    if row.role in PRIVATE_KERNEL_ROLES:
+                        sftp_concurrency_used_per_key[row.access_key].add(row.session_id)
+                    else:
+                        concurrency_used_per_key[row.access_key].add(row.session_id)
 
                 if len(occupied_slots_per_agent) > 0:
                     # Update occupied_slots for agents with running containers.
                     for aid, slots in occupied_slots_per_agent.items():
                         query = (
                             sa.update(agents).values(occupied_slots=slots).where(agents.c.id == aid)
                         )
@@ -1428,30 +1431,39 @@
                     )
                     await conn.execute(query)
 
         await execute_with_retry(_recalc)
 
         # Update keypair resource usage for keypairs with running containers.
         kp_key = "keypair.concurrency_used"
+        sftp_kp_key = "keypair.sftp_concurrency_used"
 
         async def _update(r: Redis):
             updates = {
                 f"{kp_key}.{ak}": len(session_ids)
                 for ak, session_ids in concurrency_used_per_key.items()
+            } | {
+                f"{sftp_kp_key}.{ak}": len(session_ids)
+                for ak, session_ids in sftp_concurrency_used_per_key.items()
             }
             if updates:
                 await r.mset(typing.cast(MSetType, updates))
 
         async def _update_by_fullscan(r: Redis):
             updates = {}
             keys = await r.keys(f"{kp_key}.*")
             for ak in keys:
                 session_concurrency = concurrency_used_per_key.get(ak)
                 usage = len(session_concurrency) if session_concurrency is not None else 0
                 updates[f"{kp_key}.{ak}"] = usage
+            keys = await r.keys(f"{sftp_kp_key}.*")
+            for ak in keys:
+                session_concurrency = sftp_concurrency_used_per_key.get(ak)
+                usage = len(session_concurrency) if session_concurrency is not None else 0
+                updates[f"{sftp_kp_key}.{ak}"] = usage
             if updates:
                 await r.mset(typing.cast(MSetType, updates))
 
         if do_fullscan:
             await redis_helper.execute(
                 self.redis_stat,
                 _update_by_fullscan,
@@ -1664,24 +1676,25 @@
                                         values["last_stat"] = msgpack.unpackb(kern_stat)
                                     await db_sess.execute(
                                         sa.update(KernelRow)
                                         .values(**values)
                                         .where(KernelRow.id == kernel.id),
                                     )
 
-                            if (
-                                kernel.cluster_role == DEFAULT_ROLE
-                                and kernel.role not in PRIVATE_KERNEL_ROLES
-                            ):
+                            if kernel.cluster_role == DEFAULT_ROLE:
                                 # The main session is terminated;
                                 # decrement the user's concurrency counter
+                                if kernel.is_private:
+                                    kp_key = "keypair.sftp_concurrency_used"
+                                else:
+                                    kp_key = "keypair.concurrency_used"
                                 await redis_helper.execute(
                                     self.redis_stat,
                                     lambda r: r.incrby(
-                                        f"keypair.concurrency_used.{kernel.access_key}",
+                                        f"{kp_key}.{kernel.access_key}",
                                         -1,
                                     ),
                                 )
 
                             await execute_with_retry(_update)
                             await self.event_producer.produce_event(
                                 KernelTerminatedEvent(kernel.id, target_session.id, reason),
@@ -1708,24 +1721,25 @@
                                     }
                                     await db_sess.execute(
                                         sa.update(KernelRow)
                                         .values(**values)
                                         .where(KernelRow.id == kernel.id),
                                     )
 
-                            if (
-                                kernel.cluster_role == DEFAULT_ROLE
-                                and kernel.role not in PRIVATE_KERNEL_ROLES
-                            ):
+                            if kernel.cluster_role == DEFAULT_ROLE:
                                 # The main session is terminated;
                                 # decrement the user's concurrency counter
+                                if kernel.is_private:
+                                    kp_key = "keypair.sftp_concurrency_used"
+                                else:
+                                    kp_key = "keypair.concurrency_used"
                                 await redis_helper.execute(
                                     self.redis_stat,
                                     lambda r: r.incrby(
-                                        f"keypair.concurrency_used.{kernel.access_key}",
+                                        f"{kp_key}.{kernel.access_key}",
                                         -1,
                                     ),
                                 )
 
                             await execute_with_retry(_update)
                             await self.event_producer.produce_event(
                                 KernelTerminatingEvent(kernel.id, target_session.id, reason),
@@ -2172,14 +2186,15 @@
             SlotName(k): SlotTypes(v[0]) for k, v in agent_info["resource_slots"].items()
         }
         available_slots = ResourceSlot(
             {SlotName(k): Decimal(v[1]) for k, v in agent_info["resource_slots"].items()}
         )
         current_addr = agent_info["addr"]
         sgroup = agent_info.get("scaling_group", "default")
+        auto_terminate_abusing_kernel = agent_info["auto_terminate_abusing_kernel"]
         async with self.heartbeat_lock:
             instance_rejoin = False
 
             # Update "last seen" timestamp for liveness tracking
             await redis_helper.execute(
                 self.redis_live,
                 lambda r: r.hset("agent.last_seen", agent_id, now.timestamp()),
@@ -2196,14 +2211,15 @@
                                 agents.c.addr,
                                 agents.c.public_host,
                                 agents.c.scaling_group,
                                 agents.c.available_slots,
                                 agents.c.version,
                                 agents.c.compute_plugins,
                                 agents.c.architecture,
+                                agents.c.auto_terminate_abusing_kernel,
                             ]
                         )
                         .select_from(agents)
                         .where(agents.c.id == agent_id)
                         .with_for_update()
                     )
                     result = await conn.execute(fetch_query)
@@ -2224,14 +2240,15 @@
                                 "addr": agent_info["addr"],
                                 "public_host": agent_info["public_host"],
                                 "first_contact": now,
                                 "lost_at": sa.null(),
                                 "version": agent_info["version"],
                                 "compute_plugins": agent_info["compute_plugins"],
                                 "architecture": agent_info.get("architecture", "x86_64"),
+                                "auto_terminate_abusing_kernel": auto_terminate_abusing_kernel,
                             }
                         )
                         result = await conn.execute(insert_query)
                         assert result.rowcount == 1
                     elif row["status"] == AgentStatus.ALIVE:
                         updates = {}
                         if row["available_slots"] != available_slots:
@@ -2244,14 +2261,16 @@
                             updates["public_host"] = agent_info["public_host"]
                         if row["version"] != agent_info["version"]:
                             updates["version"] = agent_info["version"]
                         if row["compute_plugins"] != agent_info["compute_plugins"]:
                             updates["compute_plugins"] = agent_info["compute_plugins"]
                         if row["architecture"] != agent_info["architecture"]:
                             updates["architecture"] = agent_info["architecture"]
+                        if row["auto_terminate_abusing_kernel"] != auto_terminate_abusing_kernel:
+                            updates["auto_terminate_abusing_kernel"] = auto_terminate_abusing_kernel
                         # occupied_slots are updated when kernels starts/terminates
                         if updates:
                             await self.shared_config.update_resource_slots(slot_key_and_units)
                             update_query = (
                                 sa.update(agents).values(updates).where(agents.c.id == agent_id)
                             )
                             await conn.execute(update_query)
@@ -2268,14 +2287,15 @@
                                     "addr": agent_info["addr"],
                                     "public_host": agent_info["public_host"],
                                     "lost_at": sa.null(),
                                     "available_slots": available_slots,
                                     "version": agent_info["version"],
                                     "compute_plugins": agent_info["compute_plugins"],
                                     "architecture": agent_info["architecture"],
+                                    "auto_terminate_abusing_kernel": auto_terminate_abusing_kernel,
                                 }
                             )
                             .where(agents.c.id == agent_id)
                         )
                         await conn.execute(update_query)
                     else:
                         log.error("should not reach here! {0}", type(row["status"]))
@@ -2594,23 +2614,28 @@
             invoke_timeout=None,
         ) as rpc:
             return await rpc.call.get_local_config()
 
     async def get_abusing_report(
         self,
         kernel_id: KernelId,
-        agent_id: AgentId,
-        agent_addr: str,
-    ) -> Optional[Mapping[str, str]]:
-        async with RPCContext(
-            agent_id,
-            agent_addr,
-            invoke_timeout=None,
-        ) as rpc:
-            return await rpc.call.get_abusing_report(str(kernel_id))
+    ) -> Optional[AbuseReport]:
+        hash_name = "abuse_report"
+        abusing_report: Optional[dict[str, str]] = await redis_helper.execute(
+            self.redis_stat,
+            lambda r: r.hgetall(hash_name),
+            encoding="utf-8",
+        )
+        kern_id = str(kernel_id)
+        if abusing_report is None or (result := abusing_report.get(kern_id)) is None:
+            return None
+        return {
+            "kernel": kern_id,
+            "abuse_report": result,
+        }
 
 
 async def check_scaling_group(
     conn: SAConnection,
     scaling_group: str | None,
     session_type: SessionTypes,
     access_key: AccessKey,
```

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/scheduler/dispatcher.py` & `backend.ai-manager-23.3.3/ai/backend/manager/scheduler/dispatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,25 +28,24 @@
     SessionCancelledEvent,
     SessionEnqueuedEvent,
     SessionPreparingEvent,
     SessionScheduledEvent,
     SessionTerminatedEvent,
 )
 from ai.backend.common.logging import BraceStyleAdapter
-from ai.backend.common.types import AgentId, ClusterMode, ResourceSlot, aobject
+from ai.backend.common.types import AgentId, ClusterMode, ResourceSlot, SessionId, aobject
 from ai.backend.manager.models.agent import AgentRow
 from ai.backend.manager.types import DistributedLockFactory
 from ai.backend.plugin.entrypoint import scan_entrypoints
 
 from ..api.exceptions import GenericBadRequest, InstanceNotAvailable
 from ..defs import LockID
 from ..exceptions import convert_to_status_data
 from ..models import (
     AgentStatus,
-    KernelRole,
     KernelRow,
     KernelStatus,
     ScalingGroupRow,
     SessionRow,
     SessionStatus,
     list_schedulable_agents_by_sgroup,
     recalc_agent_resource_occupancy,
@@ -262,62 +261,67 @@
         return load_scheduler(scheduler_name, sgroup_opts, scheduler_specific_config)
 
     async def _schedule_in_sgroup(
         self,
         sched_ctx: SchedulingContext,
         sgroup_name: str,
     ) -> None:
+        async def _apply_cancellation(
+            db_sess: SASession, session_ids: list[SessionId], reason="pending-timeout"
+        ):
+            now = datetime.now(tzutc())
+            kernel_query = (
+                sa.update(KernelRow)
+                .values(
+                    status=KernelStatus.CANCELLED,
+                    status_info=reason,
+                    terminated_at=now,
+                    status_history=sql_json_merge(
+                        KernelRow.status_history,
+                        (),
+                        {
+                            KernelStatus.CANCELLED.name: now.isoformat(),
+                        },
+                    ),
+                )
+                .where(KernelRow.session_id.in_(session_ids))
+            )
+            await db_sess.execute(kernel_query)
+            query = (
+                sa.update(SessionRow)
+                .values(
+                    status=SessionStatus.CANCELLED,
+                    status_info=reason,
+                    terminated_at=now,
+                    status_history=sql_json_merge(
+                        SessionRow.status_history,
+                        (),
+                        {
+                            SessionStatus.CANCELLED.name: now.isoformat(),
+                        },
+                    ),
+                )
+                .where(SessionRow.id.in_(session_ids))
+            )
+            await db_sess.execute(query)
+
         async with self.db.begin_readonly_session() as db_sess:
             scheduler = await self._load_scheduler(db_sess, sgroup_name)
             existing_sessions, pending_sessions, cancelled_sessions = await _list_managed_sessions(
                 db_sess, sgroup_name, scheduler.sgroup_opts.pending_timeout
             )
 
         if cancelled_sessions:
-            now = datetime.now(tzutc())
             session_ids = [item.id for item in cancelled_sessions]
 
-            async def _apply_cancellation():
+            async def _update():
                 async with self.db.begin_session() as db_sess:
-                    kernel_query = (
-                        sa.update(KernelRow)
-                        .values(
-                            status=KernelStatus.CANCELLED,
-                            status_info="pending-timeout",
-                            terminated_at=now,
-                            status_history=sql_json_merge(
-                                KernelRow.status_history,
-                                (),
-                                {
-                                    KernelStatus.CANCELLED.name: now.isoformat(),
-                                },
-                            ),
-                        )
-                        .where(KernelRow.session_id.in_(session_ids))
-                    )
-                    await db_sess.execute(kernel_query)
-                    query = (
-                        sa.update(SessionRow)
-                        .values(
-                            status=SessionStatus.CANCELLED,
-                            status_info="pending-timeout",
-                            terminated_at=now,
-                            status_history=sql_json_merge(
-                                SessionRow.status_history,
-                                (),
-                                {
-                                    SessionStatus.CANCELLED.name: now.isoformat(),
-                                },
-                            ),
-                        )
-                        .where(SessionRow.id.in_(session_ids))
-                    )
-                    await db_sess.execute(query)
+                    await _apply_cancellation(db_sess, session_ids)
 
-            await execute_with_retry(_apply_cancellation)
+            await execute_with_retry(_update)
             for item in cancelled_sessions:
                 await self.event_producer.produce_event(
                     SessionCancelledEvent(
                         item.id,
                         item.creation_id,
                         reason=KernelLifecycleEventReason.PENDING_TIMEOUT,
                     ),
@@ -370,18 +374,18 @@
                 async with self.db.begin_session() as db_sess:
                     predicates: list[Tuple[str, Awaitable[PredicateResult]]] = [
                         (
                             "reserved_time",
                             check_reserved_batch_session(db_sess, sched_ctx, sess_ctx),
                         ),
                         ("dependencies", check_dependencies(db_sess, sched_ctx, sess_ctx)),
+                        ("concurrency", check_concurrency(db_sess, sched_ctx, sess_ctx)),
                     ]
-                    if any([kernel.role != KernelRole.SYSTEM for kernel in sess_ctx.kernels]):
+                    if not sess_ctx.is_private:
                         predicates += [
-                            ("concurrency", check_concurrency(db_sess, sched_ctx, sess_ctx)),
                             (
                                 "keypair_resource_limit",
                                 check_keypair_resource_limit(db_sess, sched_ctx, sess_ctx),
                             ),
                             (
                                 "user_group_resource_limit",
                                 check_group_resource_limit(db_sess, sched_ctx, sess_ctx),
@@ -434,15 +438,15 @@
                 "last_try": datetime.now(tzutc()).isoformat(),
                 "failed_predicates": failed_predicates,
                 "passed_predicates": passed_predicates,
             }
             if has_failure:
                 log.debug(log_fmt + "predicate-checks-failed (temporary)", *log_args)
 
-                async def _update() -> None:
+                async def _cancel_failed_system_session() -> None:
                     async with self.db.begin_session() as db_sess:
                         await _rollback_predicate_mutations(
                             db_sess,
                             sched_ctx,
                             sess_ctx,
                         )
                         query = (
@@ -454,22 +458,31 @@
                                     ("scheduler", "retries"),
                                     parent_updates=status_update_data,
                                 ),
                             )
                             .where(SessionRow.id == sess_ctx.id)
                         )
                         await db_sess.execute(query)
+                        if sess_ctx.is_private:
+                            await _apply_cancellation(db_sess, [sess_ctx.id])
+                            await self.event_producer.produce_event(
+                                SessionCancelledEvent(
+                                    sess_ctx.id,
+                                    sess_ctx.creation_id,
+                                    reason=KernelLifecycleEventReason.PENDING_TIMEOUT,
+                                )
+                            )
 
-                await execute_with_retry(_update)
+                await execute_with_retry(_cancel_failed_system_session)
                 # Predicate failures are *NOT* permanent errors.
                 # We need to retry the scheduling afterwards.
                 continue
             else:
 
-                async def _update() -> None:
+                async def _update_session_status_data() -> None:
                     async with self.db.begin_session() as db_sess:
                         kernel_query = (
                             sa.update(KernelRow)
                             .where(KernelRow.session_id == sess_ctx.id)
                             .values(
                                 status_data=sql_json_merge(
                                     KernelRow.status_data,
@@ -488,15 +501,15 @@
                                     ("scheduler",),
                                     obj=status_update_data,
                                 ),
                             )
                         )
                         await db_sess.execute(session_query)
 
-                await execute_with_retry(_update)
+                await execute_with_retry(_update_session_status_data)
 
             async with self.db.begin_readonly_session() as db_sess:
                 schedulable_sess = await SessionRow.get_session_by_id(
                     db_sess,
                     sess_ctx.id,
                     eager_loading_op=(
                         noload("*"),
@@ -578,15 +591,15 @@
                     compatible_candidate_agents, sess_ctx
                 )
                 if cand_agent is None:
                     raise InstanceNotAvailable(
                         extra_msg=(
                             "Could not find a contiguous resource region in any agent "
                             "big enough to host the session "
-                            f"({sess_ctx.id})"
+                            f"(id: {sess_ctx.id}, resource group: {sess_ctx.scaling_group_name})"
                         ),
                     )
                 assert cand_agent is not None
                 agent_id = cand_agent
             async with self.db.begin_session() as agent_db_sess:
                 query = sa.select(AgentRow.available_slots).where(AgentRow.id == agent_id)
                 available_agent_slots = (await agent_db_sess.execute(query)).scalar()
@@ -778,17 +791,17 @@
                         # Let the scheduler check the resource availability and decide the target agent
                         agent = scheduler.assign_agent_for_kernel(
                             compatible_candidate_agents, kernel
                         )
                         if agent is None:
                             raise InstanceNotAvailable(
                                 extra_msg=(
-                                    "Could not find a contiguous resource region in any agent "
-                                    "big enough to host a kernel in the session "
-                                    f"({sess_ctx.id})"
+                                    "Could not find a contiguous resource region in any agent big"
+                                    f" enough to host a kernel in the session (id: {sess_ctx.id},"
+                                    f" resource group: {sess_ctx.scaling_group_name})"
                                 ),
                             )
                     assert agent is not None
 
                     async def _reserve() -> None:
                         nonlocal agent_alloc_ctx, candidate_agents
                         async with agent_db_sess.begin_nested():
```

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/scheduler/drf.py` & `backend.ai-manager-23.3.3/ai/backend/manager/scheduler/drf.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/scheduler/fifo.py` & `backend.ai-manager-23.3.3/ai/backend/manager/scheduler/fifo.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/scheduler/mof.py` & `backend.ai-manager-23.3.3/ai/backend/manager/scheduler/mof.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/scheduler/predicates.py` & `backend.ai-manager-23.3.3/ai/backend/manager/scheduler/predicates.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,26 +65,34 @@
     sched_ctx: SchedulingContext,
     sess_ctx: SessionRow,
 ) -> PredicateResult:
     async def _get_max_concurrent_sessions() -> int:
         resouce_policy_q = sa.select(KeyPairRow.resource_policy).where(
             KeyPairRow.access_key == sess_ctx.access_key
         )
-        select_query = sa.select(KeyPairResourcePolicyRow.max_concurrent_sessions).where(
+        if sess_ctx.is_private:
+            concurrent_session_column = KeyPairResourcePolicyRow.max_concurrent_sftp_sessions
+        else:
+            concurrent_session_column = KeyPairResourcePolicyRow.max_concurrent_sessions
+        select_query = sa.select(concurrent_session_column).where(
             KeyPairResourcePolicyRow.name == resouce_policy_q.scalar_subquery()
         )
         result = await db_sess.execute(select_query)
         return result.scalar()
 
     max_concurrent_sessions = await execute_with_retry(_get_max_concurrent_sessions)
+    if sess_ctx.is_private:
+        redis_key = f"keypair.sftp_concurrency_used.{sess_ctx.access_key}"
+    else:
+        redis_key = f"keypair.concurrency_used.{sess_ctx.access_key}"
     ok, concurrency_used = await redis_helper.execute_script(
         sched_ctx.registry.redis_stat,
         "check_keypair_concurrency_used",
         _check_keypair_concurrency_script,
-        [f"keypair.concurrency_used.{sess_ctx.access_key}"],
+        [redis_key],
         [max_concurrent_sessions],
     )
     if ok == 0:
         return PredicateResult(
             False,
             f"You cannot run more than {max_concurrent_sessions} concurrent sessions",
         )
```

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/scheduler/types.py` & `backend.ai-manager-23.3.3/ai/backend/manager/scheduler/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/server.py` & `backend.ai-manager-23.3.3/ai/backend/manager/server.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/ai/backend/manager/types.py` & `backend.ai-manager-23.3.3/ai/backend/manager/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.2/backend.ai_manager.egg-info/PKG-INFO` & `backend.ai-manager-23.3.3/backend.ai_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-manager
-Version: 23.3.2
+Version: 23.3.3
 Summary: Backend.AI Manager
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Requires-Python: >=3.11,<3.12
 Description-Content-Type: text/markdown
 
 Backend.AI Manager with API Gateway
 ===================================
```

### Comparing `backend.ai-manager-23.3.2/backend.ai_manager.egg-info/SOURCES.txt` & `backend.ai-manager-23.3.3/backend.ai_manager.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py
 ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py
 ai/backend/manager/models/alembic/versions/1e673659b283_add_clusterized_column_to_agents_table.py
 ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py
 ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py
 ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py
 ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py
+ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py
 ai/backend/manager/models/alembic/versions/213a04e90ecf_merge.py
 ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py
 ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py
 ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py
 ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py
 ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py
 ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py
@@ -140,14 +141,15 @@
 ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py
 ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py
 ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py
 ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py
 ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py
 ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py
 ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py
+ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py
 ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py
 ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py
 ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py
 ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py
 ai/backend/manager/models/alembic/versions/95f51fc6ffdb_merge.py
 ai/backend/manager/models/alembic/versions/97f6c80c8aa5_merge.py
 ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py
@@ -174,17 +176,19 @@
 ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py
 ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py
 ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py
 ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py
 ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py
 ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py
 ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py
+ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py
 ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py
 ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py
 ai/backend/manager/models/alembic/versions/d643752544de_.py
+ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py
 ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py
 ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py
 ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py
 ai/backend/manager/models/alembic/versions/dc9b66466e43_remove_clusterized.py
 ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py
 ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py
 ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py
```

### Comparing `backend.ai-manager-23.3.2/backend.ai_manager.egg-info/requires.txt` & `backend.ai-manager-23.3.3/backend.ai_manager.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 aiohttp_sse>=2.0
 aiohttp~=3.8.1
 aiomonitor-ng~=0.7.2
 aiotools~=1.6.1
 alembic~=1.8.1
 async_timeout~=4.0
 attrs>=20.3
-backend.ai-cli==23.03.2
-backend.ai-common==23.03.2
-backend.ai-plugin==23.03.2
+backend.ai-cli==23.03.3
+backend.ai-common==23.03.3
+backend.ai-plugin==23.03.3
 callosum~=0.9.10
 click>=7.1.2
 cryptography>=2.8
 graphene~=2.1.9
 lark-parser~=0.11.3
 more-itertools~=8.13.0
 msgpack>=1.0.5rc1
 multidict>=6.0
 passlib[bcrypt]>=1.7.4
 python-dateutil>=2.8
 pyzmq~=24.0.1
-redis[hiredis]~=4.3.4
+redis[hiredis]~=4.5.5
 setproctitle~=1.2.2
 tabulate~=0.8.9
 tenacity>=8.0
 trafaret~=2.1
 typing_extensions~=4.3
 yarl~=1.8.2
```

### Comparing `backend.ai-manager-23.3.2/backend_shim.py` & `backend.ai-manager-23.3.3/backend_shim.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 build_wheel = True
 build_sdist = True
 wheel_config_settings = {
 }
 sdist_config_settings = {
 }
 
-os.makedirs(dist_dir, exist_ok=True)
+# Python 2.7 doesn't have the exist_ok arg on os.makedirs().
+try:
+    os.makedirs(dist_dir)
+except OSError as e:
+    if e.errno != errno.EEXIST:
+        raise
+
 wheel_path = backend.build_wheel(dist_dir, wheel_config_settings) if build_wheel else None
 sdist_path = backend.build_sdist(dist_dir, sdist_config_settings) if build_sdist else None
 
 if wheel_path:
     print("wheel: {wheel_path}".format(wheel_path=wheel_path))
 if sdist_path:
     print("sdist: {sdist_path}".format(sdist_path=sdist_path))
```

### Comparing `backend.ai-manager-23.3.2/setup.py` & `backend.ai-manager-23.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Environment :: No Input/Output (Daemon)',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development',
         'Development Status :: 5 - Production/Stable',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)',
     ],
     'description': 'Backend.AI Manager',
     'entry_points': {
         'backendai_cli_v10': [
             'mgr = ai.backend.manager.cli.__main__:main',
             'mgr.start-server = ai.backend.manager.server:main',
@@ -44,32 +45,32 @@
         'aiohttp_sse>=2.0',
         'aiohttp~=3.8.1',
         'aiomonitor-ng~=0.7.2',
         'aiotools~=1.6.1',
         'alembic~=1.8.1',
         'async_timeout~=4.0',
         'attrs>=20.3',
-        """backend.ai-cli==23.03.2
+        """backend.ai-cli==23.03.3
 """,
-        """backend.ai-common==23.03.2
+        """backend.ai-common==23.03.3
 """,
-        """backend.ai-plugin==23.03.2
+        """backend.ai-plugin==23.03.3
 """,
         'callosum~=0.9.10',
         'click>=7.1.2',
         'cryptography>=2.8',
         'graphene~=2.1.9',
         'lark-parser~=0.11.3',
         'more-itertools~=8.13.0',
         'msgpack>=1.0.5rc1',
         'multidict>=6.0',
         'passlib[bcrypt]>=1.7.4',
         'python-dateutil>=2.8',
         'pyzmq~=24.0.1',
-        'redis[hiredis]~=4.3.4',
+        'redis[hiredis]~=4.5.5',
         'setproctitle~=1.2.2',
         'tabulate~=0.8.9',
         'tenacity>=8.0',
         'trafaret~=2.1',
         'typing_extensions~=4.3',
         'uvloop>=0.17; sys_platform != "Windows"',
         'yarl~=1.8.2',
@@ -368,11 +369,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.2
+    'version': """23.03.3
 """,
     'zip_safe': False,
 })
```

