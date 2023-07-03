# Comparing `tmp/zit-0.0.1a1.tar.gz` & `tmp/zit-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zit-0.0.1a1.tar", max compression
+gzip compressed data, was "zit-0.0.2a0.tar", max compression
```

## Comparing `zit-0.0.1a1.tar` & `zit-0.0.2a0.tar`

### file list

```diff
@@ -1,7 +1,25 @@
--rw-r--r--   0        0        0      420 2022-01-09 15:40:30.445293 zit-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-01-09 08:55:56.174938 zit-0.0.1a1/zit/__init__.py
--rw-r--r--   0        0        0        0 2022-01-09 09:47:29.534983 zit-0.0.1a1/zit/auth.py
--rw-r--r--   0        0        0      112 2022-01-09 15:13:01.395269 zit-0.0.1a1/zit/lambdaOpts.py
--rw-r--r--   0        0        0      687 2022-01-09 15:18:14.935274 zit-0.0.1a1/zit/main.py
--rw-r--r--   0        0        0      603 2022-01-09 15:40:55.094321 zit-0.0.1a1/setup.py
--rw-r--r--   0        0        0      472 2022-01-09 15:40:55.094479 zit-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0      986 2023-07-03 13:17:09.144798 zit-0.0.2a0/pyproject.toml
+-rw-r--r--   0        0        0       72 2022-01-10 03:44:16.795928 zit-0.0.2a0/zit/__init__.py
+-rw-r--r--   0        0        0     1544 2023-04-14 12:30:48.576605 zit-0.0.2a0/zit/auth.py
+-rw-r--r--   0        0        0      527 2023-05-01 05:42:53.369475 zit-0.0.2a0/zit/config.py
+-rw-r--r--   0        0        0     6412 2023-07-03 12:45:23.075406 zit-0.0.2a0/zit/dashboard.py
+-rw-r--r--   0        0        0       60 2023-06-15 21:58:13.307052 zit-0.0.2a0/zit/dataset/__init__.py
+-rw-r--r--   0        0        0      407 2023-05-11 08:42:13.675272 zit-0.0.2a0/zit/dataset/build.py
+-rw-r--r--   0        0        0        0 2023-06-15 21:56:33.152907 zit-0.0.2a0/zit/dataset/classification.py
+-rw-r--r--   0        0        0     2029 2023-06-15 17:30:11.785818 zit-0.0.2a0/zit/dataset/convert.py
+-rw-r--r--   0        0        0     1460 2023-06-19 00:08:05.186263 zit-0.0.2a0/zit/dataset/detection.py
+-rw-r--r--   0        0        0      427 2023-05-11 07:24:56.576494 zit-0.0.2a0/zit/dataset/factory.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:37:14.408208 zit-0.0.2a0/zit/dataset/keypoints.py
+-rw-r--r--   0        0        0    15732 2023-06-18 22:35:18.479099 zit-0.0.2a0/zit/dataset/manager.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:37:56.638196 zit-0.0.2a0/zit/dataset/multilabel_classification.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:36:54.588213 zit-0.0.2a0/zit/dataset/segmentation.py
+-rw-r--r--   0        0        0    10862 2023-05-11 08:20:08.065614 zit-0.0.2a0/zit/formula.py
+-rw-r--r--   0        0        0      617 2023-04-16 19:16:58.258259 zit-0.0.2a0/zit/main.py
+-rw-r--r--   0        0        0      670 2023-06-28 06:34:04.531830 zit-0.0.2a0/zit/routes/__init__.py
+-rw-r--r--   0        0        0      520 2023-06-18 22:26:38.078376 zit-0.0.2a0/zit/routes/dataset/annotations.py
+-rw-r--r--   0        0        0      831 2023-06-18 22:58:55.749634 zit-0.0.2a0/zit/routes/dataset/categories.py
+-rw-r--r--   0        0        0     3214 2023-06-18 21:57:11.118740 zit-0.0.2a0/zit/routes/dataset/images.py
+-rw-r--r--   0        0        0     2126 2023-06-28 09:53:59.159211 zit-0.0.2a0/zit/routes/dataset/queries.py
+-rw-r--r--   0        0        0      402 2023-06-16 09:25:23.231629 zit-0.0.2a0/zit/utils.py
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 zit-0.0.2a0/setup.py
+-rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 zit-0.0.2a0/PKG-INFO
```

