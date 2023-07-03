# Comparing `tmp/sharetop-1.4.4.tar.gz` & `tmp/sharetop-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharetop-1.4.4.tar", last modified: Thu May 25 04:25:00 2023, max compression
+gzip compressed data, was "sharetop-1.4.5.tar", last modified: Mon Jul  3 03:57:20 2023, max compression
```

## Comparing `sharetop-1.4.4.tar` & `sharetop-1.4.5.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 04:25:00.875611 sharetop-1.4.4/
--rw-rw-rw-   0        0        0     1066 2023-04-26 14:07:21.000000 sharetop-1.4.4/LICENSE
--rw-rw-rw-   0        0        0    48208 2023-05-25 04:25:00.875611 sharetop-1.4.4/PKG-INFO
--rw-rw-rw-   0        0        0    46771 2023-05-19 00:45:05.000000 sharetop-1.4.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-25 04:25:00.875611 sharetop-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-04-29 06:50:50.000000 sharetop-1.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 04:25:00.822380 sharetop-1.4.4/sharetop/
--rw-rw-rw-   0        0        0      297 2023-05-18 12:23:41.000000 sharetop-1.4.4/sharetop/__init__.py
--rw-rw-rw-   0        0        0      386 2023-05-25 04:24:40.000000 sharetop-1.4.4/sharetop/__version__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 04:25:00.839050 sharetop-1.4.4/sharetop/api/
--rw-rw-rw-   0        0        0      306 2023-05-18 12:23:41.000000 sharetop-1.4.4/sharetop/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 04:25:00.842405 sharetop-1.4.4/sharetop/application/
--rw-rw-rw-   0        0        0       33 2023-04-21 11:53:52.000000 sharetop-1.4.4/sharetop/application/__init__.py
--rw-rw-rw-   0        0        0     4146 2023-04-30 13:59:24.000000 sharetop-1.4.4/sharetop/application/base.py
-drwxrwxrwx   0        0        0        0 2023-05-25 04:25:00.842405 sharetop-1.4.4/sharetop/core/
--rw-rw-rw-   0        0        0        0 2023-04-08 05:23:09.000000 sharetop-1.4.4/sharetop/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 04:25:00.842405 sharetop-1.4.4/sharetop/core/bond/
--rw-rw-rw-   0        0        0      758 2023-04-25 21:15:03.000000 sharetop-1.4.4/sharetop/core/bond/__init__.py
--rw-rw-rw-   0        0        0     1869 2023-04-24 04:28:03.000000 sharetop-1.4.4/sharetop/core/bond/config.py
--rw-rw-rw-   0        0        0     9356 2023-04-26 00:46:59.000000 sharetop-1.4.4/sharetop/core/bond/get_bond_info.py
--rw-rw-rw-   0        0        0    19572 2023-04-26 00:53:29.000000 sharetop-1.4.4/sharetop/core/bond/get_bond_public_info.py
--rw-rw-rw-   0        0        0      598 2023-04-10 05:06:06.000000 sharetop-1.4.4/sharetop/core/cache.py
-drwxrwxrwx   0        0        0        0 2023-05-25 04:25:00.842405 sharetop-1.4.4/sharetop/core/capital_flow/
--rw-rw-rw-   0        0        0      240 2023-05-19 00:38:55.000000 sharetop-1.4.4/sharetop/core/capital_flow/__init__.py
--rw-rw-rw-   0        0        0     6319 2023-05-25 01:13:19.000000 sharetop-1.4.4/sharetop/core/capital_flow/capital_flow_monitor.py
-drwxrwxrwx   0        0        0        0 2023-05-25 04:25:00.842405 sharetop-1.4.4/sharetop/core/common/
--rw-rw-rw-   0        0        0      188 2023-04-27 15:24:55.000000 sharetop-1.4.4/sharetop/core/common/__init__.py
--rw-rw-rw-   0        0        0     3721 2023-05-25 01:16:42.000000 sharetop-1.4.4/sharetop/core/common/common_base.py
--rw-rw-rw-   0        0        0     8688 2023-05-25 01:16:42.000000 sharetop-1.4.4/sharetop/core/common/config.py
--rw-rw-rw-   0        0        0    12268 2023-05-19 23:26:57.000000 sharetop-1.4.4/sharetop/core/common/getter.py
--rw-rw-rw-   0        0        0      750 2023-04-09 05:42:43.000000 sharetop-1.4.4/sharetop/core/config.py
-drwxrwxrwx   0        0        0        0 2023-05-25 04:25:00.842405 sharetop-1.4.4/sharetop/core/country/
--rw-rw-rw-   0        0        0      101 2023-05-16 01:30:15.000000 sharetop-1.4.4/sharetop/core/country/__init__.py
--rw-rw-rw-   0        0        0      491 2023-05-09 01:30:20.000000 sharetop-1.4.4/sharetop/core/country/config.py
--rw-rw-rw-   0        0        0      494 2023-05-11 04:40:55.000000 sharetop-1.4.4/sharetop/core/country/country_base_info.py
-drwxrwxrwx   0        0        0        0 2023-05-25 04:25:00.859515 sharetop-1.4.4/sharetop/core/fund/
--rw-rw-rw-   0        0        0      931 2023-05-03 07:19:55.000000 sharetop-1.4.4/sharetop/core/fund/__init__.py
--rw-rw-rw-   0        0        0      412 2023-04-22 11:35:14.000000 sharetop-1.4.4/sharetop/core/fund/config.py
--rw-rw-rw-   0        0        0     2509 2023-04-26 00:53:29.000000 sharetop-1.4.4/sharetop/core/fund/fund_list.py
--rw-rw-rw-   0        0        0     1471 2023-04-26 00:53:29.000000 sharetop-1.4.4/sharetop/core/fund/get_fund_base_info.py
--rw-rw-rw-   0        0        0     2377 2023-04-27 15:28:32.000000 sharetop-1.4.4/sharetop/core/fund/get_fund_history_data.py
--rw-rw-rw-   0        0        0     3601 2023-04-27 01:02:03.000000 sharetop-1.4.4/sharetop/core/fund/get_fund_industry_info.py
--rw-rw-rw-   0        0        0     5387 2023-04-27 15:28:32.000000 sharetop-1.4.4/sharetop/core/fund/get_fund_invest_info.py
--rw-rw-rw-   0        0        0    12687 2023-05-03 07:31:14.000000 sharetop-1.4.4/sharetop/core/fund/get_fund_rank.py
--rw-rw-rw-   0        0        0     1466 2023-04-22 03:27:53.000000 sharetop-1.4.4/sharetop/core/fund/get_fund_real_time.py
--rw-rw-rw-   0        0        0     2401 2023-04-26 00:53:29.000000 sharetop-1.4.4/sharetop/core/fund/get_period_change_info.py
--rw-rw-rw-   0        0        0     2336 2023-04-26 00:53:29.000000 sharetop-1.4.4/sharetop/core/fund/get_types_percentage_info.py
-drwxrwxrwx   0        0        0        0 2023-05-25 04:25:00.859515 sharetop-1.4.4/sharetop/core/futures/
--rw-rw-rw-   0        0        0      272 2023-04-27 14:23:26.000000 sharetop-1.4.4/sharetop/core/futures/__init__.py
--rw-rw-rw-   0        0        0     9922 2023-04-28 01:45:42.000000 sharetop-1.4.4/sharetop/core/futures/get_futures_info.py
-drwxrwxrwx   0        0        0        0 2023-05-25 04:25:00.859515 sharetop-1.4.4/sharetop/core/oil/
--rw-rw-rw-   0        0        0      402 2023-05-16 01:17:51.000000 sharetop-1.4.4/sharetop/core/oil/__init__.py
--rw-rw-rw-   0        0        0     1685 2023-05-15 00:28:25.000000 sharetop-1.4.4/sharetop/core/oil/config.py
--rw-rw-rw-   0        0        0     2970 2023-05-16 01:17:51.000000 sharetop-1.4.4/sharetop/core/oil/oil_detail.py
-drwxrwxrwx   0        0        0        0 2023-05-25 04:25:00.859515 sharetop-1.4.4/sharetop/core/pig/
--rw-rw-rw-   0        0        0       76 2023-05-16 01:17:51.000000 sharetop-1.4.4/sharetop/core/pig/__init__.py
--rw-rw-rw-   0        0        0      163 2023-05-16 00:42:46.000000 sharetop-1.4.4/sharetop/core/pig/config.py
--rw-rw-rw-   0        0        0     1127 2023-05-16 00:59:27.000000 sharetop-1.4.4/sharetop/core/pig/pig_detail.py
-drwxrwxrwx   0        0        0        0 2023-05-25 04:25:00.859515 sharetop-1.4.4/sharetop/core/stock/
--rw-rw-rw-   0        0        0      453 2023-05-18 12:23:41.000000 sharetop-1.4.4/sharetop/core/stock/__init__.py
--rw-rw-rw-   0        0        0     4606 2023-04-28 01:45:42.000000 sharetop-1.4.4/sharetop/core/stock/bill_monitor.py
--rw-rw-rw-   0        0        0     1163 2023-04-13 13:52:05.000000 sharetop-1.4.4/sharetop/core/stock/config.py
--rw-rw-rw-   0        0        0    14368 2023-05-04 12:15:59.000000 sharetop-1.4.4/sharetop/core/stock/getter.py
--rw-rw-rw-   0        0        0    10088 2023-04-30 13:59:24.000000 sharetop-1.4.4/sharetop/core/stock/quarterly_report.py
--rw-rw-rw-   0        0        0    10010 2023-04-30 13:59:24.000000 sharetop-1.4.4/sharetop/core/stock/rank_list.py
--rw-rw-rw-   0        0        0      377 2023-05-02 14:39:20.000000 sharetop-1.4.4/sharetop/core/stock/stock_base_info.py
--rw-rw-rw-   0        0        0     6349 2023-05-04 04:01:07.000000 sharetop-1.4.4/sharetop/core/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 04:25:00.875611 sharetop-1.4.4/sharetop/crawl/
--rw-rw-rw-   0        0        0       29 2023-04-09 23:19:21.000000 sharetop-1.4.4/sharetop/crawl/__init__.py
--rw-rw-rw-   0        0        0      861 2023-05-11 04:25:42.000000 sharetop-1.4.4/sharetop/crawl/base.py
--rw-rw-rw-   0        0        0     3298 2023-05-24 14:55:28.000000 sharetop-1.4.4/sharetop/crawl/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-25 04:25:00.875611 sharetop-1.4.4/sharetop/parser/
--rw-rw-rw-   0        0        0       27 2023-04-10 00:54:05.000000 sharetop-1.4.4/sharetop/parser/__init__.py
--rw-rw-rw-   0        0        0     4239 2023-05-23 12:33:52.000000 sharetop-1.4.4/sharetop/parser/base.py
--rw-rw-rw-   0        0        0     2906 2023-05-19 00:08:10.000000 sharetop-1.4.4/sharetop/parser/config.py
-drwxrwxrwx   0        0        0        0 2023-05-25 04:25:00.875611 sharetop-1.4.4/sharetop/test/
--rw-rw-rw-   0        0        0        0 2023-04-29 10:57:35.000000 sharetop-1.4.4/sharetop/test/__init__.py
--rw-rw-rw-   0        0        0      199 2023-05-17 04:49:54.000000 sharetop-1.4.4/sharetop/test/captial.py
--rw-rw-rw-   0        0        0      261 2023-04-30 13:54:58.000000 sharetop-1.4.4/sharetop/test/test1.py
--rw-rw-rw-   0        0        0     1997 2023-05-02 03:48:40.000000 sharetop-1.4.4/sharetop/test/test2-akshare.py
--rw-rw-rw-   0        0        0     3709 2023-05-03 07:10:48.000000 sharetop-1.4.4/sharetop/test/test3.py
--rw-rw-rw-   0        0        0      219 2023-05-04 04:00:10.000000 sharetop-1.4.4/sharetop/test/test4.py
--rw-rw-rw-   0        0        0      643 2023-05-24 14:56:05.000000 sharetop-1.4.4/sharetop/test/test5.py
--rw-rw-rw-   0        0        0      443 2023-05-25 01:58:54.000000 sharetop-1.4.4/sharetop/test/test6.py
-drwxrwxrwx   0        0        0        0 2023-05-25 04:25:00.839050 sharetop-1.4.4/sharetop.egg-info/
--rw-rw-rw-   0        0        0    48208 2023-05-25 04:25:00.000000 sharetop-1.4.4/sharetop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2165 2023-05-25 04:25:00.000000 sharetop-1.4.4/sharetop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 04:25:00.000000 sharetop-1.4.4/sharetop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-25 04:25:00.000000 sharetop-1.4.4/sharetop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-25 04:25:00.000000 sharetop-1.4.4/sharetop.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.513057 sharetop-1.4.5/
+-rw-rw-rw-   0        0        0     1066 2023-04-26 14:07:21.000000 sharetop-1.4.5/LICENSE
+-rw-rw-rw-   0        0        0    51232 2023-07-03 03:57:20.512673 sharetop-1.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0    49753 2023-05-25 04:36:48.000000 sharetop-1.4.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 03:57:20.513057 sharetop-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-04-29 06:50:50.000000 sharetop-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.436267 sharetop-1.4.5/sharetop/
+-rw-rw-rw-   0        0        0      297 2023-05-18 12:23:41.000000 sharetop-1.4.5/sharetop/__init__.py
+-rw-rw-rw-   0        0        0      386 2023-07-03 03:53:57.000000 sharetop-1.4.5/sharetop/__version__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.459158 sharetop-1.4.5/sharetop/api/
+-rw-rw-rw-   0        0        0      306 2023-07-02 13:11:41.000000 sharetop-1.4.5/sharetop/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.461390 sharetop-1.4.5/sharetop/application/
+-rw-rw-rw-   0        0        0       33 2023-04-21 11:53:52.000000 sharetop-1.4.5/sharetop/application/__init__.py
+-rw-rw-rw-   0        0        0     4459 2023-07-03 03:12:50.000000 sharetop-1.4.5/sharetop/application/base.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.465391 sharetop-1.4.5/sharetop/core/
+-rw-rw-rw-   0        0        0        0 2023-04-08 05:23:09.000000 sharetop-1.4.5/sharetop/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.470390 sharetop-1.4.5/sharetop/core/bond/
+-rw-rw-rw-   0        0        0      758 2023-04-25 21:15:03.000000 sharetop-1.4.5/sharetop/core/bond/__init__.py
+-rw-rw-rw-   0        0        0     1869 2023-04-24 04:28:03.000000 sharetop-1.4.5/sharetop/core/bond/config.py
+-rw-rw-rw-   0        0        0     9356 2023-04-26 00:46:59.000000 sharetop-1.4.5/sharetop/core/bond/get_bond_info.py
+-rw-rw-rw-   0        0        0    19572 2023-04-26 00:53:29.000000 sharetop-1.4.5/sharetop/core/bond/get_bond_public_info.py
+-rw-rw-rw-   0        0        0      598 2023-04-10 05:06:06.000000 sharetop-1.4.5/sharetop/core/cache.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.472634 sharetop-1.4.5/sharetop/core/capital_flow/
+-rw-rw-rw-   0        0        0      322 2023-05-25 04:33:54.000000 sharetop-1.4.5/sharetop/core/capital_flow/__init__.py
+-rw-rw-rw-   0        0        0     6235 2023-05-25 04:36:48.000000 sharetop-1.4.5/sharetop/core/capital_flow/capital_flow_monitor.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.476972 sharetop-1.4.5/sharetop/core/common/
+-rw-rw-rw-   0        0        0      188 2023-04-27 15:24:55.000000 sharetop-1.4.5/sharetop/core/common/__init__.py
+-rw-rw-rw-   0        0        0     3721 2023-05-25 01:16:42.000000 sharetop-1.4.5/sharetop/core/common/common_base.py
+-rw-rw-rw-   0        0        0     8688 2023-05-25 01:16:42.000000 sharetop-1.4.5/sharetop/core/common/config.py
+-rw-rw-rw-   0        0        0    12268 2023-07-03 03:49:09.000000 sharetop-1.4.5/sharetop/core/common/getter.py
+-rw-rw-rw-   0        0        0      750 2023-04-09 05:42:43.000000 sharetop-1.4.5/sharetop/core/config.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.479539 sharetop-1.4.5/sharetop/core/country/
+-rw-rw-rw-   0        0        0      101 2023-05-16 01:30:15.000000 sharetop-1.4.5/sharetop/core/country/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-05-09 01:30:20.000000 sharetop-1.4.5/sharetop/core/country/config.py
+-rw-rw-rw-   0        0        0      506 2023-07-03 01:12:16.000000 sharetop-1.4.5/sharetop/core/country/country_base_info.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.490394 sharetop-1.4.5/sharetop/core/fund/
+-rw-rw-rw-   0        0        0      931 2023-05-03 07:19:55.000000 sharetop-1.4.5/sharetop/core/fund/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-04-22 11:35:14.000000 sharetop-1.4.5/sharetop/core/fund/config.py
+-rw-rw-rw-   0        0        0     2509 2023-04-26 00:53:29.000000 sharetop-1.4.5/sharetop/core/fund/fund_list.py
+-rw-rw-rw-   0        0        0     1471 2023-04-26 00:53:29.000000 sharetop-1.4.5/sharetop/core/fund/get_fund_base_info.py
+-rw-rw-rw-   0        0        0     2377 2023-04-27 15:28:32.000000 sharetop-1.4.5/sharetop/core/fund/get_fund_history_data.py
+-rw-rw-rw-   0        0        0     3601 2023-04-27 01:02:03.000000 sharetop-1.4.5/sharetop/core/fund/get_fund_industry_info.py
+-rw-rw-rw-   0        0        0     5387 2023-04-27 15:28:32.000000 sharetop-1.4.5/sharetop/core/fund/get_fund_invest_info.py
+-rw-rw-rw-   0        0        0    12687 2023-05-03 07:31:14.000000 sharetop-1.4.5/sharetop/core/fund/get_fund_rank.py
+-rw-rw-rw-   0        0        0     1466 2023-04-22 03:27:53.000000 sharetop-1.4.5/sharetop/core/fund/get_fund_real_time.py
+-rw-rw-rw-   0        0        0     2401 2023-04-26 00:53:29.000000 sharetop-1.4.5/sharetop/core/fund/get_period_change_info.py
+-rw-rw-rw-   0        0        0     2336 2023-04-26 00:53:29.000000 sharetop-1.4.5/sharetop/core/fund/get_types_percentage_info.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.491346 sharetop-1.4.5/sharetop/core/futures/
+-rw-rw-rw-   0        0        0      272 2023-04-27 14:23:26.000000 sharetop-1.4.5/sharetop/core/futures/__init__.py
+-rw-rw-rw-   0        0        0     9922 2023-04-28 01:45:42.000000 sharetop-1.4.5/sharetop/core/futures/get_futures_info.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.494346 sharetop-1.4.5/sharetop/core/oil/
+-rw-rw-rw-   0        0        0      402 2023-05-16 01:17:51.000000 sharetop-1.4.5/sharetop/core/oil/__init__.py
+-rw-rw-rw-   0        0        0     1685 2023-05-15 00:28:25.000000 sharetop-1.4.5/sharetop/core/oil/config.py
+-rw-rw-rw-   0        0        0     2970 2023-05-16 01:17:51.000000 sharetop-1.4.5/sharetop/core/oil/oil_detail.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.496728 sharetop-1.4.5/sharetop/core/pig/
+-rw-rw-rw-   0        0        0       76 2023-05-16 01:17:51.000000 sharetop-1.4.5/sharetop/core/pig/__init__.py
+-rw-rw-rw-   0        0        0      163 2023-05-16 00:42:46.000000 sharetop-1.4.5/sharetop/core/pig/config.py
+-rw-rw-rw-   0        0        0     1127 2023-05-16 00:59:27.000000 sharetop-1.4.5/sharetop/core/pig/pig_detail.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.503658 sharetop-1.4.5/sharetop/core/stock/
+-rw-rw-rw-   0        0        0      453 2023-05-18 12:23:41.000000 sharetop-1.4.5/sharetop/core/stock/__init__.py
+-rw-rw-rw-   0        0        0     4606 2023-04-28 01:45:42.000000 sharetop-1.4.5/sharetop/core/stock/bill_monitor.py
+-rw-rw-rw-   0        0        0     1163 2023-04-13 13:52:05.000000 sharetop-1.4.5/sharetop/core/stock/config.py
+-rw-rw-rw-   0        0        0    14368 2023-05-04 12:15:59.000000 sharetop-1.4.5/sharetop/core/stock/getter.py
+-rw-rw-rw-   0        0        0    10088 2023-04-30 13:59:24.000000 sharetop-1.4.5/sharetop/core/stock/quarterly_report.py
+-rw-rw-rw-   0        0        0    10010 2023-04-30 13:59:24.000000 sharetop-1.4.5/sharetop/core/stock/rank_list.py
+-rw-rw-rw-   0        0        0      377 2023-05-02 14:39:20.000000 sharetop-1.4.5/sharetop/core/stock/stock_base_info.py
+-rw-rw-rw-   0        0        0     6349 2023-05-04 04:01:07.000000 sharetop-1.4.5/sharetop/core/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.505673 sharetop-1.4.5/sharetop/crawl/
+-rw-rw-rw-   0        0        0       29 2023-04-09 23:19:21.000000 sharetop-1.4.5/sharetop/crawl/__init__.py
+-rw-rw-rw-   0        0        0      861 2023-05-11 04:25:42.000000 sharetop-1.4.5/sharetop/crawl/base.py
+-rw-rw-rw-   0        0        0     3298 2023-05-24 14:55:28.000000 sharetop-1.4.5/sharetop/crawl/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.506672 sharetop-1.4.5/sharetop/parser/
+-rw-rw-rw-   0        0        0       27 2023-04-10 00:54:05.000000 sharetop-1.4.5/sharetop/parser/__init__.py
+-rw-rw-rw-   0        0        0     4239 2023-05-23 12:33:52.000000 sharetop-1.4.5/sharetop/parser/base.py
+-rw-rw-rw-   0        0        0     2906 2023-05-19 00:08:10.000000 sharetop-1.4.5/sharetop/parser/config.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.511672 sharetop-1.4.5/sharetop/test/
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:57:35.000000 sharetop-1.4.5/sharetop/test/__init__.py
+-rw-rw-rw-   0        0        0      199 2023-05-17 04:49:54.000000 sharetop-1.4.5/sharetop/test/captial.py
+-rw-rw-rw-   0        0        0      336 2023-07-03 03:45:37.000000 sharetop-1.4.5/sharetop/test/test1.py
+-rw-rw-rw-   0        0        0     1997 2023-05-02 03:48:40.000000 sharetop-1.4.5/sharetop/test/test2-akshare.py
+-rw-rw-rw-   0        0        0     3709 2023-05-03 07:10:48.000000 sharetop-1.4.5/sharetop/test/test3.py
+-rw-rw-rw-   0        0        0      219 2023-05-04 04:00:10.000000 sharetop-1.4.5/sharetop/test/test4.py
+-rw-rw-rw-   0        0        0      643 2023-05-24 14:56:05.000000 sharetop-1.4.5/sharetop/test/test5.py
+-rw-rw-rw-   0        0        0      860 2023-06-04 02:11:02.000000 sharetop-1.4.5/sharetop/test/test6.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.457651 sharetop-1.4.5/sharetop.egg-info/
+-rw-rw-rw-   0        0        0    51232 2023-07-03 03:57:20.000000 sharetop-1.4.5/sharetop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2165 2023-07-03 03:57:20.000000 sharetop-1.4.5/sharetop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 03:57:20.000000 sharetop-1.4.5/sharetop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-07-03 03:57:20.000000 sharetop-1.4.5/sharetop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-03 03:57:20.000000 sharetop-1.4.5/sharetop.egg-info/top_level.txt
```

### Comparing `sharetop-1.4.4/LICENSE` & `sharetop-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/PKG-INFO` & `sharetop-1.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharetop
-Version: 1.4.4
+Version: 1.4.5
 Summary: Provide data related to the economic market
 Home-page: https://github.com/nrliangxy/sharetop
 Author: nrliangxy
 Author-email: nrliangxy@foxmail.com
 License: MIT
 Project-URL: Source, https://github.com/nrliangxy/sharetop
 Keywords: data,finance,quant,stock,fund,futures,share
@@ -340,14 +340,56 @@
 
 [1 rows x 28 columns], '300033':        今日主力净流入        超大单流入        超大单流出  ...    5日大单净流入      5日中单净流入      5日小单净流入
 0  388495062.0  530087824.0  205526730.0  ... -2282457.0 -190202898.0 -120267946.0
 
 [1 rows x 28 columns]}
 ```
 
+- 股市行业，概念，区域资金流向
+
+```python
+>>> import sharetop as sp
+>>> sp.capital_flow.get_sector_real_time_capital_flow('area', '10')
+      行业  10日涨跌幅(%)     10日主力净流入额  ...  10日小单净流入净占比(%)    股票名称    股票代码
+0   贵州板块      -2.41 -2.083888e+07  ...            1.74    贵州茅台  600519
+1   宁夏板块      -2.13 -1.763856e+08  ...            3.35    宝丰能源  600989
+2   海南板块      -3.34 -4.854156e+08  ...            1.92    钧达股份  002865
+3   青海板块      -2.23 -6.745363e+08  ...            3.51    藏格矿业  000408
+4   广西板块      -2.68 -9.937139e+08  ...            3.79    皇氏集团  002329
+5   吉林板块      -2.59 -1.155900e+09  ...            2.97    金冠股份  300510
+6   甘肃板块      -3.10 -1.230404e+09  ...            4.33    金刚光伏  300093
+7    内蒙古      -2.51 -1.247756e+09  ...            2.39    兴业矿业  000426
+8   西藏板块      -1.40 -1.297749e+09  ...            2.96    西藏矿业  000762
+9    黑龙江      -1.74 -1.643403e+09  ...            3.24    哈药股份  600664
+10  云南板块      -3.67 -1.963538e+09  ...            3.30    昆药集团  600422
+11  山西板块      -2.01 -2.684929e+09  ...            3.81    大秦铁路  601006
+12  江西板块       0.94 -2.855563e+09  ...            3.48  *ST 正邦  002157
+13  辽宁板块       0.02 -3.258344e+09  ...            2.21    抚顺特钢  600399
+14  重庆板块      -3.16 -3.914550e+09  ...            4.43    太极集团  600129
+15  天津板块      -1.16 -4.458393e+09  ...            3.25   TCL中环  002129
+16  陕西板块      -1.29 -4.627671e+09  ...            3.14    源杰科技  688498
+17  河北板块      -2.23 -4.794085e+09  ...            3.56    晶澳科技  002459
+18  河南板块       0.06 -4.851007e+09  ...            3.74    众智科技  301361
+19  湖北板块       0.21 -5.617115e+09  ...            2.77    航天南湖  688552
+20  湖南板块      -1.49 -5.735864e+09  ...            3.52     国科微  300672
+21  四川板块       0.32 -6.178380e+09  ...            2.70     新易盛  300502
+22  新疆板块      -4.10 -6.270602e+09  ...            5.56    西部建设  002302
+23  安徽板块      -0.04 -6.859943e+09  ...            2.82    晶合集成  688249
+24  山东板块       0.08 -8.224411e+09  ...            2.83    浪潮信息  000977
+25  福建板块      -1.20 -9.065944e+09  ...            2.67    恺英网络  002517
+26  江苏板块       2.09 -1.550369e+10  ...            2.27    天孚通信  300394
+27  浙江板块       1.08 -2.070258e+10  ...            2.78    C安杰思  688581
+28  上海板块      -1.21 -2.474813e+10  ...            3.44    中微公司  688012
+29  广东板块       0.39 -3.796577e+10  ...            2.77   C飞测-U  688361
+30  北京板块      -3.92 -6.096971e+10  ...            4.05     C航天  688562
+
+[31 rows x 14 columns]
+```
+
+
 ### Fund
 
 - 获取基金历史净值信息
 
 ```python
 >>> import sharetop as sp
 >>> sp.fund.get_fund_history('010434')
```

### Comparing `sharetop-1.4.4/README.md` & `sharetop-1.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -320,14 +320,56 @@
 
 [1 rows x 28 columns], '300033':        今日主力净流入        超大单流入        超大单流出  ...    5日大单净流入      5日中单净流入      5日小单净流入
 0  388495062.0  530087824.0  205526730.0  ... -2282457.0 -190202898.0 -120267946.0
 
 [1 rows x 28 columns]}
 ```
 
+- 股市行业，概念，区域资金流向
+
+```python
+>>> import sharetop as sp
+>>> sp.capital_flow.get_sector_real_time_capital_flow('area', '10')
+      行业  10日涨跌幅(%)     10日主力净流入额  ...  10日小单净流入净占比(%)    股票名称    股票代码
+0   贵州板块      -2.41 -2.083888e+07  ...            1.74    贵州茅台  600519
+1   宁夏板块      -2.13 -1.763856e+08  ...            3.35    宝丰能源  600989
+2   海南板块      -3.34 -4.854156e+08  ...            1.92    钧达股份  002865
+3   青海板块      -2.23 -6.745363e+08  ...            3.51    藏格矿业  000408
+4   广西板块      -2.68 -9.937139e+08  ...            3.79    皇氏集团  002329
+5   吉林板块      -2.59 -1.155900e+09  ...            2.97    金冠股份  300510
+6   甘肃板块      -3.10 -1.230404e+09  ...            4.33    金刚光伏  300093
+7    内蒙古      -2.51 -1.247756e+09  ...            2.39    兴业矿业  000426
+8   西藏板块      -1.40 -1.297749e+09  ...            2.96    西藏矿业  000762
+9    黑龙江      -1.74 -1.643403e+09  ...            3.24    哈药股份  600664
+10  云南板块      -3.67 -1.963538e+09  ...            3.30    昆药集团  600422
+11  山西板块      -2.01 -2.684929e+09  ...            3.81    大秦铁路  601006
+12  江西板块       0.94 -2.855563e+09  ...            3.48  *ST 正邦  002157
+13  辽宁板块       0.02 -3.258344e+09  ...            2.21    抚顺特钢  600399
+14  重庆板块      -3.16 -3.914550e+09  ...            4.43    太极集团  600129
+15  天津板块      -1.16 -4.458393e+09  ...            3.25   TCL中环  002129
+16  陕西板块      -1.29 -4.627671e+09  ...            3.14    源杰科技  688498
+17  河北板块      -2.23 -4.794085e+09  ...            3.56    晶澳科技  002459
+18  河南板块       0.06 -4.851007e+09  ...            3.74    众智科技  301361
+19  湖北板块       0.21 -5.617115e+09  ...            2.77    航天南湖  688552
+20  湖南板块      -1.49 -5.735864e+09  ...            3.52     国科微  300672
+21  四川板块       0.32 -6.178380e+09  ...            2.70     新易盛  300502
+22  新疆板块      -4.10 -6.270602e+09  ...            5.56    西部建设  002302
+23  安徽板块      -0.04 -6.859943e+09  ...            2.82    晶合集成  688249
+24  山东板块       0.08 -8.224411e+09  ...            2.83    浪潮信息  000977
+25  福建板块      -1.20 -9.065944e+09  ...            2.67    恺英网络  002517
+26  江苏板块       2.09 -1.550369e+10  ...            2.27    天孚通信  300394
+27  浙江板块       1.08 -2.070258e+10  ...            2.78    C安杰思  688581
+28  上海板块      -1.21 -2.474813e+10  ...            3.44    中微公司  688012
+29  广东板块       0.39 -3.796577e+10  ...            2.77   C飞测-U  688361
+30  北京板块      -3.92 -6.096971e+10  ...            4.05     C航天  688562
+
+[31 rows x 14 columns]
+```
+
+
 ### Fund
 
 - 获取基金历史净值信息
 
 ```python
 >>> import sharetop as sp
 >>> sp.fund.get_fund_history('010434')
```

### Comparing `sharetop-1.4.4/setup.py` & `sharetop-1.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/application/base.py` & `sharetop-1.4.5/sharetop/application/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,22 +31,31 @@
     def deal_fields(self, data, fields_list):
         f59 = data['f59']
         for _ in fields_list:
             item = data[_] / math.pow(10, f59)
             data[_] = item
         return data
 
+    def deal_price_fields(self, data, fields_list):
+        f152 = data['f152']
+        for _ in fields_list:
+            item = data[_] / math.pow(10, f152)
+            data[_] = item
+        return data
+
     def deal_real_time_data(self, columns, fields_k_v):
         data = self.json_data['data']
         if not data:
             columns.insert(0, '代码')
             columns.insert(0, '名称')
             return pd.DataFrame(columns=columns)
-        deal_fields_list = ["f43", "f169", "f44", "f45", "f46", "f60", "f71", "f164", "f167", "f170", "f171"]
+        deal_real_time_price = ["f170"]
+        deal_fields_list = ["f43", "f169", "f44", "f45", "f46", "f60", "f71", "f164", "f167", "f171"]
         data = self.deal_fields(data, deal_fields_list)
+        data = self.deal_price_fields(data, deal_real_time_price)
         r = {v: data.get(k) for k, v in fields_k_v.items()}
         return pd.DataFrame([r])
 
     def deal_market_realtime(self, columns):
         df = pd.DataFrame(self.json_data['data']['diff'])
         df = df.rename(columns=columns)
         df: pd.DataFrame = df[columns.values()]
```

### Comparing `sharetop-1.4.4/sharetop/core/bond/__init__.py` & `sharetop-1.4.5/sharetop/core/bond/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/bond/config.py` & `sharetop-1.4.5/sharetop/core/bond/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/bond/get_bond_info.py` & `sharetop-1.4.5/sharetop/core/bond/get_bond_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/bond/get_bond_public_info.py` & `sharetop-1.4.5/sharetop/core/bond/get_bond_public_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/cache.py` & `sharetop-1.4.5/sharetop/core/cache.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/capital_flow/capital_flow_monitor.py` & `sharetop-1.4.5/sharetop/core/capital_flow/capital_flow_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-from ..utils import get_quote_id, to_numeric, requests_obj
+from ..utils import to_numeric
 from ..common.getter import get_history_bill as get_history_bill_for_stock
 from ..common.getter import get_real_time_bill_data_one
-from ...crawl.settings import *
 from ..common.common_base import CommonFunc
 from typing import Dict, List, Union
 import pandas as pd
-from enum import Enum
 
 common_func_obj = CommonFunc()
 
 
 @to_numeric
 def get_history_bill(stock_code: str) -> pd.DataFrame:
     """
```

### Comparing `sharetop-1.4.4/sharetop/core/common/common_base.py` & `sharetop-1.4.5/sharetop/core/common/common_base.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/common/config.py` & `sharetop-1.4.5/sharetop/core/common/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/common/getter.py` & `sharetop-1.4.5/sharetop/core/common/getter.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/config.py` & `sharetop-1.4.5/sharetop/core/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/fund/__init__.py` & `sharetop-1.4.5/sharetop/core/fund/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/fund/fund_list.py` & `sharetop-1.4.5/sharetop/core/fund/fund_list.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/fund/get_fund_base_info.py` & `sharetop-1.4.5/sharetop/core/fund/get_fund_base_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/fund/get_fund_history_data.py` & `sharetop-1.4.5/sharetop/core/fund/get_fund_history_data.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/fund/get_fund_industry_info.py` & `sharetop-1.4.5/sharetop/core/fund/get_fund_industry_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/fund/get_fund_invest_info.py` & `sharetop-1.4.5/sharetop/core/fund/get_fund_invest_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/fund/get_fund_rank.py` & `sharetop-1.4.5/sharetop/core/fund/get_fund_rank.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/fund/get_fund_real_time.py` & `sharetop-1.4.5/sharetop/core/fund/get_fund_real_time.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/fund/get_period_change_info.py` & `sharetop-1.4.5/sharetop/core/fund/get_period_change_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/fund/get_types_percentage_info.py` & `sharetop-1.4.5/sharetop/core/fund/get_types_percentage_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/futures/get_futures_info.py` & `sharetop-1.4.5/sharetop/core/futures/get_futures_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/oil/config.py` & `sharetop-1.4.5/sharetop/core/oil/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/oil/oil_detail.py` & `sharetop-1.4.5/sharetop/core/oil/oil_detail.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/pig/pig_detail.py` & `sharetop-1.4.5/sharetop/core/pig/pig_detail.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/stock/bill_monitor.py` & `sharetop-1.4.5/sharetop/core/stock/bill_monitor.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/stock/config.py` & `sharetop-1.4.5/sharetop/core/stock/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/stock/getter.py` & `sharetop-1.4.5/sharetop/core/stock/getter.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/stock/quarterly_report.py` & `sharetop-1.4.5/sharetop/core/stock/quarterly_report.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/stock/rank_list.py` & `sharetop-1.4.5/sharetop/core/stock/rank_list.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/core/utils.py` & `sharetop-1.4.5/sharetop/core/utils.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/crawl/base.py` & `sharetop-1.4.5/sharetop/crawl/base.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/crawl/settings.py` & `sharetop-1.4.5/sharetop/crawl/settings.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/parser/base.py` & `sharetop-1.4.5/sharetop/parser/base.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/parser/config.py` & `sharetop-1.4.5/sharetop/parser/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/test/test2-akshare.py` & `sharetop-1.4.5/sharetop/test/test2-akshare.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/test/test3.py` & `sharetop-1.4.5/sharetop/test/test3.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop/test/test5.py` & `sharetop-1.4.5/sharetop/test/test5.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.4/sharetop.egg-info/PKG-INFO` & `sharetop-1.4.5/sharetop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharetop
-Version: 1.4.4
+Version: 1.4.5
 Summary: Provide data related to the economic market
 Home-page: https://github.com/nrliangxy/sharetop
 Author: nrliangxy
 Author-email: nrliangxy@foxmail.com
 License: MIT
 Project-URL: Source, https://github.com/nrliangxy/sharetop
 Keywords: data,finance,quant,stock,fund,futures,share
@@ -340,14 +340,56 @@
 
 [1 rows x 28 columns], '300033':        今日主力净流入        超大单流入        超大单流出  ...    5日大单净流入      5日中单净流入      5日小单净流入
 0  388495062.0  530087824.0  205526730.0  ... -2282457.0 -190202898.0 -120267946.0
 
 [1 rows x 28 columns]}
 ```
 
+- 股市行业，概念，区域资金流向
+
+```python
+>>> import sharetop as sp
+>>> sp.capital_flow.get_sector_real_time_capital_flow('area', '10')
+      行业  10日涨跌幅(%)     10日主力净流入额  ...  10日小单净流入净占比(%)    股票名称    股票代码
+0   贵州板块      -2.41 -2.083888e+07  ...            1.74    贵州茅台  600519
+1   宁夏板块      -2.13 -1.763856e+08  ...            3.35    宝丰能源  600989
+2   海南板块      -3.34 -4.854156e+08  ...            1.92    钧达股份  002865
+3   青海板块      -2.23 -6.745363e+08  ...            3.51    藏格矿业  000408
+4   广西板块      -2.68 -9.937139e+08  ...            3.79    皇氏集团  002329
+5   吉林板块      -2.59 -1.155900e+09  ...            2.97    金冠股份  300510
+6   甘肃板块      -3.10 -1.230404e+09  ...            4.33    金刚光伏  300093
+7    内蒙古      -2.51 -1.247756e+09  ...            2.39    兴业矿业  000426
+8   西藏板块      -1.40 -1.297749e+09  ...            2.96    西藏矿业  000762
+9    黑龙江      -1.74 -1.643403e+09  ...            3.24    哈药股份  600664
+10  云南板块      -3.67 -1.963538e+09  ...            3.30    昆药集团  600422
+11  山西板块      -2.01 -2.684929e+09  ...            3.81    大秦铁路  601006
+12  江西板块       0.94 -2.855563e+09  ...            3.48  *ST 正邦  002157
+13  辽宁板块       0.02 -3.258344e+09  ...            2.21    抚顺特钢  600399
+14  重庆板块      -3.16 -3.914550e+09  ...            4.43    太极集团  600129
+15  天津板块      -1.16 -4.458393e+09  ...            3.25   TCL中环  002129
+16  陕西板块      -1.29 -4.627671e+09  ...            3.14    源杰科技  688498
+17  河北板块      -2.23 -4.794085e+09  ...            3.56    晶澳科技  002459
+18  河南板块       0.06 -4.851007e+09  ...            3.74    众智科技  301361
+19  湖北板块       0.21 -5.617115e+09  ...            2.77    航天南湖  688552
+20  湖南板块      -1.49 -5.735864e+09  ...            3.52     国科微  300672
+21  四川板块       0.32 -6.178380e+09  ...            2.70     新易盛  300502
+22  新疆板块      -4.10 -6.270602e+09  ...            5.56    西部建设  002302
+23  安徽板块      -0.04 -6.859943e+09  ...            2.82    晶合集成  688249
+24  山东板块       0.08 -8.224411e+09  ...            2.83    浪潮信息  000977
+25  福建板块      -1.20 -9.065944e+09  ...            2.67    恺英网络  002517
+26  江苏板块       2.09 -1.550369e+10  ...            2.27    天孚通信  300394
+27  浙江板块       1.08 -2.070258e+10  ...            2.78    C安杰思  688581
+28  上海板块      -1.21 -2.474813e+10  ...            3.44    中微公司  688012
+29  广东板块       0.39 -3.796577e+10  ...            2.77   C飞测-U  688361
+30  北京板块      -3.92 -6.096971e+10  ...            4.05     C航天  688562
+
+[31 rows x 14 columns]
+```
+
+
 ### Fund
 
 - 获取基金历史净值信息
 
 ```python
 >>> import sharetop as sp
 >>> sp.fund.get_fund_history('010434')
```

### Comparing `sharetop-1.4.4/sharetop.egg-info/SOURCES.txt` & `sharetop-1.4.5/sharetop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

