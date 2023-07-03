# Comparing `tmp/ovs-cluster-agent-2.2.3.tar.gz` & `tmp/ovs-cluster-agent-2.2.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovs-cluster-agent-2.2.3.tar", last modified: Mon Jul  3 20:51:06 2023, max compression
+gzip compressed data, was "ovs-cluster-agent-2.2.3rc1.tar", last modified: Thu Jun 22 17:31:14 2023, max compression
```

## Comparing `ovs-cluster-agent-2.2.3.tar` & `ovs-cluster-agent-2.2.3rc1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:51:06.343183 ovs-cluster-agent-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-03 20:51:06.343183 ovs-cluster-agent-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:51:06.343183 ovs-cluster-agent-2.2.3/cluster_agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:51:06.343183 ovs-cluster-agent-2.2.3/cluster_agent/identity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/identity/cluster_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:51:06.343183 ovs-cluster-agent-2.2.3/cluster_agent/identity/slurm_user/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/identity/slurm_user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/identity/slurm_user/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/identity/slurm_user/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/identity/slurm_user/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:51:06.343183 ovs-cluster-agent-2.2.3/cluster_agent/identity/slurm_user/mappers/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/identity/slurm_user/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/identity/slurm_user/mappers/ldap.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/identity/slurm_user/mappers/mapper_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/identity/slurm_user/mappers/single_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/identity/slurmrestd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:51:06.343183 ovs-cluster-agent-2.2.3/cluster_agent/jobbergate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/jobbergate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/jobbergate/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/jobbergate/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/jobbergate/finish.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/jobbergate/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/jobbergate/submit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:51:06.343183 ovs-cluster-agent-2.2.3/cluster_agent/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/scripts/agentconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:51:06.343183 ovs-cluster-agent-2.2.3/cluster_agent/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/cluster_agent/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:51:06.343183 ovs-cluster-agent-2.2.3/ovs_cluster_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-03 20:51:06.000000 ovs-cluster-agent-2.2.3/ovs_cluster_agent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-03 20:51:06.000000 ovs-cluster-agent-2.2.3/ovs_cluster_agent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:51:06.000000 ovs-cluster-agent-2.2.3/ovs_cluster_agent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-03 20:51:06.000000 ovs-cluster-agent-2.2.3/ovs_cluster_agent.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-03 20:51:06.000000 ovs-cluster-agent-2.2.3/ovs_cluster_agent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 20:51:06.000000 ovs-cluster-agent-2.2.3/ovs_cluster_agent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 20:51:06.343183 ovs-cluster-agent-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:51:06.343183 ovs-cluster-agent-2.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:51:06.343183 ovs-cluster-agent-2.2.3/tests/identity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/tests/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/tests/identity/test_cluster_api_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/tests/identity/test_slurmrestd_identity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:51:06.343183 ovs-cluster-agent-2.2.3/tests/jobbergate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/tests/jobbergate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/tests/jobbergate/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/tests/jobbergate/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/tests/jobbergate/test_finish.py
--rw-r--r--   0 runner    (1001) docker     (123)    17373 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/tests/jobbergate/test_submit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12434 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/tests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-03 20:50:56.000000 ovs-cluster-agent-2.2.3/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.137419 ovs-cluster-agent-2.2.3rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-22 17:31:14.137419 ovs-cluster-agent-2.2.3rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.133419 ovs-cluster-agent-2.2.3rc1/cluster_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.133419 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/cluster_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.133419 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.133419 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/mappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/mappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/mappers/ldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/mappers/mapper_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/mappers/single_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurmrestd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.133419 ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.133419 ovs-cluster-agent-2.2.3rc1/cluster_agent/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/scripts/agentconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.133419 ovs-cluster-agent-2.2.3rc1/cluster_agent/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/cluster_agent/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.133419 ovs-cluster-agent-2.2.3rc1/ovs_cluster_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-22 17:31:13.000000 ovs-cluster-agent-2.2.3rc1/ovs_cluster_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-22 17:31:14.000000 ovs-cluster-agent-2.2.3rc1/ovs_cluster_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 17:31:13.000000 ovs-cluster-agent-2.2.3rc1/ovs_cluster_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-22 17:31:13.000000 ovs-cluster-agent-2.2.3rc1/ovs_cluster_agent.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-22 17:31:13.000000 ovs-cluster-agent-2.2.3rc1/ovs_cluster_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-22 17:31:13.000000 ovs-cluster-agent-2.2.3rc1/ovs_cluster_agent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 17:31:14.137419 ovs-cluster-agent-2.2.3rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.133419 ovs-cluster-agent-2.2.3rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.137419 ovs-cluster-agent-2.2.3rc1/tests/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/identity/test_cluster_api_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/identity/test_slurmrestd_identity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:14.137419 ovs-cluster-agent-2.2.3rc1/tests/jobbergate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/jobbergate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/jobbergate/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/jobbergate/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/jobbergate/test_finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17373 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/jobbergate/test_submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12434 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-22 17:31:02.000000 ovs-cluster-agent-2.2.3rc1/tests/test_settings.py
```

### Comparing `ovs-cluster-agent-2.2.3/LICENSE` & `ovs-cluster-agent-2.2.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/PKG-INFO` & `ovs-cluster-agent-2.2.3rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ovs-cluster-agent
-Version: 2.2.3
+Version: 2.2.3rc1
 Summary: Cluster API data aggregator
 Home-page: https://github.com/omnivector-solutions/ovs-cluster-agent/
 Author: omnivector-solutions
 Author-email: info@omnivector.solutions
 License: MIT
-Download-URL: https://github.com/omnivector-solutions/ovs-cluster-agent/dist/cluster-agent-2.2.3tar.gz
+Download-URL: https://github.com/omnivector-solutions/ovs-cluster-agent/dist/cluster-agent-2.2.3-rc.1tar.gz
 Description: # cluster-agent
         
         # Table of contents
         
         - [Project setup](#project-setup)
           - [Dependencies](#dependencies)
         - [Install the package](#install-the-package)
```

### Comparing `ovs-cluster-agent-2.2.3/README.md` & `ovs-cluster-agent-2.2.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/cluster_agent/agent.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/agent.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/cluster_agent/identity/cluster_api.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/cluster_api.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/cluster_agent/identity/slurm_user/factory.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/factory.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/cluster_agent/identity/slurm_user/mappers/ldap.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/mappers/ldap.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/cluster_agent/identity/slurm_user/mappers/mapper_base.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/mappers/mapper_base.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/cluster_agent/identity/slurm_user/mappers/single_user.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurm_user/mappers/single_user.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/cluster_agent/identity/slurmrestd.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/identity/slurmrestd.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/cluster_agent/jobbergate/api.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/api.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/cluster_agent/jobbergate/constants.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/constants.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/cluster_agent/jobbergate/finish.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/finish.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/cluster_agent/jobbergate/schemas.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/schemas.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/cluster_agent/jobbergate/submit.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/jobbergate/submit.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/cluster_agent/main.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/main.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/cluster_agent/scripts/agentconfig.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/scripts/agentconfig.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/cluster_agent/settings.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/settings.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/cluster_agent/utils/exception.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/utils/exception.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/cluster_agent/utils/logging.py` & `ovs-cluster-agent-2.2.3rc1/cluster_agent/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/ovs_cluster_agent.egg-info/PKG-INFO` & `ovs-cluster-agent-2.2.3rc1/ovs_cluster_agent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ovs-cluster-agent
-Version: 2.2.3
+Version: 2.2.3rc1
 Summary: Cluster API data aggregator
 Home-page: https://github.com/omnivector-solutions/ovs-cluster-agent/
 Author: omnivector-solutions
 Author-email: info@omnivector.solutions
 License: MIT
-Download-URL: https://github.com/omnivector-solutions/ovs-cluster-agent/dist/cluster-agent-2.2.3tar.gz
+Download-URL: https://github.com/omnivector-solutions/ovs-cluster-agent/dist/cluster-agent-2.2.3-rc.1tar.gz
 Description: # cluster-agent
         
         # Table of contents
         
         - [Project setup](#project-setup)
           - [Dependencies](#dependencies)
         - [Install the package](#install-the-package)
```

### Comparing `ovs-cluster-agent-2.2.3/ovs_cluster_agent.egg-info/SOURCES.txt` & `ovs-cluster-agent-2.2.3rc1/ovs_cluster_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/setup.py` & `ovs-cluster-agent-2.2.3rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from os.path import dirname, join
 
 here = dirname(__file__)
 
-_VERSION = "2.2.3"
+_VERSION = "2.2.3-rc.1"
 
 setup(
     name="ovs-cluster-agent",
     version=_VERSION,
     description="Cluster API data aggregator",
     long_description=open(join(here, "README.md")).read(),
     long_description_content_type="text/markdown",
```

### Comparing `ovs-cluster-agent-2.2.3/tests/conftest.py` & `ovs-cluster-agent-2.2.3rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/tests/identity/test_cluster_api_identity.py` & `ovs-cluster-agent-2.2.3rc1/tests/identity/test_cluster_api_identity.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/tests/identity/test_slurmrestd_identity.py` & `ovs-cluster-agent-2.2.3rc1/tests/identity/test_slurmrestd_identity.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/tests/jobbergate/conftest.py` & `ovs-cluster-agent-2.2.3rc1/tests/jobbergate/conftest.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/tests/jobbergate/test_api.py` & `ovs-cluster-agent-2.2.3rc1/tests/jobbergate/test_api.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/tests/jobbergate/test_finish.py` & `ovs-cluster-agent-2.2.3rc1/tests/jobbergate/test_finish.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/tests/jobbergate/test_submit.py` & `ovs-cluster-agent-2.2.3rc1/tests/jobbergate/test_submit.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/tests/test_agent.py` & `ovs-cluster-agent-2.2.3rc1/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/tests/test_main.py` & `ovs-cluster-agent-2.2.3rc1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ovs-cluster-agent-2.2.3/tests/test_settings.py` & `ovs-cluster-agent-2.2.3rc1/tests/test_settings.py`

 * *Files identical despite different names*

