# Comparing `tmp/bacteria-1.4.0.tar.gz` & `tmp/bacteria-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacteria-1.4.0.tar", last modified: Sun Jul  2 10:17:16 2023, max compression
+gzip compressed data, was "bacteria-1.5.0.tar", last modified: Mon Jul  3 20:09:23 2023, max compression
```

## Comparing `bacteria-1.4.0.tar` & `bacteria-1.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 10:17:16.698000 bacteria-1.4.0/
--rw-rw-rw-   0        0        0      593 2023-07-02 10:17:16.474000 bacteria-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      826 2023-07-02 10:17:02.000000 bacteria-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 10:17:15.242000 bacteria-1.4.0/bacteria/
--rw-rw-rw-   0        0        0       34 2023-04-27 16:19:58.000000 bacteria-1.4.0/bacteria/__init__.py
--rw-rw-rw-   0        0        0   147859 2023-07-02 10:14:13.000000 bacteria-1.4.0/bacteria/functions.py
-drwxrwxrwx   0        0        0        0 2023-07-02 10:17:16.379000 bacteria-1.4.0/bacteria.egg-info/
--rw-rw-rw-   0        0        0      593 2023-07-02 10:17:12.000000 bacteria-1.4.0/bacteria.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-07-02 10:17:12.000000 bacteria-1.4.0/bacteria.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 10:17:12.000000 bacteria-1.4.0/bacteria.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-07-02 10:17:12.000000 bacteria-1.4.0/bacteria.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-02 10:17:12.000000 bacteria-1.4.0/bacteria.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 10:17:16.666000 bacteria-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1096 2023-07-02 10:16:39.000000 bacteria-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 20:09:22.915000 bacteria-1.5.0/
+-rw-rw-rw-   0        0        0      593 2023-07-03 20:09:22.474000 bacteria-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      826 2023-07-02 10:17:02.000000 bacteria-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 20:09:20.316000 bacteria-1.5.0/bacteria/
+-rw-rw-rw-   0        0        0       34 2023-04-27 16:19:58.000000 bacteria-1.5.0/bacteria/__init__.py
+-rw-rw-rw-   0        0        0   147845 2023-07-03 20:08:16.000000 bacteria-1.5.0/bacteria/functions.py
+drwxrwxrwx   0        0        0        0 2023-07-03 20:09:22.279000 bacteria-1.5.0/bacteria.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-07-03 20:09:13.000000 bacteria-1.5.0/bacteria.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-07-03 20:09:15.000000 bacteria-1.5.0/bacteria.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 20:09:13.000000 bacteria-1.5.0/bacteria.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-07-03 20:09:14.000000 bacteria-1.5.0/bacteria.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-03 20:09:15.000000 bacteria-1.5.0/bacteria.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 20:09:22.798000 bacteria-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1096 2023-07-03 20:08:39.000000 bacteria-1.5.0/setup.py
```

### Comparing `bacteria-1.4.0/PKG-INFO` & `bacteria-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 1.4.0
+Version: 1.5.0
 Summary: Super Segger Analysis in Python.
 Home-page: https://bacteria.readthedocs.io
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-1.4.0/README.md` & `bacteria-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `bacteria-1.4.0/bacteria/functions.py` & `bacteria-1.5.0/bacteria/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,15 +458,15 @@
         If True the lentgh filter will be used. If True
         alongised with 'daughter' the two filters will be used
     plot : bool (optional)
         Plot the histogram pre and pos filter the data
         
     Returns
     --------------
-    df_2d : DataFrame
+    df_2d : DataFramef
         Filtered DataFrame of 2D data
     df_3d : DataFrame
         Filtered DataFrame of 3D data
     gc_filter : nd.array
         Array with good cells ID after filter
     """
 
@@ -1241,37 +1241,37 @@
         
     Returns
     --------------
     time : nd.array
         1D time vector with the uniques time points (fps)
     mean : nd.array
         1D time vector with the mean for 
-        each time point
+        each time points
     ci : nd.array
         array(2,bins) with inferior Confidence
         Interval in the first column and the 
     """
     len_data = []
     times = natsorted(set(df['Time (fps)'].values))
     mean = np.zeros((len(times),))
     ci = np.zeros((len(times),2))
 
     for idx,ts in enumerate(times):
         temp = df[df['Time (fps)']==ts][column].values
         mean[idx] = np.mean(temp)
         len_data.append(len(df[df['Time (fps)']==ts][column].values))
         if len(temp) > 1:
-            ci[idx,:] = bac.ci_bootstrap(temp,conf = conf, method = method, plot = False)
+            ci[idx,:] = ci_bootstrap(temp,conf = conf, method = method, plot = False)
         else:
             ci[idx,:] = [-temp[0],+temp[0]]
 
     if smooth:
-        mean = bac.smooth(mean,10)
-        ci[:,0] =  bac.smooth(ci[:,0],10)
-        ci[:,1] =  bac.smooth(ci[:,1],10)
+        mean = smooth(mean,10)
+        ci[:,0] =  smooth(ci[:,0],10)
+        ci[:,1] =  smooth(ci[:,1],10)
 
     if plot_hist:
         plt.hist(len_data)
         plt.ylabel('Amount of time points')
         plt.xlabel('len(derivative)')
         plt.show()
```

### Comparing `bacteria-1.4.0/bacteria.egg-info/PKG-INFO` & `bacteria-1.5.0/bacteria.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 1.4.0
+Version: 1.5.0
 Summary: Super Segger Analysis in Python.
 Home-page: https://bacteria.readthedocs.io
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-1.4.0/setup.py` & `bacteria-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
  
 with open("README.md", "r") as fh:
     long_description = fh.read()
   
 setuptools.setup(
     name = 'bacteria',         
     packages = ['bacteria'],   
-    version = '1.4.0',      
+    version = '1.5.0',      
     license='MIT',       
     description = 'Super Segger Analysis in Python.',
     long_description_content_type="text/x-rst",
     url = 'https://bacteria.readthedocs.io',  
     download_url = 'https://github.com/tuliofalmeida/bacteria',    
     keywords = ['Data analysis', 'Cell analysis', 'Bacteria', 'SuperSegger'],   
     install_requires=[
```

