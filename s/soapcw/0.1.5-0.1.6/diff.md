# Comparing `tmp/soapcw-0.1.5.tar.gz` & `tmp/soapcw-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soapcw-0.1.5.tar", last modified: Tue Jun 13 08:56:05 2023, max compression
+gzip compressed data, was "soapcw-0.1.6.tar", last modified: Mon Jul  3 20:08:27 2023, max compression
```

## Comparing `soapcw-0.1.5.tar` & `soapcw-0.1.6.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:56:05.439011 soapcw-0.1.5/
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-06-13 08:53:32.000000 soapcw-0.1.5/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)     3508 2023-06-13 08:53:32.000000 soapcw-0.1.5/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-06-13 08:53:32.000000 soapcw-0.1.5/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-13 08:53:32.000000 soapcw-0.1.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-13 08:53:32.000000 soapcw-0.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2394 2023-06-13 08:56:05.439011 soapcw-0.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1389 2023-06-13 08:53:32.000000 soapcw-0.1.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:56:05.429011 soapcw-0.1.5/docs/
--rw-rw-rw-   0 root         (0) root         (0)      605 2023-06-13 08:53:32.000000 soapcw-0.1.5/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-06-13 08:53:32.000000 soapcw-0.1.5/docs/authors.rst
--rwxrwxrwx   0 root         (0) root         (0)     4930 2023-06-13 08:53:32.000000 soapcw-0.1.5/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-13 08:53:32.000000 soapcw-0.1.5/docs/contributing.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-06-13 08:53:32.000000 soapcw-0.1.5/docs/history.rst
--rw-rw-rw-   0 root         (0) root         (0)     1193 2023-06-13 08:53:32.000000 soapcw-0.1.5/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-06-13 08:53:32.000000 soapcw-0.1.5/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      766 2023-06-13 08:53:32.000000 soapcw-0.1.5/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:56:05.429011 soapcw-0.1.5/docs/pipeline_usage/
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-06-13 08:53:32.000000 soapcw-0.1.5/docs/pipeline_usage/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4690 2023-06-13 08:53:32.000000 soapcw-0.1.5/docs/pipeline_usage/run_pipeline.rst
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-13 08:53:32.000000 soapcw-0.1.5/docs/readme.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:56:05.430011 soapcw-0.1.5/docs/usage/
--rw-rw-rw-   0 root         (0) root         (0)      280 2023-06-13 08:53:32.000000 soapcw-0.1.5/docs/usage/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:56:05.431011 soapcw-0.1.5/pipeline/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 08:53:32.000000 soapcw-0.1.5/pipeline/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:56:05.431011 soapcw-0.1.5/pipeline/css/
--rw-rw-rw-   0 root         (0) root         (0)     3022 2023-06-13 08:53:32.000000 soapcw-0.1.5/pipeline/css/general.css
--rwxrwxrwx   0 root         (0) root         (0)     6999 2023-06-13 08:53:32.000000 soapcw-0.1.5/pipeline/make_dag_files_astro.py
--rwxrwxrwx   0 root         (0) root         (0)     6963 2023-06-13 08:53:32.000000 soapcw-0.1.5/pipeline/make_dag_files_lines.py
--rw-rw-rw-   0 root         (0) root         (0)    38221 2023-06-13 08:53:32.000000 soapcw-0.1.5/pipeline/make_html_page.py
--rwxrwxrwx   0 root         (0) root         (0)    36446 2023-06-13 08:53:32.000000 soapcw-0.1.5/pipeline/run_full_soap_astro.py
--rwxrwxrwx   0 root         (0) root         (0)    39626 2023-06-13 08:53:32.000000 soapcw-0.1.5/pipeline/run_full_soap_lines.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:56:05.431011 soapcw-0.1.5/pipeline/scripts/
--rw-rw-rw-   0 root         (0) root         (0)    16899 2023-06-13 08:53:32.000000 soapcw-0.1.5/pipeline/scripts/table_scripts.js
--rw-rw-rw-   0 root         (0) root         (0)     2156 2023-06-13 08:53:32.000000 soapcw-0.1.5/pipeline/soap_config_parser.py
--rw-rw-rw-   0 root         (0) root         (0)      984 2023-06-13 08:56:05.440011 soapcw-0.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4183 2023-06-13 08:53:32.000000 soapcw-0.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:56:05.434011 soapcw-0.1.5/soapcw/
--rw-rw-rw-   0 root         (0) root         (0)      556 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      406 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:56:05.436011 soapcw-0.1.5/soapcw/cnn/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/cnn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4682 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/cnn/cnn_data_dag_gen.py
--rwxrwxrwx   0 root         (0) root         (0)    17315 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/cnn/cnn_data_gen.py
--rw-rw-rw-   0 root         (0) root         (0)    13220 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/cnn/generate_gaussian_train_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11006 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/cnn/generate_test_data.py
--rw-rw-rw-   0 root         (0) root         (0)    17031 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/cnn/generate_train_data.py
--rwxrwxrwx   0 root         (0) root         (0)     5822 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/cnn/narrowband_sfts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:56:05.436011 soapcw-0.1.5/soapcw/cnn/pytorch/
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/cnn/pytorch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3019 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/cnn/pytorch/load_models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:56:05.437011 soapcw-0.1.5/soapcw/cnn/pytorch/models/
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/cnn/pytorch/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6338 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/cnn/pytorch/models/cnn.py
--rw-rw-rw-   0 root         (0) root         (0)     9628 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/cnn/pytorch/models/combined_cnn.py
--rw-rw-rw-   0 root         (0) root         (0)     7893 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/cnn/train_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:56:05.437011 soapcw-0.1.5/soapcw/cw/
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/cw/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    42241 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/cw/generate_data.py
--rw-rw-rw-   0 root         (0) root         (0)    19576 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/cw/load_sfts.py
--rw-rw-rw-   0 root         (0) root         (0)     8660 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/cw/make_sfts.py
--rw-rw-rw-   0 root         (0) root         (0)     9450 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/cw/sft.py
--rw-rw-rw-   0 root         (0) root         (0)     8567 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/cw/timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)     1687 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/cw/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:56:05.438011 soapcw-0.1.5/soapcw/line_aware_stat/
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/line_aware_stat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11721 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/line_aware_stat/gen_lookup.pyx
--rw-rw-rw-   0 root         (0) root         (0)    38004 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/line_aware_stat/gen_lookup_python.py
--rwxrwxrwx   0 root         (0) root         (0)     6514 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/line_aware_stat/save_lookup.py
--rw-rw-rw-   0 root         (0) root         (0)     3354 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/soap_config_parser.py
--rw-r--r--   0 root         (0) root         (0)  2250446 2023-06-13 08:56:04.000000 soapcw-0.1.5/soapcw/soapcw.c
--rw-rw-rw-   0 root         (0) root         (0)    63288 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/soapcw.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:56:05.438011 soapcw-0.1.5/soapcw/tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2885 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/tools/plots.py
--rw-rw-rw-   0 root         (0) root         (0)     9044 2023-06-13 08:53:32.000000 soapcw-0.1.5/soapcw/tools/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:56:05.435011 soapcw-0.1.5/soapcw.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2394 2023-06-13 08:56:05.000000 soapcw-0.1.5/soapcw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1822 2023-06-13 08:56:05.000000 soapcw-0.1.5/soapcw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 08:56:05.000000 soapcw-0.1.5/soapcw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      484 2023-06-13 08:56:05.000000 soapcw-0.1.5/soapcw.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 08:56:05.000000 soapcw-0.1.5/soapcw.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       45 2023-06-13 08:56:05.000000 soapcw-0.1.5/soapcw.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:56:05.000000 soapcw-0.1.5/soapcw.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:56:05.439011 soapcw-0.1.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)   445283 2023-06-13 08:53:32.000000 soapcw-0.1.5/tests/SNR_injections.ipynb
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-06-13 08:53:32.000000 soapcw-0.1.5/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1130 2023-06-13 08:53:32.000000 soapcw-0.1.5/tests/test_cwload.py
--rw-rw-rw-   0 root         (0) root         (0)     3602 2023-06-13 08:53:32.000000 soapcw-0.1.5/tests/test_line_aware_stat.py
--rw-rw-rw-   0 root         (0) root         (0)     4290 2023-06-13 08:53:32.000000 soapcw-0.1.5/tests/test_soap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.890154 soapcw-0.1.6/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-03 20:06:51.000000 soapcw-0.1.6/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3508 2023-07-03 20:06:51.000000 soapcw-0.1.6/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-07-03 20:06:51.000000 soapcw-0.1.6/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-03 20:06:51.000000 soapcw-0.1.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-07-03 20:06:51.000000 soapcw-0.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-07-03 20:08:27.890154 soapcw-0.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1389 2023-07-03 20:06:51.000000 soapcw-0.1.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.882154 soapcw-0.1.6/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      605 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/authors.rst
+-rwxrwxrwx   0 root         (0) root         (0)     4930 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/contributing.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/history.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      766 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.882154 soapcw-0.1.6/docs/pipeline_usage/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/pipeline_usage/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6317 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/pipeline_usage/run_pipeline.rst
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/readme.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.882154 soapcw-0.1.6/docs/usage/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/usage/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.883154 soapcw-0.1.6/pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 20:06:52.000000 soapcw-0.1.6/pipeline/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.883154 soapcw-0.1.6/pipeline/css/
+-rw-rw-rw-   0 root         (0) root         (0)     3163 2023-07-03 20:06:51.000000 soapcw-0.1.6/pipeline/css/general.css
+-rwxrwxrwx   0 root         (0) root         (0)     7001 2023-07-03 20:06:51.000000 soapcw-0.1.6/pipeline/make_dag_files_astro.py
+-rwxrwxrwx   0 root         (0) root         (0)     6963 2023-07-03 20:06:51.000000 soapcw-0.1.6/pipeline/make_dag_files_lines.py
+-rw-rw-rw-   0 root         (0) root         (0)    38283 2023-07-03 20:06:51.000000 soapcw-0.1.6/pipeline/make_html_page.py
+-rwxrwxrwx   0 root         (0) root         (0)    37055 2023-07-03 20:06:51.000000 soapcw-0.1.6/pipeline/run_full_soap_astro.py
+-rwxrwxrwx   0 root         (0) root         (0)    40172 2023-07-03 20:06:51.000000 soapcw-0.1.6/pipeline/run_full_soap_lines.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.883154 soapcw-0.1.6/pipeline/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)    18806 2023-07-03 20:06:51.000000 soapcw-0.1.6/pipeline/scripts/table_scripts.js
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2023-07-03 20:06:51.000000 soapcw-0.1.6/pipeline/soap_config_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      984 2023-07-03 20:08:27.890154 soapcw-0.1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4209 2023-07-03 20:06:51.000000 soapcw-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.886154 soapcw-0.1.6/soapcw/
+-rw-rw-rw-   0 root         (0) root         (0)      589 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.887154 soapcw-0.1.6/soapcw/cnn/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4682 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/cnn_data_dag_gen.py
+-rwxrwxrwx   0 root         (0) root         (0)    17946 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/cnn_data_gen.py
+-rw-rw-rw-   0 root         (0) root         (0)    12490 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/generate_gaussian_train_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11006 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/generate_test_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    20005 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/generate_train_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     5822 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/narrowband_sfts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.887154 soapcw-0.1.6/soapcw/cnn/pytorch/
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/pytorch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3019 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/pytorch/load_models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.888154 soapcw-0.1.6/soapcw/cnn/pytorch/models/
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/pytorch/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6685 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/pytorch/models/cnn.py
+-rw-rw-rw-   0 root         (0) root         (0)     9628 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/pytorch/models/combined_cnn.py
+-rw-rw-rw-   0 root         (0) root         (0)    11582 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/train_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.888154 soapcw-0.1.6/soapcw/cw/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cw/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    42241 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cw/generate_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    19576 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cw/load_sfts.py
+-rw-rw-rw-   0 root         (0) root         (0)     8660 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cw/make_sfts.py
+-rw-rw-rw-   0 root         (0) root         (0)     9450 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cw/sft.py
+-rw-rw-rw-   0 root         (0) root         (0)     8567 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cw/timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1687 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cw/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.889154 soapcw-0.1.6/soapcw/line_aware_stat/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/line_aware_stat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11721 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/line_aware_stat/gen_lookup.pyx
+-rw-rw-rw-   0 root         (0) root         (0)    38004 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/line_aware_stat/gen_lookup_python.py
+-rwxrwxrwx   0 root         (0) root         (0)     6514 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/line_aware_stat/save_lookup.py
+-rw-rw-rw-   0 root         (0) root         (0)     4047 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/soap_config_parser.py
+-rw-r--r--   0 root         (0) root         (0)  2250446 2023-07-03 20:08:27.000000 soapcw-0.1.6/soapcw/soapcw.c
+-rw-rw-rw-   0 root         (0) root         (0)    63288 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/soapcw.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.889154 soapcw-0.1.6/soapcw/tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 20:06:52.000000 soapcw-0.1.6/soapcw/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2885 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/tools/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)     9044 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/tools/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.886154 soapcw-0.1.6/soapcw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-07-03 20:08:27.000000 soapcw-0.1.6/soapcw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1822 2023-07-03 20:08:27.000000 soapcw-0.1.6/soapcw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 20:08:27.000000 soapcw-0.1.6/soapcw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      484 2023-07-03 20:08:27.000000 soapcw-0.1.6/soapcw.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 20:08:27.000000 soapcw-0.1.6/soapcw.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-03 20:08:27.000000 soapcw-0.1.6/soapcw.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-03 20:08:27.000000 soapcw-0.1.6/soapcw.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.890154 soapcw-0.1.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)   445283 2023-07-03 20:06:51.000000 soapcw-0.1.6/tests/SNR_injections.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-03 20:06:51.000000 soapcw-0.1.6/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2023-07-03 20:06:51.000000 soapcw-0.1.6/tests/test_cwload.py
+-rw-rw-rw-   0 root         (0) root         (0)     3602 2023-07-03 20:06:51.000000 soapcw-0.1.6/tests/test_line_aware_stat.py
+-rw-rw-rw-   0 root         (0) root         (0)     4290 2023-07-03 20:06:51.000000 soapcw-0.1.6/tests/test_soap.py
```

### Comparing `soapcw-0.1.5/CONTRIBUTING.rst` & `soapcw-0.1.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/LICENSE` & `soapcw-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/PKG-INFO` & `soapcw-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soapcw
-Version: 0.1.5
+Version: 0.1.6
 Summary: SOAP is a rapid algorithm to search for continuous sources of gravitational waves, with a wider application to long duration narrowband signals.
 Home-page: https://git.ligo.org/joseph.bayley/soapcw
 Author: Joe Bayley
 Author-email: joseph.bayley@glasgow.ac.uk
 License: MIT license
 Download-URL: https://git.ligo.org/joseph.bayley/soapcw/-/archive/0.1.2/soapcw-0.1.2.tar.gz
 Keywords: soapcw,soap,gravitational waves,pulsars,neutron stars,continuous waves
```

### Comparing `soapcw-0.1.5/README.rst` & `soapcw-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/docs/Makefile` & `soapcw-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/docs/conf.py` & `soapcw-0.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/docs/index.rst` & `soapcw-0.1.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/docs/installation.rst` & `soapcw-0.1.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/docs/make.bat` & `soapcw-0.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/pipeline/css/general.css` & `soapcw-0.1.6/pipeline/css/general.css`

 * *Files 3% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     padding: 20px;
     max-width: 25%;
   }
 
   /* div boxes */
   .box {
     background-color: #f1f1f1;
-    border: 4px solid rgba(6, 109, 6, 0.5);
+    border: 4px solid rgba(35, 48, 90, 0.606);
     margin: 2px;
     padding: 6px;
     text-align: center;
 
   }
   
   /* Main column */
@@ -110,17 +110,17 @@
   .imagewrap {
     margin: auto;
     display: inline-block;
     align-items: center;
     position: relative;
   }
 
-
+/* rgba(6, 109, 6, 0.5) */
   .btn-cl {
-    background-color: rgba(6, 109, 6, 0.5);
+    background-color: rgba(35, 48, 90, 0.606);
   }
 
   .sortable tr {
     cursor: pointer;
 }
   
   /* Responsive layout - when the screen is less than 700px wide, make the two columns stack on top of each other instead of next to each other */
@@ -134,11 +134,15 @@
   @media screen and (max-width: 400px) {
     .navbar a {
       float: none;
       width: 100%;
     }
   }
 
-  table.dataTable tbody tr:hover td
+  table.dataTable tbody tr:hover td 
+  {
+    background-color:rgba(35, 48, 90, 0.606);
+  }
+  table.dataTable tbody tr.selected td 
   {
-    background-color:#1c7b1b94;
+    background-color:rgba(35, 48, 90, 0.606);
   }
```

### Comparing `soapcw-0.1.5/pipeline/make_dag_files_astro.py` & `soapcw-0.1.6/pipeline/make_dag_files_lines.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         f.write('executable = {}\n'.format(execute))
         f.write('getenv  = True\n')
         f.write('RequestMemory = {} \n'.format(config["condor"]["memory"]))
         f.write(f'request_disk={config["condor"]["request_disk"]}\n')
         f.write('log = {}/{}_$(cluster).log\n'.format(cdirs["log_dir"],comment))
         f.write('error = {}/{}_$(cluster).err\n'.format(cdirs["err_dir"],comment))
         f.write('output = {}/{}_$(cluster).out\n'.format(cdirs["output_dir"],comment))
-        args = f'arguments = --config-file {config_file} -s $(bandstart) -e $(bandend) -r {config["data"]["obs_run"]} -l {config["lookuptable"]["lookup_dir"]} -w {config["condor"]["band_load_size"]} -sd {config["output"]["sub_directory"]}'
+        args = f'arguments = --config-file {config_file} -s $(bandstart) -e $(bandend) -r {config["data"]["obs_run"]} -w {config["condor"]["band_load_size"]} -sd {config["output"]["sub_directory"]}'
 
         f.write(args + "\n")
         #f.write('accounting_group = aluk.dev.s6.cw.viterbi\n')
         f.write(f'accounting_group = {config["condor"]["accounting_group"]}\n')
         f.write('queue\n')
     if verbose:
         print(time.time(), "generated subfile")
@@ -79,15 +79,15 @@
     ##
     ## Make the sub file for SOAP run and summary page generation
     ##
 
     bs1 = config["data"]["band_starts"]
     be1 = config["data"]["band_ends"]
 
-    run_sub_comment = "soap_astro_F{}_{}_{}".format(bs1[0],be1[0],config["data"]["obs_run"])
+    run_sub_comment = "soap_line_F{}_{}_{}".format(bs1[0],be1[0],config["data"]["obs_run"])
     html_sub_comment = "soap_html_F{}_{}_{}".format(bs1[0],be1[0],config["data"]["obs_run"])
 
     run_sub_filename = "{}/{}.sub".format(condor_dirs["condor_dir"],run_sub_comment)
     html_sub_filename = "{}/{}.sub".format(condor_dirs["condor_dir"],html_sub_comment)
 
     write_plot_subfile(run_sub_filename,config,config_file,condor_dirs,run_sub_comment,verbose=verbose)
     write_html_subfile(html_sub_filename,config,config_file,condor_dirs,html_sub_comment,verbose=verbose)
@@ -146,15 +146,15 @@
         order_string = "PARENT {} CHILD {} \n".format(" ".join(jobids),jobid)
         f.write(job_string)
         f.write(retry_string)
         #f.write(vars_string)
         f.write(order_string)
     if verbose:
         print(time.time(), "generated dag file")
-
+    
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("-c", "--config-file", help="configuration file for soap")
     try:                                                     
         args = parser.parse_args()  
     except:  
@@ -164,12 +164,12 @@
 
     config = SOAPConfig(args.config_file)
     #config = configparser.ConfigParser()
     #config.read(config_file)
 
     write_dagfile(config_file, config)
 
-if __name__ == '__main__':
+if __name__ == '__main__()':
     main()
```

### Comparing `soapcw-0.1.5/pipeline/make_dag_files_lines.py` & `soapcw-0.1.6/pipeline/make_dag_files_astro.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         f.write('executable = {}\n'.format(execute))
         f.write('getenv  = True\n')
         f.write('RequestMemory = {} \n'.format(config["condor"]["memory"]))
         f.write(f'request_disk={config["condor"]["request_disk"]}\n')
         f.write('log = {}/{}_$(cluster).log\n'.format(cdirs["log_dir"],comment))
         f.write('error = {}/{}_$(cluster).err\n'.format(cdirs["err_dir"],comment))
         f.write('output = {}/{}_$(cluster).out\n'.format(cdirs["output_dir"],comment))
-        args = f'arguments = --config-file {config_file} -s $(bandstart) -e $(bandend) -r {config["data"]["obs_run"]} -w {config["condor"]["band_load_size"]} -sd {config["output"]["sub_directory"]}'
+        args = f'arguments = --config-file {config_file} -s $(bandstart) -e $(bandend) -r {config["data"]["obs_run"]} -l {config["lookuptable"]["lookup_dir"]} -w {config["condor"]["band_load_size"]} -sd {config["output"]["sub_directory"]}'
 
         f.write(args + "\n")
         #f.write('accounting_group = aluk.dev.s6.cw.viterbi\n')
         f.write(f'accounting_group = {config["condor"]["accounting_group"]}\n')
         f.write('queue\n')
     if verbose:
         print(time.time(), "generated subfile")
@@ -79,16 +79,16 @@
     ##
     ## Make the sub file for SOAP run and summary page generation
     ##
 
     bs1 = config["data"]["band_starts"]
     be1 = config["data"]["band_ends"]
 
-    run_sub_comment = "soap_line_F{}_{}_{}".format(bs1[0],be1[0],config["data"]["obs_run"])
-    html_sub_comment = "soap_html_F{}_{}_{}".format(bs1[0],be1[0],config["data"]["obs_run"])
+    run_sub_comment = "soap_astro_F{}_{}_{}".format(bs1[0],be1[-1],config["data"]["obs_run"])
+    html_sub_comment = "soap_html_F{}_{}_{}".format(bs1[0],be1[-1],config["data"]["obs_run"])
 
     run_sub_filename = "{}/{}.sub".format(condor_dirs["condor_dir"],run_sub_comment)
     html_sub_filename = "{}/{}.sub".format(condor_dirs["condor_dir"],html_sub_comment)
 
     write_plot_subfile(run_sub_filename,config,config_file,condor_dirs,run_sub_comment,verbose=verbose)
     write_html_subfile(html_sub_filename,config,config_file,condor_dirs,html_sub_comment,verbose=verbose)
 
@@ -146,15 +146,15 @@
         order_string = "PARENT {} CHILD {} \n".format(" ".join(jobids),jobid)
         f.write(job_string)
         f.write(retry_string)
         #f.write(vars_string)
         f.write(order_string)
     if verbose:
         print(time.time(), "generated dag file")
-    
+
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("-c", "--config-file", help="configuration file for soap")
     try:                                                     
         args = parser.parse_args()  
     except:  
@@ -164,12 +164,12 @@
 
     config = SOAPConfig(args.config_file)
     #config = configparser.ConfigParser()
     #config.read(config_file)
 
     write_dagfile(config_file, config)
 
-if __name__ == '__main__()':
+if __name__ == '__main__':
     main()
```

### Comparing `soapcw-0.1.5/pipeline/make_html_page.py` & `soapcw-0.1.6/pipeline/make_html_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,22 +278,22 @@
 
             </html>'''
 
     return html
 
 
 
-def create_run_page(run_headings):
+def create_run_page(run_headings, obs_run="run"):
 
 
     html = f'''
     <!DOCTYPE html>
     <html lang="en">
     <head>
-    <title>O3</title>
+    <title>{obs_run}</title>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
     <link rel="stylesheet" href="../../../css/general.css" media="screen" type="text/css">
 
     <link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.2.0/css/bootstrap.min.css" rel="stylesheet">   
     <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.7.1/jquery.min.js"></script>
     <link rel="stylesheet" href="https://cdn.datatables.net/1.10.2/css/jquery.dataTables.min.css"></style>
@@ -394,22 +394,22 @@
     # button to be added to show all of the frequency bands
     """ <div class="box" id="showalldiv">
         <button type="button" class="btn btn-cl py-3" id="showallbutton" onclick="loadAllBands(event)"> Load all bands</button>
         </div>"""
 
     return html
 
-def create_line_run_page(run_headings):
+def create_line_run_page(run_headings, obs_run="run"):
 
 
     html = f'''
     <!DOCTYPE html>
     <html lang="en">
     <head>
-    <title>O3</title>
+    <title>{obs_run}</title>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
     <link rel="stylesheet" href="../../../../css/general.css" media="screen" type="text/css">
 
     <link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.2.0/css/bootstrap.min.css" rel="stylesheet">   
     <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.7.1/jquery.min.js"></script>
     <link rel="stylesheet" href="https://cdn.datatables.net/1.10.2/css/jquery.dataTables.min.css"></style>
@@ -720,21 +720,21 @@
                     sub_headings += f'<l1><a href="{public_dir}/{head}/{subhead}/{subhead}.html"> {subhead} </a></li> </br>'
 
                     if os.path.exists(os.path.join(subdir, "table.json")):
                         if force_overwrite:
                             try:
                                 make_json_from_hdf5(subdir, linepaths, table_order, hwinjfile=hwinjfile)
                             except:
-                                print(f"WARNING: Cannot recreate json table, no new updates to {subhead}, {subdir}")
+                                print(f"WARNING: Cannot recreate json table")
                         else:
                             print(f"WARNING: No new updates to {subhead}, {subdir}")
                     else:
                         make_json_from_hdf5(subdir, linepaths, table_order, hwinjfile=hwinjfile)
 
-                    run_html = create_run_page(run_headings)
+                    run_html = create_run_page(run_headings, obs_run=head)
                     with open(os.path.join(subdir, f"{subhead}.html"), "w") as f:
                         f.write(run_html)
             sub_headings += "</ul>"
 
     return run_headings, sub_headings
 
 def get_html_string_week(root_dir, linepath=None, table_order=None):
@@ -759,36 +759,36 @@
                                     try:
                                         make_json_from_hdf5(weekdir, linepaths, table_order)
                                     except:
                                         print(f"WARNING: Cannot recreate json table, no new updates to {subhead}, {weekdir}")
                                 else:
                                     make_json_from_hdf5(weekdir, linepaths, table_order)
 
-                                run_html = create_line_run_page(line_run_headings)
+                                run_html = create_line_run_page(line_run_headings, obs_run=head)
                                 with open(os.path.join(weekdir, f"{subhead}.html"), "w") as f:
                                     f.write(run_html)
                             else:
                                 sub_headings += f'<l1><a href="./{head}/{subhead}/{subhead}.html"> {subhead} </a></li> </br>'
 
                                 if os.path.exists(os.path.join(subdir, "table.json")):
                                     try:
                                         make_json_from_hdf5(subdir, linepaths, table_order)
                                     except:
                                         print(f"WARNING: Cannot recreate json table, no new updates to {subhead}, {subdir}")
                                 else:
                                     make_json_from_hdf5(subdir, linepaths, table_order)
 
-                                run_html = create_line_run_page(line_run_headings)
+                                run_html = create_line_run_page(line_run_headings, obs_run=head)
                                 with open(os.path.join(subdir, f"{subhead}.html"), "w") as f:
                                     f.write(run_html)
                 sub_headings += "</ul>"
 
     return run_headings, sub_headings
 
-def write_pages(root_dir, linepaths, table_order, force_overwrite=False, hwinjfile=None):
+def write_pages(root_dir, linepaths, table_order, force_overwrite=False, hwinjfile=None, obs_run="run"):
     """ Generate and write the html pages with the inputs from the directory structure"""
     
     make_directory_structure(root_dir)
 
     astro_dir = os.path.join(root_dir, "astrophysical")
 
     run_headings,sub_headings = get_html_string(astro_dir, linepaths=linepaths, table_order=table_order, force_overwrite=force_overwrite, hwinjfile=hwinjfile)
```

### Comparing `soapcw-0.1.5/pipeline/run_full_soap_astro.py` & `soapcw-0.1.6/pipeline/run_full_soap_astro.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,35 +59,45 @@
         for path, subdirs, files in os.walk(sftpath):
             #print(path, subdirs, files)
             for name in files:
                 if name != "" and name.endswith(".sft"):
                     sftlist.append(os.path.join(path, name))
     return sftlist
 
-def get_sft_files_find(output_dir, sftpaths):
+def get_sft_files_find(output_dir, sftpaths, force_overwrite=False):
     sftlist = []
     if type(sftpaths) == str:
         sftpaths = sftpaths.split(",")
     fnames = []
     for sftpath in sftpaths:
         pathsplit = sftpath.split('/')
         pathappend = pathsplit[-2] if pathsplit[-1] == "" else pathsplit[-1]
         fname = os.path.join(output_dir, f"{pathappend}_sftfile.txt")
         fnames.append(fname)
         sftpath = sftpath.strip()
-        if not os.path.isfile(fname):
+        print("SFTpath", sftpath)
+        if not os.path.isfile(fname) or force_overwrite:
             with open(fname, "w") as f:
-                findout = subprocess.run([
+                findout1 = subprocess.Popen([
                         "find",
                         sftpath,
                         "-name",
-                        "*.sft",
+                        "*.sft"
                     ], 
-                    stdout=f,
+                    stdout=subprocess.PIPE,
                     shell=False)
+                findout = subprocess.run([
+                    "sort"],
+                    stdin=findout1.stdout,
+                    stdout=f,
+                    shell=False
+                )
+                print(findout)
+        else:
+            print("SFT filelist exists: not continuing")
 
     return fnames
 
 def av_noise(noise,nsft=48):
     """
     get the median noise floor for every nsft sfts
     """
@@ -115,19 +125,20 @@
 
     # define the transition matrix for soap
     tr = soap.tools.transition_matrix_2d(config["transitionmatrix"]["left_right_prob"],
                                         config["transitionmatrix"]["det1_prob"],
                                         config["transitionmatrix"]["det2_prob"])
 
     # run soap search using the two detector line aware statistic (one detector in gaps)
+
     if len(getattr(sft,"det_names")) == 2:
         # SOAP using SNR based statistic
-        if config["lookuptable"]["type"] == "power":
+        if config["lookuptable"]["lookup_type"] == "power":
             soaprun = soap.two_detector(tr,sft.H1.downsamp_summed_norm_sft_power[:,ind_start:ind_end],sft.L1.downsamp_summed_norm_sft_power[:,ind_start:ind_end],lookup_file_2det=lookup_2,lookup_file_1det=lookup_1)
-        elif config["lookuptable"]["type"] == "amplitude":
+        elif config["lookuptable"]["lookup_type"] == "amplitude":
             # SOAP using amplitude statistics
             # get the ratio of duty cycle and noise floor of the two detectors (used if using amplitude based statistic_
             fractions = 1./(sft.L1.summed_dutycycle*sft.H1.summed_rng_med/(sft.H1.summed_dutycycle*sft.L1.summed_rng_med))
             # where there is no data (i.e. nans) set the detectors to equal sensitivity
             fractions[np.isnan(fractions)] = 1
             soaprun = soap.two_detector(tr,sft.H1.downsamp_summed_norm_sft_power[:,ind_start:ind_end],sft.L1.downsamp_summed_norm_sft_power[:,ind_start:ind_end],lookup_file_2det=lookup_2,fractions = fractions)
 
@@ -217,18 +228,18 @@
 
     Returns:
         _type_: _description_
     """
 
     # plot images 
     H_imlim = set_limit(H_temp_sft, cut=plotcut)
-    H_im = ax[0].imshow(H_temp_sft.T,cmap="YlGnBu",aspect="auto",origin="lower",vmin=H_imlim[0],vmax=H_imlim[1])
+    H_im = ax[0].imshow(H_temp_sft.T,cmap="cividis",aspect="auto",origin="lower",vmin=H_imlim[0],vmax=H_imlim[1], interpolation="none")
     L_imlim = set_limit(L_temp_sft, cut=plotcut)
-    L_im = ax[1].imshow(L_temp_sft.T,cmap="YlGnBu",aspect="auto",origin="lower",vmin=L_imlim[0],vmax=L_imlim[1])
-    imv = ax[2].imshow(soaprun.vitmap.T,cmap="YlGnBu",aspect="auto",origin="lower")
+    L_im = ax[1].imshow(L_temp_sft.T,cmap="cividis",aspect="auto",origin="lower",vmin=L_imlim[0],vmax=L_imlim[1], interpolation="none")
+    imv = ax[2].imshow(soaprun.vitmap.T,cmap="cividis",aspect="auto",origin="lower", interpolation="none")
             
     # plot track power s
     Hpwline, = ax[3].plot(np.arange(sum_nsft),np.array(soap.tools.track_power(soaprun.vit_track1,H_temp_sft)),color="C3",label="H1")
     Lpwline, = ax[3].plot(np.arange(sum_nsft),np.array(soap.tools.track_power(soaprun.vit_track2,L_temp_sft)),color="C2",label="L1")
 
     # plot viterbi statistic
     Hstatline, = ax[4].plot(np.arange(sum_nsft),np.array(soap.tools.stat_on_path(soaprun.vit_track,soaprun.V)),color="C3",label="H1")
@@ -391,33 +402,53 @@
     
     # get the sft files and start/end times
     outpath = os.path.join(*[config["output"]["save_directory"],config["data"]["obs_run"]])    
 
     if not os.path.isdir(outpath):
         os.makedirs(outpath)
 
+    # set output directories
+    outpath = os.path.join(outpath,config["output"]["sub_directory"])
+    outpath_save = outpath
+
+    if os.path.isdir(outpath_save):
+        pathexists = True
+    else:
+        pathexists = False
+
+    outpath_save_plots = os.path.join(outpath_save,"plots")
+    outpath_save_track = os.path.join(outpath_save,"tracks")
+    output_save_files = os.path.join(outpath_save, "data")
+            
+    for direc in [outpath_save_plots,outpath_save_track, output_save_files]:
+        if not os.path.isdir(direc):
+            os.makedirs(direc)
+        else:
+            pass
+
     #print(sftfiles)
     sftfiles = config["input"]["load_directory"]
     print("num files: ", len(sftfiles))
     start_load = time.time()
 
-    sft_filelists = get_sft_files_find(outpath, sftfiles)
+    sft_filelists = get_sft_files_find(outpath, sftfiles, config["output"]["overwrite_files"])
 
     sftlist = []
     for sftfile in sft_filelists:
         with open(sftfile,"r") as f:
             sftlist.extend(f.readlines())
 
     sttime = [float(os.path.basename(name).split("-")[-2]) for name in sftlist]
 
     print("numsfts: {}".format(len(sftlist)))
     print("Time find fnames: ", time.time() - start_load)
     tmin = np.min(sttime) 
-    tmax = np.max(sttime) + 1800 # start of last sft plus length (in this case we are only using 1800s sfts)
+    tmax = np.max(sttime) + 1800 # start of last sft plus length (in this case we are only using 1800s sfts
     #tmax = min(sttime) + 48*10*1800 # smaller range for testing
+    print(f"minmaxtime, {tmin} --> {tmax}")
     
     # get the sfts in the specified time range 
     start_range = time.time()
     sftlist = get_sfts_in_range(tmin,tmax,sftlist)
     time_getsftsrange = time.time() - start_range
     print("time_getsftsrange: ", time_getsftsrange)
 
@@ -435,31 +466,14 @@
 
     # define start times in gps and date format
     start_time_gps = Time(tmin,format="gps")
     end_time_gps = Time(tmax,format="gps")
     startdatestring = start_time_gps.iso.split(" ")[0].replace("-","")
     enddatestring = end_time_gps.iso.split(" ")[0].replace("-","")
 
-    # set output directories
-    outpath_save = os.path.join(outpath,config["output"]["sub_directory"])
-
-    if os.path.isdir(outpath_save):
-        pathexists = True
-    else:
-        pathexists = False
-                
-    outpath_save_plots = os.path.join(outpath_save,"plots")
-    outpath_save_track = os.path.join(outpath_save,"tracks")
-    output_save_files = os.path.join(outpath_save, "data")
-            
-    for direc in [outpath_save_plots,outpath_save_track, output_save_files]:
-        if not os.path.isdir(direc):
-            os.makedirs(direc)
-        else:
-            pass
 
     # combine all filenames infor format input to lalpulsar loading (via LoadSFT)
     filenames = ";".join([s.strip() for s in sftlist])
 
     # load in the sfts, normalise them to the running median and fill the gaps
     start_load_sft = time.time()
     sft, stride, degfree, plotcut, width = load_sft_band(config, filenames, minfreq, maxfreq, tmin, tmax, verbose=verbose)
@@ -672,15 +686,15 @@
         fig.savefig(save_path_track,bbox_inches="tight",dpi=60)
         
         av_save.append(time.time() - st_sv)
         del H_temp_sft,L_temp_sft, soaprun, temp_noise
      
     # write table of statistics 
     tablefile = os.path.join(output_save_files,f"table_{minfreq}_{maxfreq}.hdf5")
-    if os.path.isfile(tablefile):
+    if os.path.isfile(tablefile) and config["output"]["overwrite_files"] == False:
         new_tablefile = os.path.join(output_save_files,f"table_{minfreq}_{maxfreq}_{np.random.randint(low=0,high=1000)}.hdf5")
         print(f"File exists: {tablefile}, writing to {new_tablefile}")
         tablefile = new_tablefile
         #with open(new_tablefile,"wb") as f:  
         #    pickle.dump(table_data, f)
     else:
         tablefile = tablefile
```

### Comparing `soapcw-0.1.5/pipeline/run_full_soap_lines.py` & `soapcw-0.1.6/pipeline/run_full_soap_lines.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,34 +59,47 @@
         for path, subdirs, files in os.walk(sftpath):
             #print(path, subdirs, files)
             for name in files:
                 if name != "" and name.endswith(".sft"):
                     sftlist.append(os.path.join(path, name))
     return sftlist
 
-def get_sft_files_find(output_dir, sftpaths):
+def get_sft_files_find(output_dir, sftpaths, overwrite_file=False):
     sftlist = []
     if type(sftpaths) == str:
         sftpaths = sftpaths.split(",")
     fnames = []
     for sftpath in sftpaths:
         pathsplit = sftpath.split('/')
         pathappend = pathsplit[-2] if pathsplit[-1] == "" else pathsplit[-1]
         fname = os.path.join(output_dir, f"{pathappend}_sftfile.txt")
         fnames.append(fname)
         sftpath = sftpath.strip()
-        with open(fname, "w") as f:
-            findout = subprocess.run([
-                    "find",
-                    sftpath,
-                    "-name",
-                    "*.sft",
-                ], 
-                stdout=f,
-                shell=False)
+        print("sftfilename", fname)
+        if not os.path.isfile(fname) or overwrite_file:
+            with open(fname, "w") as f:
+                findout1 = subprocess.Popen([
+                        "find",
+                        sftpath,
+                        "-name",
+                        "*.sft"
+                    ], 
+                    stdout=subprocess.PIPE,
+                    shell=False)
+                findout = subprocess.run([
+                    "sort"],
+                    stdin=findout1.stdout,
+                    stdout=f,
+                    shell=False
+                )
+
+                print(findout)
+        else:
+            print("SFT filelist exists")
+
 
     return fnames
 
 def av_noise(noise,nsft=48):
     """
     get the median noise floor for every nsft sfts
     """
@@ -215,19 +228,19 @@
 
     Returns:
         _type_: _description_
     """
 
     # plot images 
     H_imlim = set_limit(H_temp_sft, cut=plotcut)
-    H_im = ax[0].imshow(H_temp_sft.T,cmap="YlGnBu",aspect="auto",origin="lower",vmin=H_imlim[0],vmax=H_imlim[1], interpolation="none")
+    H_im = ax[0].imshow(H_temp_sft.T,cmap="cividis",aspect="auto",origin="lower",vmin=H_imlim[0],vmax=H_imlim[1], interpolation="none")
     L_imlim = set_limit(L_temp_sft, cut=plotcut)
-    L_im = ax[1].imshow(L_temp_sft.T,cmap="YlGnBu",aspect="auto",origin="lower",vmin=L_imlim[0],vmax=L_imlim[1], interpolation="none")
-    imvh1 = ax[2].imshow(soaprunH1.vitmap.T,cmap="YlGnBu",aspect="auto",origin="lower", interpolation="none")
-    imvl1 = ax[3].imshow(soaprunL1.vitmap.T,cmap="YlGnBu",aspect="auto",origin="lower", interpolation="none")
+    L_im = ax[1].imshow(L_temp_sft.T,cmap="cividis",aspect="auto",origin="lower",vmin=L_imlim[0],vmax=L_imlim[1], interpolation="none")
+    imvh1 = ax[2].imshow(soaprunH1.vitmap.T,cmap="cividis",aspect="auto",origin="lower", interpolation="none")
+    imvl1 = ax[3].imshow(soaprunL1.vitmap.T,cmap="cividis",aspect="auto",origin="lower", interpolation="none")
             
     # plot track power s
     Hpwline, = ax[4].plot(np.arange(sum_nsft),np.array(soap.tools.track_power(soaprunH1.vit_track,H_temp_sft)),color="C3",label="H1")
     Lpwline, = ax[4].plot(np.arange(sum_nsft),np.array(soap.tools.track_power(soaprunL1.vit_track,L_temp_sft)),color="C2",label="L1")
 
     # plot viterbi statistic
     Hstatline, = ax[5].plot(np.arange(sum_nsft),np.array(soap.tools.stat_on_path(soaprunH1.vit_track,soaprunH1.V)),color="C3",label="H1")
@@ -417,16 +430,17 @@
                 print(f"WARNING!!! - Overwriting current existing directory: {outpath_save}")
 
     # get the list of sft filenames by iterating over subdirs 
     # this saves the filelise to a file
     sftfiles = config["input"]["load_directory"]
     print("num files: ", len(sftfiles))
     start_load = time.time()
-    sft_filelists = get_sft_files_find(outpath, sftfiles)
+    sft_filelists = get_sft_files_find(outpath, sftfiles, overwrite_file=config["output"]["overwrite_files"])
 
+    print("SFT filelist", sft_filelists)
     # load in the sft filelists 
     sftlist = []
     for sftfile in sft_filelists:
         with open(sftfile,"r") as f:
             sftlist.extend(f.readlines())
     
     if len(sftlist) == 0:
```

### Comparing `soapcw-0.1.5/pipeline/scripts/table_scripts.js` & `soapcw-0.1.6/pipeline/scripts/table_scripts.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,38 +1,44 @@
 $(document).ready(function() {
 
+    /* Initially load the table json file containing data*/
     $.getJSON('./table.json', function(data) {
         let keys = Object.keys(data[0]);
 
         const loadMoreButton = document.getElementById("showallbutton");
 
         let startIndex = 0;
         const table = document.getElementById("inTable");
+        /* Create the headers for the table*/
         let head = table.createTHead();
         let hrow = head.insertRow(0);
         for (let i = 0; i < keys.length; i++) {
             let hcol = hrow.insertCell(i);
             hcol.innerHTML = keys[i];
         }
+        /* Load the table rows using below function*/
         let table2 = loadTableElements(startIndex, data);
 
         /*let jtable = $('#inTable').DataTable({searching: false, paging: false, info: false, "bAutoWidth": false,});*/
+        /* Make the checkboxed for each column and sort the columns by selected sort column*/
         makeCheckBoxes(data);
         /*loadTableData(data);*/
         let stat_index = get_plot_column(table2, "lineaware_stat");
         const sortdrop = document.getElementById("sortby");
         sortdrop.selectedIndex = stat_index;
         const sortorder = document.getElementById("sortorder");
         sortorder.selectedIndex = 1;
+        /* reload the page the set each of these*/
         reloadPage()
 
 
     });
 
 
+    /* initialise the data table for jquery*/
     $('#inTable').load(function() {
         let table = $('#inTable').DataTable({
             "ordering": false,
             searching: false,
             paging: false,
             info: false,
             "bAutoWidth": false,
@@ -45,14 +51,15 @@
         makeInfoTable(table, row);
         table.column(index).visible(true);
         table.column(index).visible(false);
 
 
     });
 
+    /* Show images and the infor table when a row is clicked in the table*/
     $('#inTable').on('click', 'tbody tr', function() {
         /*
         let table = $('#inTable').DataTable({retrieve:true});
         let index = get_plot_column(table, "plot_path");
 
         var d0 = $(this).find("td").eq(0).text();
         var d1 = $(this).find("td").eq(1).text();
@@ -67,57 +74,69 @@
         }).fnGetData($(this));
         var newpath = rowdata[index];
         /*var newpath = table.rows(table.rows()[0][this.rowIndex]-1).data()[0][index];*/
         const image = document.getElementById("image");
         image.setAttribute("value", $(this).context.sectionRowIndex);
         changeImg(newpath);
         makeInfoTable(table, rowdata);
+        $('#inTable tr').removeClass("selected");
+        $(this).addClass('selected');
+
     });
 });
 
 function nextTablePage(event) {
+    /* Move to the next page of the table*/
+    /* This selects the next 10 items from the entire json dataset and displays them in a table*/
     let itemsPerPage = 10;
     $.getJSON('./table.json', function(data) {
         let lpage = document.getElementById("lastpagebutton");
         let npage = document.getElementById("lastpagebutton");
         npage.value = parseInt(npage.value) + parseInt(itemsPerPage);
         lpage.value = parseInt(lpage.value) + parseInt(itemsPerPage);
+
         const image = document.getElementById("image");
         image.setAttribute("value", 0);
+
         data = checkFilters(data);
         /*event.target.value = parseInt(event.target.value) + parseInt(itemsPerPage);*/
         if (parseInt(npage.value) > parseInt(data.length)) {
             window.alert("End of table");
         } else {
             let table = loadTableElements(npage.value, data);
             setVisible(data);
         }
     });
 };
 
 function lastTablePage(event) {
     $.getJSON('./table.json', function(data) {
+        /* Move to the previous page of the table*/
+        /* This selects the previous 10 items from the entire json dataset and displays them in a table*/
         let itemsPerPage = 10;
         let lpage = document.getElementById("lastpagebutton");
         let npage = document.getElementById("lastpagebutton");
         npage.value = parseInt(npage.value) - parseInt(itemsPerPage);
         lpage.value = parseInt(lpage.value) - parseInt(itemsPerPage);
+
         const image = document.getElementById("image");
-        image.setAttribute("value", 0);
+        image.setAttribute("value", 9);
+
         data = checkFilters(data);
         if (lpage.value < 0) {
             window.alert("End of table");
         } else {
             let table = loadTableElements(lpage.value, data);
             setVisible(data);
         }
     });
 };
 
 function reloadPage() {
+    /* reload the entire page checking the filters and loading appropriate table rows*/
     $.getJSON('./table.json', function(data) {
         let lpage = document.getElementById("lastpagebutton");
         let npage = document.getElementById("lastpagebutton");
         lpage.value = 0;
         npage.value = 0;
         data = checkFilters(data);
         loadTableElements(0, data);
@@ -316,14 +335,19 @@
         if (headers[i] == key) {
             index = i;
         }
     }
     return index;
 }
 
+function highlightRow(table, row) {
+    table.removeClass("highlight");
+    row.addClass("highlight");
+}
+
 function nextImage(event) {
 
     let table = $('#inTable').DataTable({
         retrieve: true,
         searching: false,
         paging: false,
         info: false,
@@ -336,22 +360,30 @@
         'opacity': 0.5
     });
     let value = image.getAttribute("value");
     let newrow = parseInt(value) + 1
     if (newrow > $('#inTable tr').length - 2) {
         nextTablePage(event);
         /*window.alert("After end of table");*/
+        newrow = 0;
     } else {
         let row = table.row(newrow).data();
         let index = get_plot_column(table, "plot_path");
         var newpath = row[index];
         changeImg(newpath);
         image.setAttribute("value", newrow);
         makeInfoTable(table, row);
+        $('#inTable tr').removeClass("selected");
+        $('#inTable tr').each(function() {
+            if (this._DT_RowIndex == newrow) {
+                $(this).addClass('selected');
+            }
+        })
     }
+
     $("#image").css({
         'opacity': 1.0
     });
 
 }
 
 function previousImage(event) {
@@ -368,30 +400,49 @@
     const image = document.getElementById("image");
     let value = image.getAttribute("value");
     let newrow = parseInt(value) - 1
     $("#image").css({
         'opacity': 0.5
     });
     if (newrow < 0) {
-        lastTablePage(event);
+        table = lastTablePage(event);
         /*window.alert("Before start of table");*/
+        newrow = 9;
     } else {
         let row = table.row(newrow).data();
         let index = get_plot_column(table, "plot_path");
         var newpath = row[index];
         changeImg(newpath);
         image.setAttribute("value", newrow);
         makeInfoTable(table, row);
+        $('#inTable tr').removeClass("selected");
+        $('#inTable tr').each(function() {
+            if (this._DT_RowIndex == newrow) {
+                $(this).addClass('selected');
+            }
+        })
     }
+
+
+
     $("#image").css({
         'opacity': 1.0
     });
 }
 
 function changeImg(newpath) {
+    /* change the image based on the input new path */
+    /* If the button for hiding and showing track is clicked the show the appropriate image*/
+
+    const button = document.getElementById("trackbutton");
+    if (button.value == 1) {
+        newpath = newpath.replace("/track_", "/notrack_");
+    } else {
+        newpath = newpath.replace("/notrack_", "/track_")
+    }
 
     $("#plotlink").attr("href", newpath);
 
     $("#image").attr("src", newpath);
 
 }
```

### Comparing `soapcw-0.1.5/setup.cfg` & `soapcw-0.1.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.5
+current_version = 0.1.6
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
 
@@ -17,15 +17,15 @@
 [flake8]
 exclude = docs
 
 [aliases]
 
 [metadata]
 name = soapcw
-version = 0.1.5
+version = 0.1.6
 
 [options]
 packages = soapcw, pipeline
 
 [options.entry_points]
 console_scripts = 
 	soapcw-make-dag-files-lines = pipeline.make_dag_files_lines:main
```

### Comparing `soapcw-0.1.5/setup.py` & `soapcw-0.1.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     ext_modules = [
     Extension("soapcw.soapcw",
               [ "soapcw/soapcw.pyx" ]),]
 
 
 cmdclass = { 'build_ext': build_ext , }
 
-setup_requirements = ["cython", "matplotlib", "numpy", "torch", "scipy", "lalsuite"]
+setup_requirements = ["cython", "matplotlib", "numpy", "torch", "torch-summary", "scipy", "lalsuite", "regex"]
 
 test_requirements = ["cython"]
 
 setup(
     author="Joe Bayley",
     author_email='joseph.bayley@glasgow.ac.uk',
     classifiers=[
```

### Comparing `soapcw-0.1.5/soapcw/__init__.py` & `soapcw-0.1.6/soapcw/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,13 +6,14 @@
 __email__ = 'joseph.bayley@glasgow.ac.uk'
 __version__ = '0.1.0'
 from .soapcw import single_detector, two_detector, three_detector, single_detector_gaps
 from .tools import tools, plots
 from .cnn import __init__
 from .line_aware_stat import __init__
 from .cw import __init__
+from . import soap_config_parser
 
 #try:
 #    from .lookup_table import gen_lookup_python, save_lookup, gen_lookup
 #except:
 #    from .lookup_table import gen_lookup_python, save_lookup
```

### Comparing `soapcw-0.1.5/soapcw/cnn/cnn_data_dag_gen.py` & `soapcw-0.1.6/soapcw/cnn/cnn_data_dag_gen.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/soapcw/cnn/cnn_data_gen.py` & `soapcw-0.1.6/soapcw/cnn/cnn_data_gen.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,18 +44,18 @@
     lindir = os.path.join(indir,"L1")
 
     hname = None
     lname = None
 
     # loops over files to find one with matching string
     for fname in os.listdir(hindir):
+        #print("F{:0>4}Hz".format(int(bandmin)), fname)
         if "F{:0>4}Hz".format(int(bandmin)) in fname:
             hname = fname
 
-
     for fname in os.listdir(lindir):
         #if "F{}_{}.sft".format(bandmin,bandmax) in fname:
         if "F{:0>4}Hz".format(int(bandmin)) in fname:
             lname = fname
 
     if hname is None or lname is None:
         print("NO SFT FOUND {}, {}, {}, F{:0>4}Hz".format(indir, bandmin, bandmax, int(bandmin)))
@@ -345,17 +345,40 @@
                 gaussian_train.loop_band_train_augment(loadpath=args.load_dir,path=save_dir,bandmin=args.band_min,bandmax=args.band_max, band_width=args.band_width,resize_image=args.resize_image, nonoise=args.no_noise,snr_min=args.snr_min,snr_max=args.snr_max,nperband=1,test=True,save_options=args.save_options.split(" "))
 
         elif args.data_type in ["train", "validation"]:
             save_dir = os.path.join(config["general"]["save_dir"], args.data_type)
 
             print("runtype", args.run_type)
             if args.run_type == "gaussian" or args.run_type == "gauss":
-                generate_gaussian_train_data.loop_band_train_augment(config, path=save_dir,bandmin=args.band_min,bandmax=args.band_max, band_width=args.band_width, nonoise=args.no_noise,snr_min=config["data"]["snrmin"],snr_max=config["data"]["snrmax"],nperband=args.nperband,test=False,save_options=config["data"]["save_options"])
+                generate_gaussian_train_data.loop_band_train_augment(
+                    config, 
+                    path=save_dir,
+                    bandmin=args.band_min,
+                    bandmax=args.band_max, 
+                    band_width=args.band_width, 
+                    nonoise=args.no_noise,
+                    snr_min=config["data"]["snrmin"],
+                    snr_max=config["data"]["snrmax"],
+                    nperband=args.nperband,
+                    test=False,
+                    save_options=config["data"]["save_options"]
+                    )
             else:
-                generate_train_data.loop_band_train_augment(config, args.load_dir,save_dir,args.band_min,args.band_max,args.band_width,args.resize_image, nonoise=args.no_noise,snr_min=args.snr_min,snr_max=args.snr_max)
+                generate_train_data.loop_band_train_augment(
+                    config, 
+                    save_dir,
+                    args.band_min,
+                    args.band_max,
+                    args.band_width,
+                    config["data"]["resize_image"], 
+                    gen_noise_only=config["data"]["gen_noise_only"],
+                    snr_min=config["data"]["snrmin"],
+                    snr_max=config["data"]["snrmax"],
+                    save_options=config["data"]["save_options"]
+                    )
 
         """
         elif args.mdc == True:
             mdc_test.loop_band_mdc(args.save_dir,args.load_dir,args.noise_dir,args.band_min,args.band_max,args.band_width,args.resize_image)
         elif args.search == True:
             generate_test_data.loop_band_test_data(args.load_dir,args.save_dir,args.band_min,args.band_max,args.band_width,args.resize_image,search = True)
         """
```

### Comparing `soapcw-0.1.5/soapcw/cnn/generate_gaussian_train_data.py` & `soapcw-0.1.6/soapcw/cnn/generate_gaussian_train_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,42 +9,14 @@
 import h5py
 
 def loop_band_train_augment(config, path,bandmin,bandmax,band_width,loadpath=None,nonoise=False,snr_min = 50,snr_max=150,nperband=10,test=False, save_options=None):
     """
     loop over bands to create training data
     """
 
-    """
-    # !!!!!!!!!changed the widths of bands as a test, probably change back at some poitn!!!!!!!
-    if 40 <= bandmin <= 500: 
-        stride = 1
-        degfree = 96
-        plotcut = stride*180
-        width = 0.2
-        brange = "band_40_500"
-    elif 500 < bandmin <= 1000:
-        stride = 2
-        degfree = int(stride*96)
-        plotcut = stride*180
-        width = 0.3
-        brange = "band_500_1000"
-    elif 1000 < bandmin <= 1500:
-        stride = 3
-        degfree = int(stride*96)
-        plotcut = stride*180
-        width = 0.4
-        brange = "band_1000_1500"
-    elif 1500 < bandmin <= 2000:
-        stride = 4
-        degfree = int(stride*96)
-        plotcut = stride*180
-        width = 0.5
-        brange = "band_1500_2000"
-    """
-
     tsft = 1800.
     for i, (minband, maxband) in enumerate(zip(config["data"]["band_starts"], config["data"]["band_ends"])):
         if minband <= bandmin < maxband:
             stride = config["data"]["strides"][i]
             degfree = int(2 * config["data"]["n_summed_sfts"] * stride)
             width = config["data"]["band_widths"][i]
             nbin = 180#int(width*tsft)
@@ -82,16 +54,16 @@
         sfts_noise.sum_sfts()
 
         nsft = len(noise_est[0])
         tstart = sfts_noise.H1.epochs[0]
 
     else:
         noise_est = 1,1 
-        nsft = 22538
-        tstart = 931052949
+        nsft = config["data"]["nsfts"]
+        tstart = config["data"]["tstart"]
 
     # make appropriate directoes
     if not os.path.isdir(path):
         os.makedirs(path)
     erange = 15
 
     snrrange = [snr_min,snr_max]
@@ -156,15 +128,16 @@
             for key in save_options:
                 if split == "even":
                     even_noise_save_outs[key].append(noise_outputs[key])
                     even_signal_save_outs[key].append(signal_outputs[key])
                 elif split == "odd":
                     odd_noise_save_outs[key].append(noise_outputs[key])
                     odd_signal_save_outs[key].append(signal_outputs[key])
-            
+
+             
     even_noise_filenames = os.path.join(*[path,"even",brange,noise_out_snr,f"freq_{bandmin}_{bandmax}_{nperband*len(range_bands)}.hdf5"])
     even_signal_filenames = os.path.join(*[path,"even",brange,signal_out_snr,f"freq_{bandmin}_{bandmax}_{nperband*len(range_bands)}.hdf5"])
     odd_noise_filenames = os.path.join(*[path,"odd",brange,noise_out_snr,f"freq_{bandmin}_{bandmax}_{nperband*len(range_bands)}.hdf5"])
     odd_signal_filenames = os.path.join(*[path,"odd",brange,signal_out_snr,f"freq_{bandmin}_{bandmax}_{nperband*len(range_bands)}.hdf5"])
 
     for fname, temp_data in zip([even_noise_filenames, even_signal_filenames, odd_noise_filenames, odd_signal_filenames], [even_noise_save_outs, even_signal_save_outs, odd_noise_save_outs, odd_signal_save_outs]):
         if not os.path.isdir(os.path.dirname(fname)):
```

### Comparing `soapcw-0.1.5/soapcw/cnn/generate_test_data.py` & `soapcw-0.1.6/soapcw/cnn/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/soapcw/cnn/generate_train_data.py` & `soapcw-0.1.6/soapcw/cnn/generate_train_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import numpy as np
 from soapcw import cw
 import time
 import os
 import datetime
 import copy
 import pickle
+import h5py
 
 def roll_in_time(indata,numbins = 100,sh=None):
     """Roll the data in time by a given number of bins, preserving the location of the gaps
 
     Args:
         indata (2d array): input data
         numbins (int, optional): number of time bins to roll by. Defaults to 100.
@@ -81,34 +82,32 @@
         
     return data
 
 
 
 def loop_band_train_augment(
     config,
-    loadpath,
     path,
     bandmin,
     bandmax,
     band_width,
     resize_image=True,
-    nonoise=False,
+    gen_noise_only=False,
     snr_min = 50,
     snr_max=150, 
     save_options = None):
     """Loop over the data in load directory and augment to create training data
 
     Args:
-        loadpath (_type_): _description_
         path (_type_): _description_
         bandmin (_type_): _description_
         bandmax (_type_): _description_
         band_width (_type_): _description_
         resize_image (bool, optional): _description_. Defaults to True.
-        nonoise (bool, optional): _description_. Defaults to False.
+        gen_noise_only (bool, optional): _description_. Defaults to False.
         snr_min (int, optional): _description_. Defaults to 50.
         snr_max (int, optional): _description_. Defaults to 150.
         save_options (_type_, optional): _description_. Defaults to None.
     """
 
     start_time = time.time()
     tsft = 1800.
@@ -116,15 +115,15 @@
     for i, (minband, maxband) in enumerate(zip(config["data"]["band_starts"], config["data"]["band_ends"])):
         if minband <= bandmin < maxband:
             stride = config["data"]["strides"][i]
             degfree = int(2 * config["data"]["n_summed_sfts"] * stride)
             width = config["data"]["band_widths"][i]
             nbin = 180#int(width*tsft)
             plotcut = stride * nbin
-            brange = f"band_{minband:d}_{maxband:d}"
+            brange = f"band_{int(minband)}_{int(maxband)}"
             break
         else:
             continue
 
 
 
     # in 2Hz band set frequencies and indicies with 0.1 Hz bands not overlapping
@@ -133,34 +132,44 @@
     
     # set which bands are odd and even with and ondex of 1 or 0
     odd_even = np.zeros(len(range_bands))
     odd_even[1::2] = 1
 
     bl,be = bandmin,bandmax
 
-    tmin, tmax = None,None#931035615.,931035615.+1800*100
+    if config["data"]["tstart"] is not None:
+        tmin = config["data"]["tstart"]
+    else:
+        tmin = None
+    if config["data"]["tend"] is not None:
+        tmax = config["data"]["tend"]
+    else:
+        tmax = None
+
+    #tmin, tmax = None,None#931035615.,931035615.+1800*100
 
     # set integer Hz as vetos, this will cut out a few bins surrounding
     vetolist = list(np.arange(bandmin,bandmax))
 
     # find the appropriate sft files
-    hname,lname = cnn_data_gen.find_sft_file(loadpath,bandmin,bandmax)
+    hname,lname = cnn_data_gen.find_sft_file(config["general"]["narrowband_sft_dir"],bandmin,bandmax)
     
     # load in the narrowbanded sfts, normalise them, fill in the gaps and save the running median
-    sfts = cw.LoadSFT("{};{}".format(hname,lname),norm=True,filled=True,vetolist = vetolist,save_rngmed=True)
+    sfts = cw.LoadSFT("{};{}".format(hname,lname),norm=True,filled=True,vetolist = vetolist,save_rngmed=True, tmin=tmin,tmax=tmax)
+
+    print("SFTs Loaded ...")
 
     # make appropriate directoes
     if not os.path.isdir(path):
         os.makedirs(path)
     erange = 15
 
     snrrange = [snr_min,snr_max]
     noise_out_snr = "snr_0.0_0.0"
     signal_out_snr = "snr_{}_{}".format(snr_min, snr_max)
-    save_options = ["stats","paths", "pars", "powers","vit_imgs","H_imgs","L_imgs"]
 
     even_noise_filenames = {}
     even_signal_filenames = {}
     odd_noise_filenames = {}
     odd_signal_filenames = {}
 
     even_noise_save_outs = {}
@@ -172,15 +181,15 @@
         even_noise_save_outs[dirname] = []
         even_signal_save_outs[dirname] = []
         odd_noise_save_outs[dirname] = []
         odd_signal_save_outs[dirname] = []
 
     skip_list = []#config["data"]["hardware_injections"]
 
-
+    print(f"iterating over Nbands: {len(range_bands)}")
     # main loop over all sub bands
     for i in range(len(range_bands)):
         
         # set initial band frequency
         k = range_bands[i]
         # band width is 0.1 Hz
         width = 0.1
@@ -224,54 +233,94 @@
             flow = k + cts / tsft
             
             # amke copy of data so dont overwrite sft
             datah = copy.deepcopy(sfts.H1.norm_sft_power[:,cts:cte])
             datal = copy.deepcopy(sfts.L1.norm_sft_power[:,cts:cte])
             
             # run injections function with new data, this saves noise iamge and injects signal and saves signal images
-            noise_outs1, signal_outs1 = run_and_inj(datah,datal,flow,width,resize_image=resize_image,av_sh=av_sh,nonoise=nonoise,snrrange=snrrange, save_options=  save_options, stride = stride, degfree = degfree, brange = brange, sfts=sfts)
+            noise_outs1, signal_outs1 = run_and_inj(datah,datal,flow,width,resize_image=resize_image,av_sh=av_sh,gen_noise_only=gen_noise_only,snrrange=snrrange, save_options=  save_options, stride = stride, degfree = degfree, brange = brange, sfts=sfts)
             
             del datah, datal
             
             # flip data in time
         
             datah,shH = flip_data_time(copy.deepcopy(sfts.H1.norm_sft_power[:,cts:cte]),sh=av_sh[0])
             datal,shL = flip_data_time(copy.deepcopy(sfts.L1.norm_sft_power[:,cts:cte]),sh=av_sh[1])
             
-            noise_outs2, signal_outs2 = run_and_inj(datah,datal,flow,width,resize_image=resize_image,av_sh=[shH,shL],nonoise=nonoise,snrrange=snrrange, save_options=save_options, stride = stride, degfree = degfree, brange = brange,sfts=sfts)
+            noise_outs2, signal_outs2 = run_and_inj(datah,datal,flow,width,resize_image=resize_image,av_sh=[shH,shL],gen_noise_only=gen_noise_only,snrrange=snrrange, save_options=save_options, stride = stride, degfree = degfree, brange = brange,sfts=sfts)
         
             del datah,datal
         
             # flip data in freq
         
             datah = flip_data_freq(copy.deepcopy(sfts.H1.norm_sft_power[:,cts:cte]))
             datal = flip_data_freq(copy.deepcopy(sfts.L1.norm_sft_power[:,cts:cte]))
         
-            noise_outs3, signal_outs3 = run_and_inj(datah,datal,flow,width,resize_image=resize_image,av_sh=av_sh,nonoise=nonoise,snrrange=snrrange, save_options=save_options, stride = stride, degfree = degfree, brange = brange,sfts=sfts)
+            noise_outs3, signal_outs3 = run_and_inj(datah,datal,flow,width,resize_image=resize_image,av_sh=av_sh,gen_noise_only=gen_noise_only,snrrange=snrrange, save_options=save_options, stride = stride, degfree = degfree, brange = brange,sfts=sfts)
             
             del datah,datal
             
             # roll data in time by 100 bins
         
             datah,shH = roll_in_time(copy.deepcopy(sfts.H1.norm_sft_power[:,cts:cte]),numbins=100,sh=av_sh[0])
             datal,shL = roll_in_time(copy.deepcopy(sfts.L1.norm_sft_power[:,cts:cte]),numbins=100,sh=av_sh[1])
         
-            noise_outs4, signal_outs4 = run_and_inj(datah,datal,flow,width,resize_image=resize_image,av_sh=[shH,shL],nonoise=nonoise,snrrange=snrrange, save_options=save_options, stride = stride, degfree = degfree, brange = brange,sfts=sfts)
+            noise_outs4, signal_outs4 = run_and_inj(datah,datal,flow,width,resize_image=resize_image,av_sh=[shH,shL],gen_noise_only=gen_noise_only,snrrange=snrrange, save_options=save_options, stride = stride, degfree = degfree, brange = brange,sfts=sfts)
             
             del datah,datal
 
             for key in save_options:
                 if split == "even":
-                    even_noise_save_outs[key].append([noise_outs1[key],noise_outs2[key],noise_outs3[key],noise_outs4[key] ])
-                    even_signal_save_outs[key].append([signal_outs1[key],signal_outs2[key],signal_outs3[key],signal_outs4[key]])
+                    even_noise_save_outs[key].extend([noise_outs1[key],noise_outs2[key],noise_outs3[key],noise_outs4[key] ])
+                    even_signal_save_outs[key].extend([signal_outs1[key],signal_outs2[key],signal_outs3[key],signal_outs4[key]])
                 elif split == "odd":
-                    odd_noise_save_outs[key].append([noise_outs1[key],noise_outs2[key],noise_outs3[key],noise_outs4[key] ])
-                    odd_signal_save_outs[key].append([signal_outs1[key],signal_outs2[key],signal_outs3[key],signal_outs4[key]])
+                    odd_noise_save_outs[key].extend([noise_outs1[key],noise_outs2[key],noise_outs3[key],noise_outs4[key] ])
+                    odd_signal_save_outs[key].extend([signal_outs1[key],signal_outs2[key],signal_outs3[key],signal_outs4[key]])
+
+
+    print("saving data to file .......")
+
 
+    even_noise_filenames = os.path.join(*[path,"even",brange,noise_out_snr,f"freq_{bandmin}_{bandmax}_{len(shifts)*len(range_bands)}.hdf5"])
+    even_signal_filenames = os.path.join(*[path,"even",brange,signal_out_snr,f"freq_{bandmin}_{bandmax}_{len(shifts)*len(range_bands)}.hdf5"])
+    odd_noise_filenames = os.path.join(*[path,"odd",brange,noise_out_snr,f"freq_{bandmin}_{bandmax}_{len(shifts)*len(range_bands)}.hdf5"])
+    odd_signal_filenames = os.path.join(*[path,"odd",brange,signal_out_snr,f"freq_{bandmin}_{bandmax}_{len(shifts)*len(range_bands)}.hdf5"])
 
+    for fname, temp_data in zip([even_noise_filenames, even_signal_filenames, odd_noise_filenames, odd_signal_filenames], [even_noise_save_outs, even_signal_save_outs, odd_noise_save_outs, odd_signal_save_outs]):
+        if not os.path.isdir(os.path.dirname(fname)):
+            os.makedirs(os.path.dirname(fname))
+       # print(fname, save_options)
+        with h5py.File(fname,"w") as f:
+            for key in save_options:
+                if key == "pars":
+                    # pars are stored as a dictionary so have to be saved differently to hdf5
+                    try:
+                        parkeys = list(temp_data[key][0].keys())
+                    except:
+                        print(np.shape(temp_data))
+                        print("temp_datakeys", temp_data[key][0])
+                        raise Exception(f"temp data has no data: {fname}")
+                    f.create_dataset("parnames", data = parkeys)
+                    f.create_dataset("pars", data = np.array([[td[key] for key in parkeys] for td in temp_data[key]]))
+                else:
+                    try:
+                        f.create_dataset(key, shape=np.shape(temp_data[key]), data=np.array(temp_data[key]))
+                    except ValueError as e:
+                        print(key)
+                        print(len(temp_data[key]))
+                        lengths = [temp_data[key][i] for i in range(len(temp_data[key]))]
+                        print(len(temp_data[key][0]))
+                        print(max(lengths), min(lengths))
+                        #print(np.shape(temp_data[key]))
+                        #print(np.array(temp_data[key]).dtype)
+                        #print(np.array(temp_data[key]).shape)
+                        print(e)
+                        raise Exception("Error on hdf5 save array")
+
+    """
     for key in save_options:
         even_noise_filenames[key] = os.path.join(*[path,"even",key,brange,noise_out_snr,"freq_{}_{}.pkl".format(bandmin, len(even_noise_save_outs[key]))])
         even_signal_filenames[key] = os.path.join(*[path,"even",key,brange,signal_out_snr,"freq_{}_{}.pkl".format(bandmin, len(even_signal_save_outs[key]))])
         odd_noise_filenames[key] = os.path.join(*[path,"odd",key,brange,noise_out_snr,"freq_{}_{}.pkl".format(bandmin, len(odd_noise_save_outs[key]))])
         odd_signal_filenames[key] = os.path.join(*[path,"odd",key,brange,signal_out_snr,"freq_{}_{}.pkl".format(bandmin, len(odd_signal_save_outs[key]))])
     
         for fname in [even_noise_filenames[key], even_signal_filenames[key], odd_noise_filenames[key], odd_signal_filenames[key]]:
@@ -282,36 +331,36 @@
             pickle.dump(even_noise_save_outs[key], f)
         with open(odd_noise_filenames[key],"wb") as f:
             pickle.dump(odd_noise_save_outs[key], f)
         with open(even_signal_filenames[key],"wb") as f:
             pickle.dump(even_signal_save_outs[key], f)
         with open(odd_signal_filenames[key],"wb") as f:
             pickle.dump(odd_signal_save_outs[key], f)
-
+    """
 
     end_time = time.time()
     date = datetime.datetime.now().strftime("%d/%m/%Y %H:%M:%S")
     with open(os.path.join(path,"timing.txt"),"a") as f:
         f.write("time-for-gen    {}    {} \n".format(end_time-start_time,date))
 
 
 
 
-def run_and_inj(datah,datal,fmin,width,resize_image=False,snrrange = (50,150),av_sh=None,nonoise=False, save_options = None, stride = 1,degfree = 96, brange = "", sfts = None):
+def run_and_inj(datah,datal,fmin,width,resize_image=False,snrrange = (50,150),av_sh=None,gen_noise_only=False, save_options = None, stride = 1,degfree = 96, brange = "", sfts = None):
     """_summary_
 
     Args:
         datah (_type_): input hanford detector data
         datal (_type_): input livingston detector data
         fmin (_type_): minimum frequency of band [Hz]
         width (_type_): band width [Hz]
         resize_image (bool, optional): _description_. Defaults to False.
         snrrange (tuple, optional): _description_. Defaults to (50,150).
         av_sh (_type_, optional): _description_. Defaults to None.
-        nonoise (bool, optional): _description_. Defaults to False.
+        gen_noise_only (bool, optional): _description_. Defaults to False.
         save_options (_type_, optional): _description_. Defaults to None.
         stride (int, optional): _description_. Defaults to 1.
         degfree (int, optional): _description_. Defaults to 96.
         brange (str, optional): _description_. Defaults to "".
         sfts (_type_, optional): _description_. Defaults to None.
 
     Returns:
@@ -323,16 +372,16 @@
         return 0
 
     if av_sh is not None:
         Sn = {"H1":av_sh[0],"L1":av_sh[1]}
     # hardcoded start times as nsft
     nsft, tstart, tsft, flow, fhigh = sfts.H1.nsft, sfts.H1.epochs[0], 1800., fmin,fmin+width
     fmax = fmin + width
-    # not no noise means that we also generate the noise bands as well as the injected bands
-    if not nonoise: 
+    # not gen_noise_only means that we also generate the noise bands as well as the injected bands
+    if gen_noise_only: 
         # save noise realisation 1
         out_snr_noise = "snr_0.0_0.0"
         sig = cw.GenerateSignal()
         sig.alpha = 0
         sig.delta = 0
         sig.cosi = 0
         sig.phi0 = 0
@@ -345,26 +394,25 @@
         sig.fmax = fmax
         sig.tref = tstart
         
         Sn = {"H1":av_sh[0],"L1":av_sh[1]}
         data = sig.get_spectrogram(tstart = tstart, nsft = nsft,tref=tstart,tsft=tsft,fmin=fmin,fmax=fmax,snr=0,dets= ["H1","L1"],Sn=Sn)
         data.sum_sfts()
         data.downsamp_frequency(stride=stride,data_type="summed_norm_sft_power",remove_original=False)
-        pars = {}
-        pars["tref"] = tstart
-        pars["snr"] = 0
-        pars["av_sh"] = np.nanmedian(av_sh)
-        pars["h0"] = 0
-        pars["depth"] = np.inf
-        pars["fmin"] = fmin
-        pars["fmax"] = fmax
-
-        
-        noise_outs = cnn_data_gen.return_outputs(out_snr=out_snr_noise,datah=data.H1.downsamp_summed_norm_sft_power,datal=data.L1.downsamp_summed_norm_sft_power, fmin=fmin,fmax=fmax,snr=0,depth=0,h0=0, resize_image=resize_image, save_options = save_options, epochs = data.H1.summed_epochs, degfree = degfree, brange = brange, pars = pars)
 
+        noise_outputs = cnn_data_gen.return_outputs(out_snr=out_snr_noise,datah=data.H1.downsamp_summed_norm_sft_power,datal=data.L1.downsamp_summed_norm_sft_power, fmin=fmin,fmax=fmax,snr=0,depth=0,h0=0, resize_image=resize_image, save_options = save_options, epochs = data.H1.summed_epochs, degfree = degfree, brange = brange)
+        noise_outputs["pars"] = {"snr":0}
+        noise_outputs["pars"]["tref"] = tstart
+        noise_outputs["pars"]["snr"] = 0
+        noise_outputs["pars"]["h0"] = 0
+        noise_outputs["pars"]["depth"] = np.inf
+        noise_outputs["pars"]["av_sh"] = np.nanmedian(av_sh)
+        noise_outputs["pars"]["width"] = width
+        noise_outputs["pars"]["fmin"] = data.H1.fmin
+        noise_outputs["pars"]["fmax"] = data.H1.fmax
     # inject signal into band
 
     sig = cw.GenerateSignal()
     
     snrstart,snrend = snrrange[0],snrrange[1]
             
     sigfreq = np.random.uniform(0,1)*(width)*0.5 + flow + (width)*0.25
@@ -394,16 +442,16 @@
     sig.earth_ephem = "/home/joseph.bayley/repositories/lalsuite/lalpulsar/lib/earth00-40-DE430.dat.gz"
     sig.sun_ephem = "/home/joseph.bayley/repositories/lalsuite/lalpulsar/lib/sun00-40-DE430.dat.gz"
     sig.snr = snr
     sig.fmin = fmin
     sig.fmax = fmax
     sig.tref = tstart
 
-    print("MEANS",flow,fhigh)
-    print(np.mean(datah,axis=1),np.mean(datal,axis=1))
+    #print("MEANS",flow,fhigh)
+    #print(np.mean(datah,axis=1),np.mean(datal,axis=1))
             
     data = sig.get_spectrogram(tstart = tstart, nsft = len(datah),tref=tstart,tsft=tsft,fmin=flow,fmax=fhigh,snr=snr,noise_spect={"H1":datah,"L1":datal})
     data.sum_sfts()
     data.downsamp_frequency(stride=stride,data_type="summed_norm_sft_power",remove_original=False)
 
     epochs = data.H1.summed_epochs
 
@@ -418,8 +466,8 @@
     pars["depth"] = data.depth
     pars["fmin"] = fmin
     pars["fmax"] = fmax
 
     out_snr_inj = "snr_{}_{}".format(snrstart,snrend)
     signal_outs = cnn_data_gen.return_outputs(out_snr=out_snr_inj,datah=data.H1.downsamp_summed_norm_sft_power,datal=data.L1.downsamp_summed_norm_sft_power, fmin=fmin,fmax=fmax,snr=snr, depth=data.depth,h0=h0,resize_image=resize_image,pars=pars,inj_track=inj_track,epochs=epochs, save_options=save_options, degfree = degfree, brange = brange)
 
-    return noise_outs, signal_outs
+    return noise_outputs, signal_outs
```

### Comparing `soapcw-0.1.5/soapcw/cnn/narrowband_sfts.py` & `soapcw-0.1.6/soapcw/cnn/narrowband_sfts.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/soapcw/cnn/pytorch/load_models.py` & `soapcw-0.1.6/soapcw/cnn/pytorch/load_models.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/soapcw/cnn/pytorch/models/cnn.py` & `soapcw-0.1.6/soapcw/cnn/pytorch/models/cnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 import torch.nn as nn
 import numpy as np
 
 class CNN(nn.Module):
 
-    def __init__(self, input_dim, output_dim, fc_layers = [], conv_layers = [], stride = 1, device="cpu", dropout=0.1, inchannels = 1):
+    def __init__(self, input_dim, output_dim, fc_layers = [], conv_layers = [], stride = 1, device="cpu", dropout=0.1, inchannels = 1, avg_pool_size=None):
         """
         args
         ----------
         input_dim: int
             length of input time series
         latent_dim: int
             number of variables in latent space
@@ -27,14 +27,15 @@
         self.inchannels = inchannels
         
         # convolutional parts
         self.fc_layers = fc_layers
         self.conv_layers = conv_layers
         self.num_conv = len(self.conv_layers)
         self.stride = stride
+        self.avg_pool_size = avg_pool_size
 
         self.activation = nn.LeakyReLU()
         self.out_activation = nn.Sigmoid()#nn.Softmax()
         self.drop = nn.Dropout(p=dropout)
 
         self.small_const = 1e-6
         
@@ -85,16 +86,21 @@
             conv_network.add_module("pool_r_conv{}".format(i),module = maxpool)
             # define the output size of the layer
             outsize = self.conv_out_size(insize[0], insize[1], padding, dilation, filt_size, stride, maxpool_size) # output of one filter
             layer_out_sizes.append((conv_layers[i][0],outsize[0],outsize[1]))
             insize = outsize
             inchannels = conv_layers[i][0]
 
-        # define the input size to fully connected layer
-        lin_input_size = np.prod(layer_out_sizes[-1]) if num_conv > 0 else np.prod(self.input_dim)
+        if self.avg_pool_size is not None and num_conv > 0:
+            conv_network.add_module("avgpool", nn.AdaptiveAvgPool2d((self.avg_pool_size, self.avg_pool_size)))
+            lin_input_size = self.avg_pool_size*self.avg_pool_size*layer_out_sizes[-1][0]
+        else:
+            # define the input size to fully connected layer
+            lin_input_size = np.prod(layer_out_sizes[-1]) if num_conv > 0 else np.prod(self.input_dim)
+
         if append_dim:
             lin_input_size += append_dim
         layer_size = int(lin_input_size)
         # hidden layers
         for i in range(num_fc):
             lin_network.add_module("r_lin{}".format(i),module=nn.Linear(layer_size, fc_layers[i]))
             if i == num_fc - 1:
```

### Comparing `soapcw-0.1.5/soapcw/cnn/pytorch/models/combined_cnn.py` & `soapcw-0.1.6/soapcw/cnn/pytorch/models/combined_cnn.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/soapcw/cnn/train_model.py` & `soapcw-0.1.6/soapcw/cnn/train_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 import torch
 import torch.nn as nn
+import torchsummary
 import os
 import h5py
 import numpy as np
 from soapcw.cnn.pytorch import models
 import argparse
 import time
+import matplotlib.pyplot as plt
 
 class LoadData(torch.utils.data.Dataset):
 
-    def __init__(self, noise_load_directory, signal_load_directory, load_types = ["stats", "vit_imgs", "H_imgs", "L_imgs"], shuffle=True):
+    def __init__(self, noise_load_directory, signal_load_directory, load_types = ["stats", "vit_imgs", "H_imgs", "L_imgs"], shuffle=True, nfile_load="all"):
         self.load_types = load_types
         self.noise_load_directory = noise_load_directory
         self.signal_load_directory = signal_load_directory
-        self.get_filenames()
-        self.n_load_types = len(self.load_types) - 1 if "H_imgs" in self.load_types else len(self.load_types)
         self.shuffle = shuffle
+        self.nfile_load = nfile_load
+        self.get_filenames()
+        if "H_imgs" in self.load_types and "L_imgs" in self.load_types and "vit_imgs" in self.load_types:
+            self.n_load_types = len(self.load_types) - 2
+        elif "H_imgs" in self.load_types and "L_imgs" in self.load_types and "vit_imgs" not in self.load_types:
+            self.n_load_types = len(self.load_types) - 1
+        else:
+            self.n_load_types = len(self.load_types)
 
     def __len__(self,):
         return min(len(self.noise_filenames), len(self.signal_filenames))
 
     def __getitem__(self, idx):
         """_summary_
 
@@ -27,23 +35,25 @@
             idx (int): index
 
         Returns:
             _type_: data, truths arrays
         """
         noise_data, pars, pname = self.load_file(self.noise_filenames[idx])
         signal_data, pars, pname = self.load_file(self.signal_filenames[idx]) 
+        #print(self.n_load_types)
+
+        tot_data = [torch.cat([torch.Tensor(noise_data[i]).squeeze(), torch.Tensor(signal_data[i]).squeeze()], dim=0) for i in range(self.n_load_types)]
 
-        tot_data = [torch.cat([torch.Tensor(noise_data[i]), torch.Tensor(signal_data[i])], dim=0) for i in range(self.n_load_types)]
-        
         truths = torch.cat([torch.zeros(len(noise_data[0])), torch.ones(len(signal_data[0]))])
         if self.shuffle:
             shuffle_inds = np.arange(len(truths))
             np.random.shuffle(shuffle_inds)
             truths = truths[shuffle_inds]
             tot_data = [tot_data[i][shuffle_inds] for i in range(len(tot_data))]
+
         return tot_data, truths 
 
     def load_file(self, fname):
         """loads in one hdf5 containing data 
 
         Args:
             fname (string): filename
@@ -51,18 +61,21 @@
         Returns:
             _type_: data and parameters associated with files
         """
         with h5py.File(fname, "r") as f:
             output_data = []
             imgdone = False
             for data_type in self.load_types:
-                if data_type in ["H_imgs", "L_imgs"]:
+                if data_type in ["H_imgs", "L_imgs", "vit_imgs"]:
                     if imgdone:
                         continue
-                    elif data_type == "H_imgs" and "L_imgs" in self.load_types:
+                    elif "H_imgs" in self.load_types and "L_imgs" in self.load_types and "vit_imgs" in self.load_types:
+                        output_data.append(np.transpose(np.concatenate([np.expand_dims(f["H_imgs"], -1), np.expand_dims(f["L_imgs"], -1), np.expand_dims(f["vit_imgs"], -1)], axis=-1), (0,3,2,1)))
+                        imgdone = True
+                    elif "H_imgs" in self.load_types and "L_imgs" in self.load_types and "vit_imgs" not in self.load_types:
                         output_data.append(np.transpose(np.concatenate([np.expand_dims(f["H_imgs"], -1), np.expand_dims(f["L_imgs"], -1)], axis=-1), (0,3,2,1)))
                         imgdone = True
                 else:
                     output_data.append(np.array(f[data_type]))
 
             pars = np.array(f["pars"])
             parnames = list(f["parnames"])
@@ -70,55 +83,98 @@
         return output_data, pars, parnames
 
     def get_filenames(self):
 
         self.noise_filenames = [os.path.join(self.noise_load_directory, fname) for fname in os.listdir(self.noise_load_directory)]
         self.signal_filenames = [os.path.join(self.signal_load_directory, fname) for fname in os.listdir(self.signal_load_directory)]
 
+        if self.shuffle:
+            np.random.shuffle(self.noise_filenames)
+            np.random.shuffle(self.signal_filenames)
+
+        if self.nfile_load != "all":
+            self.noise_filenames = self.noise_filenames[:self.nfile_load]
+            self.signal_filenames = self.signal_filenames[:self.nfile_load]
+
 
 def train_batch(model, optimiser, loss_fn, batch_data, batch_labels, model_type="spectrogram", train=True, device="cpu"):
     model.train(train)
     if train:
         optimiser.zero_grad()
 
-    if model_type == "spectrogram":
+    if model_type in ["spectrogram", "vitmapspectrogram"]:
         output = model(torch.Tensor(batch_data[0]).to(device))
         loss = loss_fn(output.flatten(), batch_labels.to(device).flatten())
         if train:
             loss.backward()
             optimiser.step()
     
     return loss.item()
 
-def train_model(model_type, save_dir, load_dir, learning_rate, img_dim, conv_layers, fc_layers, device="cpu", load_model=None, bandtype="even", snrmin=40,snrmax=200, fmin=20,fmax=500, n_epochs=10):
+def train_model(model_type, save_dir, load_dir, learning_rate, img_dim, conv_layers, fc_layers, avg_pool_size=None, device="cpu", load_model=None, bandtype="even", snrmin=40,snrmax=200, fmin=20,fmax=500, n_epochs=10, save_interval=100):
+    """_summary_
 
+    Args:
+        model_type (_type_): _description_
+        save_dir (_type_): _description_
+        load_dir (_type_): _description_
+        learning_rate (_type_): _description_
+        img_dim (_type_): _description_
+        conv_layers (_type_): _description_
+        fc_layers (_type_): _description_
+        avg_pool_size (_type_, optional): _description_. Defaults to None.
+        device (str, optional): _description_. Defaults to "cpu".
+        load_model (_type_, optional): _description_. Defaults to None.
+        bandtype (str, optional): _description_. Defaults to "even".
+        snrmin (int, optional): _description_. Defaults to 40.
+        snrmax (int, optional): _description_. Defaults to 200.
+        fmin (int, optional): _description_. Defaults to 20.
+        fmax (int, optional): _description_. Defaults to 500.
+        n_epochs (int, optional): _description_. Defaults to 10.
+        save_interval (int, optional): _description_. Defaults to 100.
+
+    Raises:
+        Exception: _description_
+    """
+    other_bandtype = "odd" if bandtype == "even" else "even"
     train_noise_dir = os.path.join(load_dir, "train", bandtype, f"band_{fmin}_{fmax}", "snr_0.0_0.0")
     train_signal_dir = os.path.join(load_dir, "train", bandtype, f"band_{fmin}_{fmax}", f"snr_{float(snrmin)}_{float(snrmax)}")
 
-    val_noise_dir = os.path.join(load_dir, "validation", bandtype, f"band_{fmin}_{fmax}", "snr_0.0_0.0")
-    val_signal_dir = os.path.join(load_dir, "validation", bandtype, f"band_{fmin}_{fmax}", f"snr_{float(snrmin)}_{float(snrmax)}")
+    val_noise_dir = os.path.join(load_dir, "train", other_bandtype, f"band_{fmin}_{fmax}", "snr_0.0_0.0")
+    val_signal_dir = os.path.join(load_dir, "train", other_bandtype, f"band_{fmin}_{fmax}", f"snr_{float(snrmin)}_{float(snrmax)}")
 
     if model_type == "spectrogram":
         load_types = ["H_imgs", "L_imgs"]
-        model = models.cnn.CNN(input_dim=img_dim, output_dim=1, fc_layers=fc_layers, conv_layers=conv_layers, inchannels=2, device=device).to(device)
+        inchannels = 2
+        model = models.cnn.CNN(input_dim=img_dim, output_dim=1, fc_layers=fc_layers, conv_layers=conv_layers, inchannels=inchannels, avg_pool_size=avg_pool_size, device=device).to(device)
     elif model_type == "vitmap":
         load_types = ["vit_imgs"]
-        model = models.cnn.CNN(input_dim=img_dim, output_dim=1, fc_layers=fc_layers, conv_layers=conv_layers, inchannels=1, device=device).to(device)
-    elif model_type == "vitmapspect":
+        inchannels = 1
+        model = models.cnn.CNN(input_dim=img_dim, output_dim=1, fc_layers=fc_layers, conv_layers=conv_layers, inchannels=inchannels, avg_pool_size=avg_pool_size, device=device).to(device)
+    elif model_type == "vitmapspectrogram":
         load_types = ["vit_imgs", "H_imgs", "L_imgs"]
-        model = models.cnn.CNN(input_dim=img_dim, output_dim=1, fc_layers=fc_layers, conv_layers=conv_layers, inchannels=3, device=device).to(device)
-    elif model_type == "vitmapspectstat":
+        inchannels = 3
+        model = models.cnn.CNN(input_dim=img_dim, output_dim=1, fc_layers=fc_layers, conv_layers=conv_layers, inchannels=inchannels, avg_pool_size=avg_pool_size, device=device).to(device)
+    elif model_type == "vitmapspectrogramstat":
         load_types = ["vit_imgs", "H_imgs", "L_imgs", "stat"]
     else:
-        raise Exception(f"Load type {model_type} not defined select from [spectrogram, vitmap, vit_imgs, vitmapspect, vitmapspectstat]")
+        raise Exception(f"Load type {model_type} not defined select from [spectrogram, vitmap, vit_imgs, vitmapspectrogram, vitmapspectstatgram]")
+
+    print("model")
+    print(torchsummary.summary(model, (1, inchannels, img_dim[0], img_dim[1])))
 
     print("model loaded")
 
     train_dataset = LoadData(train_noise_dir, train_signal_dir, load_types=load_types)
-    validation_dataset = LoadData(val_noise_dir, val_signal_dir, load_types=load_types)
+    validation_dataset = LoadData(val_noise_dir, val_signal_dir, load_types=load_types, nfile_load=2)
+    print("Training data len: ", len(train_dataset))
+    print("Validation data len: ", len(validation_dataset))
+    trd0 = train_dataset[0]
+    print("datashape: ", [np.shape(trd0[0][i]) for i in range(len(trd0[0]))])
+    print(train_noise_dir)
     print("data loaded")
 
     optimiser = torch.optim.Adam(model.parameters(), lr = learning_rate)
     loss_fn = torch.nn.BCELoss()
 
     if load_model is not None:
         checkpoint = model.load(load_model)
@@ -129,39 +185,55 @@
     all_losses = []
     all_val_losses = []
     print("training....")
     for epoch in range(n_epochs):
 
         epoch_start = time.time()
         losses = []
-        mean_batch_time = []
+        mean_batch_time = [time.time()]
+        batch_times = [time.time()]
         for batch_data, batch_labels in train_dataset:
-            bt_start = time.time()
+            bt_start = batch_times[-1]
             loss = train_batch(model, optimiser, loss_fn, batch_data, batch_labels, device=device)    
             losses.append(loss)
-            batch_time = time.time() - bt_start
+            batch_times.append(time.time())
+            batch_time = batch_times[-1] - bt_start
             mean_batch_time.append(batch_time)
-            print(f"batch_time: {batch_time}")
+            if verbose:
+                print(f"batch_time: {batch_time}")
 
-        print(f"mean_batch_time: {np.mean(mean_batch_time)}")
+        print(f"mean_batch_time: {np.mean(batch_times)}")
         
         with torch.no_grad():
             val_losses = []
-            for batch_data, batch_labels in validation_dataset:
-                loss = train_batch(model, optimiser, loss_fn, batch_data, batch_labels, train=False, device=device)    
-                val_losses.append(loss)
+            for i, (batch_data, batch_labels) in enumerate(validation_dataset):
+                vloss = train_batch(model, optimiser, loss_fn, batch_data, batch_labels, train=False, device=device)    
+                val_losses.append(vloss)
+                if i > 10:
+                    break
         
-        all_losses.append(np.mean(losses))
-        all_val_losses.append(np.mean(val_losses))
-        print(f"Epoch: {epoch}, Loss: {np.mean(losses)} val_loss: {np.mean(val_losses)}, epoch_time: {time.time() - epoch_start}")
-        if epoch % 100 == 0:
+        mloss = np.mean(losses)
+        mvloss = np.mean(val_losses)
+        all_losses.extend(losses)
+        all_val_losses.append(mvloss)
+        print(f"Epoch: {epoch}, Loss: {mloss} val_loss: {mvloss}, epoch_time: {time.time() - epoch_start}")
+        if epoch % save_interval == 0:
             torch.save({
                 "model_state_dict": model.state_dict(),
                 "optimiser_state_dict": optimiser.state_dict(),
-            }, os.path.join(save_dir, f"model_{model_type}.pt"))
+            }, os.path.join(save_dir, f"model_{model_type}_for_{other_bandtype}.pt"))
+
+
+            fig, ax = plt.subplots()
+            ax.plot(all_losses, label="training loss")
+            ax.set_xlabel("iteration")
+            ax.set_ylabel("Loss")
+            ax.legend()
+            fig.savefig(os.path.join(save_dir, f"losses_for_{other_bandtype}.png"))
+
 
 
 def main():
     parser = argparse.ArgumentParser(description=__doc__, formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument('-v', '--verbose', help='display status', action='store_true')
     parser.add_argument("-c", "--config-file", help="config file contatining parameters")
 
@@ -173,20 +245,24 @@
         sys.exit(1)
 
     from soapcw.soap_config_parser import SOAPConfig
 
     if args.config_file is not None:
         cfg = SOAPConfig(args.config_file)
 
-    train_model(cfg["model"]["model_type"], 
-                cfg["model"]["save_dir"], 
-                cfg["general"]["save_dir"], 
-                cfg["model"]["learning_rate"], 
-                cfg["model"]["img_dim"], 
-                cfg["model"]["conv_layers"], 
-                cfg["model"]["fc_layers"],
-                n_epochs = cfg["model"]["n_epochs"],
-                device=device)
+    for bandtype in cfg["model"]["band_types"]:
+        train_model(cfg["model"]["model_type"], 
+                    cfg["model"]["save_dir"], 
+                    cfg["general"]["save_dir"], 
+                    cfg["model"]["learning_rate"], 
+                    cfg["model"]["img_dim"], 
+                    cfg["model"]["conv_layers"], 
+                    cfg["model"]["fc_layers"],
+                    avg_pool_size=cfg["model"]["avg_pool_size"],
+                    bandtype = bandtype,
+                    n_epochs = cfg["model"]["n_epochs"],
+                    device=device,
+                    save_interval=cfg["model"]["save_interval"])
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `soapcw-0.1.5/soapcw/cw/generate_data.py` & `soapcw-0.1.6/soapcw/cw/generate_data.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/soapcw/cw/load_sfts.py` & `soapcw-0.1.6/soapcw/cw/load_sfts.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/soapcw/cw/make_sfts.py` & `soapcw-0.1.6/soapcw/cw/make_sfts.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/soapcw/cw/sft.py` & `soapcw-0.1.6/soapcw/cw/sft.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/soapcw/cw/timeseries.py` & `soapcw-0.1.6/soapcw/cw/timeseries.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/soapcw/cw/tools.py` & `soapcw-0.1.6/soapcw/cw/tools.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/soapcw/line_aware_stat/gen_lookup.pyx` & `soapcw-0.1.6/soapcw/line_aware_stat/gen_lookup.pyx`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/soapcw/line_aware_stat/gen_lookup_python.py` & `soapcw-0.1.6/soapcw/line_aware_stat/gen_lookup_python.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/soapcw/line_aware_stat/save_lookup.py` & `soapcw-0.1.6/soapcw/line_aware_stat/save_lookup.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/soapcw/soap_config_parser.py` & `soapcw-0.1.6/pipeline/soap_config_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     def __init__(self, config_file):
         cfg = configparser.ConfigParser()
         cfg.read(config_file)
 
         self.config_file = os.path.abspath(config_file)
         self.float_list = ["band_starts","band_ends","band_widths"]
         self.int_list = ["strides","fc_layers","img_dim"]
-        self.string_list = ["load_directory","save_options", "type"]
+        self.string_list = ["load_directory","save_options"]
         self.tuple_list = ["conv_layers"]
         self.floats = ["band_load_size", "snr_width_line", "snr_width_signal", "prob_line", "left_right_prob", "det1_prob", "det2_prob","snrmin","snrmax","learning_rate","data_load_size"]
         self.ints = ["memory", "request_disk", "n_jobs", "n_summed_sfts","n_epochs"]
-        self.bool = ["resize_image"]
+        self.bools = ["resize_image", "overwrite_files"]
 
         self.config = self.parse_config(cfg)
 
     def __getitem__(self, key):
         return self.config[key]
 
     def load_list(self, val, partype):
@@ -61,15 +61,15 @@
                     parsed_dict[key][key2] = self.load_list(val2, "int")
                 elif key2 in self.string_list:
                     parsed_dict[key][key2] = self.load_list(val2, "string")
                 elif key2 in self.floats:
                     parsed_dict[key][key2] = float(val2)
                 elif key2 in self.ints:
                     parsed_dict[key][key2] = int(val2)
-                elif key2 in self.bool:
+                elif key2 in self.bools:
                     parsed_dict[key][key2] = self.get_bool(val2)
                 elif key2 in self.tuple_list:
                     temp_out = []
                     for mod in regex.split(r"\s*,\s*(?![^(]*\))", val2.strip("[").strip("]")):
                         if mod == "":
                             continue
                         out_tuple = tuple([int(vl) for vl in mod.strip("\n").strip("(").strip(")").split(",")])
```

### Comparing `soapcw-0.1.5/soapcw/soapcw.c` & `soapcw-0.1.6/soapcw/soapcw.c`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/soapcw/soapcw.pyx` & `soapcw-0.1.6/soapcw/soapcw.pyx`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/soapcw/tools/plots.py` & `soapcw-0.1.6/soapcw/tools/plots.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/soapcw/tools/tools.py` & `soapcw-0.1.6/soapcw/tools/tools.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/soapcw.egg-info/PKG-INFO` & `soapcw-0.1.6/soapcw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soapcw
-Version: 0.1.5
+Version: 0.1.6
 Summary: SOAP is a rapid algorithm to search for continuous sources of gravitational waves, with a wider application to long duration narrowband signals.
 Home-page: https://git.ligo.org/joseph.bayley/soapcw
 Author: Joe Bayley
 Author-email: joseph.bayley@glasgow.ac.uk
 License: MIT license
 Download-URL: https://git.ligo.org/joseph.bayley/soapcw/-/archive/0.1.2/soapcw-0.1.2.tar.gz
 Keywords: soapcw,soap,gravitational waves,pulsars,neutron stars,continuous waves
```

### Comparing `soapcw-0.1.5/soapcw.egg-info/SOURCES.txt` & `soapcw-0.1.6/soapcw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/tests/SNR_injections.ipynb` & `soapcw-0.1.6/tests/SNR_injections.ipynb`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/tests/test_cwload.py` & `soapcw-0.1.6/tests/test_cwload.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/tests/test_line_aware_stat.py` & `soapcw-0.1.6/tests/test_line_aware_stat.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.5/tests/test_soap.py` & `soapcw-0.1.6/tests/test_soap.py`

 * *Files identical despite different names*

