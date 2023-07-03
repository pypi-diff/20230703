# Comparing `tmp/python-gerrit-api-3.0.0.tar.gz` & `tmp/python-gerrit-api-3.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-gerrit-api-3.0.0.tar", last modified: Mon Jul  3 14:03:25 2023, max compression
+gzip compressed data, was "python-gerrit-api-3.0.0.dev1.tar", last modified: Fri Jun 30 15:46:47 2023, max compression
```

## Comparing `python-gerrit-api-3.0.0.tar` & `python-gerrit-api-3.0.0.dev1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:03:25.851405 python-gerrit-api-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11011 2023-07-03 14:03:25.851405 python-gerrit-api-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:03:25.835405 python-gerrit-api-3.0.0/gerrit/
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:03:25.835405 python-gerrit-api-3.0.0/gerrit/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18363 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/accounts/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/accounts/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/accounts/emails.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/accounts/gpg_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/accounts/ssh_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:03:25.839405 python-gerrit-api-3.0.0/gerrit/changes/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/changes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27452 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/changes/change.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/changes/changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/changes/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/changes/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/changes/reviewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:03:25.839405 python-gerrit-api-3.0.0/gerrit/changes/revision/
--rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/changes/revision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/changes/revision/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/changes/revision/drafts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/changes/revision/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:03:25.839405 python-gerrit-api-3.0.0/gerrit/config/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/config/caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/config/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:03:25.843405 python-gerrit-api-3.0.0/gerrit/groups/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/groups/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/groups/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/groups/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/groups/subgroups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:03:25.843405 python-gerrit-api-3.0.0/gerrit/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/plugins/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:03:25.843405 python-gerrit-api-3.0.0/gerrit/projects/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/projects/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/projects/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/projects/dashboards.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/projects/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/projects/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/projects/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/projects/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/projects/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:03:25.847405 python-gerrit-api-3.0.0/gerrit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/utils/gerritbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gerrit/utils/requester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:03:25.847405 python-gerrit-api-3.0.0/gitiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/gitiles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:03:25.847405 python-gerrit-api-3.0.0/python_gerrit_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11011 2023-07-03 14:03:25.000000 python-gerrit-api-3.0.0/python_gerrit_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-03 14:03:25.000000 python-gerrit-api-3.0.0/python_gerrit_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:03:25.000000 python-gerrit-api-3.0.0/python_gerrit_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 14:03:25.000000 python-gerrit-api-3.0.0/python_gerrit_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 14:03:25.000000 python-gerrit-api-3.0.0/python_gerrit_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 14:03:25.851405 python-gerrit-api-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:03:25.851405 python-gerrit-api-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/tests/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/tests/test_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/tests/test_gitiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/tests/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-07-03 14:03:13.000000 python-gerrit-api-3.0.0/tests/test_revision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.369120 python-gerrit-api-3.0.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-30 15:46:47.369120 python-gerrit-api-3.0.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.353120 python-gerrit-api-3.0.0.dev1/gerrit/
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.357120 python-gerrit-api-3.0.0.dev1/gerrit/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18363 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/accounts/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/accounts/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/accounts/emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/accounts/gpg_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/accounts/ssh_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.357120 python-gerrit-api-3.0.0.dev1/gerrit/changes/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27452 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/reviewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.357120 python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/
+-rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/drafts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.357120 python-gerrit-api-3.0.0.dev1/gerrit/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/config/caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/config/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.361120 python-gerrit-api-3.0.0.dev1/gerrit/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/groups/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/groups/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/groups/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/groups/subgroups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.361120 python-gerrit-api-3.0.0.dev1/gerrit/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/plugins/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.361120 python-gerrit-api-3.0.0.dev1/gerrit/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.365120 python-gerrit-api-3.0.0.dev1/gerrit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/utils/gerritbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/utils/requester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.365120 python-gerrit-api-3.0.0.dev1/gitiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gitiles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.365120 python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-30 15:46:47.000000 python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-30 15:46:47.000000 python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:46:47.000000 python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-30 15:46:47.000000 python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-30 15:46:47.000000 python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 15:46:47.369120 python-gerrit-api-3.0.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.369120 python-gerrit-api-3.0.0.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/tests/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/tests/test_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/tests/test_gitiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/tests/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/tests/test_revision.py
```

### Comparing `python-gerrit-api-3.0.0/LICENSE` & `python-gerrit-api-3.0.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/PKG-INFO` & `python-gerrit-api-3.0.0.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gerrit-api
-Version: 3.0.0
+Version: 3.0.0.dev1
 Summary: Python wrapper for the Gerrit REST API.
 Home-page: https://github.com/shijl0925/python-gerrit-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: MIT
 Keywords: api gerrit client wrapper
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python-gerrit-api-3.0.0/README.rst` & `python-gerrit-api-3.0.0.dev1/README.rst`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/__init__.py` & `python-gerrit-api-3.0.0.dev1/gerrit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-__version__ = "3.0.0"
+__version__ = "3.0.0.dev1"
 
 import netrc
 from gerrit.utils.requester import Requester
 from gerrit.utils.common import (
     decode_response,
     strip_trailing_slash
 )
```

### Comparing `python-gerrit-api-3.0.0/gerrit/accounts/account.py` & `python-gerrit-api-3.0.0.dev1/gerrit/accounts/account.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/accounts/accounts.py` & `python-gerrit-api-3.0.0.dev1/gerrit/accounts/accounts.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/accounts/emails.py` & `python-gerrit-api-3.0.0.dev1/gerrit/accounts/emails.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/accounts/gpg_keys.py` & `python-gerrit-api-3.0.0.dev1/gerrit/accounts/gpg_keys.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/accounts/ssh_keys.py` & `python-gerrit-api-3.0.0.dev1/gerrit/accounts/ssh_keys.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/changes/change.py` & `python-gerrit-api-3.0.0.dev1/gerrit/changes/change.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/changes/changes.py` & `python-gerrit-api-3.0.0.dev1/gerrit/changes/changes.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/changes/edit.py` & `python-gerrit-api-3.0.0.dev1/gerrit/changes/edit.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/changes/messages.py` & `python-gerrit-api-3.0.0.dev1/gerrit/changes/messages.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/changes/reviewers.py` & `python-gerrit-api-3.0.0.dev1/gerrit/changes/reviewers.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/changes/revision/__init__.py` & `python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/__init__.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/changes/revision/comments.py` & `python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/comments.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/changes/revision/drafts.py` & `python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/drafts.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/changes/revision/files.py` & `python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/files.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/config/caches.py` & `python-gerrit-api-3.0.0.dev1/gerrit/config/caches.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/config/config.py` & `python-gerrit-api-3.0.0.dev1/gerrit/config/config.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/config/tasks.py` & `python-gerrit-api-3.0.0.dev1/gerrit/config/tasks.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/groups/group.py` & `python-gerrit-api-3.0.0.dev1/gerrit/groups/group.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/groups/groups.py` & `python-gerrit-api-3.0.0.dev1/gerrit/groups/groups.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/groups/members.py` & `python-gerrit-api-3.0.0.dev1/gerrit/groups/members.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/groups/subgroups.py` & `python-gerrit-api-3.0.0.dev1/gerrit/groups/subgroups.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/plugins/plugins.py` & `python-gerrit-api-3.0.0.dev1/gerrit/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/projects/branches.py` & `python-gerrit-api-3.0.0.dev1/gerrit/projects/branches.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/projects/commit.py` & `python-gerrit-api-3.0.0.dev1/gerrit/projects/commit.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/projects/dashboards.py` & `python-gerrit-api-3.0.0.dev1/gerrit/projects/dashboards.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/projects/labels.py` & `python-gerrit-api-3.0.0.dev1/gerrit/projects/labels.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/projects/project.py` & `python-gerrit-api-3.0.0.dev1/gerrit/projects/project.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/projects/projects.py` & `python-gerrit-api-3.0.0.dev1/gerrit/projects/projects.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/projects/tags.py` & `python-gerrit-api-3.0.0.dev1/gerrit/projects/tags.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/projects/webhooks.py` & `python-gerrit-api-3.0.0.dev1/gerrit/projects/webhooks.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/utils/common.py` & `python-gerrit-api-3.0.0.dev1/gerrit/utils/common.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/utils/exceptions.py` & `python-gerrit-api-3.0.0.dev1/gerrit/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/utils/gerritbase.py` & `python-gerrit-api-3.0.0.dev1/gerrit/utils/gerritbase.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gerrit/utils/requester.py` & `python-gerrit-api-3.0.0.dev1/gerrit/utils/requester.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/gitiles/__init__.py` & `python-gerrit-api-3.0.0.dev1/gitiles/__init__.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/python_gerrit_api.egg-info/PKG-INFO` & `python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gerrit-api
-Version: 3.0.0
+Version: 3.0.0.dev1
 Summary: Python wrapper for the Gerrit REST API.
 Home-page: https://github.com/shijl0925/python-gerrit-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: MIT
 Keywords: api gerrit client wrapper
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python-gerrit-api-3.0.0/python_gerrit_api.egg-info/SOURCES.txt` & `python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/setup.py` & `python-gerrit-api-3.0.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/tests/test_accounts.py` & `python-gerrit-api-3.0.0.dev1/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/tests/test_changes.py` & `python-gerrit-api-3.0.0.dev1/tests/test_changes.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/tests/test_gitiles.py` & `python-gerrit-api-3.0.0.dev1/tests/test_gitiles.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/tests/test_groups.py` & `python-gerrit-api-3.0.0.dev1/tests/test_groups.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/tests/test_projects.py` & `python-gerrit-api-3.0.0.dev1/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.0/tests/test_revision.py` & `python-gerrit-api-3.0.0.dev1/tests/test_revision.py`

 * *Files identical despite different names*

