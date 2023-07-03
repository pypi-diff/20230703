# Comparing `tmp/chainsaddiction-0.2.3.tar.gz` & `tmp/chainsaddiction-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainsaddiction-0.2.3.tar", last modified: Sun Jul  2 20:07:13 2023, max compression
+gzip compressed data, was "chainsaddiction-0.2.4.tar", last modified: Mon Jul  3 19:28:34 2023, max compression
```

## Comparing `chainsaddiction-0.2.3.tar` & `chainsaddiction-0.2.4.tar`

### file list

```diff
@@ -1,272 +1,272 @@
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:13.002029 chainsaddiction-0.2.3/
--rw-r--r--   0 pmind      (502) staff       (20)      235 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/.gitignore
--rw-r--r--   0 pmind      (502) staff       (20)       96 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/.gitmodules
--rw-r--r--   0 pmind      (502) staff       (20)      336 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/.readthedocs.yaml
--rw-r--r--   0 pmind      (502) staff       (20)      335 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/CHANGELOG.md
--rw-r--r--   0 pmind      (502) staff       (20)     1487 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/LICENSE
--rw-r--r--   0 pmind      (502) staff       (20)       58 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/MANIFEST.in
--rw-r--r--   0 pmind      (502) staff       (20)     1938 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)     3851 2023-07-02 20:07:12.999961 chainsaddiction-0.2.3/PKG-INFO
--rw-r--r--   0 pmind      (502) staff       (20)     1223 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/README.md
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.778272 chainsaddiction-0.2.3/docs/
--rw-r--r--   0 pmind      (502) staff       (20)      584 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)      791 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/make.bat
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.781376 chainsaddiction-0.2.3/docs/source/
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.782178 chainsaddiction-0.2.3/docs/source/api/
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.787760 chainsaddiction-0.2.3/docs/source/api/c/
--rw-r--r--   0 pmind      (502) staff       (20)      483 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/api/c/basics.rst
--rw-r--r--   0 pmind      (502) staff       (20)     1792 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/api/c/dataset.rst
--rw-r--r--   0 pmind      (502) staff       (20)      279 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/api/c/index.rst
--rw-r--r--   0 pmind      (502) staff       (20)      116 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/api/c/internal.rst
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.792087 chainsaddiction-0.2.3/docs/source/api/c/poishmm/
--rw-r--r--   0 pmind      (502) staff       (20)      200 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/api/c/poishmm/index.rst
--rw-r--r--   0 pmind      (502) staff       (20)     5120 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/api/c/poishmm/pois-hmm.rst
--rw-r--r--   0 pmind      (502) staff       (20)     4161 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/api/c/poishmm/pois-params.rst
--rw-r--r--   0 pmind      (502) staff       (20)     1952 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/api/c/poishmm/pois-probs.rst
--rw-r--r--   0 pmind      (502) staff       (20)     2260 2023-06-30 09:02:51.000000 chainsaddiction-0.2.3/docs/source/api/c/utils.rst
--rw-r--r--   0 pmind      (502) staff       (20)      337 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/api/index.rst
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.794834 chainsaddiction-0.2.3/docs/source/api/python/
--rw-r--r--   0 pmind      (502) staff       (20)      169 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/api/python/index.rst
--rw-r--r--   0 pmind      (502) staff       (20)     2123 2023-06-30 09:02:51.000000 chainsaddiction-0.2.3/docs/source/api/python/poishmm.rst
--rw-r--r--   0 pmind      (502) staff       (20)      805 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/api/python/utils.rst
--rw-r--r--   0 pmind      (502) staff       (20)     1897 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/conf.py
--rw-r--r--   0 pmind      (502) staff       (20)     2229 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/docs/source/getting-started.rst
--rw-r--r--   0 pmind      (502) staff       (20)      526 2023-06-30 09:02:51.000000 chainsaddiction-0.2.3/docs/source/index.rst
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.796251 chainsaddiction-0.2.3/docs/source/usrguide/
--rw-r--r--   0 pmind      (502) staff       (20)     1442 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/usrguide/examples.rst
--rw-r--r--   0 pmind      (502) staff       (20)      198 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/docs/source/usrguide/index.rst
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.798458 chainsaddiction-0.2.3/include/
--rw-r--r--   0 pmind      (502) staff       (20)      464 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/include/chainsaddiction.h
--rw-r--r--   0 pmind      (502) staff       (20)      159 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/include/libvmath.h
--rw-r--r--   0 pmind      (502) staff       (20)     1079 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/pyproject.toml
--rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-30 09:02:51.000000 chainsaddiction-0.2.3/requirements-dev.txt
--rw-r--r--   0 pmind      (502) staff       (20)       38 2023-07-02 20:07:13.002449 chainsaddiction-0.2.3/setup.cfg
--rw-r--r--   0 pmind      (502) staff       (20)     1458 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/setup.py
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.759240 chainsaddiction-0.2.3/src/
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.809973 chainsaddiction-0.2.3/src/chainsaddiction/
--rw-r--r--   0 pmind      (502) staff       (20)      249 2023-07-02 14:18:19.000000 chainsaddiction-0.2.3/src/chainsaddiction/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)        0 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/__init__.py
--rw-r--r--   0 pmind      (502) staff       (20)     2026 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/dataset.c
--rw-r--r--   0 pmind      (502) staff       (20)     1953 2023-07-02 14:48:22.000000 chainsaddiction-0.2.3/src/chainsaddiction/dataset.h
--rw-r--r--   0 pmind      (502) staff       (20)      301 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/err.h
--rw-r--r--   0 pmind      (502) staff       (20)      861 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/libma.c
--rw-r--r--   0 pmind      (502) staff       (20)     1831 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/libma.h
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.828990 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/
--rw-r--r--   0 pmind      (502) staff       (20)     1240 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)      294 2023-06-30 09:02:51.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/__init__.pyi
--rw-r--r--   0 pmind      (502) staff       (20)     4383 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-em.c
--rw-r--r--   0 pmind      (502) staff       (20)     2212 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-em.h
--rw-r--r--   0 pmind      (502) staff       (20)     1844 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-fwbw.c
--rw-r--r--   0 pmind      (502) staff       (20)     2153 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-fwbw.h
--rw-r--r--   0 pmind      (502) staff       (20)     4864 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-hmm.c
--rw-r--r--   0 pmind      (502) staff       (20)     2099 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-hmm.h
--rw-r--r--   0 pmind      (502) staff       (20)     4534 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-params.c
--rw-r--r--   0 pmind      (502) staff       (20)     2116 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-params.h
--rw-r--r--   0 pmind      (502) staff       (20)      964 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-probs.c
--rw-r--r--   0 pmind      (502) staff       (20)     1130 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-probs.h
--rw-r--r--   0 pmind      (502) staff       (20)     9619 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/poishmm-module.c
--rw-r--r--   0 pmind      (502) staff       (20)     1109 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/poishmm-module.h
--rw-r--r--   0 pmind      (502) staff       (20)     2263 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/poishmm-object.h
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.841528 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/
--rw-r--r--   0 pmind      (502) staff       (20)     1594 2023-07-02 11:49:32.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/Makefile
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.847042 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/data/
--rw-r--r--   0 pmind      (502) staff       (20)      222 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/data/earthquakes.lprobs
--rw-r--r--   0 pmind      (502) staff       (20)       85 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/data/params-3s
--rw-r--r--   0 pmind      (502) staff       (20)      199 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/data/params-4s
--rw-r--r--   0 pmind      (502) staff       (20)      101 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/data/ppr1
--rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/data/ppr2
--rw-r--r--   0 pmind      (502) staff       (20)      110 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/data/ppr3
--rw-r--r--   0 pmind      (502) staff       (20)      119 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/data/ppr4
--rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/data/ppr5
--rw-r--r--   0 pmind      (502) staff       (20)      135 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/data/std3s.poisparams
--rw-r--r--   0 pmind      (502) staff       (20)      896 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/runtest.c
--rw-r--r--   0 pmind      (502) staff       (20)     4808 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-em.c
--rw-r--r--   0 pmind      (502) staff       (20)      294 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-em.h
--rw-r--r--   0 pmind      (502) staff       (20)     6676 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-hmm.c
--rw-r--r--   0 pmind      (502) staff       (20)      546 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-hmm.h
--rw-r--r--   0 pmind      (502) staff       (20)     1239 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-params.c
--rw-r--r--   0 pmind      (502) staff       (20)      220 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-params.h
--rw-r--r--   0 pmind      (502) staff       (20)      699 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-probs.c
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-probs.h
--rw-r--r--   0 pmind      (502) staff       (20)        0 2023-06-30 09:02:51.000000 chainsaddiction-0.2.3/src/chainsaddiction/py.typed
--rw-r--r--   0 pmind      (502) staff       (20)     3103 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/read.c
--rw-r--r--   0 pmind      (502) staff       (20)     1556 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/read.h
--rw-r--r--   0 pmind      (502) staff       (20)      196 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/restrict.h
--rw-r--r--   0 pmind      (502) staff       (20)      335 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/scalar.h
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.850698 chainsaddiction-0.2.3/src/chainsaddiction/tests/
--rw-r--r--   0 pmind      (502) staff       (20)      822 2023-07-02 14:18:30.000000 chainsaddiction-0.2.3/src/chainsaddiction/tests/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)      593 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/tests/runtest.c
--rw-r--r--   0 pmind      (502) staff       (20)     2464 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/tests/test-dataset.c
--rw-r--r--   0 pmind      (502) staff       (20)      626 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/tests/test-dataset.h
--rw-r--r--   0 pmind      (502) staff       (20)     3103 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/tests/test-read.c
--rw-r--r--   0 pmind      (502) staff       (20)      397 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/tests/test-read.h
--rw-r--r--   0 pmind      (502) staff       (20)      142 2023-06-30 09:02:51.000000 chainsaddiction-0.2.3/src/chainsaddiction/typing.py
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.855020 chainsaddiction-0.2.3/src/chainsaddiction/utils/
--rw-r--r--   0 pmind      (502) staff       (20)      430 2023-07-02 11:08:18.000000 chainsaddiction-0.2.3/src/chainsaddiction/utils/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)      207 2023-06-30 09:02:51.000000 chainsaddiction-0.2.3/src/chainsaddiction/utils/__init__.pyi
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.859702 chainsaddiction-0.2.3/src/chainsaddiction/utils/tests/
--rw-r--r--   0 pmind      (502) staff       (20)     1116 2023-07-02 14:25:01.000000 chainsaddiction-0.2.3/src/chainsaddiction/utils/tests/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)      169 2023-07-02 13:06:36.000000 chainsaddiction-0.2.3/src/chainsaddiction/utils/tests/runtest.c
--rw-r--r--   0 pmind      (502) staff       (20)     2280 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/utils/tests/test-utils.c
--rw-r--r--   0 pmind      (502) staff       (20)      248 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/utils/tests/test-utils.h
--rw-r--r--   0 pmind      (502) staff       (20)     4882 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/chainsaddiction/utils/utils-module.c
--rw-r--r--   0 pmind      (502) staff       (20)      795 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/utils/utils-module.h
--rw-r--r--   0 pmind      (502) staff       (20)     3119 2023-07-01 19:30:23.000000 chainsaddiction-0.2.3/src/chainsaddiction/utils/utils.c
--rw-r--r--   0 pmind      (502) staff       (20)     1467 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/chainsaddiction/utils/utils.h
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.813672 chainsaddiction-0.2.3/src/chainsaddiction.egg-info/
--rw-r--r--   0 pmind      (502) staff       (20)     3851 2023-07-02 20:07:12.000000 chainsaddiction-0.2.3/src/chainsaddiction.egg-info/PKG-INFO
--rw-r--r--   0 pmind      (502) staff       (20)     7974 2023-07-02 20:07:12.000000 chainsaddiction-0.2.3/src/chainsaddiction.egg-info/SOURCES.txt
--rw-r--r--   0 pmind      (502) staff       (20)        1 2023-07-02 20:07:12.000000 chainsaddiction-0.2.3/src/chainsaddiction.egg-info/dependency_links.txt
--rw-r--r--   0 pmind      (502) staff       (20)        6 2023-07-02 20:07:12.000000 chainsaddiction-0.2.3/src/chainsaddiction.egg-info/requires.txt
--rw-r--r--   0 pmind      (502) staff       (20)       22 2023-07-02 20:07:12.000000 chainsaddiction-0.2.3/src/chainsaddiction.egg-info/top_level.txt
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.872678 chainsaddiction-0.2.3/src/vmath/
--rw-r--r--   0 pmind      (502) staff       (20)      659 2023-07-02 10:49:38.000000 chainsaddiction-0.2.3/src/vmath/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)      773 2023-07-02 10:49:20.000000 chainsaddiction-0.2.3/src/vmath/alloc.h
--rw-r--r--   0 pmind      (502) staff       (20)      440 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/vmath/config.h
--rw-r--r--   0 pmind      (502) staff       (20)     1473 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/vmath/core.c
--rw-r--r--   0 pmind      (502) staff       (20)      932 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/vmath/core.h
--rw-r--r--   0 pmind      (502) staff       (20)     4047 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/vmath/print.h
--rw-r--r--   0 pmind      (502) staff       (20)     1349 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/vmath/rnd.c
--rw-r--r--   0 pmind      (502) staff       (20)     2907 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/vmath/rnd.h
--rw-r--r--   0 pmind      (502) staff       (20)      682 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/vmath/stats.c
--rw-r--r--   0 pmind      (502) staff       (20)     1008 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/vmath/stats.h
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.884006 chainsaddiction-0.2.3/src/vmath/tests/
--rw-r--r--   0 pmind      (502) staff       (20)      807 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/vmath/tests/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)     1294 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/vmath/tests/runtest.c
--rw-r--r--   0 pmind      (502) staff       (20)     2573 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/vmath/tests/test_rnd.c
--rw-r--r--   0 pmind      (502) staff       (20)      344 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/vmath/tests/test_rnd.h
--rw-r--r--   0 pmind      (502) staff       (20)     1108 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/vmath/tests/test_stats.c
--rw-r--r--   0 pmind      (502) staff       (20)      273 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/vmath/tests/test_stats.h
--rw-r--r--   0 pmind      (502) staff       (20)    23250 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/vmath/tests/test_vmath.c
--rw-r--r--   0 pmind      (502) staff       (20)     1182 2023-07-02 20:06:40.000000 chainsaddiction-0.2.3/src/vmath/tests/test_vmath.h
--rw-r--r--   0 pmind      (502) staff       (20)    13402 2023-07-02 19:08:05.000000 chainsaddiction-0.2.3/src/vmath/vmath.c
--rw-r--r--   0 pmind      (502) staff       (20)    18516 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/src/vmath/vmath.h
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.891368 chainsaddiction-0.2.3/tests/
--rw-r--r--   0 pmind      (502) staff       (20)      142 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)      179 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/README
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.898804 chainsaddiction-0.2.3/tests/data/
--rw-r--r--   0 pmind      (502) staff       (20)     1299 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/S4_N100
--rw-r--r--   0 pmind      (502) staff       (20)     6535 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/S4_N500
--rw-r--r--   0 pmind      (502) staff       (20)      967 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/S4_N50_MID
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.900416 chainsaddiction-0.2.3/tests/data/centroids/
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.909180 chainsaddiction-0.2.3/tests/data/centroids/2s/
--rw-r--r--   0 pmind      (502) staff       (20)        8 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/2s/delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)       93 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/2s/gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/2s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)      100 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/2s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      489 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/2s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/2s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)    68467 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/2s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)       43 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/2s/lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)    68421 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/2s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)    72888 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/2s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/2s/local-decoding.txt
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.919295 chainsaddiction-0.2.3/tests/data/centroids/3s/
--rw-r--r--   0 pmind      (502) staff       (20)       12 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/3s/delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      187 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/3s/gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/3s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)      100 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/3s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      489 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/3s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/3s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)   102650 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/3s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)       64 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/3s/lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)   102555 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/3s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)   105803 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/3s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/3s/local-decoding.txt
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.931388 chainsaddiction-0.2.3/tests/data/centroids/4s/
--rw-r--r--   0 pmind      (502) staff       (20)       38 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/4s/delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      356 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/4s/gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/4s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)      100 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/4s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      489 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/4s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/4s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)   135537 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/4s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)       85 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/4s/lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)   135631 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/4s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)   141473 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/4s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/4s/local-decoding.txt
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.946299 chainsaddiction-0.2.3/tests/data/centroids/5s/
--rw-r--r--   0 pmind      (502) staff       (20)       44 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/5s/delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      553 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/5s/gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/5s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)      100 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/5s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      489 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/5s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/5s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)   170825 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/5s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)      107 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/5s/lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)   170730 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/5s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)   176569 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/5s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/5s/local-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)     6164 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/centroids/centroids
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.947080 chainsaddiction-0.2.3/tests/data/earthquakes/
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.958894 chainsaddiction-0.2.3/tests/data/earthquakes/2s/
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/2s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/2s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      493 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/2s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       39 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/2s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)     4872 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/2s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)     4826 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/2s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)     5138 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/2s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)       27 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/2s/ldelta.txt
--rw-r--r--   0 pmind      (502) staff       (20)       93 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/2s/lgamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       42 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/2s/llambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/2s/local-decoding.txt
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.968229 chainsaddiction-0.2.3/tests/data/earthquakes/3s/
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/3s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/3s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      493 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/3s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       39 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/3s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)     7304 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/3s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)     7249 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/3s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)     7516 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/3s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)       50 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/3s/ldelta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      210 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/3s/lgamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/3s/llambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/3s/local-decoding.txt
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.980755 chainsaddiction-0.2.3/tests/data/earthquakes/4s/
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/4s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/4s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      493 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/4s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       39 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/4s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)     9724 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/4s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)     9672 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/4s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)     9894 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/4s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)       71 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/4s/ldelta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      368 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/4s/lgamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       88 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/4s/llambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/4s/local-decoding.txt
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.991639 chainsaddiction-0.2.3/tests/data/earthquakes/5s/
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/5s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/5s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      493 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/5s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       39 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/5s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)    12138 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/5s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)    12048 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/5s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)    12274 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/5s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)       76 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/5s/ldelta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      571 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/5s/lgamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)      110 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/5s/llambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/5s/local-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)      315 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/earthquakes/earthquakes
--rw-r--r--   0 pmind      (502) staff       (20)        0 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/empty
--rw-r--r--   0 pmind      (502) staff       (20)       31 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/params_2s
--rw-r--r--   0 pmind      (502) staff       (20)      104 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/params_3s
--rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/params_4s
--rw-r--r--   0 pmind      (502) staff       (20)      104 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/params_4s_MID
--rw-r--r--   0 pmind      (502) staff       (20)      206 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/test_15_100_50
--rw-r--r--   0 pmind      (502) staff       (20)       10 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/data/wrong_format
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.992372 chainsaddiction-0.2.3/tests/params/
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.766045 chainsaddiction-0.2.3/tests/params/earthquakes/
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.994610 chainsaddiction-0.2.3/tests/params/earthquakes/3/
--rw-r--r--   0 pmind      (502) staff       (20)      127 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/params/earthquakes/3/linear.p
--rw-r--r--   0 pmind      (502) staff       (20)      127 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/params/earthquakes/3/quantile.p
--rw-r--r--   0 pmind      (502) staff       (20)      127 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/params/earthquakes/3/random.p
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-02 20:07:12.998175 chainsaddiction-0.2.3/tests/params/earthquakes/4/
--rw-r--r--   0 pmind      (502) staff       (20)      250 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/params/earthquakes/4/linear.p
--rw-r--r--   0 pmind      (502) staff       (20)      228 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/params/earthquakes/4/quantile.p
--rw-r--r--   0 pmind      (502) staff       (20)      232 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/params/earthquakes/4/random.p
--rw-r--r--   0 pmind      (502) staff       (20)      199 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/params/params-4s
--rw-r--r--   0 pmind      (502) staff       (20)      862 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/test-ext-earthquakes.py
--rw-r--r--   0 pmind      (502) staff       (20)     1069 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/test-utils.py
--rw-r--r--   0 pmind      (502) staff       (20)     1084 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tests/utils.py
--rw-r--r--   0 pmind      (502) staff       (20)      101 2023-06-20 13:23:44.000000 chainsaddiction-0.2.3/tox.ini
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:34.091040 chainsaddiction-0.2.4/
+-rw-r--r--   0 pmind      (502) staff       (20)      235 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/.gitignore
+-rw-r--r--   0 pmind      (502) staff       (20)       96 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/.gitmodules
+-rw-r--r--   0 pmind      (502) staff       (20)      336 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/.readthedocs.yaml
+-rw-r--r--   0 pmind      (502) staff       (20)      387 2023-07-03 19:27:22.000000 chainsaddiction-0.2.4/CHANGELOG.md
+-rw-r--r--   0 pmind      (502) staff       (20)     1487 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/LICENSE
+-rw-r--r--   0 pmind      (502) staff       (20)       58 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/MANIFEST.in
+-rw-r--r--   0 pmind      (502) staff       (20)     1938 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/Makefile
+-rw-r--r--   0 pmind      (502) staff       (20)     3851 2023-07-03 19:28:34.090579 chainsaddiction-0.2.4/PKG-INFO
+-rw-r--r--   0 pmind      (502) staff       (20)     1223 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/README.md
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.717789 chainsaddiction-0.2.4/docs/
+-rw-r--r--   0 pmind      (502) staff       (20)      584 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/Makefile
+-rw-r--r--   0 pmind      (502) staff       (20)      791 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/make.bat
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.722085 chainsaddiction-0.2.4/docs/source/
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.724496 chainsaddiction-0.2.4/docs/source/api/
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.733572 chainsaddiction-0.2.4/docs/source/api/c/
+-rw-r--r--   0 pmind      (502) staff       (20)      483 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/api/c/basics.rst
+-rw-r--r--   0 pmind      (502) staff       (20)     1792 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/api/c/dataset.rst
+-rw-r--r--   0 pmind      (502) staff       (20)      279 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/api/c/index.rst
+-rw-r--r--   0 pmind      (502) staff       (20)      116 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/api/c/internal.rst
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.740144 chainsaddiction-0.2.4/docs/source/api/c/poishmm/
+-rw-r--r--   0 pmind      (502) staff       (20)      200 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/api/c/poishmm/index.rst
+-rw-r--r--   0 pmind      (502) staff       (20)     5120 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/api/c/poishmm/pois-hmm.rst
+-rw-r--r--   0 pmind      (502) staff       (20)     4161 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/api/c/poishmm/pois-params.rst
+-rw-r--r--   0 pmind      (502) staff       (20)     1952 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/api/c/poishmm/pois-probs.rst
+-rw-r--r--   0 pmind      (502) staff       (20)     2260 2023-06-30 09:02:51.000000 chainsaddiction-0.2.4/docs/source/api/c/utils.rst
+-rw-r--r--   0 pmind      (502) staff       (20)      337 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/api/index.rst
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.743869 chainsaddiction-0.2.4/docs/source/api/python/
+-rw-r--r--   0 pmind      (502) staff       (20)      169 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/api/python/index.rst
+-rw-r--r--   0 pmind      (502) staff       (20)     2123 2023-06-30 09:02:51.000000 chainsaddiction-0.2.4/docs/source/api/python/poishmm.rst
+-rw-r--r--   0 pmind      (502) staff       (20)      805 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/api/python/utils.rst
+-rw-r--r--   0 pmind      (502) staff       (20)     1897 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/conf.py
+-rw-r--r--   0 pmind      (502) staff       (20)     2229 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/docs/source/getting-started.rst
+-rw-r--r--   0 pmind      (502) staff       (20)      526 2023-06-30 09:02:51.000000 chainsaddiction-0.2.4/docs/source/index.rst
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.753147 chainsaddiction-0.2.4/docs/source/usrguide/
+-rw-r--r--   0 pmind      (502) staff       (20)     1442 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/usrguide/examples.rst
+-rw-r--r--   0 pmind      (502) staff       (20)      198 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/usrguide/index.rst
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.755857 chainsaddiction-0.2.4/include/
+-rw-r--r--   0 pmind      (502) staff       (20)      464 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/include/chainsaddiction.h
+-rw-r--r--   0 pmind      (502) staff       (20)      159 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/include/libvmath.h
+-rw-r--r--   0 pmind      (502) staff       (20)     1079 2023-07-03 19:27:22.000000 chainsaddiction-0.2.4/pyproject.toml
+-rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-30 09:02:51.000000 chainsaddiction-0.2.4/requirements-dev.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       38 2023-07-03 19:28:34.091168 chainsaddiction-0.2.4/setup.cfg
+-rw-r--r--   0 pmind      (502) staff       (20)     1458 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/setup.py
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.689972 chainsaddiction-0.2.4/src/
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.768633 chainsaddiction-0.2.4/src/chainsaddiction/
+-rw-r--r--   0 pmind      (502) staff       (20)      249 2023-07-02 14:18:19.000000 chainsaddiction-0.2.4/src/chainsaddiction/Makefile
+-rw-r--r--   0 pmind      (502) staff       (20)        0 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/__init__.py
+-rw-r--r--   0 pmind      (502) staff       (20)     2028 2023-07-03 19:27:22.000000 chainsaddiction-0.2.4/src/chainsaddiction/dataset.c
+-rw-r--r--   0 pmind      (502) staff       (20)     1953 2023-07-03 18:58:10.000000 chainsaddiction-0.2.4/src/chainsaddiction/dataset.h
+-rw-r--r--   0 pmind      (502) staff       (20)      301 2023-07-03 18:58:31.000000 chainsaddiction-0.2.4/src/chainsaddiction/err.h
+-rw-r--r--   0 pmind      (502) staff       (20)      861 2023-07-03 18:59:33.000000 chainsaddiction-0.2.4/src/chainsaddiction/libma.c
+-rw-r--r--   0 pmind      (502) staff       (20)     1831 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/libma.h
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.788627 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/
+-rw-r--r--   0 pmind      (502) staff       (20)     1240 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/Makefile
+-rw-r--r--   0 pmind      (502) staff       (20)      543 2023-07-03 19:27:22.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/__init__.pyi
+-rw-r--r--   0 pmind      (502) staff       (20)     4383 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-em.c
+-rw-r--r--   0 pmind      (502) staff       (20)     2212 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-em.h
+-rw-r--r--   0 pmind      (502) staff       (20)     1844 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-fwbw.c
+-rw-r--r--   0 pmind      (502) staff       (20)     2153 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-fwbw.h
+-rw-r--r--   0 pmind      (502) staff       (20)     4864 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-hmm.c
+-rw-r--r--   0 pmind      (502) staff       (20)     2099 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-hmm.h
+-rw-r--r--   0 pmind      (502) staff       (20)     4534 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-params.c
+-rw-r--r--   0 pmind      (502) staff       (20)     2116 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-params.h
+-rw-r--r--   0 pmind      (502) staff       (20)      965 2023-07-03 19:27:22.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-probs.c
+-rw-r--r--   0 pmind      (502) staff       (20)     1132 2023-07-03 19:27:22.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-probs.h
+-rw-r--r--   0 pmind      (502) staff       (20)     9737 2023-07-03 19:27:22.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/poishmm-module.c
+-rw-r--r--   0 pmind      (502) staff       (20)     1108 2023-07-03 19:27:22.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/poishmm-module.h
+-rw-r--r--   0 pmind      (502) staff       (20)     2417 2023-07-03 19:27:22.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/poishmm-object.h
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.799414 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/
+-rw-r--r--   0 pmind      (502) staff       (20)     1594 2023-07-02 11:49:32.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/Makefile
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.814244 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/data/
+-rw-r--r--   0 pmind      (502) staff       (20)      222 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/data/earthquakes.lprobs
+-rw-r--r--   0 pmind      (502) staff       (20)       85 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/data/params-3s
+-rw-r--r--   0 pmind      (502) staff       (20)      199 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/data/params-4s
+-rw-r--r--   0 pmind      (502) staff       (20)      101 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/data/ppr1
+-rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/data/ppr2
+-rw-r--r--   0 pmind      (502) staff       (20)      110 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/data/ppr3
+-rw-r--r--   0 pmind      (502) staff       (20)      119 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/data/ppr4
+-rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/data/ppr5
+-rw-r--r--   0 pmind      (502) staff       (20)      135 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/data/std3s.poisparams
+-rw-r--r--   0 pmind      (502) staff       (20)      896 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/runtest.c
+-rw-r--r--   0 pmind      (502) staff       (20)     4808 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-em.c
+-rw-r--r--   0 pmind      (502) staff       (20)      294 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-em.h
+-rw-r--r--   0 pmind      (502) staff       (20)     6676 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-hmm.c
+-rw-r--r--   0 pmind      (502) staff       (20)      546 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-hmm.h
+-rw-r--r--   0 pmind      (502) staff       (20)     1239 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-params.c
+-rw-r--r--   0 pmind      (502) staff       (20)      220 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-params.h
+-rw-r--r--   0 pmind      (502) staff       (20)      699 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-probs.c
+-rw-r--r--   0 pmind      (502) staff       (20)      214 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-probs.h
+-rw-r--r--   0 pmind      (502) staff       (20)        0 2023-06-30 09:02:51.000000 chainsaddiction-0.2.4/src/chainsaddiction/py.typed
+-rw-r--r--   0 pmind      (502) staff       (20)     3103 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/chainsaddiction/read.c
+-rw-r--r--   0 pmind      (502) staff       (20)     1561 2023-07-03 19:27:22.000000 chainsaddiction-0.2.4/src/chainsaddiction/read.h
+-rw-r--r--   0 pmind      (502) staff       (20)      196 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/restrict.h
+-rw-r--r--   0 pmind      (502) staff       (20)      337 2023-07-03 19:27:22.000000 chainsaddiction-0.2.4/src/chainsaddiction/scalar.h
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.823988 chainsaddiction-0.2.4/src/chainsaddiction/tests/
+-rw-r--r--   0 pmind      (502) staff       (20)      822 2023-07-02 14:18:30.000000 chainsaddiction-0.2.4/src/chainsaddiction/tests/Makefile
+-rw-r--r--   0 pmind      (502) staff       (20)      593 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/tests/runtest.c
+-rw-r--r--   0 pmind      (502) staff       (20)     2464 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/tests/test-dataset.c
+-rw-r--r--   0 pmind      (502) staff       (20)      626 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/tests/test-dataset.h
+-rw-r--r--   0 pmind      (502) staff       (20)     3103 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/tests/test-read.c
+-rw-r--r--   0 pmind      (502) staff       (20)      397 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/tests/test-read.h
+-rw-r--r--   0 pmind      (502) staff       (20)      142 2023-06-30 09:02:51.000000 chainsaddiction-0.2.4/src/chainsaddiction/typing.py
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.834888 chainsaddiction-0.2.4/src/chainsaddiction/utils/
+-rw-r--r--   0 pmind      (502) staff       (20)      430 2023-07-02 11:08:18.000000 chainsaddiction-0.2.4/src/chainsaddiction/utils/Makefile
+-rw-r--r--   0 pmind      (502) staff       (20)      207 2023-06-30 09:02:51.000000 chainsaddiction-0.2.4/src/chainsaddiction/utils/__init__.pyi
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.839293 chainsaddiction-0.2.4/src/chainsaddiction/utils/tests/
+-rw-r--r--   0 pmind      (502) staff       (20)     1116 2023-07-02 14:25:01.000000 chainsaddiction-0.2.4/src/chainsaddiction/utils/tests/Makefile
+-rw-r--r--   0 pmind      (502) staff       (20)      169 2023-07-02 13:06:36.000000 chainsaddiction-0.2.4/src/chainsaddiction/utils/tests/runtest.c
+-rw-r--r--   0 pmind      (502) staff       (20)     2280 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/chainsaddiction/utils/tests/test-utils.c
+-rw-r--r--   0 pmind      (502) staff       (20)      248 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/chainsaddiction/utils/tests/test-utils.h
+-rw-r--r--   0 pmind      (502) staff       (20)     4882 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/chainsaddiction/utils/utils-module.c
+-rw-r--r--   0 pmind      (502) staff       (20)      795 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/utils/utils-module.h
+-rw-r--r--   0 pmind      (502) staff       (20)     3119 2023-07-01 19:30:23.000000 chainsaddiction-0.2.4/src/chainsaddiction/utils/utils.c
+-rw-r--r--   0 pmind      (502) staff       (20)     1467 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/utils/utils.h
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.773143 chainsaddiction-0.2.4/src/chainsaddiction.egg-info/
+-rw-r--r--   0 pmind      (502) staff       (20)     3851 2023-07-03 19:28:33.000000 chainsaddiction-0.2.4/src/chainsaddiction.egg-info/PKG-INFO
+-rw-r--r--   0 pmind      (502) staff       (20)     7974 2023-07-03 19:28:33.000000 chainsaddiction-0.2.4/src/chainsaddiction.egg-info/SOURCES.txt
+-rw-r--r--   0 pmind      (502) staff       (20)        1 2023-07-03 19:28:33.000000 chainsaddiction-0.2.4/src/chainsaddiction.egg-info/dependency_links.txt
+-rw-r--r--   0 pmind      (502) staff       (20)        6 2023-07-03 19:28:33.000000 chainsaddiction-0.2.4/src/chainsaddiction.egg-info/requires.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       22 2023-07-03 19:28:33.000000 chainsaddiction-0.2.4/src/chainsaddiction.egg-info/top_level.txt
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.908062 chainsaddiction-0.2.4/src/vmath/
+-rw-r--r--   0 pmind      (502) staff       (20)      659 2023-07-02 10:49:38.000000 chainsaddiction-0.2.4/src/vmath/Makefile
+-rw-r--r--   0 pmind      (502) staff       (20)      773 2023-07-02 10:49:20.000000 chainsaddiction-0.2.4/src/vmath/alloc.h
+-rw-r--r--   0 pmind      (502) staff       (20)      440 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/vmath/config.h
+-rw-r--r--   0 pmind      (502) staff       (20)     1473 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/vmath/core.c
+-rw-r--r--   0 pmind      (502) staff       (20)      932 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/vmath/core.h
+-rw-r--r--   0 pmind      (502) staff       (20)     4047 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/vmath/print.h
+-rw-r--r--   0 pmind      (502) staff       (20)     1349 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/vmath/rnd.c
+-rw-r--r--   0 pmind      (502) staff       (20)     2907 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/vmath/rnd.h
+-rw-r--r--   0 pmind      (502) staff       (20)      682 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/vmath/stats.c
+-rw-r--r--   0 pmind      (502) staff       (20)     1008 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/vmath/stats.h
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.924279 chainsaddiction-0.2.4/src/vmath/tests/
+-rw-r--r--   0 pmind      (502) staff       (20)      807 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/vmath/tests/Makefile
+-rw-r--r--   0 pmind      (502) staff       (20)     1294 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/vmath/tests/runtest.c
+-rw-r--r--   0 pmind      (502) staff       (20)     2573 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/vmath/tests/test_rnd.c
+-rw-r--r--   0 pmind      (502) staff       (20)      344 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/vmath/tests/test_rnd.h
+-rw-r--r--   0 pmind      (502) staff       (20)     1108 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/vmath/tests/test_stats.c
+-rw-r--r--   0 pmind      (502) staff       (20)      273 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/vmath/tests/test_stats.h
+-rw-r--r--   0 pmind      (502) staff       (20)    23250 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/vmath/tests/test_vmath.c
+-rw-r--r--   0 pmind      (502) staff       (20)     1182 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/vmath/tests/test_vmath.h
+-rw-r--r--   0 pmind      (502) staff       (20)    13402 2023-07-02 19:08:05.000000 chainsaddiction-0.2.4/src/vmath/vmath.c
+-rw-r--r--   0 pmind      (502) staff       (20)    18516 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/vmath/vmath.h
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.932782 chainsaddiction-0.2.4/tests/
+-rw-r--r--   0 pmind      (502) staff       (20)      142 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/Makefile
+-rw-r--r--   0 pmind      (502) staff       (20)      179 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/README
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.949621 chainsaddiction-0.2.4/tests/data/
+-rw-r--r--   0 pmind      (502) staff       (20)     1299 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/S4_N100
+-rw-r--r--   0 pmind      (502) staff       (20)     6535 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/S4_N500
+-rw-r--r--   0 pmind      (502) staff       (20)      967 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/S4_N50_MID
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.950674 chainsaddiction-0.2.4/tests/data/centroids/
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.973070 chainsaddiction-0.2.4/tests/data/centroids/2s/
+-rw-r--r--   0 pmind      (502) staff       (20)        8 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/2s/delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       93 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/2s/gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/2s/global-decoding.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      100 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/2s/init-delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      489 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/2s/init-gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/2s/init-lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)    68467 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/2s/lalpha.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       43 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/2s/lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)    68421 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/2s/lbeta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)    72888 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/2s/lcsp.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/2s/local-decoding.txt
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.991444 chainsaddiction-0.2.4/tests/data/centroids/3s/
+-rw-r--r--   0 pmind      (502) staff       (20)       12 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/3s/delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      187 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/3s/gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/3s/global-decoding.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      100 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/3s/init-delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      489 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/3s/init-gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/3s/init-lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)   102650 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/3s/lalpha.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       64 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/3s/lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)   102555 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/3s/lbeta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)   105803 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/3s/lcsp.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/3s/local-decoding.txt
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:34.010329 chainsaddiction-0.2.4/tests/data/centroids/4s/
+-rw-r--r--   0 pmind      (502) staff       (20)       38 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/4s/delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      356 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/4s/gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/4s/global-decoding.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      100 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/4s/init-delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      489 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/4s/init-gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/4s/init-lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)   135537 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/4s/lalpha.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       85 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/4s/lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)   135631 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/4s/lbeta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)   141473 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/4s/lcsp.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/4s/local-decoding.txt
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:34.032920 chainsaddiction-0.2.4/tests/data/centroids/5s/
+-rw-r--r--   0 pmind      (502) staff       (20)       44 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/5s/delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      553 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/5s/gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/5s/global-decoding.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      100 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/5s/init-delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      489 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/5s/init-gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/5s/init-lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)   170825 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/5s/lalpha.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      107 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/5s/lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)   170730 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/5s/lbeta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)   176569 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/5s/lcsp.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/5s/local-decoding.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     6164 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/centroids
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:34.034250 chainsaddiction-0.2.4/tests/data/earthquakes/
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:34.043233 chainsaddiction-0.2.4/tests/data/earthquakes/2s/
+-rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/2s/global-decoding.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/2s/init-delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      493 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/2s/init-gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       39 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/2s/init-lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     4872 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/2s/lalpha.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     4826 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/2s/lbeta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     5138 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/2s/lcsp.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       27 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/2s/ldelta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       93 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/2s/lgamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       42 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/2s/llambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/2s/local-decoding.txt
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:34.057134 chainsaddiction-0.2.4/tests/data/earthquakes/3s/
+-rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/3s/global-decoding.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/3s/init-delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      493 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/3s/init-gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       39 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/3s/init-lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     7304 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/3s/lalpha.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     7249 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/3s/lbeta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     7516 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/3s/lcsp.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       50 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/3s/ldelta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      210 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/3s/lgamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/3s/llambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/3s/local-decoding.txt
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:34.069407 chainsaddiction-0.2.4/tests/data/earthquakes/4s/
+-rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/4s/global-decoding.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/4s/init-delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      493 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/4s/init-gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       39 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/4s/init-lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     9724 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/4s/lalpha.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     9672 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/4s/lbeta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)     9894 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/4s/lcsp.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       71 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/4s/ldelta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      368 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/4s/lgamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       88 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/4s/llambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/4s/local-decoding.txt
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:34.082521 chainsaddiction-0.2.4/tests/data/earthquakes/5s/
+-rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/5s/global-decoding.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/5s/init-delta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      493 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/5s/init-gamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       39 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/5s/init-lambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)    12138 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/5s/lalpha.txt
+-rw-r--r--   0 pmind      (502) staff       (20)    12048 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/5s/lbeta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)    12274 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/5s/lcsp.txt
+-rw-r--r--   0 pmind      (502) staff       (20)       76 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/5s/ldelta.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      571 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/5s/lgamma.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      110 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/5s/llambda.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/5s/local-decoding.txt
+-rw-r--r--   0 pmind      (502) staff       (20)      315 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/earthquakes
+-rw-r--r--   0 pmind      (502) staff       (20)        0 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/empty
+-rw-r--r--   0 pmind      (502) staff       (20)       31 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/params_2s
+-rw-r--r--   0 pmind      (502) staff       (20)      104 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/params_3s
+-rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/params_4s
+-rw-r--r--   0 pmind      (502) staff       (20)      104 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/params_4s_MID
+-rw-r--r--   0 pmind      (502) staff       (20)      206 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/test_15_100_50
+-rw-r--r--   0 pmind      (502) staff       (20)       10 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/wrong_format
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:34.083673 chainsaddiction-0.2.4/tests/params/
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.698583 chainsaddiction-0.2.4/tests/params/earthquakes/
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:34.086097 chainsaddiction-0.2.4/tests/params/earthquakes/3/
+-rw-r--r--   0 pmind      (502) staff       (20)      127 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/params/earthquakes/3/linear.p
+-rw-r--r--   0 pmind      (502) staff       (20)      127 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/params/earthquakes/3/quantile.p
+-rw-r--r--   0 pmind      (502) staff       (20)      127 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/params/earthquakes/3/random.p
+drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:34.089852 chainsaddiction-0.2.4/tests/params/earthquakes/4/
+-rw-r--r--   0 pmind      (502) staff       (20)      250 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/params/earthquakes/4/linear.p
+-rw-r--r--   0 pmind      (502) staff       (20)      228 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/params/earthquakes/4/quantile.p
+-rw-r--r--   0 pmind      (502) staff       (20)      232 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/params/earthquakes/4/random.p
+-rw-r--r--   0 pmind      (502) staff       (20)      199 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/params/params-4s
+-rw-r--r--   0 pmind      (502) staff       (20)      862 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/test-ext-earthquakes.py
+-rw-r--r--   0 pmind      (502) staff       (20)     1069 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/test-utils.py
+-rw-r--r--   0 pmind      (502) staff       (20)     1084 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/utils.py
+-rw-r--r--   0 pmind      (502) staff       (20)      101 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tox.ini
```

### Comparing `chainsaddiction-0.2.3/LICENSE` & `chainsaddiction-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/Makefile` & `chainsaddiction-0.2.4/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/PKG-INFO` & `chainsaddiction-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainsaddiction
-Version: 0.2.3
+Version: 0.2.4
 Summary: HMM with Poisson-distributed latent variables.
 Author-email: Michael Blaß <mblass@posteo.net>
 License: Copyright 2019 Michael Blaß michael.blass@uni-hamburg.de
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `chainsaddiction-0.2.3/README.md` & `chainsaddiction-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/docs/Makefile` & `chainsaddiction-0.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/docs/make.bat` & `chainsaddiction-0.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/docs/source/api/c/dataset.rst` & `chainsaddiction-0.2.4/docs/source/api/c/dataset.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/docs/source/api/c/poishmm/pois-hmm.rst` & `chainsaddiction-0.2.4/docs/source/api/c/poishmm/pois-hmm.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/docs/source/api/c/poishmm/pois-params.rst` & `chainsaddiction-0.2.4/docs/source/api/c/poishmm/pois-params.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/docs/source/api/c/poishmm/pois-probs.rst` & `chainsaddiction-0.2.4/docs/source/api/c/poishmm/pois-probs.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/docs/source/api/c/utils.rst` & `chainsaddiction-0.2.4/docs/source/api/c/utils.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/docs/source/api/python/poishmm.rst` & `chainsaddiction-0.2.4/docs/source/api/python/poishmm.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/docs/source/api/python/utils.rst` & `chainsaddiction-0.2.4/docs/source/api/python/utils.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/docs/source/conf.py` & `chainsaddiction-0.2.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/docs/source/getting-started.rst` & `chainsaddiction-0.2.4/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/docs/source/index.rst` & `chainsaddiction-0.2.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/docs/source/usrguide/examples.rst` & `chainsaddiction-0.2.4/docs/source/usrguide/examples.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/pyproject.toml` & `chainsaddiction-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "chainsaddiction"
-version = "0.2.3"
+version = "0.2.4"
 authors = [{name = "Michael Blaß", email = "mblass@posteo.net"}]
 description = "HMM with Poisson-distributed latent variables."
 keywords = ["hmm", "poisson", "hidden-markov model"]
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
 	"License :: OSI Approved :: BSD License",
```

### Comparing `chainsaddiction-0.2.3/setup.py` & `chainsaddiction-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/dataset.c` & `chainsaddiction-0.2.4/src/chainsaddiction/dataset.c`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     return this;
 }
 
 
 DataSet *
 DataSet_NewFromFile (const char *path)
 {
-    size_t n_elem = 0;
-    FILE   *file  = Ca_OpenFile (path, "r");
+    size_t  n_elem = 0;
+    FILE    *file  = Ca_OpenFile (path, "r");
     DataSet *this  = DataSet_NewEmpty ();
 
     Ca_CountLines (file, &n_elem);
     if (n_elem == 0)
     {
         fprintf (stderr, "Empty file: %s\n", path);
         DataSet_Delete (this);
```

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/dataset.h` & `chainsaddiction-0.2.4/src/chainsaddiction/dataset.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/libma.c` & `chainsaddiction-0.2.4/src/chainsaddiction/libma.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/libma.h` & `chainsaddiction-0.2.4/src/chainsaddiction/libma.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/Makefile` & `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-em.c` & `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-em.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-em.h` & `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-em.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-fwbw.c` & `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-fwbw.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-fwbw.h` & `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-fwbw.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-hmm.c` & `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-hmm.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-hmm.h` & `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-hmm.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-params.c` & `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-params.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-params.h` & `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-params.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-probs.c` & `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-probs.c`

 * *Files 0% similar despite different names*

```diff
@@ -28,13 +28,13 @@
     {
         fprintf (stderr, "Could not allocate memory for PoisProbs object.\n");
         return NULL;
     }
     probs->lsdp     = MA_SCALAR_ZEROS (n_elem);
     probs->lalpha   = MA_SCALAR_ZEROS (n_elem);
     probs->lbeta    = MA_SCALAR_ZEROS (n_elem);
-    probs->lcsp    = MA_SCALAR_ZEROS (n_elem);
+    probs->lcsp     = MA_SCALAR_ZEROS (n_elem);
     probs->n_obs    = n_obs;
     probs->m_states = m_states;
 
     return probs;
 }
```

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/pois-probs.h` & `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-probs.h`

 * *Files 0% similar despite different names*

```diff
@@ -15,25 +15,25 @@
  */
 typedef struct PoisProbs {
     size_t n_obs;
     size_t m_states;
     scalar *lsdp;       /**< Log of the state dependent probabilities   */
     scalar *lalpha;     /**< Log forward probabilities                  */
     scalar *lbeta;      /**< Log backward probabilities                 */
-    scalar *lcsp;      /**< Log conditional expectations               */
+    scalar *lcsp;       /**< Log conditional expectations               */
 } PoisProbs;
 
 
 #define PoisProbs_Delete(probs)     \
 if (probs)                          \
 {                                   \
     free (probs->lsdp);             \
     free (probs->lalpha);           \
     free (probs->lbeta);            \
-    free (probs->lcsp);            \
+    free (probs->lcsp);             \
     free (probs);                   \
     probs = NULL;                   \
 }
 
 
 PoisProbs *
 PoisProbs_New (
```

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/poishmm-module.c` & `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/poishmm-module.c`

 * *Files 4% similar despite different names*

```diff
@@ -20,26 +20,26 @@
     UNUSED (args);
     UNUSED (kwds);
 
     PyCh_PoisHmm *self = NULL;
     self = (PyCh_PoisHmm *) type->tp_alloc (type, 0);
     if (self != NULL)
     {
-        self->err = 1;
-        self->n_iter = 0;
-        self->llk = 0.0;
-        self->aic = 0.0;
-        self->bic = 0.0;
-        self->m_states = 0;
-        self->lambda = NULL;
-        self->delta = NULL;
-        self->gamma = NULL;
-        self->lalpha = NULL;
-        self->lbeta = NULL;
-        self->lcsp = NULL;
+        self->err       = 1;
+        self->n_iter    = 0;
+        self->llk       = 0.0;
+        self->aic       = 0.0;
+        self->bic       = 0.0;
+        self->m_states  = 0;
+        self->lambda    = NULL;
+        self->delta     = NULL;
+        self->gamma     = NULL;
+        self->lalpha    = NULL;
+        self->lbeta     = NULL;
+        self->lcsp      = NULL;
     }
     return (PyObject *) self;
 }
 
 
 static int
 PyCh_PoisHmm_CInit (PyCh_PoisHmm *self, const size_t n_obs, const size_t m_states)
@@ -49,15 +49,15 @@
     const npy_intp dims_data[]    = { (npy_intp) n_obs,    (npy_intp) m_states };
 
     self->lambda = PyArray_SimpleNew (PyCh_VECTOR, dims_vector, NPY_LONGDOUBLE);
     self->gamma  = PyArray_SimpleNew (PyCh_MATRIX, dims_matrix, NPY_LONGDOUBLE);
     self->delta  = PyArray_SimpleNew (PyCh_VECTOR, dims_vector, NPY_LONGDOUBLE);
     self->lalpha = PyArray_SimpleNew (PyCh_DATA,   dims_data,   NPY_LONGDOUBLE);
     self->lbeta  = PyArray_SimpleNew (PyCh_DATA,   dims_data,   NPY_LONGDOUBLE);
-    self->lcsp  = PyArray_SimpleNew (PyCh_DATA,   dims_data,   NPY_LONGDOUBLE);
+    self->lcsp   = PyArray_SimpleNew (PyCh_DATA,   dims_data,   NPY_LONGDOUBLE);
     return 0;
 }
 
 
 static void
 PyCh_PoisHmm_Set (PyCh_PoisHmm *out, PoisHmm *hmm)
 {
@@ -70,36 +70,35 @@
     long double *gamma_est  = hmm->params->gamma;
     long double *delta_est  = hmm->params->delta;
 
     PyObject *wrap_lalpha = PyArray_SimpleNewFromData (PyCh_DATA, dims_data,
                                 NPY_LONGDOUBLE, (void *) hmm->probs->lalpha);
     PyObject *wrap_lbeta  = PyArray_SimpleNewFromData (PyCh_DATA, dims_data,
                                 NPY_LONGDOUBLE, (void *) hmm->probs->lbeta);
-    PyObject *wrap_lcsp  = PyArray_SimpleNewFromData (PyCh_DATA, dims_data,
+    PyObject *wrap_lcsp   = PyArray_SimpleNewFromData (PyCh_DATA, dims_data,
                                 NPY_LONGDOUBLE, (void *) hmm->probs->lcsp);
 
-    out->err = 0;
+    out->err    = 0;
     out->n_iter = hmm->n_iter;
-    out->llk = (double) hmm->llh;
-    out->aic = (double) hmm->aic;
-    out->bic = (double) hmm->bic;
+    out->llk    = (double) hmm->llh;
+    out->aic    = (double) hmm->aic;
 
     for (size_t i = 0; i < hmm->m_states; i++)
     {
         *lambda_out++ = *lambda_est++;
         *delta_out++  = expl (*delta_est++);
         for (size_t j = 0; j < hmm->m_states; j++)
         {
             *gamma_out++ = expl (*gamma_est++);
         }
     }
 
     PyArray_CopyInto ((PyArrayObject *) out->lalpha, (PyArrayObject *) wrap_lalpha);
     PyArray_CopyInto ((PyArrayObject *) out->lbeta,  (PyArrayObject *) wrap_lbeta);
-    PyArray_CopyInto ((PyArrayObject *) out->lcsp,  (PyArrayObject *) wrap_lcsp);
+    PyArray_CopyInto ((PyArrayObject *) out->lcsp,   (PyArrayObject *) wrap_lcsp);
 }
 
 
 static PyObject *
 poishmm_fit (PyObject *self, PyObject *args)
 {
     UNUSED (self);
@@ -110,20 +109,20 @@
 
     PyArrayObject *arr_lambda = NULL;
     PyArrayObject *arr_gamma  = NULL;
     PyArrayObject *arr_delta  = NULL;
     PyArrayObject *arr_inp    = NULL;
 
 
-    DataSet inp = { NULL, 0, false };
-    PoisHmm hmm = { true, 0, 0, 0, 0, 0.0, 0.0, 0.0, 0.0, NULL, NULL, NULL };
-    PoisParams *init = NULL;
-    PoisParams *working = NULL;
-    PoisProbs *probs = NULL;
-    PyCh_PoisHmm *out = NULL;
+    DataSet      inp      = { NULL, 0, false };
+    PoisHmm      hmm      = { true, 0, 0, 0, 0, 0.0, 0.0, 0.0, 0.0, NULL, NULL, NULL };
+    PoisParams   *init    = NULL;
+    PoisParams   *working = NULL;
+    PoisProbs    *probs   = NULL;
+    PyCh_PoisHmm *out     = NULL;
 
     double tol_buffer = 0;
     if (!PyArg_ParseTuple (args, "llldOOOO",
                 &hmm.n_obs,
                 &hmm.m_states,
                 &hmm.max_iter,
                 &tol_buffer,
@@ -141,35 +140,35 @@
     if ((arr_lambda == NULL) || (arr_gamma == NULL) || (arr_delta == NULL) || (arr_inp == NULL))
     {
         const char msg[] = "poishmm.fit: Could not convert input arrays.";
         PyErr_SetString (PyExc_MemoryError, msg);
         goto fail;
     }
 
-    init = PoisParams_New (hmm.m_states);
+    init    = PoisParams_New (hmm.m_states);
     working = PoisParams_New (hmm.m_states);
-    probs = PoisProbs_New (hmm.n_obs, hmm.m_states);
+    probs   = PoisProbs_New  (hmm.n_obs, hmm.m_states);
 
     if ((init == NULL) || (working == NULL) || (probs == NULL))
     {
         const char msg[] = "poishmm.fit: Could not create PoisHmm members.";
         PyErr_SetString (PyExc_MemoryError, msg);
         goto fail;
     }
 
     PoisParams_SetLambda (init, PyArray_DATA (arr_lambda));
     PoisParams_SetGamma  (init, PyArray_DATA (arr_gamma));
     PoisParams_SetDelta  (init, PyArray_DATA (arr_delta));
     PoisParams_CopyLog   (init, working);
 
-    hmm.init = init;
+    hmm.init   = init;
     hmm.params = working;
-    hmm.probs = probs;
-    inp.size = PyArray_SIZE (arr_inp);
-    inp.data = PyArray_DATA (arr_inp);
+    hmm.probs  = probs;
+    inp.size   = PyArray_SIZE (arr_inp);
+    inp.data   = PyArray_DATA (arr_inp);
 
     PoisHmm_EstimateParams (&hmm, &inp);
     if (hmm.err)
     {
         PyErr_WarnEx (PyExc_Warning, "No convergence.", 1);
     }
 
@@ -199,24 +198,25 @@
 }
 
 
 static PyObject *
 poishmm_read_params (PyObject *self, PyObject *args)
 {
     UNUSED (self);
-    char *path = NULL;
-    PoisParams *params = NULL;
-    PyObject *arr_lambda = NULL;
-    PyObject *arr_delta  = NULL;
-    PyObject *arr_gamma  = NULL;
-    PyObject *out_lambda = NULL;
-    PyObject *out_delta  = NULL;
-    PyObject *out_gamma  = NULL;
-    PyObject *out_states = NULL;
-    PyObject *out = NULL;
+
+    char       *path       = NULL;
+    PoisParams *params     = NULL;
+    PyObject   *arr_lambda = NULL;
+    PyObject   *arr_delta  = NULL;
+    PyObject   *arr_gamma  = NULL;
+    PyObject   *out_lambda = NULL;
+    PyObject   *out_delta  = NULL;
+    PyObject   *out_gamma  = NULL;
+    PyObject   *out_states = NULL;
+    PyObject   *out        = NULL;
 
     if (!PyArg_ParseTuple (args, "s", &path))
     {
         PyErr_SetString (PyExc_TypeError, "read_params: Could not parse argument.");
         return NULL;
     }
```

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/poishmm-module.h` & `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/poishmm-module.h`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #include "structmember.h"
 
 #include "chainsaddiction.h"
 #include "poishmm/pois-hmm.h"
 #include "poishmm/pois-params.h"
 #include "poishmm/poishmm-object.h"
 
-
 #define poishmm_fit_doc                                                 \
     "Estimate HMM parameters given an observation time series by "      \
     "Expectation Maximization\n\n"                                      \
     "fit_em(n_obs: int, m_states: int, max_iter: int, tol: float, "     \
     "sdm: array-like, tpm: array-like, distr: array-like, "             \
     "data: array-like) -> Fit\n"
```

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/poishmm-object.h` & `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/poishmm-object.h`

 * *Files 16% similar despite different names*

```diff
@@ -32,34 +32,34 @@
 PyCh_PoisHmm_CInit (PyCh_PoisHmm *self, const size_t n_states, const size_t m_states);
 
 static void
 PyCh_PoisHmm_Set (PyCh_PoisHmm *out, PoisHmm *hmm);
 
 
 static PyMemberDef PyCh_PoisHmm_members[] = {
-    {"err", T_INT, offsetof (PyCh_PoisHmm, err), 0, "Error number"},
-    {"n_iter", T_ULONG, offsetof (PyCh_PoisHmm, n_iter), 0, "Number of iterations"},
-    {"llk", T_DOUBLE, offsetof (PyCh_PoisHmm, llk), 0, "Log likelihood"},
-    {"aic", T_DOUBLE, offsetof (PyCh_PoisHmm, aic), 0, "Akaike information criterion"},
-    {"bic", T_DOUBLE, offsetof (PyCh_PoisHmm, bic), 0, "Bayesian information criterion"},
-    {"m_states", T_ULONG, offsetof (PyCh_PoisHmm, m_states), 0, "Number of states"},
-    {"lambda_", T_OBJECT, offsetof (PyCh_PoisHmm, lambda), 0, "State-dependent means"},
-    {"gamma_", T_OBJECT, offsetof (PyCh_PoisHmm, gamma), 0, "Transition probability matrix"},
-    {"delta_", T_OBJECT, offsetof (PyCh_PoisHmm, delta), 0, "Initial distribution"},
-    {"lalpha", T_OBJECT, offsetof (PyCh_PoisHmm, lalpha), 0, "Forward probabilities"},
-    {"lbeta", T_OBJECT, offsetof (PyCh_PoisHmm, lbeta), 0, "Backward probabilities"},
-    {"lcsp", T_OBJECT, offsetof (PyCh_PoisHmm, lcsp), 0, "Log of the conditional expectations"},
+    {"err",         T_INT,      offsetof (PyCh_PoisHmm, err),       0, "Error number"},
+    {"n_iter",      T_ULONG,    offsetof (PyCh_PoisHmm, n_iter),    0, "Number of iterations"},
+    {"llk",         T_DOUBLE,   offsetof (PyCh_PoisHmm, llk),       0, "Log likelihood"},
+    {"aic",         T_DOUBLE,   offsetof (PyCh_PoisHmm, aic),       0, "Akaike information criterion"},
+    {"bic",         T_DOUBLE,   offsetof (PyCh_PoisHmm, bic),       0, "Bayesian information criterion"},
+    {"m_states",    T_ULONG,    offsetof (PyCh_PoisHmm, m_states),  0, "Number of states"},
+    {"lambda_",     T_OBJECT,   offsetof (PyCh_PoisHmm, lambda),    0, "State-dependent means"},
+    {"gamma_",      T_OBJECT,   offsetof (PyCh_PoisHmm, gamma),     0, "Transition probability matrix"},
+    {"delta_",      T_OBJECT,   offsetof (PyCh_PoisHmm, delta),     0, "Initial distribution"},
+    {"lalpha",      T_OBJECT,   offsetof (PyCh_PoisHmm, lalpha),    0, "Forward probabilities"},
+    {"lbeta",       T_OBJECT,   offsetof (PyCh_PoisHmm, lbeta),     0, "Backward probabilities"},
+    {"lcsp",        T_OBJECT,   offsetof (PyCh_PoisHmm, lcsp),      0, "Log of the conditional expectations"},
     {NULL, -1, 0, 0, NULL}  /* Sentinel */
 };
 
 
 static PyTypeObject PyCh_PoisHmm_Type = {
     PyVarObject_HEAD_INIT (NULL, 0)
     .tp_name = "poishmm.PoisHmm",
-    .tp_doc = "Hidden Markov Model with Poiss-distributet latent variables.",
+    .tp_doc = "Hidden Markov Model with Poisson-distributed latent variables.",
     .tp_basicsize = sizeof (PyCh_PoisHmm),
     .tp_itemsize = 0,
     .tp_flags = Py_TPFLAGS_DEFAULT,
     .tp_new = PyCh_PoisHmm_New,
     .tp_dealloc = (destructor) PyCh_PoisHmm_Delete,
     .tp_members = PyCh_PoisHmm_members,
 };
```

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/Makefile` & `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/runtest.c` & `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/runtest.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-em.c` & `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-em.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-hmm.c` & `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-hmm.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-hmm.h` & `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-hmm.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-params.c` & `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-params.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/poishmm/tests/test-pois-probs.c` & `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-probs.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/read.c` & `chainsaddiction-0.2.4/src/chainsaddiction/read.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/read.h` & `chainsaddiction-0.2.4/src/chainsaddiction/read.h`

 * *Files 14% similar despite different names*

```diff
@@ -27,30 +27,30 @@
  */
 extern FILE *
 Ca_OpenFile (const char *path, const char *mode);
 
 
 /** Close an open file stream.
   *
-  *\param[in]   file    Open file stream.
+  * \param[in]   file    Open file stream.
   *
-  *\return  0 on suceess, `EOF` on failure.
+  * \return  0 on suceess, `EOF` on failure.
 */
 extern int
 Ca_CloseFile (FILE *file);
 
 
 /** Read numerical data from file.
  *
  * Numbers have to be separated by newline.
  *
- *\param[in]   file    Open file stream.
- *\param[out]  target  Pointer to allocated memory.
+ * \param[in]   file    Open file stream.
+ * \param[out]  target  Pointer to allocated memory.
  *
- *\return  Number of read lines.
+ * \return  Number of read lines.
 */
 extern size_t
 Ca_ReadDataFile (FILE *stream, size_t n_lines, scalar *target);
 
 
 /** Count to number of lines in a file.
  *
```

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/tests/Makefile` & `chainsaddiction-0.2.4/src/chainsaddiction/tests/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/tests/runtest.c` & `chainsaddiction-0.2.4/src/chainsaddiction/tests/runtest.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/tests/test-dataset.c` & `chainsaddiction-0.2.4/src/chainsaddiction/tests/test-dataset.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/tests/test-dataset.h` & `chainsaddiction-0.2.4/src/chainsaddiction/tests/test-dataset.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/tests/test-read.c` & `chainsaddiction-0.2.4/src/chainsaddiction/tests/test-read.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/utils/tests/Makefile` & `chainsaddiction-0.2.4/src/chainsaddiction/utils/tests/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/utils/tests/test-utils.c` & `chainsaddiction-0.2.4/src/chainsaddiction/utils/tests/test-utils.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/utils/utils-module.c` & `chainsaddiction-0.2.4/src/chainsaddiction/utils/utils-module.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/utils/utils-module.h` & `chainsaddiction-0.2.4/src/chainsaddiction/utils/utils-module.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/utils/utils.c` & `chainsaddiction-0.2.4/src/chainsaddiction/utils/utils.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction/utils/utils.h` & `chainsaddiction-0.2.4/src/chainsaddiction/utils/utils.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction.egg-info/PKG-INFO` & `chainsaddiction-0.2.4/src/chainsaddiction.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainsaddiction
-Version: 0.2.3
+Version: 0.2.4
 Summary: HMM with Poisson-distributed latent variables.
 Author-email: Michael Blaß <mblass@posteo.net>
 License: Copyright 2019 Michael Blaß michael.blass@uni-hamburg.de
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `chainsaddiction-0.2.3/src/chainsaddiction.egg-info/SOURCES.txt` & `chainsaddiction-0.2.4/src/chainsaddiction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/vmath/Makefile` & `chainsaddiction-0.2.4/src/vmath/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/vmath/alloc.h` & `chainsaddiction-0.2.4/src/vmath/alloc.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/vmath/core.c` & `chainsaddiction-0.2.4/src/vmath/core.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/vmath/core.h` & `chainsaddiction-0.2.4/src/vmath/core.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/vmath/print.h` & `chainsaddiction-0.2.4/src/vmath/print.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/vmath/rnd.c` & `chainsaddiction-0.2.4/src/vmath/rnd.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/vmath/rnd.h` & `chainsaddiction-0.2.4/src/vmath/rnd.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/vmath/stats.c` & `chainsaddiction-0.2.4/src/vmath/stats.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/vmath/stats.h` & `chainsaddiction-0.2.4/src/vmath/stats.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/vmath/tests/Makefile` & `chainsaddiction-0.2.4/src/vmath/tests/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/vmath/tests/runtest.c` & `chainsaddiction-0.2.4/src/vmath/tests/runtest.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/vmath/tests/test_rnd.c` & `chainsaddiction-0.2.4/src/vmath/tests/test_rnd.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/vmath/tests/test_stats.c` & `chainsaddiction-0.2.4/src/vmath/tests/test_stats.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/vmath/tests/test_vmath.c` & `chainsaddiction-0.2.4/src/vmath/tests/test_vmath.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/vmath/tests/test_vmath.h` & `chainsaddiction-0.2.4/src/vmath/tests/test_vmath.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/vmath/vmath.c` & `chainsaddiction-0.2.4/src/vmath/vmath.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/src/vmath/vmath.h` & `chainsaddiction-0.2.4/src/vmath/vmath.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/S4_N100` & `chainsaddiction-0.2.4/tests/data/S4_N100`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/S4_N500` & `chainsaddiction-0.2.4/tests/data/S4_N500`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/S4_N50_MID` & `chainsaddiction-0.2.4/tests/data/S4_N50_MID`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/centroids/2s/lalpha.txt` & `chainsaddiction-0.2.4/tests/data/centroids/2s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/centroids/2s/lbeta.txt` & `chainsaddiction-0.2.4/tests/data/centroids/2s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/centroids/2s/lcsp.txt` & `chainsaddiction-0.2.4/tests/data/centroids/2s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/centroids/3s/lalpha.txt` & `chainsaddiction-0.2.4/tests/data/centroids/3s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/centroids/3s/lbeta.txt` & `chainsaddiction-0.2.4/tests/data/centroids/3s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/centroids/3s/lcsp.txt` & `chainsaddiction-0.2.4/tests/data/centroids/3s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/centroids/4s/lalpha.txt` & `chainsaddiction-0.2.4/tests/data/centroids/4s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/centroids/4s/lbeta.txt` & `chainsaddiction-0.2.4/tests/data/centroids/4s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/centroids/4s/lcsp.txt` & `chainsaddiction-0.2.4/tests/data/centroids/4s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/centroids/5s/gamma.txt` & `chainsaddiction-0.2.4/tests/data/centroids/5s/gamma.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/centroids/5s/global-decoding.txt` & `chainsaddiction-0.2.4/tests/data/centroids/5s/global-decoding.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/centroids/5s/lalpha.txt` & `chainsaddiction-0.2.4/tests/data/centroids/5s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/centroids/5s/lbeta.txt` & `chainsaddiction-0.2.4/tests/data/centroids/5s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/centroids/5s/lcsp.txt` & `chainsaddiction-0.2.4/tests/data/centroids/5s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/centroids/5s/local-decoding.txt` & `chainsaddiction-0.2.4/tests/data/centroids/5s/local-decoding.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/centroids/centroids` & `chainsaddiction-0.2.4/tests/data/centroids/centroids`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/earthquakes/2s/lalpha.txt` & `chainsaddiction-0.2.4/tests/data/earthquakes/2s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/earthquakes/2s/lbeta.txt` & `chainsaddiction-0.2.4/tests/data/earthquakes/2s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/earthquakes/2s/lcsp.txt` & `chainsaddiction-0.2.4/tests/data/earthquakes/2s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/earthquakes/3s/lalpha.txt` & `chainsaddiction-0.2.4/tests/data/earthquakes/3s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/earthquakes/3s/lbeta.txt` & `chainsaddiction-0.2.4/tests/data/earthquakes/3s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/earthquakes/3s/lcsp.txt` & `chainsaddiction-0.2.4/tests/data/earthquakes/3s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/earthquakes/4s/lalpha.txt` & `chainsaddiction-0.2.4/tests/data/earthquakes/4s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/earthquakes/4s/lbeta.txt` & `chainsaddiction-0.2.4/tests/data/earthquakes/4s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/earthquakes/4s/lcsp.txt` & `chainsaddiction-0.2.4/tests/data/earthquakes/4s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/earthquakes/5s/lalpha.txt` & `chainsaddiction-0.2.4/tests/data/earthquakes/5s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/earthquakes/5s/lbeta.txt` & `chainsaddiction-0.2.4/tests/data/earthquakes/5s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/earthquakes/5s/lcsp.txt` & `chainsaddiction-0.2.4/tests/data/earthquakes/5s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/data/earthquakes/5s/lgamma.txt` & `chainsaddiction-0.2.4/tests/data/earthquakes/5s/lgamma.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/test-ext-earthquakes.py` & `chainsaddiction-0.2.4/tests/test-ext-earthquakes.py`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/test-utils.py` & `chainsaddiction-0.2.4/tests/test-utils.py`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.3/tests/utils.py` & `chainsaddiction-0.2.4/tests/utils.py`

 * *Files identical despite different names*

