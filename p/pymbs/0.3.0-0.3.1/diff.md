# Comparing `tmp/pymbs-0.3.0.tar.gz` & `tmp/pymbs-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymbs-0.3.0.tar", last modified: Wed Sep 18 20:26:50 2019, max compression
+gzip compressed data, was "pymbs-0.3.1.tar", last modified: Mon Jul  3 00:15:52 2023, max compression
```

## Comparing `pymbs-0.3.0.tar` & `pymbs-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,256 @@
-drwxr-xr-x   0 btf        (501) staff       (20)        0 2019-09-18 20:26:50.000000 pymbs-0.3.0/
--rw-r--r--   0 btf        (501) staff       (20)     2320 2019-09-18 20:23:11.000000 pymbs-0.3.0/CHANGES.rst
--rw-r--r--   0 btf        (501) staff       (20)    34523 2019-07-30 17:36:42.000000 pymbs-0.3.0/LICENSE
--rw-r--r--   0 btf        (501) staff       (20)       40 2019-08-26 09:54:55.000000 pymbs-0.3.0/MANIFEST.in
--rw-r--r--   0 btf        (501) staff       (20)     2683 2019-09-18 20:26:50.000000 pymbs-0.3.0/PKG-INFO
--rw-r--r--   0 btf        (501) staff       (20)     1129 2019-08-28 15:43:23.000000 pymbs-0.3.0/README.rst
-drwxr-xr-x   0 btf        (501) staff       (20)        0 2019-09-18 20:26:50.000000 pymbs-0.3.0/pymbs/
--rw-r--r--   0 btf        (501) staff       (20)      856 2019-08-29 02:10:25.000000 pymbs-0.3.0/pymbs/__init__.py
--rw-r--r--   0 btf        (501) staff       (20)     2731 2019-09-18 20:22:11.000000 pymbs-0.3.0/pymbs/__version__.py
--rw-r--r--   0 btf        (501) staff       (20)    12710 2019-09-18 17:10:45.000000 pymbs-0.3.0/pymbs/api.py
-drwxr-xr-x   0 btf        (501) staff       (20)        0 2019-09-18 20:26:50.000000 pymbs-0.3.0/pymbs/config/
--rw-r--r--   0 btf        (501) staff       (20)      681 2019-09-15 17:16:15.000000 pymbs-0.3.0/pymbs/config/pymbs_logging.json
--rw-r--r--   0 btf        (501) staff       (20)    14251 2019-09-18 15:41:00.000000 pymbs-0.3.0/pymbs/config.py
--rw-r--r--   0 btf        (501) staff       (20)    19859 2019-09-18 15:41:00.000000 pymbs-0.3.0/pymbs/core.py
--rw-r--r--   0 btf        (501) staff       (20)     2504 2019-09-15 17:16:15.000000 pymbs-0.3.0/pymbs/enums.py
--rw-r--r--   0 btf        (501) staff       (20)     7318 2019-09-18 15:41:00.000000 pymbs-0.3.0/pymbs/exceptions.py
--rw-r--r--   0 btf        (501) staff       (20)     3594 2019-08-27 21:42:15.000000 pymbs-0.3.0/pymbs/log.py
--rw-r--r--   0 btf        (501) staff       (20)     4275 2019-09-15 17:16:15.000000 pymbs-0.3.0/pymbs/payment_rules.py
--rw-r--r--   0 btf        (501) staff       (20)    12500 2019-09-18 15:41:00.000000 pymbs-0.3.0/pymbs/tranche.py
--rw-r--r--   0 btf        (501) staff       (20)     9247 2019-09-18 15:41:00.000000 pymbs-0.3.0/pymbs/utils.py
-drwxr-xr-x   0 btf        (501) staff       (20)        0 2019-09-18 20:26:50.000000 pymbs-0.3.0/pymbs.egg-info/
--rw-r--r--   0 btf        (501) staff       (20)     2683 2019-09-18 20:26:50.000000 pymbs-0.3.0/pymbs.egg-info/PKG-INFO
--rw-r--r--   0 btf        (501) staff       (20)      440 2019-09-18 20:26:50.000000 pymbs-0.3.0/pymbs.egg-info/SOURCES.txt
--rw-r--r--   0 btf        (501) staff       (20)        1 2019-09-18 20:26:50.000000 pymbs-0.3.0/pymbs.egg-info/dependency_links.txt
--rw-r--r--   0 btf        (501) staff       (20)        1 2019-09-18 20:26:50.000000 pymbs-0.3.0/pymbs.egg-info/not-zip-safe
--rw-r--r--   0 btf        (501) staff       (20)       73 2019-09-18 20:26:50.000000 pymbs-0.3.0/pymbs.egg-info/requires.txt
--rw-r--r--   0 btf        (501) staff       (20)        6 2019-09-18 20:26:50.000000 pymbs-0.3.0/pymbs.egg-info/top_level.txt
--rw-r--r--   0 btf        (501) staff       (20)       38 2019-09-18 20:26:50.000000 pymbs-0.3.0/setup.cfg
--rw-r--r--   0 btf        (501) staff       (20)     2606 2019-09-15 17:16:15.000000 pymbs-0.3.0/setup.py
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.338280 pymbs-0.3.1/
+-rw-r--r--   0 btf        (501) staff       (20)      693 2023-07-02 22:35:28.000000 pymbs-0.3.1/.gitignore
+-rw-r--r--   0 btf        (501) staff       (20)      884 2019-09-15 17:16:15.000000 pymbs-0.3.1/.gitlab-ci.yml
+-rw-r--r--   0 btf        (501) staff       (20)    71091 2019-07-31 16:54:17.000000 pymbs-0.3.1/Basic_Working_Example.ipynb
+-rw-r--r--   0 btf        (501) staff       (20)     2610 2023-07-03 00:13:32.000000 pymbs-0.3.1/CHANGES.rst
+-rw-r--r--   0 btf        (501) staff       (20)    34523 2019-07-30 17:36:42.000000 pymbs-0.3.1/LICENSE
+-rw-r--r--   0 btf        (501) staff       (20)       40 2019-08-26 09:54:55.000000 pymbs-0.3.1/MANIFEST.in
+-rw-r--r--   0 btf        (501) staff       (20)     2215 2023-07-03 00:15:52.337904 pymbs-0.3.1/PKG-INFO
+-rw-r--r--   0 btf        (501) staff       (20)     1085 2023-07-03 00:05:45.000000 pymbs-0.3.1/README.rst
+-rw-r--r--   0 btf        (501) staff       (20)      728 2019-08-28 15:43:23.000000 pymbs-0.3.1/TODO.rst
+-rw-r--r--   0 btf        (501) staff       (20)    34523 2019-08-27 21:42:14.000000 pymbs-0.3.1/agpl-3.0.txt
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.166825 pymbs-0.3.1/docs/
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.180609 pymbs-0.3.1/docs/build/
+-rw-r--r--   0 btf        (501) staff       (20)      230 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/.buildinfo
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.197661 pymbs-0.3.1/docs/build/.doctrees/
+-rw-r--r--   0 btf        (501) staff       (20)    20924 2023-07-03 00:02:41.000000 pymbs-0.3.1/docs/build/.doctrees/caveats.doctree
+-rw-r--r--   0 btf        (501) staff       (20)    20351 2023-07-03 00:13:47.000000 pymbs-0.3.1/docs/build/.doctrees/changes.doctree
+-rw-r--r--   0 btf        (501) staff       (20)    10100 2019-08-27 23:30:18.000000 pymbs-0.3.1/docs/build/.doctrees/configuration.doctree
+-rw-r--r--   0 btf        (501) staff       (20)   143964 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/.doctrees/environment.pickle
+-rw-r--r--   0 btf        (501) staff       (20)     6322 2023-07-03 00:13:47.000000 pymbs-0.3.1/docs/build/.doctrees/getting_started.doctree
+-rw-r--r--   0 btf        (501) staff       (20)     4414 2023-07-03 00:13:47.000000 pymbs-0.3.1/docs/build/.doctrees/index.doctree
+-rw-r--r--   0 btf        (501) staff       (20)    18788 2019-08-20 22:42:01.000000 pymbs-0.3.1/docs/build/.doctrees/itunesapp.api.doctree
+-rw-r--r--   0 btf        (501) staff       (20)     6118 2019-08-20 22:42:01.000000 pymbs-0.3.1/docs/build/.doctrees/itunesapp.doctree
+-rw-r--r--   0 btf        (501) staff       (20)     5242 2023-07-03 00:13:47.000000 pymbs-0.3.1/docs/build/.doctrees/log_file.doctree
+-rw-r--r--   0 btf        (501) staff       (20)     2837 2023-07-03 00:13:47.000000 pymbs-0.3.1/docs/build/.doctrees/modules.doctree
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.198624 pymbs-0.3.1/docs/build/.doctrees/other/
+-rw-r--r--   0 btf        (501) staff       (20)     3026 2019-08-20 22:42:01.000000 pymbs-0.3.1/docs/build/.doctrees/other/changes.doctree
+-rw-r--r--   0 btf        (501) staff       (20)     2654 2019-08-20 22:42:01.000000 pymbs-0.3.1/docs/build/.doctrees/other/index.doctree
+-rw-r--r--   0 btf        (501) staff       (20)    35886 2019-08-20 22:42:01.000000 pymbs-0.3.1/docs/build/.doctrees/pietunes.api.doctree
+-rw-r--r--   0 btf        (501) staff       (20)     5155 2019-08-20 22:42:01.000000 pymbs-0.3.1/docs/build/.doctrees/pietunes.core.doctree
+-rw-r--r--   0 btf        (501) staff       (20)     5935 2019-08-20 22:42:01.000000 pymbs-0.3.1/docs/build/.doctrees/pietunes.doctree
+-rw-r--r--   0 btf        (501) staff       (20)    12807 2019-08-20 22:42:01.000000 pymbs-0.3.1/docs/build/.doctrees/pietunes.enums.doctree
+-rw-r--r--   0 btf        (501) staff       (20)     5308 2019-08-20 22:42:01.000000 pymbs-0.3.1/docs/build/.doctrees/pietunes.script_support.doctree
+-rw-r--r--   0 btf        (501) staff       (20)     9748 2023-07-03 00:13:47.000000 pymbs-0.3.1/docs/build/.doctrees/project.doctree
+-rw-r--r--   0 btf        (501) staff       (20)    62315 2023-07-03 00:13:47.000000 pymbs-0.3.1/docs/build/.doctrees/pymbs.api.doctree
+-rw-r--r--   0 btf        (501) staff       (20)    37435 2023-07-03 00:13:47.000000 pymbs-0.3.1/docs/build/.doctrees/pymbs.config.doctree
+-rw-r--r--   0 btf        (501) staff       (20)     5234 2023-07-03 00:13:47.000000 pymbs-0.3.1/docs/build/.doctrees/pymbs.core.doctree
+-rw-r--r--   0 btf        (501) staff       (20)     6016 2023-07-03 00:13:47.000000 pymbs-0.3.1/docs/build/.doctrees/pymbs.doctree
+-rw-r--r--   0 btf        (501) staff       (20)    50973 2023-07-03 00:13:47.000000 pymbs-0.3.1/docs/build/.doctrees/pymbs.enums.doctree
+-rw-r--r--   0 btf        (501) staff       (20)    36150 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/.doctrees/pymbs.exceptions.doctree
+-rw-r--r--   0 btf        (501) staff       (20)    12523 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/.doctrees/pymbs.log.doctree
+-rw-r--r--   0 btf        (501) staff       (20)    16472 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/.doctrees/pymbs.payment_rules.doctree
+-rw-r--r--   0 btf        (501) staff       (20)    60750 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/.doctrees/pymbs.tranche.doctree
+-rw-r--r--   0 btf        (501) staff       (20)    22589 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/.doctrees/pymbs.utils.doctree
+-rw-r--r--   0 btf        (501) staff       (20)    28593 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/.doctrees/run_the_model.doctree
+-rw-r--r--   0 btf        (501) staff       (20)     5534 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/.doctrees/setup.doctree
+-rw-r--r--   0 btf        (501) staff       (20)    31371 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/.doctrees/setup_anaconda.doctree
+-rw-r--r--   0 btf        (501) staff       (20)    27651 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/.doctrees/setup_modeling.doctree
+-rw-r--r--   0 btf        (501) staff       (20)     6263 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/.doctrees/todo.doctree
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.220028 pymbs-0.3.1/docs/build/_images/
+-rw-r--r--   0 btf        (501) staff       (20)    39426 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/build/_images/add_channel.jpg
+-rw-r--r--   0 btf        (501) staff       (20)   215663 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/build/_images/anaconda_environments.jpg
+-rw-r--r--   0 btf        (501) staff       (20)   190349 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/build/_images/anaconda_navigator.jpg
+-rw-r--r--   0 btf        (501) staff       (20)    30051 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/build/_images/create_new_env.jpg
+-rw-r--r--   0 btf        (501) staff       (20)   241199 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/build/_images/fhl2618_repo.jpg
+-rw-r--r--   0 btf        (501) staff       (20)   359608 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/build/_images/freakin_windows.jpg
+-rw-r--r--   0 btf        (501) staff       (20)    49307 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/build/_images/install_packages.jpg
+-rw-r--r--   0 btf        (501) staff       (20)   117048 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/build/_images/install_pymbs.jpg
+-rw-r--r--   0 btf        (501) staff       (20)   144154 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/build/_images/jupyter_lab_initial.jpg
+-rw-r--r--   0 btf        (501) staff       (20)   157790 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/build/_images/model_file.jpg
+-rw-r--r--   0 btf        (501) staff       (20)   241707 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/build/_images/model_in_jupyter_lab.jpg
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.222902 pymbs-0.3.1/docs/build/_modules/
+-rw-r--r--   0 btf        (501) staff       (20)     3569 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/_modules/index.html
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.231629 pymbs-0.3.1/docs/build/_modules/pymbs/
+-rw-r--r--   0 btf        (501) staff       (20)    45358 2023-07-03 00:02:43.000000 pymbs-0.3.1/docs/build/_modules/pymbs/api.html
+-rw-r--r--   0 btf        (501) staff       (20)    43725 2023-07-02 22:23:41.000000 pymbs-0.3.1/docs/build/_modules/pymbs/config.html
+-rw-r--r--   0 btf        (501) staff       (20)     9586 2023-07-02 22:23:41.000000 pymbs-0.3.1/docs/build/_modules/pymbs/enums.html
+-rw-r--r--   0 btf        (501) staff       (20)    28170 2023-07-02 22:23:41.000000 pymbs-0.3.1/docs/build/_modules/pymbs/exceptions.html
+-rw-r--r--   0 btf        (501) staff       (20)    15195 2023-07-02 22:23:41.000000 pymbs-0.3.1/docs/build/_modules/pymbs/log.html
+-rw-r--r--   0 btf        (501) staff       (20)    23060 2023-07-03 00:02:43.000000 pymbs-0.3.1/docs/build/_modules/pymbs/payment_rules.html
+-rw-r--r--   0 btf        (501) staff       (20)    55828 2023-07-02 22:23:41.000000 pymbs-0.3.1/docs/build/_modules/pymbs/tranche.html
+-rw-r--r--   0 btf        (501) staff       (20)    40975 2023-07-02 22:23:41.000000 pymbs-0.3.1/docs/build/_modules/pymbs/utils.html
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.244252 pymbs-0.3.1/docs/build/_sources/
+-rw-r--r--   0 btf        (501) staff       (20)     4145 2023-07-02 23:40:49.000000 pymbs-0.3.1/docs/build/_sources/caveats.rst.txt
+-rw-r--r--   0 btf        (501) staff       (20)       31 2019-07-30 17:36:42.000000 pymbs-0.3.1/docs/build/_sources/changes.rst.txt
+-rw-r--r--   0 btf        (501) staff       (20)     1026 2023-07-02 23:10:45.000000 pymbs-0.3.1/docs/build/_sources/getting_started.rst.txt
+-rw-r--r--   0 btf        (501) staff       (20)      250 2019-08-28 15:40:02.000000 pymbs-0.3.1/docs/build/_sources/index.rst.txt
+-rw-r--r--   0 btf        (501) staff       (20)      851 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/build/_sources/log_file.rst.txt
+-rw-r--r--   0 btf        (501) staff       (20)      192 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/build/_sources/modules.rst.txt
+-rw-r--r--   0 btf        (501) staff       (20)       30 2019-07-30 17:36:42.000000 pymbs-0.3.1/docs/build/_sources/project.rst.txt
+-rw-r--r--   0 btf        (501) staff       (20)      125 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/build/_sources/pymbs.api.rst.txt
+-rw-r--r--   0 btf        (501) staff       (20)      141 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/build/_sources/pymbs.config.rst.txt
+-rw-r--r--   0 btf        (501) staff       (20)      118 2019-07-30 20:30:31.000000 pymbs-0.3.1/docs/build/_sources/pymbs.core.rst.txt
+-rw-r--r--   0 btf        (501) staff       (20)      121 2019-08-20 09:06:14.000000 pymbs-0.3.1/docs/build/_sources/pymbs.enums.rst.txt
+-rw-r--r--   0 btf        (501) staff       (20)      136 2019-08-20 09:06:14.000000 pymbs-0.3.1/docs/build/_sources/pymbs.exceptions.rst.txt
+-rw-r--r--   0 btf        (501) staff       (20)      115 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/build/_sources/pymbs.log.rst.txt
+-rw-r--r--   0 btf        (501) staff       (20)      147 2019-08-20 09:06:14.000000 pymbs-0.3.1/docs/build/_sources/pymbs.payment_rules.rst.txt
+-rw-r--r--   0 btf        (501) staff       (20)      187 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/build/_sources/pymbs.rst.txt
+-rw-r--r--   0 btf        (501) staff       (20)      127 2019-08-20 09:06:14.000000 pymbs-0.3.1/docs/build/_sources/pymbs.tranche.rst.txt
+-rw-r--r--   0 btf        (501) staff       (20)      121 2019-08-20 09:06:14.000000 pymbs-0.3.1/docs/build/_sources/pymbs.utils.rst.txt
+-rw-r--r--   0 btf        (501) staff       (20)     6496 2019-08-28 15:43:23.000000 pymbs-0.3.1/docs/build/_sources/run_the_model.rst.txt
+-rw-r--r--   0 btf        (501) staff       (20)      938 2019-08-28 15:43:23.000000 pymbs-0.3.1/docs/build/_sources/setup.rst.txt
+-rw-r--r--   0 btf        (501) staff       (20)     7077 2023-07-02 23:53:04.000000 pymbs-0.3.1/docs/build/_sources/setup_anaconda.rst.txt
+-rw-r--r--   0 btf        (501) staff       (20)     5951 2019-08-28 15:43:23.000000 pymbs-0.3.1/docs/build/_sources/setup_modeling.rst.txt
+-rw-r--r--   0 btf        (501) staff       (20)       27 2019-08-20 22:42:01.000000 pymbs-0.3.1/docs/build/_sources/todo.rst.txt
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.253263 pymbs-0.3.1/docs/build/_static/
+-rw-r--r--   0 btf        (501) staff       (20)    11193 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/_static/alabaster.css
+-rw-r--r--   0 btf        (501) staff       (20)    15228 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/_static/basic.css
+-rw-r--r--   0 btf        (501) staff       (20)       50 2019-08-20 22:42:01.000000 pymbs-0.3.1/docs/build/_static/custom.css
+-rw-r--r--   0 btf        (501) staff       (20)     8171 2023-03-09 19:22:36.000000 pymbs-0.3.1/docs/build/_static/doctools.js
+-rw-r--r--   0 btf        (501) staff       (20)      421 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/_static/documentation_options.js
+-rw-r--r--   0 btf        (501) staff       (20)      286 2020-04-12 20:45:11.000000 pymbs-0.3.1/docs/build/_static/file.png
+-rw-r--r--   0 btf        (501) staff       (20)   280364 2020-04-12 20:45:11.000000 pymbs-0.3.1/docs/build/_static/jquery-3.4.1.js
+-rw-r--r--   0 btf        (501) staff       (20)    89501 2023-03-09 19:22:36.000000 pymbs-0.3.1/docs/build/_static/jquery.js
+-rw-r--r--   0 btf        (501) staff       (20)     4758 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/_static/language_data.js
+-rw-r--r--   0 btf        (501) staff       (20)       90 2020-04-12 20:45:11.000000 pymbs-0.3.1/docs/build/_static/minus.png
+-rw-r--r--   0 btf        (501) staff       (20)       90 2020-04-12 20:45:11.000000 pymbs-0.3.1/docs/build/_static/plus.png
+-rw-r--r--   0 btf        (501) staff       (20)     5327 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/_static/pygments.css
+-rw-r--r--   0 btf        (501) staff       (20)    17088 2023-03-09 19:22:36.000000 pymbs-0.3.1/docs/build/_static/searchtools.js
+-rw-r--r--   0 btf        (501) staff       (20)    35168 2020-04-12 20:45:11.000000 pymbs-0.3.1/docs/build/_static/underscore-1.3.1.js
+-rw-r--r--   0 btf        (501) staff       (20)    19530 2023-03-09 19:22:36.000000 pymbs-0.3.1/docs/build/_static/underscore.js
+-rw-r--r--   0 btf        (501) staff       (20)     9442 2023-07-03 00:02:43.000000 pymbs-0.3.1/docs/build/caveats.html
+-rw-r--r--   0 btf        (501) staff       (20)     9201 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/changes.html
+-rw-r--r--   0 btf        (501) staff       (20)    23266 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/genindex.html
+-rw-r--r--   0 btf        (501) staff       (20)     5997 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/getting_started.html
+-rw-r--r--   0 btf        (501) staff       (20)     6499 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/index.html
+-rw-r--r--   0 btf        (501) staff       (20)     4222 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/log_file.html
+-rw-r--r--   0 btf        (501) staff       (20)     4967 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/modules.html
+-rw-r--r--   0 btf        (501) staff       (20)     1740 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/objects.inv
+-rw-r--r--   0 btf        (501) staff       (20)     6782 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/project.html
+-rw-r--r--   0 btf        (501) staff       (20)     5444 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/py-modindex.html
+-rw-r--r--   0 btf        (501) staff       (20)    23624 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/pymbs.api.html
+-rw-r--r--   0 btf        (501) staff       (20)    17159 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/pymbs.config.html
+-rw-r--r--   0 btf        (501) staff       (20)     5151 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/pymbs.core.html
+-rw-r--r--   0 btf        (501) staff       (20)    22318 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/pymbs.enums.html
+-rw-r--r--   0 btf        (501) staff       (20)    15712 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/pymbs.exceptions.html
+-rw-r--r--   0 btf        (501) staff       (20)     6329 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/pymbs.html
+-rw-r--r--   0 btf        (501) staff       (20)     7834 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/pymbs.log.html
+-rw-r--r--   0 btf        (501) staff       (20)    10719 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/pymbs.payment_rules.html
+-rw-r--r--   0 btf        (501) staff       (20)    27117 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/pymbs.tranche.html
+-rw-r--r--   0 btf        (501) staff       (20)    13363 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/pymbs.utils.html
+-rw-r--r--   0 btf        (501) staff       (20)    13412 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/run_the_model.html
+-rw-r--r--   0 btf        (501) staff       (20)     3331 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/search.html
+-rw-r--r--   0 btf        (501) staff       (20)    30461 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/searchindex.js
+-rw-r--r--   0 btf        (501) staff       (20)     5410 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/setup.html
+-rw-r--r--   0 btf        (501) staff       (20)    15476 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/setup_anaconda.html
+-rw-r--r--   0 btf        (501) staff       (20)    12386 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/setup_modeling.html
+-rw-r--r--   0 btf        (501) staff       (20)     5054 2023-07-03 00:13:48.000000 pymbs-0.3.1/docs/build/todo.html
+-rw-r--r--   0 btf        (501) staff       (20)     1492 2020-04-12 22:45:37.000000 pymbs-0.3.1/docs/docs.py
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.262012 pymbs-0.3.1/docs/source/
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.287118 pymbs-0.3.1/docs/source/_images/
+-rw-r--r--   0 btf        (501) staff       (20)    39426 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/source/_images/add_channel.jpg
+-rw-r--r--   0 btf        (501) staff       (20)   215663 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/source/_images/anaconda_environments.jpg
+-rw-r--r--   0 btf        (501) staff       (20)   190349 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/source/_images/anaconda_navigator.jpg
+-rw-r--r--   0 btf        (501) staff       (20)    30051 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/source/_images/create_new_env.jpg
+-rw-r--r--   0 btf        (501) staff       (20)   241199 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/source/_images/fhl2618_repo.jpg
+-rw-r--r--   0 btf        (501) staff       (20)   359608 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/source/_images/freakin_windows.jpg
+-rw-r--r--   0 btf        (501) staff       (20)    49307 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/source/_images/install_packages.jpg
+-rw-r--r--   0 btf        (501) staff       (20)   117048 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/source/_images/install_pymbs.jpg
+-rw-r--r--   0 btf        (501) staff       (20)   144154 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/source/_images/jupyter_lab_initial.jpg
+-rw-r--r--   0 btf        (501) staff       (20)   157790 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/source/_images/model_file.jpg
+-rw-r--r--   0 btf        (501) staff       (20)   241707 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/source/_images/model_in_jupyter_lab.jpg
+-rw-r--r--   0 btf        (501) staff       (20)   206153 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/source/_images/not_installed.jpg
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.289631 pymbs-0.3.1/docs/source/_static/
+-rw-r--r--   0 btf        (501) staff       (20)       50 2019-08-20 22:42:01.000000 pymbs-0.3.1/docs/source/_static/custom.css
+-rw-r--r--   0 btf        (501) staff       (20)     4145 2023-07-02 23:40:49.000000 pymbs-0.3.1/docs/source/caveats.rst
+-rw-r--r--   0 btf        (501) staff       (20)       31 2019-07-30 17:36:42.000000 pymbs-0.3.1/docs/source/changes.rst
+-rw-r--r--   0 btf        (501) staff       (20)     6948 2023-07-02 22:38:20.000000 pymbs-0.3.1/docs/source/conf.py
+-rw-r--r--   0 btf        (501) staff       (20)     1026 2023-07-02 23:10:45.000000 pymbs-0.3.1/docs/source/getting_started.rst
+-rw-r--r--   0 btf        (501) staff       (20)      250 2019-08-28 15:40:02.000000 pymbs-0.3.1/docs/source/index.rst
+-rw-r--r--   0 btf        (501) staff       (20)      851 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/source/log_file.rst
+-rw-r--r--   0 btf        (501) staff       (20)      192 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/source/modules.rst
+-rw-r--r--   0 btf        (501) staff       (20)       30 2019-07-30 17:36:42.000000 pymbs-0.3.1/docs/source/project.rst
+-rw-r--r--   0 btf        (501) staff       (20)      125 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/source/pymbs.api.rst
+-rw-r--r--   0 btf        (501) staff       (20)      141 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/source/pymbs.config.rst
+-rw-r--r--   0 btf        (501) staff       (20)      118 2019-07-30 20:30:31.000000 pymbs-0.3.1/docs/source/pymbs.core.rst
+-rw-r--r--   0 btf        (501) staff       (20)      121 2019-08-20 09:06:14.000000 pymbs-0.3.1/docs/source/pymbs.enums.rst
+-rw-r--r--   0 btf        (501) staff       (20)      136 2019-08-20 09:06:14.000000 pymbs-0.3.1/docs/source/pymbs.exceptions.rst
+-rw-r--r--   0 btf        (501) staff       (20)      115 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/source/pymbs.log.rst
+-rw-r--r--   0 btf        (501) staff       (20)      147 2019-08-20 09:06:14.000000 pymbs-0.3.1/docs/source/pymbs.payment_rules.rst
+-rw-r--r--   0 btf        (501) staff       (20)      187 2019-08-27 21:42:15.000000 pymbs-0.3.1/docs/source/pymbs.rst
+-rw-r--r--   0 btf        (501) staff       (20)      127 2019-08-20 09:06:14.000000 pymbs-0.3.1/docs/source/pymbs.tranche.rst
+-rw-r--r--   0 btf        (501) staff       (20)      121 2019-08-20 09:06:14.000000 pymbs-0.3.1/docs/source/pymbs.utils.rst
+-rw-r--r--   0 btf        (501) staff       (20)     6496 2019-08-28 15:43:23.000000 pymbs-0.3.1/docs/source/run_the_model.rst
+-rw-r--r--   0 btf        (501) staff       (20)      938 2019-08-28 15:43:23.000000 pymbs-0.3.1/docs/source/setup.rst
+-rw-r--r--   0 btf        (501) staff       (20)     7077 2023-07-02 23:53:04.000000 pymbs-0.3.1/docs/source/setup_anaconda.rst
+-rw-r--r--   0 btf        (501) staff       (20)     5951 2019-08-28 15:43:23.000000 pymbs-0.3.1/docs/source/setup_modeling.rst
+-rw-r--r--   0 btf        (501) staff       (20)       27 2019-08-20 22:42:01.000000 pymbs-0.3.1/docs/source/todo.rst
+-rw-r--r--   0 btf        (501) staff       (20)     1218 2023-07-02 23:03:06.000000 pymbs-0.3.1/meta.yaml
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.290038 pymbs-0.3.1/public/
+-rw-r--r--   0 btf        (501) staff       (20)        0 2019-08-20 22:54:24.000000 pymbs-0.3.1/public/.gitkeep
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.294112 pymbs-0.3.1/pymbs/
+-rw-r--r--   0 btf        (501) staff       (20)      856 2019-08-29 02:10:25.000000 pymbs-0.3.1/pymbs/__init__.py
+-rw-r--r--   0 btf        (501) staff       (20)     2732 2023-07-02 23:06:58.000000 pymbs-0.3.1/pymbs/__version__.py
+-rw-r--r--   0 btf        (501) staff       (20)    12718 2023-07-02 22:33:13.000000 pymbs-0.3.1/pymbs/api.py
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.297073 pymbs-0.3.1/pymbs/config/
+-rw-r--r--   0 btf        (501) staff       (20)      681 2020-07-01 00:12:25.000000 pymbs-0.3.1/pymbs/config/pymbs_logging.json
+-rw-r--r--   0 btf        (501) staff       (20)    14251 2019-09-18 15:41:00.000000 pymbs-0.3.1/pymbs/config.py
+-rw-r--r--   0 btf        (501) staff       (20)    21646 2023-07-02 22:33:13.000000 pymbs-0.3.1/pymbs/core.py
+-rw-r--r--   0 btf        (501) staff       (20)     2504 2019-09-15 17:16:15.000000 pymbs-0.3.1/pymbs/enums.py
+-rw-r--r--   0 btf        (501) staff       (20)     7318 2019-09-18 15:41:00.000000 pymbs-0.3.1/pymbs/exceptions.py
+-rw-r--r--   0 btf        (501) staff       (20)     3594 2020-07-01 00:18:10.000000 pymbs-0.3.1/pymbs/log.py
+-rw-r--r--   0 btf        (501) staff       (20)     4335 2023-07-02 22:33:13.000000 pymbs-0.3.1/pymbs/payment_rules.py
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.300293 pymbs-0.3.1/pymbs/templates/
+-rw-r--r--   0 btf        (501) staff       (20)      595 2019-09-15 17:16:15.000000 pymbs-0.3.1/pymbs/templates/no_config.j2
+-rw-r--r--   0 btf        (501) staff       (20)      535 2019-09-15 17:16:15.000000 pymbs-0.3.1/pymbs/templates/no_config_data.j2
+-rw-r--r--   0 btf        (501) staff       (20)      272 2019-09-15 17:16:15.000000 pymbs-0.3.1/pymbs/templates/no_data.j2
+-rw-r--r--   0 btf        (501) staff       (20)      258 2019-09-15 17:16:15.000000 pymbs-0.3.1/pymbs/templates/no_file.j2
+-rw-r--r--   0 btf        (501) staff       (20)     1260 2019-09-15 17:16:15.000000 pymbs-0.3.1/pymbs/templates/rounding_error.j2
+-rw-r--r--   0 btf        (501) staff       (20)     1300 2019-09-15 17:16:15.000000 pymbs-0.3.1/pymbs/templates/rounding_error_wals.j2
+-rw-r--r--   0 btf        (501) staff       (20)    12500 2019-09-18 15:41:00.000000 pymbs-0.3.1/pymbs/tranche.py
+-rw-r--r--   0 btf        (501) staff       (20)     9247 2019-09-18 15:41:00.000000 pymbs-0.3.1/pymbs/utils.py
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.296717 pymbs-0.3.1/pymbs.egg-info/
+-rw-r--r--   0 btf        (501) staff       (20)     2215 2023-07-03 00:15:51.000000 pymbs-0.3.1/pymbs.egg-info/PKG-INFO
+-rw-r--r--   0 btf        (501) staff       (20)     7290 2023-07-03 00:15:52.000000 pymbs-0.3.1/pymbs.egg-info/SOURCES.txt
+-rw-r--r--   0 btf        (501) staff       (20)        1 2023-07-03 00:15:51.000000 pymbs-0.3.1/pymbs.egg-info/dependency_links.txt
+-rw-r--r--   0 btf        (501) staff       (20)        1 2023-07-03 00:15:51.000000 pymbs-0.3.1/pymbs.egg-info/not-zip-safe
+-rw-r--r--   0 btf        (501) staff       (20)       93 2023-07-03 00:15:51.000000 pymbs-0.3.1/pymbs.egg-info/requires.txt
+-rw-r--r--   0 btf        (501) staff       (20)        6 2023-07-03 00:15:51.000000 pymbs-0.3.1/pymbs.egg-info/top_level.txt
+-rw-r--r--   0 btf        (501) staff       (20)      166 2023-07-02 22:33:13.000000 pymbs-0.3.1/requirements-dev.txt
+-rw-r--r--   0 btf        (501) staff       (20)       38 2023-07-03 00:15:52.338365 pymbs-0.3.1/setup.cfg
+-rw-r--r--   0 btf        (501) staff       (20)     2631 2023-07-02 23:05:54.000000 pymbs-0.3.1/setup.py
+-rw-r--r--   0 btf        (501) staff       (20)     1573 2019-08-29 02:56:47.000000 pymbs-0.3.1/tasks.py
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.301470 pymbs-0.3.1/tests/
+-rw-r--r--   0 btf        (501) staff       (20)        0 2019-08-29 02:57:23.000000 pymbs-0.3.1/tests/__init__.py
+-rw-r--r--   0 btf        (501) staff       (20)     2478 2019-09-15 17:16:15.000000 pymbs-0.3.1/tests/conftest.py
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.155142 pymbs-0.3.1/tests/data/
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.302004 pymbs-0.3.1/tests/data/config/
+-rw-r--r--   0 btf        (501) staff       (20)       45 2019-09-15 17:16:15.000000 pymbs-0.3.1/tests/data/config/config.yaml
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.154979 pymbs-0.3.1/tests/data/input/
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.302426 pymbs-0.3.1/tests/data/input/empty_project/
+-rw-r--r--   0 btf        (501) staff       (20)        0 2019-09-15 17:16:15.000000 pymbs-0.3.1/tests/data/input/empty_project/.gitkeep
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.309659 pymbs-0.3.1/tests/data/input/fhl2618/
+-rw-r--r--   0 btf        (501) staff       (20)   175884 2019-09-15 17:16:15.000000 pymbs-0.3.1/tests/data/input/fhl2618/2618model.ipynb
+-rw-r--r--   0 btf        (501) staff       (20)    39521 2019-09-15 17:16:15.000000 pymbs-0.3.1/tests/data/input/fhl2618/fhl2618.cdi
+-rw-r--r--   0 btf        (501) staff       (20)      478 2019-09-15 17:16:15.000000 pymbs-0.3.1/tests/data/input/fhl2618/fhl2618_model.json
+-rw-r--r--   0 btf        (501) staff       (20)      379 2019-09-15 17:16:15.000000 pymbs-0.3.1/tests/data/input/fhl2618/fhl2618_pps.json
+-rw-r--r--   0 btf        (501) staff       (20)    16905 2019-09-15 17:16:15.000000 pymbs-0.3.1/tests/data/input/fhl2618/fhl2618_sc.json
+-rw-r--r--   0 btf        (501) staff       (20)     1429 2019-09-15 17:16:15.000000 pymbs-0.3.1/tests/data/input/fhl2618/fhl2618_tree.py
+-rw-r--r--   0 btf        (501) staff       (20)    43993 2019-09-18 15:41:00.000000 pymbs-0.3.1/tests/data/input/fhl2618/fhl2618_ts.json
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.332912 pymbs-0.3.1/tests/data/reference/
+-rw-r--r--   0 btf        (501) staff       (20)     1103 2019-09-18 15:41:00.000000 pymbs-0.3.1/tests/data/reference/ac.pickle
+-rw-r--r--   0 btf        (501) staff       (20)   533172 2019-09-15 17:16:15.000000 pymbs-0.3.1/tests/data/reference/cf_group_3_api.pickle
+-rw-r--r--   0 btf        (501) staff       (20)   533165 2019-09-15 17:16:15.000000 pymbs-0.3.1/tests/data/reference/cf_group_3_core.pickle
+-rw-r--r--   0 btf        (501) staff       (20)  1728831 2019-09-15 17:16:15.000000 pymbs-0.3.1/tests/data/reference/cf_group_all_api.pickle
+-rw-r--r--   0 btf        (501) staff       (20)    48406 2019-09-18 15:41:00.000000 pymbs-0.3.1/tests/data/reference/model.pickle
+-rw-r--r--   0 btf        (501) staff       (20)     6775 2019-09-18 15:41:00.000000 pymbs-0.3.1/tests/data/reference/tranches_group_1.pickle
+-rw-r--r--   0 btf        (501) staff       (20)     2129 2019-09-18 15:41:00.000000 pymbs-0.3.1/tests/data/reference/tranches_group_2.pickle
+-rw-r--r--   0 btf        (501) staff       (20)     1759 2019-09-18 15:41:00.000000 pymbs-0.3.1/tests/data/reference/tranches_group_3.pickle
+-rw-r--r--   0 btf        (501) staff       (20)     2192 2019-09-18 15:41:00.000000 pymbs-0.3.1/tests/data/reference/tranches_group_4.pickle
+-rw-r--r--   0 btf        (501) staff       (20)     8897 2019-09-18 15:41:00.000000 pymbs-0.3.1/tests/data/reference/tranches_group_all.pickle
+-rw-r--r--   0 btf        (501) staff       (20)     2019 2019-09-15 17:16:15.000000 pymbs-0.3.1/tests/data/reference/wals_10dec_group_all_api.pickle
+-rw-r--r--   0 btf        (501) staff       (20)     1659 2019-09-15 17:16:15.000000 pymbs-0.3.1/tests/data/reference/wals_1dec_group_all_api.pickle
+-rw-r--r--   0 btf        (501) staff       (20)      902 2019-09-15 17:16:15.000000 pymbs-0.3.1/tests/data/reference/wals_5dec_group_3_api.pickle
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.333958 pymbs-0.3.1/tests/func/
+-rw-r--r--   0 btf        (501) staff       (20)      818 2019-08-29 02:10:25.000000 pymbs-0.3.1/tests/func/__init__.py
+-rw-r--r--   0 btf        (501) staff       (20)     2772 2019-09-15 17:16:15.000000 pymbs-0.3.1/tests/func/test_core.py
+-rw-r--r--   0 btf        (501) staff       (20)     1184 2019-08-29 02:57:09.000000 pymbs-0.3.1/tests/qa.py
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.334914 pymbs-0.3.1/tests/sub/
+-rw-r--r--   0 btf        (501) staff       (20)      820 2019-08-29 02:10:25.000000 pymbs-0.3.1/tests/sub/__init__.py
+-rw-r--r--   0 btf        (501) staff       (20)    10873 2019-09-18 15:41:00.000000 pymbs-0.3.1/tests/sub/test_api.py
+drwxr-xr-x   0 btf        (501) staff       (20)        0 2023-07-03 00:15:52.337168 pymbs-0.3.1/tests/unit/
+-rw-r--r--   0 btf        (501) staff       (20)      812 2019-08-29 02:10:25.000000 pymbs-0.3.1/tests/unit/__init__.py
+-rw-r--r--   0 btf        (501) staff       (20)     6053 2019-09-18 15:41:00.000000 pymbs-0.3.1/tests/unit/test_core.py
+-rw-r--r--   0 btf        (501) staff       (20)     5373 2019-09-15 17:16:15.000000 pymbs-0.3.1/tests/unit/test_utils.py
+-rw-r--r--   0 btf        (501) staff       (20)     1574 2019-09-15 17:16:15.000000 pymbs-0.3.1/tests/unit/test_version.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pymbs-0.3.0/CHANGES.rst` & `pymbs-0.3.1/CHANGES.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,29 @@
+
 ==========
 Change Log
 ==========
 
 
+0.3.1
+-----
+
+Changes:
+~~~~~~~~
+
+- Update dependencies to recent versions
+- Update code base to handle Pandas 2.0
+- Update URLs in Documentation
+- Add stub for payment to a schedule in payment rules
+
+Fixed:
+~~~~~~
+- Fixed bug in setup.py that resulted in omission of Jinja template files
+
+
 0.3.0
 -----
 
 Changes:
 ~~~~~~~~
 
 - Version 0.3.0 introduces a new Terms Sheet format that is **NOT**
```

### Comparing `pymbs-0.3.0/LICENSE` & `pymbs-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymbs-0.3.0/PKG-INFO` & `pymbs-0.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,75 @@
 Metadata-Version: 2.1
 Name: pymbs
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library for use in modeling Mortgage-Backed Securities.
 Home-page: https://pypi.org/project/pymbs/
 Author: Brian Farrell
 Author-email: brian.farrell@me.com
 License: AGPLv3
-Description: 
-        ============
-        Introduction
-        ============
-        
-        PyMBS is a Python library for use in modeling Mortgage-Backed Securities.
-        
-            * This is a modern Python library that requires ``Python>=3.6``
-        
-        
-        Objectives
-        ----------
-        #. Create a modern, stable Python library with a clearly-defined API  
-        #. Provide as close to 100% Test Coverage as possible [#f1]_
-        #. Provide clear documentation with full coverage of the API and example code.
-        
-        
-        
-        Installing
-        ----------
-        
-        Install using `conda`:
-        
-        .. code-block:: bash
-        
-           conda install -c btf pymbs
-        
-        
-        Install using `pip`:
-        
-        .. code-block:: bash
-        
-           pip install pymbs
-        
-        
-        Links
-        -----
-        
-        * Documentation: https://brianfarrell.gitlab.io/pymbs/
-        * License: https://www.gnu.org/licenses/agpl.html
-        * Anaconda Cloud: https://anaconda.org/btf/pymbs/
-        * PyPi Releases: https://pypi.org/project/pymbs/
-        * Code: https://gitlab.trove.fm/btf/pymbs
-        * Issue tracker:
-        * Test status:
-        * Test coverage:
-        
-        .. rubric:: Footnotes
-        
-        .. [#f1] | This project started-out as a Proof of Concept (POC).
-                 | At that point, no automated testing was involved.
-                 | Going forward, all new development and bug fixes will be test-driven.
-        
 Keywords: financial modeling analysis mortgage securities
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.6.0
+Requires-Python: >=3.10.0
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+
+============
+Introduction
+============
+
+PyMBS is a Python library for use in modeling Mortgage-Backed Securities.
+
+    * This is a modern Python library that requires ``Python>=3.10``
+
+
+Objectives
+----------
+#. Create a modern, stable Python library with a clearly-defined API  
+#. Provide as close to 100% Test Coverage as possible [#f1]_
+#. Provide clear documentation with full coverage of the API and example code.
+
+
+
+Installing
+----------
+
+Install using `conda`:
+
+.. code-block:: bash
+
+   conda install -c btf pymbs
+
+
+Install using `pip`:
+
+.. code-block:: bash
+
+   pip install pymbs
+
+
+Links
+-----
+
+* Documentation: https://brianfarrell.gitlab.io/pymbs/
+* License: https://www.gnu.org/licenses/agpl.html
+* Anaconda Cloud: https://anaconda.org/btf/pymbs/
+* PyPi Releases: https://pypi.org/project/pymbs/
+* Code: https://gitlab.com/brianfarrell/pymbs
+
+.. rubric:: Footnotes
+
+.. [#f1] | This project started-out as a Proof of Concept (POC).
+         | At that point, no automated testing was involved.
+         | Going forward, all new development and bug fixes will be test-driven.
```

### Comparing `pymbs-0.3.0/README.rst` & `pymbs-0.3.1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 ============
 Introduction
 ============
 
 PyMBS is a Python library for use in modeling Mortgage-Backed Securities.
 
-    * This is a modern Python library that requires ``Python>=3.6``
+    * This is a modern Python library that requires ``Python>=3.10``
 
 
 Objectives
 ----------
 #. Create a modern, stable Python library with a clearly-defined API  
 #. Provide as close to 100% Test Coverage as possible [#f1]_
 #. Provide clear documentation with full coverage of the API and example code.
@@ -36,17 +36,14 @@
 Links
 -----
 
 * Documentation: https://brianfarrell.gitlab.io/pymbs/
 * License: https://www.gnu.org/licenses/agpl.html
 * Anaconda Cloud: https://anaconda.org/btf/pymbs/
 * PyPi Releases: https://pypi.org/project/pymbs/
-* Code: https://gitlab.trove.fm/btf/pymbs
-* Issue tracker:
-* Test status:
-* Test coverage:
+* Code: https://gitlab.com/brianfarrell/pymbs
 
 .. rubric:: Footnotes
 
 .. [#f1] | This project started-out as a Proof of Concept (POC).
          | At that point, no automated testing was involved.
          | Going forward, all new development and bug fixes will be test-driven.
```

### Comparing `pymbs-0.3.0/pymbs/__init__.py` & `pymbs-0.3.1/pymbs/__init__.py`

 * *Files identical despite different names*

### Comparing `pymbs-0.3.0/pymbs/__version__.py` & `pymbs-0.3.1/pymbs/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,13 +78,13 @@
         f'{s1}' + f'.'.join([tag for tag in version.pre_tags]) + \
         f'{s2}{version.post_tag}'
 
     return v
 
 
 # To increment the version, increment it in the Version tuple _version_t_
-_version_t_ = Version(0, 3, 0, version_pre_tags, version_post_tag)
+_version_t_ = Version(0, 3, 1, version_pre_tags, version_post_tag)
 _short_version_ = _basic_version(_version_t_)
 __version__ = _version_to_string(_version_t_)
 
-_version_min_python_t_ = Version(3, 6, 0, [], '')
+_version_min_python_t_ = Version(3, 10, 0, [], '')
 _version_min_python_ = _version_to_string(_version_min_python_t_)
```

### Comparing `pymbs-0.3.0/pymbs/api.py` & `pymbs-0.3.1/pymbs/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 __all__ = ['load_deal', 'load_assumed_collat', 'load_model', 'run_collat_cf',
            'run_wals', 'show_wals', 'load_tranches', 'disperse_cf']
 
 logger = get_logger(__name__)
 
 pd.set_option('display.max_rows', config.max_rows)
-pd.set_option('precision', config.precision)
+pd.set_option('display.precision', config.precision)
 
 
 def load_deal(series_id: str) -> dict:
     """Load the Terms Sheet for the REMIC Series name provided.
 
     The Terms Sheet is essential for modeling the deal. If this function is
     not called at the start, most of the other functions will fail.
```

### Comparing `pymbs-0.3.0/pymbs/config/pymbs_logging.json` & `pymbs-0.3.1/pymbs/config/pymbs_logging.json`

 * *Files identical despite different names*

### Comparing `pymbs-0.3.0/pymbs/config.py` & `pymbs-0.3.1/pymbs/config.py`

 * *Files identical despite different names*

### Comparing `pymbs-0.3.0/pymbs/core.py` & `pymbs-0.3.1/pymbs/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,16 +70,28 @@
             try:
                 group_collat = ts['groups'][group].get('collateral')
             except KeyError:
                 raise CollatError(group)
             if group_collat:
                 ac = _get_assumed_collat(group, group_collat)
                 if assumed_collat is not None:
-                    assumed_collat = assumed_collat.append(
-                        ac, ignore_index=True
+                    # TODO: Refactor to pass a curated list to the
+                    # - DataFrame constructor
+                    # As of pandas 2.0, append (previously deprecated)
+                    # was removed.  You need to use concat instead, and
+                    # even this is really not ideal.  It's better to
+                    # create/append to a python list first, then pass that
+                    # list to the DataFrame constructor, if possible.
+                    # See https://github.com/pandas-dev/pandas/issues/35407
+                    # for more information.
+                    # We'll use `concat` here for now, as a quick fix, but
+                    # we should implement an appropriate long-term fix in
+                    # the future.
+                    assumed_collat = pd.concat(
+                        [assumed_collat, ac], ignore_index=True
                     )
                 else:
                     assumed_collat = ac
     else:
         try:
             group_collat = ts['groups'][group_id].get('collateral')
         except KeyError:
@@ -96,16 +108,19 @@
 def _get_assumed_collat(group_id, group_collat):
     assumed_collat = None
     assumed = group_collat.get('assumed')
     if assumed:
         for item in assumed:
             if assumed_collat is not None:
                 item['group_id'] = group_id
-                assumed_collat = assumed_collat.append(
-                    pd.Series(item), ignore_index=True
+                # TODO: Refactor to pass a curated list to the
+                # - DataFrame constructor
+                # - See TODO in _load_assumed_collat, above
+                assumed_collat = pd.concat(
+                    [assumed_collat, pd.Series(item)], ignore_index=True
                 )
             else:
                 assumed_collat = pd.DataFrame(item, index=[0])
                 assumed_collat.insert(0, "group_id", group_id)
 
     return assumed_collat
 
@@ -440,15 +455,37 @@
     return wals
 
 
 def _pivot_wal_table(wals):
     column_order = [wal for wal in wals['prepay_scenario'].unique()]
 
     def f(x):
-        return (x.pivot('tranche_id', 'prepay_scenario', 'wal'))
+        """The pandas.DataFrame.pivot method now expects named parameters
+        rather than positional parameters.
+
+        Args:
+            columns: str or object or a list of str
+                     Column to use to make new frame’s columns.
+
+            index: str or object or a list of str, optional
+                   Column to use to make new frame’s index. If not given,
+                   uses existing index.
+
+            values: str, object or a list of the previous, optional
+                    Column(s) to use for populating new frame’s values.
+                    If not specified, all remaining columns will be used and
+                    the result will have hierarchically indexed columns.
+        """
+        return (
+            x.pivot(
+                index='tranche_id',
+                columns='prepay_scenario',
+                values='wal'
+            )
+        )
 
     _wal_table = wals.groupby('group_id', group_keys=True).apply(f)
     wal_table = _wal_table.reindex(columns=column_order)
 
     return wal_table
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymbs-0.3.0/pymbs/enums.py` & `pymbs-0.3.1/pymbs/enums.py`

 * *Files identical despite different names*

### Comparing `pymbs-0.3.0/pymbs/exceptions.py` & `pymbs-0.3.1/pymbs/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymbs-0.3.0/pymbs/log.py` & `pymbs-0.3.1/pymbs/log.py`

 * *Files identical despite different names*

### Comparing `pymbs-0.3.0/pymbs/payment_rules.py` & `pymbs-0.3.1/pymbs/payment_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,7 +133,11 @@
             if current_payment < cleanup:
                 current_payment = d0
             payment.buckets[bucket[0]] = current_payment
 
 
 def pay_concurrent(bucket, tranches, ratios):
     pass
+
+
+def pay_to_schedule(bucket, tranches, schedule):
+    pass
```

### Comparing `pymbs-0.3.0/pymbs/tranche.py` & `pymbs-0.3.1/pymbs/tranche.py`

 * *Files identical despite different names*

### Comparing `pymbs-0.3.0/pymbs/utils.py` & `pymbs-0.3.1/pymbs/utils.py`

 * *Files identical despite different names*

### Comparing `pymbs-0.3.0/pymbs.egg-info/PKG-INFO` & `pymbs-0.3.1/pymbs.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,75 @@
 Metadata-Version: 2.1
 Name: pymbs
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library for use in modeling Mortgage-Backed Securities.
 Home-page: https://pypi.org/project/pymbs/
 Author: Brian Farrell
 Author-email: brian.farrell@me.com
 License: AGPLv3
-Description: 
-        ============
-        Introduction
-        ============
-        
-        PyMBS is a Python library for use in modeling Mortgage-Backed Securities.
-        
-            * This is a modern Python library that requires ``Python>=3.6``
-        
-        
-        Objectives
-        ----------
-        #. Create a modern, stable Python library with a clearly-defined API  
-        #. Provide as close to 100% Test Coverage as possible [#f1]_
-        #. Provide clear documentation with full coverage of the API and example code.
-        
-        
-        
-        Installing
-        ----------
-        
-        Install using `conda`:
-        
-        .. code-block:: bash
-        
-           conda install -c btf pymbs
-        
-        
-        Install using `pip`:
-        
-        .. code-block:: bash
-        
-           pip install pymbs
-        
-        
-        Links
-        -----
-        
-        * Documentation: https://brianfarrell.gitlab.io/pymbs/
-        * License: https://www.gnu.org/licenses/agpl.html
-        * Anaconda Cloud: https://anaconda.org/btf/pymbs/
-        * PyPi Releases: https://pypi.org/project/pymbs/
-        * Code: https://gitlab.trove.fm/btf/pymbs
-        * Issue tracker:
-        * Test status:
-        * Test coverage:
-        
-        .. rubric:: Footnotes
-        
-        .. [#f1] | This project started-out as a Proof of Concept (POC).
-                 | At that point, no automated testing was involved.
-                 | Going forward, all new development and bug fixes will be test-driven.
-        
 Keywords: financial modeling analysis mortgage securities
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.6.0
+Requires-Python: >=3.10.0
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+
+============
+Introduction
+============
+
+PyMBS is a Python library for use in modeling Mortgage-Backed Securities.
+
+    * This is a modern Python library that requires ``Python>=3.10``
+
+
+Objectives
+----------
+#. Create a modern, stable Python library with a clearly-defined API  
+#. Provide as close to 100% Test Coverage as possible [#f1]_
+#. Provide clear documentation with full coverage of the API and example code.
+
+
+
+Installing
+----------
+
+Install using `conda`:
+
+.. code-block:: bash
+
+   conda install -c btf pymbs
+
+
+Install using `pip`:
+
+.. code-block:: bash
+
+   pip install pymbs
+
+
+Links
+-----
+
+* Documentation: https://brianfarrell.gitlab.io/pymbs/
+* License: https://www.gnu.org/licenses/agpl.html
+* Anaconda Cloud: https://anaconda.org/btf/pymbs/
+* PyPi Releases: https://pypi.org/project/pymbs/
+* Code: https://gitlab.com/brianfarrell/pymbs
+
+.. rubric:: Footnotes
+
+.. [#f1] | This project started-out as a Proof of Concept (POC).
+         | At that point, no automated testing was involved.
+         | Going forward, all new development and bug fixes will be test-driven.
```

### Comparing `pymbs-0.3.0/setup.py` & `pymbs-0.3.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,33 +23,34 @@
 
 from pymbs.__version__ import __version__, _version_min_python_
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 required = [
-    "ipython>=7.7.0",
-    "jinja2>=2.10.1",
-    "numpy>=1.16.4",
-    "pandas>=0.25.0",
-    "pyyaml>=5.1.2",
+    "ipython>=8.14.0",
+    "jinja2>=3.1.2",
+    "numpy>=1.23.5",
+    "numpy-financial>=1.0.0",
+    "pandas>=2.0.2",
+    "pyyaml>=6.0",
 ]
 
 setup(
     name='pymbs',
     version=__version__,
     python_requires=f">={_version_min_python_}",
     install_requires=required,
     setup_requires=required,
 
     packages=find_packages(
         exclude=["*.tests", "*.tests.*", "tests.*", "tests"]
     ),
     package_data={
-        'pymbs': ['config/*.json', 'config/*.yaml', 'templates/*.html'],
+        'pymbs': ['config/*.json', 'config/*.yaml', 'templates/*.j2'],
     },
 
     license='AGPLv3',
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Financial and Insurance Industry",
         "License :: OSI Approved :: GNU Affero General Public License v3",
```

