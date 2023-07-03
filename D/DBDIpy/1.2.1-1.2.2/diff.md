# Comparing `tmp/DBDIpy-1.2.1.tar.gz` & `tmp/DBDIpy-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DBDIpy-1.2.1.tar", last modified: Wed May  3 08:34:42 2023, max compression
+gzip compressed data, was "DBDIpy-1.2.2.tar", last modified: Mon Jul  3 12:34:41 2023, max compression
```

## Comparing `DBDIpy-1.2.1.tar` & `DBDIpy-1.2.2.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 lw         (501) staff       (20)        0 2023-05-03 08:34:42.769547 DBDIpy-1.2.1/
-drwxr-xr-x   0 lw         (501) staff       (20)        0 2023-05-03 08:34:42.762767 DBDIpy-1.2.1/DBDIpy/
--rw-r--r--   0 lw         (501) staff       (20)      307 2023-03-16 12:30:32.000000 DBDIpy-1.2.1/DBDIpy/__init__.py
--rw-r--r--   0 lw         (501) staff       (20)     6078 2023-01-11 08:49:53.000000 DBDIpy-1.2.1/DBDIpy/align_spectra.py
--rw-r--r--   0 lw         (501) staff       (20)     1795 2022-11-04 08:07:13.000000 DBDIpy-1.2.1/DBDIpy/export_to_spectra.py
--rw-r--r--   0 lw         (501) staff       (20)     5249 2023-03-16 13:49:15.000000 DBDIpy-1.2.1/DBDIpy/identify_adducts.py
--rw-r--r--   0 lw         (501) staff       (20)     3258 2022-11-04 08:58:51.000000 DBDIpy-1.2.1/DBDIpy/impute_intensities.py
--rw-r--r--   0 lw         (501) staff       (20)     4129 2022-11-04 08:57:50.000000 DBDIpy-1.2.1/DBDIpy/plot_adducts.py
--rw-r--r--   0 lw         (501) staff       (20)     3884 2023-03-16 14:02:37.000000 DBDIpy-1.2.1/DBDIpy/propose_adducts.py
-drwxr-xr-x   0 lw         (501) staff       (20)        0 2023-05-03 08:34:42.768969 DBDIpy-1.2.1/DBDIpy/tests/
--rw-r--r--   0 lw         (501) staff       (20)     4417 2023-05-03 08:21:55.000000 DBDIpy-1.2.1/DBDIpy/tests/testLW.py
--rw-r--r--   0 lw         (501) staff       (20)     1397 2022-10-20 11:54:12.000000 DBDIpy-1.2.1/DBDIpy/tests/test_align_spectra.py
--rw-r--r--   0 lw         (501) staff       (20)     5390 2022-10-20 14:45:33.000000 DBDIpy-1.2.1/DBDIpy/tests/test_identify_adducts.py
--rw-r--r--   0 lw         (501) staff       (20)      883 2022-11-04 08:28:05.000000 DBDIpy-1.2.1/DBDIpy/tests/test_impute_intensities.py
--rw-r--r--   0 lw         (501) staff       (20)     1841 2022-10-20 10:04:59.000000 DBDIpy-1.2.1/DBDIpy/tests/test_plot_adducts.py
--rw-r--r--   0 lw         (501) staff       (20)     1088 2023-03-16 14:02:29.000000 DBDIpy-1.2.1/DBDIpy/tests/test_propose_adducts.py
-drwxr-xr-x   0 lw         (501) staff       (20)        0 2023-05-03 08:34:42.766189 DBDIpy-1.2.1/DBDIpy.egg-info/
--rw-r--r--   0 lw         (501) staff       (20)    17102 2023-05-03 08:34:42.000000 DBDIpy-1.2.1/DBDIpy.egg-info/PKG-INFO
--rw-r--r--   0 lw         (501) staff       (20)      550 2023-05-03 08:34:42.000000 DBDIpy-1.2.1/DBDIpy.egg-info/SOURCES.txt
--rw-r--r--   0 lw         (501) staff       (20)        1 2023-05-03 08:34:42.000000 DBDIpy-1.2.1/DBDIpy.egg-info/dependency_links.txt
--rw-r--r--   0 lw         (501) staff       (20)       65 2023-05-03 08:34:42.000000 DBDIpy-1.2.1/DBDIpy.egg-info/requires.txt
--rw-r--r--   0 lw         (501) staff       (20)        7 2023-05-03 08:34:42.000000 DBDIpy-1.2.1/DBDIpy.egg-info/top_level.txt
--rw-r--r--   0 lw         (501) staff       (20)    17102 2023-05-03 08:34:42.769321 DBDIpy-1.2.1/PKG-INFO
--rw-r--r--   0 lw         (501) staff       (20)    16529 2023-05-03 07:37:43.000000 DBDIpy-1.2.1/README.md
--rw-r--r--   0 lw         (501) staff       (20)       38 2023-05-03 08:34:42.769592 DBDIpy-1.2.1/setup.cfg
--rw-r--r--   0 lw         (501) staff       (20)     1261 2023-05-03 07:32:39.000000 DBDIpy-1.2.1/setup.py
+drwxr-xr-x   0 lw         (501) staff       (20)        0 2023-07-03 12:34:41.098205 DBDIpy-1.2.2/
+drwxr-xr-x   0 lw         (501) staff       (20)        0 2023-07-03 12:34:41.092137 DBDIpy-1.2.2/DBDIpy/
+-rw-r--r--   0 lw         (501) staff       (20)      491 2023-05-15 14:59:19.000000 DBDIpy-1.2.2/DBDIpy/__init__.py
+-rw-r--r--   0 lw         (501) staff       (20)     6342 2023-05-15 15:06:11.000000 DBDIpy-1.2.2/DBDIpy/align_spectra.py
+-rw-r--r--   0 lw         (501) staff       (20)     4850 2023-05-15 14:46:07.000000 DBDIpy-1.2.2/DBDIpy/dbdipy_auxiliaries.py
+-rw-r--r--   0 lw         (501) staff       (20)     1795 2022-11-04 08:07:13.000000 DBDIpy-1.2.2/DBDIpy/export_to_spectra.py
+-rw-r--r--   0 lw         (501) staff       (20)    10488 2023-05-15 15:00:27.000000 DBDIpy-1.2.2/DBDIpy/identify_adducts.py
+-rw-r--r--   0 lw         (501) staff       (20)     3258 2022-11-04 08:58:51.000000 DBDIpy-1.2.2/DBDIpy/impute_intensities.py
+-rw-r--r--   0 lw         (501) staff       (20)       36 2023-05-15 09:11:05.000000 DBDIpy-1.2.2/DBDIpy/plot_adducts_MS2.py
+-rw-r--r--   0 lw         (501) staff       (20)     4133 2023-05-13 20:38:26.000000 DBDIpy-1.2.2/DBDIpy/plot_adducts_XIC.py
+-rw-r--r--   0 lw         (501) staff       (20)     3884 2023-03-16 14:02:37.000000 DBDIpy-1.2.2/DBDIpy/propose_adducts.py
+drwxr-xr-x   0 lw         (501) staff       (20)        0 2023-07-03 12:34:41.097778 DBDIpy-1.2.2/DBDIpy/tests/
+-rw-r--r--   0 lw         (501) staff       (20)     5568 2023-05-15 14:36:55.000000 DBDIpy-1.2.2/DBDIpy/tests/testLW.py
+-rw-r--r--   0 lw         (501) staff       (20)     1397 2022-10-20 11:54:12.000000 DBDIpy-1.2.2/DBDIpy/tests/test_align_spectra.py
+-rw-r--r--   0 lw         (501) staff       (20)     5418 2023-05-15 14:59:01.000000 DBDIpy-1.2.2/DBDIpy/tests/test_identify_adducts.py
+-rw-r--r--   0 lw         (501) staff       (20)      883 2022-11-04 08:28:05.000000 DBDIpy-1.2.2/DBDIpy/tests/test_impute_intensities.py
+-rw-r--r--   0 lw         (501) staff       (20)      105 2023-05-13 20:37:45.000000 DBDIpy-1.2.2/DBDIpy/tests/test_plot_adducts_MS2.py
+-rw-r--r--   0 lw         (501) staff       (20)     1865 2023-05-13 20:40:01.000000 DBDIpy-1.2.2/DBDIpy/tests/test_plot_adducts_XIC.py
+-rw-r--r--   0 lw         (501) staff       (20)     1088 2023-03-16 14:02:29.000000 DBDIpy-1.2.2/DBDIpy/tests/test_propose_adducts.py
+drwxr-xr-x   0 lw         (501) staff       (20)        0 2023-07-03 12:34:41.093335 DBDIpy-1.2.2/DBDIpy.egg-info/
+-rw-r--r--   0 lw         (501) staff       (20)    17414 2023-07-03 12:34:41.000000 DBDIpy-1.2.2/DBDIpy.egg-info/PKG-INFO
+-rw-r--r--   0 lw         (501) staff       (20)      652 2023-07-03 12:34:41.000000 DBDIpy-1.2.2/DBDIpy.egg-info/SOURCES.txt
+-rw-r--r--   0 lw         (501) staff       (20)        1 2023-07-03 12:34:41.000000 DBDIpy-1.2.2/DBDIpy.egg-info/dependency_links.txt
+-rw-r--r--   0 lw         (501) staff       (20)       65 2023-07-03 12:34:41.000000 DBDIpy-1.2.2/DBDIpy.egg-info/requires.txt
+-rw-r--r--   0 lw         (501) staff       (20)        7 2023-07-03 12:34:41.000000 DBDIpy-1.2.2/DBDIpy.egg-info/top_level.txt
+-rw-r--r--   0 lw         (501) staff       (20)    17414 2023-07-03 12:34:41.098027 DBDIpy-1.2.2/PKG-INFO
+-rw-r--r--   0 lw         (501) staff       (20)    16848 2023-07-03 12:32:27.000000 DBDIpy-1.2.2/README.md
+-rw-r--r--   0 lw         (501) staff       (20)       38 2023-07-03 12:34:41.098264 DBDIpy-1.2.2/setup.cfg
+-rw-r--r--   0 lw         (501) staff       (20)     1261 2023-07-03 12:30:29.000000 DBDIpy-1.2.2/setup.py
```

### Comparing `DBDIpy-1.2.1/DBDIpy/align_spectra.py` & `DBDIpy-1.2.2/DBDIpy/align_spectra.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-def align_spectra(spec, ppm_window = 2):
+def align_spectra(spec, ms_level = 1, ppm_window = 2):
     
     """Feature building from a list of spectra.
     Aligns detected peaks in a list of matchms.Spectra objects into two-dimensional tabular data.
     Utilizes data loaded by matchms.importing module and connects to matchMS (pre-)processing workflows.
     (Function optimized for runtime)
     
     Parameters
@@ -32,14 +32,20 @@
     import pandas as pd
     import numpy as np
     
     
     if not isinstance(spec[0], matchms.Spectrum):
         raise TypeError("Argument for spec should be a list of matchms.Spectrum.")
         
+     ###################################################   
+     ##make a subset of spectrums list based on ms level
+     ##demo data: mzml file with ms1 AND ms2 information
+     ################################################### 
+        
+        
     aldf = pd.DataFrame({"mean": spec[0].peaks.mz, "scan1": spec[0].peaks.intensities})
     aldf = aldf.reset_index(drop = True)
     
     massdf = pd.DataFrame({"scan1": spec[0].peaks.mz})
     
     for s in tqdm(range(1, len(spec)), desc = 'progress'):                                                            ## s iterates over number oof spectra
                                                                                                                       ## p iterates over number of peaks in spectrum
```

### Comparing `DBDIpy-1.2.1/DBDIpy/export_to_spectra.py` & `DBDIpy-1.2.2/DBDIpy/export_to_spectra.py`

 * *Files identical despite different names*

### Comparing `DBDIpy-1.2.1/DBDIpy/identify_adducts.py` & `DBDIpy-1.2.2/DBDIpy/identify_adducts.py`

 * *Files 23% similar despite different names*

```diff
@@ -1 +1 @@
-def identify_adducts(df, masses, custom_adducts = None, method = "pearson", threshold = 0.90, mass_error = 2):        """Finds different ion species of a single analyte molecule.     Computes pointwise correlation of XIC traces to identify in-source adducts or in-source fragments    generated during direct infusion mass spectrometric data aquisition.     Putative identification of adducts and fragments is based on a correlation threshold and mass differences.         Parameters    ----------        df : pd.DataFrame         A DataFrame of equal-length ion traces formated as rows.         Input DataFrame can be provided by align_spectra() and impute_intensities().        masses : pd.series              A series of m/z values for specification of adduct or fragment types.             Use of theoretic masses is strongly recommended for higher precission.            If theoretic masses are not available, adapt mass_error             in accordance to the type of your mass analyzer.            adduct_rules : pd.DataFrame, optional                  The function searches for 1-Oxygen and 2-Oxygen adducts                   and in-source water-losses by default.                   Custom adduct rules need to be specified in a DataFrame as following:                  custom_adducts = pd.DataFrame({'deltamz': [mz1, mz2, mz3],                                                 'motive': ["motive1", "motive2", "motive3"]}).         method : str, {'pearson’, ‘spearman’, ‘kendall’}            Correlation method for pointwise compariation of XIC traces.                 threshold : float                Correlation treshold to associate two ions. Default is 0.9.                   mass_error : int or float                 Tolerance of the mass spectrometer in ppm. Default is 2 ppm.         Returns    -------    A dictionary of DataFrames containing pairwise information about correlation of XIC traces and     putatively identified in-source adducts or in-source fragments.            Raises    ------    ValueError        If the input DataFrame contains missing values.            See Also    --------    DBDIpy.align_spectra(), DBDIpy.impute_intensities() : For preparation of the input data.        """#%%library import     import pandas as pd    from tqdm import tqdm    #%%check if user imput is valid        if not isinstance(df, pd.DataFrame):        raise TypeError("Argument for df should be of instance pandas.DataFrame.")              if df.isnull().values.any():        raise ValueError("Input DataFrame contains missing values.")        if masses.size != df.shape[0]:        raise ValueError("Incompatible dimensions of mass list and number of XIC.")            if df.shape[1] < 10:        raise Warning("Low number of scans! Consider providing more scans to improve reliability of correlation results.")        #%%correlation matrix calculation                cormat = df.T.corr(method = method)    #%%set up adduct rules       massdifflib = pd.DataFrame({'deltamz': [15.994915, 31.98983, 18.010565],                                 'motive': ["O", "O2", "H2O"]})         if custom_adducts is not None:          if not isinstance(custom_adducts, pd.DataFrame):             raise TypeError("Wrong format for custom adduct rules.")              if list(massdifflib.columns) == list(custom_adducts.columns):             massdifflib = pd.concat([massdifflib, custom_adducts])             massdifflib = massdifflib.reset_index(drop = True)                       else:             raise TypeError("Wrong format for custom adduct rules. See documentation for example.")                 massdifflib["mass_upper"] = massdifflib["deltamz"] + massdifflib["deltamz"] * mass_error * 1e-6     massdifflib["mass_lower"] = massdifflib["deltamz"] - massdifflib["deltamz"] * mass_error * 1e-6 #%%refine correlations by mass differences    res_internal = pd.DataFrame({"base_mz": [], "base_index": [], "match_mz": [],                             "match_index": [], "mzdiff": [],"corr": []})         for i in tqdm(range(len(cormat)), desc='progress'):        featnow = cormat.iloc[:,i]                                                              featnow = featnow[(featnow > threshold) & (featnow < 1)]                 mzi = masses[i]                                                mz_matches = masses[featnow.index]                                  mz_diff = abs(mz_matches - mzi)                                                            for j in range(len(featnow)):                    res_internal.loc[len(res_internal)] = [masses[i], i, masses[featnow.index[j]],                                                   featnow.index[j], mz_diff.values[j],                                                   featnow.values[j]]      #%%extract different adduct types to lists    reslist = {}       for a in range(massdifflib.shape[0]):                dfnow = res_internal.loc[(res_internal["mzdiff"] >= massdifflib.loc[a, "mass_lower"]) &                                 (res_internal["mzdiff"] <= massdifflib.loc[a, "mass_upper"])]                reslist[massdifflib.loc[a, "motive"]] = dfnow            return reslist
+def identify_adducts_MS1(df, masses, custom_adducts = None, method = "pearson", threshold = 0.90, mass_error = 2):        """Finds different ion species of a single analyte molecule.     Computes pointwise correlation of XIC traces to identify in-source adducts or in-source fragments    generated during direct infusion mass spectrometric data aquisition.     Putative identification of adducts and fragments is based on a correlation threshold and mass differences.         Parameters    ----------        df : pd.DataFrame         A DataFrame of equal-length ion traces formated as rows.         Input DataFrame can be provided by align_spectra() and impute_intensities().        masses : pd.series              A series of m/z values for specification of adduct or fragment types.             Use of theoretic masses is strongly recommended for higher precission.            If theoretic masses are not available, adapt mass_error             in accordance to the type of your mass analyzer.            adduct_rules : pd.DataFrame, optional                  The function searches for 1-Oxygen and 2-Oxygen adducts                   and in-source water-losses by default.                   Custom adduct rules need to be specified in a DataFrame as following:                  custom_adducts = pd.DataFrame({'deltamz': [mz1, mz2, mz3],                                                 'motive': ["motive1", "motive2", "motive3"]}).         method : str, {'pearson’, ‘spearman’, ‘kendall’}            Correlation method for pointwise compariation of XIC traces.                 threshold : float                Correlation treshold to associate two ions. Default is 0.9.                   mass_error : int or float                 Tolerance of the mass spectrometer in ppm. Default is 2 ppm.         Returns    -------    A dictionary of DataFrames containing pairwise information about correlation of XIC traces and     putatively identified in-source adducts or in-source fragments.            Raises    ------    ValueError        If the input DataFrame contains missing values.            See Also    --------    DBDIpy.align_spectra(), DBDIpy.impute_intensities() : For preparation of the input data.        """#library import     import pandas as pd    from tqdm import tqdm    #check if user imput is valid        if not isinstance(df, pd.DataFrame):        raise TypeError("Argument for df should be of instance pandas.DataFrame.")              if df.isnull().values.any():        raise ValueError("Input DataFrame contains missing values.")        if masses.size != df.shape[0]:        raise ValueError("Incompatible dimensions of mass list and number of XIC.")            if df.shape[1] < 10:        raise Warning("Low number of scans! Consider providing more scans to improve reliability of correlation results.")        #correlation matrix calculation                cormat = df.T.corr(method = method)    #set up adduct rules       massdifflib = pd.DataFrame({'deltamz': [15.994915, 31.98983, 18.010565],                                 'motive': ["O", "O2", "H2O"]})         if custom_adducts is not None:          if not isinstance(custom_adducts, pd.DataFrame):             raise TypeError("Wrong format for custom adduct rules.")              if list(massdifflib.columns) == list(custom_adducts.columns):             massdifflib = pd.concat([massdifflib, custom_adducts])             massdifflib = massdifflib.reset_index(drop = True)                       else:             raise TypeError("Wrong format for custom adduct rules. See documentation for example.")                 massdifflib["mass_upper"] = massdifflib["deltamz"] + massdifflib["deltamz"] * mass_error * 1e-6     massdifflib["mass_lower"] = massdifflib["deltamz"] - massdifflib["deltamz"] * mass_error * 1e-6 #refine correlations by mass differences    res_internal = pd.DataFrame({"base_mz": [], "base_index": [], "match_mz": [],                             "match_index": [], "mzdiff": [],"corr": []})         for i in tqdm(range(len(cormat)), desc='progress'):        featnow = cormat.iloc[:,i]                                                              featnow = featnow[(featnow > threshold) & (featnow < 1)]                 mzi = masses[i]                                                mz_matches = masses[featnow.index]                                  mz_diff = abs(mz_matches - mzi)                                                            for j in range(len(featnow)):                    res_internal.loc[len(res_internal)] = [masses[i], i, masses[featnow.index[j]],                                                   featnow.index[j], mz_diff.values[j],                                                   featnow.values[j]]      #extract different adduct types to lists    reslist = {}       for a in range(massdifflib.shape[0]):                dfnow = res_internal.loc[(res_internal["mzdiff"] >= massdifflib.loc[a, "mass_lower"]) &                                 (res_internal["mzdiff"] <= massdifflib.loc[a, "mass_upper"])]                reslist[massdifflib.loc[a, "motive"]] = dfnow            return reslist#%%def identify_adducts_MS2(df, masses, custom_adducts = None, method = "pearson", threshold = 0.90, mass_error = 2):        """Finds different ion species of a single analyte molecule.     Computes pointwise correlation of XIC traces to identify in-source adducts or in-source fragments    generated during direct infusion mass spectrometric data aquisition.     Putative identification of adducts and fragments is based on a correlation threshold and mass differences.         Parameters    ----------        df : pd.DataFrame         A DataFrame of equal-length ion traces formated as rows.         Input DataFrame can be provided by align_spectra() and impute_intensities().        masses : pd.series              A series of m/z values for specification of adduct or fragment types.             Use of theoretic masses is strongly recommended for higher precission.            If theoretic masses are not available, adapt mass_error             in accordance to the type of your mass analyzer.            adduct_rules : pd.DataFrame, optional                  The function searches for 1-Oxygen and 2-Oxygen adducts                   and in-source water-losses by default.                   Custom adduct rules need to be specified in a DataFrame as following:                  custom_adducts = pd.DataFrame({'deltamz': [mz1, mz2, mz3],                                                 'motive': ["motive1", "motive2", "motive3"]}).         method : str, {'pearson’, ‘spearman’, ‘kendall’}            Correlation method for pointwise compariation of XIC traces.                 threshold : float                Correlation treshold to associate two ions. Default is 0.9.                   mass_error : int or float                 Tolerance of the mass spectrometer in ppm. Default is 2 ppm.         Returns    -------    A dictionary of DataFrames containing pairwise information about correlation of XIC traces and     putatively identified in-source adducts or in-source fragments.            Raises    ------    ValueError        If the input DataFrame contains missing values.            See Also    --------    DBDIpy.align_spectra(), DBDIpy.impute_intensities() : For preparation of the input data.        """#library import     import pandas as pd    from tqdm import tqdm    #check if user imput is valid        if not isinstance(df, pd.DataFrame):        raise TypeError("Argument for df should be of instance pandas.DataFrame.")              if df.isnull().values.any():        raise ValueError("Input DataFrame contains missing values.")        if masses.size != df.shape[0]:        raise ValueError("Incompatible dimensions of mass list and number of XIC.")            if df.shape[1] < 10:        raise Warning("Low number of scans! Consider providing more scans to improve reliability of correlation results.")        #correlation matrix calculation                cormat = df.T.corr(method = method)    #set up adduct rules       massdifflib = pd.DataFrame({'deltamz': [15.994915, 31.98983, 18.010565],                                 'motive': ["O", "O2", "H2O"]})         if custom_adducts is not None:          if not isinstance(custom_adducts, pd.DataFrame):             raise TypeError("Wrong format for custom adduct rules.")              if list(massdifflib.columns) == list(custom_adducts.columns):             massdifflib = pd.concat([massdifflib, custom_adducts])             massdifflib = massdifflib.reset_index(drop = True)                       else:             raise TypeError("Wrong format for custom adduct rules. See documentation for example.")                 massdifflib["mass_upper"] = massdifflib["deltamz"] + massdifflib["deltamz"] * mass_error * 1e-6     massdifflib["mass_lower"] = massdifflib["deltamz"] - massdifflib["deltamz"] * mass_error * 1e-6 #refine correlations by mass differences    res_internal = pd.DataFrame({"base_mz": [], "base_index": [], "match_mz": [],                             "match_index": [], "mzdiff": [],"corr": []})         for i in tqdm(range(len(cormat)), desc='progress'):        featnow = cormat.iloc[:,i]                                                              featnow = featnow[(featnow > threshold) & (featnow < 1)]                 mzi = masses[i]                                                mz_matches = masses[featnow.index]                                  mz_diff = abs(mz_matches - mzi)                                                            for j in range(len(featnow)):                    res_internal.loc[len(res_internal)] = [masses[i], i, masses[featnow.index[j]],                                                   featnow.index[j], mz_diff.values[j],                                                   featnow.values[j]]      #extract different adduct types to lists    reslist = {}       for a in range(massdifflib.shape[0]):                dfnow = res_internal.loc[(res_internal["mzdiff"] >= massdifflib.loc[a, "mass_lower"]) &                                 (res_internal["mzdiff"] <= massdifflib.loc[a, "mass_upper"])]                reslist[massdifflib.loc[a, "motive"]] = dfnow            return reslist
```

### Comparing `DBDIpy-1.2.1/DBDIpy/impute_intensities.py` & `DBDIpy-1.2.2/DBDIpy/impute_intensities.py`

 * *Files identical despite different names*

### Comparing `DBDIpy-1.2.1/DBDIpy/plot_adducts.py` & `DBDIpy-1.2.2/DBDIpy/plot_adducts_XIC.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-def plot_adducts(IDs, df, metadata = None, transform = False):
+def plot_adducts_XIC(IDs, df, metadata = None, transform = False):
     
     """Visualizes identified adducts or in-source fragments.
     A graphical tool for the visualization of correlated XIC traces identified by 
     identify_adducts(). 
     The temporal evolution of selected features is plotted to inspect correlation results 
     and adduct information.
```

### Comparing `DBDIpy-1.2.1/DBDIpy/propose_adducts.py` & `DBDIpy-1.2.2/DBDIpy/propose_adducts.py`

 * *Files identical despite different names*

### Comparing `DBDIpy-1.2.1/DBDIpy/tests/testLW.py` & `DBDIpy-1.2.2/DBDIpy/tests/testLW.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1 +1 @@
-import pandas as pdimport numpy as npimport featherimport matplotlib.pyplot as pltimport DBDIpy as dbdiimport os##macOSintensities_raw = feather.read_dataframe("/Users/lw/Nextcloud/Project212/src/data/example_dataset.feather")annotation_metadata = feather.read_dataframe("/Users/lw/Nextcloud/Project212/src/data/example_metadata.feather")##windowsintensities_raw = feather.read_dataframe("C:/Users/weidner.leopold/Nextcloud/Project212/src/data/example_dataset.feather")##intensities_raw = feather.read_dataframe("C:/Users/weidner.leopold/Nextcloud/Project212/src/data/example_all_dataset.feather")annotation_metadata = feather.read_dataframe("C:/Users/weidner.leopold/Nextcloud/Project212/src/data/example_metadata.feather")##annotation_metadata = feather.read_dataframe("C:/Users/weidner.leopold/Nextcloud/Project212/src/data/example_all_metadata.feather")#%%setup imp moduleIDs = annotation_metadata["ID"]intensities_raw = intensities_raw.drop("ID", axis = 1)df = intensities_raw.copy()#%%test imputation moduleraw_imp = dbdi.impute_intensities(intensities_raw, method = "linear")raw_imp_lin = dbdi.impute_intensities(intensities_raw, method = "linear")raw_imp_quad = dbdi.impute_intensities(intensities_raw, method = "quadratic")raw_imp_ind = dbdi.impute_intensities(intensities_raw, method = "previous")## indices of oxygen series from C15H17O2N 55 -> 66 ->> 83 ->>> 99#%%setup corr mudulemethod = "spearman"custom_adducts = Nonemass_error = 0.1masses = annotation_metadata.iloc[:,3]threshold = 0.95adducts095 =  dbdi.identify_adducts(raw_imp, annotation_metadata["ThMass.Ion"],                          custom_adducts = pd.DataFrame({'deltamz': [47.984744], 'motive': ["O3"]}),                         method = "spearman", threshold = 0.90, mass_error = 5)   #%%setup import from mgfimport timefrom matchms.importing import load_from_mgfpath_data = "/Users/lw/Nextcloud/Project212/src/data"  file_mgf = os.path.join(path_data, "example_dataset.mgf")spectrums = list(load_from_mgf(file_mgf))starttime = time.process_time()testXX = dbdi.align_spectra(spectrums)elapsed = time.process_time() - starttimeprint(elapsed)   ##7.24 sec#%% import-export-cylcefrom matchms import exportingftints = intensities_raw.copy()ftints["mean"] = annotation_metadata["ThMass.Ion"]testX =  export_to_spectra(ftints, 88)exporting.save_as_mgf(testX, filename = "example_dataset.mgf")os.getcwd()O1 = reslist["O"]O2 = reslist["O2"]O3 = reslist["O3"]H2O = reslist["H2O"]x = np.intersect1d(O3["base_index"], np.intersect1d(O1["base_index"],O2["base_index"]))a = np.intersect1d(x , H2O["base_index"])#%% plotting module IDs = [55,66,83,99]df = raw_imp.copy()transform = Truetest = dbdi.plot_adducts([55,66,83,99], df = raw_imp)test = dbdi.plot_adducts(IDs, df, metadata = annotation_metadata, transform = False)plot_adducts(2,2)test.gca().get_title()specs_aligned = specs_aligned.apply(lambda col:pd.to_numeric(col, errors='coerce'))#%% path = r'D:\Users\.....'path = path.replace('\\' , '/')feather.write_dataframe(raw_imp, "demo_filled.feather")os.getcwd()#%% for resubmissionintensities_raw = feather.read_dataframe("C:/Users/weidner.leopold/Documents/10_Publications/02_Online_Roasting/data-RiedFresh/2023-01-23-example_dataset-resubmission.feather")annotation_metadata = feather.read_dataframe("C:/Users/weidner.leopold/Documents/10_Publications/02_Online_Roasting/data-RiedFresh/2023-01-23-example__metadata2-resubmission.feather")IDs = annotation_metadata["ID"]intensities_raw = intensities_raw.drop("ID", axis = 1)raw_imp = dbdi.impute_intensities(intensities_raw, method = "linear")ca = pd.DataFrame({'deltamz': [47.984744, 63.979658], 'motive': ["O3", "O4"]})adducts095 =  dbdi.identify_adducts(raw_imp, annotation_metadata["ThMass.Ion"],                          custom_adducts = ca, method = "spearman", threshold = 0.95, mass_error = 5)searchres4plotting = {k:len(v) for k, v in adducts095.items()}#%% propose adductsx = propose_adducts(ID = 55, df = raw_imp,                 masses = annotation_metadata["ThMass.Ion"],                method = "pearson", threshold = 0.95,                 mass_error = 0.005,                custom_adducts =  pd.DataFrame({'mass_diff': [18.010565],                                                   'annotation': ["[M-XYX+H]+"]}))            
+import pandas as pdimport numpy as npimport featherimport matplotlib.pyplot as pltimport DBDIpy as dbdiimport os##macOSintensities_raw = feather.read_dataframe("/Users/lw/Nextcloud/Project212/src/data/example_dataset.feather")annotation_metadata = feather.read_dataframe("/Users/lw/Nextcloud/Project212/src/data/example_metadata.feather")##windowsintensities_raw = feather.read_dataframe("C:/Users/weidner.leopold/Nextcloud/Project212/src/data/example_dataset.feather")##intensities_raw = feather.read_dataframe("C:/Users/weidner.leopold/Nextcloud/Project212/src/data/example_all_dataset.feather")annotation_metadata = feather.read_dataframe("C:/Users/weidner.leopold/Nextcloud/Project212/src/data/example_metadata.feather")##annotation_metadata = feather.read_dataframe("C:/Users/weidner.leopold/Nextcloud/Project212/src/data/example_all_metadata.feather")#%%setup imp moduleIDs = annotation_metadata["ID"]intensities_raw = intensities_raw.drop("ID", axis = 1)df = intensities_raw.copy()#%%test imputation moduleraw_imp = dbdi.impute_intensities(intensities_raw, method = "linear")raw_imp_lin = dbdi.impute_intensities(intensities_raw, method = "linear")raw_imp_quad = dbdi.impute_intensities(intensities_raw, method = "quadratic")raw_imp_ind = dbdi.impute_intensities(intensities_raw, method = "previous")## indices of oxygen series from C15H17O2N 55 -> 66 ->> 83 ->>> 99#%%setup corr mudulemethod = "spearman"custom_adducts = Nonemass_error = 0.1masses = annotation_metadata.iloc[:,3]threshold = 0.95adducts095 =  dbdi.identify_adducts(raw_imp, annotation_metadata["ThMass.Ion"],                          custom_adducts = pd.DataFrame({'deltamz': [47.984744], 'motive': ["O3"]}),                         method = "spearman", threshold = 0.90, mass_error = 5)   #%%setup import from mgfimport timefrom matchms.importing import load_from_mgfpath_data = "/Users/lw/Nextcloud/Project212/src/data"  file_mgf = os.path.join(path_data, "example_dataset.mgf")spectrums = list(load_from_mgf(file_mgf))starttime = time.process_time()testXX = dbdi.align_spectra(spectrums)elapsed = time.process_time() - starttimeprint(elapsed)   ##7.24 sec#%% import-export-cylcefrom matchms import exportingftints = intensities_raw.copy()ftints["mean"] = annotation_metadata["ThMass.Ion"]testX =  dbdi.export_to_spectra(ftints, 89)exporting.save_as_mgf(testX, filename = "example_dataset.mgf")os.getcwd()O1 = reslist["O"]O2 = reslist["O2"]O3 = reslist["O3"]H2O = reslist["H2O"]x = np.intersect1d(O3["base_index"], np.intersect1d(O1["base_index"],O2["base_index"]))a = np.intersect1d(x , H2O["base_index"])#%% plotting module IDs = [55,66,83,99]df = raw_imp.copy()transform = Truetest = dbdi.plot_adducts([55,66,83,99], df = raw_imp)test = dbdi.plot_adducts(IDs, df, metadata = annotation_metadata, transform = False)plot_adducts(2,2)test.gca().get_title()specs_aligned = specs_aligned.apply(lambda col:pd.to_numeric(col, errors='coerce'))#%% path = r'D:\Users\.....'path = path.replace('\\' , '/')feather.write_dataframe(raw_imp, "demo_filled.feather")os.getcwd()#%% for resubmissionintensities_raw = feather.read_dataframe("C:/Users/weidner.leopold/Documents/10_Publications/02_Online_Roasting/data-RiedFresh/2023-01-23-example_dataset-resubmission.feather")annotation_metadata = feather.read_dataframe("C:/Users/weidner.leopold/Documents/10_Publications/02_Online_Roasting/data-RiedFresh/2023-01-23-example__metadata2-resubmission.feather")IDs = annotation_metadata["ID"]intensities_raw = intensities_raw.drop("ID", axis = 1)raw_imp = dbdi.impute_intensities(intensities_raw, method = "linear")ca = pd.DataFrame({'deltamz': [47.984744, 63.979658], 'motive': ["O3", "O4"]})adducts095 =  dbdi.identify_adducts(raw_imp, annotation_metadata["ThMass.Ion"],                          custom_adducts = ca, method = "spearman", threshold = 0.95, mass_error = 5)searchres4plotting = {k:len(v) for k, v in adducts095.items()}#%% propose adductsx = propose_adducts(ID = 55, df = raw_imp,                 masses = annotation_metadata["ThMass.Ion"],                method = "pearson", threshold = 0.95,                 mass_error = 0.005,                custom_adducts =  pd.DataFrame({'mass_diff': [18.010565],                                                   'annotation': ["[M-XYX+H]+"]}))        #%% consensus spectrumfrom matchms import SpectrumtestX =  dbdi.export_to_spectra(ftints, 89)testX[0].peaks.mztestX[1].peaks.mztestX[0].peaks.intensitiestestX[1].peaks.intensitiesx = [testX[0], testX[1]]x[0].set("ms_level",1)x[1].set("ms_level",1)x[0].set("precursor_mz",55)x[1].set("precursor_mz",56)x[1].get("ms_level")x[1].metadataspectrum2 = Spectrum(mz=np.array([100, 150, 200.1002, 350.505]),                    intensities=np.array([0.7, 0.2, 0.1, 10]))spectrum3 = Spectrum(mz=np.array([100, 150.002, 200.2, 350.506]),                    intensities=np.array([0.8, 0.9, 0.8, 11]))spectrum4 = Spectrum(mz=np.array([100, 150.003, 200.1, 350.502]),                    intensities=np.array([0.1, 0.1, 0.05, 99]))x = [spectrum2, spectrum3, spectrum4]path_data = "/Users/lw/Nextcloud/Project212/src/data"  file_mgf = os.path.join(path_data, "fragment_spectra.mgf")spectrums = list(load_from_mgf(file_mgf))test = make_consensus_spectrum(spectrums, mzd = 0.005, minProp = 0.5,                                intensityFun = "sum", mzFun = "median")test.peaks.mztest.metadataspectrums[0].metadata
```

### Comparing `DBDIpy-1.2.1/DBDIpy/tests/test_align_spectra.py` & `DBDIpy-1.2.2/DBDIpy/tests/test_align_spectra.py`

 * *Files identical despite different names*

### Comparing `DBDIpy-1.2.1/DBDIpy/tests/test_identify_adducts.py` & `DBDIpy-1.2.2/DBDIpy/tests/test_identify_adducts.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,81 +9,81 @@
 ##test data is available under https://doi.org/10.5281/zenodo.7221089
 
 #%%trigger input errors
 
 def test_input_TypeErr():
     with pytest.raises(TypeError):
         annotation_metadata = feather.read_dataframe("C:/Users/weidner.leopold/Nextcloud/Project212/src/data/example_metadata.feather")
-        dbdi.identify_adducts([212], masses = annotation_metadata["ThMass.Ion"],
+        dbdi.identify_adducts_MS1([212], masses = annotation_metadata["ThMass.Ion"],
                               custom_adducts = None, method = "spearman", 
                               threshold = 0.90, mass_error = 2)
         
         
 def test_input_ValErr():
     with pytest.raises(ValueError):
         testdata = feather.read_dataframe("C:/Users/weidner.leopold/Nextcloud/Project212/src/data/example_dataset.feather")
         annotation_metadata = feather.read_dataframe("C:/Users/weidner.leopold/Nextcloud/Project212/src/data/example_metadata.feather")
         testdata = testdata.drop("ID", axis = 1)
         imputed = dbdi.impute_intensities(testdata, method = "linear")
-        dbdi.identify_adducts(df = imputed, masses = annotation_metadata["ThMass.Ion"][0:5],
+        dbdi.identify_adducts_MS1(df = imputed, masses = annotation_metadata["ThMass.Ion"][0:5],
                               custom_adducts = None, method = "spearman", 
                               threshold = 0.90, mass_error = 2)
 
 def test_input_NaN():
     with pytest.raises(ValueError):
         testdata = feather.read_dataframe("C:/Users/weidner.leopold/Nextcloud/Project212/src/data/example_dataset.feather")
         annotation_metadata = feather.read_dataframe("C:/Users/weidner.leopold/Nextcloud/Project212/src/data/example_metadata.feather")
         testdata = testdata.drop("ID", axis = 1)
         imputed = dbdi.impute_intensities(testdata, method = "linear")
         for c in range(1, imputed.shape[1]-1):
             imputed.iloc[random.randint(0, 99), c] = np.nan  
-        dbdi.identify_adducts(df = imputed, masses = annotation_metadata["ThMass.Ion"],
+        dbdi.identify_adducts_MS1(df = imputed, masses = annotation_metadata["ThMass.Ion"],
                               custom_adducts = None, method = "spearman", 
                               threshold = 0.90, mass_error = 2)
 
 def test_input_custadd():
     with pytest.raises(TypeError):
         testdata = feather.read_dataframe("C:/Users/weidner.leopold/Nextcloud/Project212/src/data/example_dataset.feather")
         annotation_metadata = feather.read_dataframe("C:/Users/weidner.leopold/Nextcloud/Project212/src/data/example_metadata.feather")
         testdata = testdata.drop("ID", axis = 1)
         imputed = dbdi.impute_intensities(testdata, method = "linear")
         ca = pd.DataFrame({'deltamz': [5],'motive': ["fail"], 'trash': ["trash"]})
-        dbdi.identify_adducts(df = imputed, masses = annotation_metadata["ThMass.Ion"],
+        dbdi.identify_adducts_MS1(df = imputed, masses = annotation_metadata["ThMass.Ion"],
                               custom_adducts = ca, method = "spearman", 
                               threshold = 0.90, mass_error = 2)
         
     with pytest.raises(TypeError):
         testdata = feather.read_dataframe("C:/Users/weidner.leopold/Nextcloud/Project212/src/data/example_dataset.feather")
         annotation_metadata = feather.read_dataframe("C:/Users/weidner.leopold/Nextcloud/Project212/src/data/example_metadata.feather")
         testdata = testdata.drop("ID", axis = 1)
         imputed = dbdi.impute_intensities(testdata, method = "linear")
         ca = {'deltamz': [5],'motive': ["fail"]}
-        dbdi.identify_adducts(df = imputed, masses = annotation_metadata["ThMass.Ion"],
+        dbdi.identify_adducts_MS1(df = imputed, masses = annotation_metadata["ThMass.Ion"],
                                  custom_adducts = ca, method = "spearman", 
                                  threshold = 0.90, mass_error = 2)
         
 def test_input_wrong_corr():
     with pytest.raises(ValueError):
         testdata = feather.read_dataframe("C:/Users/weidner.leopold/Nextcloud/Project212/src/data/example_dataset.feather")
         annotation_metadata = feather.read_dataframe("C:/Users/weidner.leopold/Nextcloud/Project212/src/data/example_metadata.feather")
         testdata = testdata.drop("ID", axis = 1)
         imputed = dbdi.impute_intensities(testdata, method = "linear")
-        dbdi.identify_adducts(df = imputed, masses = annotation_metadata["ThMass.Ion"],
+        dbdi.identify_adducts_MS1(df = imputed, masses = annotation_metadata["ThMass.Ion"],
                               custom_adducts = None, method = "trash", 
                               threshold = 0.90, mass_error = 2)
 
 #%% test output of function 
 def test_impute_outputn():
     testdata = feather.read_dataframe("C:/Users/weidner.leopold/Nextcloud/Project212/src/data/example_dataset.feather")
     annotation_metadata = feather.read_dataframe("C:/Users/weidner.leopold/Nextcloud/Project212/src/data/example_metadata.feather")
     testdata = testdata.drop("ID", axis = 1)
     imputed = dbdi.impute_intensities(testdata, method = "linear")
     trtest= 0.90
     ertest = 5
-    res_adductsearch =  dbdi.identify_adducts(df = imputed, masses = annotation_metadata["ThMass.Ion"],
+    res_adductsearch =  dbdi.identify_adducts_MS1(df = imputed, masses = annotation_metadata["ThMass.Ion"],
                                               threshold = trtest, mass_error = ertest)
     
     assert res_adductsearch is not None
     assert isinstance(res_adductsearch, dict)
     assert isinstance(list(res_adductsearch.values())[0], pd.DataFrame)
     assert all(list(res_adductsearch.values())[0]["corr"] > trtest)
     assert all((list(res_adductsearch.values())[0]["mzdiff"] <= 15.994915 + 15.994915 * ertest * 1e-6) &
```

### Comparing `DBDIpy-1.2.1/DBDIpy/tests/test_impute_intensities.py` & `DBDIpy-1.2.2/DBDIpy/tests/test_impute_intensities.py`

 * *Files identical despite different names*

### Comparing `DBDIpy-1.2.1/DBDIpy/tests/test_plot_adducts.py` & `DBDIpy-1.2.2/DBDIpy/tests/test_plot_adducts_XIC.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-import random import pandas as pdimport numpy as npimport DBDIpy as dbdiimport pytest#%%trigger input errorsdef test_type_errors_IDs():    with pytest.raises(TypeError):        testdata = pd.DataFrame(np.random.randint(100, 1000000, size = (100, 100)))                dbdi.plot_adducts(IDs = {}, df = testdata)        def test_type_errors_df():    with pytest.raises(TypeError):        testID = random.sample(range(1, 99), 3)                dbdi.plot_adducts(IDs = testID, df = np.zeros(shape=(100, 100)))        def test_name_errors_metadata():    with pytest.raises(NameError):        meta = pd.DataFrame(np.random.randint(0, 10, size = (5, 5)), columns = list('ABCDE'))        testdata = pd.DataFrame(np.random.randint(100, 1000000, size = (100, 100)))        testID = random.sample(range(1, 99), 3)        dbdi.plot_adducts(testID, testdata, metadata = meta, transform = False)     def test_nan_error():    with pytest.raises(ValueError):        testdata = pd.DataFrame(np.random.randint(100, 1000000, size = (100, 100)))        testdata.iloc[random.randint(1,99), random.randint(1,99)] = np.nan        testID = random.sample(range(1, 99), 3)        dbdi.plot_adducts(testID, testdata, metadata = None, transform = False)        #%%test for correct outputdef test_plot_adducts_non_scaled():        testID = random.sample(range(1, 99), 3)    testdata = pd.DataFrame(np.random.randint(100, 1000000, size = (100, 100)))    fig = dbdi.plot_adducts(testID, testdata, metadata = None, transform = False)     assert fig is not None    def test_plot_adducts_scaled():        testID = random.sample(range(1, 99), 3)    testdata = pd.DataFrame(np.random.randint(100, 1000000, size = (100, 100)))    fig = dbdi.plot_adducts(testID, testdata, metadata = None, transform = True)    assert fig is not None
+import random import pandas as pdimport numpy as npimport DBDIpy as dbdiimport pytest#%%trigger input errorsdef test_type_errors_IDs():    with pytest.raises(TypeError):        testdata = pd.DataFrame(np.random.randint(100, 1000000, size = (100, 100)))                dbdi.plot_adducts_XIC(IDs = {}, df = testdata)        def test_type_errors_df():    with pytest.raises(TypeError):        testID = random.sample(range(1, 99), 3)                dbdi.plot_adducts_XIC(IDs = testID, df = np.zeros(shape=(100, 100)))        def test_name_errors_metadata():    with pytest.raises(NameError):        meta = pd.DataFrame(np.random.randint(0, 10, size = (5, 5)), columns = list('ABCDE'))        testdata = pd.DataFrame(np.random.randint(100, 1000000, size = (100, 100)))        testID = random.sample(range(1, 99), 3)        dbdi.plot_adducts_XIC(testID, testdata, metadata = meta, transform = False)     def test_nan_error():    with pytest.raises(ValueError):        testdata = pd.DataFrame(np.random.randint(100, 1000000, size = (100, 100)))        testdata.iloc[random.randint(1,99), random.randint(1,99)] = np.nan        testID = random.sample(range(1, 99), 3)        dbdi.plot_adducts_XIC(testID, testdata, metadata = None, transform = False)        #%%test for correct outputdef test_plot_adducts_non_scaled():        testID = random.sample(range(1, 99), 3)    testdata = pd.DataFrame(np.random.randint(100, 1000000, size = (100, 100)))    fig = dbdi.plot_adducts_XIC(testID, testdata, metadata = None, transform = False)     assert fig is not None    def test_plot_adducts_scaled():        testID = random.sample(range(1, 99), 3)    testdata = pd.DataFrame(np.random.randint(100, 1000000, size = (100, 100)))    fig = dbdi.plot_adducts_XIC(testID, testdata, metadata = None, transform = True)    assert fig is not None
```

### Comparing `DBDIpy-1.2.1/DBDIpy/tests/test_propose_adducts.py` & `DBDIpy-1.2.2/DBDIpy/tests/test_propose_adducts.py`

 * *Files identical despite different names*

### Comparing `DBDIpy-1.2.1/DBDIpy.egg-info/PKG-INFO` & `DBDIpy-1.2.2/DBDIpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DBDIpy
-Version: 1.2.1
+Version: 1.2.2
 Summary: A python package for the curation and interpretation of datasets from plasma ionisation mass spectrometric.
 Home-page: https://github.com/leopold-weidner/DBDIpy
 Author: Leopold Weidner
 Author-email: leopold.weidner@tum.de
 License: docs/license.txt
 Keywords: python,bioinformatics,mass spectrometry,metabolomics,foodomics
 Classifier: Intended Audience :: Developers
@@ -14,29 +14,29 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
-# DBDIpy (Version 1.2.1)
+# DBDIpy (Version 1.2.2)
 DBDIpy is an open-source Python library for the curation and interpretation of dielectric barrier discharge ionisation mass spectrometric datasets.
 
 # Introduction
 
 Mass spectrometric data from direct injection analysis is hard to interpret as missing chromatographic separation complicates identification of fragments and adducts generated during the ionization process.
 
 Here we present an *in-silico* approach to putatively identify multiple ion species arising from one analyte compound specially tailored for time-resolved datasets from plasma ionization techniques. These are rapidly gaining popularity in applications as breath analysis, process control or food research. 
 
 DBDIpy's core functionality relys on putative identification of in-source fragments (eg. [M-H<sub>2</sub>O+H]<sup>+</sup>) and in-source generated adducts (eg. [M+nO+H]<sup>+</sup>). 
-Custom adduct species can be defined by the user and passed to this open-search algorithm. The identification is performed in a two-step procedure: 
+Custom adduct species can be defined by the user and passed to this open-search algorithm. The identification is performed in a three-step procedure (from V > 2.* on, in preparation): 
 - calculation of pointwise correlation identifies features with matching temporal intensity profiles through the experiment.
 - (exact) mass differences are used to refine the nature of potential candidates. 
-
-These putative identifications can than further be validated by the user, eg. based on tandem MS fragmentation or IMS data.              
+- calculation of MS2 spectral similarity score by ...
+       
 
 DBDIpy further comes along with functions optimized for preprocessing of experimental data and visualization of identified adducts. The library is integrated into the matchms ecosystem to assimilate DBDIpy's functionalities into existing workflows.
 
 For details, we invite you to read the [tutorial](#tutorial) or to try out the functions with our [demonstrational dataset](https://doi.org/10.5281/zenodo.7221089) or your own data!
 
 
 |                     | Badges                                                                             |
@@ -44,28 +44,31 @@
 | `License`           | [![PyPi license](https://badgen.net/pypi/license/pip/)]([https://pypi.com/project/pip/](https://opensource.org/licenses/MIT/))|
 | `Version`           | [![PyPi license](https://img.shields.io/pypi/v/DBDIpy)](https://pypi.org/project/DBDIpy/)|
 | `Downloads`         | [![Downloads](https://static.pepy.tech/badge/dbdipy/week)](https://pepy.tech/project/dbdipy)|
 | `Status`            | [![test](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/leopold-weidner/DBDIpy/graphs/commit-activity)|
 | `Updated`           | ![latest commit](https://img.shields.io/github/last-commit/leopold-weidner/DBDIpy)|
 | `Language`          | [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)|
 | `Version`           | [![Python - 3.7, 3.8, 3.9, 3.10](https://img.shields.io/static/v1?label=Python&message=3.7+,+3.8+,+3.9+,+3.10&color=2d4b65)](https://www.python.org/)|
-| `Operating Systems` | [![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg) [![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)|
+| `Operating Systems` | ![macOS](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=macos&logoColor=F0F0F0) ![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)|
 | `Documentation`     | [![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://github.com/leopold-weidner/DBDIpy)|
 | `Supporting Data`   | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7221089.svg)](https://doi.org/10.5281/zenodo.7221089)|
 | `Articel (open access)`     | [![DOI](https://img.shields.io/badge/DOI-10.1093%2Fbioinformatics%2Fbtad088-blue)](https://doi.org/10.1093/bioinformatics/btad088)|
 
 
-Latest Changes (since 1.1.0)
+Latest Changes (since V 1.2.1)
 ------------
-- new functionality to propose potential adducts / in-source fragments.
-- minor fixes.
+minor fixes
+
 
 Currently under development:
 ------------
-- implementation of MS2 spectral similarity matching to improve adduct detection.
+- major implementation for V2: modification of the former two-step search algorithm towards refinement by MS2 spectral similarity scoring.
+- addition of utility functions, e.g. calculation of consensus spectra.
+- improved spectral alignment.
+- introduction of an open search option to propose potential adducts / in-source fragments.
 - runtime optimization.
 
 
 
 User guide
 ============
 
@@ -165,15 +168,15 @@
 ```python
 ##check if NaN are present in DataFrame
 specs_imputed.isnull().values.any()
 Out[]: False
 ```
 
 
-### 3. Detection of adducts and in-source fragments
+### 3. Detection of adducts and in-source fragments: MS1 data only
 
 Based on the ``specs_imputed``, we compute pointwise correlation of XIC traces to identify in-source adducts or in-source fragments generated during the plasma ionization process. The identification is performed in a two-step procedure: 
 - First, calculation of pointwise intensity correlation identifies feature groups with matching temporal intensity profiles through the experiment.
 - Second, (exact) mass differences are used to refine the nature of potential candidates. 
 
 By default, ``identify_adducts()`` searches for [M-H<sub>2</sub>O+H]<sup>+</sup>, [M+1O+H]<sup>+</sup> and [M+2O+H]<sup>+</sup>. 
 For demonstrational purposes we also want to search for [M+3O+H]<sup>+</sup> in this example.
@@ -237,15 +240,19 @@
 Out[33]: array([55, 99], dtype=int64)
 ```
 
 This tells us that features 55 and 99 both putatively have [M+1-3O+H]<sup>+</sup> adduct ions with correlations of  r > 0.9 in our dataset.
 Let's visualize this finding!
 
 
-### 4. Visualization of correlation results
+### 4. Detection of adducts and in-source fragments: refined scoring by MS2 similarity matching
+...
+
+
+### 5. Visualization of correlation results
 
 Now that we putatively identified some related ions of a single analyte, we want to check their temporal response during the baking experiment.
 Therefore, we can use the ``plot_adducts()`` function to conveniently draw XICs.
 The demo dataset even comes along with some annotated metadata for our features, so we can decorate the plot and check our previous results!
 
 ```python
 ##load annotation metadta
@@ -266,15 +273,15 @@
 </p>
 
 We see that the XIC traces show a similar intensity profile through the experiment. The plot further tells us the correlation coefficients of the identified adducts.
 From the metadata we can see that the detected mass signals were previously annotated as C<sub>15</sub>H<sub>17</sub>O<sub>2-5</sub>N which tells us that we most probably found an Oxgen-adduct series. 
 
 If MS2 data was recorded during the experiment we now can go on further and compare fragment spectra to reassure the identifications. You might find [ms2deepscore](https://github.com/matchms/ms2deepscore) to be a usefull library to do so in an automated way. 
 
-### 5. Exporting tabular MS data to match.Spectra objects
+### 6. Exporting tabular MS data to match.Spectra objects
 
 If you want to export your (imputed) tabular data to ``matchms.Spectra`` objects, you can do so by calling the ``export_to_spectra()`` function. We just need to re-add a column containing *m/z* values of the features.
 This gives you access to the matchms suite and enables you to safe your mass spectrometric data to open file formats.
 Hint: you can manually add some metadata after construction of the list of spectra.  
 
 ```python
 ##export tabular MS data back to list of spectrums.
```

### Comparing `DBDIpy-1.2.1/DBDIpy.egg-info/SOURCES.txt` & `DBDIpy-1.2.2/DBDIpy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 README.md
 setup.py
 DBDIpy/__init__.py
 DBDIpy/align_spectra.py
+DBDIpy/dbdipy_auxiliaries.py
 DBDIpy/export_to_spectra.py
 DBDIpy/identify_adducts.py
 DBDIpy/impute_intensities.py
-DBDIpy/plot_adducts.py
+DBDIpy/plot_adducts_MS2.py
+DBDIpy/plot_adducts_XIC.py
 DBDIpy/propose_adducts.py
 DBDIpy.egg-info/PKG-INFO
 DBDIpy.egg-info/SOURCES.txt
 DBDIpy.egg-info/dependency_links.txt
 DBDIpy.egg-info/requires.txt
 DBDIpy.egg-info/top_level.txt
 DBDIpy/tests/testLW.py
 DBDIpy/tests/test_align_spectra.py
 DBDIpy/tests/test_identify_adducts.py
 DBDIpy/tests/test_impute_intensities.py
-DBDIpy/tests/test_plot_adducts.py
+DBDIpy/tests/test_plot_adducts_MS2.py
+DBDIpy/tests/test_plot_adducts_XIC.py
 DBDIpy/tests/test_propose_adducts.py
```

### Comparing `DBDIpy-1.2.1/PKG-INFO` & `DBDIpy-1.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DBDIpy
-Version: 1.2.1
+Version: 1.2.2
 Summary: A python package for the curation and interpretation of datasets from plasma ionisation mass spectrometric.
 Home-page: https://github.com/leopold-weidner/DBDIpy
 Author: Leopold Weidner
 Author-email: leopold.weidner@tum.de
 License: docs/license.txt
 Keywords: python,bioinformatics,mass spectrometry,metabolomics,foodomics
 Classifier: Intended Audience :: Developers
@@ -14,29 +14,29 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
-# DBDIpy (Version 1.2.1)
+# DBDIpy (Version 1.2.2)
 DBDIpy is an open-source Python library for the curation and interpretation of dielectric barrier discharge ionisation mass spectrometric datasets.
 
 # Introduction
 
 Mass spectrometric data from direct injection analysis is hard to interpret as missing chromatographic separation complicates identification of fragments and adducts generated during the ionization process.
 
 Here we present an *in-silico* approach to putatively identify multiple ion species arising from one analyte compound specially tailored for time-resolved datasets from plasma ionization techniques. These are rapidly gaining popularity in applications as breath analysis, process control or food research. 
 
 DBDIpy's core functionality relys on putative identification of in-source fragments (eg. [M-H<sub>2</sub>O+H]<sup>+</sup>) and in-source generated adducts (eg. [M+nO+H]<sup>+</sup>). 
-Custom adduct species can be defined by the user and passed to this open-search algorithm. The identification is performed in a two-step procedure: 
+Custom adduct species can be defined by the user and passed to this open-search algorithm. The identification is performed in a three-step procedure (from V > 2.* on, in preparation): 
 - calculation of pointwise correlation identifies features with matching temporal intensity profiles through the experiment.
 - (exact) mass differences are used to refine the nature of potential candidates. 
-
-These putative identifications can than further be validated by the user, eg. based on tandem MS fragmentation or IMS data.              
+- calculation of MS2 spectral similarity score by ...
+       
 
 DBDIpy further comes along with functions optimized for preprocessing of experimental data and visualization of identified adducts. The library is integrated into the matchms ecosystem to assimilate DBDIpy's functionalities into existing workflows.
 
 For details, we invite you to read the [tutorial](#tutorial) or to try out the functions with our [demonstrational dataset](https://doi.org/10.5281/zenodo.7221089) or your own data!
 
 
 |                     | Badges                                                                             |
@@ -44,28 +44,31 @@
 | `License`           | [![PyPi license](https://badgen.net/pypi/license/pip/)]([https://pypi.com/project/pip/](https://opensource.org/licenses/MIT/))|
 | `Version`           | [![PyPi license](https://img.shields.io/pypi/v/DBDIpy)](https://pypi.org/project/DBDIpy/)|
 | `Downloads`         | [![Downloads](https://static.pepy.tech/badge/dbdipy/week)](https://pepy.tech/project/dbdipy)|
 | `Status`            | [![test](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/leopold-weidner/DBDIpy/graphs/commit-activity)|
 | `Updated`           | ![latest commit](https://img.shields.io/github/last-commit/leopold-weidner/DBDIpy)|
 | `Language`          | [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)|
 | `Version`           | [![Python - 3.7, 3.8, 3.9, 3.10](https://img.shields.io/static/v1?label=Python&message=3.7+,+3.8+,+3.9+,+3.10&color=2d4b65)](https://www.python.org/)|
-| `Operating Systems` | [![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg) [![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)|
+| `Operating Systems` | ![macOS](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=macos&logoColor=F0F0F0) ![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)|
 | `Documentation`     | [![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://github.com/leopold-weidner/DBDIpy)|
 | `Supporting Data`   | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7221089.svg)](https://doi.org/10.5281/zenodo.7221089)|
 | `Articel (open access)`     | [![DOI](https://img.shields.io/badge/DOI-10.1093%2Fbioinformatics%2Fbtad088-blue)](https://doi.org/10.1093/bioinformatics/btad088)|
 
 
-Latest Changes (since 1.1.0)
+Latest Changes (since V 1.2.1)
 ------------
-- new functionality to propose potential adducts / in-source fragments.
-- minor fixes.
+minor fixes
+
 
 Currently under development:
 ------------
-- implementation of MS2 spectral similarity matching to improve adduct detection.
+- major implementation for V2: modification of the former two-step search algorithm towards refinement by MS2 spectral similarity scoring.
+- addition of utility functions, e.g. calculation of consensus spectra.
+- improved spectral alignment.
+- introduction of an open search option to propose potential adducts / in-source fragments.
 - runtime optimization.
 
 
 
 User guide
 ============
 
@@ -165,15 +168,15 @@
 ```python
 ##check if NaN are present in DataFrame
 specs_imputed.isnull().values.any()
 Out[]: False
 ```
 
 
-### 3. Detection of adducts and in-source fragments
+### 3. Detection of adducts and in-source fragments: MS1 data only
 
 Based on the ``specs_imputed``, we compute pointwise correlation of XIC traces to identify in-source adducts or in-source fragments generated during the plasma ionization process. The identification is performed in a two-step procedure: 
 - First, calculation of pointwise intensity correlation identifies feature groups with matching temporal intensity profiles through the experiment.
 - Second, (exact) mass differences are used to refine the nature of potential candidates. 
 
 By default, ``identify_adducts()`` searches for [M-H<sub>2</sub>O+H]<sup>+</sup>, [M+1O+H]<sup>+</sup> and [M+2O+H]<sup>+</sup>. 
 For demonstrational purposes we also want to search for [M+3O+H]<sup>+</sup> in this example.
@@ -237,15 +240,19 @@
 Out[33]: array([55, 99], dtype=int64)
 ```
 
 This tells us that features 55 and 99 both putatively have [M+1-3O+H]<sup>+</sup> adduct ions with correlations of  r > 0.9 in our dataset.
 Let's visualize this finding!
 
 
-### 4. Visualization of correlation results
+### 4. Detection of adducts and in-source fragments: refined scoring by MS2 similarity matching
+...
+
+
+### 5. Visualization of correlation results
 
 Now that we putatively identified some related ions of a single analyte, we want to check their temporal response during the baking experiment.
 Therefore, we can use the ``plot_adducts()`` function to conveniently draw XICs.
 The demo dataset even comes along with some annotated metadata for our features, so we can decorate the plot and check our previous results!
 
 ```python
 ##load annotation metadta
@@ -266,15 +273,15 @@
 </p>
 
 We see that the XIC traces show a similar intensity profile through the experiment. The plot further tells us the correlation coefficients of the identified adducts.
 From the metadata we can see that the detected mass signals were previously annotated as C<sub>15</sub>H<sub>17</sub>O<sub>2-5</sub>N which tells us that we most probably found an Oxgen-adduct series. 
 
 If MS2 data was recorded during the experiment we now can go on further and compare fragment spectra to reassure the identifications. You might find [ms2deepscore](https://github.com/matchms/ms2deepscore) to be a usefull library to do so in an automated way. 
 
-### 5. Exporting tabular MS data to match.Spectra objects
+### 6. Exporting tabular MS data to match.Spectra objects
 
 If you want to export your (imputed) tabular data to ``matchms.Spectra`` objects, you can do so by calling the ``export_to_spectra()`` function. We just need to re-add a column containing *m/z* values of the features.
 This gives you access to the matchms suite and enables you to safe your mass spectrometric data to open file formats.
 Hint: you can manually add some metadata after construction of the list of spectra.  
 
 ```python
 ##export tabular MS data back to list of spectrums.
```

### Comparing `DBDIpy-1.2.1/README.md` & `DBDIpy-1.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# DBDIpy (Version 1.2.1)
+# DBDIpy (Version 1.2.2)
 DBDIpy is an open-source Python library for the curation and interpretation of dielectric barrier discharge ionisation mass spectrometric datasets.
 
 # Introduction
 
 Mass spectrometric data from direct injection analysis is hard to interpret as missing chromatographic separation complicates identification of fragments and adducts generated during the ionization process.
 
 Here we present an *in-silico* approach to putatively identify multiple ion species arising from one analyte compound specially tailored for time-resolved datasets from plasma ionization techniques. These are rapidly gaining popularity in applications as breath analysis, process control or food research. 
 
 DBDIpy's core functionality relys on putative identification of in-source fragments (eg. [M-H<sub>2</sub>O+H]<sup>+</sup>) and in-source generated adducts (eg. [M+nO+H]<sup>+</sup>). 
-Custom adduct species can be defined by the user and passed to this open-search algorithm. The identification is performed in a two-step procedure: 
+Custom adduct species can be defined by the user and passed to this open-search algorithm. The identification is performed in a three-step procedure (from V > 2.* on, in preparation): 
 - calculation of pointwise correlation identifies features with matching temporal intensity profiles through the experiment.
 - (exact) mass differences are used to refine the nature of potential candidates. 
-
-These putative identifications can than further be validated by the user, eg. based on tandem MS fragmentation or IMS data.              
+- calculation of MS2 spectral similarity score by ...
+       
 
 DBDIpy further comes along with functions optimized for preprocessing of experimental data and visualization of identified adducts. The library is integrated into the matchms ecosystem to assimilate DBDIpy's functionalities into existing workflows.
 
 For details, we invite you to read the [tutorial](#tutorial) or to try out the functions with our [demonstrational dataset](https://doi.org/10.5281/zenodo.7221089) or your own data!
 
 
 |                     | Badges                                                                             |
@@ -24,28 +24,31 @@
 | `License`           | [![PyPi license](https://badgen.net/pypi/license/pip/)]([https://pypi.com/project/pip/](https://opensource.org/licenses/MIT/))|
 | `Version`           | [![PyPi license](https://img.shields.io/pypi/v/DBDIpy)](https://pypi.org/project/DBDIpy/)|
 | `Downloads`         | [![Downloads](https://static.pepy.tech/badge/dbdipy/week)](https://pepy.tech/project/dbdipy)|
 | `Status`            | [![test](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/leopold-weidner/DBDIpy/graphs/commit-activity)|
 | `Updated`           | ![latest commit](https://img.shields.io/github/last-commit/leopold-weidner/DBDIpy)|
 | `Language`          | [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)|
 | `Version`           | [![Python - 3.7, 3.8, 3.9, 3.10](https://img.shields.io/static/v1?label=Python&message=3.7+,+3.8+,+3.9+,+3.10&color=2d4b65)](https://www.python.org/)|
-| `Operating Systems` | [![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg) [![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)|
+| `Operating Systems` | ![macOS](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=macos&logoColor=F0F0F0) ![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)|
 | `Documentation`     | [![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://github.com/leopold-weidner/DBDIpy)|
 | `Supporting Data`   | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7221089.svg)](https://doi.org/10.5281/zenodo.7221089)|
 | `Articel (open access)`     | [![DOI](https://img.shields.io/badge/DOI-10.1093%2Fbioinformatics%2Fbtad088-blue)](https://doi.org/10.1093/bioinformatics/btad088)|
 
 
-Latest Changes (since 1.1.0)
+Latest Changes (since V 1.2.1)
 ------------
-- new functionality to propose potential adducts / in-source fragments.
-- minor fixes.
+minor fixes
+
 
 Currently under development:
 ------------
-- implementation of MS2 spectral similarity matching to improve adduct detection.
+- major implementation for V2: modification of the former two-step search algorithm towards refinement by MS2 spectral similarity scoring.
+- addition of utility functions, e.g. calculation of consensus spectra.
+- improved spectral alignment.
+- introduction of an open search option to propose potential adducts / in-source fragments.
 - runtime optimization.
 
 
 
 User guide
 ============
 
@@ -145,15 +148,15 @@
 ```python
 ##check if NaN are present in DataFrame
 specs_imputed.isnull().values.any()
 Out[]: False
 ```
 
 
-### 3. Detection of adducts and in-source fragments
+### 3. Detection of adducts and in-source fragments: MS1 data only
 
 Based on the ``specs_imputed``, we compute pointwise correlation of XIC traces to identify in-source adducts or in-source fragments generated during the plasma ionization process. The identification is performed in a two-step procedure: 
 - First, calculation of pointwise intensity correlation identifies feature groups with matching temporal intensity profiles through the experiment.
 - Second, (exact) mass differences are used to refine the nature of potential candidates. 
 
 By default, ``identify_adducts()`` searches for [M-H<sub>2</sub>O+H]<sup>+</sup>, [M+1O+H]<sup>+</sup> and [M+2O+H]<sup>+</sup>. 
 For demonstrational purposes we also want to search for [M+3O+H]<sup>+</sup> in this example.
@@ -217,15 +220,19 @@
 Out[33]: array([55, 99], dtype=int64)
 ```
 
 This tells us that features 55 and 99 both putatively have [M+1-3O+H]<sup>+</sup> adduct ions with correlations of  r > 0.9 in our dataset.
 Let's visualize this finding!
 
 
-### 4. Visualization of correlation results
+### 4. Detection of adducts and in-source fragments: refined scoring by MS2 similarity matching
+...
+
+
+### 5. Visualization of correlation results
 
 Now that we putatively identified some related ions of a single analyte, we want to check their temporal response during the baking experiment.
 Therefore, we can use the ``plot_adducts()`` function to conveniently draw XICs.
 The demo dataset even comes along with some annotated metadata for our features, so we can decorate the plot and check our previous results!
 
 ```python
 ##load annotation metadta
@@ -246,15 +253,15 @@
 </p>
 
 We see that the XIC traces show a similar intensity profile through the experiment. The plot further tells us the correlation coefficients of the identified adducts.
 From the metadata we can see that the detected mass signals were previously annotated as C<sub>15</sub>H<sub>17</sub>O<sub>2-5</sub>N which tells us that we most probably found an Oxgen-adduct series. 
 
 If MS2 data was recorded during the experiment we now can go on further and compare fragment spectra to reassure the identifications. You might find [ms2deepscore](https://github.com/matchms/ms2deepscore) to be a usefull library to do so in an automated way. 
 
-### 5. Exporting tabular MS data to match.Spectra objects
+### 6. Exporting tabular MS data to match.Spectra objects
 
 If you want to export your (imputed) tabular data to ``matchms.Spectra`` objects, you can do so by calling the ``export_to_spectra()`` function. We just need to re-add a column containing *m/z* values of the features.
 This gives you access to the matchms suite and enables you to safe your mass spectrometric data to open file formats.
 Hint: you can manually add some metadata after construction of the list of spectra.  
 
 ```python
 ##export tabular MS data back to list of spectrums.
```

### Comparing `DBDIpy-1.2.1/setup.py` & `DBDIpy-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
    name = 'DBDIpy',
-   version = '1.2.1',
+   version = '1.2.2',
    author = 'Leopold Weidner',
    author_email = 'leopold.weidner@tum.de',
    packages = ['DBDIpy', 'DBDIpy.tests'],
    url = 'https://github.com/leopold-weidner/DBDIpy',
    license = 'docs/license.txt',
    description =    'A python package for the curation and interpretation of datasets from plasma ionisation mass spectrometric.',
    long_description_content_type='text/markdown',
```

