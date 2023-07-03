# Comparing `tmp/roboto_sdk-0.1.3a1.tar.gz` & `tmp/roboto_sdk-0.1.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboto_sdk-0.1.3a1.tar", max compression
+gzip compressed data, was "roboto_sdk-0.1.3a2.tar", max compression
```

## Comparing `roboto_sdk-0.1.3a1.tar` & `roboto_sdk-0.1.3a2.tar`

### file list

```diff
@@ -1,86 +1,87 @@
--rw-r--r--   0        0        0       22 2023-05-31 20:34:51.104994 roboto_sdk-0.1.3a1/README.md
--rw-r--r--   0        0        0      950 2023-06-30 22:24:22.193303 roboto_sdk-0.1.3a1/pyproject.toml
--rw-r--r--   0        0        0       62 2023-05-31 20:34:51.105420 roboto_sdk-0.1.3a1/src/roboto_sdk/__init__.py
--rw-r--r--   0        0        0       48 2023-05-31 20:51:22.684541 roboto_sdk-0.1.3a1/src/roboto_sdk/auth/__init__.py
--rw-r--r--   0        0        0     4034 2023-06-30 22:13:00.631826 roboto_sdk-0.1.3a1/src/roboto_sdk/auth/pat.py
--rw-r--r--   0        0        0      132 2023-05-31 21:34:25.532839 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/__init__.py
--rw-r--r--   0        0        0      334 2023-06-21 21:00:10.362037 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/command/__init__.py
--rw-r--r--   0        0        0     1182 2023-06-21 21:02:17.537089 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/command/args.py
--rw-r--r--   0        0        0     2033 2023-06-21 21:18:40.940344 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/command/model.py
--rw-r--r--   0        0        0      790 2023-06-29 16:05:04.384582 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/context.py
--rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/datasets/__init__.py
--rw-r--r--   0        0        0     6691 2023-06-29 16:05:04.385345 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/datasets/commands.py
--rw-r--r--   0        0        0     3584 2023-06-30 22:13:00.626079 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/entry.py
--rw-r--r--   0        0        0      108 2023-06-21 21:18:40.926071 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/help/__init__.py
--rw-r--r--   0        0        0      167 2023-06-21 21:18:40.928579 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/help/args.py
--rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/orgs/__init__.py
--rw-r--r--   0        0        0     3386 2023-06-28 22:21:48.431065 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/orgs/commands.py
--rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/tokens/__init__.py
--rw-r--r--   0        0        0     3301 2023-06-27 00:52:24.673209 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/tokens/commands.py
--rw-r--r--   0        0        0      110 2023-06-21 18:17:36.115870 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/triggers/__init__.py
--rw-r--r--   0        0        0     2874 2023-06-21 21:18:41.332847 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/triggers/commands.py
--rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/users/__init__.py
--rw-r--r--   0        0        0      733 2023-06-23 21:06:13.848323 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/users/commands.py
--rw-r--r--   0        0        0       48 2023-06-21 18:17:36.116077 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/__init__.py
--rw-r--r--   0        0        0     1633 2023-06-29 15:35:56.463310 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/__init__.py
--rw-r--r--   0        0        0     7019 2023-06-29 15:35:56.463411 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/action.py
--rw-r--r--   0        0        0     2804 2023-06-29 15:35:56.463471 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/action_delegate.py
--rw-r--r--   0        0        0     5167 2023-06-29 15:35:56.463534 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/action_http_delegate.py
--rw-r--r--   0        0        0      651 2023-06-29 15:35:56.463581 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/action_http_resources.py
--rw-r--r--   0        0        0      792 2023-06-29 15:35:56.463632 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/action_record.py
--rw-r--r--   0        0        0      106 2023-06-29 15:35:56.463681 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/error.py
--rw-r--r--   0        0        0     4294 2023-06-29 15:35:56.463871 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/invocation.py
--rw-r--r--   0        0        0     1653 2023-06-29 15:35:56.463945 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/invocation_delegate.py
--rw-r--r--   0        0        0     4684 2023-06-29 15:35:56.464027 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/invocation_http_delegate.py
--rw-r--r--   0        0        0      534 2023-06-29 15:35:56.464078 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/invocation_http_resources.py
--rw-r--r--   0        0        0     1592 2023-06-29 15:35:56.464142 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/invocation_record.py
--rw-r--r--   0        0        0      546 2023-06-29 15:35:56.464218 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/datasets/__init__.py
--rw-r--r--   0        0        0     9572 2023-06-29 15:35:56.464288 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/datasets/dataset.py
--rw-r--r--   0        0        0     2132 2023-06-29 15:35:56.464354 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/datasets/delegate.py
--rw-r--r--   0        0        0     4759 2023-06-29 15:35:56.464409 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/datasets/http_delegate.py
--rw-r--r--   0        0        0      340 2023-06-29 15:35:56.464452 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/datasets/http_resources.py
--rw-r--r--   0        0        0      817 2023-06-29 15:35:56.464498 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/datasets/record.py
--rw-r--r--   0        0        0      436 2023-06-29 15:35:56.464570 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/files/__init__.py
--rw-r--r--   0        0        0     1156 2023-06-29 15:35:56.464729 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/files/delegate.py
--rw-r--r--   0        0        0      771 2023-06-29 15:35:56.464889 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/files/file.py
--rw-r--r--   0        0        0     2110 2023-06-29 15:35:56.464947 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/files/http_delegate.py
--rw-r--r--   0        0        0      168 2023-06-29 15:35:56.464990 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/files/http_resources.py
--rw-r--r--   0        0        0      385 2023-06-29 15:35:56.465086 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/files/record.py
--rw-r--r--   0        0        0     2320 2023-06-29 15:35:56.465141 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/files/s3_delegate.py
--rw-r--r--   0        0        0      633 2023-06-29 21:05:11.294925 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/__init__.py
--rw-r--r--   0        0        0     1620 2023-06-29 00:30:17.060813 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/delegate.py
--rw-r--r--   0        0        0     3610 2023-06-29 00:30:17.061047 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/http_delegate.py
--rw-r--r--   0        0        0      359 2023-06-28 06:35:03.341928 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/http_resources.py
--rw-r--r--   0        0        0     2381 2023-06-29 00:30:17.061322 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/org.py
--rw-r--r--   0        0        0     1145 2023-06-28 21:49:35.087173 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/org_role.py
--rw-r--r--   0        0        0      563 2023-06-29 21:05:11.295549 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/record.py
--rw-r--r--   0        0        0      387 2023-06-23 21:06:13.848727 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/tokens/__init__.py
--rw-r--r--   0        0        0      818 2023-06-27 00:52:24.673479 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/tokens/delegate.py
--rw-r--r--   0        0        0     1968 2023-06-27 00:52:24.673652 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/tokens/http_delegate.py
--rw-r--r--   0        0        0      184 2023-06-27 00:52:24.673821 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/tokens/http_resources.py
--rw-r--r--   0        0        0      412 2023-06-27 00:52:24.673996 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/tokens/record.py
--rw-r--r--   0        0        0     1807 2023-06-27 00:52:24.674186 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/tokens/token.py
--rw-r--r--   0        0        0      391 2023-06-21 18:17:36.116185 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/triggers/__init__.py
--rw-r--r--   0        0        0     2255 2023-06-21 18:17:36.116295 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/triggers/http_delegate.py
--rw-r--r--   0        0        0      205 2023-06-21 18:17:36.116397 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/triggers/http_resources.py
--rw-r--r--   0        0        0     2661 2023-06-29 16:05:04.386157 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/triggers/trigger.py
--rw-r--r--   0        0        0      857 2023-06-21 18:17:36.116610 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/triggers/trigger_delegate.py
--rw-r--r--   0        0        0      249 2023-06-21 18:17:36.116722 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/triggers/trigger_record.py
--rw-r--r--   0        0        0      262 2023-06-23 21:06:13.849582 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/users/__init__.py
--rw-r--r--   0        0        0     1016 2023-06-23 21:17:31.788229 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/users/http_delegate.py
--rw-r--r--   0        0        0     1200 2023-06-23 21:17:31.796065 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/users/user.py
--rw-r--r--   0        0        0      451 2023-06-23 21:17:31.793509 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/users/user_delegate.py
--rw-r--r--   0        0        0      162 2023-06-23 21:06:13.850109 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/users/user_record.py
--rw-r--r--   0        0        0      704 2023-06-29 00:30:17.043102 roboto_sdk-0.1.3a1/src/roboto_sdk/http/__init__.py
--rw-r--r--   0        0        0      216 2023-06-23 21:06:13.850449 roboto_sdk-0.1.3a1/src/roboto_sdk/http/constants.py
--rw-r--r--   0        0        0     8880 2023-06-13 17:13:48.415283 roboto_sdk-0.1.3a1/src/roboto_sdk/http/http_client.py
--rw-r--r--   0        0        0     3127 2023-06-30 22:09:49.535434 roboto_sdk-0.1.3a1/src/roboto_sdk/http/request_decorators.py
--rw-r--r--   0        0        0      994 2023-06-29 00:30:17.043313 roboto_sdk-0.1.3a1/src/roboto_sdk/http/testing_util.py
--rw-r--r--   0        0        0      158 2023-05-31 20:51:22.686567 roboto_sdk-0.1.3a1/src/roboto_sdk/logging.py
--rw-r--r--   0        0        0      211 2023-06-26 18:41:27.400684 roboto_sdk-0.1.3a1/src/roboto_sdk/pagination.py
--rw-r--r--   0        0        0      168 2023-06-25 17:00:28.638279 roboto_sdk-0.1.3a1/src/roboto_sdk/profile/__init__.py
--rw-r--r--   0        0        0     2958 2023-06-30 22:11:44.938691 roboto_sdk-0.1.3a1/src/roboto_sdk/profile/profile.py
--rw-r--r--   0        0        0        0 2023-05-31 20:34:27.418611 roboto_sdk-0.1.3a1/src/roboto_sdk/py.typed
--rw-r--r--   0        0        0      651 2023-06-13 17:13:48.417645 roboto_sdk-0.1.3a1/src/roboto_sdk/serde.py
--rw-r--r--   0        0        0      112 2023-06-01 19:18:26.925334 roboto_sdk-0.1.3a1/src/roboto_sdk/time.py
--rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 roboto_sdk-0.1.3a1/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-05-31 20:34:51.104994 roboto_sdk-0.1.3a2/README.md
+-rw-r--r--   0        0        0      949 2023-07-03 16:21:54.874816 roboto_sdk-0.1.3a2/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-03 16:08:19.143854 roboto_sdk-0.1.3a2/src/roboto_sdk/__init__.py
+-rw-r--r--   0        0        0       48 2023-07-03 16:08:19.141092 roboto_sdk-0.1.3a2/src/roboto_sdk/auth/__init__.py
+-rw-r--r--   0        0        0     4037 2023-07-03 16:08:19.139811 roboto_sdk-0.1.3a2/src/roboto_sdk/auth/pat.py
+-rw-r--r--   0        0        0      132 2023-07-03 16:08:19.152003 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/__init__.py
+-rw-r--r--   0        0        0      334 2023-07-03 16:08:19.162015 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/command/__init__.py
+-rw-r--r--   0        0        0     1182 2023-07-03 16:08:19.164617 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/command/args.py
+-rw-r--r--   0        0        0     2058 2023-07-03 16:28:40.380758 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/command/model.py
+-rw-r--r--   0        0        0      822 2023-07-03 16:28:40.367049 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/context.py
+-rw-r--r--   0        0        0      110 2023-07-03 16:08:19.148587 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/datasets/__init__.py
+-rw-r--r--   0        0        0     6714 2023-07-03 16:08:19.150367 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/datasets/commands.py
+-rw-r--r--   0        0        0     3603 2023-07-03 16:08:19.157982 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/entry.py
+-rw-r--r--   0        0        0      108 2023-07-03 16:08:19.168666 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/help/__init__.py
+-rw-r--r--   0        0        0      167 2023-07-03 16:08:19.169956 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/help/args.py
+-rw-r--r--   0        0        0      110 2023-07-03 16:08:19.153590 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/orgs/__init__.py
+-rw-r--r--   0        0        0     3386 2023-07-03 16:08:19.155109 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/orgs/commands.py
+-rw-r--r--   0        0        0      110 2023-07-03 16:08:19.165930 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/tokens/__init__.py
+-rw-r--r--   0        0        0     3301 2023-07-03 16:08:19.167288 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/tokens/commands.py
+-rw-r--r--   0        0        0      110 2023-07-03 16:08:19.145458 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/triggers/__init__.py
+-rw-r--r--   0        0        0     2874 2023-07-03 16:08:19.147004 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/triggers/commands.py
+-rw-r--r--   0        0        0      110 2023-07-03 16:08:19.159379 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/users/__init__.py
+-rw-r--r--   0        0        0      733 2023-07-03 16:08:19.160698 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/users/commands.py
+-rw-r--r--   0        0        0       48 2023-07-03 16:08:19.198130 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/__init__.py
+-rw-r--r--   0        0        0     1641 2023-07-03 16:08:19.224521 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/__init__.py
+-rw-r--r--   0        0        0     7427 2023-07-03 16:28:40.375211 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/action.py
+-rw-r--r--   0        0        0     3015 2023-07-03 16:28:40.382505 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/action_delegate.py
+-rw-r--r--   0        0        0     5168 2023-07-03 16:28:40.356951 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/action_http_delegate.py
+-rw-r--r--   0        0        0      640 2023-07-03 16:28:40.365100 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/action_http_resources.py
+-rw-r--r--   0        0        0      808 2023-07-03 16:28:40.372147 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/action_record.py
+-rw-r--r--   0        0        0      106 2023-07-03 16:08:19.223131 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/error.py
+-rw-r--r--   0        0        0     4499 2023-07-03 16:28:40.370371 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/invocation.py
+-rw-r--r--   0        0        0     1726 2023-07-03 16:28:40.384071 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/invocation_delegate.py
+-rw-r--r--   0        0        0     4768 2023-07-03 16:28:40.366150 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/invocation_http_delegate.py
+-rw-r--r--   0        0        0      566 2023-07-03 16:30:28.384279 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/invocation_http_resources.py
+-rw-r--r--   0        0        0     1652 2023-07-03 16:30:28.386808 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/invocation_record.py
+-rw-r--r--   0        0        0      546 2023-07-03 16:08:19.192761 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/datasets/__init__.py
+-rw-r--r--   0        0        0     9836 2023-07-03 16:28:40.373480 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/datasets/dataset.py
+-rw-r--r--   0        0        0     2215 2023-07-03 16:28:40.371324 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/datasets/delegate.py
+-rw-r--r--   0        0        0     4911 2023-07-03 16:28:40.387575 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/datasets/http_delegate.py
+-rw-r--r--   0        0        0      340 2023-07-03 16:08:19.190087 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/datasets/http_resources.py
+-rw-r--r--   0        0        0      867 2023-07-03 16:08:19.196854 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/datasets/record.py
+-rw-r--r--   0        0        0      436 2023-07-03 16:08:19.238248 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/files/__init__.py
+-rw-r--r--   0        0        0     1181 2023-07-03 16:28:40.353092 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/files/delegate.py
+-rw-r--r--   0        0        0      802 2023-07-03 16:30:28.392185 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/files/file.py
+-rw-r--r--   0        0        0     2166 2023-07-03 16:30:27.887912 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/files/http_delegate.py
+-rw-r--r--   0        0        0      168 2023-07-03 16:08:19.235599 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/files/http_resources.py
+-rw-r--r--   0        0        0      382 2023-07-03 16:08:19.242205 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/files/record.py
+-rw-r--r--   0        0        0     2358 2023-07-03 16:30:27.887409 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/files/s3_delegate.py
+-rw-r--r--   0        0        0      728 2023-07-03 16:08:19.204997 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/__init__.py
+-rw-r--r--   0        0        0     1893 2023-07-03 16:28:40.348041 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/delegate.py
+-rw-r--r--   0        0        0     4103 2023-07-03 16:28:40.383366 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/http_delegate.py
+-rw-r--r--   0        0        0      359 2023-07-03 16:08:19.200791 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/http_resources.py
+-rw-r--r--   0        0        0     1815 2023-07-03 16:28:40.378431 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/org.py
+-rw-r--r--   0        0        0     1680 2023-07-03 16:28:40.364446 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/org_invite.py
+-rw-r--r--   0        0        0     1158 2023-07-03 16:28:40.351236 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/org_role.py
+-rw-r--r--   0        0        0      722 2023-07-03 16:08:19.209463 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/record.py
+-rw-r--r--   0        0        0      387 2023-07-03 16:08:19.249174 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/tokens/__init__.py
+-rw-r--r--   0        0        0      888 2023-07-03 16:28:40.360553 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/tokens/delegate.py
+-rw-r--r--   0        0        0     2038 2023-07-03 16:28:40.386560 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/tokens/http_delegate.py
+-rw-r--r--   0        0        0      216 2023-07-03 16:30:28.394782 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/tokens/http_resources.py
+-rw-r--r--   0        0        0      455 2023-07-03 16:30:28.399700 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/tokens/record.py
+-rw-r--r--   0        0        0     1832 2023-07-03 16:30:28.395655 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/tokens/token.py
+-rw-r--r--   0        0        0      391 2023-07-03 16:08:19.184598 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/triggers/__init__.py
+-rw-r--r--   0        0        0     2280 2023-07-03 16:28:40.388369 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/triggers/http_delegate.py
+-rw-r--r--   0        0        0      205 2023-07-03 16:08:19.182005 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/triggers/http_resources.py
+-rw-r--r--   0        0        0     2683 2023-07-03 16:28:40.381687 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/triggers/trigger.py
+-rw-r--r--   0        0        0      882 2023-07-03 16:28:40.352187 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/triggers/trigger_delegate.py
+-rw-r--r--   0        0        0      249 2023-07-03 16:08:19.188733 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/triggers/trigger_record.py
+-rw-r--r--   0        0        0      262 2023-07-03 16:08:19.215749 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/users/__init__.py
+-rw-r--r--   0        0        0     1051 2023-07-03 16:28:40.361652 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/users/http_delegate.py
+-rw-r--r--   0        0        0     1213 2023-07-03 16:28:40.362745 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/users/user.py
+-rw-r--r--   0        0        0      485 2023-07-03 16:28:40.384945 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/users/user_delegate.py
+-rw-r--r--   0        0        0      194 2023-07-03 16:30:28.374240 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/users/user_record.py
+-rw-r--r--   0        0        0      704 2023-07-03 16:08:19.177982 roboto_sdk-0.1.3a2/src/roboto_sdk/http/__init__.py
+-rw-r--r--   0        0        0      216 2023-07-03 16:08:19.176698 roboto_sdk-0.1.3a2/src/roboto_sdk/http/constants.py
+-rw-r--r--   0        0        0     9060 2023-07-03 16:28:40.379809 roboto_sdk-0.1.3a2/src/roboto_sdk/http/http_client.py
+-rw-r--r--   0        0        0     3161 2023-07-03 16:30:28.347765 roboto_sdk-0.1.3a2/src/roboto_sdk/http/request_decorators.py
+-rw-r--r--   0        0        0     1004 2023-07-03 16:28:40.363668 roboto_sdk-0.1.3a2/src/roboto_sdk/http/testing_util.py
+-rw-r--r--   0        0        0      158 2023-07-03 16:08:19.138394 roboto_sdk-0.1.3a2/src/roboto_sdk/logging.py
+-rw-r--r--   0        0        0      224 2023-07-03 16:30:28.318993 roboto_sdk-0.1.3a2/src/roboto_sdk/pagination.py
+-rw-r--r--   0        0        0      168 2023-07-03 16:08:19.172598 roboto_sdk-0.1.3a2/src/roboto_sdk/profile/__init__.py
+-rw-r--r--   0        0        0     2977 2023-07-03 16:28:40.376360 roboto_sdk-0.1.3a2/src/roboto_sdk/profile/profile.py
+-rw-r--r--   0        0        0        0 2023-05-31 20:34:27.418611 roboto_sdk-0.1.3a2/src/roboto_sdk/py.typed
+-rw-r--r--   0        0        0      651 2023-07-03 16:08:19.142504 roboto_sdk-0.1.3a2/src/roboto_sdk/serde.py
+-rw-r--r--   0        0        0      112 2023-07-03 16:08:19.137067 roboto_sdk-0.1.3a2/src/roboto_sdk/time.py
+-rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 roboto_sdk-0.1.3a2/PKG-INFO
```

### Comparing `roboto_sdk-0.1.3a1/pyproject.toml` & `roboto_sdk-0.1.3a2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 requires-python = ">=3.10"
 # Ignore this version attribute, it is here to satisfy setuptools.
 # The actual version is set by Poetry in the [tool.poetry] section.
 version = "0.0.0"
 
 [tool.poetry]
 name = "roboto_sdk"
-version = "0.1.3a1"
+version = "0.1.3a2"
 description = "Tools for interacting with roboto.ai"
 license = "MIT"
 readme = "README.md"
 authors = ["Roboto <admin@roboto.ai>"]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 boto3 = {extras = ["crt"], version = "~1.26"}
 pathspec = "~0.11"
 pydantic = "~1.10"
 tenacity = "~8.2"
 pyjwt = "~2.7"
 
 # While Poetry is used for dependency and venv management,
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/auth/pat.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/auth/pat.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     _expires: datetime.datetime
     _id_token: Optional[str]
     _profile: RobotoProfile
 
     def __init__(
         self,
         client_id: str,
-        cognito: Any | None = None,
+        cognito: Optional[Any] = None,
         profile: RobotoProfile = RobotoProfile(),
     ):
         self._client_id = client_id
         self._cognito = (
             cognito
             if cognito is not None
             else boto3.client("cognito-idp", region_name="us-west-2")
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/cli/command/args.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/cli/command/args.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/cli/command/model.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/cli/command/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 import argparse
-from typing import Any, Callable
+from typing import Any, Callable, Optional
 
 from ..context import CLIContext
 
 
 class RobotoCommand(object):
     _name: str
     _logic: Callable[
         [Any, CLIContext, argparse.ArgumentParser], None
     ]  # Args, CLIContext
-    _inner_setup_parser: Callable[[Any], None] | None  # Parser
-    _command_kwargs: dict[str, Any] | None
+    _inner_setup_parser: Optional[Callable[[Any], None]]  # Parser
+    _command_kwargs: Optional[dict[str, Any]]
 
     def __init__(
         self,
         name: str,
         logic: Callable[[Any, CLIContext, argparse.ArgumentParser], None],
-        command_kwargs: dict | None,
-        setup_parser: Callable[[Any], None] | None = None,
+        command_kwargs: Optional[dict],
+        setup_parser: Optional[Callable[[Any], None]] = None,
     ):
         self._name = name
         self._logic = logic
         self._inner_setup_parser = setup_parser
         self._command_kwargs = command_kwargs
 
     @property
@@ -44,15 +44,15 @@
             self._inner_setup_parser(parser)
 
 
 class RobotoCommandSet(object):
     _name: str
     _help: str
     _commands: list[RobotoCommand]
-    _context: CLIContext | None
+    _context: Optional[CLIContext]
 
     def __init__(self, name, help, commands):
         self._name = name
         self._help = help
         self._commands = commands
 
     def add_to_subparsers(self, parent_subparsers, context: CLIContext):
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/cli/context.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/cli/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
+from typing import Optional
+
 from ..domain.actions import ActionDelegate
 from ..domain.datasets import DatasetDelegate
 from ..domain.orgs import OrgDelegate
 from ..domain.tokens import TokenDelegate
 from ..domain.triggers import TriggerDelegate
 from ..http import HttpClient
 
 
 class CLIContext:
-    _http: HttpClient | None
+    _http: Optional[HttpClient]
     datasets: DatasetDelegate
     orgs: OrgDelegate
     tokens: TokenDelegate
     triggers: TriggerDelegate
     actions: ActionDelegate
 
     @property
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/cli/datasets/commands.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/cli/datasets/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,36 +23,38 @@
     )
 
     sys.stdout.write(json.dumps(record.to_dict()) + "\n")
 
 
 def create_setup_parser(parser):
     parser.add_argument(
-        "-m" "--metadata",
+        "-m",
+        "--metadata",
         metavar="KEY=VALUE",
         nargs="*",
         action=KeyValuePairsAction,
         help="Zero or more 'key=value' format key/value pairs which represent dataset metadata. "
         + "Metadata can be mutated after creation.",
     )
     parser.add_argument(
-        "-t" "--tag",
+        "-t",
+        "--tag",
         type=str,
         nargs="*",
         help="One or more tags to annotate this dataset. Tags can be modified after creation.",
         action="extend",
     )
     parser.add_argument("-o", "--org", type=str, help=ORG_ARG_HELP)
 
 
 def get(args, context: CLIContext, parser: argparse.ArgumentParser):
-    record = Dataset.by_id(
+    record = Dataset.from_id(
         dataset_delegate=context.datasets,
         dataset_id=args.dataset_id,
-        tenant_id=args.org,
+        org_id=args.org,
     )
     sys.stdout.write(json.dumps(record.to_dict()) + "\n")
 
 
 def get_setup_parser(parser):
     parser.add_argument(
         "-d", "--dataset-id", type=str, required=True, help=DATASET_ARG_HELP
@@ -75,15 +77,15 @@
         action=KeyValuePairsAction,
         help="Zero or more 'key=value' formatted conditions which will perform equality checks against "
         + "datasets and filter results accordingly.",
     )
 
 
 def list_files(args, context: CLIContext, parser: argparse.ArgumentParser):
-    record = Dataset.by_id(
+    record = Dataset.from_id(
         dataset_delegate=context.datasets,
         dataset_id=args.dataset_id,
     )
 
     for f in record.list_files():
         sys.stdout.write(f"{f.relative_path}\n")
 
@@ -101,15 +103,15 @@
             "Exclude filters are only supported for directory uploads, not single files."
         )
     if args.key is not None and path.is_dir():
         parser.error(
             "Key overrides are only supported for single file uploads, now directories."
         )
 
-    record = Dataset.by_id(
+    record = Dataset.from_id(
         dataset_delegate=context.datasets,
         dataset_id=args.dataset_id,
     )
 
     if path.is_dir():
         record.upload_directory(directory_path=path, exclude_patterns=args.exclude)
     else:
@@ -139,15 +141,15 @@
         type=str,
         nargs="*",
         help="Zero or more exclude filters (if path points to a directory)",
     )
 
 
 def download_files(args, context: CLIContext, parser: argparse.ArgumentParser):
-    record = Dataset.by_id(
+    record = Dataset.from_id(
         dataset_delegate=context.datasets,
         dataset_id=args.dataset_id,
     )
 
     record.download_files(
         out_path=args.path, include_patterns=args.include, exclude_patterns=args.exclude
     )
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/cli/entry.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/cli/entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,22 +46,24 @@
 
 def __populate_context(args, context: CLIContext):
     profile = (
         RobotoProfile()
         if args.config_file is None
         else RobotoProfile(config_file=args.config_file)
     )
+
     profile_entry = profile.get_entry()
+
     http_client_args: dict[str, Any] = {
         "default_endpoint": profile_entry.default_endpoint
     }
 
     if "localhost" not in profile_entry.default_endpoint:
         http_client_args["default_auth"] = PATAuthDecorator.for_client(
-            client_id=profile_entry.default_client_id
+            client_id=profile_entry.default_client_id, profile=profile
         )
     else:
         http_client_args["default_auth"] = LocalAuthDecorator(
             user_id=profile_entry.user_id
         )
 
     http = HttpClient(**http_client_args)  # type: ignore[arg-type]
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/cli/orgs/commands.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/cli/orgs/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/cli/tokens/commands.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/cli/tokens/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/cli/triggers/commands.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/cli/triggers/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/cli/users/commands.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/cli/users/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/__init__.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     CreateInvocationRequest,
     SetLogsLocationRequest,
     UpdateInvocationStatus,
 )
 from .invocation_record import (
     InvocationDataSource,
     InvocationDataSourceType,
-    InvocationDetail,
+    InvocationProvenance,
     InvocationRecord,
     InvocationSource,
     InvocationStatus,
     InvocationStatusRecord,
 )
 
 __all__ = (
@@ -50,17 +50,17 @@
     "ContainerUploadCredentials",
     "CreateActionRequest",
     "CreateInvocationRequest",
     "Invocation",
     "InvocationDataSource",
     "InvocationDataSourceType",
     "InvocationDelegate",
-    "InvocationDetail",
     "InvocationError",
     "InvocationHttpDelegate",
+    "InvocationProvenance",
     "InvocationRecord",
     "InvocationSource",
     "InvocationStatus",
     "InvocationStatusRecord",
     "SetLogsLocationRequest",
     "UpdateActionRequest",
     "UpdateCondition",
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/action_delegate.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/action_delegate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import abc
 import datetime
-from typing import Any, Literal
+from typing import Any, Literal, Optional
 
 import pydantic
 
 from ...pagination import PaginatedList
 from ...serde import pydantic_jsonable_dict
 from ...time import utcnow
 from .action_record import ActionRecord
@@ -41,54 +41,58 @@
 
 
 class ActionDelegate(abc.ABC):
     @abc.abstractmethod
     def create_action(
         self,
         name: str,
-        tenant_id: str | None = None,
-        created_by: str | None = None,
-        description: str | None = None,
-        metadata: dict[str, Any] | None = None,
-        tags: list[str] | None = None,
+        org_id: Optional[str] = None,
+        created_by: Optional[str] = None,  # A Roboto user_id
+        description: Optional[str] = None,
+        metadata: Optional[dict[str, Any]] = None,
+        tags: Optional[list[str]] = None,
     ) -> ActionRecord:
         raise NotImplementedError("create_action")
 
     @abc.abstractmethod
     def get_action_by_primary_key(
-        self, name: str, tenant_id: str | None = None
+        self, name: str, org_id: Optional[str] = None
     ) -> ActionRecord:
         raise NotImplementedError("get_action_by_primary_key")
 
     @abc.abstractmethod
     def register_container(
         self,
         record: ActionRecord,
         image_name: str,
         image_tag: str,
-        caller: str | None = None,
+        caller: Optional[str] = None,  # A Roboto user_id
     ) -> tuple[str, str]:
         raise NotImplementedError("register_container")
 
     @abc.abstractmethod
     def get_temp_container_credentials(
         self,
         record: ActionRecord,
-        caller: str | None = None,
+        caller: Optional[str] = None,  # A Roboto user_id
     ) -> ContainerCredentials:
         raise NotImplementedError("get_temp_container_credentials")
 
     @abc.abstractmethod
     def query_actions(
-        self, filters: dict[str, Any], page_token: dict[str, str] | None = None
+        self,
+        filters: dict[str, Any],
+        org_id: Optional[str] = None,
+        page_token: Optional[dict[str, str]] = None,
     ) -> PaginatedList[ActionRecord]:
         raise NotImplementedError("query_actions")
 
     @abc.abstractmethod
     def update(
         self,
         record: ActionRecord,
         updates: dict[str, Any],
-        conditions: list[UpdateCondition] | None,
-        tenant_id: str | None = None,
+        conditions: Optional[list[UpdateCondition]],
+        org_id: Optional[str] = None,
+        updated_by: Optional[str] = None,  # A Roboto user_id
     ) -> ActionRecord:
         raise NotImplementedError("update")
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/action_http_delegate.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/action_http_delegate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import http
 import json
-from typing import Any
+from typing import Any, Optional
 
-from ...http import ClientError, HttpClient
+from ...http import (
+    ORG_OVERRIDE_HEADER,
+    USER_OVERRIDE_HEADER,
+    ClientError,
+    HttpClient,
+)
 from ...logging import default_logger
 from ...pagination import PaginatedList
 from ...serde import pydantic_jsonable_dict
 from .action_delegate import (
     ActionDelegate,
     ContainerCredentials,
     UpdateCondition,
@@ -32,117 +37,119 @@
     __roboto_service_base_url: str
 
     def __init__(self, roboto_service_base_url: str, http_client: HttpClient) -> None:
         super().__init__()
         self.__http_client = http_client
         self.__roboto_service_base_url = roboto_service_base_url
 
+    def headers(
+        self, org_id: Optional[str] = None, user_id: Optional[str] = None
+    ) -> dict[str, str]:
+        headers = {"Content-Type": "application/json"}
+        if org_id:
+            headers[ORG_OVERRIDE_HEADER] = org_id
+        if user_id:
+            headers[USER_OVERRIDE_HEADER] = user_id
+        return headers
+
     def create_action(
         self,
         name: str,
-        tenant_id: str | None = None,
-        created_by: str | None = None,
-        description: str | None = None,
-        metadata: dict[str, Any] | None = None,
-        tags: list[str] | None = None,
+        org_id: Optional[str] = None,
+        created_by: Optional[str] = None,
+        description: Optional[str] = None,
+        metadata: Optional[dict[str, Any]] = None,
+        tags: Optional[list[str]] = None,
     ) -> ActionRecord:
-        """
-        `tenant_id` and `created_by` are ignored, as both are determined server-side by the identity of the caller.
-        """
         url = f"{self.__roboto_service_base_url}/v1/actions"
         request_body = CreateActionRequest(
             name=name,
             description=description,
             metadata=metadata,
             tags=tags,
         )
         response = self.__http_client.post(
             url,
             data=pydantic_jsonable_dict(request_body, exclude_none=True),
-            headers={"Content-Type": "application/json", "X-Roboto-Org-Id": tenant_id},
+            headers=self.headers(org_id, created_by),
         )
         return ActionRecord.parse_obj(response.from_json(json_path=["data"]))
 
     def get_action_by_primary_key(
-        self, name: str, tenant_id: str | None = None
+        self, name: str, org_id: Optional[str] = None
     ) -> ActionRecord:
-        """
-        `tenant_id` is ignored, as it is determined server-side by the identity of the caller.
-        """
         url = f"{self.__roboto_service_base_url}/v1/actions/{name}"
-        headers = {}
-        if tenant_id:
-            headers["X-Roboto-Org-Id"] = tenant_id
-        res = self.__http_client.get(url, headers=headers)
+        res = self.__http_client.get(url, headers=self.headers(org_id))
         return ActionRecord.parse_obj(res.from_json(json_path=["data"]))
 
     def register_container(
         self,
         record: ActionRecord,
         image_name: str,
         image_tag: str,
-        caller: str | None = None,
+        caller: Optional[str] = None,
     ) -> tuple[str, str]:
         url = f"{self.__roboto_service_base_url}/v1/actions/{record.name}/container"
         data = {
             "image_name": image_name,
             "image_tag": image_tag,
         }
 
         res = self.__http_client.put(
-            url, data=data, headers={"Content-Type": "application/json"}
+            url, data=data, headers=self.headers(user_id=caller)
         )
         parsed_res = res.from_json(json_path=["data"])
         return (parsed_res["repository_uri"], parsed_res["image_uri"])
 
     def get_temp_container_credentials(
         self,
         record: ActionRecord,
-        caller: str | None = None,
+        caller: Optional[str] = None,
     ) -> ContainerCredentials:
         url = f"{self.__roboto_service_base_url}/v1/actions/{record.name}/container/credentials"
-        res = self.__http_client.get(url)
+        res = self.__http_client.get(url, headers=self.headers(user_id=caller))
         return ContainerCredentials.parse_obj(res.from_json(json_path=["data"]))
 
     def query_actions(
-        self, filters: dict[str, Any], page_token: dict[str, str] | None = None
+        self,
+        filters: dict[str, Any],
+        org_id: Optional[str] = None,
+        page_token: Optional[dict[str, str]] = None,
     ) -> PaginatedList[ActionRecord]:
         if page_token:
             filters["page_token"] = page_token
 
         safe_filters = json.loads(json.dumps(filters))
         url = f"{self.__roboto_service_base_url}/v1/actions/query"
         res = self.__http_client.post(
-            url, data=safe_filters, headers={"Content-Type": "application/json"}
+            url, data=safe_filters, headers=self.headers(org_id)
         )
         unmarshalled = res.from_json(json_path=["data"])
         return PaginatedList(
             items=[
                 ActionRecord.parse_obj(dataset) for dataset in unmarshalled["items"]
             ],
             next_token=unmarshalled["next_token"],
         )
 
     def update(
         self,
         record: ActionRecord,
         updates: dict[str, Any],
-        conditions: list[UpdateCondition] | None,
-        tenant_id: str | None = None,
+        conditions: Optional[list[UpdateCondition]],
+        org_id: Optional[str] = None,
+        updated_by: Optional[str] = None,
     ) -> ActionRecord:
-        """
-        For most requests, `tenant_id` is ignored, as it is determined server-side by the identity of the caller.
-        It is only ever user when the caller is a Roboto service user.
-        """
         url = f"{self.__roboto_service_base_url}/v1/actions/{record.name}"
         payload = UpdateActionRequest(
             updates=updates,
             conditions=conditions if conditions is not None else [],
-            tenant_id=tenant_id,
         )
         try:
-            res = self.__http_client.patch(url, data=payload.dict())
+            res = self.__http_client.patch(
+                url, data=payload.dict(), headers=self.headers(org_id, updated_by)
+            )
             return ActionRecord.parse_obj(res.from_json(json_path=["data"]))
         except ClientError as exc:
             if exc.status == http.HTTPStatus.CONFLICT:
                 raise ActionUpdateConditionCheckFailure(exc.msg) from None
             raise
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/action_http_resources.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/action_http_resources.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-from typing import Any
+from typing import Any, Optional
 
 import pydantic
 
 from .action_delegate import UpdateCondition
 
 
 class CreateActionRequest(pydantic.BaseModel):
     # Required
     name: str
 
     # Optional
-    description: str | None = None
-    metadata: dict[str, Any] | None = pydantic.Field(default_factory=dict)
-    tags: list[str] | None = pydantic.Field(default_factory=list)
+    description: Optional[str] = None
+    metadata: Optional[dict[str, Any]] = pydantic.Field(default_factory=dict)
+    tags: Optional[list[str]] = pydantic.Field(default_factory=list)
 
 
 class ContainerUploadCredentials(pydantic.BaseModel):
     username: str
     password: str
     registry_url: str
     image_uri: str
 
 
 class UpdateActionRequest(pydantic.BaseModel):
     updates: dict[str, Any]
-    conditions: list[UpdateCondition] | None = None
-    tenant_id: str | None = None
+    conditions: Optional[list[UpdateCondition]] = None
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/action_record.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/action_record.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import datetime
-from typing import Any
+from typing import Any, Optional
 
 import pydantic
 
 
 class ActionRecord(pydantic.BaseModel):
     """
-    Actions are unique by their tenant_id and name.
+    Actions are unique by their org_id and name.
 
     Note: update Action.DISALLOWED_FOR_UPDATE if necessary when adding/updating/removing fields.
     """
 
     created: datetime.datetime  # Persisted as ISO 8601 string in UTC
     created_by: str
     modified: datetime.datetime  # Persisted as ISO 8601 string in UTC
     modified_by: str
     name: str  # Sort key
-    tenant_id: str  # Partition key
+    org_id: str  # Partition key
 
-    description: str | None = None
+    description: Optional[str] = None
     # Linked to `uri`; an Action may have a URI set but the container expected at that URI may not be available
     is_available: bool = False
-    metadata: dict[str, Any] | None = None
-    tags: list[str] | None = None
-    uri: str | None = None
+    metadata: Optional[dict[str, Any]] = None
+    tags: Optional[list[str]] = None
+    uri: Optional[str] = None
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/invocation.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/invocation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import collections.abc
-from typing import Any
+from typing import Any, Optional
 
 from ...serde import pydantic_jsonable_dict
 from .invocation_delegate import (
     InvocationDelegate,
 )
 from .invocation_record import (
     InvocationDataSource,
@@ -14,42 +14,50 @@
 
 class Invocation:
     __invocation_delegate: InvocationDelegate
     __record: InvocationRecord
 
     @classmethod
     def from_id(
-        cls, invocation_id: str, invocation_delegate: InvocationDelegate
+        cls,
+        invocation_id: str,
+        invocation_delegate: InvocationDelegate,
+        org_id: Optional[str] = None,
     ) -> "Invocation":
-        record = invocation_delegate.get_by_id(invocation_id)
+        record = invocation_delegate.get_by_id(invocation_id, org_id)
         return cls(record, invocation_delegate)
 
     @classmethod
     def query(
-        cls, filters: dict[str, Any], invocation_delegate: InvocationDelegate
+        cls,
+        filters: dict[str, Any],
+        invocation_delegate: InvocationDelegate,
+        org_id: Optional[str] = None,
     ) -> collections.abc.Generator["Invocation", None, None]:
         known_keys = set(InvocationRecord.__fields__.keys())
         actual_keys = set(filters.keys())
         unknown_keys = actual_keys - known_keys
         if unknown_keys:
             plural = len(unknown_keys) > 1
             msg = (
                 "are not known attributes of Invocation"
                 if plural
                 else "is not a known attribute of Invocation"
             )
             raise ValueError(f"{unknown_keys} {msg}. Known attributes: {known_keys}")
 
-        paginated_results = invocation_delegate.query_invocations(filters)
+        paginated_results = invocation_delegate.query_invocations(
+            filters, org_id=org_id
+        )
         while True:
             for record in paginated_results.items:
                 yield cls(record, invocation_delegate)
             if paginated_results.next_token:
                 paginated_results = invocation_delegate.query_invocations(
-                    filters, paginated_results.next_token
+                    filters, org_id=org_id, page_token=paginated_results.next_token
                 )
             else:
                 break
 
     def __init__(
         self, record: InvocationRecord, invocation_delegate: InvocationDelegate
     ) -> None:
@@ -62,30 +70,30 @@
 
     @property
     def data_source(self) -> InvocationDataSource:
         return self.__record.data_source
 
     @property
     def id(self) -> str:
-        return self.__record.id
+        return self.__record.invocation_id
 
     @property
     def input_data(self) -> list[str]:
         return self.__record.input_data
 
     @property
-    def logs_location(self) -> tuple[str, str] | None:
+    def logs_location(self) -> Optional[tuple[str, str]]:
         if not self.__record.logs_bucket or not self.__record.logs_prefix:
             return None
 
         return self.__record.logs_bucket, self.__record.logs_prefix
 
     @property
     def org_id(self) -> str:
-        return self.__record.tenant_id
+        return self.__record.org_id
 
     @property
     def status(self) -> InvocationStatus:
         status_record = self.__record.status[-1]
         return status_record.status
 
     def is_queued_for_scheduling(self) -> bool:
@@ -108,15 +116,15 @@
         )
         self.__record = updated_record
 
     def to_dict(self) -> dict[str, Any]:
         return pydantic_jsonable_dict(self.__record)
 
     def update_status(
-        self, next_status: InvocationStatus, detail: str | None = "None"
+        self, next_status: InvocationStatus, detail: Optional[str] = "None"
     ) -> None:
         if next_status == InvocationStatus.Failed:
             # Heuristic: if this is the third time the invocation has failed, it is Deadly
             num_failures = len(
                 [
                     status_record
                     for status_record in self.__record.status
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/invocation_delegate.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/invocation_delegate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import abc
-from typing import Any
+from typing import Any, Optional
 
 from ...pagination import PaginatedList
 from .invocation_record import (
     InvocationDataSourceType,
     InvocationRecord,
     InvocationSource,
     InvocationStatus,
@@ -15,41 +15,44 @@
     def create_invocation(
         self,
         action_name: str,
         input_data: list[str],
         data_source_id: str,
         data_source_type: InvocationDataSourceType,
         invocation_source: InvocationSource,
-        invocation_source_id: str | None = None,
-        tenant_id: str | None = None,
+        invocation_source_id: Optional[str] = None,
+        org_id: Optional[str] = None,
     ) -> InvocationRecord:
         """Create an Invocation"""
         raise NotImplementedError("create_invocation")
 
     @abc.abstractmethod
     def get_by_id(
-        self, invocation_id: str, org_id: str | None = None
+        self, invocation_id: str, org_id: Optional[str] = None
     ) -> InvocationRecord:
         """Get an Invocation by ID"""
         raise NotImplementedError("get_by_id")
 
     @abc.abstractmethod
     def set_logs_location(
         self, record: InvocationRecord, bucket: str, prefix: str
     ) -> InvocationRecord:
         raise NotImplementedError("set_logs_location")
 
     @abc.abstractmethod
     def update_invocation_status(
         self,
-        invocation: InvocationRecord,
+        record: InvocationRecord,
         status: InvocationStatus,
-        detail: str | None = None,
+        detail: Optional[str] = None,
     ) -> InvocationRecord:
         """Update the status of an Invocation"""
         raise NotImplementedError("update_invocation_status")
 
     @abc.abstractmethod
     def query_invocations(
-        self, filters: dict[str, Any], page_token: dict[str, str] | None = None
+        self,
+        filters: dict[str, Any],
+        org_id: Optional[str] = None,
+        page_token: Optional[dict[str, str]] = None,
     ) -> PaginatedList[InvocationRecord]:
         raise NotImplementedError("query_actions")
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/invocation_http_delegate.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/invocation_http_delegate.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import json
-from typing import Any
+from typing import Any, Optional
 
-from ...http import HttpClient
+from ...http import (
+    ORG_OVERRIDE_HEADER,
+    USER_OVERRIDE_HEADER,
+    HttpClient,
+)
 from ...logging import default_logger
 from ...pagination import PaginatedList
 from ...serde import pydantic_jsonable_dict
 from .invocation_delegate import (
     InvocationDelegate,
 )
 from .invocation_http_resources import (
@@ -31,101 +35,100 @@
     __roboto_service_base_url: str
 
     def __init__(self, roboto_service_base_url: str, http_client: HttpClient) -> None:
         super().__init__()
         self.__http_client = http_client
         self.__roboto_service_base_url = roboto_service_base_url
 
+    def headers(
+        self, org_id: Optional[str] = None, user_id: Optional[str] = None
+    ) -> dict[str, str]:
+        headers = {"Content-Type": "application/json"}
+        if org_id:
+            headers[ORG_OVERRIDE_HEADER] = org_id
+        if user_id:
+            headers[USER_OVERRIDE_HEADER] = user_id
+        return headers
+
     def create_invocation(
         self,
         action_name: str,
         input_data: list[str],
         data_source_id: str,
         data_source_type: InvocationDataSourceType,
         invocation_source: InvocationSource,
-        invocation_source_id: str | None = None,
-        tenant_id: str | None = None,
+        invocation_source_id: Optional[str] = None,
+        org_id: Optional[str] = None,
     ) -> InvocationRecord:
-        """
-        `tenant_id` and `invocation_source_id` are ignored client-side; they are determined server-side.
-        """
         url = f"{self.__roboto_service_base_url}/v1/actions/{action_name}/invoke"
         request_body = CreateInvocationRequest(
             input_data=input_data,
             data_source_id=data_source_id,
             data_source_type=data_source_type,
             invocation_source=invocation_source,
             invocation_source_id=invocation_source_id,
         )
-        headers = {"Content-Type": "application/json"}
-        if tenant_id:
-            headers["X-Roboto-Org-Id"] = tenant_id
         response = self.__http_client.post(
             url,
             data=pydantic_jsonable_dict(request_body, exclude_none=True),
-            headers=headers,
+            headers=self.headers(
+                org_id=org_id,
+                user_id=invocation_source_id
+                if invocation_source == InvocationSource.Manual
+                else None,
+            ),
         )
         return InvocationRecord.parse_obj(response.from_json(json_path=["data"]))
 
     def get_by_id(
-        self, invocation_id: str, org_id: str | None = None
+        self, invocation_id: str, org_id: Optional[str] = None
     ) -> InvocationRecord:
         url = f"{self.__roboto_service_base_url}/v1/actions/invocations/{invocation_id}"
-        headers = {}
-        if org_id:
-            headers["X-Roboto-Org-Id"] = org_id
-        response = self.__http_client.get(url, headers=headers)
+        response = self.__http_client.get(url, headers=self.headers(org_id))
         return InvocationRecord.parse_obj(response.from_json(json_path=["data"]))
 
     def set_logs_location(
         self, record: InvocationRecord, bucket: str, prefix: str
     ) -> InvocationRecord:
-        url = (
-            f"{self.__roboto_service_base_url}/v1/actions/invocations/{record.id}/logs"
-        )
-        headers = {
-            "Content-Type": "application/json",
-            "X-Roboto-Org-Id": record.tenant_id,
-        }
+        url = f"{self.__roboto_service_base_url}/v1/actions/invocations/{record.invocation_id}/logs"
         request_body = SetLogsLocationRequest(bucket=bucket, prefix=prefix)
         response = self.__http_client.patch(
             url,
             data=pydantic_jsonable_dict(request_body, exclude_none=True),
-            headers=headers,
+            headers=self.headers(record.org_id),
         )
         return InvocationRecord.parse_obj(response.from_json(json_path=["data"]))
 
     def update_invocation_status(
         self,
-        invocation: InvocationRecord,
+        record: InvocationRecord,
         status: InvocationStatus,
-        detail: str | None = None,
+        detail: Optional[str] = None,
     ) -> InvocationRecord:
-        url = f"{self.__roboto_service_base_url}/v1/actions/invocations/{invocation.id}/status"
-        headers = {
-            "Content-Type": "application/json",
-            "X-Roboto-Org-Id": invocation.tenant_id,
-        }
+        url = f"{self.__roboto_service_base_url}/v1/actions/invocations/{record.invocation_id}/status"
         response = self.__http_client.post(
             url,
             data={"status": status.value, "detail": detail},
-            headers=headers,
+            headers=self.headers(record.org_id),
         )
         return InvocationRecord.parse_obj(response.from_json(json_path=["data"]))
 
     def query_invocations(
-        self, filters: dict[str, Any], page_token: dict[str, str] | None = None
+        self,
+        filters: dict[str, Any],
+        org_id: Optional[str] = None,
+        page_token: Optional[dict[str, str]] = None,
     ) -> PaginatedList[InvocationRecord]:
         if page_token:
             filters["page_token"] = page_token
 
         safe_filters = json.loads(json.dumps(filters))
         url = f"{self.__roboto_service_base_url}/v1/actions/invocations/query"
         res = self.__http_client.post(
-            url, data=safe_filters, headers={"Content-Type": "application/json"}
+            url, data=safe_filters, headers=self.headers(org_id)
         )
         unmarshalled = res.from_json(json_path=["data"])
         return PaginatedList(
             items=[
                 InvocationRecord.parse_obj(dataset) for dataset in unmarshalled["items"]
             ],
             next_token=unmarshalled["next_token"],
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/invocation_record.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/invocation_record.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 import datetime
 import enum
+from typing import Optional
 
 import pydantic
 
 
 class InvocationDataSourceType(enum.Enum):
     """Source of data for an Action's InputBinding"""
 
     Dataset = "Dataset"
 
 
 class InvocationDataSource(pydantic.BaseModel):
-    type: InvocationDataSourceType
+    data_source_type: InvocationDataSourceType
     # The "type" determines the meaning of "id":
     #   - if type is "Dataset," id is a dataset_id
-    id: str
+    data_source_id: str
 
 
 class InvocationSource(enum.Enum):
     Trigger = "Trigger"
     Manual = "Manual"
 
 
-class InvocationDetail(pydantic.BaseModel):
-    """Details why this Action was invoked."""
-
-    type: InvocationSource
+class InvocationProvenance(pydantic.BaseModel):
+    source_type: InvocationSource
     # The “type” determines the meaning of “id:”
     #   - if type is “Trigger,” id is a TriggerId;
     #   - if type is “Manual,” id is a UserId.
-    id: str
+    source_id: str
 
 
 class InvocationStatus(enum.Enum):
     Queued = "Queued"
     Scheduled = "Scheduled"
     Downloading = "Downloading"
     Processing = "Processing"
@@ -41,22 +40,22 @@
     Completed = "Completed"
     Failed = "Failed"
     Deadly = "Deadly"
 
 
 class InvocationStatusRecord(pydantic.BaseModel):
     status: InvocationStatus
-    detail: str | None = None
+    detail: Optional[str] = None
     timestamp: datetime.datetime  # Persisted as ISO 8601 string in UTC
 
 
 class InvocationRecord(pydantic.BaseModel):
-    id: str
-    tenant_id: str
+    invocation_id: str  # Partition key
+    org_id: str
     action_name: str
     created: datetime.datetime  # Persisted as ISO 8601 string in UTC
     data_source: InvocationDataSource
     input_data: list[str]
-    invoked_by: InvocationDetail
-    logs_bucket: str | None = None
-    logs_prefix: str | None = None
+    provenance: InvocationProvenance
+    logs_bucket: Optional[str] = None
+    logs_prefix: Optional[str] = None
     status: list[InvocationStatusRecord] = pydantic.Field(default_factory=list)
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/datasets/__init__.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/datasets/dataset.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/datasets/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import collections.abc
 import pathlib
-from typing import Any
+from typing import Any, Optional
 
 import pathspec
 
 from ...serde import pydantic_jsonable_dict
 from ..files import (
     File,
     FileDelegate,
@@ -19,90 +19,91 @@
 )
 from .record import Administrator, DatasetRecord
 
 
 class Dataset:
     __delegate: DatasetDelegate
     __record: DatasetRecord
-    __files_delegate: FileDelegate | None = None
-    __temp_credentials: Credentials | None = None
+    __files_delegate: Optional[FileDelegate] = None
+    __temp_credentials: Optional[Credentials] = None
 
     @classmethod
     def create(
         cls,
         dataset_delegate: DatasetDelegate,
         administrator: Administrator = Administrator.Roboto,
         storage_location: StorageLocation = StorageLocation.S3,
-        tenant_id: str | None = None,
-        created_by: str | None = None,
-        metadata: dict[str, Any] | None = None,
-        tags: list[str] | None = None,
-        files_delegate: FileDelegate | None = None,
+        org_id: Optional[str] = None,
+        created_by: Optional[str] = None,
+        metadata: Optional[dict[str, Any]] = None,
+        tags: Optional[list[str]] = None,
+        files_delegate: Optional[FileDelegate] = None,
     ) -> "Dataset":
         record = dataset_delegate.create_dataset(
-            administrator, metadata, storage_location, tags, tenant_id, created_by
+            administrator, metadata, storage_location, tags, org_id, created_by
         )
         return cls(record, dataset_delegate, files_delegate)
 
     @classmethod
-    def by_id(
+    def from_id(
         cls,
         dataset_id: str,
         dataset_delegate: DatasetDelegate,
-        tenant_id: str | None = None,
-        files_delegate: FileDelegate | None = None,
+        org_id: Optional[str] = None,
+        files_delegate: Optional[FileDelegate] = None,
     ) -> "Dataset":
-        record = dataset_delegate.get_dataset_by_primary_key(dataset_id, tenant_id)
+        record = dataset_delegate.get_dataset_by_primary_key(dataset_id, org_id)
         return cls(record, dataset_delegate, files_delegate)
 
     @classmethod
     def query(
         cls,
         filters: dict[str, Any],
         dataset_delegate: DatasetDelegate,
-        files_delegate: FileDelegate | None = None,
+        files_delegate: Optional[FileDelegate] = None,
+        org_id: Optional[str] = None,
     ) -> collections.abc.Generator["Dataset", None, None]:
         known_keys = set(DatasetRecord.__fields__.keys())
         actual_keys = set(filters.keys())
         unknown_keys = actual_keys - known_keys
         if unknown_keys:
             plural = len(unknown_keys) > 1
             msg = (
                 "are not known attributes of Dataset"
                 if plural
                 else "is not a known attribute of Dataset"
             )
             raise ValueError(f"{unknown_keys} {msg}. Known attributes: {known_keys}")
 
-        paginated_results = dataset_delegate.query_datasets(filters)
+        paginated_results = dataset_delegate.query_datasets(filters, org_id=org_id)
         while True:
             for record in paginated_results.items:
                 yield cls(record, dataset_delegate, files_delegate)
             if paginated_results.next_token:
                 paginated_results = dataset_delegate.query_datasets(
-                    filters, paginated_results.next_token
+                    filters, org_id=org_id, page_token=paginated_results.next_token
                 )
             else:
                 break
 
     def __init__(
         self,
         record: DatasetRecord,
         delegate: DatasetDelegate,
-        files_delegate: FileDelegate | None = None,
+        files_delegate: Optional[FileDelegate] = None,
     ) -> None:
         self.__delegate = delegate
         self.__files_delegate = files_delegate
         self.__record = record
 
     def download_files(
         self,
         out_path: pathlib.Path,
-        include_patterns: list[str] | None = None,
-        exclude_patterns: list[str] | None = None,
+        include_patterns: Optional[list[str]] = None,
+        exclude_patterns: Optional[list[str]] = None,
     ) -> None:
         """
         Download files associated with this dataset to the given directory.
         If `out_path` does not exist, it will be created.
 
         `include_patterns` and `exclude_patterns` are lists of gitignore-style patterns.
         See https://git-scm.com/docs/gitignore.
@@ -121,21 +122,21 @@
             self.__record.storage_location != StorageLocation.S3
             or self.__record.administrator != Administrator.Roboto
         ):
             raise NotImplementedError(
                 "Only S3-backed storage administered by Roboto is supported at this time."
             )
 
-        include_pattern_spec: pathspec.PathSpec | None = None
+        include_pattern_spec: Optional[pathspec.PathSpec] = None
         if include_patterns is not None:
             include_pattern_spec = pathspec.PathSpec.from_lines(
                 pathspec.patterns.GitWildMatchPattern, include_patterns
             )
 
-        exclude_pattern_spec: pathspec.PathSpec | None = None
+        exclude_pattern_spec: Optional[pathspec.PathSpec] = None
         if exclude_patterns is not None:
             exclude_pattern_spec = pathspec.GitIgnoreSpec.from_lines(exclude_patterns)
 
         if not out_path.is_dir():
             out_path.mkdir(parents=True)
 
         credentials = self.get_temporary_credentials(AccessMode.ReadOnly)
@@ -159,43 +160,47 @@
                 """Given file matches one of the exclude patterns."""
                 continue
 
             local_path = out_path / file.relative_path
             files_delegate.download_file(file.key, local_path)
 
     def get_temporary_credentials(
-        self, mode: AccessMode = AccessMode.ReadOnly
+        self,
+        mode: AccessMode = AccessMode.ReadOnly,
+        caller: Optional[str] = None,  # A Roboto user_id
     ) -> Credentials:
         if self.__temp_credentials is None or self.__temp_credentials.is_expired():
             self.__temp_credentials = self.__delegate.get_temporary_credentials(
-                self.__record, mode
+                self.__record, mode, caller
             )
         return self.__temp_credentials
 
     def list_files(self) -> collections.abc.Generator[File, None, None]:
-        paginated_results = self.__delegate.list_files(self.__record.id)
+        paginated_results = self.__delegate.list_files(
+            self.__record.dataset_id, self.__record.org_id
+        )
         while True:
             for record in paginated_results.items:
                 yield File(record)
             if paginated_results.next_token:
                 paginated_results = self.__delegate.list_files(
-                    self.__record.id,
-                    self.__record.tenant_id,
+                    self.__record.dataset_id,
+                    self.__record.org_id,
                     paginated_results.next_token,
                 )
             else:
                 break
 
     def to_dict(self) -> dict[str, Any]:
         return pydantic_jsonable_dict(self.__record)
 
     def upload_directory(
         self,
         directory_path: pathlib.Path,
-        exclude_patterns: list[str] | None = None,
+        exclude_patterns: Optional[list[str]] = None,
     ) -> None:
         """
         Upload everything, recursively, in directory, ignoring files that match any of the ignore patterns.
 
         `exclude_patterns` is a list of gitignore-style patterns.
         See https://git-scm.com/docs/gitignore#_pattern_format.
 
@@ -211,15 +216,15 @@
             ],
         )
         ```
         """
         if not directory_path.is_dir():
             raise ValueError(f"{directory_path} is not a directory")
 
-        exclude_spec: pathspec.PathSpec | None = None
+        exclude_spec: Optional[pathspec.PathSpec] = None
         if exclude_patterns is not None:
             exclude_spec = pathspec.GitIgnoreSpec.from_lines(
                 exclude_patterns,
             )
 
         def _upload_directory(directory_path: pathlib.Path, key_prefix: str) -> None:
             for path in directory_path.iterdir():
@@ -265,12 +270,12 @@
             )
         )
         key = f"{credentials.required_prefix}/{key.lstrip('/')}"
         files_delegate.upload_file(
             local_file_path,
             key,
             tags={
-                FileTag.DatasetId: self.__record.id,
-                FileTag.TenantId: self.__record.tenant_id,
+                FileTag.DatasetId: self.__record.dataset_id,
+                FileTag.OrgId: self.__record.org_id,
                 FileTag.CommonPrefix: credentials.required_prefix,
             },
         )
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/datasets/delegate.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/datasets/delegate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import abc
 import datetime
 import enum
-from typing import Any
+from typing import Any, Optional
 
 import pydantic
 
 from ...pagination import PaginatedList
 from ...serde import pydantic_jsonable_dict
 from ...time import utcnow
 from ..files import FileRecord
@@ -37,43 +37,46 @@
 
 
 class DatasetDelegate(abc.ABC):
     @abc.abstractmethod
     def create_dataset(
         self,
         administrator: Administrator = Administrator.Roboto,
-        metadata: dict[str, Any] | None = None,
+        metadata: Optional[dict[str, Any]] = None,
         storage_location: StorageLocation = StorageLocation.S3,
-        tags: list[str] | None = None,
-        tenant_id: str | None = None,
-        created_by: str | None = None,
+        tags: Optional[list[str]] = None,
+        org_id: Optional[str] = None,
+        created_by: Optional[str] = None,
     ) -> DatasetRecord:
         raise NotImplementedError("create_dataset")
 
     @abc.abstractmethod
     def get_dataset_by_primary_key(
         self,
         dataset_id: str,
-        tenant_id: str | None = None,
+        org_id: Optional[str] = None,
     ) -> DatasetRecord:
         raise NotImplementedError("get_dataset_by_primary_key")
 
     @abc.abstractmethod
     def get_temporary_credentials(
-        self, record: DatasetRecord, mode: AccessMode, caller: str | None = None
+        self, record: DatasetRecord, mode: AccessMode, caller: Optional[str] = None
     ) -> Credentials:
         raise NotImplementedError("get_temporary_credentials")
 
     @abc.abstractmethod
     def list_files(
         self,
         dataset_id: str,
-        tenant_id: str | None = None,
-        page_token: dict[str, str] | None = None,
+        org_id: Optional[str] = None,
+        page_token: Optional[dict[str, str]] = None,
     ) -> PaginatedList[FileRecord]:
         raise NotImplementedError("list_files")
 
     @abc.abstractmethod
     def query_datasets(
-        self, filters: dict[str, Any], page_token: dict[str, str] | None = None
+        self,
+        filters: dict[str, Any],
+        org_id: Optional[str] = None,
+        page_token: Optional[dict[str, str]] = None,
     ) -> PaginatedList[DatasetRecord]:
         raise NotImplementedError("query_datasets")
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/datasets/http_delegate.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/datasets/http_delegate.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import json
-from typing import Any
+from typing import Any, Optional
 import urllib.parse
 
-from ...http import HttpClient
+from ...http import (
+    ORG_OVERRIDE_HEADER,
+    USER_OVERRIDE_HEADER,
+    HttpClient,
+)
 from ...pagination import PaginatedList
 from ...serde import pydantic_jsonable_dict
 from ..files import FileRecord
 from .delegate import (
     AccessMode,
     Credentials,
     DatasetDelegate,
@@ -24,105 +28,110 @@
     __roboto_service_base_url: str
 
     def __init__(self, roboto_service_base_url: str, http_client: HttpClient) -> None:
         super().__init__()
         self.__http_client = http_client
         self.__roboto_service_base_url = roboto_service_base_url
 
+    def headers(
+        self, org_id: Optional[str], user_id: Optional[str] = None
+    ) -> dict[str, str]:
+        headers = {"Content-Type": "application/json"}
+        if org_id:
+            headers[ORG_OVERRIDE_HEADER] = org_id
+        if user_id:
+            headers[USER_OVERRIDE_HEADER] = user_id
+        return headers
+
     def create_dataset(
         self,
         administrator: Administrator = Administrator.Roboto,
-        metadata: dict[str, Any] | None = None,
+        metadata: Optional[dict[str, Any]] = None,
         storage_location: StorageLocation = StorageLocation.S3,
-        tags: list[str] | None = None,
-        tenant_id: str | None = None,
-        created_by: str | None = None,
+        tags: Optional[list[str]] = None,
+        org_id: Optional[str] = None,
+        created_by: Optional[str] = None,
     ) -> DatasetRecord:
         """
         Create a new dataset.
-
-        `tenant_id` and `created_by` are ignored, as both are determined server-side by the identity of the caller.
         """
         url = f"{self.__roboto_service_base_url}/v1/datasets"
         request_body = CreateDatasetRequest(
             administrator=administrator,
             metadata=metadata if metadata is not None else {},
             storage_location=storage_location,
             tags=tags if tags is not None else [],
         )
         response = self.__http_client.post(
             url,
             data=pydantic_jsonable_dict(request_body),
-            headers={"Content-Type": "application/json"},
+            headers=self.headers(org_id, created_by),
         )
         return DatasetRecord.parse_obj(response.from_json(json_path=["data"]))
 
     def get_dataset_by_primary_key(
         self,
         dataset_id: str,
-        tenant_id: str | None = None,
+        org_id: Optional[str] = None,
     ) -> DatasetRecord:
         """
-        Get a dataset by its primary key (tenant_id, dataset_id)
-
-        `tenant_id` is ignored, as it is determined server-side by the identity of the caller.
+        Get a dataset by its primary key (org_id, dataset_id)
         """
         url = f"{self.__roboto_service_base_url}/v1/datasets/{dataset_id}"
-        response = self.__http_client.get(url)
+        response = self.__http_client.get(url, headers=self.headers(org_id))
         return DatasetRecord.parse_obj(response.from_json(json_path=["data"]))
 
     def get_temporary_credentials(
-        self, record: DatasetRecord, mode: AccessMode, caller: str | None = None
+        self, record: DatasetRecord, mode: AccessMode, caller: Optional[str] = None
     ) -> Credentials:
         """
         Get temporary credentials to access a dataset.
-
-        `caller` is ignored, as it is determined server-side by the identity of the caller.
         """
         query_params = {"mode": mode.value}
         encoded_qs = urllib.parse.urlencode(query_params)
-        url = f"{self.__roboto_service_base_url}/v1/datasets/{record.id}/credentials?{encoded_qs}"
-        response = self.__http_client.get(url)
+        url = f"{self.__roboto_service_base_url}/v1/datasets/{record.dataset_id}/credentials?{encoded_qs}"
+        response = self.__http_client.get(url, self.headers(record.org_id, caller))
         return Credentials.parse_obj(response.from_json(json_path=["data"]))
 
     def list_files(
         self,
         dataset_id: str,
-        tenant_id: str | None = None,
-        page_token: dict[str, str] | None = None,
+        org_id: Optional[str] = None,
+        page_token: Optional[dict[str, str]] = None,
     ) -> PaginatedList[FileRecord]:
         """
         List files associated with dataset.
 
         Files are associated with datasets in an eventually-consistent manner,
         so there will likely be delay between a file being uploaded and it appearing in this list.
-
-        `tenant_id` is ignored, as it is determined server-side by the identity of the caller.
         """
         url = f"{self.__roboto_service_base_url}/v1/datasets/{dataset_id}/files"
         if page_token:
             query_str = urllib.parse.urlencode(page_token)
             url = f"{url}?{query_str}"
-        response = self.__http_client.get(url)
+        response = self.__http_client.get(url, headers=self.headers(org_id))
         unmarshalled = response.from_json(json_path=["data"])
         return PaginatedList(
             items=[FileRecord.parse_obj(file) for file in unmarshalled["items"]],
             next_token=unmarshalled["next_token"],
         )
 
     def query_datasets(
-        self, filters: dict[str, Any], page_token: dict[str, str] | None = None
+        self,
+        filters: dict[str, Any],
+        org_id: Optional[str] = None,
+        page_token: Optional[dict[str, str]] = None,
     ) -> PaginatedList[DatasetRecord]:
         if page_token:
             filters["page_token"] = page_token
 
         safe_filters = json.loads(json.dumps(filters))
         url = f"{self.__roboto_service_base_url}/v1/datasets/query"
         res = self.__http_client.post(
-            url, data=safe_filters, headers={"Content-Type": "application/json"}
+            url, data=safe_filters, headers=self.headers(org_id)
         )
         unmarshalled = res.from_json(json_path=["data"])
         return PaginatedList(
             items=[
                 DatasetRecord.parse_obj(dataset) for dataset in unmarshalled["items"]
             ],
             next_token=unmarshalled["next_token"],
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/datasets/record.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/datasets/record.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 class StorageLocation(str, enum.Enum):
     # Other supported locations might be "GCP" or "Azure"
     S3 = "S3"
 
 
 class DatasetRecord(pydantic.BaseModel):
-    # Primary key
-    id: str
-    tenant_id: str
+    # Primary key, defined in CDK
+    org_id: str  # partition key
+    dataset_id: str  # sort key
 
     administrator: Administrator
     # Persisted as ISO 8601 string in UTC
     created: datetime.datetime
     created_by: str
     metadata: dict[str, Any] = pydantic.Field(default_factory=dict)
     # Persisted as ISO 8601 string in UTC
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/files/delegate.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/files/delegate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import abc
 import enum
 import pathlib
+from typing import Optional
 
 from .record import FileRecord
 
 
 class FileTag(enum.Enum):
     DatasetId = "dataset_id"
-    TenantId = "tenant_id"
+    OrgId = "org_id"
     # Path to file relative to common prefix
     CommonPrefix = "common_prefix"
 
 
 class FileDelegate(abc.ABC):
     @abc.abstractmethod
     def delete_file(self, key: str) -> None:
@@ -22,15 +23,15 @@
         raise NotImplementedError("download_file")
 
     @abc.abstractmethod
     def upload_file(
         self,
         local_path: pathlib.Path,
         key: str,
-        tags: dict[FileTag, str] | None = None,
+        tags: Optional[dict[FileTag, str]] = None,
     ) -> None:
         raise NotImplementedError("upload_file")
 
     @abc.abstractmethod
     def protected_upsert_file_record(
         self,
         bucket: str,
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/files/file.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/files/file.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from typing import Optional
 import urllib.parse
 
 from .record import FileRecord
 
 
 class File:
     __record: FileRecord
-    __parsed_uri: urllib.parse.ParseResult | None = None
+    __parsed_uri: Optional[urllib.parse.ParseResult] = None
 
     def __init__(self, record: FileRecord):
         self.__record = record
 
     @property
     def uri(self) -> str:
         return self.__record.uri
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/files/http_delegate.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/files/http_delegate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pathlib
+from typing import Optional
 
 from ...http import HttpClient
 from ...serde import pydantic_jsonable_dict
 from .delegate import FileDelegate, FileTag
 from .http_resources import (
     CreateFileRequest,
     DeleteFileRequest,
@@ -27,15 +28,18 @@
     def delete_file(self, key: str) -> None:
         raise NotImplementedError("delete_file")
 
     def download_file(self, key: str, local_path: pathlib.Path) -> None:
         raise NotImplementedError("download_file")
 
     def upload_file(
-        self, local_path: pathlib.Path, key: str, tags: dict[FileTag, str] | None = None
+        self,
+        local_path: pathlib.Path,
+        key: str,
+        tags: Optional[dict[FileTag, str]] = None,
     ) -> None:
         raise NotImplementedError("upload_file")
 
     def protected_upsert_file_record(
         self,
         bucket: str,
         key: str,
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/files/s3_delegate.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/files/s3_delegate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pathlib
-from typing import Any, Protocol
+from typing import Any, Optional, Protocol
 import urllib.parse
 
 import boto3
 
 from .delegate import FileDelegate, FileTag
 from .record import FileRecord
 
@@ -39,15 +39,18 @@
         )
 
     def download_file(self, key: str, local_path: pathlib.Path) -> None:
         local_path.parent.mkdir(parents=True, exist_ok=True)
         self.__s3_bucket.download_file(key, str(local_path))
 
     def upload_file(
-        self, local_path: pathlib.Path, key: str, tags: dict[FileTag, str] | None = None
+        self,
+        local_path: pathlib.Path,
+        key: str,
+        tags: Optional[dict[FileTag, str]] = None,
     ) -> None:
         upload_file_args: dict[str, Any] = {
             "Filename": str(local_path),
             "Key": key,
         }
 
         if tags is not None:
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/__init__.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,30 +5,34 @@
 from .http_delegate import OrgHttpDelegate
 from .http_resources import (
     BindEmailDomainRequest,
     CreateOrgRequest,
     InviteUserRequest,
 )
 from .org import Org
+from .org_invite import OrgInvite
 from .org_role import OrgRole
 from .record import (
+    OrgInviteRecord,
     OrgRecord,
     OrgRoleName,
     OrgRoleRecord,
     OrgTier,
     OrgType,
 )
 
 __all__ = [
     "BindEmailDomainRequest",
     "CreateOrgRequest",
     "InviteUserRequest",
     "Org",
     "OrgDelegate",
     "OrgHttpDelegate",
+    "OrgInvite",
+    "OrgInviteRecord",
     "OrgRecord",
     "OrgRole",
     "OrgRoleName",
     "OrgRoleRecord",
     "OrgTier",
     "OrgType",
 ]
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/delegate.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/delegate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
 import abc
+from typing import Optional
 
 from .record import (
+    OrgInviteRecord,
     OrgRecord,
     OrgRoleRecord,
     OrgType,
 )
 
 
 class OrgDelegate(abc.ABC):
     @abc.abstractmethod
     def create_org(
         self,
-        creator_user_id: str | None,
+        creator_user_id: Optional[str],
         name: str,
         org_type: OrgType,
         bind_email_domain: bool = False,
     ) -> OrgRecord:
         raise NotImplementedError("create_org")
 
     @abc.abstractmethod
-    def orgs_for_user(self, user_id: str | None) -> list[OrgRecord]:
+    def orgs_for_user(self, user_id: Optional[str]) -> list[OrgRecord]:
         raise NotImplementedError("orgs_for_user")
 
     @abc.abstractmethod
-    def org_roles_for_user(self, user_id: str | None) -> list[OrgRoleRecord]:
+    def org_roles_for_user(self, user_id: Optional[str]) -> list[OrgRoleRecord]:
         raise NotImplementedError("org_roles_for_user")
 
     @abc.abstractmethod
     def get_org_by_id(self, org_id: str) -> OrgRecord:
         raise NotImplementedError("get_org_by_id")
 
     @abc.abstractmethod
@@ -38,18 +40,24 @@
 
     @abc.abstractmethod
     def bind_email_domain(self, org_id: str, email_domain: str):
         raise NotImplementedError("bind_email_domain")
 
     @abc.abstractmethod
     def invite_user_to_org(
-        self, invited_user_id: str, org_id: str, inviting_user_id: str | None = None
-    ):
+        self, invited_user_id: str, org_id: str, inviting_user_id: Optional[str] = None
+    ) -> OrgInviteRecord:
         raise NotImplementedError("invite_user_to_org")
 
     @abc.abstractmethod
-    def accept_org_invite(self, invite_id: str, user_id: str | None = None):
+    def accept_org_invite(self, invite_id: str, user_id: Optional[str] = None):
         raise NotImplementedError("accept_org_invite")
 
     @abc.abstractmethod
-    def decline_org_invite(self, invite_id: str, user_id: str | None = None):
+    def decline_org_invite(self, invite_id: str, user_id: Optional[str] = None):
         raise NotImplementedError("accept_org_invite")
+
+    @abc.abstractmethod
+    def get_org_invite(
+        self, invite_id: str, user_id: Optional[str] = None
+    ) -> OrgInviteRecord:
+        raise NotImplementedError("get_org_invite")
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/http_delegate.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/http_delegate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
+from typing import Optional
 
 from ...http import (
     ORG_OVERRIDE_HEADER,
     USER_OVERRIDE_HEADER,
     HttpClient,
 )
 from ...serde import pydantic_jsonable_dict
 from .delegate import OrgDelegate
 from .http_resources import (
     BindEmailDomainRequest,
     CreateOrgRequest,
     InviteUserRequest,
 )
 from .record import (
+    OrgInviteRecord,
     OrgRecord,
     OrgRoleRecord,
     OrgType,
 )
 
 
 class OrgHttpDelegate(OrgDelegate):
@@ -25,15 +27,15 @@
 
     def __init__(self, http_client: HttpClient):
         super().__init__()
         self.__http_client = http_client
 
     def create_org(
         self,
-        creator_user_id: str | None,
+        creator_user_id: Optional[str],
         name: str,
         org_type: OrgType,
         bind_email_domain: bool = False,
     ) -> OrgRecord:
         url = self.__http_client.url("v1/orgs")
         headers = {"Content-Type": "application/json"}
 
@@ -44,23 +46,23 @@
             name=name, org_type=org_type, bind_email_domain=bind_email_domain
         )
         response = self.__http_client.post(
             url=url, headers=headers, data=pydantic_jsonable_dict(request_body)
         )
         return OrgRecord.parse_obj(response.from_json(json_path=["data"]))
 
-    def orgs_for_user(self, user_id: str | None) -> list[OrgRecord]:
+    def orgs_for_user(self, user_id: Optional[str]) -> list[OrgRecord]:
         url = self.__http_client.url("v1/orgs/list")
         response = self.__http_client.get(url=url)
         return [
             OrgRecord.parse_obj(record)
             for record in response.from_json(json_path=["data"])
         ]
 
-    def org_roles_for_user(self, user_id: str | None) -> list[OrgRoleRecord]:
+    def org_roles_for_user(self, user_id: Optional[str]) -> list[OrgRoleRecord]:
         url = self.__http_client.url("v1/orgs/roles")
         response = self.__http_client.get(url=url)
         return [
             OrgRoleRecord.parse_obj(record)
             for record in response.from_json(json_path=["data"])
         ]
 
@@ -80,23 +82,31 @@
         headers = {ORG_OVERRIDE_HEADER: org_id}
         request_body = BindEmailDomainRequest(email_domain=email_domain)
         self.__http_client.put(
             url=url, headers=headers, data=pydantic_jsonable_dict(request_body)
         )
 
     def invite_user_to_org(
-        self, invited_user_id: str, org_id: str, inviting_user_id: str | None = None
-    ):
+        self, invited_user_id: str, org_id: str, inviting_user_id: Optional[str] = None
+    ) -> OrgInviteRecord:
         url = self.__http_client.url("v1/orgs/invites")
         headers = {ORG_OVERRIDE_HEADER: org_id}
         request_body = InviteUserRequest(invited_user_id=invited_user_id)
-        self.__http_client.post(
+        response = self.__http_client.post(
             url=url, headers=headers, data=pydantic_jsonable_dict(request_body)
         )
+        return OrgInviteRecord.parse_obj(response.from_json(json_path=["data"]))
 
-    def accept_org_invite(self, invite_id: str, user_id: str | None = None):
+    def accept_org_invite(self, invite_id: str, user_id: Optional[str] = None):
         url = self.__http_client.url(f"v1/orgs/invites/accept/{invite_id}")
         self.__http_client.post(url=url)
 
-    def decline_org_invite(self, invite_id: str, user_id: str | None = None):
+    def decline_org_invite(self, invite_id: str, user_id: Optional[str] = None):
         url = self.__http_client.url(f"v1/orgs/invites/decline/{invite_id}")
         self.__http_client.post(url=url)
+
+    def get_org_invite(
+        self, invite_id: str, user_id: Optional[str] = None
+    ) -> OrgInviteRecord:
+        url = self.__http_client.url(f"v1/orgs/invites/id/{invite_id}")
+        response = self.__http_client.get(url=url)
+        return OrgInviteRecord.parse_obj(response.from_json(json_path=["data"]))
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/org.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/org.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
-from typing import Any
+from typing import Any, Optional
 
 from ...serde import pydantic_jsonable_dict
 from .delegate import OrgDelegate
 from .record import OrgRecord, OrgType
 
 
 class Org:
     __record: OrgRecord
     __org_delegate: OrgDelegate
 
     @classmethod
     def create(
         cls,
-        creator_user_id: str | None,
+        creator_user_id: Optional[str],
         name: str,
         org_type: OrgType,
         org_delegate: OrgDelegate,
         bind_email_domain: bool = False,
     ):
         record = org_delegate.create_org(
             creator_user_id=creator_user_id,
@@ -30,39 +30,28 @@
 
     @classmethod
     def by_org_id(cls, org_id: str, org_delegate: OrgDelegate) -> "Org":
         record = org_delegate.get_org_by_id(org_id=org_id)
         return cls(record=record, org_delegate=org_delegate)
 
     @classmethod
-    def by_user_id(cls, user_id: str | None, org_delegate: OrgDelegate) -> list["Org"]:
+    def by_user_id(
+        cls, user_id: Optional[str], org_delegate: OrgDelegate
+    ) -> list["Org"]:
         records = org_delegate.orgs_for_user(user_id=user_id)
         return [cls(record=record, org_delegate=org_delegate) for record in records]
 
     def delete(self) -> None:
         self.__org_delegate.delete_org(org_id=self.org_id)
 
     def bind_email_domain(self, email_domain: str) -> None:
         self.__org_delegate.bind_email_domain(
             org_id=self.__record.org_id, email_domain=email_domain
         )
 
-    def invite_user(self, invited_user_id: str, inviting_user_id: str | None = None):
-        self.__org_delegate.invite_user_to_org(
-            invited_user_id=invited_user_id,
-            inviting_user_id=inviting_user_id,
-            org_id=self.__record.org_id,
-        )
-
-    def accept_invite(self, invite_id: str, user_id: str | None = None):
-        self.__org_delegate.accept_org_invite(invite_id=invite_id, user_id=user_id)
-
-    def decline_invite(self, invite_id: str, user_id: str | None = None):
-        self.__org_delegate.decline_org_invite(invite_id=invite_id, user_id=user_id)
-
     def __init__(self, record: OrgRecord, org_delegate: OrgDelegate):
         self.__record = record
         self.__org_delegate = org_delegate
 
     def to_dict(self) -> dict[str, Any]:
         return pydantic_jsonable_dict(self.__record)
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/org_role.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/org_role.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
-from typing import Any
+from typing import Any, Optional
 
 from ...serde import pydantic_jsonable_dict
 from .delegate import OrgDelegate
 from .org import Org
 from .record import OrgRoleName, OrgRoleRecord
 
 
 class OrgRole:
     __record: OrgRoleRecord
     __org_delegate: OrgDelegate
     __org: Org
 
     @classmethod
     def by_user_id(
-        cls, user_id: str | None, org_delegate: OrgDelegate
+        cls, user_id: Optional[str], org_delegate: OrgDelegate
     ) -> list["OrgRole"]:
         records = org_delegate.org_roles_for_user(user_id=user_id)
         return [cls(record=record, org_delegate=org_delegate) for record in records]
 
     def __init__(self, record: OrgRoleRecord, org_delegate: OrgDelegate):
         self.__record = record
         self.__org_delegate = org_delegate
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/record.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/record.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
 import enum
 
 import pydantic
 
+from ..users import UserRecord
+
 
 class OrgType(str, enum.Enum):
     individual = "individual"
     team = "team"
 
 
 class OrgTier(str, enum.Enum):
@@ -29,7 +31,14 @@
     owner = "owner"
 
 
 class OrgRoleRecord(pydantic.BaseModel):
     user_id: str
     org: OrgRecord
     roles: list[OrgRoleName]
+
+
+class OrgInviteRecord(pydantic.BaseModel):
+    invite_id: str
+    user_id: str
+    invited_by: UserRecord
+    org: OrgRecord
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/tokens/http_delegate.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/tokens/http_delegate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
+from typing import Optional
 
 from ...http import (
     USER_OVERRIDE_HEADER,
     HttpClient,
 )
 from ...serde import pydantic_jsonable_dict
 from .delegate import TokenDelegate
@@ -14,26 +15,30 @@
 class TokenHttpDelegate(TokenDelegate):
     __http_client: HttpClient
 
     def __init__(self, http_client: HttpClient):
         super().__init__()
         self.__http_client = http_client
 
-    def get_tokens_for_user(self, user_id: str | None) -> list[TokenRecord]:
+    def get_tokens_for_user(self, user_id: Optional[str]) -> list[TokenRecord]:
         url = self.__http_client.url("v1/tokens")
         headers = {}
         if user_id is not None:
             headers[USER_OVERRIDE_HEADER] = user_id
 
         response = self.__http_client.get(url=url, headers=headers)
         unmarshalled = response.from_json(json_path=["data"])
         return [TokenRecord.parse_obj(record) for record in unmarshalled]
 
     def create_token(
-        self, user_id: str | None, expiry_days: int, name: str, description: str | None
+        self,
+        user_id: Optional[str],
+        expiry_days: int,
+        name: str,
+        description: Optional[str],
     ) -> TokenRecord:
         url = self.__http_client.url("v1/tokens")
         headers = {"Content-Type": "application/json"}
         if user_id is not None:
             headers[USER_OVERRIDE_HEADER] = user_id
 
         data = CreateTokenRequest(
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/tokens/token.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/tokens/token.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
-from typing import Any
+from typing import Any, Optional
 
 from ...serde import pydantic_jsonable_dict
 from .delegate import TokenDelegate
 from .record import TokenRecord
 
 
 class Token:
@@ -14,26 +14,26 @@
     @classmethod
     def by_token_id(cls, token_id: str, token_delegate: TokenDelegate) -> "Token":
         record = token_delegate.get_token_by_token_id(token_id=token_id)
         return cls(record=record, token_delegate=token_delegate)
 
     @classmethod
     def by_user_id(
-        cls, user_id: str | None, token_delegate: TokenDelegate
+        cls, user_id: Optional[str], token_delegate: TokenDelegate
     ) -> list["Token"]:
         records = token_delegate.get_tokens_for_user(user_id=user_id)
         return [cls(record=record, token_delegate=token_delegate) for record in records]
 
     @classmethod
     def create(
         cls,
-        user_id: str | None,
+        user_id: Optional[str],
         expiry_days: int,
         name: str,
-        description: str | None,
+        description: Optional[str],
         token_delegate: TokenDelegate,
     ):
         record = token_delegate.create_token(
             user_id=user_id, expiry_days=expiry_days, name=name, description=description
         )
         return cls(record=record, token_delegate=token_delegate)
 
@@ -47,13 +47,13 @@
         self.__record = record
         self.__token_delegate = token_delegate
 
     def to_dict(self) -> dict[str, Any]:
         return pydantic_jsonable_dict(self.__record)
 
     @property
-    def secret(self) -> str | None:
+    def secret(self) -> Optional[str]:
         return self.__record.secret
 
     @property
-    def user_id(self) -> str | None:
+    def user_id(self) -> Optional[str]:
         return self.__record.user_id
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/triggers/http_delegate.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/triggers/http_delegate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
-from typing import Any
+from typing import Any, Optional
 
 from ...http import (
     ORG_OVERRIDE_HEADER,
     HttpClient,
 )
 from ...pagination import PaginatedList
 from ...serde import pydantic_jsonable_dict
@@ -17,43 +17,43 @@
     __http_client: HttpClient
 
     def __init__(self, http_client: HttpClient):
         super().__init__()
         self.__http_client = http_client
 
     def create_trigger(
-        self, name: str, org_id: str | None, action_name: str
+        self, name: str, org_id: Optional[str], action_name: str
     ) -> TriggerRecord:
         url = self.__http_client.url("v1/triggers")
         headers = {"Content-Type": "application/json"}
         if org_id is not None:
             headers[ORG_OVERRIDE_HEADER] = org_id
 
         request_body = CreateTriggerRequest(name=name, action_name=action_name)
 
         response = self.__http_client.post(
             url, data=pydantic_jsonable_dict(request_body), headers=headers
         )
         return TriggerRecord.parse_obj(response.from_json(json_path=["data"]))
 
     def get_trigger_by_primary_key(
-        self, name: str, org_id: str | None
+        self, name: str, org_id: Optional[str]
     ) -> TriggerRecord:
         url = self.__http_client.url(f"v1/triggers/{name}")
         headers = {}
         if org_id is not None:
             headers[ORG_OVERRIDE_HEADER] = org_id
         response = self.__http_client.get(url, headers=headers)
         return TriggerRecord.parse_obj(response.from_json(json_path=["data"]))
 
     def query_triggers(
         self,
-        filters: dict[str, Any] | None,
-        org_id: str | None,
-        page_token: dict[str, str] | None = None,
+        filters: Optional[dict[str, Any]],
+        org_id: Optional[str],
+        page_token: Optional[dict[str, str]] = None,
     ) -> PaginatedList[TriggerRecord]:
         url = self.__http_client.url("v1/triggers")
 
         headers = {}
         if org_id is not None:
             headers = {ORG_OVERRIDE_HEADER: org_id}
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/triggers/trigger.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/triggers/trigger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
 import collections.abc
-from typing import Any
+from typing import Any, Optional
 
 from ...domain.actions import ActionDelegate
 from ...serde import pydantic_jsonable_dict
 from .trigger_delegate import TriggerDelegate
 from .trigger_record import TriggerRecord
 
 
@@ -14,15 +14,15 @@
     __action_delegate: ActionDelegate
     __trigger_delegate: TriggerDelegate
 
     @classmethod
     def create(
         cls,
         name: str,
-        org_id: str | None,
+        org_id: Optional[str],
         action_name: str,
         action_delegate: ActionDelegate,
         trigger_delegate: TriggerDelegate,
     ) -> "Trigger":
         record = trigger_delegate.create_trigger(
             name=name, org_id=org_id, action_name=action_name
         )
@@ -33,30 +33,30 @@
         )
 
     # And version?
     @classmethod
     def by_name(
         cls,
         name: str,
-        org_id: str | None,
+        org_id: Optional[str],
         action_delegate: ActionDelegate,
         trigger_delegate: TriggerDelegate,
     ) -> "Trigger":
         record = trigger_delegate.get_trigger_by_primary_key(name=name, org_id=org_id)
         return cls(
             record=record,
             action_delegate=action_delegate,
             trigger_delegate=trigger_delegate,
         )
 
     @classmethod
     def query(
         cls,
-        filters: dict[str, Any] | None,
-        org_id: str | None,
+        filters: Optional[dict[str, Any]],
+        org_id: Optional[str],
         action_delegate: ActionDelegate,
         trigger_delegate: TriggerDelegate,
     ) -> collections.abc.Generator["Trigger", None, None]:
         paginated_results = trigger_delegate.query_triggers(
             filters=filters, org_id=org_id
         )
         while True:
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/users/http_delegate.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/users/http_delegate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
+from typing import Optional
+
 from ...http import (
     USER_OVERRIDE_HEADER,
     HttpClient,
 )
 from .user_delegate import UserDelegate
 from .user_record import UserRecord
 
@@ -11,23 +13,23 @@
 class UserHttpDelegate(UserDelegate):
     __http_client: HttpClient
 
     def __init__(self, http_client: HttpClient):
         super().__init__()
         self.__http_client = http_client
 
-    def get_user_by_id(self, user_id: str | None) -> UserRecord:
+    def get_user_by_id(self, user_id: Optional[str]) -> UserRecord:
         url = self.__http_client.url("v1/users")
         headers = {}
         if user_id is not None:
             headers[USER_OVERRIDE_HEADER] = user_id
 
         response = self.__http_client.get(url=url, headers=headers)
         return UserRecord.parse_obj(response.from_json(json_path=["data"]))
 
-    def delete_user(self, user_id: str | None) -> None:
+    def delete_user(self, user_id: Optional[str]) -> None:
         url = self.__http_client.url("v1/users")
         headers = {}
         if user_id is not None:
             headers[USER_OVERRIDE_HEADER] = user_id
 
         self.__http_client.delete(url=url, headers=headers)
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/users/user.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/users/user.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
-from typing import Any
+from typing import Any, Optional
 
 from ...serde import pydantic_jsonable_dict
 from .user_delegate import UserDelegate
 from .user_record import UserRecord
 
 
 class User:
     __record: UserRecord
     __user_delegate: UserDelegate
 
     @classmethod
-    def by_id(cls, user_id: str | None, user_delegate: UserDelegate):
+    def by_id(cls, user_id: Optional[str], user_delegate: UserDelegate):
         record = user_delegate.get_user_by_id(user_id=user_id)
         return cls(record=record, user_delegate=user_delegate)
 
     def __init__(self, record: UserRecord, user_delegate: UserDelegate):
         self.__record = record
         self.__user_delegate = user_delegate
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/http/__init__.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/http/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/http/request_decorators.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/http/request_decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 import os
+from typing import Optional
 
 import boto3
 from botocore.auth import SigV4Auth
 from botocore.awsrequest import AWSRequest
 from botocore.credentials import (
     ReadOnlyCredentials,
 )
@@ -74,16 +75,16 @@
         if not region:
             raise ValueError("One of AWS_REGION or AWS_DEFAULT_REGION must be set.")
         return region
 
     def __init__(
         self,
         service: str,
-        credentials: ReadOnlyCredentials | None = None,
-        region: str | None = None,
+        credentials: Optional[ReadOnlyCredentials] = None,
+        region: Optional[str] = None,
     ):
         self.__credentials = (
             credentials if credentials else SigV4AuthDecorator.lookup_credentials()
         )
         self.__region = region if region else SigV4AuthDecorator.lookup_region()
         self.__service = service
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/http/testing_util.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/http/testing_util.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     __url: str
 
     def __init__(
         self,
         url: str,
         response_data: typing.Any,
         status_code: int = 200,
-        headers: dict[str, str] | None = None,
+        headers: typing.Optional[dict[str, str]] = None,
     ) -> None:
         self.__status_code = status_code
         self.__headers = headers or dict()
         self.__response_data = response_data
         self.__url = url
 
     def __call__(self, *args, **kwargs) -> HttpResponse:
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/profile/profile.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/profile/profile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 import enum
 import json
 import os
 import pathlib
-from typing import Any
+from typing import Any, Optional
 
 import pydantic
 
 from ..logging import default_logger
 
 log = default_logger()
 
@@ -38,16 +38,16 @@
     __config_file: pathlib.Path
 
     def __init__(self, config_file: pathlib.Path = DEFAULT_ROBOTO_PROFILE_FILE):
         self.__config_file = config_file
 
     def __base_entry_from_file(
         self,
-        profile_name: str | None,
-    ) -> tuple[RobotoProfileFileType, RobotoProfileEntry | None]:
+        profile_name: Optional[str],
+    ) -> tuple[RobotoProfileFileType, Optional[RobotoProfileEntry]]:
         if not self.__config_file.is_file():
             return RobotoProfileFileType.none, None
 
         with open(self.__config_file, "r") as f:
             contents: dict[str, Any] = json.loads(f.read())
 
         profile_to_check = "default" if profile_name is None else profile_name
@@ -68,15 +68,15 @@
             )
         except pydantic.ValidationError:
             log.warning(
                 f"Couldn't parse {self.__config_file} as single-profile 'implicit' type"
             )
             return RobotoProfileFileType.malformed, None
 
-    def get_entry(self, profile_name: str | None = None) -> RobotoProfileEntry:
+    def get_entry(self, profile_name: Optional[str] = None) -> RobotoProfileEntry:
         profile_to_check = (
             profile_name
             if profile_name is not None
             else os.getenv(PROFILE_ENV_VAR, "default")
         )
         # TODO - Support AWS style order of precedence
         file_type, entry = self.__base_entry_from_file(profile_to_check)
```

### Comparing `roboto_sdk-0.1.3a1/src/roboto_sdk/serde.py` & `roboto_sdk-0.1.3a2/src/roboto_sdk/serde.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a1/PKG-INFO` & `roboto_sdk-0.1.3a2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: roboto-sdk
-Version: 0.1.3a1
+Version: 0.1.3a2
 Summary: Tools for interacting with roboto.ai
 License: MIT
 Author: Roboto
 Author-email: admin@roboto.ai
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3[crt] (>=1.26,<1.27)
 Requires-Dist: pathspec (>=0.11,<0.12)
 Requires-Dist: pydantic (>=1.10,<1.11)
 Requires-Dist: pyjwt (>=2.7,<2.8)
 Requires-Dist: tenacity (>=8.2,<8.3)
```

