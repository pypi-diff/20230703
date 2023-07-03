# Comparing `tmp/vix_utils-0.1.2.tar.gz` & `tmp/vix_utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vix_utils-0.1.2.tar", last modified: Mon Mar 13 14:15:58 2023, max compression
+gzip compressed data, was "vix_utils-0.1.3.tar", last modified: Mon Jul  3 16:09:19 2023, max compression
```

## Comparing `vix_utils-0.1.2.tar` & `vix_utils-0.1.3.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0      318 2023-03-10 23:48:00.822126 vix_utils-0.1.2/.gitignore
--rw-r--r--   0        0        0     1120 2023-03-10 23:48:00.823055 vix_utils-0.1.2/.vscode/launch.json
--rw-r--r--   0        0        0      152 2023-03-10 23:48:00.823055 vix_utils-0.1.2/.vscode/settings.json
--rw-r--r--   0        0        0     1099 2023-02-18 15:43:57.735181 vix_utils-0.1.2/LICENSE
--rw-r--r--   0        0        0     2542 2023-03-10 23:48:00.824055 vix_utils-0.1.2/README.md
--rwxr-xr-x   0        0        0       39 2023-02-18 15:43:57.737182 vix_utils-0.1.2/build.cmd
--rw-r--r--   0        0        0      654 2023-02-18 15:43:57.737182 vix_utils-0.1.2/docs/Makefile
--rw-r--r--   0        0        0     1907 2023-02-18 15:43:57.738179 vix_utils-0.1.2/docs/conf.py
--rw-r--r--   0        0        0      463 2023-02-18 15:43:57.738179 vix_utils-0.1.2/docs/index.rst
--rwxr-xr-x   0        0        0      795 2023-02-18 15:43:57.739179 vix_utils-0.1.2/docs/make.bat
--rw-r--r--   0        0        0  2042633 2023-03-09 22:38:07.135739 vix_utils-0.1.2/iPath - VXX_VXZ - Pricing Supplement (November 2022).PDF
--rw-r--r--   0        0        0  2755794 2023-02-18 15:43:57.755747 vix_utils-0.1.2/iPath - VXX_VXZ - Pricing Supplement (upsize Feb 2021).pdf
--rw-r--r--   0        0        0     1500 2023-03-09 22:38:07.137738 vix_utils-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      780 2023-03-13 14:15:08.365021 vix_utils-0.1.2/src/vix_utils/__init__.py
--rw-r--r--   0        0        0  1851085 2023-03-09 22:38:07.154230 vix_utils-0.1.2/src/vix_utils/cfe-rule-book.pdf
--rw-r--r--   0        0        0     5348 2023-03-10 23:48:00.825055 vix_utils-0.1.2/src/vix_utils/continuous_maturity.py
--rw-r--r--   0        0        0     4628 2023-03-09 22:38:07.156232 vix_utils-0.1.2/src/vix_utils/data_notes.md
--rw-r--r--   0        0        0    27002 2023-03-10 23:48:00.826054 vix_utils-0.1.2/src/vix_utils/download_vix_futures.py
--rw-r--r--   0        0        0     2282 2023-03-10 23:48:00.826054 vix_utils-0.1.2/src/vix_utils/examples/sample_load_data.py
--rw-r--r--   0        0        0     3286 2023-03-10 23:48:00.827055 vix_utils-0.1.2/src/vix_utils/examples/sample_plots.py
--rw-r--r--   0        0        0        0 2023-03-09 22:38:07.159231 vix_utils-0.1.2/src/vix_utils/examples/sample_utils.py
--rw-r--r--   0        0        0     1275 2023-02-18 15:43:57.759745 vix_utils-0.1.2/src/vix_utils/futures_utils.py
--rw-r--r--   0        0        0      521 2023-03-09 22:38:07.159231 vix_utils-0.1.2/src/vix_utils/location.py
--rw-r--r--   0        0        0    28653 2023-03-09 22:38:07.160232 vix_utils-0.1.2/src/vix_utils/old_download_vix_futures.py
--rw-r--r--   0        0        0     3862 2023-03-09 22:38:07.160232 vix_utils-0.1.2/src/vix_utils/vix_cash_term_structure.py
--rw-r--r--   0        0        0    11856 2023-03-10 23:48:00.827055 vix_utils-0.1.2/src/vix_utils/vix_futures_dates.py
--rw-r--r--   0        0        0     4623 2023-03-13 14:15:08.366022 vix_utils-0.1.2/src/vix_utils/vixutil.py
--rw-r--r--   0        0        0      479 2023-02-18 15:43:57.760745 vix_utils-0.1.2/test.ps1
--rw-r--r--   0        0        0       49 2023-03-09 22:38:07.162231 vix_utils-0.1.2/test/__init__.py
--rw-r--r--   0        0        0    21050 2023-03-09 22:38:07.163231 vix_utils-0.1.2/test/data_samples/200705_200805_futures/2007-05-16.m_5.CFE_VX_K2007.csv
--rw-r--r--   0        0        0      155 2023-03-09 22:38:07.163231 vix_utils-0.1.2/test/data_samples/200705_200805_futures/2008-05-21.m_5.CFE_VX_K2008.csv
--rw-r--r--   0        0        0    35432 2023-03-09 22:38:07.164231 vix_utils-0.1.2/test/data_samples/200705_200805_futures/2008-05-21.m_5.CFE_VX_K2008_jun1_2006.csv
--rw-r--r--   0        0        0      525 2023-03-10 23:48:00.828055 vix_utils-0.1.2/test/test_monthly_settlements.py
--rw-r--r--   0        0        0     2087 2023-03-10 23:48:00.830054 vix_utils-0.1.2/test/test_monthly_tenor.py
--rw-r--r--   0        0        0     2587 2023-03-09 22:38:07.165231 vix_utils-0.1.2/test/test_read_vix_futures_history.py
--rw-r--r--   0        0        0      308 2023-03-09 22:38:07.166231 vix_utils-0.1.2/test/test_trade_and_settlement_dates.py
--rw-r--r--   0        0        0     1969 2023-03-09 22:38:07.166231 vix_utils-0.1.2/test/test_weekly_settlements.py
--rw-r--r--   0        0        0     3444 1970-01-01 00:00:00.000000 vix_utils-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      341 2023-07-03 16:07:46.288309 vix_utils-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1120 2023-03-10 23:48:00.823055 vix_utils-0.1.3/.vscode/launch.json
+-rw-r--r--   0        0        0      152 2023-03-10 23:48:00.823055 vix_utils-0.1.3/.vscode/settings.json
+-rw-r--r--   0        0        0     1099 2023-02-18 15:43:57.735181 vix_utils-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2878 2023-07-03 16:07:46.289451 vix_utils-0.1.3/README.md
+-rwxr-xr-x   0        0        0       39 2023-02-18 15:43:57.737182 vix_utils-0.1.3/build.cmd
+-rw-r--r--   0        0        0      654 2023-07-03 15:25:12.586098 vix_utils-0.1.3/docs/Makefile
+-rw-r--r--   0        0        0     1907 2023-07-03 15:25:12.587092 vix_utils-0.1.3/docs/conf.py
+-rw-r--r--   0        0        0      463 2023-07-03 15:25:12.587092 vix_utils-0.1.3/docs/index.rst
+-rwxr-xr-x   0        0        0      795 2023-07-03 15:25:12.588092 vix_utils-0.1.3/docs/make.bat
+-rw-r--r--   0        0        0  2042633 2023-03-09 22:38:07.135739 vix_utils-0.1.3/iPath - VXX_VXZ - Pricing Supplement (November 2022).PDF
+-rw-r--r--   0        0        0  2755794 2023-02-18 15:43:57.755747 vix_utils-0.1.3/iPath - VXX_VXZ - Pricing Supplement (upsize Feb 2021).pdf
+-rw-r--r--   0        0        0     1500 2023-07-03 15:25:12.588092 vix_utils-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      780 2023-07-03 16:07:46.291463 vix_utils-0.1.3/src/vix_utils/__init__.py
+-rw-r--r--   0        0        0  1851085 2023-03-09 22:38:07.154230 vix_utils-0.1.3/src/vix_utils/cfe-rule-book.pdf
+-rw-r--r--   0        0        0     5348 2023-03-10 23:48:00.825055 vix_utils-0.1.3/src/vix_utils/continuous_maturity.py
+-rw-r--r--   0        0        0     4628 2023-03-09 22:38:07.156232 vix_utils-0.1.3/src/vix_utils/data_notes.md
+-rw-r--r--   0        0        0    27002 2023-03-10 23:48:00.826054 vix_utils-0.1.3/src/vix_utils/download_vix_futures.py
+-rw-r--r--   0        0        0     2282 2023-03-10 23:48:00.826054 vix_utils-0.1.3/src/vix_utils/examples/sample_load_data.py
+-rw-r--r--   0        0        0     3231 2023-07-03 15:25:12.589092 vix_utils-0.1.3/src/vix_utils/examples/sample_plots.py
+-rw-r--r--   0        0        0        0 2023-03-09 22:38:07.159231 vix_utils-0.1.3/src/vix_utils/examples/sample_utils.py
+-rw-r--r--   0        0        0   218666 2023-07-03 16:05:53.634326 vix_utils-0.1.3/src/vix_utils/examples/vix_utils use in Jupyter.ipynb
+-rw-r--r--   0        0        0     1275 2023-02-18 15:43:57.759745 vix_utils-0.1.3/src/vix_utils/futures_utils.py
+-rw-r--r--   0        0        0      521 2023-03-09 22:38:07.159231 vix_utils-0.1.3/src/vix_utils/location.py
+-rw-r--r--   0        0        0    28653 2023-03-09 22:38:07.160232 vix_utils-0.1.3/src/vix_utils/old_download_vix_futures.py
+-rw-r--r--   0        0        0     3862 2023-03-09 22:38:07.160232 vix_utils-0.1.3/src/vix_utils/vix_cash_term_structure.py
+-rw-r--r--   0        0        0    11856 2023-03-10 23:48:00.827055 vix_utils-0.1.3/src/vix_utils/vix_futures_dates.py
+-rw-r--r--   0        0        0     4623 2023-03-13 14:15:08.366022 vix_utils-0.1.3/src/vix_utils/vixutil.py
+-rw-r--r--   0        0        0      479 2023-02-18 15:43:57.760745 vix_utils-0.1.3/test.ps1
+-rw-r--r--   0        0        0       49 2023-03-09 22:38:07.162231 vix_utils-0.1.3/test/__init__.py
+-rw-r--r--   0        0        0    21050 2023-03-09 22:38:07.163231 vix_utils-0.1.3/test/data_samples/200705_200805_futures/2007-05-16.m_5.CFE_VX_K2007.csv
+-rw-r--r--   0        0        0      155 2023-03-09 22:38:07.163231 vix_utils-0.1.3/test/data_samples/200705_200805_futures/2008-05-21.m_5.CFE_VX_K2008.csv
+-rw-r--r--   0        0        0    35432 2023-03-09 22:38:07.164231 vix_utils-0.1.3/test/data_samples/200705_200805_futures/2008-05-21.m_5.CFE_VX_K2008_jun1_2006.csv
+-rw-r--r--   0        0        0      525 2023-03-10 23:48:00.828055 vix_utils-0.1.3/test/test_monthly_settlements.py
+-rw-r--r--   0        0        0     2087 2023-03-10 23:48:00.830054 vix_utils-0.1.3/test/test_monthly_tenor.py
+-rw-r--r--   0        0        0     2587 2023-03-09 22:38:07.165231 vix_utils-0.1.3/test/test_read_vix_futures_history.py
+-rw-r--r--   0        0        0      308 2023-03-09 22:38:07.166231 vix_utils-0.1.3/test/test_trade_and_settlement_dates.py
+-rw-r--r--   0        0        0     1969 2023-03-09 22:38:07.166231 vix_utils-0.1.3/test/test_weekly_settlements.py
+-rw-r--r--   0        0        0     3775 1970-01-01 00:00:00.000000 vix_utils-0.1.3/PKG-INFO
```

### Comparing `vix_utils-0.1.2/.vscode/launch.json` & `vix_utils-0.1.3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/LICENSE` & `vix_utils-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/README.md` & `vix_utils-0.1.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 Vix Cash Data are downloaded from [CBOE Historical Volatility Indexes](https://www.cboe.com/tradable_products/vix/vix_historical_data/).
 
 
 There is an API for Python to load the data into Pandas DataFrames.  If you do your analysis in Python, use the API.
 
 Since there is no documentation yet, look at the examples in the src/vix_utils/examples folder.
 
+*Important note for Juypter notebooks.*  
+You must use  async_get_vix_index_histories and async_load_vix_term_structure 
+rather than get_vix_index_histories and load_vix_term_structure.  There is an example Jupyter notebook "vix_utils use in Jupyter.ipynb" in the src/vix_utils/examples folder. 
+ 
 If you do your analysis in other tools such as R or excel, you can use the command line tool vixutil.
 
 `vixutil -h` will give the help.  The data are availble in record and wide formats.  Just run it and look at the excel or csv output to see what they look like.
 
  
 
 
@@ -36,15 +40,16 @@
 
 The sample to load all the various data frames can be run as:
 'vix_sample_load_data'
 
 The sample to plot the history of futures and cash term structures:
 `vix_sample_plots`
 
-When you run the samples, they will print out the Python script file names so you can find them wherever pip installs them.
+To load the sample Jupyter notebook, run vix_sample_load_data to figure out where the examples folder is. Browse there with Jupyter and open a notebook.   
+
 
 ### Development 
 
 Clone from  [github repository](https://github.com/dougransom/vix_utils).
 
  
 `pip install -e .[test,examples]` will:
```

### Comparing `vix_utils-0.1.2/docs/Makefile` & `vix_utils-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/docs/conf.py` & `vix_utils-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/docs/make.bat` & `vix_utils-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/iPath - VXX_VXZ - Pricing Supplement (November 2022).PDF` & `vix_utils-0.1.3/iPath - VXX_VXZ - Pricing Supplement (November 2022).PDF`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/iPath - VXX_VXZ - Pricing Supplement (upsize Feb 2021).pdf` & `vix_utils-0.1.3/iPath - VXX_VXZ - Pricing Supplement (upsize Feb 2021).pdf`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/pyproject.toml` & `vix_utils-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/src/vix_utils/__init__.py` & `vix_utils-0.1.3/src/vix_utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 A library for preparing   VIX Futures and Cash Term Structures for analysis,
 including a  continuous maturity VIX Futures term structure.
 """
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 
 from .download_vix_futures import  \
 pivot_futures_on_monthly_tenor,select_monthly_futures,async_load_vix_term_structure,load_vix_term_structure
 
 from .vix_cash_term_structure import \
     async_get_vix_index_histories,  \
     get_vix_index_histories,    \
```

### Comparing `vix_utils-0.1.2/src/vix_utils/cfe-rule-book.pdf` & `vix_utils-0.1.3/src/vix_utils/cfe-rule-book.pdf`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/src/vix_utils/continuous_maturity.py` & `vix_utils-0.1.3/src/vix_utils/continuous_maturity.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/src/vix_utils/data_notes.md` & `vix_utils-0.1.3/src/vix_utils/data_notes.md`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/src/vix_utils/download_vix_futures.py` & `vix_utils-0.1.3/src/vix_utils/download_vix_futures.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/src/vix_utils/examples/sample_load_data.py` & `vix_utils-0.1.3/src/vix_utils/examples/sample_load_data.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/src/vix_utils/examples/sample_plots.py` & `vix_utils-0.1.3/src/vix_utils/examples/sample_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """
 Example use of vixutil to plot the term structure.
-Be sure to run vixutil -r first to download the data.
 """
 import vix_utils 
 import pandas as pd
 import logging  
 import asyncio
 import sys
 import matplotlib.pyplot as plt
```

### Comparing `vix_utils-0.1.2/src/vix_utils/futures_utils.py` & `vix_utils-0.1.3/src/vix_utils/futures_utils.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/src/vix_utils/location.py` & `vix_utils-0.1.3/src/vix_utils/location.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/src/vix_utils/old_download_vix_futures.py` & `vix_utils-0.1.3/src/vix_utils/old_download_vix_futures.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/src/vix_utils/vix_cash_term_structure.py` & `vix_utils-0.1.3/src/vix_utils/vix_cash_term_structure.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/src/vix_utils/vix_futures_dates.py` & `vix_utils-0.1.3/src/vix_utils/vix_futures_dates.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/src/vix_utils/vixutil.py` & `vix_utils-0.1.3/src/vix_utils/vixutil.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/test/data_samples/200705_200805_futures/2007-05-16.m_5.CFE_VX_K2007.csv` & `vix_utils-0.1.3/test/data_samples/200705_200805_futures/2007-05-16.m_5.CFE_VX_K2007.csv`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/test/data_samples/200705_200805_futures/2008-05-21.m_5.CFE_VX_K2008_jun1_2006.csv` & `vix_utils-0.1.3/test/data_samples/200705_200805_futures/2008-05-21.m_5.CFE_VX_K2008_jun1_2006.csv`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/test/test_monthly_settlements.py` & `vix_utils-0.1.3/test/test_monthly_settlements.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/test/test_monthly_tenor.py` & `vix_utils-0.1.3/test/test_monthly_tenor.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/test/test_read_vix_futures_history.py` & `vix_utils-0.1.3/test/test_read_vix_futures_history.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/test/test_weekly_settlements.py` & `vix_utils-0.1.3/test/test_weekly_settlements.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.2/PKG-INFO` & `vix_utils-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vix_utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: Provide VIX Cash and Futures Term Structure as Pandas dataframes
 Keywords: vix,volatility,pandas,vix term structure,cboe
 Author-email: Doug Ransom <doug@ransom.vip>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
@@ -37,14 +37,18 @@
 Vix Cash Data are downloaded from [CBOE Historical Volatility Indexes](https://www.cboe.com/tradable_products/vix/vix_historical_data/).
 
 
 There is an API for Python to load the data into Pandas DataFrames.  If you do your analysis in Python, use the API.
 
 Since there is no documentation yet, look at the examples in the src/vix_utils/examples folder.
 
+*Important note for Juypter notebooks.*  
+You must use  async_get_vix_index_histories and async_load_vix_term_structure 
+rather than get_vix_index_histories and load_vix_term_structure.  There is an example Jupyter notebook "vix_utils use in Jupyter.ipynb" in the src/vix_utils/examples folder. 
+ 
 If you do your analysis in other tools such as R or excel, you can use the command line tool vixutil.
 
 `vixutil -h` will give the help.  The data are availble in record and wide formats.  Just run it and look at the excel or csv output to see what they look like.
 
  
 
 
@@ -63,15 +67,16 @@
 
 The sample to load all the various data frames can be run as:
 'vix_sample_load_data'
 
 The sample to plot the history of futures and cash term structures:
 `vix_sample_plots`
 
-When you run the samples, they will print out the Python script file names so you can find them wherever pip installs them.
+To load the sample Jupyter notebook, run vix_sample_load_data to figure out where the examples folder is. Browse there with Jupyter and open a notebook.   
+
 
 ### Development 
 
 Clone from  [github repository](https://github.com/dougransom/vix_utils).
 
  
 `pip install -e .[test,examples]` will:
```

