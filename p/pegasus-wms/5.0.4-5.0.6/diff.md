# Comparing `tmp/pegasus-wms-5.0.4.tar.gz` & `tmp/pegasus-wms-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "../../dist/pegasus-wms-5.0.4.tar", last modified: Thu Feb  9 02:02:56 2023, max compression
+gzip compressed data, was "pegasus-wms-5.0.6.tar", last modified: Mon Jul  3 15:44:38 2023, max compression
```

## Comparing `pegasus-wms-5.0.4.tar` & `pegasus-wms-5.0.6.tar`

### file list

```diff
@@ -1,140 +1,196 @@
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/Pegasus/
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/Pegasus/cli/
--rwxr-xr-x   0 bamboo     (550) users      (100)    77728 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-analyzer.py
--rwxr-xr-x   0 bamboo     (550) users      (100)     8569 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-config.py
--rwxr-xr-x   0 bamboo     (550) users      (100)    20339 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-cwl-converter.py
--rw-r--r--   0 bamboo     (550) users      (100)     9717 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-dagman.py
--rwxr-xr-x   0 bamboo     (550) users      (100)      715 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-db-admin.py
--rwxr-xr-x   0 bamboo     (550) users      (100)       85 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-em.py
--rw-r--r--   0 bamboo     (550) users      (100)     1128 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-exitcode.py
--rwxr-xr-x   0 bamboo     (550) users      (100)    21709 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-graphviz.py
--rwxr-xr-x   0 bamboo     (550) users      (100)      185 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-init.py
--rwxr-xr-x   0 bamboo     (550) users      (100)     8563 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-metadata.py
--rwxr-xr-x   0 bamboo     (550) users      (100)    68997 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-monitord.py
--rw-r--r--   0 bamboo     (550) users      (100)      798 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-preflight-check.py
--rwxr-xr-x   0 bamboo     (550) users      (100)     2581 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-remove.py
--rwxr-xr-x   0 bamboo     (550) users      (100)    10373 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-run.py
--rwxr-xr-x   0 bamboo     (550) users      (100)       73 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-service.py
--rwxr-xr-x   0 bamboo     (550) users      (100)    76787 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-statistics.py
--rwxr-xr-x   0 bamboo     (550) users      (100)       67 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-submitdir.py
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/Pegasus/db/
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/Pegasus/db/admin/
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/
--rw-r--r--   0 bamboo     (550) users      (100)        0 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/__init__.py
--rw-r--r--   0 bamboo     (550) users      (100)      991 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/base_version.py
--rw-r--r--   0 bamboo     (550) users      (100)     3149 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v0.py
--rw-r--r--   0 bamboo     (550) users      (100)     6495 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v1.py
--rw-r--r--   0 bamboo     (550) users      (100)     1213 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v10.py
--rw-r--r--   0 bamboo     (550) users      (100)     2296 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v11.py
--rw-r--r--   0 bamboo     (550) users      (100)    22985 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v12.py
--rw-r--r--   0 bamboo     (550) users      (100)     1599 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v13.py
--rw-r--r--   0 bamboo     (550) users      (100)     1541 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v14.py
--rw-r--r--   0 bamboo     (550) users      (100)     4998 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v2.py
--rw-r--r--   0 bamboo     (550) users      (100)     1651 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v3.py
--rw-r--r--   0 bamboo     (550) users      (100)     1646 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v4.py
--rw-r--r--   0 bamboo     (550) users      (100)     3496 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v5.py
--rw-r--r--   0 bamboo     (550) users      (100)     8536 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v6.py
--rw-r--r--   0 bamboo     (550) users      (100)     1918 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v7.py
--rw-r--r--   0 bamboo     (550) users      (100)     1608 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v8.py
--rw-r--r--   0 bamboo     (550) users      (100)     1223 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v9.py
--rw-r--r--   0 bamboo     (550) users      (100)       84 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/admin/__init__.py
--rw-r--r--   0 bamboo     (550) users      (100)    23123 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/admin/admin_loader.py
--rw-r--r--   0 bamboo     (550) users      (100)    15076 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/admin/commands.py
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/Pegasus/db/workflow/
--rw-r--r--   0 bamboo     (550) users      (100)    32323 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/workflow/__init__.py
--rw-r--r--   0 bamboo     (550) users      (100)    77572 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/workflow/stampede_statistics.py
--rw-r--r--   0 bamboo     (550) users      (100)    32554 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/workflow/stampede_wf_statistics.py
--rw-r--r--   0 bamboo     (550) users      (100)       32 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/__init__.py
--rw-r--r--   0 bamboo     (550) users      (100)     4239 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/base_loader.py
--rw-r--r--   0 bamboo     (550) users      (100)    22956 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/connection.py
--rw-r--r--   0 bamboo     (550) users      (100)    13908 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/dashboard_loader.py
--rw-r--r--   0 bamboo     (550) users      (100)    16339 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/ensembles.py
--rw-r--r--   0 bamboo     (550) users      (100)      728 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/errors.py
--rw-r--r--   0 bamboo     (550) users      (100)     3760 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/expunge.py
--rw-r--r--   0 bamboo     (550) users      (100)    31291 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/schema.py
--rw-r--r--   0 bamboo     (550) users      (100)    45010 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/db/workflow_loader.py
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/Pegasus/monitoring/
--rw-r--r--   0 bamboo     (550) users      (100)      603 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/monitoring/__init__.py
--rw-r--r--   0 bamboo     (550) users      (100)    24846 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/monitoring/event_output.py
--rw-r--r--   0 bamboo     (550) users      (100)    39728 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/monitoring/job.py
--rw-r--r--   0 bamboo     (550) users      (100)     3985 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/monitoring/metadata.py
--rw-r--r--   0 bamboo     (550) users      (100)    36089 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/monitoring/notifications.py
--rw-r--r--   0 bamboo     (550) users      (100)   129645 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/monitoring/workflow.py
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/Pegasus/netlogger/
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/Pegasus/netlogger/parsers/
--rw-r--r--   0 bamboo     (550) users      (100)        0 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/netlogger/parsers/__init__.py
--rw-r--r--   0 bamboo     (550) users      (100)    23024 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/netlogger/parsers/base.py
--rw-r--r--   0 bamboo     (550) users      (100)     2293 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/netlogger/parsers/nlreadline.py
--rw-r--r--   0 bamboo     (550) users      (100)        0 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/netlogger/__init__.py
--rw-r--r--   0 bamboo     (550) users      (100)    87459 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/netlogger/configobj.py
--rw-r--r--   0 bamboo     (550) users      (100)     9846 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/netlogger/magicdate.py
--rw-r--r--   0 bamboo     (550) users      (100)    14361 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/netlogger/nlapi.py
--rw-r--r--   0 bamboo     (550) users      (100)     9975 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/netlogger/nldate.py
--rw-r--r--   0 bamboo     (550) users      (100)    24001 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/netlogger/nllog.py
--rw-r--r--   0 bamboo     (550) users      (100)    24035 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/netlogger/util.py
--rw-r--r--   0 bamboo     (550) users      (100)      551 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/netlogger/version.py
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/Pegasus/plots_stats/
--rw-r--r--   0 bamboo     (550) users      (100)        0 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/plots_stats/__init__.py
--rwxr-xr-x   0 bamboo     (550) users      (100)     8097 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/plots_stats/utils.py
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/Pegasus/service/
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/Pegasus/service/dashboard/
--rw-r--r--   0 bamboo     (550) users      (100)      160 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/dashboard/__init__.py
--rw-r--r--   0 bamboo     (550) users      (100)    23135 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/dashboard/dashboard.py
--rw-r--r--   0 bamboo     (550) users      (100)    34367 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/dashboard/queries.py
--rw-r--r--   0 bamboo     (550) users      (100)    24051 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/dashboard/views.py
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/Pegasus/service/ensembles/
--rw-r--r--   0 bamboo     (550) users      (100)      371 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/ensembles/__init__.py
--rw-r--r--   0 bamboo     (550) users      (100)      643 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/ensembles/api.py
--rw-r--r--   0 bamboo     (550) users      (100)     2472 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/ensembles/bundle.py
--rw-r--r--   0 bamboo     (550) users      (100)    20943 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/ensembles/commands.py
--rw-r--r--   0 bamboo     (550) users      (100)    17214 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/ensembles/manager.py
--rw-r--r--   0 bamboo     (550) users      (100)    12818 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/ensembles/trigger.py
--rw-r--r--   0 bamboo     (550) users      (100)    14603 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/ensembles/views.py
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/Pegasus/service/monitoring/
--rw-r--r--   0 bamboo     (550) users      (100)      798 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/monitoring/__init__.py
--rw-r--r--   0 bamboo     (550) users      (100)     1894 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/monitoring/errors.py
--rw-r--r--   0 bamboo     (550) users      (100)    55498 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/monitoring/queries.py
--rw-r--r--   0 bamboo     (550) users      (100)    36231 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/monitoring/views.py
--rw-r--r--   0 bamboo     (550) users      (100)       49 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/__init__.py
--rw-r--r--   0 bamboo     (550) users      (100)     1941 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/_encoder.py
--rw-r--r--   0 bamboo     (550) users      (100)     6134 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/_query.py
--rw-r--r--   0 bamboo     (550) users      (100)     1770 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/_serialize.py
--rw-r--r--   0 bamboo     (550) users      (100)     2470 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/_sort.py
--rw-r--r--   0 bamboo     (550) users      (100)     1269 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/auth.py
--rw-r--r--   0 bamboo     (550) users      (100)     5124 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/base.py
--rw-r--r--   0 bamboo     (550) users      (100)     1262 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/defaults.py
--rw-r--r--   0 bamboo     (550) users      (100)     2886 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/filters.py
--rw-r--r--   0 bamboo     (550) users      (100)     6742 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/lifecycle.py
--rw-r--r--   0 bamboo     (550) users      (100)     6360 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/service/server.py
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/Pegasus/tools/
--rwxr-xr-x   0 bamboo     (550) users      (100)    41167 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/tools/kickstart_parser.py
--rw-r--r--   0 bamboo     (550) users      (100)    13458 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/tools/properties.py
--rw-r--r--   0 bamboo     (550) users      (100)    21819 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/tools/utils.py
--rw-r--r--   0 bamboo     (550) users      (100)     3316 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/cluster.py
--rw-r--r--   0 bamboo     (550) users      (100)     2743 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/command.py
--rw-r--r--   0 bamboo     (550) users      (100)    15370 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/exitcode.py
--rw-r--r--   0 bamboo     (550) users      (100)    14973 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/init-old.py
--rw-r--r--   0 bamboo     (550) users      (100)    13078 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/init.py
--rw-r--r--   0 bamboo     (550) users      (100)     1631 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/kickstart.py
--rw-r--r--   0 bamboo     (550) users      (100)     2531 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/properties.py
--rw-r--r--   0 bamboo     (550) users      (100)     3670 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/replica_catalog.py
--rw-r--r--   0 bamboo     (550) users      (100)     5445 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/site_catalog.py
--rw-r--r--   0 bamboo     (550) users      (100)    21734 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/submitdir.py
--rw-r--r--   0 bamboo     (550) users      (100)     6167 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/transformation_catalog.py
--rw-r--r--   0 bamboo     (550) users      (100)     1084 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/user.py
--rw-r--r--   0 bamboo     (550) users      (100)     6839 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/src/Pegasus/workflow.py
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/pegasus_wms.egg-info/
--rw-r--r--   0 bamboo     (550) users      (100)     1996 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/pegasus_wms.egg-info/PKG-INFO
--rw-r--r--   0 bamboo     (550) users      (100)     4061 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/pegasus_wms.egg-info/SOURCES.txt
--rw-r--r--   0 bamboo     (550) users      (100)        1 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/pegasus_wms.egg-info/dependency_links.txt
--rw-r--r--   0 bamboo     (550) users      (100)        1 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/pegasus_wms.egg-info/not-zip-safe
--rw-r--r--   0 bamboo     (550) users      (100)      284 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/pegasus_wms.egg-info/requires.txt
--rw-r--r--   0 bamboo     (550) users      (100)        8 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/src/pegasus_wms.egg-info/top_level.txt
--rw-r--r--   0 bamboo     (550) users      (100)    11368 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/LICENSE
--rw-r--r--   0 bamboo     (550) users      (100)       60 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/MANIFEST.in
--rw-r--r--   0 bamboo     (550) users      (100)      425 2023-02-09 02:02:36.000000 pegasus-wms-5.0.4/README.md
--rw-r--r--   0 bamboo     (550) users      (100)      176 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/setup.cfg
--rw-r--r--   0 bamboo     (550) users      (100)     3972 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/setup.py
--rw-r--r--   0 bamboo     (550) users      (100)     1996 2023-02-09 02:02:56.000000 pegasus-wms-5.0.4/PKG-INFO
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.799395 pegasus-wms-5.0.6/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    11368 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/LICENSE
+-rw-r--r--   0 rynge     (1000) rynge     (1000)       60 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/MANIFEST.in
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1875 2023-07-03 15:44:38.799395 pegasus-wms-5.0.6/PKG-INFO
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      425 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/README.md
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      615 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/pyproject.toml
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      176 2023-07-03 15:44:38.799395 pegasus-wms-5.0.6/setup.cfg
+-rw-------   0 rynge     (1000) rynge     (1000)     3987 2023-07-03 15:44:37.000000 pegasus-wms-5.0.6/setup.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.759394 pegasus-wms-5.0.6/src/
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.771394 pegasus-wms-5.0.6/src/Pegasus/
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.775395 pegasus-wms-5.0.6/src/Pegasus/cli/
+-rwxr-xr-x   0 rynge     (1000) rynge     (1000)    77728 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-analyzer.py
+-rwxr-xr-x   0 rynge     (1000) rynge     (1000)     8569 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-config.py
+-rwxr-xr-x   0 rynge     (1000) rynge     (1000)    20339 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-cwl-converter.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     9717 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-dagman.py
+-rwxr-xr-x   0 rynge     (1000) rynge     (1000)      715 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-db-admin.py
+-rwxr-xr-x   0 rynge     (1000) rynge     (1000)       85 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-em.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1128 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-exitcode.py
+-rwxr-xr-x   0 rynge     (1000) rynge     (1000)    21709 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-graphviz.py
+-rwxr-xr-x   0 rynge     (1000) rynge     (1000)      185 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-init.py
+-rwxr-xr-x   0 rynge     (1000) rynge     (1000)     8563 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-metadata.py
+-rwxr-xr-x   0 rynge     (1000) rynge     (1000)    68997 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-monitord.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      798 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-preflight-check.py
+-rwxr-xr-x   0 rynge     (1000) rynge     (1000)     2581 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-remove.py
+-rwxr-xr-x   0 rynge     (1000) rynge     (1000)    10373 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-run.py
+-rwxr-xr-x   0 rynge     (1000) rynge     (1000)       73 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-service.py
+-rwxr-xr-x   0 rynge     (1000) rynge     (1000)    76787 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-statistics.py
+-rwxr-xr-x   0 rynge     (1000) rynge     (1000)       67 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-submitdir.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     3316 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/cluster.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     2743 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/command.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.775395 pegasus-wms-5.0.6/src/Pegasus/db/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)       32 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/db/__init__.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.775395 pegasus-wms-5.0.6/src/Pegasus/db/admin/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)       84 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/db/admin/__init__.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    23123 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/db/admin/admin_loader.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    15076 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/db/admin/commands.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.779394 pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)        0 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/__init__.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      991 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/base_version.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     3149 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v0.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     6495 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v1.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1213 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v10.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     2296 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v11.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    22985 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v12.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1599 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v13.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1541 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v14.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     4998 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v2.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1651 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v3.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1646 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v4.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     3496 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v5.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     8536 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v6.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1918 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v7.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1608 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v8.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1223 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v9.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     4239 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/db/base_loader.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    22956 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/db/connection.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    13908 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/db/dashboard_loader.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    16339 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/db/ensembles.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      728 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/db/errors.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     3760 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/db/expunge.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    31291 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/db/schema.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.779394 pegasus-wms-5.0.6/src/Pegasus/db/workflow/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    32323 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/db/workflow/__init__.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    77572 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/db/workflow/stampede_statistics.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    32554 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/db/workflow/stampede_wf_statistics.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    45010 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/db/workflow_loader.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    15370 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/exitcode.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    14973 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/init-old.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    13078 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/init.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1631 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/kickstart.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.783394 pegasus-wms-5.0.6/src/Pegasus/monitoring/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      603 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/monitoring/__init__.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    24846 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/monitoring/event_output.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    39728 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/monitoring/job.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     3985 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/monitoring/metadata.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    36089 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/monitoring/notifications.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)   129645 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/monitoring/workflow.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.783394 pegasus-wms-5.0.6/src/Pegasus/netlogger/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)        0 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/netlogger/__init__.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    87459 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/netlogger/configobj.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     9846 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/netlogger/magicdate.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    14361 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/netlogger/nlapi.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     9975 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/netlogger/nldate.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    24001 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/netlogger/nllog.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.783394 pegasus-wms-5.0.6/src/Pegasus/netlogger/parsers/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)        0 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/netlogger/parsers/__init__.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    23024 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/netlogger/parsers/base.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     2293 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/netlogger/parsers/nlreadline.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    24035 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/netlogger/util.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      551 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/netlogger/version.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.783394 pegasus-wms-5.0.6/src/Pegasus/plots_stats/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)        0 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/plots_stats/__init__.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     8097 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/plots_stats/utils.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     2531 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/properties.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     3670 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/replica_catalog.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.787395 pegasus-wms-5.0.6/src/Pegasus/service/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      542 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/TODO.md
+-rw-r--r--   0 rynge     (1000) rynge     (1000)       49 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/__init__.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1941 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/_encoder.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     6134 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/_query.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1770 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/_serialize.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     2470 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/_sort.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1269 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/auth.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     5124 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/base.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.787395 pegasus-wms-5.0.6/src/Pegasus/service/dashboard/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      160 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/dashboard/__init__.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    23135 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/dashboard/dashboard.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    34367 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/dashboard/queries.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    24051 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/dashboard/views.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1262 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/defaults.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.787395 pegasus-wms-5.0.6/src/Pegasus/service/ensembles/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      371 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/ensembles/__init__.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      643 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/ensembles/api.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     2472 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/ensembles/bundle.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    20943 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/ensembles/commands.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    17214 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/ensembles/manager.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    12818 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/ensembles/trigger.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    14603 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/ensembles/views.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     2886 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/filters.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     6742 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/lifecycle.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.791395 pegasus-wms-5.0.6/src/Pegasus/service/monitoring/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      798 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/monitoring/__init__.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1894 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/monitoring/errors.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    55498 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/monitoring/queries.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    35141 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/monitoring/swagger.yml
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    36231 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/monitoring/views.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     5001 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/server.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.791395 pegasus-wms-5.0.6/src/Pegasus/service/static/
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.791395 pegasus-wms-5.0.6/src/Pegasus/service/static/css/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     9742 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/static/css/pe-icon-7-stroke.css
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     5295 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/static/css/style.css
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1406 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/static/favicon.ico
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.791395 pegasus-wms-5.0.6/src/Pegasus/service/static/fonts/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    58680 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/static/fonts/Pe-icon-7-stroke.eot
+-rw-r--r--   0 rynge     (1000) rynge     (1000)   164020 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/static/fonts/Pe-icon-7-stroke.svg
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    58480 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/static/fonts/Pe-icon-7-stroke.ttf
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    58556 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/static/fonts/Pe-icon-7-stroke.woff
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.795395 pegasus-wms-5.0.6/src/Pegasus/service/static/images/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    16977 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/static/images/about.png
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     7364 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/static/images/ajax-loader-1.gif
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.795395 pegasus-wms-5.0.6/src/Pegasus/service/static/images/footer/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    20441 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/static/images/footer/isi.png
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     9314 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/static/images/footer/pegasus.jpg
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    14725 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/static/images/footer/stampede.png
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    12706 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/static/images/footer/usc.png
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    48065 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/static/images/help.png
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     5971 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/static/images/home.png
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1775 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/static/images/list.png
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     7364 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/static/images/please-wait.gif
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    10513 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/static/images/reload.png
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.795395 pegasus-wms-5.0.6/src/Pegasus/service/static/js/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     9996 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/static/js/charts.js
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     2651 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/static/js/script.js
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    12694 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/static/js/statistics.js
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.795395 pegasus-wms-5.0.6/src/Pegasus/service/templates/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1929 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/templates/base-error.html
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     3274 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/templates/base.html
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.799395 pegasus-wms-5.0.6/src/Pegasus/service/templates/error/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      183 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/service/templates/error/404.html
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      676 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/templates/error/catch_all.html
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1238 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/templates/error/database_migration_error.html
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      379 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/templates/error/error_response.html
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      601 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/templates/error/master_database_missing.html
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      480 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/templates/error/stampede_database_missing.html
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.799395 pegasus-wms-5.0.6/src/Pegasus/service/templates/error/workflow/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      597 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/templates/error/workflow/workflow_details_missing.html
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     7949 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/templates/file-browser.html
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1616 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/templates/footer.html
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1016 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/templates/header.html
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      531 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/templates/info.html
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.799395 pegasus-wms-5.0.6/src/Pegasus/service/templates/workflow/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     3369 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/templates/workflow/charts.html
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.799395 pegasus-wms-5.0.6/src/Pegasus/service/templates/workflow/job/
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.799395 pegasus-wms-5.0.6/src/Pegasus/service/templates/workflow/job/invocation/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     4408 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/templates/workflow/job/invocation/invocation_details.html
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    13366 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/templates/workflow/job/job_details.html
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     2945 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/templates/workflow/statistics.html
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    28747 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/templates/workflow/workflow_details.html
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     5097 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/service/templates/workflow.html
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     5445 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/site_catalog.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    21734 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/submitdir.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.799395 pegasus-wms-5.0.6/src/Pegasus/tools/
+-rwxr-xr-x   0 rynge     (1000) rynge     (1000)    41167 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/tools/kickstart_parser.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    13458 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/tools/properties.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    21819 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/tools/utils.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     6167 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/transformation_catalog.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1084 2023-06-30 20:04:01.000000 pegasus-wms-5.0.6/src/Pegasus/user.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     6960 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/src/Pegasus/workflow.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:38.799395 pegasus-wms-5.0.6/src/pegasus_wms.egg-info/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1875 2023-07-03 15:44:37.000000 pegasus-wms-5.0.6/src/pegasus_wms.egg-info/PKG-INFO
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     6185 2023-07-03 15:44:38.000000 pegasus-wms-5.0.6/src/pegasus_wms.egg-info/SOURCES.txt
+-rw-r--r--   0 rynge     (1000) rynge     (1000)        1 2023-07-03 15:44:37.000000 pegasus-wms-5.0.6/src/pegasus_wms.egg-info/dependency_links.txt
+-rw-r--r--   0 rynge     (1000) rynge     (1000)        1 2023-07-03 15:44:37.000000 pegasus-wms-5.0.6/src/pegasus_wms.egg-info/not-zip-safe
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      282 2023-07-03 15:44:37.000000 pegasus-wms-5.0.6/src/pegasus_wms.egg-info/requires.txt
+-rw-r--r--   0 rynge     (1000) rynge     (1000)        8 2023-07-03 15:44:37.000000 pegasus-wms-5.0.6/src/pegasus_wms.egg-info/top_level.txt
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     3488 2023-07-03 15:42:39.000000 pegasus-wms-5.0.6/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-analyzer.py` & `pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-analyzer.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-config.py` & `pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-config.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-cwl-converter.py` & `pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-cwl-converter.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-dagman.py` & `pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-dagman.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-db-admin.py` & `pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-db-admin.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-exitcode.py` & `pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-exitcode.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-graphviz.py` & `pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-graphviz.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-metadata.py` & `pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-metadata.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-monitord.py` & `pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-monitord.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-preflight-check.py` & `pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-preflight-check.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-remove.py` & `pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-remove.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-run.py` & `pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-run.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/cli/pegasus-statistics.py` & `pegasus-wms-5.0.6/src/Pegasus/cli/pegasus-statistics.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/base_version.py` & `pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/base_version.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v0.py` & `pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v0.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v1.py` & `pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v1.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v10.py` & `pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v10.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v11.py` & `pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v11.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v12.py` & `pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v12.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v13.py` & `pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v13.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v14.py` & `pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v14.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v2.py` & `pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v2.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v3.py` & `pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v3.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v4.py` & `pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v4.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v5.py` & `pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v5.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v6.py` & `pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v6.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v7.py` & `pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v7.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v8.py` & `pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v8.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/admin/versions/v9.py` & `pegasus-wms-5.0.6/src/Pegasus/db/admin/versions/v9.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/admin/admin_loader.py` & `pegasus-wms-5.0.6/src/Pegasus/db/admin/admin_loader.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/admin/commands.py` & `pegasus-wms-5.0.6/src/Pegasus/db/admin/commands.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/workflow/__init__.py` & `pegasus-wms-5.0.6/src/Pegasus/db/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/workflow/stampede_statistics.py` & `pegasus-wms-5.0.6/src/Pegasus/db/workflow/stampede_statistics.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/workflow/stampede_wf_statistics.py` & `pegasus-wms-5.0.6/src/Pegasus/db/workflow/stampede_wf_statistics.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/base_loader.py` & `pegasus-wms-5.0.6/src/Pegasus/db/base_loader.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/connection.py` & `pegasus-wms-5.0.6/src/Pegasus/db/connection.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/dashboard_loader.py` & `pegasus-wms-5.0.6/src/Pegasus/db/dashboard_loader.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/ensembles.py` & `pegasus-wms-5.0.6/src/Pegasus/db/ensembles.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/errors.py` & `pegasus-wms-5.0.6/src/Pegasus/db/errors.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/expunge.py` & `pegasus-wms-5.0.6/src/Pegasus/db/expunge.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/schema.py` & `pegasus-wms-5.0.6/src/Pegasus/db/schema.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/db/workflow_loader.py` & `pegasus-wms-5.0.6/src/Pegasus/db/workflow_loader.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/monitoring/__init__.py` & `pegasus-wms-5.0.6/src/Pegasus/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/monitoring/event_output.py` & `pegasus-wms-5.0.6/src/Pegasus/monitoring/event_output.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/monitoring/job.py` & `pegasus-wms-5.0.6/src/Pegasus/monitoring/job.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/monitoring/metadata.py` & `pegasus-wms-5.0.6/src/Pegasus/monitoring/metadata.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/monitoring/notifications.py` & `pegasus-wms-5.0.6/src/Pegasus/monitoring/notifications.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/monitoring/workflow.py` & `pegasus-wms-5.0.6/src/Pegasus/monitoring/workflow.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/netlogger/parsers/base.py` & `pegasus-wms-5.0.6/src/Pegasus/netlogger/parsers/base.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/netlogger/parsers/nlreadline.py` & `pegasus-wms-5.0.6/src/Pegasus/netlogger/parsers/nlreadline.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/netlogger/configobj.py` & `pegasus-wms-5.0.6/src/Pegasus/netlogger/configobj.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/netlogger/magicdate.py` & `pegasus-wms-5.0.6/src/Pegasus/netlogger/magicdate.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/netlogger/nlapi.py` & `pegasus-wms-5.0.6/src/Pegasus/netlogger/nlapi.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/netlogger/nldate.py` & `pegasus-wms-5.0.6/src/Pegasus/netlogger/nldate.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/netlogger/nllog.py` & `pegasus-wms-5.0.6/src/Pegasus/netlogger/nllog.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/netlogger/util.py` & `pegasus-wms-5.0.6/src/Pegasus/netlogger/util.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/netlogger/version.py` & `pegasus-wms-5.0.6/src/Pegasus/netlogger/version.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/plots_stats/utils.py` & `pegasus-wms-5.0.6/src/Pegasus/plots_stats/utils.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/dashboard/dashboard.py` & `pegasus-wms-5.0.6/src/Pegasus/service/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/dashboard/queries.py` & `pegasus-wms-5.0.6/src/Pegasus/service/dashboard/queries.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/dashboard/views.py` & `pegasus-wms-5.0.6/src/Pegasus/service/dashboard/views.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/ensembles/api.py` & `pegasus-wms-5.0.6/src/Pegasus/service/ensembles/api.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/ensembles/bundle.py` & `pegasus-wms-5.0.6/src/Pegasus/service/ensembles/bundle.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/ensembles/commands.py` & `pegasus-wms-5.0.6/src/Pegasus/service/ensembles/commands.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/ensembles/manager.py` & `pegasus-wms-5.0.6/src/Pegasus/service/ensembles/manager.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/ensembles/trigger.py` & `pegasus-wms-5.0.6/src/Pegasus/service/ensembles/trigger.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/ensembles/views.py` & `pegasus-wms-5.0.6/src/Pegasus/service/ensembles/views.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/monitoring/__init__.py` & `pegasus-wms-5.0.6/src/Pegasus/service/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/monitoring/errors.py` & `pegasus-wms-5.0.6/src/Pegasus/service/monitoring/errors.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/monitoring/queries.py` & `pegasus-wms-5.0.6/src/Pegasus/service/monitoring/queries.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/monitoring/views.py` & `pegasus-wms-5.0.6/src/Pegasus/service/monitoring/views.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/_encoder.py` & `pegasus-wms-5.0.6/src/Pegasus/service/_encoder.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/_query.py` & `pegasus-wms-5.0.6/src/Pegasus/service/_query.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/_serialize.py` & `pegasus-wms-5.0.6/src/Pegasus/service/_serialize.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/_sort.py` & `pegasus-wms-5.0.6/src/Pegasus/service/_sort.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/auth.py` & `pegasus-wms-5.0.6/src/Pegasus/service/auth.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/base.py` & `pegasus-wms-5.0.6/src/Pegasus/service/base.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/defaults.py` & `pegasus-wms-5.0.6/src/Pegasus/service/defaults.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/filters.py` & `pegasus-wms-5.0.6/src/Pegasus/service/filters.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/lifecycle.py` & `pegasus-wms-5.0.6/src/Pegasus/service/lifecycle.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/service/server.py` & `pegasus-wms-5.0.6/src/Pegasus/service/server.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import logging
 import os
-import random
 
 import click
 import flask
-from OpenSSL import crypto
 from werkzeug.middleware.dispatcher import DispatcherMiddleware
 from werkzeug.serving import run_simple
 
 from Pegasus.service import cache
 from Pegasus.service._encoder import PegasusJsonEncoder
 from Pegasus.service.base import BooleanConverter
 from Pegasus.service.filters import register_jinja2_filters
@@ -16,53 +14,14 @@
 
 log = logging.getLogger(__name__)
 
 # Services
 services = ["dashboard", "monitoring"]
 
 
-def generate_self_signed_certificate(certfile, pkeyfile):
-    """
-    SSL.
-    :param certfile:
-    :param pkeyfile:
-    :return:
-    If certfile and pkeyfile don't exist, create a self-signed certificate
-    """
-
-    if os.path.isfile(certfile) and os.path.isfile(pkeyfile):
-        return
-
-    logging.info("Generating self-signed certificate")
-
-    pkey = crypto.PKey()
-    pkey.generate_key(crypto.TYPE_RSA, 2048)
-
-    cert = crypto.X509()
-
-    sub = cert.get_subject()
-    sub.C = "US"
-    sub.ST = "California"
-    sub.L = "Marina Del Rey"
-    sub.O = "University of Southern California"
-    sub.OU = "Information Sciences Institute"
-    sub.CN = "Pegasus Service"
-
-    cert.set_version(1)
-    cert.set_serial_number(random.randint(0, 2 ** 32))
-    cert.gmtime_adj_notBefore(0)
-    cert.gmtime_adj_notAfter(10 * 365 * 24 * 60 * 60)  # 10 years
-    cert.set_issuer(sub)
-    cert.set_pubkey(pkey)
-    cert.sign(pkey, "sha1")
-
-    open(certfile, "wb").write(crypto.dump_certificate(crypto.FILETYPE_PEM, cert))
-    open(pkeyfile, "wb").write(crypto.dump_privatekey(crypto.FILETYPE_PEM, pkey))
-
-
 def run(host="localhost", port=5000, debug=True, verbose=logging.INFO, **kwargs):
     app = create_app(env=os.getenv("FLASK_ENV", "development"))
 
     if debug:
         app.config.update(DEBUG=True)
         logging.getLogger().setLevel(logging.DEBUG)
 
@@ -77,20 +36,18 @@
 
     pegasusdir = os.path.expanduser("~/.pegasus")
     if not os.path.isdir(pegasusdir):
         os.makedirs(pegasusdir, mode=0o744)
 
     cert = app.config.get("CERTIFICATE", None)
     pkey = app.config.get("PRIVATE_KEY", None)
-    if cert is None or pkey is None:
-        log.warning("SSL is not configured: Using self-signed certificate")
-        cert = os.path.expanduser("~/.pegasus/selfcert.pem")
-        pkey = os.path.expanduser("~/.pegasus/selfkey.pem")
-        generate_self_signed_certificate(cert, pkey)
-    ssl_context = (cert, pkey)
+    if cert and pkey:
+        ssl_context = (cert, pkey)
+    else:
+        ssl_context = "adhoc"
 
     if os.getuid() != 0:
         log.warning("Service not running as root: Will not be able to switch users")
 
     options = {}
     if app.config.get("MAX_PROCESSES", None):
         options = {
```

### Comparing `pegasus-wms-5.0.4/src/Pegasus/tools/kickstart_parser.py` & `pegasus-wms-5.0.6/src/Pegasus/tools/kickstart_parser.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/tools/properties.py` & `pegasus-wms-5.0.6/src/Pegasus/tools/properties.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/tools/utils.py` & `pegasus-wms-5.0.6/src/Pegasus/tools/utils.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/cluster.py` & `pegasus-wms-5.0.6/src/Pegasus/cluster.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/command.py` & `pegasus-wms-5.0.6/src/Pegasus/command.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/exitcode.py` & `pegasus-wms-5.0.6/src/Pegasus/exitcode.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/init-old.py` & `pegasus-wms-5.0.6/src/Pegasus/init-old.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/init.py` & `pegasus-wms-5.0.6/src/Pegasus/init.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/kickstart.py` & `pegasus-wms-5.0.6/src/Pegasus/kickstart.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/properties.py` & `pegasus-wms-5.0.6/src/Pegasus/properties.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/replica_catalog.py` & `pegasus-wms-5.0.6/src/Pegasus/replica_catalog.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/site_catalog.py` & `pegasus-wms-5.0.6/src/Pegasus/site_catalog.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/submitdir.py` & `pegasus-wms-5.0.6/src/Pegasus/submitdir.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/transformation_catalog.py` & `pegasus-wms-5.0.6/src/Pegasus/transformation_catalog.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/user.py` & `pegasus-wms-5.0.6/src/Pegasus/user.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/src/Pegasus/workflow.py` & `pegasus-wms-5.0.6/src/Pegasus/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,19 @@
                 args.append(a)
 
             job.args = args
 
             # add uses
             uses = set()
             for u in j["uses"]:
-                f = File(u["lfn"], size=u.get("size"))
+                f = File(
+                    u["lfn"],
+                    size=u.get("size"),
+                    for_planning=u.get("forPlanning", False),
+                )
                 try:
                     f.metadata = u["metadata"]
                 except KeyError:
                     pass
 
                 uses.add(
                     _Use(
```

### Comparing `pegasus-wms-5.0.4/src/pegasus_wms.egg-info/PKG-INFO` & `pegasus-wms-5.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,20 @@
 Metadata-Version: 2.1
 Name: pegasus-wms
-Version: 5.0.4
+Version: 5.0.6
 Summary: Pegasus Workflow Management System Python Codebase
 Home-page: http://pegasus.isi.edu
 Author: Pegasus Team
 Author-email: pegasus@isi.edu
 License: Apache2
 Project-URL: Documentation, https://pegasus.isi.edu/documentation/
 Project-URL: Changes, https://pegasus.isi.edu/blog/?category_name=Release
 Project-URL: Source Code, https://github.com/pegasus-isi/pegasus
 Project-URL: Issue Tracker, https://jira.isi.edu/projects/PM/issues
-Description: Pegasus Workflow Management System Python API
-        =============================================
-        
-        This package contains the Python APIs for Pegasus WMS, including:
-        
-        1. The DAX API (Versions 2 and 3)
-        2. The PDAX API (Version 2)
-        3. The monitoring API
-        4. The Stampede database API
-        5. The Pegasus statistics API
-        6. The Pegasus plots API
-        7. Misc. Pegasus utilities
-        8. The pegasus service, including the ensemble manager and dashboard
-        
-        
 Keywords: scientific workflows
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -41,10 +25,26 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-Provides-Extra: mysql
 Provides-Extra: cwl
+Provides-Extra: mysql
 Provides-Extra: postgresql
+License-File: LICENSE
+
+Pegasus Workflow Management System Python API
+=============================================
+
+This package contains the Python APIs for Pegasus WMS, including:
+
+1. The DAX API (Versions 2 and 3)
+2. The PDAX API (Version 2)
+3. The monitoring API
+4. The Stampede database API
+5. The Pegasus statistics API
+6. The Pegasus plots API
+7. Misc. Pegasus utilities
+8. The pegasus service, including the ensemble manager and dashboard
+
```

### Comparing `pegasus-wms-5.0.4/LICENSE` & `pegasus-wms-5.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pegasus-wms-5.0.4/setup.py` & `pegasus-wms-5.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,34 +8,35 @@
 
 install_requires = [
     # Utils
     # DAX/Workflow
     "PyYAML>5.3",
     # pegasus-init
     "GitPython>1.0",
-    "pamela>=1.0",
+    "pamela>=1.0,<1.1.0",
     "pika>=1.1.0",
-    "Flask>1.1",
+    "Flask>1.1,<2.3",
     "Flask-Caching>1.8",
     "requests>2.23",
     "sqlalchemy>1.3,<1.4",
     "pegasus-wms.api",
     "pegasus-wms.dax",
     "pegasus-wms.common",
     "pegasus-wms.worker",
 ]
 
+
 #
 # Install conditional dependencies
 #
 def setup_installer_dependencies():
     global install_requires
 
     if subprocess.call(["which", "mysql_config"]) == 0:
-        install_requires.append("mysqlclient<2.0.0")
+        install_requires.append("pymysql<=0.10.1")
 
 
 #
 # Utility function to read the pegasus Version.in file
 #
 def read_version():
     return (
@@ -84,15 +85,15 @@
     return [path.replace(dirname, "") for path in items]
 
 
 setup_installer_dependencies()
 
 setup(
     name="pegasus-wms",
-    version="5.0.4",
+    version="5.0.6",
     author="Pegasus Team",
     author_email="pegasus@isi.edu",
     description="Pegasus Workflow Management System Python Codebase",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     license="Apache2",
     url="http://pegasus.isi.edu",
@@ -127,11 +128,11 @@
     package_data={"Pegasus.service": find_package_data("src/Pegasus/service/")},
     include_package_data=True,
     zip_safe=False,
     install_requires=install_requires,
     convert_2to3_doctests=[],
     extras_require={
         "postgresql": ["psycopg2"],
-        "mysql": ["mysqlclient"],
+        "mysql": ["pymysql<=0.10.1"],
         "cwl": ["cwl-utils==0.11", "jsonschema==3.2.0"],
     },
 )
```

### Comparing `pegasus-wms-5.0.4/PKG-INFO` & `pegasus-wms-5.0.6/src/pegasus_wms.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,20 @@
 Metadata-Version: 2.1
 Name: pegasus-wms
-Version: 5.0.4
+Version: 5.0.6
 Summary: Pegasus Workflow Management System Python Codebase
 Home-page: http://pegasus.isi.edu
 Author: Pegasus Team
 Author-email: pegasus@isi.edu
 License: Apache2
 Project-URL: Documentation, https://pegasus.isi.edu/documentation/
 Project-URL: Changes, https://pegasus.isi.edu/blog/?category_name=Release
 Project-URL: Source Code, https://github.com/pegasus-isi/pegasus
 Project-URL: Issue Tracker, https://jira.isi.edu/projects/PM/issues
-Description: Pegasus Workflow Management System Python API
-        =============================================
-        
-        This package contains the Python APIs for Pegasus WMS, including:
-        
-        1. The DAX API (Versions 2 and 3)
-        2. The PDAX API (Version 2)
-        3. The monitoring API
-        4. The Stampede database API
-        5. The Pegasus statistics API
-        6. The Pegasus plots API
-        7. Misc. Pegasus utilities
-        8. The pegasus service, including the ensemble manager and dashboard
-        
-        
 Keywords: scientific workflows
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -41,10 +25,26 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-Provides-Extra: mysql
 Provides-Extra: cwl
+Provides-Extra: mysql
 Provides-Extra: postgresql
+License-File: LICENSE
+
+Pegasus Workflow Management System Python API
+=============================================
+
+This package contains the Python APIs for Pegasus WMS, including:
+
+1. The DAX API (Versions 2 and 3)
+2. The PDAX API (Version 2)
+3. The monitoring API
+4. The Stampede database API
+5. The Pegasus statistics API
+6. The Pegasus plots API
+7. Misc. Pegasus utilities
+8. The pegasus service, including the ensemble manager and dashboard
+
```

