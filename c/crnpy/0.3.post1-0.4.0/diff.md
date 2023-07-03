# Comparing `tmp/crnpy-0.3.post1.tar.gz` & `tmp/crnpy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crnpy-0.3.post1.tar", last modified: Fri Jun 16 23:49:30 2023, max compression
+gzip compressed data, was "crnpy-0.4.0.tar", last modified: Mon Jul  3 20:15:16 2023, max compression
```

## Comparing `crnpy-0.3.post1.tar` & `crnpy-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:49:30.905187 crnpy-0.3.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-16 23:49:21.000000 crnpy-0.3.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-16 23:49:30.905187 crnpy-0.3.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-16 23:49:21.000000 crnpy-0.3.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 23:49:30.905187 crnpy-0.3.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-16 23:49:21.000000 crnpy-0.3.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:49:30.901188 crnpy-0.3.post1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:49:30.905187 crnpy-0.3.post1/src/crnpy/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-16 23:49:21.000000 crnpy-0.3.post1/src/crnpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53443 2023-06-16 23:49:21.000000 crnpy-0.3.post1/src/crnpy/crnpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-06-16 23:49:21.000000 crnpy-0.3.post1/src/crnpy/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:49:30.905187 crnpy-0.3.post1/src/crnpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-16 23:49:30.000000 crnpy-0.3.post1/src/crnpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-16 23:49:30.000000 crnpy-0.3.post1/src/crnpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 23:49:30.000000 crnpy-0.3.post1/src/crnpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 23:49:30.000000 crnpy-0.3.post1/src/crnpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:15:16.219850 crnpy-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-03 20:15:05.000000 crnpy-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-03 20:15:16.219850 crnpy-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-03 20:15:05.000000 crnpy-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 20:15:16.219850 crnpy-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-03 20:15:05.000000 crnpy-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:15:16.215850 crnpy-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:15:16.215850 crnpy-0.4.0/src/crnpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-03 20:15:05.000000 crnpy-0.4.0/src/crnpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58185 2023-07-03 20:15:05.000000 crnpy-0.4.0/src/crnpy/crnpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-07-03 20:15:05.000000 crnpy-0.4.0/src/crnpy/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:15:16.219850 crnpy-0.4.0/src/crnpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-03 20:15:16.000000 crnpy-0.4.0/src/crnpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-03 20:15:16.000000 crnpy-0.4.0/src/crnpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:15:16.000000 crnpy-0.4.0/src/crnpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 20:15:16.000000 crnpy-0.4.0/src/crnpy.egg-info/top_level.txt
```

### Comparing `crnpy-0.3.post1/LICENSE` & `crnpy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crnpy-0.3.post1/README.md` & `crnpy-0.4.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,40 @@
+[![GitHub Workflow Status (building)](https://img.shields.io/github/actions/workflow/status/soilwater/crnpy/python-package.yml)](https://github.com/soilwater/crnpy/actions/workflows/python-package.yml)
+[![GitHub Workflow Status (publish)](https://img.shields.io/github/actions/workflow/status/soilwater/crnpy/python-publish.yml?label=publish)](https://github.com/soilwater/crnpy/actions/workflows/python-publish.yml)
+[![PyPI - Status](https://img.shields.io/pypi/v/crnpy)](https://pypi.org/project/crnpy/)
+[![GitHub commits since latest release (by SemVer including pre-releases)](https://img.shields.io/github/commits-since/soilwater/crnpy/latest/main)](https://github.com/soilwater/crnpy)
+
 # Cosmic-Ray Neutron Python (CRNPy) Library
 
-<img src="/docs/img/logo/crnpy-logo.png" alt="CRNPY logo" width="250"/>
+<img src="https://raw.githubusercontent.com/soilwater/crnpy/main/docs/img/logo/crnpy-logo.png" alt="CRNPY logo" width="250"/>
 
 ## Overview
 
 Welcome to the homepage of the CRNPy (Cosmic-Ray Neutron Python) library, an open-source Python library designed for the processing and conversion of raw neutron counts from Cosmic-Ray Neutron Probes (CRNP) into accurate field-level soil moisture data.
 
 This library has been developed with the intent of providing a comprehensive yet easy-to-use workflow for processing raw data from a variety of CRNP, encompassing multiple manufacturers and models.
 
 ## Key Features
 - Versatility: CRNPy can handle data from various CRNP manufacturers and models. It has been successfully tested on both roving and stationary CRNP.
 - Modularity: The library is designed to be modular, allowing users to easily customize the processing workflow to their needs.
-- Accuracy: The library shows excellent agreement with ground-based measurements, making it a reliable tool for scientific research and practical applications.
-- Correction Routines: The correction functions of the library have been effectively used to represent field and watershed scale soil moisture conditions.
+- Instrument agnostic: It can be used with any CRNP, allowing users to process data from multiple instruments with their own workflow.
 
-![CRNPy Processing Workflow](docs/img/workflow.png)
+![CRNPy Processing Workflow](https://raw.githubusercontent.com/soilwater/crnpy/main/docs/img/workflow.png)
 Overview of the proposed CRNPy processing workflow. Final user can choose to use the entire workflow, part of it, or build functions on top of it depending on their needs, dashed lines indicate optional steps.
 
 
 ## Installation
 
 To install the CRNPy library, you can use Python's package manager, pip. Simply open your command line or terminal and type:
 
 ```pip install crnpy```
 
 ## Authors
-The CRNPy library was conceived and developed by Joaquin Peraza and Andres Patrignani in the Soil Water Processes Lab at Kansas State University. The team's passion for making soil moisture data more accessible and easier to process culminated in this powerful tool.
 
-The Soil Water Processes Lab at Kansas State University is a leading research group focused on understanding and modeling soil water processes. The lab combines a range of experimental and computational approaches to tackle some of the most pressing issues in soil and water research. The development of the CRNPy library is a testament to the lab's commitment to pushing the boundaries of soil science through the innovative use of technology. like to acknowledge the contributions of the wider scientific community in testing and providing feedback on the library, which has been instrumental in its ongoing development.
+The CRNPy library was developed by:
+
+- Joaquin Peraza
+- Andres Patrignani
+
+in the Soil Water Processes Lab at Kansas State University. The team's passion for making soil moisture data more accessible and easier to process culminated in this powerful tool.
+
+The Soil Water Processes Lab at Kansas State University is a leading research group focused on understanding and modeling soil water processes. The lab combines a range of experimental and computational approaches to tackle some of the most pressing issues in soil and water research. The development of the CRNPy library is a testament to the lab's commitment to pushing the boundaries of soil science through the innovative use of technology. The authors would like to acknowledge the contributions of the wider scientific community in testing and providing feedback on the library, which has been instrumental in its ongoing development.
```

### Comparing `crnpy-0.3.post1/src/crnpy/crnpy.py` & `crnpy-0.4.0/src/crnpy/crnpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 # produce an error message if the python version is less than required
 if sys.version_info < python_version:
     msg = "Module only runs on python version >= %s" % python_version_str
     raise Exception(msg)
 
 
-def format_dates_df(df, col='timestamp', format='%Y-%m-%d %H:%M:%S', freq='H', round_time=True):
+def fill_missing_timestamps(df, col='timestamp', format='%Y-%m-%d %H:%M:%S', freq='H', round_time=True):
     """Helper function to change the format and round timestamps.
 
      Args:
          df (pandas.DataFrame): DataFrame with timestamp in the index.
          col (str, optional): Column with the timestamp. Default is 'timestamp'.
          format (str, optional): Format of the timestamp. Default is '%Y-%m-%d %H:%M:%S'.
          freq (str, optional): Rounding interval. 'H' for hourly, 'M' for minute, or None. Default is 'H'.
@@ -70,48 +70,61 @@
             source = pd.concat([df,new_line])
 
     df.sort_values(by=col, inplace=True)
     df.reset_index(drop=True, inplace=True)
     df.set_index(col, inplace=True)
     return df
 
-def count_time(df):
+def count_time(counts=None, timestamp_col=None):
     """Approximate counting time.
 
     Args:
-        df (pandas.DataFrame): Dataframe containing only the columns with neutron counts and timestamp in the index.
+        counts (pandas.DataFrame): DataFrame with neutron counts, might have DateTimeIndex.
+        timestamp_col (pandas.Series): Series with timestamps. If counts has a DateTimeIndex, timestamp_col is not needed.
 
     Returns:
-        (pandas.DataFrame): Dataframe with the approximate counting time for each observation.
+        (pandas.Series): Series with the approximate counting time for each observation.
 
     Examples:
         Using `count_time` in a console environment:
 
         >>> df = pd.DataFrame(...)
-        >>> count_time(df)
+        >>> count_time(timestamp_col=df['timestamp'])
         0   3600.0
         1   3600.0
         2   3600.0
     """
+    if timestamp_col is not None:
+        if not isinstance(timestamp_col, pd.Series):
+            raise TypeError('timestamp_col must be a pandas Series.')
+        if timestamp_col.dtype != 'datetime64[ns]':
+            raise TypeError('timestamp_col must be a pandas Series with datetime64[ns] dtype.')
 
-    # Check that index is a timestamp
-    if type(df.index) != pd.core.indexes.datetimes.DatetimeIndex:
-        raise ValueError('Index must be a timestamp.')
+        count_time = timestamp_col.diff().dt.total_seconds()
+        return count_time
 
-    # Calculate time difference between rows
-    count_time = df.index.to_series().diff().dt.total_seconds()
+    if counts is not None:
+        if not isinstance(counts, pd.DataFrame):
+            raise TypeError('counts must be a pandas DataFrame.')
 
-    return count_time
+        if not counts.index.dtype == 'datetime64[ns]':
+            raise TypeError('counts must have a DateTimeIndex.')
 
-def fill_counts(counts, count_times=None, expected_time=False, threshold=0.25, limit=3):
+        count_time = counts.index.to_series().diff().dt.total_seconds()
+        return count_time
+
+    raise TypeError('Either counts or timestamp_col must be provided.')
+
+def fill_counts(counts, count_times=None, timestamp_col=None, expected_time=False, threshold=0.25, limit=3):
     """Fill missing neutron counts. Observation periods shorter than threshold are discarded (replaced with NaN).
     
     Args:
-        counts (pandas.DataFrame): DataFrame with neutron counts, might have count_time column(s).
-        count_time (pandas.Series or pandas.DataFrame): Counting time in seconds. If a DataFrame is provided, it must have the same number of columns as df.
+        counts (pandas.DataFrame): DataFrame with neutron counts, might have DateTimeIndex.
+        count_time (pandas.Series or pandas.DataFrame): Counting time in seconds. If a DataFrame is provided, it must have the same number of columns as `counts`.
+        timestamp_col (pandas.Series): Series with timestamps. If counts has a DateTimeIndex, timestamp_col is not needed.
         expected_time (int): Expected counting time in seconds. If not provided, it is calculated as the median of the counting times.
         threshold (float): Minimum fraction of the neutron integration time. Default is 0.25.
 
     Returns:
         (pandas.DataFrame): DataFrame with linearly interpolated neutron counts.
 
     Examples:
@@ -125,18 +138,27 @@
         3   102.0
     """
 
     counts=counts.copy()
 
     if type(counts.index) == pd.core.indexes.datetimes.DatetimeIndex and isinstance(count_times, type(None)):
         print("No count time columns provided. Using timestamp index to compute count time.")
-        count_times = counts.index.to_series().diff().dt.total_seconds()
+        count_times = count_time(timestamp_col=counts.index.to_series())
 
-    if type(counts.index) != pd.core.indexes.datetimes.DatetimeIndex and isinstance(count_times, type(None)):
-        raise ValueError('Index must be a timestamp or count times must be provided.')
+    elif not isinstance(timestamp_col, type(None)) and isinstance(count_times, type(None)):
+        if timestamp_col.dtype != 'datetime64[ns]':
+            if len(timestamp_col) != len(counts):
+                raise ValueError('Timestamp column length does not match number of readings.')
+            print("No count time columns provided. Using timestamp column to compute count time.")
+            count_times = count_time(timestamp_col=timestamp_col)
+        else:
+            raise TypeError('Timestamp column must be a pandas Series with datetime64[ns] dtype.')
+
+    if type(counts.index) != pd.core.indexes.datetimes.DatetimeIndex and isinstance(count_times, type(None)) and isinstance(timestamp_col, type(None)):
+        raise ValueError('Count_times must be provided, or timestamp_col must be provided, or counts must have a DatetimeIndex.')
 
     if len(counts) != len(count_times):
         raise ValueError('Count times length does not match number of readings.')
 
     if expected_time is False:
         expected_time = count_times.median()
         print('Using median count time as expected count time:', expected_time)
@@ -159,70 +181,84 @@
         idx_nan = np.where(count_times < time_threshold)
         counts.loc[idx_nan] = np.nan
 
     # Fill missing values with linear interpolation and round to nearest integer
     counts = counts.interpolate(method='linear', limit=limit, limit_direction='both').round()
     return counts
 
-def normalize_counts(counts, count_time=3600, count_times=None):
+def adjust_temporal_counts(counts, count_time=3600, count_times=None, timestamp_col=None):
     """Normalize neutron counts to the desired counting time.
     
     Args:
         counts (pandas.DataFrame): Dataframe containing only the columns with neutron counts.
         count_time (int): Count time in seconds for normalization. Default is 3600 seconds.
-        count_times (pandas.Series or pandas.DataFrame): Counting time in seconds. If a DataFrame is provided, it must have the same number of columns as df.
+        count_times (pandas.Series or pandas.DataFrame): Counting time in seconds. If a DataFrame is provided, it must have the same number of columns as counts.
+        timestamp_col (pandas.Series): Timestamp column, used to calculate count time if count_times is not provided, it must have the same number of rows as counts.
         
     Returns:
         (pandas.DataFrame): Normalized neutron counts.
 
     """
 
     if count_times is None and type(counts.index) == pd.core.indexes.datetimes.DatetimeIndex:
         print("No count_times columns provided. Using timestamp index to compute count time.")
         count_times = counts.index.to_series().diff().dt.total_seconds()
 
+    elif count_times is None and not isinstance(timestamp_col, type(None)):
+        if len(timestamp_col) != len(counts):
+            raise ValueError('Timestamp column length does not match number of readings.')
+        print("No count_times columns provided. Using timestamp column to compute count time.")
+        if timestamp_col.dtype != 'datetime64[ns]':
+            raise TypeError('Timestamp column must be a pandas Series with datetime64[ns] dtype.')
+        count_times = count_time(timestamp_col=timestamp_col)
+
+
     if isinstance(count_times, type(None)):
-        raise ValueError('Count time must be provided or index must be a timestamp.')
+        raise ValueError('Count time must be provided, or `timestamp_col` must be provided, or counts must have a DatetimeIndex.')
 
     if len(counts) != len(count_times):
         raise ValueError('Count times length does not match number of readings.')
 
-
     #Normalize counts rounded to integer
     if type(count_times) == pd.core.series.Series or len(count_times.columns) == 1:
         normalized_counts = counts.div(count_times, axis=0).mul(count_time).round()
         return normalized_counts
     else:
         normalized_counts = counts.copy()
         count_times = count_times.copy()
         for i in range(len(count_times.columns)):
             normalized_counts[normalized_counts.columns[i]] = normalized_counts.iloc[:,i].div(count_times.iloc[:,i], axis=0).mul(count_time).round()
         return normalized_counts
 
 
-
-def compute_total_raw_counts(counts, nan_strategy=None):
+def compute_total_raw_counts(counts, nan_strategy=None, timestamp_col=None):
     """Compute the sum of uncorrected neutron counts for all detectors.
 
     Args:
         counts (pandas.DataFrame): Dataframe containing only the columns with neutron counts.
         nan_strategy (str): Strategy to use for NaN values. Options are 'interpolate', 'average', or None. Default is None.
 
     Returns:
         (pandas.DataFrame): Dataframe with the sum of uncorrected neutron counts for all detectors.
     """
+
     counts=counts.copy()
 
     if counts.isnull().values.any():
         if nan_strategy is None:
             raise ValueError('NaN values found. Please fill missing values or provide a strategy. See documentation for more information.')
         elif nan_strategy == 'interpolate':
             print('NaN values found. Interpolating missing values using fill_counts().')
-            if type(counts.index) != pd.core.indexes.datetimes.DatetimeIndex:
-                raise ValueError('Index must be a timestamp to use interpolation strategy.')
+            if not isinstance(timestamp_col, type(None)):
+                if type(timestamp_col) != pd.core.series.Series:
+                    if timestamp_col.dtype != 'datetime64[ns]':
+                        raise TypeError('Timestamp column must be a pandas Series with datetime64[ns] dtype.')
+                counts = fill_counts(counts, timestamp_col)
+            elif type(counts.index) != pd.core.indexes.datetimes.DatetimeIndex:
+                raise ValueError('`timestamp_col` must be provided if `counts` does not have a DatetimeIndex.')
             counts = fill_counts(counts)
         elif nan_strategy == 'average':
             if len(counts.columns) == 1:
                 raise ValueError('Only one detector found. Cannot use average strategy.')
             print('NaN values found. Replacing missing values with average of other detectors before summing.')
             counts = counts.apply(lambda x: x.fillna(counts.mean(axis=1)),axis=0)
         else:
@@ -250,15 +286,14 @@
         or
         (pandas.DataFrame, pandas.DataFrame): Dataframe without outliers and dataframe with outliers.
 
     References:
         Iglewicz, B. and Hoaglin, D.C., 1993. How to detect and handle outliers (Vol. 16). Asq Press.
     """
 
-
     if min_counts is not None:
         lower_count = np.sum(raw_counts < min_counts)
         if lower_count > len(raw_counts) * 0.25:
             print(f"WARNING: Discarded {lower_count} counts below {min_counts}. This is more than 25% of the total number of readings. Consider increasing the minimum counts threshold.")
         else:
             print(f"Discarded counts below {min_counts}: {lower_count}")
         raw_counts = raw_counts[raw_counts >= min_counts]
@@ -300,81 +335,149 @@
     References:
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.interpolate.html
     """
 
     # Fill missing values in atmospheric variables
     return cols_atm.interpolate(method='pchip', limit=limit, limit_direction='both')
 
-def atm_correction(raw_counts, pressure, humidity, temp, Pref, Aref, L, incoming_neutrons=None, incoming_Ref=None):
-    r"""Correct neutron counts for atmospheric factors and incoming neutron flux.
 
-    This function corrects neutron counts for atmospheric pressure, and absolute humidity using the method described in Zreda et al. (2012) and Anderson et al. (2017). The correction is performed using the following equation:
+def pressure_correction(raw_counts, pressure, Pref, L):
+    r"""Correct neutron counts for atmospheric pressure.
+
+    This function corrects neutron counts for atmospheric pressure using the method described in Andreasen et al. (2017).
+    The correction is performed using the following equation:
 
     $$
-    C_{corrected} = \frac{C_{raw} \cdot f_w}{f_p \cdot f_i}
+    C_{corrected} = \frac{C_{raw}}{fp}
     $$
 
+    where:
+
+    - Ccorrected: corrected neutron counts
+    - Craw: raw neutron counts
     - fp: pressure correction factor
-    - fw: abosolute humidity correction factor
-    - fi: incoming neutron flux correction factor
-    
+
+    $$
+    fp = e^{\frac{P_{ref} - P}{L}}
+    $$
+
+    where:
+
+    - P: atmospheric pressure
+    - Pref: reference atmospheric pressure
+    - L: Atmospheric attenuation coefficient.
+
+
     Args:
         raw_counts (list or array): Neutron counts to correct.
-        pressure (list or array): Atmospheric pressure readings.
-        humidity (list or array): Atmospheric humidity readings in %.
-        temp (list or array): Atmospheric temperature readings in Celsius.
-        Pref (float): Reference atmospheric pressure in millibars (mbar).
-        Aref (float): Reference absolute humidity.
+        pressure (list or array): Atmospheric pressure readings. Long-term average pressure is recommended.
+        Pref (float): Reference atmospheric pressure.
         L (float): Atmospheric attenuation coefficient.
-        incoming_neutrons (list or array): Incoming neutron flux. Default is None.
-        incoming_Ref (float): Reference incoming neutron flux. Default is None.
-        
+
     Returns:
-        (numpy.array): Total neutron counts corrected by atmospheric conditions.
-        
-    References:
-        Zreda, M., Shuttleworth, W. J., Zeng, X., Zweck, C., Desilets, D., Franz, T., et al. (2012).
-        COSMOS: the cosmic-ray soil moisture observing system. Hydrol. Earth Syst. Sci. 16, 4079–4099.
-        doi: 10.5194/hess-16-4079-2012
+        (list): Corrected neutron counts.
 
-        Andreasen, M., Jensen, K.H., Desilets, D., Franz, T.E., Zreda, M., Bogena, H.R. and Looms, M.C., 2017.
-        Status and perspectives on the cosmic‐ray neutron method for soil moisture estimation and other
-        environmental science applications. Vadose zone journal, 16(8), pp.1-11. doi.org/10.2136/vzj2017.04.0086
+    References:
+        M. Andreasen, K.H. Jensen, D. Desilets, T.E. Franz, M. Zreda, H.R. Bogena, and M.C. Looms. 2017. Status and perspectives on the cosmic-ray neutron method for soil moisture estimation and other environmental science applications. Vadose Zone J. 16(8). doi:10.2136/vzj2017.04.0086
     """
 
-    ### Barometric pressure factor
+    # Compute pressure correction factor
     fp = np.exp((Pref - pressure) / L) # Zreda et al. 2017 Eq 5.
+    # Compute corrected neutron counts
+    corrected_counts = raw_counts / fp
+    return np.round(corrected_counts)
 
-    ### Atmospheric water vapor factor
-    # Saturation vapor pressure
-    e_sat = 0.611 * np.exp(17.502 * temp / (temp + 240.97)) * 1000 # in Pascals Eq. 3.8 p.41 Environmental Biophysics (Campbell and Norman)
 
-    # Vapor pressure Pascals
-    Pw = e_sat * humidity/100
+def humidity_correction(raw_counts, humidity, temp, Aref):
+    r"""Correct neutron counts for absolute humidity.
 
-    # Absolute humidity (g/m^3)
-    C = 2.16679 # g K/J;
-    A = C * Pw / (temp + 273.15)
+    This function corrects neutron counts for absolute humidity using the method described in Rosolem et al. (2013) and Anderson et al. (2017). The correction is performed using the following equation:
+
+    $$
+    C_{corrected} = C_{raw} \cdot f_w
+    $$
+
+    where:
+
+    - Ccorrected: corrected neutron counts
+    - Craw: raw neutron counts
+    - fw: absolute humidity correction factor
+
+    $$
+    f_w = 1 + 0.0054(A - A_{ref})
+    $$
+
+    where:
+
+    - A: absolute humidity
+    - Aref: reference absolute humidity
+
+    Args:
+        raw_counts (list or array): Neutron counts to correct.
+        humidity (list or array): Relative humidity readings.
+        temp (list or array): Temperature readings (Celsius).
+        Aref (float): Reference absolute humidity (g/m^3). The day of the instrument calibration is recommended.
+
+    Returns:
+        (list): Corrected neutron counts.
+
+    References:
+        M. Andreasen, K.H. Jensen, D. Desilets, T.E. Franz, M. Zreda, H.R. Bogena, and M.C. Looms. 2017. Status and perspectives on the cosmic-ray neutron method for soil moisture estimation and other environmental science applications. Vadose Zone J. 16(8). doi:10.2136/vzj2017.04.0086
+    """
+
+    A = estimate_abs_humidity(humidity, temp)
     fw = 1 + 0.0054*(A - Aref) # Zreda et al. 2017 Eq 6.
+    corrected_counts = raw_counts * fw
+    return np.round(corrected_counts)
 
-    ### Incoming neutron flux factor
-    if incoming_neutrons is None:
-        fi = 1
-        warnings.warn("Ignoring incoming neutron flux correction factor (using value fi=1)")
-    else:
-        if incoming_Ref is None and not isinstance(incoming_neutrons, type(None)):
-            incoming_Ref = incoming_neutrons[0]
-            warnings.warn('Reference incoming neutron flux not provided. Using first value of incoming neutron flux.')
+def incoming_flux_correction(raw_counts, incoming_neutrons, incoming_Ref=None):
+    r"""Correct neutron counts for incoming neutron flux.
 
-        fi = incoming_neutrons/incoming_Ref
-        fi.fillna(1.0, inplace=True) # Use a value of 1 for days without data
+    This function corrects neutron counts for incoming neutron flux using the method described in Anderson et al. (2017). The correction is performed using the following equation:
 
-    # Apply correction factors
-    return np.round((raw_counts*fw)/(fp*fi))
+    $$
+    C_{corrected} = \frac{C_{raw}}{f_i}
+    $$
+
+    where:
 
+    - Ccorrected: corrected neutron counts
+    - Craw: raw neutron counts
+    - fi: incoming neutron flux correction factor
+
+    $$
+    f_i = \frac{I_{ref}}{I}
+    $$
+
+    where:
+
+    - I: incoming neutron flux
+    - Iref: reference incoming neutron flux
+
+    Args:
+        raw_counts (list or array): Neutron counts to correct.
+        incoming_neutrons (list or array): Incoming neutron flux readings.
+        incoming_Ref (float): Reference incoming neutron flux. Baseline incoming neutron flux.
+
+    Returns:
+        (list): Corrected neutron counts.
+
+    References:
+        M. Andreasen, K.H. Jensen, D. Desilets, T.E. Franz, M. Zreda, H.R. Bogena, and M.C. Looms. 2017. Status and perspectives on the cosmic-ray neutron method for soil moisture estimation and other environmental science applications. Vadose Zone J. 16(8). doi:10.2136/vzj2017.04.0086
+
+
+    """
+    if incoming_Ref is None and not isinstance(incoming_neutrons, type(None)):
+        incoming_Ref = incoming_neutrons[0]
+        warnings.warn('Reference incoming neutron flux not provided. Using first value of incoming neutron flux.')
+    fi = incoming_neutrons / incoming_Ref
+    fi.fillna(1.0, inplace=True)  # Use a value of 1 for days without data
+
+    # Apply correction factors
+    return np.round(raw_counts / fi)
 
 
 def get_incoming_neutron_flux(start_date, end_date, station, utc_offset=0, expand_window = 0,  verbose=False):
     """Function to retrieve neutron flux from the Neutron Monitor Database.
 
     Args:
         start_date (datetime): Start date of the time series.
@@ -485,62 +588,62 @@
     # Interpolate nan values
     df_flux = df_flux['counts'].interpolate(method='nearest', limit_direction='both')
 
     # Retur only the values for the selected timestamps
     return df_flux.loc[timestamps]
 
 
-def smooth_1D(corrected_counts,window=5,order=3, method='moving_median'):
+def smooth_1d(values, window=5, order=3, method='moving_median'):
     """Use a Savitzky-Golay filter to smooth the signal of corrected neutron counts or another one-dimensional array (e.g. computed volumetric water content).
 
     Args:
-        corrected_counts (pd.DataFrame): Dataframe containing the corrected neutron counts.
+        values (pd.DataFrame or pd.Serie): Dataframe containing the values to smooth.
         window (int): Window size for the Savitzky-Golay filter. Default is 5.
         method (str): Method to use for smoothing the data. Default is 'moving_median'.
             Options are 'moving_average', 'moving_median' and 'savitzky_golay'.
         order (int): Order of the Savitzky-Golay filter. Default is 3.
 
     Returns:
-        (pd.DataFrame): DataFrame with smoothed neutron counts.
+        (pd.DataFrame): DataFrame with smoothed values.
 
     References:
         Franz, T.E., Wahbi, A., Zhang, J., Vreugdenhil, M., Heng, L., Dercon, G., Strauss, P., Brocca, L. and Wagner, W., 2020.
         Practical data products from cosmic-ray neutron sensing for hydrological applications. Frontiers in Water, 2, p.9.
         doi.org/10.3389/frwa.2020.00009
     """
 
     if method == 'moving_average':
-        corrected_counts = corrected_counts.rolling(window=window, center=True, min_periods=1).mean()
+        corrected_counts = values.rolling(window=window, center=True, min_periods=1).mean()
     elif method == 'moving_median':
-        corrected_counts = corrected_counts.rolling(window=window, center=True, min_periods=1).median()
+        corrected_counts = values.rolling(window=window, center=True, min_periods=1).median()
 
     elif method == 'savitzky_golay':
-        if corrected_counts.isna().any():
+        if values.isna().any():
             print('Dataframe contains NaN values. Please remove NaN values before smoothing the data.')
 
-        if type(corrected_counts) == pd.core.series.Series:
-            filtered = np.round(savgol_filter(corrected_counts,window,order))
-            corrected_counts = pd.DataFrame(filtered,columns=['counts'], index=corrected_counts.index)
-        elif type(corrected_counts) == pd.core.frame.DataFrame:
-            for col in corrected_counts.columns:
-                corrected_counts[col] = np.round(savgol_filter(corrected_counts[col],window,order))
+        if type(values) == pd.core.series.Series:
+            filtered = savgol_filter(values,window,order)
+            corrected_counts = pd.DataFrame(filtered,columns=['smoothed'], index=values.index)
+        elif type(values) == pd.core.frame.DataFrame:
+            for col in values.columns:
+                values[col] = savgol_filter(values[col],window,order)
     else:
         raise ValueError('Invalid method. Please select a valid filtering method., options are: moving_average, moving_median, savitzky_golay')
     corrected_counts = corrected_counts.ffill(limit=window).bfill(limit=window).copy()
     return corrected_counts
 
 
 def bwe_correction(counts, bwe, r2_N0=0.05):
     """Function to correct for biomass effects in neutron counts.
     following the approach described in Baatz et al., 2015.
 
     Args:
         counts (array or pd.Series or pd.DataFrame): Array of ephithermal neutron counts.
         bwe (float): Biomass water equivalent kg m-2.
-        r2_N0 (float): Ratio of the neutron counts reduction (counts kg-1) to the neutron calibration constant (N0). Default is 0.05 (Baatz et al., 2015).
+        r2_N0 (float): Ratio of neutron counts with biomass to neutron counts without biomass. Default is 0.05.
 
     Returns:
         (array or pd.Series or pd.DataFrame): Array of corrected neutron counts for biomass effects.
 
     References:
         Baatz, R., H. R. Bogena, H.-J. Hendricks Franssen, J. A. Huisman, C. Montzka, and H. Vereecken (2015),
         An empiricalvegetation correction for soil water content quantification using cosmic ray probes,
@@ -631,15 +734,15 @@
 
 
 
 def sensing_depth(vwc, pressure, p_ref, bulk_density, Wlat, dist, method='Schron_2017'):
     # Convert docstring to google format
     """Function that computes the estimated sensing depth of the cosmic-ray neutron probe.
     The function offers several methods to compute the depth at which 86 % of the neutrons
-    probes the soil profile.
+    probe the soil profile.
 
     Args:
         vwc (array or pd.Series or pd.DataFrame): Estimated volumetric water content for each timestamp.
         pressure (array or pd.Series or pd.DataFrame): Atmospheric pressure in hPa for each timestamp.
         p_ref (float): Reference pressure in hPa.
         bulk_density (float): Soil bulk density.
         Wlat (float): Lattice water content.
@@ -671,15 +774,15 @@
             r_start = d/Fp
 
             # Compute soil depth that accounts for 86% of the neutron flux
             D86 = 1/ bulk_density * (8.321+0.14249*(0.96655 + np.exp(-0.01*r_start))*(20+(Wlat+vwc)) / (0.0429+(Wlat+vwc)))
             results.append(D86)
 
     elif method == 'Franz_2012':
-        results = [5.8/(bulk_density*Wlat+vwc+0.0829)]
+        results = 5.8/(bulk_density*Wlat+vwc+0.0829)
 
     return results
 
 def estimate_abs_humidity(RH, temp):
     """
     Compute the actual vapor pressure (e) in g m^-3 using RH (%) and current temperature (c) observations.
 
@@ -802,14 +905,15 @@
         Franz, T.E., Wahbi, A., Zhang, J., Vreugdenhil, M., Heng, L., Dercon, G., Strauss, P., Brocca, L. and Wagner, W., 2020.
         Practical data products from cosmic-ray neutron sensing for hydrological applications. Frontiers in Water, 2, p.9.
 
         Rossini, P. and Patrignani, A., 2021. Predicting rootzone soil moisture from surface observations in cropland using an exponential filter.
         Soil Science Society of America Journal.
     """
 
+
     # Parameters
     t_delta = 1
     sm_min = np.min(sm)
     sm_max = np.max(sm)
     ms = (sm-sm_min)/(sm_max-sm_min)
 
     # Pre-allocate soil water index array
@@ -876,30 +980,30 @@
     points = np.array( (X.flatten(), Y.flatten()) ).T
     values = Z.flatten()
     zq = griddata(points, values, (xq,yq))
 
     return np.round(zq,2)
 
 
-def find_neutron_detectors(Rc, start_date=None, end_date=None):
+def find_neutron_monitor(Rc, start_date=None, end_date=None):
     """Search for potential reference neutron monitoring stations based on cutoff rigidity.
     
     Args:
         Rc (float): Cutoff rigidity in GV. Values in range 1.0 to 3.0 GV.
         start_date (datetime): Start date for the period of interest.   
         end_date (datetime): End date for the period of interest.
         
     Returns:
         (list): List of top five stations with closes cutoff rigidity.
             User needs to select station according to site altitude.
             
     Examples:
         >>> from crnpy import crnpy
         >>> Rc = 2.40 # 2.40 Newark, NJ, US
-        >>> crnpy.find_neutron_detectors(Rc)
+        >>> crnpy.find_neutron_monitor(Rc)
         Select a station with an altitude similar to that of your location. For more information go to: 'https://www.nmdb.eu/nest/help.php#helpstations
 
         Your cutoff rigidity is 2.4 GV
                 STID                          NAME     R  Altitude_m
         40   NEWK                        Newark  2.40          50
         33   MOSC                        Moscow  2.43         200
         27   KIEL                          Kiel  2.36          54
@@ -949,15 +1053,15 @@
 
 
 def estimate_lattice_water(clay_content, total_carbon=None):
     r"""Estimate the amount of water in the lattice of clay minerals.
 
     ![img1](img/lattice_water_simple.png) | ![img2](img/lattice_water_multiple.png)
     :-------------------------:|:-------------------------:
-    $\omega_{lat} = 1.241 + 0.069 * clay(\%)$ | $\omega_{lat} = -0.028 + 0.077 * clay(\%) + 0.459 * carbon(\%)$
+    $\omega_{lat} = 0.097 * clay(\%)$ | $\omega_{lat} = -0.028 + 0.077 * clay(\%) + 0.459 * carbon(\%)$
     Linear regression [lattice water (%) as a function of clay (%)] done with data from Soil Water Processes Lab and Dong and Ochsner (2018) |  Multiple linear regression [lattice water (%) as a function of clay (%) and soil carbon (%)] done with data from Soil Water Processes Lab.
 
     Args:
         clay_content (float): Clay content in the soil in percent.
         total_carbon (float, optional): Total carbon content in the soil in percent.
             If None, the amount of water is estimated based on clay content only.
 
@@ -967,15 +1071,15 @@
     References:
         Dong, J., & Ochsner, T. E. (2018). Soil texture often exerts a stronger influence than precipitation
          on mesoscale soil moisture patterns. Water Resources Research, 54, 2199– 2211.
          https://doi.org/10.1002/2017WR021692
 
     """
     if total_carbon is None:
-        lattice_water = 1.241 + 0.069 * clay_content
+        lattice_water = 0.097 * clay_content
     else:
         lattice_water = -0.028 + 0.077 * clay_content + 0.459 * total_carbon
     return lattice_water
 
 
 def latlon_to_utm(lat, lon, utm_zone_number, missing_values=None):
     """Convert geographic coordinates (lat, lon) to projected coordinates (utm) using the Military Grid Reference System.
@@ -1077,15 +1181,15 @@
     Returns:
         (ndarray): Numpy array of distances from the point (px,py) to all the points in x and y vectors.
     """
     d = np.sqrt((px - x) ** 2 + (py - y) ** 2)
     return d
 
 
-def smooth_2D(x, y, z, buffer=100, min_neighbours=3, method='mean', rnd=False):
+def spatial_average(x, y, z, buffer=100, min_neighbours=3, method='mean', rnd=False):
     """Moving buffer filter to smooth georeferenced two-dimensional data.
 
     Args:
         x (list or array): UTM x coordinates in meters.
         y (list or array): UTM y coordinates in meters.
         z (list or array): Values to be smoothed.
         buffer (float): Radial buffer distance in meters.
@@ -1152,15 +1256,15 @@
         neighborhood (float): Only points within this radius in meters are considered for the interpolation.
         p (int): Exponent of the inverse distance weight formula. Typically, p=1 or p=2.
 
     Returns:
         (array): Interpolated values.
 
     References:
-        [https://soilwater.github.io/pynotes-agriscience/notebooks/inverse_distance_weighting.html](https://soilwater.github.io/pynotes-agriscience/notebooks/inverse_distance_weighting.html)
+        [https://en.wikipedia.org/wiki/Inverse_distance_weighting](https://en.wikipedia.org/wiki/Inverse_distance_weighting)
 
 
     """
 
     # Flatten arrays to handle 1D and 2D arrays with the same code
     s = X_pred.shape  # Save shape
     X_pred = X_pred.flatten()
@@ -1169,24 +1273,24 @@
     # Pre-allocate output array
     Z_pred = np.full_like(X_pred, np.nan)
 
     for n in range(X_pred.size):
         # Distance between current and observed points
         d = euclidean_distance(X_pred[n], Y_pred[n], x, y)
 
-        # Select points within neighborhood only for interpolateion
+        # Select points within neighborhood only for interpolation
         idx_neighbors = d < neighborhood
 
         # Compute interpolated value at point of interest
         Z_pred[n] = np.sum(z[idx_neighbors] / d[idx_neighbors] ** p) / np.sum(1 / d[idx_neighbors] ** p)
 
     return np.reshape(Z_pred, s)
 
 
-def interpolate_2D(x, y, z, dx=100, dy=100, method='cubic', neighborhood=1000):
+def interpolate_2d(x, y, z, dx=100, dy=100, method='cubic', neighborhood=1000):
     """Function for interpolating irregular spatial data into a regular grid.
 
     Args:
         x (list or array): UTM x coordinates in meters.
         y (list or array): UTM y coordinates in meters.
         z (list or array): Values to be interpolated.
         dx (float): Pixel width in meters.
@@ -1228,8 +1332,39 @@
 
     else:
         raise f"Method {method} does not exist. Provide either 'cubic', 'linear', 'nearest', or 'idw'."
 
     return X_pred, Y_pred, Z_pred
 
 
+def estimate_locations(x, y):
+    """Function to estimate the intermediate locations between two points, assuming the measurements were taken at a constant speed.
+
+    Args:
+        x (array): x coordinates.
+        y (array): y coordinates.
+
+    Returns:
+        x_est (array): Estimated x coordinates.
+        y_est (array): Estimated y coordinates.
+    """
+
+    # Make it datatype agnostic
+    if(isinstance(x, pd.Series)):
+        x = x.values
+    if(isinstance(y, pd.Series)):
+        y = y.values
+
+    # Do the average of the two points
+    x_est = (x[1:] + x[:-1]) / 2
+    y_est = (y[1:] + y[:-1]) / 2
+
+    # Add the first point to match the length of the original array
+    x_est = np.insert(x_est, 0, x[0])
+    y_est = np.insert(y_est, 0, y[0])
+
+
+    return x_est, y_est
+
+
+
```

### Comparing `crnpy-0.3.post1/src/crnpy/data.py` & `crnpy-0.4.0/src/crnpy/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """## crnpy.data
 Data module for crnpy.
 
 This module contains data for the crnpy package.
 
 Attributes:
     cutoff_rigidity (list): Cutoff rigidity values for the whole world. See [crnpy.crnpy.cutoff_rigidity][]
-    neutron_detectors (list): Neutron detector locations. See [crnpy.crnpy.find_neutron_detectors][]
+    neutron_detectors (list): Neutron detector locations. See [crnpy.crnpy.find_neutron_monitor][]
 
 """
 
 cutoff_rigidity = [[0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
                    [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
                    [0.0, 0.0, 0.02, 0.02, 0.02, 0.03, 0.03, 0.04, 0.03, 0.03, 0.04, 0.03, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
                    [0.04, 0.07, 0.09, 0.08, 0.13, 0.08, 0.16, 0.14, 0.13, 0.15, 0.17, 0.13, 0.08, 0.04, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.02, 0.05, 0.04],
```

