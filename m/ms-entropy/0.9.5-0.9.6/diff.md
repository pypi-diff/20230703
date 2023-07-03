# Comparing `tmp/ms_entropy-0.9.5.tar.gz` & `tmp/ms_entropy-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_entropy-0.9.5.tar", last modified: Thu Jun 29 01:08:29 2023, max compression
+gzip compressed data, was "ms_entropy-0.9.6.tar", last modified: Mon Jul  3 17:58:57 2023, max compression
```

## Comparing `ms_entropy-0.9.5.tar` & `ms_entropy-0.9.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:08:29.938910 ms_entropy-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-06-29 01:08:29.938910 ms_entropy-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:08:29.922910 ms_entropy-0.9.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:08:29.926910 ms_entropy-0.9.5/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:08:29.926910 ms_entropy-0.9.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/examples/example-2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/examples/example-multiple_cores.py
--rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/examples/example-search_mona-with_pickle_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/examples/example-search_mona-with_read_write_functions-low_memory_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/examples/example-search_mona-with_read_write_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/examples/example-with_individual_search_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/examples/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:08:29.930910 ms_entropy-0.9.5/ms_entropy/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:08:29.938910 ms_entropy-0.9.5/ms_entropy/entropy_search/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/entropy_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/entropy_search/fast_flash_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)   881493 2023-06-29 01:08:29.000000 ms_entropy-0.9.5/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.c
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    20155 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/entropy_search/flash_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    29246 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/entropy_search/flash_entropy_search_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    17592 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:08:29.934910 ms_entropy-0.9.5/ms_entropy/file_io/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/file_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/file_io/lbm2_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/file_io/mgf_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/file_io/msp_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/file_io/mzml_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/file_io/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/file_io/spec_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:08:29.934910 ms_entropy-0.9.5/ms_entropy/pipe/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/pipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/pipe/df.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/pipe/entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/pipe/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/pipe/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/pipe/pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:08:29.938910 ms_entropy-0.9.5/ms_entropy/spectra/
--rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/spectra/CleanSpectrum.c
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/spectra/CleanSpectrum.h
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/spectra/SpectralEntropy.c
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/spectra/SpectralEntropy.h
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/spectra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/spectra/entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)   344231 2023-06-29 01:08:29.000000 ms_entropy-0.9.5/ms_entropy/spectra/entropy_cython.c
--rw-r--r--   0 runner    (1001) docker     (123)    11171 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/spectra/entropy_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    11241 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/spectra/entropy_numba.py
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/spectra/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/ms_entropy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:08:29.938910 ms_entropy-0.9.5/ms_entropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-06-29 01:08:29.000000 ms_entropy-0.9.5/ms_entropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-29 01:08:29.000000 ms_entropy-0.9.5/ms_entropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 01:08:29.000000 ms_entropy-0.9.5/ms_entropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-29 01:08:29.000000 ms_entropy-0.9.5/ms_entropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-29 01:08:29.000000 ms_entropy-0.9.5/ms_entropy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-29 01:08:29.938910 ms_entropy-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:08:29.934910 ms_entropy-0.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/tests/test_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-06-29 01:08:19.000000 ms_entropy-0.9.5/tests/test_entropy_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:58:57.494240 ms_entropy-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19465 2023-07-03 17:58:57.494240 ms_entropy-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:58:57.478240 ms_entropy-0.9.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:58:57.482240 ms_entropy-0.9.6/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:58:57.482240 ms_entropy-0.9.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/examples/example-2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/examples/example-multiple_cores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/examples/example-search_mona-with_pickle_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/examples/example-search_mona-with_read_write_functions-low_memory_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/examples/example-search_mona-with_read_write_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/examples/example-with_individual_search_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/examples/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:58:57.486240 ms_entropy-0.9.6/ms_entropy/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:58:57.494240 ms_entropy-0.9.6/ms_entropy/entropy_search/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/entropy_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/entropy_search/fast_flash_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)   881493 2023-07-03 17:58:56.000000 ms_entropy-0.9.6/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    20155 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/entropy_search/flash_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29246 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/entropy_search/flash_entropy_search_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17592 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:58:57.486240 ms_entropy-0.9.6/ms_entropy/file_io/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/file_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/file_io/lbm2_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/file_io/mgf_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/file_io/msp_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/file_io/mzml_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/file_io/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/file_io/spec_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:58:57.490240 ms_entropy-0.9.6/ms_entropy/pipe/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/pipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/pipe/df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/pipe/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/pipe/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/pipe/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/pipe/pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:58:57.494240 ms_entropy-0.9.6/ms_entropy/spectra/
+-rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/spectra/CleanSpectrum.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/spectra/CleanSpectrum.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/spectra/SpectralEntropy.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/spectra/SpectralEntropy.h
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/spectra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/spectra/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)   344231 2023-07-03 17:58:56.000000 ms_entropy-0.9.6/ms_entropy/spectra/entropy_cython.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11171 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/spectra/entropy_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    11241 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/spectra/entropy_numba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/spectra/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:58:57.490240 ms_entropy-0.9.6/ms_entropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19465 2023-07-03 17:58:57.000000 ms_entropy-0.9.6/ms_entropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-03 17:58:57.000000 ms_entropy-0.9.6/ms_entropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 17:58:57.000000 ms_entropy-0.9.6/ms_entropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-03 17:58:57.000000 ms_entropy-0.9.6/ms_entropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 17:58:57.000000 ms_entropy-0.9.6/ms_entropy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-03 17:58:57.494240 ms_entropy-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:58:57.490240 ms_entropy-0.9.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/tests/test_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/tests/test_entropy_search.py
```

### Comparing `ms_entropy-0.9.5/LICENSE` & `ms_entropy-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/PKG-INFO` & `ms_entropy-0.9.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms_entropy
-Version: 0.9.5
+Version: 0.9.6
 Summary: This package provides a Python implementation of calculating spectral entropy, entropy similarity, and Flash entropy search for mass spectrometry data.
 Author-email: Yuanyue Li <liyuanyue@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -219,18 +219,18 @@
 
 [![DOI](https://zenodo.org/badge/232434019.svg)](https://zenodo.org/badge/latestdoi/232434019)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7972082.svg)](https://doi.org/10.5281/zenodo.7972082)
 [![Test MS Entropy package](https://github.com/YuanyueLi/MSEntropy/actions/workflows/run_test.yml/badge.svg?branch=main)](https://github.com/YuanyueLi/MSEntropy/actions/workflows/run_test.yml)
 
 If you find this package useful, please consider citing the following papers:
 
-Li, Y., Fiehn, O., Flash entropy search to query all mass spectral
+> Li, Y., Fiehn, O., Flash entropy search to query all mass spectral
 libraries in real time. 04 April 2023, PREPRINT (Version 1) available at Research Square. [https://doi.org/10.21203/rs.3.rs-2693233/v1](https://doi.org/10.21203/rs.3.rs-2693233/v1)
-
-Li, Y., Kind, T., Folz, J. _et al._ Spectral entropy outperforms MS/MS dot product similarity for small-molecule compound identification. _Nat Methods_ **18**, 1524–1531 (2021). [https://doi.org/10.1038/s41592-021-01331-z](https://doi.org/10.1038/s41592-021-01331-z)
+>
+> Li, Y., Kind, T., Folz, J. _et al._ Spectral entropy outperforms MS/MS dot product similarity for small-molecule compound identification. _Nat Methods_ **18**, 1524–1531 (2021). [https://doi.org/10.1038/s41592-021-01331-z](https://doi.org/10.1038/s41592-021-01331-z)
 
 # Theoritical Background
 
 `Spectral entropy` is an useful property to measure the complexity of a spectrum. It is inspried by the concept of Shannon entropy in information theory. [(ref)](https://doi.org/10.1038/s41592-021-01331-z)
 
 `Entropy similarity`, which measured spectral similarity based on spectral entropy, has been shown to outperform dot product similarity in compound identification. [(ref)](https://doi.org/10.1038/s41592-021-01331-z)
 
@@ -258,14 +258,16 @@
 entropy_search.build_index(spectral_library)
 entropy_similarity = entropy_search.search(
     precursor_mz=query_spectrum_precursor_mz, peaks=query_spectrum_peaks)
 ```
 
 ## For R users
 
+A document is available here: [https://cran.r-project.org/web/packages/msentropy/msentropy.pdf](https://cran.r-project.org/web/packages/msentropy/msentropy.pdf)
+
 ### Installation
 
 ```R
 install.packages("msentropy")
 ```
 
 ### Usage
@@ -335,7 +337,15 @@
     int max_peak_num = -1;
 
     // Calculate entropy similarity, the data in spec_a and spec_b will modified.
     float similarity = calculate_entropy_similarity(*spec_a, spec_a_len, *spec_b, spec_b_len, ms2_tolerance_in_da, ms2_tolerance_in_ppm, clean_spectra, min_mz, max_mz, noise_threshold, max_peak_num);
     printf("Entropy Similarity: %f\n", similarity);
 }
 ```
+
+An example is available in folder [languages/c folder](https://github.com/YuanyueLi/MSEntropy/tree/main/languages/c) and [Example.c](https://github.com/YuanyueLi/MSEntropy/blob/main/languages/c/Example.c), [CMakeLists.txt](https://github.com/YuanyueLi/MSEntropy/blob/main/languages/c/CMakeLists.txt)
+
+## For JavaScript users
+
+An example is available in folder [languages/javascript folder](https://github.com/YuanyueLi/MSEntropy/tree/main/languages/javascript) and [example.js](https://github.com/YuanyueLi/MSEntropy/blob/main/languages/javascript/example.js)
+
+Also, refer to [MSViewer repository](https://github.com/YuanyueLi/MSViewer) for a working example of using this package in a web application.
```

### Comparing `ms_entropy-0.9.5/README.md` & `ms_entropy-0.9.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [![DOI](https://zenodo.org/badge/232434019.svg)](https://zenodo.org/badge/latestdoi/232434019)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7972082.svg)](https://doi.org/10.5281/zenodo.7972082)
 [![Test MS Entropy package](https://github.com/YuanyueLi/MSEntropy/actions/workflows/run_test.yml/badge.svg?branch=main)](https://github.com/YuanyueLi/MSEntropy/actions/workflows/run_test.yml)
 
 If you find this package useful, please consider citing the following papers:
 
-Li, Y., Fiehn, O., Flash entropy search to query all mass spectral
+> Li, Y., Fiehn, O., Flash entropy search to query all mass spectral
 libraries in real time. 04 April 2023, PREPRINT (Version 1) available at Research Square. [https://doi.org/10.21203/rs.3.rs-2693233/v1](https://doi.org/10.21203/rs.3.rs-2693233/v1)
-
-Li, Y., Kind, T., Folz, J. _et al._ Spectral entropy outperforms MS/MS dot product similarity for small-molecule compound identification. _Nat Methods_ **18**, 1524–1531 (2021). [https://doi.org/10.1038/s41592-021-01331-z](https://doi.org/10.1038/s41592-021-01331-z)
+>
+> Li, Y., Kind, T., Folz, J. _et al._ Spectral entropy outperforms MS/MS dot product similarity for small-molecule compound identification. _Nat Methods_ **18**, 1524–1531 (2021). [https://doi.org/10.1038/s41592-021-01331-z](https://doi.org/10.1038/s41592-021-01331-z)
 
 # Theoritical Background
 
 `Spectral entropy` is an useful property to measure the complexity of a spectrum. It is inspried by the concept of Shannon entropy in information theory. [(ref)](https://doi.org/10.1038/s41592-021-01331-z)
 
 `Entropy similarity`, which measured spectral similarity based on spectral entropy, has been shown to outperform dot product similarity in compound identification. [(ref)](https://doi.org/10.1038/s41592-021-01331-z)
 
@@ -39,14 +39,16 @@
 entropy_search.build_index(spectral_library)
 entropy_similarity = entropy_search.search(
     precursor_mz=query_spectrum_precursor_mz, peaks=query_spectrum_peaks)
 ```
 
 ## For R users
 
+A document is available here: [https://cran.r-project.org/web/packages/msentropy/msentropy.pdf](https://cran.r-project.org/web/packages/msentropy/msentropy.pdf)
+
 ### Installation
 
 ```R
 install.packages("msentropy")
 ```
 
 ### Usage
@@ -116,7 +118,15 @@
     int max_peak_num = -1;
 
     // Calculate entropy similarity, the data in spec_a and spec_b will modified.
     float similarity = calculate_entropy_similarity(*spec_a, spec_a_len, *spec_b, spec_b_len, ms2_tolerance_in_da, ms2_tolerance_in_ppm, clean_spectra, min_mz, max_mz, noise_threshold, max_peak_num);
     printf("Entropy Similarity: %f\n", similarity);
 }
 ```
+
+An example is available in folder [languages/c folder](https://github.com/YuanyueLi/MSEntropy/tree/main/languages/c) and [Example.c](https://github.com/YuanyueLi/MSEntropy/blob/main/languages/c/Example.c), [CMakeLists.txt](https://github.com/YuanyueLi/MSEntropy/blob/main/languages/c/CMakeLists.txt)
+
+## For JavaScript users
+
+An example is available in folder [languages/javascript folder](https://github.com/YuanyueLi/MSEntropy/tree/main/languages/javascript) and [example.js](https://github.com/YuanyueLi/MSEntropy/blob/main/languages/javascript/example.js)
+
+Also, refer to [MSViewer repository](https://github.com/YuanyueLi/MSViewer) for a working example of using this package in a web application.
```

### Comparing `ms_entropy-0.9.5/docs/source/conf.py` & `ms_entropy-0.9.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/examples/example-2.py` & `ms_entropy-0.9.6/examples/example-2.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/examples/example-multiple_cores.py` & `ms_entropy-0.9.6/examples/example-multiple_cores.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/examples/example-search_mona-with_pickle_functions.py` & `ms_entropy-0.9.6/examples/example-search_mona-with_pickle_functions.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/examples/example-search_mona-with_read_write_functions-low_memory_usage.py` & `ms_entropy-0.9.6/examples/example-search_mona-with_read_write_functions-low_memory_usage.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/examples/example-search_mona-with_read_write_functions.py` & `ms_entropy-0.9.6/examples/example-search_mona-with_read_write_functions.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/examples/example-with_individual_search_function.py` & `ms_entropy-0.9.6/examples/example-with_individual_search_function.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/examples/example.py` & `ms_entropy-0.9.6/examples/example.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/entropy_search/fast_flash_entropy_search.py` & `ms_entropy-0.9.6/ms_entropy/entropy_search/fast_flash_entropy_search.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.c` & `ms_entropy-0.9.6/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.pyx` & `ms_entropy-0.9.6/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/entropy_search/flash_entropy_search.py` & `ms_entropy-0.9.6/ms_entropy/entropy_search/flash_entropy_search.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/entropy_search/flash_entropy_search_core.py` & `ms_entropy-0.9.6/ms_entropy/entropy_search/flash_entropy_search_core.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py` & `ms_entropy-0.9.6/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/file_io/lbm2_file.py` & `ms_entropy-0.9.6/ms_entropy/file_io/lbm2_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/file_io/mgf_file.py` & `ms_entropy-0.9.6/ms_entropy/file_io/mgf_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/file_io/msp_file.py` & `ms_entropy-0.9.6/ms_entropy/file_io/msp_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/file_io/mzml_file.py` & `ms_entropy-0.9.6/ms_entropy/file_io/mzml_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/file_io/shared.py` & `ms_entropy-0.9.6/ms_entropy/file_io/shared.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/file_io/spec_file.py` & `ms_entropy-0.9.6/ms_entropy/file_io/spec_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/pipe/entropy.py` & `ms_entropy-0.9.6/ms_entropy/pipe/entropy.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/pipe/functions.py` & `ms_entropy-0.9.6/ms_entropy/pipe/functions.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/pipe/pipe.py` & `ms_entropy-0.9.6/ms_entropy/pipe/pipe.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/spectra/CleanSpectrum.c` & `ms_entropy-0.9.6/ms_entropy/spectra/CleanSpectrum.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/spectra/CleanSpectrum.h` & `ms_entropy-0.9.6/ms_entropy/spectra/CleanSpectrum.h`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/spectra/SpectralEntropy.c` & `ms_entropy-0.9.6/ms_entropy/spectra/SpectralEntropy.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/spectra/SpectralEntropy.h` & `ms_entropy-0.9.6/ms_entropy/spectra/SpectralEntropy.h`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/spectra/entropy.py` & `ms_entropy-0.9.6/ms_entropy/spectra/entropy.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/spectra/entropy_cython.c` & `ms_entropy-0.9.6/ms_entropy/spectra/entropy_cython.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/spectra/entropy_cython.pyx` & `ms_entropy-0.9.6/ms_entropy/spectra/entropy_cython.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/spectra/entropy_numba.py` & `ms_entropy-0.9.6/ms_entropy/spectra/entropy_numba.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy/spectra/tools.py` & `ms_entropy-0.9.6/ms_entropy/spectra/tools.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/ms_entropy.egg-info/PKG-INFO` & `ms_entropy-0.9.6/ms_entropy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-entropy
-Version: 0.9.5
+Version: 0.9.6
 Summary: This package provides a Python implementation of calculating spectral entropy, entropy similarity, and Flash entropy search for mass spectrometry data.
 Author-email: Yuanyue Li <liyuanyue@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -219,18 +219,18 @@
 
 [![DOI](https://zenodo.org/badge/232434019.svg)](https://zenodo.org/badge/latestdoi/232434019)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7972082.svg)](https://doi.org/10.5281/zenodo.7972082)
 [![Test MS Entropy package](https://github.com/YuanyueLi/MSEntropy/actions/workflows/run_test.yml/badge.svg?branch=main)](https://github.com/YuanyueLi/MSEntropy/actions/workflows/run_test.yml)
 
 If you find this package useful, please consider citing the following papers:
 
-Li, Y., Fiehn, O., Flash entropy search to query all mass spectral
+> Li, Y., Fiehn, O., Flash entropy search to query all mass spectral
 libraries in real time. 04 April 2023, PREPRINT (Version 1) available at Research Square. [https://doi.org/10.21203/rs.3.rs-2693233/v1](https://doi.org/10.21203/rs.3.rs-2693233/v1)
-
-Li, Y., Kind, T., Folz, J. _et al._ Spectral entropy outperforms MS/MS dot product similarity for small-molecule compound identification. _Nat Methods_ **18**, 1524–1531 (2021). [https://doi.org/10.1038/s41592-021-01331-z](https://doi.org/10.1038/s41592-021-01331-z)
+>
+> Li, Y., Kind, T., Folz, J. _et al._ Spectral entropy outperforms MS/MS dot product similarity for small-molecule compound identification. _Nat Methods_ **18**, 1524–1531 (2021). [https://doi.org/10.1038/s41592-021-01331-z](https://doi.org/10.1038/s41592-021-01331-z)
 
 # Theoritical Background
 
 `Spectral entropy` is an useful property to measure the complexity of a spectrum. It is inspried by the concept of Shannon entropy in information theory. [(ref)](https://doi.org/10.1038/s41592-021-01331-z)
 
 `Entropy similarity`, which measured spectral similarity based on spectral entropy, has been shown to outperform dot product similarity in compound identification. [(ref)](https://doi.org/10.1038/s41592-021-01331-z)
 
@@ -258,14 +258,16 @@
 entropy_search.build_index(spectral_library)
 entropy_similarity = entropy_search.search(
     precursor_mz=query_spectrum_precursor_mz, peaks=query_spectrum_peaks)
 ```
 
 ## For R users
 
+A document is available here: [https://cran.r-project.org/web/packages/msentropy/msentropy.pdf](https://cran.r-project.org/web/packages/msentropy/msentropy.pdf)
+
 ### Installation
 
 ```R
 install.packages("msentropy")
 ```
 
 ### Usage
@@ -335,7 +337,15 @@
     int max_peak_num = -1;
 
     // Calculate entropy similarity, the data in spec_a and spec_b will modified.
     float similarity = calculate_entropy_similarity(*spec_a, spec_a_len, *spec_b, spec_b_len, ms2_tolerance_in_da, ms2_tolerance_in_ppm, clean_spectra, min_mz, max_mz, noise_threshold, max_peak_num);
     printf("Entropy Similarity: %f\n", similarity);
 }
 ```
+
+An example is available in folder [languages/c folder](https://github.com/YuanyueLi/MSEntropy/tree/main/languages/c) and [Example.c](https://github.com/YuanyueLi/MSEntropy/blob/main/languages/c/Example.c), [CMakeLists.txt](https://github.com/YuanyueLi/MSEntropy/blob/main/languages/c/CMakeLists.txt)
+
+## For JavaScript users
+
+An example is available in folder [languages/javascript folder](https://github.com/YuanyueLi/MSEntropy/tree/main/languages/javascript) and [example.js](https://github.com/YuanyueLi/MSEntropy/blob/main/languages/javascript/example.js)
+
+Also, refer to [MSViewer repository](https://github.com/YuanyueLi/MSViewer) for a working example of using this package in a web application.
```

### Comparing `ms_entropy-0.9.5/ms_entropy.egg-info/SOURCES.txt` & `ms_entropy-0.9.6/ms_entropy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/pyproject.toml` & `ms_entropy-0.9.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/setup.py` & `ms_entropy-0.9.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy as np
 import os
 
 
 os.environ["CFLAGS"] = "-O3 -Wno-cpp -Wno-unused-function"
 
 setup(
+    name="ms_entropy",
     package_dir={"": "."},
     ext_modules=cythonize(
         [
             Extension(
                 "ms_entropy.spectra.entropy_cython",
                 [r"ms_entropy/spectra/entropy_cython.pyx", r"ms_entropy/spectra/CleanSpectrum.c", r"ms_entropy/spectra/SpectralEntropy.c"],
             ),
```

### Comparing `ms_entropy-0.9.5/tests/test_entropy.py` & `ms_entropy-0.9.6/tests/test_entropy.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.5/tests/test_entropy_search.py` & `ms_entropy-0.9.6/tests/test_entropy_search.py`

 * *Files identical despite different names*

