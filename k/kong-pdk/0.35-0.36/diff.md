# Comparing `tmp/kong_pdk-0.35.tar.gz` & `tmp/kong_pdk-0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kong_pdk-0.35.tar", last modified: Tue Jun 20 08:11:51 2023, max compression
+gzip compressed data, was "kong_pdk-0.36.tar", last modified: Mon Jul  3 09:04:13 2023, max compression
```

## Comparing `kong_pdk-0.35.tar` & `kong_pdk-0.36.tar`

### file list

```diff
@@ -1,50 +1,53 @@
-drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-06-20 08:11:51.047006 kong_pdk-0.35/
--rw-r--r--   0 fffonion   (501) staff       (20)    11345 2021-03-22 08:08:14.000000 kong_pdk-0.35/LICENSE
--rw-r--r--   0 fffonion   (501) staff       (20)    11264 2023-06-20 08:11:51.047075 kong_pdk-0.35/PKG-INFO
--rw-r--r--   0 fffonion   (501) staff       (20)     2750 2022-10-20 08:28:19.000000 kong_pdk-0.35/README.md
-drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-06-20 08:11:51.042161 kong_pdk-0.35/kong_pdk/
--rw-r--r--   0 fffonion   (501) staff       (20)        0 2021-03-26 09:39:18.000000 kong_pdk-0.35/kong_pdk/__init__.py
--rw-r--r--   0 fffonion   (501) staff       (20)     6221 2022-10-07 10:57:34.000000 kong_pdk-0.35/kong_pdk/cli.py
--rw-r--r--   0 fffonion   (501) staff       (20)      661 2023-06-20 08:11:41.000000 kong_pdk-0.35/kong_pdk/const.py
--rw-r--r--   0 fffonion   (501) staff       (20)       90 2021-08-05 15:07:12.000000 kong_pdk-0.35/kong_pdk/exception.py
--rw-r--r--   0 fffonion   (501) staff       (20)       23 2021-08-05 15:07:12.000000 kong_pdk-0.35/kong_pdk/kong.py
--rw-r--r--   0 fffonion   (501) staff       (20)     4093 2023-06-20 04:09:23.000000 kong_pdk-0.35/kong_pdk/listener.py
--rw-r--r--   0 fffonion   (501) staff       (20)     5547 2021-08-05 15:07:12.000000 kong_pdk-0.35/kong_pdk/logger.py
--rw-r--r--   0 fffonion   (501) staff       (20)     2639 2022-10-07 10:57:34.000000 kong_pdk-0.35/kong_pdk/module.py
-drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-06-20 08:11:51.043361 kong_pdk-0.35/kong_pdk/pdk/
--rw-r--r--   0 fffonion   (501) staff       (20)     1427 2023-06-20 04:09:23.000000 kong_pdk-0.35/kong_pdk/pdk/__init__.py
-drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-06-20 08:11:51.045209 kong_pdk-0.35/kong_pdk/pdk/kong/
--rw-r--r--   0 fffonion   (501) staff       (20)     1233 2023-06-20 04:09:23.000000 kong_pdk-0.35/kong_pdk/pdk/kong/__init__.py
-drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-06-20 08:11:51.045508 kong_pdk-0.35/kong_pdk/pdk/kong/client/
--rw-r--r--   0 fffonion   (501) staff       (20)     8888 2023-06-20 04:09:23.000000 kong_pdk-0.35/kong_pdk/pdk/kong/client/__init__.py
--rw-r--r--   0 fffonion   (501) staff       (20)     4943 2023-06-20 04:09:23.000000 kong_pdk-0.35/kong_pdk/pdk/kong/client/tls.py
--rw-r--r--   0 fffonion   (501) staff       (20)     1205 2023-06-20 04:09:23.000000 kong_pdk-0.35/kong_pdk/pdk/kong/cluster.py
-drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-06-20 08:11:51.046041 kong_pdk-0.35/kong_pdk/pdk/kong/ctx/
--rw-r--r--   0 fffonion   (501) staff       (20)      376 2023-06-20 04:09:23.000000 kong_pdk-0.35/kong_pdk/pdk/kong/ctx/__init__.py
--rw-r--r--   0 fffonion   (501) staff       (20)      892 2023-06-20 04:09:23.000000 kong_pdk-0.35/kong_pdk/pdk/kong/ctx/shared.py
--rw-r--r--   0 fffonion   (501) staff       (20)      999 2023-06-20 04:09:23.000000 kong_pdk-0.35/kong_pdk/pdk/kong/ip.py
--rw-r--r--   0 fffonion   (501) staff       (20)    18220 2023-06-20 04:09:23.000000 kong_pdk-0.35/kong_pdk/pdk/kong/log.py
-drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-06-20 08:11:51.046385 kong_pdk-0.35/kong_pdk/pdk/kong/nginx/
--rw-r--r--   0 fffonion   (501) staff       (20)     3100 2023-06-20 04:09:23.000000 kong_pdk-0.35/kong_pdk/pdk/kong/nginx/__init__.py
--rw-r--r--   0 fffonion   (501) staff       (20)      894 2023-06-20 04:09:23.000000 kong_pdk-0.35/kong_pdk/pdk/kong/nginx/shared.py
--rw-r--r--   0 fffonion   (501) staff       (20)     3678 2023-06-20 04:09:23.000000 kong_pdk-0.35/kong_pdk/pdk/kong/node.py
--rw-r--r--   0 fffonion   (501) staff       (20)      699 2023-06-20 04:09:23.000000 kong_pdk-0.35/kong_pdk/pdk/kong/plugin.py
--rw-r--r--   0 fffonion   (501) staff       (20)    22936 2023-06-20 04:09:23.000000 kong_pdk-0.35/kong_pdk/pdk/kong/request.py
--rw-r--r--   0 fffonion   (501) staff       (20)    18572 2023-06-20 04:09:23.000000 kong_pdk-0.35/kong_pdk/pdk/kong/response.py
--rw-r--r--   0 fffonion   (501) staff       (20)     1281 2023-06-20 04:09:23.000000 kong_pdk-0.35/kong_pdk/pdk/kong/router.py
-drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-06-20 08:11:51.046866 kong_pdk-0.35/kong_pdk/pdk/kong/service/
--rw-r--r--   0 fffonion   (501) staff       (20)     4831 2023-06-20 04:09:23.000000 kong_pdk-0.35/kong_pdk/pdk/kong/service/__init__.py
--rw-r--r--   0 fffonion   (501) staff       (20)    13919 2023-06-20 04:09:23.000000 kong_pdk-0.35/kong_pdk/pdk/kong/service/request.py
--rw-r--r--   0 fffonion   (501) staff       (20)     5710 2023-06-20 04:09:23.000000 kong_pdk-0.35/kong_pdk/pdk/kong/service/response.py
--rw-r--r--   0 fffonion   (501) staff       (20)     4451 2023-06-20 04:09:23.000000 kong_pdk-0.35/kong_pdk/pdk/kong/vault.py
--rw-r--r--   0 fffonion   (501) staff       (20)    10729 2023-06-20 08:08:34.000000 kong_pdk-0.35/kong_pdk/server.py
-drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-06-20 08:11:51.043216 kong_pdk-0.35/kong_pdk.egg-info/
--rw-r--r--   0 fffonion   (501) staff       (20)    11264 2023-06-20 08:11:51.000000 kong_pdk-0.35/kong_pdk.egg-info/PKG-INFO
--rw-r--r--   0 fffonion   (501) staff       (20)     1052 2023-06-20 08:11:51.000000 kong_pdk-0.35/kong_pdk.egg-info/SOURCES.txt
--rw-r--r--   0 fffonion   (501) staff       (20)        1 2023-06-20 08:11:51.000000 kong_pdk-0.35/kong_pdk.egg-info/dependency_links.txt
--rw-r--r--   0 fffonion   (501) staff       (20)       71 2023-06-20 08:11:51.000000 kong_pdk-0.35/kong_pdk.egg-info/entry_points.txt
--rw-r--r--   0 fffonion   (501) staff       (20)        1 2021-03-26 09:39:30.000000 kong_pdk-0.35/kong_pdk.egg-info/not-zip-safe
--rw-r--r--   0 fffonion   (501) staff       (20)       15 2023-06-20 08:11:51.000000 kong_pdk-0.35/kong_pdk.egg-info/requires.txt
--rw-r--r--   0 fffonion   (501) staff       (20)      137 2023-06-20 08:11:51.000000 kong_pdk-0.35/kong_pdk.egg-info/top_level.txt
--rw-r--r--   0 fffonion   (501) staff       (20)      184 2023-06-20 08:11:51.047346 kong_pdk-0.35/setup.cfg
--rw-r--r--   0 fffonion   (501) staff       (20)     1999 2022-10-07 10:57:34.000000 kong_pdk-0.35/setup.py
+drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-07-03 09:04:13.680771 kong_pdk-0.36/
+-rw-r--r--   0 fffonion   (501) staff       (20)    11345 2021-03-22 08:08:14.000000 kong_pdk-0.36/LICENSE
+-rw-r--r--   0 fffonion   (501) staff       (20)    11677 2023-07-03 09:04:13.680863 kong_pdk-0.36/PKG-INFO
+-rw-r--r--   0 fffonion   (501) staff       (20)     2750 2023-06-27 06:41:55.000000 kong_pdk-0.36/README.md
+drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-07-03 09:04:13.675220 kong_pdk-0.36/kong_pdk/
+-rw-r--r--   0 fffonion   (501) staff       (20)        0 2021-03-26 09:39:18.000000 kong_pdk-0.36/kong_pdk/__init__.py
+-rw-r--r--   0 fffonion   (501) staff       (20)     6221 2023-06-27 06:41:55.000000 kong_pdk-0.36/kong_pdk/cli.py
+-rw-r--r--   0 fffonion   (501) staff       (20)      661 2023-07-03 09:04:01.000000 kong_pdk-0.36/kong_pdk/const.py
+-rw-r--r--   0 fffonion   (501) staff       (20)       90 2023-06-27 06:41:55.000000 kong_pdk-0.36/kong_pdk/exception.py
+-rw-r--r--   0 fffonion   (501) staff       (20)       23 2023-06-27 06:41:55.000000 kong_pdk-0.36/kong_pdk/kong.py
+-rw-r--r--   0 fffonion   (501) staff       (20)     4093 2023-06-27 06:41:55.000000 kong_pdk-0.36/kong_pdk/listener.py
+-rw-r--r--   0 fffonion   (501) staff       (20)     5547 2023-06-27 06:41:55.000000 kong_pdk-0.36/kong_pdk/logger.py
+-rw-r--r--   0 fffonion   (501) staff       (20)     2639 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/module.py
+drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-07-03 09:04:13.676980 kong_pdk-0.36/kong_pdk/pdk/
+-rw-r--r--   0 fffonion   (501) staff       (20)     1427 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/pdk/__init__.py
+drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-07-03 09:04:13.678614 kong_pdk-0.36/kong_pdk/pdk/kong/
+-rw-r--r--   0 fffonion   (501) staff       (20)     1233 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/pdk/kong/__init__.py
+drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-07-03 09:04:13.678920 kong_pdk-0.36/kong_pdk/pdk/kong/client/
+-rw-r--r--   0 fffonion   (501) staff       (20)     8888 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/pdk/kong/client/__init__.py
+-rw-r--r--   0 fffonion   (501) staff       (20)     4943 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/pdk/kong/client/tls.py
+-rw-r--r--   0 fffonion   (501) staff       (20)     1205 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/pdk/kong/cluster.py
+drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-07-03 09:04:13.679227 kong_pdk-0.36/kong_pdk/pdk/kong/ctx/
+-rw-r--r--   0 fffonion   (501) staff       (20)      376 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/pdk/kong/ctx/__init__.py
+-rw-r--r--   0 fffonion   (501) staff       (20)      892 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/pdk/kong/ctx/shared.py
+drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-07-03 09:04:13.679533 kong_pdk-0.36/kong_pdk/pdk/kong/enterprise_edition/
+-rw-r--r--   0 fffonion   (501) staff       (20)      391 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/pdk/kong/enterprise_edition/__init__.py
+-rw-r--r--   0 fffonion   (501) staff       (20)     6502 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/pdk/kong/enterprise_edition/jwe.py
+-rw-r--r--   0 fffonion   (501) staff       (20)      999 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/pdk/kong/ip.py
+-rw-r--r--   0 fffonion   (501) staff       (20)    18220 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/pdk/kong/log.py
+drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-07-03 09:04:13.679998 kong_pdk-0.36/kong_pdk/pdk/kong/nginx/
+-rw-r--r--   0 fffonion   (501) staff       (20)     3100 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/pdk/kong/nginx/__init__.py
+-rw-r--r--   0 fffonion   (501) staff       (20)      894 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/pdk/kong/nginx/shared.py
+-rw-r--r--   0 fffonion   (501) staff       (20)     3678 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/pdk/kong/node.py
+-rw-r--r--   0 fffonion   (501) staff       (20)      699 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/pdk/kong/plugin.py
+-rw-r--r--   0 fffonion   (501) staff       (20)    22936 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/pdk/kong/request.py
+-rw-r--r--   0 fffonion   (501) staff       (20)    18572 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/pdk/kong/response.py
+-rw-r--r--   0 fffonion   (501) staff       (20)     1281 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/pdk/kong/router.py
+drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-07-03 09:04:13.680598 kong_pdk-0.36/kong_pdk/pdk/kong/service/
+-rw-r--r--   0 fffonion   (501) staff       (20)     4831 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/pdk/kong/service/__init__.py
+-rw-r--r--   0 fffonion   (501) staff       (20)    13919 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/pdk/kong/service/request.py
+-rw-r--r--   0 fffonion   (501) staff       (20)     5710 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/pdk/kong/service/response.py
+-rw-r--r--   0 fffonion   (501) staff       (20)     4451 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/pdk/kong/vault.py
+-rw-r--r--   0 fffonion   (501) staff       (20)    10729 2023-06-27 06:41:56.000000 kong_pdk-0.36/kong_pdk/server.py
+drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-07-03 09:04:13.676817 kong_pdk-0.36/kong_pdk.egg-info/
+-rw-r--r--   0 fffonion   (501) staff       (20)    11677 2023-07-03 09:04:13.000000 kong_pdk-0.36/kong_pdk.egg-info/PKG-INFO
+-rw-r--r--   0 fffonion   (501) staff       (20)     1145 2023-07-03 09:04:13.000000 kong_pdk-0.36/kong_pdk.egg-info/SOURCES.txt
+-rw-r--r--   0 fffonion   (501) staff       (20)        1 2023-07-03 09:04:13.000000 kong_pdk-0.36/kong_pdk.egg-info/dependency_links.txt
+-rw-r--r--   0 fffonion   (501) staff       (20)       71 2023-07-03 09:04:13.000000 kong_pdk-0.36/kong_pdk.egg-info/entry_points.txt
+-rw-r--r--   0 fffonion   (501) staff       (20)        1 2021-03-26 09:39:30.000000 kong_pdk-0.36/kong_pdk.egg-info/not-zip-safe
+-rw-r--r--   0 fffonion   (501) staff       (20)       15 2023-07-03 09:04:13.000000 kong_pdk-0.36/kong_pdk.egg-info/requires.txt
+-rw-r--r--   0 fffonion   (501) staff       (20)      174 2023-07-03 09:04:13.000000 kong_pdk-0.36/kong_pdk.egg-info/top_level.txt
+-rw-r--r--   0 fffonion   (501) staff       (20)      184 2023-07-03 09:04:13.681362 kong_pdk-0.36/setup.cfg
+-rw-r--r--   0 fffonion   (501) staff       (20)     2043 2023-07-03 09:04:01.000000 kong_pdk-0.36/setup.py
```

### Comparing `kong_pdk-0.35/LICENSE` & `kong_pdk-0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/PKG-INFO` & `kong_pdk-0.36/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kong_pdk
-Version: 0.35
+Version: 0.36
 Summary: Kong PDK for Python and Plugin Server
 Home-page: https://github.com/Kong/kong-python-pdk
 Author: Kong
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
@@ -105,14 +105,20 @@
 - Hot reload
 
 
 <a name="unreleased"></a>
 ## [Unreleased]
 
 
+<a name="0.3.6"></a>
+## [0.3.6] - 2023-06-27
+### bug fixes
+- add missing file enterprise_edition [e8d7c86](https://github.com/Kong/kong-python-pdk/commit/e8d7c86a533c81e988308c7dd252d98544304a78)
+
+
 <a name="0.3.5"></a>
 ## [0.3.5] - 2023-06-20
 ### bug fixes
 - delete message queue when they are not needed any more ([#122](https://github.com/Kong/kong-python-pdk/issues/122)) [ffeb2f2](https://github.com/Kong/kong-python-pdk/commit/ffeb2f2185a107f0e6547c4336905fe5dd01bfd0)
 
 
 <a name="0.3.4"></a>
@@ -157,14 +163,15 @@
 ### bug fixes
 - listener to use msgpack.Unpacker iterrator [bed56c4](https://github.com/Kong/kong-python-pdk/commit/bed56c49160d1adb0e591f69b74337ced7820dba)
 
 
 <a name="0.2.5"></a>
 ## [0.2.5] - 2021-06-24
 ### bug fixes
+- listener to use msgpack.Unpacker iterrator [bed56c4](https://github.com/Kong/kong-python-pdk/commit/bed56c49160d1adb0e591f69b74337ced7820dba)
 - use .py file for type hint ([#13](https://github.com/Kong/kong-python-pdk/issues/13)) [1bf3820](https://github.com/Kong/kong-python-pdk/commit/1bf3820e316f73d6021897b5979af4826e9f34d6)
 
 
 <a name="0.2.4"></a>
 ## [0.2.4] - 2021-06-17
 ### bug fixes
 - check correct flags existence in dedicated server ([#10](https://github.com/Kong/kong-python-pdk/issues/10)) [b18dd45](https://github.com/Kong/kong-python-pdk/commit/b18dd458def039a6a2dad4c42baa7b55d64fe027)
@@ -225,15 +232,16 @@
 
 <a name="0.1.1"></a>
 ## [0.1.1] - 2020-02-20
 
 <a name="0.1.0"></a>
 ## 0.1.0 - 2020-01-03
 
-[Unreleased]: https://github.com/Kong/kong-python-pdk/compare/0.3.5...HEAD
+[Unreleased]: https://github.com/Kong/kong-python-pdk/compare/0.3.6...HEAD
+[0.3.6]: https://github.com/Kong/kong-python-pdk/compare/0.3.5...0.3.6
 [0.3.5]: https://github.com/Kong/kong-python-pdk/compare/0.3.4...0.3.5
 [0.3.4]: https://github.com/Kong/kong-python-pdk/compare/0.3.2...0.3.4
 [0.3.2]: https://github.com/Kong/kong-python-pdk/compare/0.3.1...0.3.2
 [0.3.1]: https://github.com/Kong/kong-python-pdk/compare/0.3.0...0.3.1
 [0.3.0]: https://github.com/Kong/kong-python-pdk/compare/0.2.7...0.3.0
 [0.2.7]: https://github.com/Kong/kong-python-pdk/compare/0.2.6...0.2.7
 [0.2.6]: https://github.com/Kong/kong-python-pdk/compare/0.2.5...0.2.6
```

### Comparing `kong_pdk-0.35/README.md` & `kong_pdk-0.36/README.md`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/cli.py` & `kong_pdk-0.36/kong_pdk/cli.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/const.py` & `kong_pdk-0.36/kong_pdk/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 PY3K = sys.version_info.major == 3
 IRONPYTHON = sys.platform == 'cli'
 EXEBUNDLE = getattr(sys, 'frozen', False)
 LOCALE = locale.getdefaultlocale()[0]
 CODEPAGE = locale.getdefaultlocale()[1] or 'ascii'
 
-__version__ = 0.35
+__version__ = 0.36
 
 # https://github.com/soimort/you-get/you-get
 if getattr(sys, 'frozen', False):
     # The application is frozen
     FILEPATH = os.path.dirname(os.path.realpath(sys.executable))
 else:
     # The application is not frozen
```

### Comparing `kong_pdk-0.35/kong_pdk/listener.py` & `kong_pdk-0.36/kong_pdk/listener.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/logger.py` & `kong_pdk-0.36/kong_pdk/logger.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/module.py` & `kong_pdk-0.36/kong_pdk/module.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/pdk/__init__.py` & `kong_pdk-0.36/kong_pdk/pdk/__init__.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/pdk/kong/__init__.py` & `kong_pdk-0.36/kong_pdk/pdk/kong/__init__.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/pdk/kong/client/__init__.py` & `kong_pdk-0.36/kong_pdk/pdk/kong/client/__init__.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/pdk/kong/client/tls.py` & `kong_pdk-0.36/kong_pdk/pdk/kong/client/tls.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/pdk/kong/cluster.py` & `kong_pdk-0.36/kong_pdk/pdk/kong/cluster.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/pdk/kong/ctx/shared.py` & `kong_pdk-0.36/kong_pdk/pdk/kong/ctx/shared.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/pdk/kong/ip.py` & `kong_pdk-0.36/kong_pdk/pdk/kong/ip.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/pdk/kong/log.py` & `kong_pdk-0.36/kong_pdk/pdk/kong/log.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/pdk/kong/nginx/__init__.py` & `kong_pdk-0.36/kong_pdk/pdk/kong/nginx/__init__.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/pdk/kong/nginx/shared.py` & `kong_pdk-0.36/kong_pdk/pdk/kong/nginx/shared.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/pdk/kong/node.py` & `kong_pdk-0.36/kong_pdk/pdk/kong/node.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/pdk/kong/plugin.py` & `kong_pdk-0.36/kong_pdk/pdk/kong/plugin.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/pdk/kong/request.py` & `kong_pdk-0.36/kong_pdk/pdk/kong/request.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/pdk/kong/response.py` & `kong_pdk-0.36/kong_pdk/pdk/kong/response.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/pdk/kong/router.py` & `kong_pdk-0.36/kong_pdk/pdk/kong/router.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/pdk/kong/service/__init__.py` & `kong_pdk-0.36/kong_pdk/pdk/kong/service/__init__.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/pdk/kong/service/request.py` & `kong_pdk-0.36/kong_pdk/pdk/kong/service/request.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/pdk/kong/service/response.py` & `kong_pdk-0.36/kong_pdk/pdk/kong/service/response.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/pdk/kong/vault.py` & `kong_pdk-0.36/kong_pdk/pdk/kong/vault.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk/server.py` & `kong_pdk-0.36/kong_pdk/server.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.35/kong_pdk.egg-info/PKG-INFO` & `kong_pdk-0.36/kong_pdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kong-pdk
-Version: 0.35
+Version: 0.36
 Summary: Kong PDK for Python and Plugin Server
 Home-page: https://github.com/Kong/kong-python-pdk
 Author: Kong
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
@@ -105,14 +105,20 @@
 - Hot reload
 
 
 <a name="unreleased"></a>
 ## [Unreleased]
 
 
+<a name="0.3.6"></a>
+## [0.3.6] - 2023-06-27
+### bug fixes
+- add missing file enterprise_edition [e8d7c86](https://github.com/Kong/kong-python-pdk/commit/e8d7c86a533c81e988308c7dd252d98544304a78)
+
+
 <a name="0.3.5"></a>
 ## [0.3.5] - 2023-06-20
 ### bug fixes
 - delete message queue when they are not needed any more ([#122](https://github.com/Kong/kong-python-pdk/issues/122)) [ffeb2f2](https://github.com/Kong/kong-python-pdk/commit/ffeb2f2185a107f0e6547c4336905fe5dd01bfd0)
 
 
 <a name="0.3.4"></a>
@@ -157,14 +163,15 @@
 ### bug fixes
 - listener to use msgpack.Unpacker iterrator [bed56c4](https://github.com/Kong/kong-python-pdk/commit/bed56c49160d1adb0e591f69b74337ced7820dba)
 
 
 <a name="0.2.5"></a>
 ## [0.2.5] - 2021-06-24
 ### bug fixes
+- listener to use msgpack.Unpacker iterrator [bed56c4](https://github.com/Kong/kong-python-pdk/commit/bed56c49160d1adb0e591f69b74337ced7820dba)
 - use .py file for type hint ([#13](https://github.com/Kong/kong-python-pdk/issues/13)) [1bf3820](https://github.com/Kong/kong-python-pdk/commit/1bf3820e316f73d6021897b5979af4826e9f34d6)
 
 
 <a name="0.2.4"></a>
 ## [0.2.4] - 2021-06-17
 ### bug fixes
 - check correct flags existence in dedicated server ([#10](https://github.com/Kong/kong-python-pdk/issues/10)) [b18dd45](https://github.com/Kong/kong-python-pdk/commit/b18dd458def039a6a2dad4c42baa7b55d64fe027)
@@ -225,15 +232,16 @@
 
 <a name="0.1.1"></a>
 ## [0.1.1] - 2020-02-20
 
 <a name="0.1.0"></a>
 ## 0.1.0 - 2020-01-03
 
-[Unreleased]: https://github.com/Kong/kong-python-pdk/compare/0.3.5...HEAD
+[Unreleased]: https://github.com/Kong/kong-python-pdk/compare/0.3.6...HEAD
+[0.3.6]: https://github.com/Kong/kong-python-pdk/compare/0.3.5...0.3.6
 [0.3.5]: https://github.com/Kong/kong-python-pdk/compare/0.3.4...0.3.5
 [0.3.4]: https://github.com/Kong/kong-python-pdk/compare/0.3.2...0.3.4
 [0.3.2]: https://github.com/Kong/kong-python-pdk/compare/0.3.1...0.3.2
 [0.3.1]: https://github.com/Kong/kong-python-pdk/compare/0.3.0...0.3.1
 [0.3.0]: https://github.com/Kong/kong-python-pdk/compare/0.2.7...0.3.0
 [0.2.7]: https://github.com/Kong/kong-python-pdk/compare/0.2.6...0.2.7
 [0.2.6]: https://github.com/Kong/kong-python-pdk/compare/0.2.5...0.2.6
```

### Comparing `kong_pdk-0.35/kong_pdk.egg-info/SOURCES.txt` & `kong_pdk-0.36/kong_pdk.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -29,12 +29,14 @@
 kong_pdk/pdk/kong/response.py
 kong_pdk/pdk/kong/router.py
 kong_pdk/pdk/kong/vault.py
 kong_pdk/pdk/kong/client/__init__.py
 kong_pdk/pdk/kong/client/tls.py
 kong_pdk/pdk/kong/ctx/__init__.py
 kong_pdk/pdk/kong/ctx/shared.py
+kong_pdk/pdk/kong/enterprise_edition/__init__.py
+kong_pdk/pdk/kong/enterprise_edition/jwe.py
 kong_pdk/pdk/kong/nginx/__init__.py
 kong_pdk/pdk/kong/nginx/shared.py
 kong_pdk/pdk/kong/service/__init__.py
 kong_pdk/pdk/kong/service/request.py
 kong_pdk/pdk/kong/service/response.py
```

### Comparing `kong_pdk-0.35/setup.py` & `kong_pdk-0.36/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     'kong_pdk',
     'kong_pdk/pdk',
     'kong_pdk/pdk/kong',
     'kong_pdk/pdk/kong/client',
     'kong_pdk/pdk/kong/ctx',
     'kong_pdk/pdk/kong/nginx',
     'kong_pdk/pdk/kong/service',
+    'kong_pdk/pdk/kong/enterprise_edition',
 ]
 requires = ['gevent', 'msgpack']
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description='Kong PDK for Python and Plugin Server',
```

