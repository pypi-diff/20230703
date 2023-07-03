# Comparing `tmp/damo-1.8.7.tar.gz` & `tmp/damo-1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-1.8.7.tar", last modified: Mon Jun 26 17:48:13 2023, max compression
+gzip compressed data, was "damo-1.8.8.tar", last modified: Mon Jul  3 17:22:48 2023, max compression
```

## Comparing `damo-1.8.7.tar` & `damo-1.8.8.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-26 17:48:13.863841 damo-1.8.7/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8162 2023-06-26 17:48:13.863841 damo-1.8.7/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7641 2023-06-26 17:48:09.000000 damo-1.8.7/README.md
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2022-04-22 09:53:30.000000 damo-1.8.7/pyproject.toml
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-06-26 17:48:13.863841 damo-1.8.7/setup.cfg
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-13 14:44:13.000000 damo-1.8.7/setup.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-26 17:48:13.839842 damo-1.8.7/src/
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-26 17:48:13.859841 damo-1.8.7/src/damo/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-06-26 17:48:09.000000 damo-1.8.7/src/damo/__init__.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7358 2023-06-04 17:35:27.000000 damo-1.8.7/src/damo/_damo_deprecated.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-05-21 19:11:52.000000 damo-1.8.7/src/damo/_damo_deprecation_notice.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/_damo_dist.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9673 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/_damo_fmt_str.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/_damo_fs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/_damo_paddr_layout.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/_damo_subcmds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    34675 2023-06-17 18:34:52.000000 damo-1.8.7/src/damo/_damon.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    11111 2023-06-25 18:34:34.000000 damo-1.8.7/src/damo/_damon_args.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    16293 2023-06-24 19:25:59.000000 damo-1.8.7/src/damo/_damon_dbgfs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    23604 2023-06-25 18:16:50.000000 damo-1.8.7/src/damo/_damon_result.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19134 2023-06-04 19:28:46.000000 damo-1.8.7/src/damo/_damon_sysfs.py
--rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3992 2023-06-25 17:52:33.000000 damo-1.8.7/src/damo/damo.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2023 2023-06-18 17:20:10.000000 damo-1.8.7/src/damo/damo_adjust.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      892 2023-06-18 18:06:08.000000 damo-1.8.7/src/damo/damo_convert_record_format.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/damo_features.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/damo_fmt_json.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13386 2023-06-18 17:39:30.000000 damo-1.8.7/src/damo/damo_heats.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/damo_lru_sort.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3029 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/damo_monitor.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2743 2023-06-18 17:30:14.000000 damo-1.8.7/src/damo/damo_nr_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/damo_reclaim.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5725 2023-06-25 17:13:05.000000 damo-1.8.7/src/damo/damo_record.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4094 2023-06-18 17:31:57.000000 damo-1.8.7/src/damo/damo_record_info.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1173 2023-06-04 19:50:04.000000 damo-1.8.7/src/damo/damo_report.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3766 2023-06-24 18:02:53.000000 damo-1.8.7/src/damo/damo_report_raw.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1511 2023-06-17 18:37:36.000000 damo-1.8.7/src/damo/damo_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5105 2023-06-25 18:54:44.000000 damo-1.8.7/src/damo/damo_show.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      542 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/damo_start.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2383 2023-06-10 19:35:18.000000 damo-1.8.7/src/damo/damo_stat.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1058 2023-06-25 17:28:02.000000 damo-1.8.7/src/damo/damo_stat_kdamonds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2956 2023-06-18 18:12:17.000000 damo-1.8.7/src/damo/damo_stat_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1001 2023-06-25 17:28:02.000000 damo-1.8.7/src/damo/damo_stat_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3354 2023-06-25 17:28:02.000000 damo-1.8.7/src/damo/damo_status.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      654 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/damo_stop.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      865 2023-05-29 19:12:16.000000 damo-1.8.7/src/damo/damo_translate_damos.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-05-20 19:08:28.000000 damo-1.8.7/src/damo/damo_tune.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3930 2023-06-18 17:35:51.000000 damo-1.8.7/src/damo/damo_validate.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-06-26 17:47:10.000000 damo-1.8.7/src/damo/damo_version.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5551 2023-06-18 17:22:23.000000 damo-1.8.7/src/damo/damo_wss.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-26 17:48:13.859841 damo-1.8.7/src/damo.egg-info/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8162 2023-06-26 17:48:13.000000 damo-1.8.7/src/damo.egg-info/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1249 2023-06-26 17:48:13.000000 damo-1.8.7/src/damo.egg-info/SOURCES.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-06-26 17:48:13.000000 damo-1.8.7/src/damo.egg-info/dependency_links.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-06-26 17:48:13.000000 damo-1.8.7/src/damo.egg-info/entry_points.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-06-26 17:48:13.000000 damo-1.8.7/src/damo.egg-info/top_level.txt
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-03 17:22:48.400680 damo-1.8.8/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8360 2023-07-03 17:22:48.396680 damo-1.8.8/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7839 2023-07-03 17:22:44.000000 damo-1.8.8/README.md
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2022-04-22 09:53:30.000000 damo-1.8.8/pyproject.toml
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-07-03 17:22:48.400680 damo-1.8.8/setup.cfg
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-13 14:44:13.000000 damo-1.8.8/setup.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-03 17:22:48.380680 damo-1.8.8/src/
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-03 17:22:48.396680 damo-1.8.8/src/damo/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-07-03 17:22:44.000000 damo-1.8.8/src/damo/__init__.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7358 2023-06-04 17:35:27.000000 damo-1.8.8/src/damo/_damo_deprecated.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-05-21 19:11:52.000000 damo-1.8.8/src/damo/_damo_deprecation_notice.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/_damo_dist.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9673 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/_damo_fmt_str.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/_damo_fs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/_damo_paddr_layout.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/_damo_subcmds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    35325 2023-07-02 19:16:32.000000 damo-1.8.8/src/damo/_damon.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    11832 2023-07-02 17:35:49.000000 damo-1.8.8/src/damo/_damon_args.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    16293 2023-06-24 19:25:59.000000 damo-1.8.8/src/damo/_damon_dbgfs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    26299 2023-07-02 19:16:32.000000 damo-1.8.8/src/damo/_damon_result.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19598 2023-07-02 18:42:47.000000 damo-1.8.8/src/damo/_damon_sysfs.py
+-rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3992 2023-06-25 17:52:33.000000 damo-1.8.8/src/damo/damo.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2023 2023-06-18 17:20:10.000000 damo-1.8.8/src/damo/damo_adjust.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      892 2023-06-18 18:06:08.000000 damo-1.8.8/src/damo/damo_convert_record_format.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/damo_features.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/damo_fmt_json.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13386 2023-06-18 17:39:30.000000 damo-1.8.8/src/damo/damo_heats.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/damo_lru_sort.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3029 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/damo_monitor.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2743 2023-06-18 17:30:14.000000 damo-1.8.8/src/damo/damo_nr_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/damo_reclaim.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5725 2023-06-25 17:13:05.000000 damo-1.8.8/src/damo/damo_record.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4094 2023-06-18 17:31:57.000000 damo-1.8.8/src/damo/damo_record_info.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1173 2023-06-04 19:50:04.000000 damo-1.8.8/src/damo/damo_report.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3766 2023-06-24 18:02:53.000000 damo-1.8.8/src/damo/damo_report_raw.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1511 2023-06-17 18:37:36.000000 damo-1.8.8/src/damo/damo_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7610 2023-07-02 19:16:32.000000 damo-1.8.8/src/damo/damo_show.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      542 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/damo_start.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2383 2023-06-10 19:35:18.000000 damo-1.8.8/src/damo/damo_stat.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1044 2023-07-02 19:29:16.000000 damo-1.8.8/src/damo/damo_stat_kdamonds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3150 2023-07-02 19:28:36.000000 damo-1.8.8/src/damo/damo_stat_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      987 2023-07-02 19:29:03.000000 damo-1.8.8/src/damo/damo_stat_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3354 2023-06-25 17:28:02.000000 damo-1.8.8/src/damo/damo_status.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      654 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/damo_stop.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      865 2023-05-29 19:12:16.000000 damo-1.8.8/src/damo/damo_translate_damos.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-05-20 19:08:28.000000 damo-1.8.8/src/damo/damo_tune.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3930 2023-06-18 17:35:51.000000 damo-1.8.8/src/damo/damo_validate.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-07-03 17:21:47.000000 damo-1.8.8/src/damo/damo_version.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5551 2023-06-18 17:22:23.000000 damo-1.8.8/src/damo/damo_wss.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-03 17:22:48.396680 damo-1.8.8/src/damo.egg-info/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8360 2023-07-03 17:22:48.000000 damo-1.8.8/src/damo.egg-info/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1249 2023-07-03 17:22:48.000000 damo-1.8.8/src/damo.egg-info/SOURCES.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-07-03 17:22:48.000000 damo-1.8.8/src/damo.egg-info/dependency_links.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-07-03 17:22:48.000000 damo-1.8.8/src/damo.egg-info/entry_points.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-07-03 17:22:48.000000 damo-1.8.8/src/damo.egg-info/top_level.txt
```

### Comparing `damo-1.8.7/PKG-INFO` & `damo-1.8.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.8.7
+Version: 1.8.8
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -32,26 +32,29 @@
 http://www.youtube.com/watch?v=l63eqbVBZRY
 "DAMON: a demo for the Kernel Summit 2020")
 
 
 Getting Started
 ===============
 
+[![Packaging status](https://repology.org/badge/vertical-allrepos/damo.svg)](https://repology.org/project/damo/versions)
+
 Follow below instructions and commands to monitor and visualize the access
 pattern of your workload.
 
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
+    $ # install from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.7/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.7/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.8/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.8/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +62,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.7/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.8/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -87,19 +90,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.7/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.8/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.7/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.8/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
@@ -184,16 +187,16 @@
 
 Deprecated.  Use Python3.
 
 For some old distros, DAMO initially supported Python2.  Because Python2 is
 really old now, the support has deprecated.  Please use Python3 or newer.
 
 
-DAMOS singline format
----------------------
+DAMOS single line format
+------------------------
 
 Deprecated.  Use `--damos_*` command line options or json format input.
 
 One-line scheme specification format like below was initially supported.
 Because it is not flexible for extension of features, it has deprecated now.
 You may use `--damos_*` command line options or json format instead.  You may
 use `damo translate_damos` to convert your old single line DAMOS schemes
```

### Comparing `damo-1.8.7/README.md` & `damo-1.8.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -17,26 +17,29 @@
 http://www.youtube.com/watch?v=l63eqbVBZRY
 "DAMON: a demo for the Kernel Summit 2020")
 
 
 Getting Started
 ===============
 
+[![Packaging status](https://repology.org/badge/vertical-allrepos/damo.svg)](https://repology.org/project/damo/versions)
+
 Follow below instructions and commands to monitor and visualize the access
 pattern of your workload.
 
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
+    $ # install from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.7/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.7/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.8/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.8/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -44,15 +47,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.7/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.8/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -72,19 +75,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.7/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.8/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.7/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.8/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
@@ -169,16 +172,16 @@
 
 Deprecated.  Use Python3.
 
 For some old distros, DAMO initially supported Python2.  Because Python2 is
 really old now, the support has deprecated.  Please use Python3 or newer.
 
 
-DAMOS singline format
----------------------
+DAMOS single line format
+------------------------
 
 Deprecated.  Use `--damos_*` command line options or json format input.
 
 One-line scheme specification format like below was initially supported.
 Because it is not flexible for extension of features, it has deprecated now.
 You may use `--damos_*` command line options or json format instead.  You may
 use `damo translate_damos` to convert your old single line DAMOS schemes
```

### Comparing `damo-1.8.7/setup.py` & `damo-1.8.8/setup.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/_damo_deprecated.py` & `damo-1.8.8/src/damo/_damo_deprecated.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/_damo_deprecation_notice.py` & `damo-1.8.8/src/damo/_damo_deprecation_notice.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/_damo_dist.py` & `damo-1.8.8/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/_damo_fmt_str.py` & `damo-1.8.8/src/damo/_damo_fmt_str.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/_damo_fs.py` & `damo-1.8.8/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/_damo_paddr_layout.py` & `damo-1.8.8/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/_damo_subcmds.py` & `damo-1.8.8/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/_damon.py` & `damo-1.8.8/src/damo/_damon.py`

 * *Files 0% similar despite different names*

```diff
@@ -614,30 +614,40 @@
     access_pattern = None
     action = None
     quotas = None
     watermarks = None
     filters = None
     stats = None
     tried_regions = None
+    tried_bytes = None
 
     # for monitoring only by default
     def __init__(self, access_pattern=None, action=damos_action_stat,
             quotas=None, watermarks=None, filters=None, stats=None,
-            tried_regions=None):
+            tried_regions=None, tried_bytes=None):
         self.access_pattern = (access_pattern
                 if access_pattern != None else DamosAccessPattern())
         if not action in damos_actions:
             raise Exception('wrong damos action: %s' % action)
         self.action = action
         self.quotas = quotas if quotas != None else DamosQuotas()
         self.watermarks = (watermarks
                 if watermarks != None else DamosWatermarks())
         self.filters = filters if filters != None else []
         self.stats = stats
         self.tried_regions = tried_regions
+        if self.tried_regions == None:
+            self.tried_regions = []
+        self.tried_bytes = 0
+        if tried_bytes:
+            self.tried_bytes = _damo_fmt_str.text_to_bytes(
+                    tried_bytes)
+        else:
+            for region in self.tried_regions:
+                self.tried_bytes += (region.end - region.start)
 
     def to_str(self, raw):
         lines = ['action: %s' % self.action]
         lines.append('target access pattern')
         lines.append(_damo_fmt_str.indent_lines(
             self.access_pattern.to_str(raw), 4))
         lines.append('quotas')
@@ -649,15 +659,16 @@
             lines.append('filter %d' % idx)
             lines.append(_damo_fmt_str.indent_lines(
                 damos_filter.to_str(raw), 4))
         if self.stats != None:
             lines.append('statistics')
             lines.append(_damo_fmt_str.indent_lines(self.stats.to_str(raw), 4))
         if self.tried_regions != None:
-            lines.append('tried regions')
+            lines.append('tried regions (%s)' % _damo_fmt_str.format_sz(
+                    self.tried_bytes, raw))
             for region in self.tried_regions:
                 lines.append(_damo_fmt_str.indent_lines(region.to_str(raw), 4))
         return '\n'.join(lines)
 
     def __str__(self):
         return self.to_str(False)
 
@@ -907,14 +918,19 @@
     return None
 
 def update_schemes_stats(kdamond_idxs=None):
     if kdamond_idxs == None:
         kdamond_idxs = running_kdamond_idxs()
     return _damon_fs.update_schemes_stats(kdamond_idxs)
 
+def update_schemes_tried_bytes(kdamond_idxs=None):
+    if kdamond_idxs == None:
+        kdamond_idxs = running_kdamond_idxs()
+    return _damon_fs.update_schemes_tried_bytes(kdamond_idxs)
+
 def update_schemes_tried_regions(kdamond_idxs=None):
     if kdamond_idxs == None:
         kdamond_idxs = running_kdamond_idxs()
     return _damon_fs.update_schemes_tried_regions(kdamond_idxs)
 
 def update_schemes_status(stats=True, tried_regions=True):
     '''Returns error string or None'''
```

### Comparing `damo-1.8.7/src/damo/_damon_args.py` & `damo-1.8.8/src/damo/_damon_args.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,46 +159,65 @@
     try:
         pid = int(target)
         return target_type_pid
     except:
         pass
     return target_type_unknown
 
+def warn_option_override(option_name):
+    print('warning: %s is overriden by <deducible target>' % option_name)
+
 def deduce_target_update_args(args):
     args.self_started_target = False
     target_type = deduced_target_type(args.deducible_target)
     if target_type == target_type_unknown:
         return 'target \'%s\' is not supported' % args.deducible_target
     if target_type == target_type_explict and args.deducible_target == 'paddr':
+        if not args.ops in ['paddr', None]:
+            warn_option_override('--ops')
         args.ops = 'paddr'
+        if args.target_pid != None:
+            warn_option_override('--target_pid')
         args.target_pid = None
         return None
     if target_type == target_type_cmd:
         p = subprocess.Popen(args.deducible_target, shell=True,
                 executable='/bin/bash')
         pid = p.pid
         args.self_started_target = True
     elif target_type == target_type_pid:
         pid = int(args.deducible_target)
+    if args.target_pid != None:
+        print('warning: --target_pid will be ignored')
     args.target_pid = pid
-    args.ops = 'vaddr'
+    if not args.regions:
+        if not args.ops in ['vaddr', None]:
+            warn_option_override('--ops')
+        args.ops = 'vaddr'
     if args.regions:
+        if not args.ops in ['fvaddr', None]:
+            print('warning: override --ops by <deducible target> and --regions')
         args.ops = 'fvaddr'
 
 def kdamonds_for(args):
     if args.kdamonds:
         return kdamonds_from_json_arg(args.kdamonds)
 
     if args.deducible_target:
         kdamonds, e = kdamonds_from_json_arg(args.deducible_target)
         if e == None:
             return kdamonds, e
         err = deduce_target_update_args(args)
         if err:
             return None, err
+    if args.ops == None:
+        if args.target_pid == None:
+            args.ops = 'paddr'
+        else:
+            args.ops = 'vaddr'
 
     ctx, err = damon_ctx_for(args)
     if err:
         return None, err
     return [_damon.Kdamond(state=None, pid=None, contexts=[ctx])], None
 
 def self_started_target(args):
@@ -288,15 +307,14 @@
             help='damos action to apply to the target regions')
 
 def set_argparser(parser, add_record_options):
     if parser == None:
         parser = argparse.ArgumentParser()
     set_monitoring_argparser(parser)
     parser.add_argument('--ops', choices=['vaddr', 'paddr', 'fvaddr'],
-            default='paddr',
             help='monitoring operations set')
     parser.add_argument('--target_pid', type=int, help='target pid')
     set_damos_argparser(parser)
     parser.add_argument('-c', '--schemes', metavar='<json string or file>',
 	    help='data access monitoring-based operation schemes')
     parser.add_argument('--kdamonds', metavar='<json string or file>',
             help='json format kdamonds specification to run DAMON for')
```

### Comparing `damo-1.8.7/src/damo/_damon_dbgfs.py` & `damo-1.8.8/src/damo/_damon_dbgfs.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/_damon_result.py` & `damo-1.8.8/src/damo/_damon_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 class DamonSnapshot:
     '''
     Contains a snapshot of data access monitoring results
     '''
     start_time = None
     end_time = None
     regions = None
+    total_bytes = None
 
     def __init__(self, start_time, end_time):
         self.start_time = start_time
         self.end_time = end_time
         self.regions = []
 
     @classmethod
@@ -609,34 +610,110 @@
         for ctx_idx, ctx in enumerate(kdamond.contexts):
             for scheme in ctx.schemes:
                 if not scheme.effectively_equal(monitor_scheme, ctx.intervals):
                     continue
 
                 snapshot = tried_regions_to_snapshot(scheme.tried_regions,
                         ctx.intervals)
+                snapshot.total_bytes = scheme.tried_bytes
 
                 records.append(DamonRecord(kdamond_idx, ctx_idx, ctx.intervals,
                     None, None))
                 records[-1].snapshots.append(snapshot)
                 break
     return records
 
-def get_snapshot_records(access_pattern):
+def three_regions_of(pid):
+    '''
+    Return three big mapped virtual address ranges of a given process, which
+    separated by the two huge gaps[1].
+
+    [1] https://docs.kernel.org/mm/damon/design.html#vma-based-target-address-range-construction
+    '''
+    if not os.path.isfile('/proc/%s/maps' % pid):
+        print('maps file for %s pid not found' % pid)
+        exit(0)
+    with open('/proc/%s/maps' % pid, 'r') as f:
+        maps_content = f.read()
+    regions = []
+    for line in maps_content.split('\n'):
+        if line == '':
+            continue
+        start, end = [int(addr, 16) for addr in line.split()[0].split('-')]
+        if len(regions) > 0 and regions[-1].end == start:
+            regions[-1].end = end
+        else:
+            regions.append(_damon.DamonRegion(start, end))
+
+    gaps = []
+    for idx, region in enumerate(regions):
+        if idx == 0:
+            continue
+        prev_region = regions[idx - 1]
+        if region.start != prev_region.end:
+            gaps.append([prev_region.end, region.start])
+    gaps.sort(key=lambda x: x[1] - x[0], reverse=True)
+    if len(gaps) < 2:
+        return regions
+    # sort biggest two gaps in address
+    gaps = sorted(gaps[:2], key=lambda x: x[0])
+
+    return [_damon.DamonRegion(regions[0].start, gaps[0][0]),
+            _damon.DamonRegion(gaps[0][1], gaps[1][0]),
+            _damon.DamonRegion(gaps[1][1], regions[-1].end)]
+
+def install_target_regions_if_needed(kdamonds):
+    '''Returns an error string, or None'''
+    need_install = False
+    for kd in kdamonds:
+        for ctx in kd.contexts:
+            if ctx.ops != 'vaddr':
+                continue
+            need_install = True
+            for target in ctx.targets:
+                target.regions = three_regions_of(target.pid)
+    if not need_install:
+        return None
+    err = _damon.commit(kdamonds)
+    for kd in kdamonds:
+        for ctx in kd.contexts:
+            if ctx.ops != 'vaddr':
+                continue
+            for target in ctx.targets:
+                target.regions = []
+    return err
+
+def get_snapshot_records(access_pattern, total_sz_only):
     'return DamonRecord objects each having single DamonSnapshot and an error'
     running_kdamond_idxs = _damon.running_kdamond_idxs()
     if len(running_kdamond_idxs) == 0:
         return None, 'no kdamond running'
 
     orig_kdamonds = _damon.current_kdamonds()
 
+    err = install_target_regions_if_needed(orig_kdamonds)
+    if err != None:
+        return None, 'vaddr region install failed (%s)' % err
+
     monitor_scheme = _damon.Damos(access_pattern=access_pattern)
     installed, err = install_scheme(monitor_scheme)
     if err:
         return None, 'monitoring scheme install failed: %s' % err
 
+    if total_sz_only:
+        err = _damon.update_schemes_tried_bytes(running_kdamond_idxs)
+        if err == None:
+            records = tried_regions_to_records(monitor_scheme)
+
+            if installed:
+                err = _damon.commit(orig_kdamonds)
+                if err:
+                    return records, 'monitoring scheme uninstall failed: %s' % err
+            return records, None
+
     err = _damon.update_schemes_tried_regions(running_kdamond_idxs)
     if err != None:
         if installed:
             err = _damon.commit(orig_kdamonds)
             if err:
                 return None, 'monitoring scheme uninstall failed: %s' % err
         return None, 'updating schemes tried regions fail: %s' % err
```

### Comparing `damo-1.8.7/src/damo/_damon_sysfs.py` & `damo-1.8.8/src/damo/_damon_sysfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,23 @@
         err = _damo_fs.write_file(
                 state_file_of(kdamond_idx), 'update_schemes_stats')
         if err != None:
             return err
     return None
 
 'Return error'
+def update_schemes_tried_bytes(kdamond_idxs):
+    for kdamond_idx in kdamond_idxs:
+        err = _damo_fs.write_file(
+                state_file_of(kdamond_idx), 'update_schemes_tried_bytes')
+        if err != None:
+            return err
+    return None
+
+'Return error'
 def update_schemes_tried_regions(kdamond_idxs):
     for kdamond_idx in kdamond_idxs:
         err = _damo_fs.write_file(
                 state_file_of(kdamond_idx), 'update_schemes_tried_regions')
         if err != None:
             return err
     return None
@@ -373,15 +382,18 @@
             files_content_to_quotas(files_content['quotas']),
             files_content_to_watermarks(files_content['watermarks']),
             files_content_to_damos_filters(files_content['filters'])
                 if 'filters' in files_content else [],
             files_content_to_damos_stats(files_content['stats']),
             files_content_to_damos_tried_regions(
                 files_content['tried_regions'])
-                if 'tried_regions' in files_content else [])
+                if 'tried_regions' in files_content else [],
+            files_content['tried_regions']['total_bytes']
+                if 'tried_regions' in files_content and
+                    'total_bytes' in files_content['tried_regions'] else None)
 
 def files_content_to_regions(files_content):
     return [_damon.DamonRegion(
             int(kv['start']), int(kv['end']))
             for kv in numbered_dirs_content(files_content, 'nr_regions')]
 
 def files_content_to_target(files_content):
```

### Comparing `damo-1.8.7/src/damo/damo.py` & `damo-1.8.8/src/damo/damo.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/damo_adjust.py` & `damo-1.8.8/src/damo/damo_adjust.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/damo_convert_record_format.py` & `damo-1.8.8/src/damo/damo_convert_record_format.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/damo_features.py` & `damo-1.8.8/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/damo_fmt_json.py` & `damo-1.8.8/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/damo_heats.py` & `damo-1.8.8/src/damo/damo_heats.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/damo_lru_sort.py` & `damo-1.8.8/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/damo_monitor.py` & `damo-1.8.8/src/damo/damo_monitor.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/damo_nr_regions.py` & `damo-1.8.8/src/damo/damo_nr_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/damo_reclaim.py` & `damo-1.8.8/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/damo_record.py` & `damo-1.8.8/src/damo/damo_record.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/damo_record_info.py` & `damo-1.8.8/src/damo/damo_record_info.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/damo_report.py` & `damo-1.8.8/src/damo/damo_report.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/damo_report_raw.py` & `damo-1.8.8/src/damo/damo_report_raw.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/damo_schemes.py` & `damo-1.8.8/src/damo/damo_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/damo_start.py` & `damo-1.8.8/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/damo_stat.py` & `damo-1.8.8/src/damo/damo_stat.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/damo_stat_kdamonds.py` & `damo-1.8.8/src/damo/damo_stat_kdamonds.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     if not args.detail:
         damo_status.update_pr_kdamonds_summary(args.json, args.raw)
     else:
         damo_status.update_pr_kdamonds(args.json, args.raw)
 
 def main(args=None):
     _damo_deprecation_notice.will_be_deprecated('\'damo stat kdamonds\'',
-            'near future', 'Use \'damo show status kdamonds\' instead')
+            'near future', 'Use \'damo status\' instead')
 
     if not args:
         parser = argparse.ArgumentParser()
         set_argparser(parser)
         args = parser.parse_args()
 
     _damon.ensure_root_and_initialized(args)
```

### Comparing `damo-1.8.7/src/damo/damo_stat_regions.py` & `damo-1.8.8/src/damo/damo_stat_regions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 
 import damo_stat
 
+import _damo_deprecation_notice
 import _damo_fmt_str
 import _damo_subcmds
 import _damon
 import _damon_result
 
 def priority(region, weights):
     if region.nr_accesses.samples > 0:
@@ -28,15 +29,16 @@
         else:
             total_sz += (region.end - region.start)
     if size_only:
         print('%s' % _damo_fmt_str.format_sz(total_sz, raw_nr))
 
 def update_pr_schemes_tried_regions(access_pattern, size_only, sortby,
         prio_weights, raw_nr):
-    records, err = _damon_result.get_snapshot_records(access_pattern)
+    records, err = _damon_result.get_snapshot_records(access_pattern,
+            total_sz_only=False)
     if err != None:
         print(err)
     if records == None:
         return
 
     for record in records:
         print('kdamond %s ctx %s' % (record.kdamond_idx, record.context_idx))
@@ -65,14 +67,16 @@
             help='priority weights for priority calculation')
 
 def __main(args):
     update_pr_schemes_tried_regions(args.access_pattern, args.size_only,
             args.sortby, args.priority_weights, args.raw)
 
 def main(args=None):
+    _damo_deprecation_notice.will_be_deprecated('\'damo stat regions\'',
+            'near future', 'Use \'damo show\' instead')
     if not args:
         parser = argparse.ArgumentParser()
         set_argparser(parser)
         args = parser.parse_args()
 
     _damon.ensure_root_and_initialized(args)
```

### Comparing `damo-1.8.7/src/damo/damo_stat_schemes.py` & `damo-1.8.8/src/damo/damo_stat_schemes.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     if args.stat_type == 'schemes_stats':
         damo_status.update_pr_schemes_stats(args.raw)
     elif args.stat_type == 'schemes_tried_regions':
         damo_status.update_pr_schemes_tried_regions(args.raw)
 
 def main(args=None):
     _damo_deprecation_notice.will_be_deprecated('\'damo stat schemes*\'',
-            'near future', 'Use \'damo show status schemes*\' instead')
+            'near future', 'Use \'damo status\' instead')
     if not args:
         parser = argparse.ArgumentParser()
         set_argparser(parser)
         args = parser.parse_args()
 
     _damon.ensure_root_and_initialized(args)
```

### Comparing `damo-1.8.7/src/damo/damo_status.py` & `damo-1.8.8/src/damo/damo_status.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/damo_stop.py` & `damo-1.8.8/src/damo/damo_stop.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/damo_translate_damos.py` & `damo-1.8.8/src/damo/damo_translate_damos.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/damo_tune.py` & `damo-1.8.8/src/damo/damo_tune.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/damo_validate.py` & `damo-1.8.8/src/damo/damo_validate.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo/damo_wss.py` & `damo-1.8.8/src/damo/damo_wss.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.7/src/damo.egg-info/PKG-INFO` & `damo-1.8.8/src/damo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.8.7
+Version: 1.8.8
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -32,26 +32,29 @@
 http://www.youtube.com/watch?v=l63eqbVBZRY
 "DAMON: a demo for the Kernel Summit 2020")
 
 
 Getting Started
 ===============
 
+[![Packaging status](https://repology.org/badge/vertical-allrepos/damo.svg)](https://repology.org/project/damo/versions)
+
 Follow below instructions and commands to monitor and visualize the access
 pattern of your workload.
 
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
+    $ # install from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.7/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.7/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.8/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.8/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +62,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.7/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.8/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -87,19 +90,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.7/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.8/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.7/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.8/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
@@ -184,16 +187,16 @@
 
 Deprecated.  Use Python3.
 
 For some old distros, DAMO initially supported Python2.  Because Python2 is
 really old now, the support has deprecated.  Please use Python3 or newer.
 
 
-DAMOS singline format
----------------------
+DAMOS single line format
+------------------------
 
 Deprecated.  Use `--damos_*` command line options or json format input.
 
 One-line scheme specification format like below was initially supported.
 Because it is not flexible for extension of features, it has deprecated now.
 You may use `--damos_*` command line options or json format instead.  You may
 use `damo translate_damos` to convert your old single line DAMOS schemes
```

### Comparing `damo-1.8.7/src/damo.egg-info/SOURCES.txt` & `damo-1.8.8/src/damo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

