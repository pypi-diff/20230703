# Comparing `tmp/backend.ai-manager-23.3.6.tar.gz` & `tmp/backend.ai-manager-23.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-manager-23.3.6.tar", last modified: Wed Jun 14 11:13:22 2023, max compression
+gzip compressed data, was "backend.ai-manager-23.3.7.tar", last modified: Mon Jul  3 16:26:16 2023, max compression
```

## Comparing `backend.ai-manager-23.3.6.tar` & `backend.ai-manager-23.3.7.tar`

### file list

```diff
@@ -1,247 +1,250 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:22.513664 backend.ai-manager-23.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-14 11:13:22.513664 backend.ai-manager-23.3.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:22.489664 backend.ai-manager-23.3.6/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:22.489664 backend.ai-manager-23.3.6/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:22.493664 backend.ai-manager-23.3.6/ai/backend/manager/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:22.493664 backend.ai-manager-23.3.6/ai/backend/manager/api/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    40846 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/domainconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/groupconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (123)    36500 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    22820 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    76748 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/session_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    32921 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/userconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    12325 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   119753 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/api/wsproxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:22.497664 backend.ai-manager-23.3.6/ai/backend/manager/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/cli/dbschema.py
--rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/cli/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/cli/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/cli/gql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/cli/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/cli/image_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    26658 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:22.497664 backend.ai-manager-23.3.6/ai/backend/manager/container_registry/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/container_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/container_registry/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/container_registry/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/container_registry/harbor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/container_registry/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    39934 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/idle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:22.501664 backend.ai-manager-23.3.6/ai/backend/manager/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    21947 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:22.501664 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:22.513664 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/06184d82a211_add_session_creation_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/0e558d06e0e3_add_service_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/0f7a4b643940_.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/1e673659b283_add_clusterized_column_to_agents_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/213a04e90ecf_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/360af8f33d4e_merge_f83d_and_1f55.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/36b69ddee76e_.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/3cf19d906e71_.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/3f1dafab60b2_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9112 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/51dddd79aa21_add_logs_column_on_kernel_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/57e717103287_rename_clone_allowed_to_cloneable.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/5e88398bc340_add_unmanaged_path_column_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/65c4a109bbc7_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/95f51fc6ffdb_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/97f6c80c8aa5_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/a7ca9f175d5f_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py
--rw-r--r--   0 runner    (1001) docker     (123)    29414 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/bf4bae8f942e_add_kernel_host.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/c1409ad0e8da_.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/c3e74dcf1808_add_environ_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/d643752544de_.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/dc9b66466e43_remove_clusterized.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/eec98e65902a_merge_with_vfolder_clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/ff4bfca66bf8_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33946 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/dotfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/error_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    49801 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/gql.py
--rw-r--r--   0 runner    (1001) docker     (123)    24553 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    31776 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    51191 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)    20630 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/keypair.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:22.513664 backend.ai-manager-23.3.6/ai/backend/manager/models/minilang/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/minilang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/minilang/ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/minilang/queryfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/resource_preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)    23805 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    56406 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/session_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    42526 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    46387 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/models/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/pglock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:22.513664 backend.ai-manager-23.3.6/ai/backend/manager/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/plugin/error_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/plugin/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/plugin/webapp.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   159742 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:22.513664 backend.ai-manager-23.3.6/ai/backend/manager/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61786 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/scheduler/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/scheduler/drf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/scheduler/fifo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/scheduler/mof.py
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/scheduler/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/scheduler/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    30008 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/ai/backend/manager/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:22.513664 backend.ai-manager-23.3.6/backend.ai_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-14 11:13:22.000000 backend.ai-manager-23.3.6/backend.ai_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14442 2023-06-14 11:13:22.000000 backend.ai-manager-23.3.6/backend.ai_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:13:22.000000 backend.ai-manager-23.3.6/backend.ai_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-14 11:13:22.000000 backend.ai-manager-23.3.6/backend.ai_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:13:22.000000 backend.ai-manager-23.3.6/backend.ai_manager.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:13:22.000000 backend.ai-manager-23.3.6/backend.ai_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-14 11:13:22.000000 backend.ai-manager-23.3.6/backend.ai_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-14 11:13:22.000000 backend.ai-manager-23.3.6/backend.ai_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 11:13:22.513664 backend.ai-manager-23.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-06-14 11:13:21.000000 backend.ai-manager-23.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.730410 backend.ai-manager-23.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-07-03 16:26:16.730410 backend.ai-manager-23.3.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.702409 backend.ai-manager-23.3.7/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.702409 backend.ai-manager-23.3.7/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.706410 backend.ai-manager-23.3.7/ai/backend/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.710409 backend.ai-manager-23.3.7/ai/backend/manager/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41187 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/domainconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/groupconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36500 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22820 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76777 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32921 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/userconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121225 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/wsproxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.710409 backend.ai-manager-23.3.7/ai/backend/manager/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/cli/dbschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/cli/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/cli/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/cli/gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/cli/image_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26658 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.710409 backend.ai-manager-23.3.7/ai/backend/manager/container_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/container_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/container_registry/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/container_registry/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/container_registry/harbor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/container_registry/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39934 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/idle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.714409 backend.ai-manager-23.3.7/ai/backend/manager/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.714409 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.730410 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/06184d82a211_add_session_creation_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/0e558d06e0e3_add_service_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/0f7a4b643940_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/1e673659b283_add_clusterized_column_to_agents_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/213a04e90ecf_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/360af8f33d4e_merge_f83d_and_1f55.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/36b69ddee76e_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/3cf19d906e71_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/3f1dafab60b2_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9112 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/51dddd79aa21_add_logs_column_on_kernel_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/57e717103287_rename_clone_allowed_to_cloneable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/5e88398bc340_add_unmanaged_path_column_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/65c4a109bbc7_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/95f51fc6ffdb_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/97f6c80c8aa5_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/9e599b62f6f1_update_kernels_vfolder_mounts_vfid_.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/a7ca9f175d5f_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/a9eb2b002330_add_new_resource_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29414 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/bf4bae8f942e_add_kernel_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c1409ad0e8da_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c3e74dcf1808_add_environ_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d643752544de_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/dc9b66466e43_remove_clusterized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/eec98e65902a_merge_with_vfolder_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/ff4bfca66bf8_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34759 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/dotfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/error_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54934 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25170 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31776 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51383 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22869 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/keypair.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.730410 backend.ai-manager-23.3.7/ai/backend/manager/models/minilang/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/minilang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/minilang/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/minilang/queryfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24594 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/resource_preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23805 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56694 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43458 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12278 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55151 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11475 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/pglock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.730410 backend.ai-manager-23.3.7/ai/backend/manager/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/plugin/error_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/plugin/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/plugin/webapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   159742 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.730410 backend.ai-manager-23.3.7/ai/backend/manager/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61786 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/scheduler/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/scheduler/drf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/scheduler/fifo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/scheduler/mof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/scheduler/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/scheduler/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30006 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.730410 backend.ai-manager-23.3.7/backend.ai_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-07-03 16:26:16.000000 backend.ai-manager-23.3.7/backend.ai_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-07-03 16:26:16.000000 backend.ai-manager-23.3.7/backend.ai_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:26:16.000000 backend.ai-manager-23.3.7/backend.ai_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-03 16:26:16.000000 backend.ai-manager-23.3.7/backend.ai_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:26:16.000000 backend.ai-manager-23.3.7/backend.ai_manager.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:26:16.000000 backend.ai-manager-23.3.7/backend.ai_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-03 16:26:16.000000 backend.ai-manager-23.3.7/backend.ai_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-03 16:26:16.000000 backend.ai-manager-23.3.7/backend.ai_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 16:26:16.730410 backend.ai-manager-23.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/setup.py
```

### Comparing `backend.ai-manager-23.3.6/PKG-INFO` & `backend.ai-manager-23.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-manager
-Version: 23.3.6
+Version: 23.3.7
 Summary: Backend.AI Manager
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/acl.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/admin.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/admin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/auth.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -566,36 +566,39 @@
     @functools.wraps(handler)
     async def wrapped(request, *args, **kwargs):
         if request.get("is_authorized", False):
             return await handler(request, *args, **kwargs)
         raise AuthorizationFailed("Unauthorized access")
 
     set_handler_attr(wrapped, "auth_required", True)
+    set_handler_attr(wrapped, "auth_scope", "user")
     return wrapped
 
 
 def admin_required(handler):
     @functools.wraps(handler)
     async def wrapped(request, *args, **kwargs):
         if request.get("is_authorized", False) and request.get("is_admin", False):
             return await handler(request, *args, **kwargs)
         raise AuthorizationFailed("Unauthorized access")
 
     set_handler_attr(wrapped, "auth_required", True)
+    set_handler_attr(wrapped, "auth_scope", "admin")
     return wrapped
 
 
 def superadmin_required(handler):
     @functools.wraps(handler)
     async def wrapped(request, *args, **kwargs):
         if request.get("is_authorized", False) and request.get("is_superadmin", False):
             return await handler(request, *args, **kwargs)
         raise AuthorizationFailed("Unauthorized access")
 
     set_handler_attr(wrapped, "auth_required", True)
+    set_handler_attr(wrapped, "auth_scope", "superadmin")
     return wrapped
 
 
 @auth_required
 @check_api_params(
     t.Dict(
         {
@@ -798,18 +801,22 @@
             "need_password_change": False,
             "full_name": params["full_name"] if "full_name" in params else "",
             "description": params["description"] if "description" in params else "",
             "status": UserStatus.ACTIVE,
             "status_info": "user-signup",
             "role": UserRole.USER,
             "integration_id": None,
+            "resource_policy": "default",
         }
         if user_data_overriden:
             for key, val in user_data_overriden.items():
-                if key in data:  # take only valid fields
+                if (
+                    key in data  # take only valid fields
+                    and key != "resource_policy"  # resource_policy in user_data is for keypair
+                ):
                     data[key] = val
         query = users.insert().values(data)
         result = await conn.execute(query)
         if result.rowcount > 0:
             checkq = users.select().where(users.c.email == params["email"])
             result = await conn.execute(checkq)
             user = result.first()
```

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/cluster_template.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/cluster_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/context.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/domainconfig.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/domainconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/etcd.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/events.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/events.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/exceptions.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/groupconfig.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/groupconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/image.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/logs.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/logs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/manager.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     GenericBadRequest,
     InstanceNotFound,
     InvalidAPIParameters,
     ServerFrozen,
     ServiceUnavailable,
 )
 from .types import CORSOptions, WebMiddleware
-from .utils import check_api_params
+from .utils import check_api_params, set_handler_attr
 
 if TYPE_CHECKING:
     from ai.backend.manager.models.gql import GraphQueryContext
 
     from .context import RootContext
 
 log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
@@ -57,14 +57,17 @@
             if status not in allowed_status:
                 if status == ManagerStatus.FROZEN:
                     raise ServerFrozen
                 msg = f"Server is not in the required status: {allowed_status}"
                 raise ServiceUnavailable(msg)
             return await handler(request, *args, **kwargs)
 
+        set_handler_attr(wrapped, "server_status_required", True)
+        set_handler_attr(wrapped, "required_server_statuses", allowed_status)
+
         return wrapped
 
     return decorator
 
 
 READ_ALLOWED: Final = frozenset({ManagerStatus.RUNNING, ManagerStatus.FROZEN})
 ALL_ALLOWED: Final = frozenset({ManagerStatus.RUNNING})
```

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/ratelimit.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/ratelimit.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/resource.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/resource.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/scaling_group.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/service.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/service.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/session.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 from ai.backend.common.logging import BraceStyleAdapter
 from ai.backend.common.plugin.monitor import GAUGE
 from ai.backend.common.types import (
     AccessKey,
     AgentId,
     ClusterMode,
     SessionTypes,
+    VFolderID,
 )
 
 from ..config import DEFAULT_CHUNK_SIZE
 from ..defs import DEFAULT_IMAGE_ARCH, DEFAULT_ROLE
 from ..models import (
     AGENT_RESOURCE_OCCUPYING_KERNEL_STATUSES,
     DEAD_SESSION_STATUSES,
@@ -1820,15 +1821,15 @@
     try:
         async with root_ctx.storage_manager.request(
             log_vfolder["host"],
             "POST",
             "folder/file/fetch",
             json={
                 "volume": volume_name,
-                "vfid": str(log_vfolder["id"]),
+                "vfid": str(VFolderID.from_row(log_vfolder)),
                 "relpath": str(
                     PurePosixPath("task")
                     / kernel_id_str[:2]
                     / kernel_id_str[2:4]
                     / f"{kernel_id_str[4:]}.log",
                 ),
             },
```

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/session_template.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/stream.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/stream.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/types.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/userconfig.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/userconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/utils.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,16 @@
                     kwargs["query"] = query_params
             except (json.decoder.JSONDecodeError, yaml.YAMLError, yaml.MarkedYAMLError):
                 raise InvalidAPIParameters("Malformed body")
             except t.DataError as e:
                 raise InvalidAPIParameters("Input validation error", extra_data=e.as_dict())
             return await handler(request, checked_params, *args, **kwargs)
 
+        set_handler_attr(wrapped, "request_scheme", checker)
+
         return wrapped
 
     return wrap
 
 
 _danger_words = ["password", "passwd", "secret"]
```

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/vfolder.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/vfolder.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,47 +30,51 @@
 import aiohttp
 import aiohttp_cors
 import aiotools
 import attrs
 import sqlalchemy as sa
 import trafaret as t
 from aiohttp import web
+from sqlalchemy.orm import selectinload
 
 from ai.backend.common import msgpack, redis_helper
 from ai.backend.common import validators as tx
 from ai.backend.common.logging import BraceStyleAdapter
 from ai.backend.common.types import (
+    QuotaScopeID,
+    QuotaScopeType,
     RedisConnectionInfo,
     VFolderHostPermission,
     VFolderHostPermissionMap,
     VFolderID,
     VFolderUsageMode,
 )
 from ai.backend.manager.models.storage import StorageSessionManager
 
 from ..models import (
     ACTIVE_USER_STATUSES,
     AgentStatus,
+    GroupRow,
     KernelStatus,
     UserRole,
+    UserRow,
     UserStatus,
     VFolderAccessStatus,
     VFolderCloneInfo,
     VFolderDeletionInfo,
     VFolderInvitationState,
     VFolderOperationStatus,
     VFolderOwnershipType,
     VFolderPermission,
     VFolderPermissionValidator,
     agents,
     ensure_host_permission_allowed,
     filter_host_allowed_permission,
     get_allowed_vfolder_hosts_by_group,
     get_allowed_vfolder_hosts_by_user,
-    groups,
     initiate_vfolder_clone,
     initiate_vfolder_removal,
     kernels,
     keypair_resource_policies,
     keypairs,
     query_accessible_vfolders,
     query_owned_dotfiles,
@@ -328,15 +332,15 @@
 )
 async def create(request: web.Request, params: Any) -> web.Response:
     resp: Dict[str, Any] = {}
     root_ctx: RootContext = request.app["_root.context"]
     access_key = request["keypair"]["access_key"]
     user_role = request["user"]["role"]
     user_uuid: uuid.UUID = request["user"]["uuid"]
-    resource_policy = request["keypair"]["resource_policy"]
+    keypair_resource_policy = request["keypair"]["resource_policy"]
     domain_name = request["user"]["domain_name"]
     group_id_or_name = params["group"]
     log.info(
         "VFOLDER.CREATE (email:{}, ak:{}, vf:{}, vfh:{}, umod:{}, perm:{})",
         request["user"]["email"],
         access_key,
         params["name"],
@@ -366,80 +370,100 @@
         raise InvalidAPIParameters(f'{params["name"]} is reserved for internal operations.')
     if params["name"].startswith(".") and params["name"] != ".local":
         if params["group"] is not None:
             raise InvalidAPIParameters("dot-prefixed vfolders cannot be a group folder.")
 
     group_uuid: uuid.UUID | None = None
 
-    async with root_ctx.db.begin() as conn:
+    async with root_ctx.db.begin_session() as sess:
         match group_id_or_name:
             case str():
                 # Convert the group name to group uuid.
                 query = (
-                    sa.select([groups.c.id])
-                    .select_from(groups)
-                    .where(groups.c.domain_name == domain_name)
-                    .where(groups.c.name == group_id_or_name)
+                    sa.select(GroupRow)
+                    .where(
+                        (GroupRow.domain_name == domain_name) & (GroupRow.name == group_id_or_name)
+                    )
+                    .options(selectinload(GroupRow.resource_policy_row))
+                )
+                result = await sess.execute(query)
+                group_row = result.scalar()
+                _gid, max_vfolder_size = (
+                    group_row.id,
+                    group_row.resource_policy_row.max_vfolder_size,
                 )
-                _gid = await conn.scalar(query)
                 if _gid is None:
                     raise GroupNotFound(extra_data=group_id_or_name)
                 group_uuid = _gid
             case uuid.UUID():
                 # Check if the group belongs to the current domain.
                 query = (
-                    sa.select([groups.c.id])
-                    .select_from(groups)
-                    .where(groups.c.domain_name == domain_name)
-                    .where(groups.c.id == group_id_or_name)
+                    sa.select(GroupRow)
+                    .where(
+                        (GroupRow.domain_name == domain_name) & (GroupRow.id == group_id_or_name)
+                    )
+                    .options(selectinload(GroupRow.resource_policy_row))
+                )
+                result = await sess.execute(query)
+                group_row = result.scalar()
+                _gid, max_vfolder_size = (
+                    group_row.id,
+                    group_row.resource_policy_row.max_vfolder_size,
                 )
-                _gid = await conn.scalar(query)
                 if _gid is None:
                     raise GroupNotFound(extra_data=group_id_or_name)
                 group_uuid = group_id_or_name
             case None:
-                pass
+                query = (
+                    sa.select(UserRow)
+                    .where(UserRow.uuid == user_uuid)
+                    .options(selectinload(UserRow.resource_policy_row))
+                )
+                result = await sess.execute(query)
+                user_row = result.scalar()
+                max_vfolder_size = user_row.resource_policy_row.max_vfolder_size
             case _:
                 raise GroupNotFound(extra_data=group_id_or_name)
 
         # Check if group exists when it's given a non-empty value.
         if group_id_or_name and group_uuid is None:
             raise GroupNotFound(extra_data=group_id_or_name)
 
         # Determine the ownership type and the quota scope ID.
         if group_uuid is not None:
             ownership_type = "group"
-            quota_scope_id = group_uuid.hex
+            quota_scope_id = QuotaScopeID(QuotaScopeType.PROJECT, group_uuid)
             if not request["is_admin"]:
                 raise GenericForbidden("no permission")
         else:
             ownership_type = "user"
-            quota_scope_id = user_uuid.hex
+            quota_scope_id = QuotaScopeID(QuotaScopeType.USER, user_uuid)
         if ownership_type not in allowed_vfolder_types:
             raise InvalidAPIParameters(
                 f"{ownership_type}-owned vfolder is not allowed in this cluster"
             )
 
+    async with root_ctx.db.begin() as conn:
         if not unmanaged_path:
             await ensure_host_permission_allowed(
                 conn,
                 folder_host,
                 allowed_vfolder_types=allowed_vfolder_types,
                 user_uuid=user_uuid,
-                resource_policy=resource_policy,
+                resource_policy=keypair_resource_policy,
                 domain_name=domain_name,
                 group_id=group_uuid,
                 permission=VFolderHostPermission.CREATE,
             )
 
         # Check resource policy's max_vfolder_count
-        if resource_policy["max_vfolder_count"] > 0:
+        if keypair_resource_policy["max_vfolder_count"] > 0:
             query = sa.select([sa.func.count()]).where(vfolders.c.user == user_uuid)
             result = await conn.scalar(query)
-            if result >= resource_policy["max_vfolder_count"]:
+            if result >= keypair_resource_policy["max_vfolder_count"]:
                 raise InvalidAPIParameters("You cannot create more vfolders.")
 
         # DEPRECATED: Limit vfolder size quota if it is larger than max_vfolder_size of the resource policy.
         # max_vfolder_size = resource_policy.get("max_vfolder_size", 0)
         # if max_vfolder_size > 0 and (
         #     params["quota"] is None or params["quota"] <= 0 or params["quota"] > max_vfolder_size
         # ):
@@ -475,32 +499,37 @@
                 #     json={
                 #         "volume": root_ctx.storage_manager.split_host(folder_host)[1],
                 #         "qsid": str(quota_scope_id),
                 #         "options": None,
                 #     },
                 # ):
                 #     pass
+                options = {}
+                if max_vfolder_size and max_vfolder_size > 0:
+                    options["initial_max_size_for_quota_scope"] = max_vfolder_size
                 async with root_ctx.storage_manager.request(
                     folder_host,
                     "POST",
                     "folder/create",
                     json={
                         "volume": root_ctx.storage_manager.split_host(folder_host)[1],
                         "vfid": str(vfid),
+                        "options": options,
                     },
                 ):
                     pass
-        except aiohttp.ClientResponseError:
-            raise VFolderCreationFailed
+        except aiohttp.ClientResponseError as e:
+            raise VFolderCreationFailed from e
+
         # TODO: include quota scope ID in the database
         # TODO: include quota scope ID in the API response
         insert_values = {
             "id": vfid.folder_id.hex,
             "name": params["name"],
-            "quota_scope_id": quota_scope_id,
+            "quota_scope_id": str(quota_scope_id),
             "usage_mode": params["usage_mode"],
             "permission": params["permission"],
             "last_used": None,
             "max_size": int(params["quota"] / (2**20)) if params["quota"] else None,  # in MBytes
             "host": folder_host,
             "creator": request["user"]["email"],
             "ownership_type": VFolderOwnershipType(ownership_type),
@@ -509,15 +538,15 @@
             "unmanaged_path": "",
             "cloneable": params["cloneable"],
             "status": VFolderOperationStatus.READY,
         }
         resp = {
             "id": vfid.folder_id.hex,
             "name": params["name"],
-            "quota_scope_id": quota_scope_id,
+            "quota_scope_id": str(quota_scope_id),
             "host": folder_host,
             "usage_mode": params["usage_mode"].value,
             "permission": params["permission"].value,
             "max_size": int(params["quota"] / (2**20)) if params["quota"] else None,  # in MBytes
             "creator": request["user"]["email"],
             "ownership_type": ownership_type,
             "user": str(user_uuid) if ownership_type == "user" else None,
@@ -582,15 +611,15 @@
                 extra_vf_conds=extra_vf_conds,
             )
         for entry in entries:
             resp.append(
                 {
                     "name": entry["name"],
                     "id": entry["id"].hex,
-                    "quota_scope_id": entry["quota_scope_id"],
+                    "quota_scope_id": str(entry["quota_scope_id"]),
                     "host": entry["host"],
                     "status": entry["status"],
                     "usage_mode": entry["usage_mode"].value,
                     "created_at": str(entry["created_at"]),
                     "is_owner": entry["is_owner"],
                     "permission": entry["permission"].value,
                     "user": str(entry["user"]) if entry["user"] else None,
@@ -885,23 +914,23 @@
     proxy_name, volume_name = root_ctx.storage_manager.split_host(row["host"])
     async with root_ctx.storage_manager.request(
         proxy_name,
         "GET",
         "folder/usage",
         json={
             "volume": volume_name,
-            "vfid": str(row["id"]),
+            "vfid": str(VFolderID.from_row(row)),
         },
     ) as (_, storage_resp):
         usage = await storage_resp.json()
     resp = {
         "name": row["name"],
         "id": row["id"].hex,
         "host": row["host"],
-        "quota_scope_id": row["quota_scope_id"],
+        "quota_scope_id": str(row["quota_scope_id"]),
         "status": row["status"],
         "numFiles": usage["file_count"],  # legacy
         "num_files": usage["file_count"],
         "used_bytes": usage["used_bytes"],  # added in v20.09
         "created": str(row["created_at"]),  # legacy
         "created_at": str(row["created_at"]),
         "last_used": str(row["created_at"]),
@@ -925,15 +954,15 @@
         {
             t.Key("folder_host"): t.String,
             t.Key("id"): tx.UUID,
         }
     )
 )
 async def get_quota(request: web.Request, params: Any) -> web.Response:
-    await ensure_vfolder_status(request, VFolderAccessStatus.READABLE, params["id"])
+    vfolder_row = await ensure_vfolder_status(request, VFolderAccessStatus.READABLE, params["id"])
     root_ctx: RootContext = request.app["_root.context"]
     proxy_name, volume_name = root_ctx.storage_manager.split_host(params["folder_host"])
     log.info(
         "VFOLDER.GET_QUOTA (email:{}, volume_name:{}, vf:{})",
         request["user"]["email"],
         volume_name,
         params["id"],
@@ -962,15 +991,15 @@
 
     async with root_ctx.storage_manager.request(
         proxy_name,
         "GET",
         "volume/quota",
         json={
             "volume": volume_name,
-            "vfid": str(params["id"]),
+            "vfid": str(VFolderID.from_row(vfolder_row)),
         },
     ) as (_, storage_resp):
         storage_reply = await storage_resp.json()
     return web.json_response(storage_reply, status=200)
 
 
 @auth_required
@@ -981,15 +1010,15 @@
             t.Key("folder_host"): t.String,
             t.Key("id"): tx.UUID,
             t.Key("input"): t.Mapping(t.String, t.Any),
         }
     ),
 )
 async def update_quota(request: web.Request, params: Any) -> web.Response:
-    await ensure_vfolder_status(request, VFolderAccessStatus.UPDATABLE, params["id"])
+    vfolder_row = await ensure_vfolder_status(request, VFolderAccessStatus.UPDATABLE, params["id"])
     root_ctx: RootContext = request.app["_root.context"]
     folder_host = params["folder_host"]
     proxy_name, volume_name = root_ctx.storage_manager.split_host(folder_host)
     quota = int(params["input"]["size_bytes"])
     log.info(
         "VFOLDER.UPDATE_QUOTA (email:{}, volume_name:{}, quota:{}, vf:{})",
         request["user"]["email"],
@@ -1037,15 +1066,15 @@
 
     async with root_ctx.storage_manager.request(
         proxy_name,
         "PATCH",
         "volume/quota",
         json={
             "volume": volume_name,
-            "vfid": str(params["id"]),
+            "vfid": str(VFolderID.from_row(vfolder_row)),
             "size_bytes": quota,
         },
     ):
         pass
 
     # Update the quota for the vfolder in DB.
     async with root_ctx.db.begin() as conn:
@@ -2268,15 +2297,15 @@
         )
         # Folder owner OR user who have DELETE permission can delete folder.
         if not entry["is_owner"] and entry["permission"] != VFolderPermission.RW_DELETE:
             raise InvalidAPIParameters("Cannot delete the vfolder that is not owned by myself.")
 
     await initiate_vfolder_removal(
         root_ctx.db,
-        [VFolderDeletionInfo(entry["id"], folder_host)],
+        [VFolderDeletionInfo(VFolderID.from_row(entry), folder_host)],
         root_ctx.storage_manager,
         app_ctx.storage_ptask_group,
     )
     return web.Response(status=204)
 
 
 @auth_required
```

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/api/wsproxy.py` & `backend.ai-manager-23.3.7/ai/backend/manager/api/wsproxy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/cli/__main__.py` & `backend.ai-manager-23.3.7/ai/backend/manager/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/cli/context.py` & `backend.ai-manager-23.3.7/ai/backend/manager/cli/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/cli/dbschema.py` & `backend.ai-manager-23.3.7/ai/backend/manager/cli/dbschema.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/cli/etcd.py` & `backend.ai-manager-23.3.7/ai/backend/manager/cli/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/cli/fixture.py` & `backend.ai-manager-23.3.7/ai/backend/manager/cli/fixture.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/cli/gql.py` & `backend.ai-manager-23.3.7/ai/backend/manager/cli/gql.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/cli/image.py` & `backend.ai-manager-23.3.7/ai/backend/manager/cli/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/cli/image_impl.py` & `backend.ai-manager-23.3.7/ai/backend/manager/cli/image_impl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/config.py` & `backend.ai-manager-23.3.7/ai/backend/manager/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/container_registry/__init__.py` & `backend.ai-manager-23.3.7/ai/backend/manager/container_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/container_registry/base.py` & `backend.ai-manager-23.3.7/ai/backend/manager/container_registry/base.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/container_registry/docker.py` & `backend.ai-manager-23.3.7/ai/backend/manager/container_registry/docker.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/container_registry/harbor.py` & `backend.ai-manager-23.3.7/ai/backend/manager/container_registry/harbor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/container_registry/local.py` & `backend.ai-manager-23.3.7/ai/backend/manager/container_registry/local.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/defs.py` & `backend.ai-manager-23.3.7/ai/backend/manager/defs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/exceptions.py` & `backend.ai-manager-23.3.7/ai/backend/manager/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/idle.py` & `backend.ai-manager-23.3.7/ai/backend/manager/idle.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/__init__.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/acl.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/agent.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     privileged_mutation,
     set_if_set,
     simple_db_mutate,
 )
 from .group import association_groups_users
 from .kernel import AGENT_RESOURCE_OCCUPYING_KERNEL_STATUSES, kernels
 from .keypair import keypairs
-from .minilang.ordering import QueryOrderParser
-from .minilang.queryfilter import QueryFilterParser
+from .minilang.ordering import OrderSpecItem, QueryOrderParser
+from .minilang.queryfilter import FieldSpecItem, QueryFilterParser
 from .scaling_group import query_allowed_sgroups
 from .user import UserRole, users
 
 if TYPE_CHECKING:
     from ai.backend.manager.models.gql import GraphQueryContext
 
 __all__: Sequence[str] = (
@@ -235,39 +235,39 @@
     async def resolve_local_config(self, info: graphene.ResolveInfo) -> Mapping[str, Any]:
         return {
             "agent": {
                 "auto_terminate_abusing_kernel": self.auto_terminate_abusing_kernel,
             },
         }
 
-    _queryfilter_fieldspec = {
+    _queryfilter_fieldspec: Mapping[str, FieldSpecItem] = {
         "id": ("id", None),
         "status": ("status", lambda s: AgentStatus[s]),
         "status_changed": ("status_changed", dtparse),
         "region": ("region", None),
         "scaling_group": ("scaling_group", None),
         "schedulable": ("schedulabe", None),
         "addr": ("addr", None),
         "first_contact": ("first_contat", dtparse),
         "lost_at": ("lost_at", dtparse),
         "version": ("version", None),
     }
 
-    _queryorder_colmap = {
-        "id": "id",
-        "status": "status",
-        "status_changed": "status_changed",
-        "region": "region",
-        "scaling_group": "scaling_group",
-        "schedulable": "schedulable",
-        "first_contact": "first_contact",
-        "lost_at": "lost_at",
-        "version": "version",
-        "available_slots": "available_slots",
-        "occupied_slots": "occupied_slots",
+    _queryorder_colmap: Mapping[str, OrderSpecItem] = {
+        "id": ("id", None),
+        "status": ("status", None),
+        "status_changed": ("status_changed", None),
+        "region": ("region", None),
+        "scaling_group": ("scaling_group", None),
+        "schedulable": ("schedulable", None),
+        "first_contact": ("first_contact", None),
+        "lost_at": ("lost_at", None),
+        "version": ("version", None),
+        "available_slots": ("available_slots", None),
+        "occupied_slots": ("occupied_slots", None),
     }
 
     @classmethod
     async def load_count(
         cls,
         graph_ctx: GraphQueryContext,
         *,
@@ -461,28 +461,28 @@
             scaling_group=row["scaling_group"],
             schedulable=row["schedulable"],
             available_slots=row["available_slots"].to_json(),
             occupied_slots=row["occupied_slots"].to_json(),
             architecture=row["architecture"],
         )
 
-    _queryfilter_fieldspec = {
+    _queryfilter_fieldspec: Mapping[str, FieldSpecItem] = {
         "id": ("id", None),
         "status": ("status", lambda s: AgentStatus[s]),
         "scaling_group": ("scaling_group", None),
         "schedulable": ("schedulabe", None),
     }
 
-    _queryorder_colmap = {
-        "id": "id",
-        "status": "status",
-        "scaling_group": "scaling_group",
-        "schedulable": "schedulable",
-        "available_slots": "available_slots",
-        "occupied_slots": "occupied_slots",
+    _queryorder_colmap: Mapping[str, OrderSpecItem] = {
+        "id": ("id", None),
+        "status": ("status", None),
+        "scaling_group": ("scaling_group", None),
+        "schedulable": ("schedulable", None),
+        "available_slots": ("available_slots", None),
+        "occupied_slots": ("occupied_slots", None),
     }
 
     @classmethod
     async def batch_load(
         cls,
         graph_ctx: GraphQueryContext,
         agent_ids: Sequence[AgentId],
```

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/env.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/env.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/base.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 from ai.backend.common.logging import BraceStyleAdapter
 from ai.backend.common.types import (
     AbstractPermission,
     BinarySize,
     EndpointId,
     JSONSerializableMixin,
     KernelId,
+    QuotaScopeID,
     ReadableCIDR,
     ResourceSlot,
     SessionId,
     VFolderHostPermission,
     VFolderHostPermissionMap,
 )
 from ai.backend.manager.models.utils import execute_with_retry
@@ -168,14 +169,32 @@
         return EnumValueType(self._enum_cls, **self._opts)
 
     @property
     def python_type(self):
         return self._enum_class
 
 
+class QuotaScopeIDType(TypeDecorator):
+    """
+    A column type wrapper for string-based quota scope ID.
+    """
+
+    impl = sa.String
+    cache_ok = True
+
+    def load_dialect_impl(self, dialect):
+        return dialect.type_descriptor(sa.String(64))
+
+    def process_bind_param(self, value: Optional[QuotaScopeID], dialect) -> Optional[str]:
+        return str(value) if value else None
+
+    def process_result_value(self, raw_value: str, dialect) -> QuotaScopeID:
+        return QuotaScopeID.parse(raw_value)
+
+
 class ResourceSlotColumn(TypeDecorator):
     """
     A column type wrapper for ResourceSlot from JSONB.
     """
 
     impl = JSONB
     cache_ok = True
@@ -614,48 +633,56 @@
         row: Row,
     ) -> _GenericSQLBasedGQLObject:
         ...
 
 
 async def batch_result(
     graph_ctx: GraphQueryContext,
-    db_conn: SAConnection,
+    db_conn: SAConnection | SASession,
     query: sa.sql.Select,
     obj_type: Type[_GenericSQLBasedGQLObject],
     key_list: Iterable[_Key],
     key_getter: Callable[[Row], _Key],
 ) -> Sequence[Optional[_GenericSQLBasedGQLObject]]:
     """
     A batched query adaptor for (key -> item) resolving patterns.
     """
     objs_per_key: Dict[_Key, Optional[_GenericSQLBasedGQLObject]]
     objs_per_key = collections.OrderedDict()
     for key in key_list:
         objs_per_key[key] = None
-    async for row in await db_conn.stream(query):
+    if isinstance(db_conn, SASession):
+        stream_func = db_conn.stream_scalars
+    else:
+        stream_func = db_conn.stream
+    async for row in await stream_func(query):
         objs_per_key[key_getter(row)] = obj_type.from_row(graph_ctx, row)
     return [*objs_per_key.values()]
 
 
 async def batch_multiresult(
     graph_ctx: GraphQueryContext,
-    db_conn: SAConnection,
+    db_conn: SAConnection | SASession,
     query: sa.sql.Select,
     obj_type: Type[_GenericSQLBasedGQLObject],
     key_list: Iterable[_Key],
     key_getter: Callable[[Row], _Key],
 ) -> Sequence[Sequence[_GenericSQLBasedGQLObject]]:
     """
     A batched query adaptor for (key -> [item]) resolving patterns.
     """
     objs_per_key: Dict[_Key, List[_GenericSQLBasedGQLObject]]
     objs_per_key = collections.OrderedDict()
     for key in key_list:
         objs_per_key[key] = list()
-    async for row in await db_conn.stream(query):
+    if isinstance(db_conn, SASession):
+        stream_func = db_conn.stream_scalars
+    else:
+        stream_func = db_conn.stream
+    async for row in await stream_func(query):
         objs_per_key[key_getter(row)].append(
             obj_type.from_row(graph_ctx, row),
         )
     return [*objs_per_key.values()]
 
 
 async def batch_result_in_session(
```

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/domain.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/domain.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/dotfile.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/dotfile.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/endpoint.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/error_logs.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/error_logs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/gql.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/gql.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import uuid
 from typing import TYPE_CHECKING, Any, Mapping, Optional, Sequence
 
 import attrs
 import graphene
 
+from ai.backend.common.types import QuotaScopeID
 from ai.backend.manager.defs import DEFAULT_IMAGE_ARCH
 
 if TYPE_CHECKING:
     from graphql.execution.executors.asyncio import AsyncioExecutor  # pants: no-infer-dep
 
     from ai.backend.common.bgtask import BackgroundTaskManager
     from ai.backend.common.etcd import AsyncEtcd
@@ -58,17 +59,25 @@
     ComputeContainerList,
     LegacyComputeSession,
     LegacyComputeSessionList,
 )
 from .keypair import CreateKeyPair, DeleteKeyPair, KeyPair, KeyPairList, ModifyKeyPair
 from .resource_policy import (
     CreateKeyPairResourcePolicy,
+    CreateProjectResourcePolicy,
+    CreateUserResourcePolicy,
     DeleteKeyPairResourcePolicy,
+    DeleteProjectResourcePolicy,
+    DeleteUserResourcePolicy,
     KeyPairResourcePolicy,
     ModifyKeyPairResourcePolicy,
+    ModifyProjectResourcePolicy,
+    ModifyUserResourcePolicy,
+    ProjectResourcePolicy,
+    UserResourcePolicy,
 )
 from .resource_preset import (
     CreateResourcePreset,
     DeleteResourcePreset,
     ModifyResourcePreset,
     ResourcePreset,
 )
@@ -96,18 +105,22 @@
     PurgeUser,
     User,
     UserList,
     UserRole,
     UserStatus,
 )
 from .vfolder import (
+    QuotaScope,
+    SetQuotaScope,
+    UnsetQuotaScope,
     VirtualFolder,
     VirtualFolderList,
     VirtualFolderPermission,
     VirtualFolderPermissionList,
+    ensure_quota_scope_accessible_by_user,
 )
 
 
 @attrs.define(auto_attribs=True, slots=True)
 class GraphQueryContext:
     schema: graphene.Schema
     dataloader_manager: DataLoaderManager
@@ -171,14 +184,24 @@
 
     # super-admin only
     create_keypair_resource_policy = CreateKeyPairResourcePolicy.Field()
     modify_keypair_resource_policy = ModifyKeyPairResourcePolicy.Field()
     delete_keypair_resource_policy = DeleteKeyPairResourcePolicy.Field()
 
     # super-admin only
+    create_user_resource_policy = CreateUserResourcePolicy.Field()
+    modify_user_resource_policy = ModifyUserResourcePolicy.Field()
+    delete_user_resource_policy = DeleteUserResourcePolicy.Field()
+
+    # super-admin only
+    create_project_resource_policy = CreateProjectResourcePolicy.Field()
+    modify_project_resource_policy = ModifyProjectResourcePolicy.Field()
+    delete_project_resource_policy = DeleteProjectResourcePolicy.Field()
+
+    # super-admin only
     create_resource_preset = CreateResourcePreset.Field()
     modify_resource_preset = ModifyResourcePreset.Field()
     delete_resource_preset = DeleteResourcePreset.Field()
 
     # super-admin only
     create_scaling_group = CreateScalingGroup.Field()
     modify_scaling_group = ModifyScalingGroup.Field()
@@ -188,14 +211,17 @@
     associate_scaling_group_with_keypair = AssociateScalingGroupWithKeyPair.Field()
     disassociate_scaling_group_with_domain = DisassociateScalingGroupWithDomain.Field()
     disassociate_scaling_group_with_user_group = DisassociateScalingGroupWithUserGroup.Field()
     disassociate_scaling_group_with_keypair = DisassociateScalingGroupWithKeyPair.Field()
     disassociate_all_scaling_groups_with_domain = DisassociateAllScalingGroupsWithDomain.Field()
     disassociate_all_scaling_groups_with_group = DisassociateAllScalingGroupsWithGroup.Field()
 
+    set_quota_scope = SetQuotaScope.Field()
+    unset_quota_scope = UnsetQuotaScope.Field()
+
 
 class Queries(graphene.ObjectType):
     """
     All available GraphQL queries.
     """
 
     # super-admin only
@@ -343,16 +369,26 @@
 
     # NOTE: maybe add keypairs_from_user_id?
 
     keypair_resource_policy = graphene.Field(
         KeyPairResourcePolicy,
         name=graphene.String(),
     )
+    user_resource_policy = graphene.Field(
+        UserResourcePolicy,
+        name=graphene.String(),
+    )
+    project_resource_policy = graphene.Field(
+        ProjectResourcePolicy,
+        name=graphene.String(required=True),
+    )
 
     keypair_resource_policies = graphene.List(KeyPairResourcePolicy)
+    user_resource_policies = graphene.List(UserResourcePolicy)
+    project_resource_policies = graphene.List(ProjectResourcePolicy)
 
     resource_preset = graphene.Field(
         ResourcePreset,
         name=graphene.String(),
     )
 
     resource_presets = graphene.List(
@@ -524,14 +560,20 @@
         offset=graphene.Int(required=True),
         filter=graphene.String(),
         order=graphene.String(),
         # filters
         endpoint_id=graphene.UUID(),
     )
 
+    quota_scope = graphene.Field(
+        QuotaScope,
+        storage_host_name=graphene.String(required=True),
+        quota_scope_id=graphene.String(required=True),
+    )
+
     @staticmethod
     @privileged_query(UserRole.SUPERADMIN)
     async def resolve_agent(
         executor: AsyncioExecutor,
         info: graphene.ResolveInfo,
         agent_id: AgentId,
     ) -> Agent:
@@ -1090,14 +1132,84 @@
                 info.context,
                 client_access_key,
             )
         else:
             raise InvalidAPIParameters("Unknown client role")
 
     @staticmethod
+    async def resolve_user_resource_policy(
+        executor: AsyncioExecutor,
+        info: graphene.ResolveInfo,
+        name: str = None,
+    ) -> UserResourcePolicy:
+        ctx: GraphQueryContext = info.context
+        user_uuid = ctx.user["uuid"]
+        if name is None:
+            loader = ctx.dataloader_manager.get_loader(
+                ctx,
+                "UserResourcePolicy.by_user",
+            )
+            return await loader.load(user_uuid)
+        else:
+            loader = ctx.dataloader_manager.get_loader(
+                ctx,
+                "UserResourcePolicy.by_name",
+            )
+            return await loader.load(name)
+
+    @staticmethod
+    async def resolve_user_resource_policies(
+        executor: AsyncioExecutor,
+        info: graphene.ResolveInfo,
+    ) -> Sequence[UserResourcePolicy]:
+        ctx: GraphQueryContext = info.context
+        client_role = ctx.user["role"]
+        user_uuid = ctx.user["uuid"]
+        if client_role == UserRole.SUPERADMIN:
+            return await UserResourcePolicy.load_all(info.context)
+        elif client_role == UserRole.ADMIN:
+            # TODO: filter resource policies by domains?
+            return await UserResourcePolicy.load_all(info.context)
+        elif client_role == UserRole.USER:
+            return await UserResourcePolicy.batch_load_by_user(
+                info.context,
+                [user_uuid],
+            )
+        else:
+            raise InvalidAPIParameters("Unknown client role")
+
+    @staticmethod
+    async def resolve_project_resource_policy(
+        executor: AsyncioExecutor,
+        info: graphene.ResolveInfo,
+        name: str,
+    ) -> ProjectResourcePolicy:
+        ctx: GraphQueryContext = info.context
+        loader = ctx.dataloader_manager.get_loader(
+            ctx,
+            "ProjectResourcePolicy.by_name",
+        )
+        return await loader.load(name)
+
+    @staticmethod
+    async def resolve_project_resource_policies(
+        executor: AsyncioExecutor,
+        info: graphene.ResolveInfo,
+    ) -> Sequence[ProjectResourcePolicy]:
+        ctx: GraphQueryContext = info.context
+        client_role = ctx.user["role"]
+        if client_role == UserRole.SUPERADMIN:
+            return await ProjectResourcePolicy.load_all(info.context)
+        elif client_role == UserRole.ADMIN:
+            # TODO: filter resource policies by domains?
+            return await ProjectResourcePolicy.load_all(info.context)
+        else:
+            raise InvalidAPIParameters("Unknown client role")
+
+    @staticmethod
     async def resolve_resource_preset(
         executor: AsyncioExecutor,
         info: graphene.ResolveInfo,
         name: str,
     ) -> ResourcePreset:
         ctx: GraphQueryContext = info.context
         loader = ctx.dataloader_manager.get_loader(ctx, "ResourcePreset.by_name")
@@ -1558,14 +1670,39 @@
             order=order,
             project=project,
             domain_name=domain_name,
             user_uuid=user_uuid,
         )
         return RoutingList(routing_list, total_count)
 
+    @staticmethod
+    async def resolve_quota_scope(
+        executor: AsyncioExecutor,
+        info: graphene.ResolveInfo,
+        *,
+        quota_scope_id: Optional[str] = None,
+        storage_host_name: Optional[str] = None,
+    ) -> QuotaScope:
+        if not quota_scope_id or not storage_host_name:
+            raise ValueError("Either quota_scope_id and storage_host_name has to be defined")
+        graph_ctx: GraphQueryContext = info.context
+        qsid = QuotaScopeID.parse(quota_scope_id)
+        volumes_by_host = await graph_ctx.storage_manager.get_all_volumes()
+        for host, volume in volumes_by_host:
+            if f"{host}:{volume['name']}" == storage_host_name:
+                break
+        else:
+            raise ValueError(f"storage volume {storage_host_name} does not exist")
+        async with graph_ctx.db.begin_readonly_session() as sess:
+            await ensure_quota_scope_accessible_by_user(sess, qsid, graph_ctx.user)
+            return QuotaScope(
+                quota_scope_id=quota_scope_id,
+                storage_host_name=storage_host_name,
+            )
+
 
 class GQLMutationPrivilegeCheckMiddleware:
     def resolve(self, next, root, info: graphene.ResolveInfo, **args) -> Any:
         graph_ctx: GraphQueryContext = info.context
         if info.operation.operation == "mutation" and len(info.path) == 1:
             mutation_cls = getattr(Mutations, info.field_name).type
             # default is allow nobody.
```

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/group.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/group.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from graphene.types.datetime import DateTime as GQLDateTime
 from sqlalchemy.engine.row import Row
 from sqlalchemy.ext.asyncio import AsyncConnection as SAConnection
 from sqlalchemy.orm import relationship
 
 from ai.backend.common import msgpack
 from ai.backend.common.logging import BraceStyleAdapter
-from ai.backend.common.types import ResourceSlot
+from ai.backend.common.types import ResourceSlot, VFolderID
 
 from ..api.exceptions import VFolderOperationFailed
 from ..defs import RESERVED_DOTFILES
 from .base import (
     GUID,
     Base,
     IDColumn,
@@ -135,25 +135,32 @@
         default={},
     ),
     sa.UniqueConstraint("name", "domain_name", name="uq_groups_name_domain_name"),
     # dotfiles column, \x90 means empty list in msgpack
     sa.Column(
         "dotfiles", sa.LargeBinary(length=MAXIMUM_DOTFILE_SIZE), nullable=False, default=b"\x90"
     ),
+    sa.Column(
+        "resource_policy",
+        sa.String(length=256),
+        sa.ForeignKey("project_resource_policies.name"),
+        nullable=False,
+    ),
 )
 
 
 class GroupRow(Base):
     __table__ = groups
     sessions = relationship("SessionRow", back_populates="group")
     domain = relationship("DomainRow", back_populates="groups")
     scaling_groups = relationship(
         "ScalingGroupRow", secondary="sgroups_for_groups", back_populates="groups"
     )
     users = relationship("AssocGroupUserRow", back_populates="group")
+    resource_policy_row = relationship("ProjectResourcePolicyRow", back_populates="projects")
 
 
 def _build_group_query(cond: sa.sql.BinaryExpression, domain_name: str) -> sa.sql.Select:
     query = (
         sa.select([groups.c.id])
         .select_from(groups)
         .where(
@@ -226,14 +233,15 @@
     is_active = graphene.Boolean()
     created_at = GQLDateTime()
     modified_at = GQLDateTime()
     domain_name = graphene.String()
     total_resource_slots = graphene.JSONString()
     allowed_vfolder_hosts = graphene.JSONString()
     integration_id = graphene.String()
+    resource_policy = graphene.String()
 
     scaling_groups = graphene.List(lambda: graphene.String)
 
     @classmethod
     def from_row(cls, graph_ctx: GraphQueryContext, row: Row) -> Optional[Group]:
         if row is None:
             return None
@@ -244,14 +252,15 @@
             is_active=row["is_active"],
             created_at=row["created_at"],
             modified_at=row["modified_at"],
             domain_name=row["domain_name"],
             total_resource_slots=row["total_resource_slots"].to_json(),
             allowed_vfolder_hosts=row["allowed_vfolder_hosts"].to_json(),
             integration_id=row["integration_id"],
+            resource_policy=row["resource_policy"],
         )
 
     async def resolve_scaling_groups(self, info: graphene.ResolveInfo) -> Sequence[ScalingGroup]:
         graph_ctx: GraphQueryContext = info.context
         loader = graph_ctx.dataloader_manager.get_loader(
             graph_ctx,
             "ScalingGroup.by_group",
@@ -372,26 +381,28 @@
 class GroupInput(graphene.InputObjectType):
     description = graphene.String(required=False)
     is_active = graphene.Boolean(required=False, default=True)
     domain_name = graphene.String(required=True)
     total_resource_slots = graphene.JSONString(required=False)
     allowed_vfolder_hosts = graphene.JSONString(required=False)
     integration_id = graphene.String(required=False)
+    resource_policy = graphene.String(required=False, default="default")
 
 
 class ModifyGroupInput(graphene.InputObjectType):
     name = graphene.String(required=False)
     description = graphene.String(required=False)
     is_active = graphene.Boolean(required=False)
     domain_name = graphene.String(required=False)
     total_resource_slots = graphene.JSONString(required=False)
     user_update_mode = graphene.String(required=False)
     user_uuids = graphene.List(lambda: graphene.String, required=False)
     allowed_vfolder_hosts = graphene.JSONString(required=False)
     integration_id = graphene.String(required=False)
+    resource_policy = graphene.String(required=False)
 
 
 class CreateGroup(graphene.Mutation):
     allowed_roles = (UserRole.ADMIN, UserRole.SUPERADMIN)
 
     class Arguments:
         name = graphene.String(required=True)
@@ -420,14 +431,15 @@
             "name": name,
             "description": props.description,
             "is_active": props.is_active,
             "domain_name": props.domain_name,
             "total_resource_slots": ResourceSlot.from_user_input(props.total_resource_slots, None),
             "allowed_vfolder_hosts": props.allowed_vfolder_hosts,
             "integration_id": props.integration_id,
+            "resource_policy": props.resource_policy or "default",
         }
         insert_query = sa.insert(groups).values(data)
         return await simple_db_mutate_returning_item(cls, graph_ctx, insert_query, item_cls=Group)
 
 
 class ModifyGroup(graphene.Mutation):
     allowed_roles = (UserRole.ADMIN, UserRole.SUPERADMIN)
@@ -462,14 +474,15 @@
             props,
             data,
             "total_resource_slots",
             clean_func=lambda v: ResourceSlot.from_user_input(v, None),
         )
         set_if_set(props, data, "allowed_vfolder_hosts")
         set_if_set(props, data, "integration_id")
+        set_if_set(props, data, "resource_policy")
 
         if "name" in data and _rx_slug.search(data["name"]) is None:
             raise ValueError("invalid name format. slug format required.")
         if props.user_update_mode not in (None, "add", "remove"):
             raise ValueError("invalid user_update_mode")
         if not props.user_uuids:
             props.user_update_mode = None
@@ -616,15 +629,15 @@
             delete_query = sa.delete(vfolders).where(vfolders.c.group == group_id)
             result = await db_conn.execute(delete_query)
 
         storage_ptask_group = aiotools.PersistentTaskGroup()
         try:
             deleted_count = await initiate_vfolder_removal(
                 engine,
-                [VFolderDeletionInfo(vf["id"], vf["host"]) for vf in target_vfs],
+                [VFolderDeletionInfo(VFolderID.from_row(vf), vf["host"]) for vf in target_vfs],
                 storage_manager,
                 storage_ptask_group,
             )
         except VFolderOperationFailed as e:
             log.error("error on deleting vfolder filesystem directory: {0}", e.extra_msg)
             raise
         if deleted_count > 0:
```

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/image.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/kernel.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/kernel.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,16 @@
     StructuredJSONObjectListColumn,
     URLColumn,
     batch_multiresult,
     batch_result,
     mapper_registry,
 )
 from .group import groups
-from .minilang.ordering import QueryOrderParser
-from .minilang.queryfilter import QueryFilterParser
+from .minilang.ordering import OrderSpecItem, QueryOrderParser
+from .minilang.queryfilter import FieldSpecItem, QueryFilterParser
 from .user import users
 from .utils import ExtendedAsyncSAEngine, execute_with_retry, sql_json_merge
 
 if TYPE_CHECKING:
     from .gql import GraphQueryContext
 
 __all__ = (
@@ -864,15 +864,15 @@
         access_key: AccessKey | None,
     ) -> Optional[Mapping[str, Any]]:
         graph_ctx: GraphQueryContext = info.context
         if access_key is None:
             return None
         return await graph_ctx.registry.get_abusing_report(self.id)
 
-    _queryfilter_fieldspec = {
+    _queryfilter_fieldspec: Mapping[str, FieldSpecItem] = {
         "image": ("image", None),
         "architecture": ("architecture", None),
         "agent": ("agent", None),
         "agent_addr": ("agent_addr", None),
         "cluster_idx": ("cluster_idx", None),
         "local_rank": ("local_rank", None),
         "cluster_role": ("cluster_role", None),
@@ -880,28 +880,28 @@
         "status": ("status", lambda s: KernelStatus[s]),
         "status_info": ("status_info", None),
         "created_at": ("created_at", dtparse),
         "status_changed": ("status_changed", dtparse),
         "terminated_at": ("terminated_at", dtparse),
     }
 
-    _queryorder_colmap = {
-        "image": "image",
-        "architecture": "architecture",
-        "agent": "agent",
-        "agent_addr": "agent_addr",
-        "cluster_idx": "cluster_idx",
-        "local_rank": "local_rank",
-        "cluster_role": "cluster_role",
-        "cluster_hostname": "cluster_hostname",
-        "status": "status",
-        "status_info": "status_info",
-        "status_changed": "status_info",
-        "created_at": "created_at",
-        "terminated_at": "terminated_at",
+    _queryorder_colmap: Mapping[str, OrderSpecItem] = {
+        "image": ("image", None),
+        "architecture": ("architecture", None),
+        "agent": ("agent", None),
+        "agent_addr": ("agent_addr", None),
+        "cluster_idx": ("cluster_idx", None),
+        "local_rank": ("local_rank", None),
+        "cluster_role": ("cluster_role", None),
+        "cluster_hostname": ("cluster_hostname", None),
+        "status": ("status", None),
+        "status_info": ("status_info", None),
+        "status_changed": ("status_info", None),
+        "created_at": ("created_at", None),
+        "terminated_at": ("terminated_at", None),
     }
 
     @classmethod
     async def load_count(
         cls,
         ctx: GraphQueryContext,
         session_id: SessionId,
```

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/keypair.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/keypair.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import base64
 import secrets
 import uuid
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, Tuple, TypedDict
+from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Optional, Sequence, Tuple, TypedDict
 
 import graphene
 import sqlalchemy as sa
 from cryptography.hazmat.backends import default_backend as crypto_default_backend
 from cryptography.hazmat.primitives import serialization as crypto_serialization
 from cryptography.hazmat.primitives.asymmetric import rsa
 from dateutil.parser import parse as dtparse
@@ -33,17 +33,18 @@
     batch_multiresult,
     batch_result,
     mapper_registry,
     set_if_set,
     simple_db_mutate,
     simple_db_mutate_returning_item,
 )
-from .minilang.ordering import QueryOrderParser
-from .minilang.queryfilter import QueryFilterParser
+from .minilang.ordering import OrderSpecItem, QueryOrderParser
+from .minilang.queryfilter import FieldSpecItem, QueryFilterParser
 from .user import ModifyUserInput, UserRole
+from .utils import agg_to_array
 
 __all__: Sequence[str] = (
     "keypairs",
     "KeyPairRow",
     "KeyPair",
     "KeyPairList",
     "UserInfo",
@@ -160,14 +161,15 @@
     is_admin = graphene.Boolean()
     resource_policy = graphene.String()
     created_at = GQLDateTime()
     last_used = GQLDateTime()
     rate_limit = graphene.Int()
     num_queries = graphene.Int()
     user = graphene.UUID()
+    projects = graphene.List(lambda: graphene.String)
 
     ssh_public_key = graphene.String()
 
     vfolders = graphene.List("ai.backend.manager.models.VirtualFolder")
     compute_sessions = graphene.List(
         "ai.backend.manager.models.ComputeSession",
         status=graphene.String(),
@@ -208,14 +210,15 @@
             resource_policy=row["resource_policy"],
             created_at=row["created_at"],
             last_used=row["last_used"],
             rate_limit=row["rate_limit"],
             user=row["user"],
             ssh_public_key=row["ssh_public_key"],
             concurrency_limit=0,  # deprecated
+            projects=row["groups_name"],
         )
 
     async def resolve_num_queries(self, info: graphene.ResolveInfo) -> int:
         ctx: GraphQueryContext = info.context
         n = await redis_helper.execute(
             ctx.redis_stat, lambda r: r.get(f"kp:{self.access_key}:num_queries")
         )
@@ -274,55 +277,62 @@
         async with graph_ctx.db.begin_readonly() as conn:
             return [
                 obj
                 async for row in (await conn.stream(query))
                 if (obj := cls.from_row(graph_ctx, row)) is not None
             ]
 
-    _queryfilter_fieldspec = {
+    _queryfilter_fieldspec: Mapping[str, FieldSpecItem] = {
         "access_key": ("keypairs_access_key", None),
         "user_id": ("users_uuid", None),
         "email": ("users_email", None),
         "full_name": ("users_full_name", None),
         "is_active": ("keypairs_is_active", None),
         "is_admin": ("keypairs_is_admin", None),
         "resource_policy": ("keypairs_resource_policy", None),
         "created_at": ("keypairs_created_at", dtparse),
         "last_used": ("keypairs_last_used", dtparse),
         "rate_limit": ("keypairs_rate_limit", None),
         "num_queries": ("keypairs_num_queries", None),
         "ssh_public_key": ("keypairs_ssh_public_key", None),
+        "projects": ("groups_name", None),
     }
 
-    _queryorder_colmap = {
-        "access_key": "keypairs_access_key",
-        "email": "users_email",
-        "full_name": "users_full_name",
-        "is_active": "keypairs_is_active",
-        "is_admin": "keypairs_is_admin",
-        "resource_policy": "keypairs_resource_policy",
-        "created_at": "keypairs_created_at",
-        "last_used": "keypairs_last_used",
-        "rate_limit": "keypairs_rate_limit",
-        "num_queries": "keypairs_num_queries",
+    _queryorder_colmap: Mapping[str, OrderSpecItem] = {
+        "access_key": ("keypairs_access_key", None),
+        "email": ("users_email", None),
+        "full_name": ("users_full_name", None),
+        "is_active": ("keypairs_is_active", None),
+        "is_admin": ("keypairs_is_admin", None),
+        "resource_policy": ("keypairs_resource_policy", None),
+        "created_at": ("keypairs_created_at", None),
+        "last_used": ("keypairs_last_used", None),
+        "rate_limit": ("keypairs_rate_limit", None),
+        "num_queries": ("keypairs_num_queries", None),
+        "projects": ("groups_name", agg_to_array),
     }
 
     @classmethod
     async def load_count(
         cls,
         graph_ctx: GraphQueryContext,
         *,
         domain_name: str = None,
         email: str = None,
         is_active: bool = None,
         filter: str = None,
     ) -> int:
+        from .group import association_groups_users, groups
         from .user import users
 
-        j = sa.join(keypairs, users, keypairs.c.user == users.c.uuid)
+        j = (
+            sa.join(keypairs, users, keypairs.c.user == users.c.uuid)
+            .join(association_groups_users, users.c.uuid == association_groups_users.c.user_id)
+            .join(groups, association_groups_users.c.group_id == groups.c.id)
+        )
         query = sa.select([sa.func.count()]).select_from(j)
         if domain_name is not None:
             query = query.where(users.c.domain_name == domain_name)
         if email is not None:
             query = query.where(keypairs.c.user_id == email)
         if is_active is not None:
             query = query.where(keypairs.c.is_active == is_active)
@@ -342,20 +352,33 @@
         *,
         domain_name: str = None,
         email: str = None,
         is_active: bool = None,
         filter: str = None,
         order: str = None,
     ) -> Sequence[KeyPair]:
+        from .group import association_groups_users, groups
         from .user import users
 
-        j = sa.join(keypairs, users, keypairs.c.user == users.c.uuid)
+        j = (
+            sa.join(keypairs, users, keypairs.c.user == users.c.uuid)
+            .join(association_groups_users, users.c.uuid == association_groups_users.c.user_id)
+            .join(groups, association_groups_users.c.group_id == groups.c.id)
+        )
         query = (
-            sa.select([keypairs, users.c.email, users.c.full_name])
+            sa.select(
+                [
+                    keypairs,
+                    users.c.email,
+                    users.c.full_name,
+                    agg_to_array(groups.c.name).label("groups_name"),
+                ]
+            )
             .select_from(j)
+            .group_by(keypairs, users.c.email, users.c.full_name)
             .limit(limit)
             .offset(offset)
         )
         if domain_name is not None:
             query = query.where(users.c.domain_name == domain_name)
         if email is not None:
             query = query.where(keypairs.c.user_id == email)
@@ -381,22 +404,35 @@
         cls,
         graph_ctx: GraphQueryContext,
         user_ids: Sequence[uuid.UUID],
         *,
         domain_name: str = None,
         is_active: bool = None,
     ) -> Sequence[Sequence[Optional[KeyPair]]]:
+        from .group import association_groups_users, groups
         from .user import users
 
-        j = sa.join(
-            keypairs,
-            users,
-            keypairs.c.user == users.c.uuid,
+        j = (
+            sa.join(keypairs, users, keypairs.c.user == users.c.uuid)
+            .join(association_groups_users, users.c.uuid == association_groups_users.c.user_id)
+            .join(groups, association_groups_users.c.group_id == groups.c.id)
+        )
+        query = (
+            sa.select(
+                [
+                    keypairs,
+                    users.c.email,
+                    users.c.full_name,
+                    agg_to_array(groups.c.name).label("groups_name"),
+                ]
+            )
+            .select_from(j)
+            .where(keypairs.c.user_id.in_(user_ids))
+            .group_by(keypairs, users.c.email, users.c.full_name)
         )
-        query = sa.select([keypairs]).select_from(j).where(keypairs.c.user_id.in_(user_ids))
         if domain_name is not None:
             query = query.where(users.c.domain_name == domain_name)
         if is_active is not None:
             query = query.where(keypairs.c.is_active == is_active)
         async with graph_ctx.db.begin_readonly() as conn:
             return await batch_multiresult(
                 graph_ctx,
@@ -411,22 +447,35 @@
     async def batch_load_by_ak(
         cls,
         graph_ctx: GraphQueryContext,
         access_keys: Sequence[AccessKey],
         *,
         domain_name: str = None,
     ) -> Sequence[Optional[KeyPair]]:
+        from .group import association_groups_users, groups
         from .user import users
 
-        j = sa.join(
-            keypairs,
-            users,
-            keypairs.c.user == users.c.uuid,
+        j = (
+            sa.join(keypairs, users, keypairs.c.user == users.c.uuid)
+            .join(association_groups_users, users.c.uuid == association_groups_users.c.user_id)
+            .join(groups, association_groups_users.c.group_id == groups.c.id)
+        )
+        query = (
+            sa.select(
+                [
+                    keypairs,
+                    users.c.email,
+                    users.c.full_name,
+                    agg_to_array(groups.c.name).label("groups_name"),
+                ]
+            )
+            .select_from(j)
+            .where(keypairs.c.access_key.in_(access_keys))
+            .group_by(keypairs, users.c.email, users.c.full_name)
         )
-        query = sa.select([keypairs]).select_from(j).where(keypairs.c.access_key.in_(access_keys))
         if domain_name is not None:
             query = query.where(users.c.domain_name == domain_name)
         async with graph_ctx.db.begin_readonly() as conn:
             return await batch_result(
                 graph_ctx,
                 conn,
                 query,
```

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/minilang/ordering.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/minilang/ordering.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,19 @@
-from typing import Mapping
+from typing import Any, Callable, Mapping, Optional
 
 import sqlalchemy as sa
 from lark import Lark, LarkError, Transformer
+from lark.lexer import Token
 
-__all__ = ("QueryOrderParser",)
+__all__ = (
+    "QueryOrderParser",
+    "OrderSpecItem",
+)
+
+OrderSpecItem = tuple[str, Optional[Callable[[sa.Column], Any]]]
 
 _grammar = r"""
     ?start: expr
     expr   : [col ("," col)*]
     col    : ORDER? CNAME
     ORDER  : "+" | "-"
     %import common.CNAME
@@ -18,31 +24,37 @@
     _grammar,
     parser="lalr",
     maybe_placeholders=False,
 )
 
 
 class QueryOrderTransformer(Transformer):
-    def __init__(self, sa_table: sa.Table, column_map: Mapping[str, str] = None) -> None:
+    def __init__(
+        self, sa_table: sa.Table, column_map: Optional[Mapping[str, OrderSpecItem]] = None
+    ) -> None:
         super().__init__()
         self._sa_table = sa_table
         self._column_map = column_map
 
     def _get_col(self, col_name: str) -> sa.Column:
         try:
             if self._column_map:
-                col = self._sa_table.c[self._column_map[col_name]]
+                col_value, func = self._column_map[col_name]
+                if func is not None:
+                    col = func(self._sa_table.c[col_value])
+                else:
+                    col = self._sa_table.c[col_value]
             else:
                 col = self._sa_table.c[col_name]
             return col
         except KeyError:
             raise ValueError("Unknown/unsupported field name", col_name)
 
-    def col(self, *args):
-        children = args[0]
+    def col(self, *args) -> sa.sql.elements.UnaryExpression:
+        children: list[Token] = args[0]
         if len(children) == 2:
             op = children[0].value
             col = self._get_col(children[1].value)
         else:
             op = "+"  # assume ascending if not marked
             col = self._get_col(children[0].value)
         if op == "+":
@@ -50,15 +62,15 @@
         elif op == "-":
             return col.desc()
 
     expr = tuple
 
 
 class QueryOrderParser:
-    def __init__(self, column_map: Mapping[str, str] = None) -> None:
+    def __init__(self, column_map: Optional[Mapping[str, OrderSpecItem]] = None) -> None:
         self._column_map = column_map
         self._parser = _parser
 
     def append_ordering(
         self,
         sa_query: sa.sql.Select,
         order_expr: str,
```

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/minilang/queryfilter.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/minilang/queryfilter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from typing import Any, Mapping, Union
+from typing import Any, Callable, Mapping, Optional, Tuple, Type, Union
 
 import sqlalchemy as sa
 from lark import Lark, LarkError, Transformer, Tree
-
-from . import FieldSpecItem
+from lark.lexer import Token
 
 __all__ = (
     "FilterableSQLQuery",
     "QueryFilterParser",
+    "FieldSpecItem",
 )
 
+FieldSpecItem = Tuple[str, Optional[Callable[[str], Any]]]
 
 FilterableSQLQuery = Union[sa.sql.Select, sa.sql.Update, sa.sql.Delete]
 
 _grammar = r"""
     ?start: expr
     value: string
            | number
@@ -45,40 +46,43 @@
     _grammar,
     parser="lalr",
     maybe_placeholders=False,
 )
 
 
 class QueryFilterTransformer(Transformer):
-    def __init__(self, sa_table: sa.Table, fieldspec: Mapping[str, FieldSpecItem] = None) -> None:
+    def __init__(
+        self, sa_table: sa.Table, fieldspec: Optional[Mapping[str, FieldSpecItem]] = None
+    ) -> None:
         super().__init__()
         self._sa_table = sa_table
         self._fieldspec = fieldspec
 
-    def string(self, s):
-        (s,) = s
+    def string(self, token: list[Token]) -> str:
+        s = token[0]
         # SQL-side escaping is handled by SQLAlchemy
         return s[1:-1].replace('\\"', '"')
 
-    def number(self, n):
-        (n,) = n
+    def number(self, token: list[Token]) -> int | float:
+        n = token[0]
         if "." in n:
             return float(n)
         return int(n)
 
     array = list
 
-    def atom(self, a):
-        (a,) = a
+    def atom(self, token: list[Token]) -> Type[sa.sql.elements.SingletonConstant]:
+        a = token[0]
         if a.value == "null":
             return sa.null()
         elif a.value == "true":
             return sa.true()
         elif a.value == "false":
             return sa.false()
+        raise ValueError("Unknown/unsupported atomic token", a.value)
 
     def _get_col(self, col_name: str) -> sa.Column:
         try:
             if self._fieldspec:
                 col = self._sa_table.c[self._fieldspec[col_name][0]]
             else:
                 col = self._sa_table.c[col_name]
@@ -101,16 +105,16 @@
             val = self._transform_val(col_name, value.children[0])
         elif isinstance(value, list):
             val = [self._transform_val(col_name, v) for v in value]
         else:
             val = self._transform_val_leaf(col_name, value)
         return val
 
-    def binary_expr(self, *args):
-        children = args[0]
+    def binary_expr(self, *args) -> sa.sql.elements.BinaryExpression:
+        children: list[Token] = args[0]
         col = self._get_col(children[0].value)
         op = children[1].value
         val = self._transform_val(children[0].value, children[2])
         if op == "==":
             return col == val
         elif op == "!=":
             return col != val
@@ -157,15 +161,15 @@
 
     def paren_expr(self, *args):
         children = args[0]
         return children[0]
 
 
 class QueryFilterParser:
-    def __init__(self, fieldspec: Mapping[str, FieldSpecItem] = None) -> None:
+    def __init__(self, fieldspec: Optional[Mapping[str, FieldSpecItem]] = None) -> None:
         self._fieldspec = fieldspec
         self._parser = _parser
 
     def append_filter(
         self,
         sa_query: FilterableSQLQuery,
         filter_expr: str,
```

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/resource_preset.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/resource_preset.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/routing.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/routing.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/scaling_group.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/session.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,16 @@
     StructuredJSONObjectListColumn,
     URLColumn,
     batch_multiresult_in_session,
     batch_result_in_session,
 )
 from .group import GroupRow
 from .kernel import ComputeContainer, KernelRow, KernelStatus
-from .minilang.ordering import QueryOrderParser
-from .minilang.queryfilter import QueryFilterParser
+from .minilang.ordering import OrderSpecItem, QueryOrderParser
+from .minilang.queryfilter import FieldSpecItem, QueryFilterParser
 from .user import UserRow
 from .utils import ExtendedAsyncSAEngine, execute_with_retry, sql_json_merge
 
 if TYPE_CHECKING:
     from sqlalchemy.engine import Row
 
     from .gql import GraphQueryContext
@@ -695,14 +695,16 @@
             raise MainKernelNotFound(
                 f"Session (id: {self.id}) has no main kernel.",
             )
         return kerns[0]
 
     @property
     def status_changed(self) -> Optional[datetime]:
+        if self.status_history is None:
+            return None
         try:
             return datetime.fromisoformat(self.status_history[self.status.name])
         except KeyError:
             return None
 
     @property
     def resource_opts(self) -> dict[str, Any]:
@@ -1409,15 +1411,15 @@
         self.containers = containers
         return [(await con.resolve_abusing_report(info, self.access_key)) for con in containers]
 
     async def resolve_idle_checks(self, info: graphene.ResolveInfo) -> Mapping[str, Any]:
         graph_ctx: GraphQueryContext = info.context
         return await graph_ctx.idle_checker_host.get_idle_check_report(self.session_id)
 
-    _queryfilter_fieldspec = {
+    _queryfilter_fieldspec: Mapping[str, FieldSpecItem] = {
         "id": ("sessions_id", None),
         "type": ("sessions_session_type", lambda s: SessionTypes[s]),
         "name": ("sessions_name", None),
         "domain_name": ("sessions_domain_name", None),
         "group_name": ("groups_name", None),
         "user_email": ("users_email", None),
         "full_name": ("users_full_name", None),
@@ -1430,35 +1432,35 @@
         "result": ("sessions_result", lambda s: SessionResult[s]),
         "created_at": ("sessions_created_at", dtparse),
         "terminated_at": ("sessions_terminated_at", dtparse),
         "starts_at": ("sessions_starts_at", dtparse),
         "startup_command": ("sessions_startup_command", None),
     }
 
-    _queryorder_colmap = {
-        "id": "sessions_id",
-        "type": "sessions_session_type",
-        "name": "sessions_name",
+    _queryorder_colmap: Mapping[str, OrderSpecItem] = {
+        "id": ("sessions_id", None),
+        "type": ("sessions_session_type", None),
+        "name": ("sessions_name", None),
         # "image": "image",
         # "architecture": "architecture",
-        "domain_name": "sessions_domain_name",
-        "group_name": "groups_name",
-        "user_email": "users_email",
-        "full_name": "users_full_name",
-        "access_key": "sessions_access_key",
-        "scaling_group": "sessions_scaling_group_name",
-        "cluster_mode": "sessions_cluster_mode",
+        "domain_name": ("sessions_domain_name", None),
+        "group_name": ("groups_name", None),
+        "user_email": ("users_email", None),
+        "full_name": ("users_full_name", None),
+        "access_key": ("sessions_access_key", None),
+        "scaling_group": ("sessions_scaling_group_name", None),
+        "cluster_mode": ("sessions_cluster_mode", None),
         # "cluster_template": "cluster_template",
-        "cluster_size": "sessions_cluster_size",
-        "status": "sessions_status",
-        "status_info": "sessions_status_info",
-        "result": "sessions_result",
-        "created_at": "sessions_created_at",
-        "terminated_at": "sessions_terminated_at",
-        "starts_at": "sessions_starts_at",
+        "cluster_size": ("sessions_cluster_size", None),
+        "status": ("sessions_status", None),
+        "status_info": ("sessions_status_info", None),
+        "result": ("sessions_result", None),
+        "created_at": ("sessions_created_at", None),
+        "terminated_at": ("sessions_terminated_at", None),
+        "starts_at": ("sessions_starts_at", None),
     }
 
     @classmethod
     async def load_count(
         cls,
         ctx: GraphQueryContext,
         *,
```

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/session_template.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/storage.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/user.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import enum
 import logging
-from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Sequence
+from typing import TYPE_CHECKING, Any, Dict, Iterable, Mapping, Optional, Sequence
 from uuid import UUID, uuid4
 
 import aiotools
 import graphene
 import sqlalchemy as sa
 from dateutil.parser import parse as dtparse
 from graphene.types.datetime import DateTime as GQLDateTime
@@ -18,15 +18,15 @@
 from sqlalchemy.ext.asyncio import AsyncEngine as SAEngine
 from sqlalchemy.orm import relationship
 from sqlalchemy.sql.expression import bindparam
 from sqlalchemy.types import VARCHAR, TypeDecorator
 
 from ai.backend.common import redis_helper
 from ai.backend.common.logging import BraceStyleAdapter
-from ai.backend.common.types import RedisConnectionInfo
+from ai.backend.common.types import RedisConnectionInfo, VFolderID
 
 from ..api.exceptions import VFolderOperationFailed
 from .base import (
     Base,
     EnumValueType,
     IDColumn,
     IPColumn,
@@ -35,16 +35,16 @@
     batch_multiresult,
     batch_result,
     mapper_registry,
     set_if_set,
     simple_db_mutate,
     simple_db_mutate_returning_item,
 )
-from .minilang.ordering import QueryOrderParser
-from .minilang.queryfilter import QueryFilterParser
+from .minilang.ordering import OrderSpecItem, QueryOrderParser
+from .minilang.queryfilter import FieldSpecItem, QueryFilterParser
 from .storage import StorageSessionManager
 from .utils import ExtendedAsyncSAEngine
 
 if TYPE_CHECKING:
     from .gql import GraphQueryContext
 
 log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
@@ -134,22 +134,29 @@
     sa.Column("integration_id", sa.String(length=512)),
     sa.Column("domain_name", sa.String(length=64), sa.ForeignKey("domains.name"), index=True),
     sa.Column("role", EnumValueType(UserRole), default=UserRole.USER),
     sa.Column("allowed_client_ip", pgsql.ARRAY(IPColumn), nullable=True),
     sa.Column("totp_key", sa.String(length=32)),
     sa.Column("totp_activated", sa.Boolean, server_default=sa.false(), default=False),
     sa.Column("totp_activated_at", sa.DateTime(timezone=True), nullable=True),
+    sa.Column(
+        "resource_policy",
+        sa.String(length=256),
+        sa.ForeignKey("user_resource_policies.name"),
+        nullable=False,
+    ),
 )
 
 
 class UserRow(Base):
     __table__ = users
     sessions = relationship("SessionRow", back_populates="user")
     domain = relationship("DomainRow", back_populates="users")
     groups = relationship("AssocGroupUserRow", back_populates="user")
+    resource_policy_row = relationship("UserResourcePolicyRow", back_populates="users")
 
 
 class UserGroup(graphene.ObjectType):
     id = graphene.UUID()
     name = graphene.String()
 
     @classmethod
@@ -196,14 +203,15 @@
     is_active = graphene.Boolean()
     status = graphene.String()
     status_info = graphene.String()
     created_at = GQLDateTime()
     modified_at = GQLDateTime()
     domain_name = graphene.String()
     role = graphene.String()
+    resource_policy = graphene.String()
     allowed_client_ip = graphene.List(lambda: graphene.String)
     totp_activated = graphene.Boolean()
     totp_activated_at = GQLDateTime()
 
     groups = graphene.List(lambda: UserGroup)
 
     async def resolve_groups(
@@ -232,14 +240,15 @@
             is_active=True if row["status"] == UserStatus.ACTIVE else False,  # legacy
             status=row["status"],
             status_info=row["status_info"],
             created_at=row["created_at"],
             modified_at=row["modified_at"],
             domain_name=row["domain_name"],
             role=row["role"],
+            resource_policy=row["resource_policy"],
             allowed_client_ip=row["allowed_client_ip"],
             totp_activated=row["totp_activated"],
             totp_activated_at=row["totp_activated_at"],
         )
 
     @classmethod
     async def load_all(
@@ -272,48 +281,50 @@
             _statuses = ACTIVE_USER_STATUSES if is_active else INACTIVE_USER_STATUSES
             query = query.where(users.c.status.in_(_statuses))
         if limit is not None:
             query = query.limit(limit)
         async with ctx.db.begin_readonly() as conn:
             return [cls.from_row(ctx, row) async for row in (await conn.stream(query))]
 
-    _queryfilter_fieldspec = {
+    _queryfilter_fieldspec: Mapping[str, FieldSpecItem] = {
         "uuid": ("uuid", None),
         "username": ("username", None),
         "email": ("email", None),
         "need_password_change": ("need_password_change", None),
         "full_name": ("full_name", None),
         "description": ("description", None),
         "is_active": ("is_active", None),
         "status": ("status", lambda s: UserStatus[s]),
         "status_info": ("status_info", None),
         "created_at": ("created_at", dtparse),
         "modified_at": ("modified_at", dtparse),
         "domain_name": ("domain_name", None),
         "role": ("role", lambda s: UserRole[s]),
+        "resource_policy": ("domain_name", None),
         "allowed_client_ip": ("allowed_client_ip", None),
         "totp_activated": ("totp_activated", None),
         "totp_activated_at": ("totp_activated_at", dtparse),
     }
 
-    _queryorder_colmap = {
-        "uuid": "uuid",
-        "username": "username",
-        "email": "email",
-        "need_password_change": "need_password_change",
-        "full_name": "full_name",
-        "is_active": "is_active",
-        "status": "status",
-        "status_info": "status_info",
-        "created_at": "created_at",
-        "modified_at": "modified_at",
-        "domain_name": "domain_name",
-        "role": "role",
-        "totp_activated": "totp_activated",
-        "totp_activated_at": "totp_activated_at",
+    _queryorder_colmap: Mapping[str, OrderSpecItem] = {
+        "uuid": ("uuid", None),
+        "username": ("username", None),
+        "email": ("email", None),
+        "need_password_change": ("need_password_change", None),
+        "full_name": ("full_name", None),
+        "is_active": ("is_active", None),
+        "status": ("status", None),
+        "status_info": ("status_info", None),
+        "created_at": ("created_at", None),
+        "modified_at": ("modified_at", None),
+        "domain_name": ("domain_name", None),
+        "role": ("role", None),
+        "resource_policy": ("resource_policy", None),
+        "totp_activated": ("totp_activated", None),
+        "totp_activated_at": ("totp_activated_at", None),
     }
 
     @classmethod
     async def load_count(
         cls,
         ctx: GraphQueryContext,
         *,
@@ -390,15 +401,15 @@
                 )
             else:
                 qfparser = QueryFilterParser(cls._queryfilter_fieldspec)
             query = qfparser.append_filter(query, filter)
         if order is not None:
             if group_id is not None:
                 qoparser = QueryOrderParser(
-                    {k: "users_" + v for k, v in cls._queryorder_colmap.items()}
+                    {k: ("users_" + v[0], v[1]) for k, v in cls._queryorder_colmap.items()}
                 )
             else:
                 qoparser = QueryOrderParser(cls._queryorder_colmap)
             query = qoparser.append_ordering(query, order)
         else:
             query = query.order_by(
                 users.c.created_at.desc(),
@@ -483,14 +494,15 @@
     is_active = graphene.Boolean(required=False, default=True)
     status = graphene.String(required=False, default=UserStatus.ACTIVE)
     domain_name = graphene.String(required=True, default="default")
     role = graphene.String(required=False, default=UserRole.USER)
     group_ids = graphene.List(lambda: graphene.String, required=False)
     allowed_client_ip = graphene.List(lambda: graphene.String, required=False)
     totp_activated = graphene.Boolean(required=False, default=False)
+    resource_policy = graphene.String(required=False, default="default")
 
     # When creating, you MUST set all fields.
     # When modifying, set the field to "None" to skip setting the value.
 
 
 class ModifyUserInput(graphene.InputObjectType):
     username = graphene.String(required=False)
@@ -501,14 +513,15 @@
     is_active = graphene.Boolean(required=False)
     status = graphene.String(required=False)
     domain_name = graphene.String(required=False)
     role = graphene.String(required=False)
     group_ids = graphene.List(lambda: graphene.String, required=False)
     allowed_client_ip = graphene.List(lambda: graphene.String, required=False)
     totp_activated = graphene.Boolean(required=False, default=False)
+    resource_policy = graphene.String(required=False)
 
 
 class PurgeUserInput(graphene.InputObjectType):
     purge_shared_vfolders = graphene.Boolean(required=False, default=False)
 
 
 class CreateUser(graphene.Mutation):
@@ -545,14 +558,15 @@
             "description": props.description,
             "status": _status,
             "status_info": "admin-requested",  # user mutation is only for admin
             "domain_name": props.domain_name,
             "role": UserRole(props.role),
             "allowed_client_ip": props.allowed_client_ip,
             "totp_activated": props.totp_activated,
+            "resource_policy": props.resource_policy or "default",
         }
         user_insert_query = sa.insert(users).values(user_data)
 
         async def _post_func(conn: SAConnection, result: Result) -> Row:
             if result.rowcount == 0:
                 return
             created_user = result.first()
@@ -633,14 +647,15 @@
         set_if_set(props, data, "full_name")
         set_if_set(props, data, "description")
         set_if_set(props, data, "status", clean_func=UserStatus)
         set_if_set(props, data, "domain_name")
         set_if_set(props, data, "role", clean_func=UserRole)
         set_if_set(props, data, "allowed_client_ip")
         set_if_set(props, data, "totp_activated")
+        set_if_set(props, data, "resource_policy")
         if not data and not props.group_ids:
             return cls(ok=False, msg="nothing to update", user=None)
         if data.get("status") is None and props.is_active is not None:
             data["status"] = UserStatus.ACTIVE if props.is_active else UserStatus.INACTIVE
 
         if data.get("password") is not None:
             data["password_changed_at"] = sa.func.now()
@@ -1001,15 +1016,15 @@
             )
             target_vfs = result.fetchall()
 
         storage_ptask_group = aiotools.PersistentTaskGroup()
         try:
             deleted_count = await initiate_vfolder_removal(
                 engine,
-                [VFolderDeletionInfo(vf["id"], vf["host"]) for vf in target_vfs],
+                [VFolderDeletionInfo(VFolderID.from_row(vf), vf["host"]) for vf in target_vfs],
                 storage_manager,
                 storage_ptask_group,
             )
         except VFolderOperationFailed as e:
             log.error("error on deleting vfolder filesystem directory: {0}", e.extra_msg)
             raise
         if deleted_count > 0:
```

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/utils.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -328,7 +328,16 @@
     Check out tests/test_image.py for more details.
     """
     return sa.Table(
         table.name,
         new_metadata,
         *[_populate_column(c) for c in table.columns],
     )
+
+
+def agg_to_str(column: sa.Column) -> sa.sql.functions.Function:
+    # https://docs.sqlalchemy.org/en/14/dialects/postgresql.html#sqlalchemy.dialects.postgresql.aggregate_order_by
+    return sa.func.string_agg(column, psql.aggregate_order_by(sa.literal_column("','"), column))
+
+
+def agg_to_array(column: sa.Column) -> sa.sql.functions.Function:
+    return sa.func.array_agg(psql.aggregate_order_by(column, column.asc()))
```

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/models/vfolder.py` & `backend.ai-manager-23.3.7/ai/backend/manager/models/vfolder.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,40 +12,46 @@
 import graphene
 import sqlalchemy as sa
 import trafaret as t
 from dateutil.parser import parse as dtparse
 from graphene.types.datetime import DateTime as GQLDateTime
 from sqlalchemy.engine.row import Row
 from sqlalchemy.ext.asyncio import AsyncConnection as SAConnection
+from sqlalchemy.ext.asyncio import AsyncSession as SASession
+from sqlalchemy.orm import selectinload
 
 from ai.backend.common.bgtask import ProgressReporter
 from ai.backend.common.logging import BraceStyleAdapter
 from ai.backend.common.types import (
+    QuotaScopeID,
+    QuotaScopeType,
     VFolderHostPermission,
     VFolderHostPermissionMap,
     VFolderID,
     VFolderMount,
     VFolderUsageMode,
 )
 
 from ..api.exceptions import InvalidAPIParameters, VFolderNotFound, VFolderOperationFailed
 from ..defs import RESERVED_VFOLDER_PATTERNS, RESERVED_VFOLDERS, VFOLDER_DSTPATHS_MAP
 from ..types import UserScope
 from .base import (
     GUID,
+    Base,
     BigInt,
     EnumValueType,
     IDColumn,
     Item,
     PaginatedList,
+    QuotaScopeIDType,
     batch_multiresult,
     metadata,
 )
-from .minilang.ordering import QueryOrderParser
-from .minilang.queryfilter import QueryFilterParser
+from .minilang.ordering import OrderSpecItem, QueryOrderParser
+from .minilang.queryfilter import FieldSpecItem, QueryFilterParser
 from .user import UserRole
 from .utils import ExtendedAsyncSAEngine, execute_with_retry
 
 if TYPE_CHECKING:
     from ..api.context import BackgroundTaskManager
     from .gql import GraphQueryContext
     from .storage import StorageSessionManager
@@ -59,14 +65,18 @@
     "VFolderInvitationState",
     "VFolderPermission",
     "VFolderPermissionValidator",
     "VFolderOperationStatus",
     "VFolderAccessStatus",
     "VFolderCloneInfo",
     "VFolderDeletionInfo",
+    "VFolderRow",
+    "QuotaScope",
+    "SetQuotaScope",
+    "UnsetQuotaScope",
     "query_accessible_vfolders",
     "initiate_vfolder_clone",
     "initiate_vfolder_removal",
     "get_allowed_vfolder_hosts_by_group",
     "get_allowed_vfolder_hosts_by_user",
     "verify_vfolder_name",
     "prepare_vfolder_mounts",
@@ -162,15 +172,15 @@
 
 vfolders = sa.Table(
     "vfolders",
     metadata,
     IDColumn("id"),
     # host will be '' if vFolder is unmanaged
     sa.Column("host", sa.String(length=128), nullable=False),
-    sa.Column("quota_scope_id", sa.String(length=64), nullable=False),
+    sa.Column("quota_scope_id", QuotaScopeIDType, nullable=False),
     sa.Column("name", sa.String(length=64), nullable=False, index=True),
     sa.Column(
         "usage_mode",
         EnumValueType(VFolderUsageMode),
         default=VFolderUsageMode.GENERAL,
         nullable=False,
     ),
@@ -270,14 +280,18 @@
         sa.ForeignKey("vfolders.id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     ),
     sa.Column("user", GUID, sa.ForeignKey("users.uuid"), nullable=False),
 )
 
 
+class VFolderRow(Base):
+    __table__ = vfolders
+
+
 def verify_vfolder_name(folder: str) -> bool:
     if folder in RESERVED_VFOLDERS:
         return False
     for pattern in RESERVED_VFOLDER_PATTERNS:
         if pattern.match(folder):
             return False
     return True
@@ -792,15 +806,15 @@
 
 async def initiate_vfolder_clone(
     db_engine: ExtendedAsyncSAEngine,
     vfolder_info: VFolderCloneInfo,
     storage_manager: StorageSessionManager,
     background_task_manager: BackgroundTaskManager,
 ) -> tuple[uuid.UUID, uuid.UUID]:
-    source_vf_cond = vfolders.c.id == vfolder_info.source_vfolder_id
+    source_vf_cond = vfolders.c.id == vfolder_info.source_vfolder_id.folder_id
 
     async def _update_status() -> None:
         async with db_engine.begin_session() as db_session:
             query = (
                 sa.update(vfolders)
                 .values(status=VFolderOperationStatus.CLONING)
                 .where(source_vf_cond)
@@ -813,15 +827,15 @@
     source_proxy, source_volume = storage_manager.split_host(vfolder_info.source_host)
 
     # Generate the ID of the destination vfolder.
     # TODO: If we refactor to use ORM, the folder ID will be created from the database by inserting
     #       the actual object (with RETURNING clause).  In that case, we need to temporarily
     #       mark the object to be "unusable-yet" until the storage proxy craetes the destination
     #       vfolder.  After done, we need to make another transaction to clear the unusable state.
-    target_folder_id = uuid.uuid4()
+    target_folder_id = VFolderID(vfolder_info.source_vfolder_id.quota_scope_id, uuid.uuid4())
 
     async def _clone(reporter: ProgressReporter) -> None:
         try:
             async with storage_manager.request(
                 target_proxy,
                 "POST",
                 "folder/create",
@@ -829,32 +843,33 @@
                     "volume": target_volume,
                     "vfid": str(target_folder_id),
                     # 'options': {'quota': params['quota']},
                 },
             ):
                 pass
         except aiohttp.ClientResponseError:
-            raise VFolderOperationFailed(extra_msg=str(target_folder_id))
+            raise VFolderOperationFailed(extra_msg=str(target_folder_id.folder_id))
 
         async def _insert_vfolder() -> None:
             async with db_engine.begin_session() as db_session:
                 insert_values = {
-                    "id": target_folder_id,
+                    "id": target_folder_id.folder_id,
                     "name": vfolder_info.target_vfolder_name,
                     "usage_mode": vfolder_info.usage_mode,
                     "permission": vfolder_info.permission,
                     "last_used": None,
                     "host": vfolder_info.target_host,
                     # TODO: add quota_scope_id
                     "creator": vfolder_info.email,
                     "ownership_type": VFolderOwnershipType("user"),
                     "user": vfolder_info.user_id,
                     "group": None,
                     "unmanaged_path": "",
                     "cloneable": vfolder_info.cloneable,
+                    "quota_scope_id": vfolder_info.source_vfolder_id.quota_scope_id,
                 }
                 insert_query = sa.insert(vfolders, insert_values)
                 try:
                     await db_session.execute(insert_query)
                 except sa.exc.DataError:
                     # TODO: pass exception info
                     raise InvalidAPIParameters
@@ -885,38 +900,37 @@
                     .where(source_vf_cond)
                 )
                 await db_session.execute(query)
 
         await execute_with_retry(_update_source_vfolder)
 
     task_id = await background_task_manager.start(_clone)
-    return task_id, target_folder_id
+    return task_id, target_folder_id.folder_id
 
 
 async def initiate_vfolder_removal(
     db_engine: ExtendedAsyncSAEngine,
     requested_vfolders: Sequence[VFolderDeletionInfo],
     storage_manager: StorageSessionManager,
     storage_ptask_group: aiotools.PersistentTaskGroup,
 ) -> int:
     vfolder_info_len = len(requested_vfolders)
-    vfolder_ids = tuple(vf_id for vf_id, _ in requested_vfolders)
+    vfolder_ids = tuple(vf_id.folder_id for vf_id, _ in requested_vfolders)
     cond = vfolders.c.id.in_(vfolder_ids)
     if vfolder_info_len == 0:
         return 0
     elif vfolder_info_len == 1:
         cond = vfolders.c.id == vfolder_ids[0]
 
-    async with db_engine.begin_session() as db_session:
-
-        async def _update_vfolder_status() -> None:
+    async def _update_vfolder_status() -> None:
+        async with db_engine.begin_session() as db_session:
             query = sa.update(vfolders).values(status=VFolderOperationStatus.DELETING).where(cond)
             await db_session.execute(query)
 
-        await execute_with_retry(_update_vfolder_status)
+    await execute_with_retry(_update_vfolder_status)
 
     async def _delete():
         for folder_id, host_name in requested_vfolders:
             proxy_name, volume_name = storage_manager.split_host(host_name)
             try:
                 async with storage_manager.request(
                     proxy_name,
@@ -927,28 +941,75 @@
                         "vfid": str(folder_id),
                     },
                 ):
                     pass
             except aiohttp.ClientResponseError:
                 raise VFolderOperationFailed(extra_msg=str(folder_id))
 
-        async with db_engine.begin_session() as db_session:
-
-            async def _delete_row() -> None:
+        async def _delete_row() -> None:
+            async with db_engine.begin_session() as db_session:
                 await db_session.execute(sa.delete(vfolders).where(cond))
 
-            await execute_with_retry(_delete_row)
+        await execute_with_retry(_delete_row)
         log.debug("Successfully removed vFolders {}", [str(x) for x in vfolder_ids])
 
     storage_ptask_group.create_task(_delete())
     log.debug("Started removing vFolders {}", [str(x) for x in vfolder_ids])
 
     return vfolder_info_len
 
 
+async def ensure_quota_scope_accessible_by_user(
+    conn: SASession,
+    quota_scope: QuotaScopeID,
+    user: Mapping[str, Any],
+) -> None:
+    from ai.backend.manager.models import GroupRow, UserRow
+    from ai.backend.manager.models import association_groups_users as agus
+
+    # Lookup user table to match if quota is scoped to the user
+    query = sa.select(UserRow).where(UserRow.uuid == quota_scope.scope_id)
+    quota_scope_user = await conn.scalar(query)
+    if quota_scope_user:
+        match user["role"]:
+            case UserRole.SUPERADMIN:
+                return
+            case UserRole.ADMIN:
+                if quota_scope_user.domain == user["domain"]:
+                    return
+            case _:
+                if quota_scope_user.uuid == user["uuid"]:
+                    return
+        raise InvalidAPIParameters
+
+    # Lookup group table to match if quota is scoped to the group
+    query = sa.select(GroupRow).where(GroupRow.id == quota_scope.scope_id)
+    quota_scope_group = await conn.scalar(query)
+    if quota_scope_group:
+        match user["role"]:
+            case UserRole.SUPERADMIN:
+                return
+            case UserRole.ADMIN:
+                if quota_scope_group.domain == user["domain"]:
+                    return
+            case _:
+                query = (
+                    sa.select([agus.c.group_id])
+                    .select_from(agus)
+                    .where(
+                        (agus.c.group_id == quota_scope.scope_id) & (agus.c.user_id == user["uuid"])
+                    )
+                )
+                matched_group_id = await conn.scalar(query)
+                if matched_group_id:
+                    return
+
+    raise InvalidAPIParameters
+
+
 class VirtualFolder(graphene.ObjectType):
     class Meta:
         interfaces = (Item,)
 
     host = graphene.String()
     quota_scope_id = graphene.String()
     name = graphene.String()
@@ -1000,15 +1061,15 @@
             cur_size=row["cur_size"],
         )
 
     async def resolve_num_files(self, info: graphene.ResolveInfo) -> int:
         # TODO: measure on-the-fly
         return 0
 
-    _queryfilter_fieldspec = {
+    _queryfilter_fieldspec: Mapping[str, FieldSpecItem] = {
         "id": ("vfolders_id", uuid.UUID),
         "host": ("vfolders_host", None),
         "quota_scope_id": ("vfolders_quota_scope_id", None),
         "name": ("vfolders_name", None),
         "group": ("vfolders_group", uuid.UUID),
         "group_name": ("groups_name", None),
         "user": ("vfolders_user", uuid.UUID),
@@ -1022,34 +1083,34 @@
         "max_size": ("vfolders_max_size", None),
         "created_at": ("vfolders_created_at", dtparse),
         "last_used": ("vfolders_last_used", dtparse),
         "cloneable": ("vfolders_cloneable", None),
         "status": ("vfolders_status", lambda s: VFolderOperationStatus[s]),
     }
 
-    _queryorder_colmap = {
-        "id": "vfolders_id",
-        "host": "vfolders_host",
-        "quota_scope_id": "vfolders_quota_scope_id",
-        "name": "vfolders_name",
-        "group": "vfolders_group",
-        "group_name": "groups_name",
-        "user": "vfolders_user",
-        "user_email": "users_email",
-        "creator": "vfolders_creator",
-        "usage_mode": "vfolders_usage_mode",
-        "permission": "vfolders_permission",
-        "ownership_type": "vfolders_ownership_type",
-        "max_files": "vfolders_max_files",
-        "max_size": "vfolders_max_size",
-        "created_at": "vfolders_created_at",
-        "last_used": "vfolders_last_used",
-        "cloneable": "vfolders_cloneable",
-        "status": "vfolders_status",
-        "cur_size": "vfolders_cur_size",
+    _queryorder_colmap: Mapping[str, OrderSpecItem] = {
+        "id": ("vfolders_id", None),
+        "host": ("vfolders_host", None),
+        "quota_scope_id": ("vfolders_quota_scope_id", None),
+        "name": ("vfolders_name", None),
+        "group": ("vfolders_group", None),
+        "group_name": ("groups_name", None),
+        "user": ("vfolders_user", None),
+        "user_email": ("users_email", None),
+        "creator": ("vfolders_creator", None),
+        "usage_mode": ("vfolders_usage_mode", None),
+        "permission": ("vfolders_permission", None),
+        "ownership_type": ("vfolders_ownership_type", None),
+        "max_files": ("vfolders_max_files", None),
+        "max_size": ("vfolders_max_size", None),
+        "created_at": ("vfolders_created_at", None),
+        "last_used": ("vfolders_last_used", None),
+        "cloneable": ("vfolders_cloneable", None),
+        "status": ("vfolders_status", None),
+        "cur_size": ("vfolders_cur_size", None),
     }
 
     @classmethod
     async def load_count(
         cls,
         graph_ctx: GraphQueryContext,
         *,
@@ -1180,28 +1241,28 @@
             permission=row["permission"],
             vfolder=row["vfolder"],
             vfolder_name=row["name"],
             user=row["user"],
             user_email=row["email"],
         )
 
-    _queryfilter_fieldspec = {
+    _queryfilter_fieldspec: Mapping[str, FieldSpecItem] = {
         "permission": ("vfolder_permissions_permission", lambda s: VFolderPermission[s]),
         "vfolder": ("vfolder_permissions_vfolder", None),
         "vfolder_name": ("vfolders_name", None),
         "user": ("vfolder_permissions_user", None),
         "user_email": ("users_email", None),
     }
 
-    _queryorder_colmap = {
-        "permission": "vfolder_permissions_permission",
-        "vfolder": "vfolder_permissions_vfolder",
-        "vfolder_name": "vfolders_name",
-        "user": "vfolder_permissions_user",
-        "user_email": "users_email",
+    _queryorder_colmap: Mapping[str, OrderSpecItem] = {
+        "permission": ("vfolder_permissions_permission", None),
+        "vfolder": ("vfolder_permissions_vfolder", None),
+        "vfolder_name": ("vfolders_name", None),
+        "user": ("vfolder_permissions_user", None),
+        "user_email": ("users_email", None),
     }
 
     @classmethod
     async def load_count(
         cls,
         graph_ctx: GraphQueryContext,
         *,
@@ -1264,7 +1325,183 @@
 
 
 class VirtualFolderPermissionList(graphene.ObjectType):
     class Meta:
         interfaces = (PaginatedList,)
 
     items = graphene.List(VirtualFolderPermission, required=True)
+
+
+class QuotaDetails(graphene.ObjectType):
+    usage_bytes = BigInt(required=False)
+    usage_count = BigInt(required=False)
+    hard_limit_bytes = BigInt(required=False)
+
+
+class QuotaScope(graphene.ObjectType):
+    class Meta:
+        interfaces = (Item,)
+
+    id = graphene.ID(required=True)
+    quota_scope_id = graphene.String(required=True)
+    storage_host_name = graphene.String(required=True)
+    details = graphene.NonNull(QuotaDetails)
+
+    @classmethod
+    def from_vfolder_row(cls, ctx: GraphQueryContext, row: VFolderRow) -> QuotaScope:
+        return QuotaScope(
+            quota_scope_id=str(row.quota_scope_id),
+            storage_host_name=row.host,
+        )
+
+    def resolve_id(self, info: graphene.ResolveInfo) -> str:
+        return f"QuotaScope:{self.storage_host_name}/{self.quota_scope_id}"
+
+    async def resolve_details(self, info: graphene.ResolveInfo) -> Optional[int]:
+        from ai.backend.manager.models import GroupRow, UserRow
+
+        graph_ctx: GraphQueryContext = info.context
+        proxy_name, volume_name = graph_ctx.storage_manager.split_host(self.storage_host_name)
+        try:
+            async with graph_ctx.storage_manager.request(
+                proxy_name,
+                "GET",
+                "quota-scope",
+                json={"volume": volume_name, "qsid": self.quota_scope_id},
+                raise_for_status=True,
+            ) as (_, storage_resp):
+                quota_config = await storage_resp.json()
+                usage_bytes = quota_config["used_bytes"]
+                if usage_bytes is not None and usage_bytes < 0:
+                    usage_bytes = None
+                return QuotaDetails(
+                    # FIXME: limit scaning this only for fast scan capable volumes
+                    usage_bytes=usage_bytes,
+                    hard_limit_bytes=quota_config["limit_bytes"] or None,
+                    usage_count=None,  # TODO: Implement
+                )
+        except aiohttp.ClientResponseError:
+            qsid = QuotaScopeID.parse(self.quota_scope_id)
+            async with graph_ctx.db.begin_readonly_session() as sess:
+                await ensure_quota_scope_accessible_by_user(sess, qsid, graph_ctx.user)
+                if qsid.scope_type == QuotaScopeType.USER:
+                    query = (
+                        sa.select(UserRow)
+                        .where(UserRow.uuid == qsid.scope_id)
+                        .options(selectinload(UserRow.resource_policy_row))
+                    )
+                else:
+                    query = (
+                        sa.select(GroupRow)
+                        .where(GroupRow.id == qsid.scope_id)
+                        .options(selectinload(GroupRow.resource_policy_row))
+                    )
+                result = await sess.scalar(query)
+                resource_policy_constraint = result.resource_policy_row.max_vfolder_size
+                if resource_policy_constraint is not None and resource_policy_constraint < 0:
+                    resource_policy_constraint = None
+
+            return QuotaDetails(
+                usage_bytes=None,
+                hard_limit_bytes=resource_policy_constraint,
+                usage_count=None,  # TODO: Implement
+            )
+
+
+class QuotaScopeInput(graphene.InputObjectType):
+    hard_limit_bytes = BigInt(required=False)
+
+
+class SetQuotaScope(graphene.Mutation):
+    allowed_roles = (
+        UserRole.SUPERADMIN,
+        UserRole.ADMIN,
+    )
+
+    class Arguments:
+        quota_scope_id = graphene.String(required=True)
+        storage_host_name = graphene.String(required=True)
+        props = QuotaScopeInput(required=True)
+
+    quota_scope = graphene.Field(lambda: QuotaScope)
+
+    @classmethod
+    async def mutate(
+        cls,
+        root,
+        info: graphene.ResolveInfo,
+        quota_scope_id: str,
+        storage_host_name: str,
+        props: QuotaScopeInput,
+    ) -> SetQuotaScope:
+        qsid = QuotaScopeID.parse(quota_scope_id)
+        graph_ctx: GraphQueryContext = info.context
+        async with graph_ctx.db.begin_readonly_session() as sess:
+            await ensure_quota_scope_accessible_by_user(sess, qsid, graph_ctx.user)
+
+        max_vfolder_size = props.hard_limit_bytes
+        proxy_name, volume_name = graph_ctx.storage_manager.split_host(storage_host_name)
+        request_body = {
+            "volume": volume_name,
+            "qsid": str(qsid),
+            "options": {"limit_bytes": max_vfolder_size},
+        }
+        async with graph_ctx.storage_manager.request(
+            proxy_name,
+            "PATCH",
+            "quota-scope",
+            json=request_body,
+            raise_for_status=True,
+        ):
+            pass
+        return cls(
+            QuotaScope(
+                quota_scope_id=quota_scope_id,
+                storage_host_name=storage_host_name,
+            )
+        )
+
+
+class UnsetQuotaScope(graphene.Mutation):
+    allowed_roles = (
+        UserRole.SUPERADMIN,
+        UserRole.ADMIN,
+    )
+
+    class Arguments:
+        quota_scope_id = graphene.String(required=True)
+        storage_host_name = graphene.String(required=True)
+
+    quota_scope = graphene.Field(lambda: QuotaScope)
+
+    @classmethod
+    async def mutate(
+        cls,
+        root,
+        info: graphene.ResolveInfo,
+        quota_scope_id: str,
+        storage_host_name: str,
+    ) -> SetQuotaScope:
+        qsid = QuotaScopeID.parse(quota_scope_id)
+        graph_ctx: GraphQueryContext = info.context
+        proxy_name, volume_name = graph_ctx.storage_manager.split_host(storage_host_name)
+        request_body: dict[str, Any] = {
+            "volume": volume_name,
+            "qsid": str(qsid),
+        }
+        async with graph_ctx.db.begin_readonly_session() as sess:
+            await ensure_quota_scope_accessible_by_user(sess, qsid, graph_ctx.user)
+        async with graph_ctx.storage_manager.request(
+            proxy_name,
+            "DELETE",
+            "quota-scope/quota",
+            json=request_body,
+            raise_for_status=True,
+        ):
+            pass
+
+        return cls(
+            QuotaScope(
+                quota_scope_id=quota_scope_id,
+                storage_host_name=storage_host_name,
+            )
+        )
```

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/pglock.py` & `backend.ai-manager-23.3.7/ai/backend/manager/pglock.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/plugin/error_monitor.py` & `backend.ai-manager-23.3.7/ai/backend/manager/plugin/error_monitor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/plugin/webapp.py` & `backend.ai-manager-23.3.7/ai/backend/manager/plugin/webapp.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/registry.py` & `backend.ai-manager-23.3.7/ai/backend/manager/registry.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/scheduler/dispatcher.py` & `backend.ai-manager-23.3.7/ai/backend/manager/scheduler/dispatcher.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/scheduler/drf.py` & `backend.ai-manager-23.3.7/ai/backend/manager/scheduler/drf.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/scheduler/fifo.py` & `backend.ai-manager-23.3.7/ai/backend/manager/scheduler/fifo.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/scheduler/mof.py` & `backend.ai-manager-23.3.7/ai/backend/manager/scheduler/mof.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/scheduler/predicates.py` & `backend.ai-manager-23.3.7/ai/backend/manager/scheduler/predicates.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/scheduler/types.py` & `backend.ai-manager-23.3.7/ai/backend/manager/scheduler/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/server.py` & `backend.ai-manager-23.3.7/ai/backend/manager/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,14 +128,37 @@
     "stats_monitor",
     "error_monitor",
     "hook_plugin_ctx",
 ]
 
 public_interface_objs: MutableMapping[str, Any] = {}
 
+global_subapp_pkgs: Final[list[str]] = [
+    ".acl",
+    ".etcd",
+    ".events",
+    ".auth",
+    ".ratelimit",
+    ".vfolder",
+    ".admin",
+    ".service",
+    ".session",
+    ".stream",
+    ".manager",
+    ".resource",
+    ".scaling_group",
+    ".cluster_template",
+    ".session_template",
+    ".image",
+    ".userconfig",
+    ".domainconfig",
+    ".groupconfig",
+    ".logs",
+]
+
 
 async def hello(request: web.Request) -> web.Response:
     """
     Returns the API version number.
     """
     return web.json_response(
         {
@@ -512,15 +535,17 @@
     async def _set_root_ctx(subapp: web.Application):
         # Allow subapp's access to the root app properties.
         # These are the public APIs exposed to plugins as well.
         subapp["_root.context"] = root_app["_root.context"]
 
     # We must copy the public interface prior to all user-defined startup signal handlers.
     subapp.on_startup.insert(0, _set_root_ctx)
-    prefix = subapp.get("prefix", pkg_name.split(".")[-1].replace("_", "-"))
+    if "prefix" not in subapp:
+        subapp["prefix"] = pkg_name.split(".")[-1].replace("_", "-")
+    prefix = subapp["prefix"]
     root_app.add_subapp("/" + prefix, subapp)
     root_app.middlewares.extend(global_middlewares)
 
 
 def init_subapp(pkg_name: str, root_app: web.Application, create_subapp: AppCreator) -> None:
     root_ctx: RootContext = root_app["_root.context"]
     subapp, global_middlewares = create_subapp(root_ctx.cors_options)
@@ -659,37 +684,15 @@
 
 @actxmgr
 async def server_main(
     loop: asyncio.AbstractEventLoop,
     pidx: int,
     _args: List[Any],
 ) -> AsyncIterator[None]:
-    subapp_pkgs = [
-        ".acl",
-        ".etcd",
-        ".events",
-        ".auth",
-        ".ratelimit",
-        ".vfolder",
-        ".admin",
-        ".service",
-        ".session",
-        ".stream",
-        ".manager",
-        ".resource",
-        ".scaling_group",
-        ".cluster_template",
-        ".session_template",
-        ".image",
-        ".userconfig",
-        ".domainconfig",
-        ".groupconfig",
-        ".logs",
-    ]
-    root_app = build_root_app(pidx, _args[0], subapp_pkgs=subapp_pkgs)
+    root_app = build_root_app(pidx, _args[0], subapp_pkgs=global_subapp_pkgs)
     root_ctx: RootContext = root_app["_root.context"]
 
     # Start aiomonitor.
     # Port is set by config (default=50100 + pidx).
     loop.set_debug(root_ctx.local_config["debug"]["asyncio"])
     m = aiomonitor.Monitor(
         loop,
```

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/types.py` & `backend.ai-manager-23.3.7/ai/backend/manager/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/ai/backend/manager/utils.py` & `backend.ai-manager-23.3.7/ai/backend/manager/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/backend.ai_manager.egg-info/PKG-INFO` & `backend.ai-manager-23.3.7/backend.ai_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-manager
-Version: 23.3.6
+Version: 23.3.7
 Summary: Backend.AI Manager
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-manager-23.3.6/backend.ai_manager.egg-info/SOURCES.txt` & `backend.ai-manager-23.3.7/backend.ai_manager.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 ai/backend/manager/VERSION
 ai/backend/manager/__init__.py
 ai/backend/manager/config.py
 ai/backend/manager/defs.py
 ai/backend/manager/exceptions.py
 ai/backend/manager/idle.py
+ai/backend/manager/openapi.py
 ai/backend/manager/pglock.py
 ai/backend/manager/py.typed
 ai/backend/manager/registry.py
 ai/backend/manager/server.py
 ai/backend/manager/types.py
 ai/backend/manager/utils.py
 ai/backend/manager/api/__init__.py
@@ -155,17 +156,19 @@
 ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py
 ai/backend/manager/models/alembic/versions/95f51fc6ffdb_merge.py
 ai/backend/manager/models/alembic/versions/97f6c80c8aa5_merge.py
 ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py
 ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py
 ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py
 ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py
+ai/backend/manager/models/alembic/versions/9e599b62f6f1_update_kernels_vfolder_mounts_vfid_.py
 ai/backend/manager/models/alembic/versions/__init__.py
 ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py
 ai/backend/manager/models/alembic/versions/a7ca9f175d5f_merge.py
+ai/backend/manager/models/alembic/versions/a9eb2b002330_add_new_resource_policies.py
 ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py
 ai/backend/manager/models/alembic/versions/b5be363ab05c_.py
 ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py
 ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py
 ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py
 ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py
 ai/backend/manager/models/alembic/versions/bf4bae8f942e_add_kernel_host.py
```

### Comparing `backend.ai-manager-23.3.6/backend_shim.py` & `backend.ai-manager-23.3.7/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.6/setup.py` & `backend.ai-manager-23.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,27 +37,28 @@
     },
     'install_requires': (
         'Jinja2~=3.1.2',
         'PyYAML~=6.0',
         'SQLAlchemy[postgresql_asyncpg]~=1.4.40',
         'aiodataloader-ng~=0.2.1',
         'aiodocker~=0.21.0',
+        'aiofiles~=0.8.0',
         'aiohttp_cors~=0.7',
         'aiohttp_sse>=2.0',
         'aiohttp~=3.8.1',
         'aiomonitor-ng~=0.7.2',
         'aiotools~=1.6.1',
         'alembic~=1.8.1',
         'async_timeout~=4.0',
         'attrs>=20.3',
-        """backend.ai-cli==23.03.6
+        """backend.ai-cli==23.03.7
 """,
-        """backend.ai-common==23.03.6
+        """backend.ai-common==23.03.7
 """,
-        """backend.ai-plugin==23.03.6
+        """backend.ai-plugin==23.03.7
 """,
         'callosum~=0.9.10',
         'click>=7.1.2',
         'cryptography>=2.8',
         'graphene~=2.1.9',
         'lark-parser~=0.11.3',
         'more-itertools~=8.13.0',
@@ -69,14 +70,15 @@
         'redis[hiredis]~=4.5.5',
         'setproctitle~=1.3.2',
         'tabulate~=0.8.9',
         'tenacity>=8.0',
         'trafaret~=2.1',
         'types-Jinja2',
         'types-PyYAML',
+        'types-aiofiles',
         'types-click',
         'types-python-dateutil',
         'types-redis',
         'types-six',
         'types-tabulate',
         'typing_extensions~=4.3',
         'uvloop>=0.17; sys_platform != "Windows"',
@@ -376,11 +378,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.6
+    'version': """23.03.7
 """,
     'zip_safe': False,
 })
```

