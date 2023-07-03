# Comparing `tmp/skysurvey-0.7.1.tar.gz` & `tmp/skysurvey-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skysurvey-0.7.1.tar", last modified: Fri Jun 30 09:22:08 2023, max compression
+gzip compressed data, was "skysurvey-0.7.3.tar", last modified: Mon Jul  3 08:29:37 2023, max compression
```

## Comparing `skysurvey-0.7.1.tar` & `skysurvey-0.7.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-30 09:22:08.109190 skysurvey-0.7.1/
--rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-08-10 14:40:58.000000 skysurvey-0.7.1/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      747 2023-06-30 09:22:08.109241 skysurvey-0.7.1/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)     2136 2023-06-30 08:24:06.000000 skysurvey-0.7.1/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)     1205 2023-06-30 09:22:08.109530 skysurvey-0.7.1/setup.cfg
--rw-r--r--   0 rigault   (2358) staff       (20)       37 2023-06-12 09:49:45.000000 skysurvey-0.7.1/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-30 09:22:08.104800 skysurvey-0.7.1/skysurvey/
--rw-r--r--   0 rigault   (2358) staff       (20)       90 2023-06-30 09:21:49.000000 skysurvey-0.7.1/skysurvey/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)      524 2023-06-27 13:24:20.000000 skysurvey-0.7.1/skysurvey/config.py
--rw-r--r--   0 rigault   (2358) staff       (20)    27899 2023-06-29 09:38:43.000000 skysurvey-0.7.1/skysurvey/dataset.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-30 09:22:08.106149 skysurvey-0.7.1/skysurvey/examples/
--rw-r--r--   0 rigault   (2358) staff       (20)       26 2023-06-29 14:59:14.000000 skysurvey-0.7.1/skysurvey/examples/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2233 2023-06-29 14:59:29.000000 skysurvey-0.7.1/skysurvey/examples/mocksurvey.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-30 09:22:08.107007 skysurvey-0.7.1/skysurvey/survey/
--rw-r--r--   0 rigault   (2358) staff       (20)      125 2023-06-28 15:34:39.000000 skysurvey-0.7.1/skysurvey/survey/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)     9538 2023-06-29 14:45:35.000000 skysurvey-0.7.1/skysurvey/survey/core.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2849 2023-06-29 07:52:19.000000 skysurvey-0.7.1/skysurvey/survey/des.py
--rw-r--r--   0 rigault   (2358) staff       (20)    15609 2023-06-29 13:44:29.000000 skysurvey-0.7.1/skysurvey/survey/healpix.py
--rw-r--r--   0 rigault   (2358) staff       (20)      976 2023-06-30 08:20:21.000000 skysurvey-0.7.1/skysurvey/survey/lsst.py
--rw-r--r--   0 rigault   (2358) staff       (20)    13238 2023-06-29 13:35:29.000000 skysurvey-0.7.1/skysurvey/survey/polygon.py
--rw-r--r--   0 rigault   (2358) staff       (20)     8955 2023-06-29 09:16:04.000000 skysurvey-0.7.1/skysurvey/survey/survey.py
--rw-r--r--   0 rigault   (2358) staff       (20)     1938 2023-06-29 13:30:27.000000 skysurvey-0.7.1/skysurvey/survey/ztf.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-30 09:22:08.108790 skysurvey-0.7.1/skysurvey/target/
--rw-r--r--   0 rigault   (2358) staff       (20)      113 2023-05-05 08:46:40.000000 skysurvey-0.7.1/skysurvey/target/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)    11766 2023-05-05 08:45:44.000000 skysurvey-0.7.1/skysurvey/target/collection.py
--rw-r--r--   0 rigault   (2358) staff       (20)    32874 2023-06-29 18:30:17.000000 skysurvey-0.7.1/skysurvey/target/core.py
--rw-r--r--   0 rigault   (2358) staff       (20)      391 2022-10-06 08:31:16.000000 skysurvey-0.7.1/skysurvey/target/environments.py
--rw-r--r--   0 rigault   (2358) staff       (20)      165 2022-09-17 13:52:22.000000 skysurvey-0.7.1/skysurvey/target/kilonova.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2341 2023-06-09 12:22:54.000000 skysurvey-0.7.1/skysurvey/target/sncc.py
--rw-r--r--   0 rigault   (2358) staff       (20)    10033 2023-06-28 13:24:24.000000 skysurvey-0.7.1/skysurvey/target/snia.py
--rw-r--r--   0 rigault   (2358) staff       (20)      681 2023-06-02 09:01:21.000000 skysurvey-0.7.1/skysurvey/target/stars.py
--rw-r--r--   0 rigault   (2358) staff       (20)     6428 2023-06-28 13:23:49.000000 skysurvey-0.7.1/skysurvey/target/timeserie.py
--rw-r--r--   0 rigault   (2358) staff       (20)    16507 2023-05-26 07:31:27.000000 skysurvey-0.7.1/skysurvey/template.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-30 09:22:08.109100 skysurvey-0.7.1/skysurvey/tools/
--rw-r--r--   0 rigault   (2358) staff       (20)       64 2023-06-29 10:12:11.000000 skysurvey-0.7.1/skysurvey/tools/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2301 2023-06-27 14:26:14.000000 skysurvey-0.7.1/skysurvey/tools/snana.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2762 2023-06-27 08:23:39.000000 skysurvey-0.7.1/skysurvey/tools/utils.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-30 09:22:08.105825 skysurvey-0.7.1/skysurvey.egg-info/
--rw-r--r--   0 rigault   (2358) staff       (20)      747 2023-06-30 09:22:08.000000 skysurvey-0.7.1/skysurvey.egg-info/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)      922 2023-06-30 09:22:08.000000 skysurvey-0.7.1/skysurvey.egg-info/SOURCES.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-06-30 09:22:08.000000 skysurvey-0.7.1/skysurvey.egg-info/dependency_links.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-06-12 09:47:03.000000 skysurvey-0.7.1/skysurvey.egg-info/not-zip-safe
--rw-r--r--   0 rigault   (2358) staff       (20)      194 2023-06-30 09:22:08.000000 skysurvey-0.7.1/skysurvey.egg-info/requires.txt
--rw-r--r--   0 rigault   (2358) staff       (20)       10 2023-06-30 09:22:08.000000 skysurvey-0.7.1/skysurvey.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-03 08:29:37.184815 skysurvey-0.7.3/
+-rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-08-10 14:40:58.000000 skysurvey-0.7.3/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      747 2023-07-03 08:29:37.184872 skysurvey-0.7.3/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)     2136 2023-06-30 08:24:06.000000 skysurvey-0.7.3/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)     1205 2023-07-03 08:29:37.185190 skysurvey-0.7.3/setup.cfg
+-rw-r--r--   0 rigault   (2358) staff       (20)       37 2023-06-12 09:49:45.000000 skysurvey-0.7.3/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-03 08:29:37.181020 skysurvey-0.7.3/skysurvey/
+-rw-r--r--   0 rigault   (2358) staff       (20)       90 2023-07-03 08:25:02.000000 skysurvey-0.7.3/skysurvey/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      524 2023-06-27 13:24:20.000000 skysurvey-0.7.3/skysurvey/config.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    27899 2023-06-29 09:38:43.000000 skysurvey-0.7.3/skysurvey/dataset.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-03 08:29:37.182258 skysurvey-0.7.3/skysurvey/examples/
+-rw-r--r--   0 rigault   (2358) staff       (20)       26 2023-06-29 14:59:14.000000 skysurvey-0.7.3/skysurvey/examples/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2233 2023-06-29 14:59:29.000000 skysurvey-0.7.3/skysurvey/examples/mocksurvey.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-03 08:29:37.183129 skysurvey-0.7.3/skysurvey/survey/
+-rw-r--r--   0 rigault   (2358) staff       (20)      125 2023-06-28 15:34:39.000000 skysurvey-0.7.3/skysurvey/survey/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     9538 2023-06-29 14:45:35.000000 skysurvey-0.7.3/skysurvey/survey/core.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2849 2023-06-29 07:52:19.000000 skysurvey-0.7.3/skysurvey/survey/des.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    15609 2023-06-29 13:44:29.000000 skysurvey-0.7.3/skysurvey/survey/healpix.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      976 2023-06-30 08:20:21.000000 skysurvey-0.7.3/skysurvey/survey/lsst.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    13238 2023-06-29 13:35:29.000000 skysurvey-0.7.3/skysurvey/survey/polygon.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     8955 2023-06-29 09:16:04.000000 skysurvey-0.7.3/skysurvey/survey/survey.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     1938 2023-06-29 13:30:27.000000 skysurvey-0.7.3/skysurvey/survey/ztf.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-03 08:29:37.184407 skysurvey-0.7.3/skysurvey/target/
+-rw-r--r--   0 rigault   (2358) staff       (20)      113 2023-05-05 08:46:40.000000 skysurvey-0.7.3/skysurvey/target/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    12064 2023-06-30 12:09:56.000000 skysurvey-0.7.3/skysurvey/target/collection.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    33561 2023-07-03 07:33:19.000000 skysurvey-0.7.3/skysurvey/target/core.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      391 2022-10-06 08:31:16.000000 skysurvey-0.7.3/skysurvey/target/environments.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      165 2022-09-17 13:52:22.000000 skysurvey-0.7.3/skysurvey/target/kilonova.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2341 2023-06-09 12:22:54.000000 skysurvey-0.7.3/skysurvey/target/sncc.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    10038 2023-07-03 07:59:46.000000 skysurvey-0.7.3/skysurvey/target/snia.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      681 2023-06-02 09:01:21.000000 skysurvey-0.7.3/skysurvey/target/stars.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     7268 2023-07-03 07:59:22.000000 skysurvey-0.7.3/skysurvey/target/timeserie.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    16507 2023-05-26 07:31:27.000000 skysurvey-0.7.3/skysurvey/template.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-03 08:29:37.184724 skysurvey-0.7.3/skysurvey/tools/
+-rw-r--r--   0 rigault   (2358) staff       (20)       64 2023-06-29 10:12:11.000000 skysurvey-0.7.3/skysurvey/tools/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2301 2023-06-27 14:26:14.000000 skysurvey-0.7.3/skysurvey/tools/snana.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2762 2023-06-27 08:23:39.000000 skysurvey-0.7.3/skysurvey/tools/utils.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-03 08:29:37.182030 skysurvey-0.7.3/skysurvey.egg-info/
+-rw-r--r--   0 rigault   (2358) staff       (20)      747 2023-07-03 08:29:37.000000 skysurvey-0.7.3/skysurvey.egg-info/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)      922 2023-07-03 08:29:37.000000 skysurvey-0.7.3/skysurvey.egg-info/SOURCES.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-07-03 08:29:37.000000 skysurvey-0.7.3/skysurvey.egg-info/dependency_links.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-06-12 09:47:03.000000 skysurvey-0.7.3/skysurvey.egg-info/not-zip-safe
+-rw-r--r--   0 rigault   (2358) staff       (20)      194 2023-07-03 08:29:37.000000 skysurvey-0.7.3/skysurvey.egg-info/requires.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)       10 2023-07-03 08:29:37.000000 skysurvey-0.7.3/skysurvey.egg-info/top_level.txt
```

### Comparing `skysurvey-0.7.1/LICENSE` & `skysurvey-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.1/PKG-INFO` & `skysurvey-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skysurvey
-Version: 0.7.1
+Version: 0.7.3
 Summary: Simulating Transient in the sky and how to observe them
 Home-page: https://github.com/MickaelRigault/skysurvey
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: Apache Software License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `skysurvey-0.7.1/README.md` & `skysurvey-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.1/setup.cfg` & `skysurvey-0.7.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.1/skysurvey/config.py` & `skysurvey-0.7.3/skysurvey/config.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.1/skysurvey/dataset.py` & `skysurvey-0.7.3/skysurvey/dataset.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.1/skysurvey/examples/mocksurvey.py` & `skysurvey-0.7.3/skysurvey/examples/mocksurvey.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.1/skysurvey/survey/core.py` & `skysurvey-0.7.3/skysurvey/survey/core.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.1/skysurvey/survey/des.py` & `skysurvey-0.7.3/skysurvey/survey/des.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.1/skysurvey/survey/healpix.py` & `skysurvey-0.7.3/skysurvey/survey/healpix.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.1/skysurvey/survey/lsst.py` & `skysurvey-0.7.3/skysurvey/survey/lsst.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.1/skysurvey/survey/polygon.py` & `skysurvey-0.7.3/skysurvey/survey/polygon.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.1/skysurvey/survey/survey.py` & `skysurvey-0.7.3/skysurvey/survey/survey.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.1/skysurvey/survey/ztf.py` & `skysurvey-0.7.3/skysurvey/survey/ztf.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.1/skysurvey/target/collection.py` & `skysurvey-0.7.3/skysurvey/target/collection.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,14 +163,27 @@
 
     
 class TransientCollection( TargetCollection ):
     _COLLECTION_OF = Transient    
     # ============= #
     #  Methods      #
     # ============= #
+    def set_rate(self, float_or_func):
+        """ set the transient rate
+
+        Parameters
+        ----------
+        float_or_func: float, func
+            
+        """
+        if callable(float_or_func):
+            self._rate = float_or_func
+        else:
+            self._rate = float(float_or_func)
+    
     def get_rates(self, z, relative=False, **kwargs):
         """ """
         rates = self.call_down("get_rate", margs=z, **kwargs)
         if relative:
             rates /= np.nansum(rates)
         return rates
     
@@ -302,19 +315,17 @@
         if not hasattr(self,"_magabs") or self._magabs is None:
             self._magabs = self._MAGABS
             
         return self._magabs
         
     @property
     def rate(self):
-        """ rate.
-        (If float, assumed to be volumetric rate in Gpc-3 / yr-1.)
-        """
+        """ rate. (If float, assumed to be volumetric rate in Gpc-3 / yr.) """
         if not hasattr(self,"_rate"):
-            self._rate = self._RATE # default
+            self.set_rate( self._RATE) # default
             
         return self._rate
     
     
 class TSTransientCollection( TransientCollection ):
     _COLLECTION_OF = TSTransient
```

### Comparing `skysurvey-0.7.1/skysurvey/target/core.py` & `skysurvey-0.7.3/skysurvey/target/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     def __init__(self):
         """ 
         See also
         --------
         from_setting: loads an instance given model parameters (dict)
         """
-        
+        pass
         
     def __repr__(self):
         """ """
         
         return self.__str__()
     
     def __str__(self):
@@ -712,14 +712,26 @@
 
         Returns
         -------
         DataFrame
             the simulated dataframe.
 
         """
+        # => tstart, tstop format
+        if type(tstart) is str:
+            tstart = time.Time(tstart).mjd
+        elif type(tstart) is time.Time:
+            tstart = tstart.mjd
+
+        if type(tstop) is str:
+            tstop = time.Time(tstop).mjd
+        elif type(tstop) is time.Time:
+            tstop = tstop.mjd
+        
+        # => nyears and times    
         if nyears is None and (tstart is not None and tstop is not None):
             nyears = (tstop-tstart)/365.25
                 
         if nyears is not None and (tstart is not None and tstop is None):
             tstop = tstart + nyears*365.25
 
         if nyears is not None and (tstart is  None and tstop is not None):
@@ -860,14 +872,27 @@
 class Transient( Target ):
     # - Transient
     _RATE = None    
     
     # ============== #
     #  Methods       #
     # ============== #
+    def set_rate(self, float_or_func):
+        """ set the transient rate
+
+        Parameters
+        ----------
+        float_or_func: float, func
+            
+        """
+        if callable(float_or_func):
+            self._rate = float_or_func
+        else:
+            self._rate = float(float_or_func)
+    
     # Rates
     def getpdf_redshift(self, z, **kwargs):
         """ 
 
         Parameters
         ----------
         z: 1d-array
@@ -1035,10 +1060,10 @@
     # Rate
     @property
     def rate(self):
         """ rate.
         (If float, assumed to be volumetric rate in Gpc-3 / yr-1.)
         """
         if not hasattr(self,"_rate"):
-            self._rate = self._RATE # default
+            self.set_rate( self._RATE ) # default
             
         return self._rate
```

### Comparing `skysurvey-0.7.1/skysurvey/target/sncc.py` & `skysurvey-0.7.3/skysurvey/target/sncc.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.1/skysurvey/target/snia.py` & `skysurvey-0.7.3/skysurvey/target/snia.py`

 * *Files 3% similar despite different names*

```diff
@@ -251,15 +251,15 @@
     _MODEL = dict( redshift = {"kwargs": {"zmax":0.2}, "as":"z"},
                               
                    x1 = {"func": SNeIaStretch.nicolas2021}, 
                    
                    c = {"func": SNeIaColor.intrinsic_and_dust},
 
                    t0 = {"func": np.random.uniform, 
-                         "kwargs": {"low":56000, "high":57000} },
+                         "kwargs": {"low":56_000, "high":56_200} },
                        
                    magabs = {"func": SNeIaMagnitude.tripp1998,
                              "kwargs": {"x1": "@x1", "c": "@c",
                                         "mabs":-19.3, "sigmaint":0.10}
                             },
                            
                    magobs = {"func": "magabs_to_magobs", # defined in Target (mother of Transients)
@@ -280,25 +280,25 @@
 class SNeIaHostMass( Transient ):
     
     _KIND = "SNIa"
     _TEMPLATE = "salt2"
     _RATE = 2.35 * 10**4 # Perley 2020
 
     # {'func': func, 'prop': dict, 'input':, 'as':}
-    _MODEL = dict( redshift = {"param":{"zmax":0.2},
+    _MODEL = dict( redshift = {"kwargs":{"zmax":0.2},
                                   "as":"z"},
                               
                    x1 = {"func": SNeIaStretch.nicolas2021}, 
                    
                    c = {"func": SNeIaColor.intrinsic_and_dust},
 
                    hostmass = {"func": getpdf_asymetric_gaussian},
 
                    t0 = {"func": np.random.uniform, 
-                         "kwargs": {"low":56000, "high":57000} },
+                         "kwargs": {"low":56_000, "high":56_200} },
                        
                    magabs = {"func": SNeIaMagnitude.tripp_and_massstep,
                              "kwargs": { "x1": "@x1", "c": "@c", "hostmass": "@hostmass",
                                         "mabs":-19.3, "sigmaint":0.10, "split":10}
                             },
                            
                    magobs = {"func": "magabs_to_magobs", # defined in Target (mother of Transients)
```

### Comparing `skysurvey-0.7.1/skysurvey/target/stars.py` & `skysurvey-0.7.3/skysurvey/target/stars.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.1/skysurvey/target/timeserie.py` & `skysurvey-0.7.3/skysurvey/target/timeserie.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,19 +11,19 @@
     [see list](https://sncosmo.readthedocs.io/en/stable/source-list.html)
 
     Example
     -------
     >>> snii = TSTransient.from_draw("snana-2004fe", 4000)
     >>> _ = snii.show_lightcurve(["ztfg","ztfr"], index=10, in_mag=True)
     """
-    
+    _RATE = 0.001
     _MODEL = dict( redshift = {"kwargs": {"zmax": 0.05}, 
                                "as": "z"},
                    t0 = {"func": np.random.uniform,
-                         "kwargs": {"low": 56000, "high": 56000+4*365}
+                         "kwargs": {"low": 56_000, "high": 56_200}
                         },
                          
                    magabs = {"func": np.random.normal,
                              "kwargs": {"loc": -18, "scale": 1}
                             },
                              
                    magobs = {"func": "magabs_to_magobs",
@@ -34,18 +34,39 @@
                                 "kwargs": {"magobs": "@magobs"}
                             },
                    # This you need to match with the survey
                    radec = {"func": random_radec,
                             "as": ["ra","dec"]
                             }
                  )
+
+
+    def __init__(self, source_or_template=None, *args, **kwargs):
+        """ loads a TimeSerie Transient 
+
+        Parameters
+        ----------
+        source_or_template: str, `sncosmo.Source`, `sncosmo.Model`, skysurvey.Template
+            the sncosmo TimeSeriesSource, you can provide:
+            - str: the name, e.g. "v19-2013ge-corr"
+            - sncosmo.Source: a loaded sncosmo.Source
+            - sncosmo.Model: a  loaded sncosmo.Model
+            this is eventually converted into a generic skysurvey.Template.
+
+        """
+        if source_or_template is not None:
+            self.set_template(source_or_template)
+
+        super().__init__(*args, **kwargs)
     
     @classmethod
-    def from_sncosmo(cls, source, rate=1e3, model=None,
-                                magabs=None, magscatter=None):
+    def from_sncosmo(cls, source,
+                         rate=None,
+                         model=None,
+                         magabs=None, magscatter=None):
         """ loads an instance from a sncosmo TimeSeriesSource source
         (see https://sncosmo.readthedocs.io/en/stable/source-list.html#list-of-built-in-sources) 
 
         Parameters
         ----------
         source: str, `sncosmo.Source`, `sncosmo.Model`, skysurvey.Template
             the sncosmo TimeSeriesSource, you can provide:
@@ -79,31 +100,34 @@
         instance
             loaded instance. 
 
         See also
         --------
         from_draw: load an instance and draw the transient parameters
         """
-        this = cls()
-        this.set_template(source)
-        this._rate = rate
+        this = cls(source_or_template=source)            
+        if rate is not None:
+            this.set_rate(rate)
         
         if model is not None:
             self._model = model
 
         if magabs is not None:
             this.change_model_parameter(magabs={"loc":magabs})
             
         if magscatter is not None:
             this.change_model_parameter(magabs={"scale":magscatter})
             
         return this
     
     @classmethod
-    def from_draw(cls, source, size, rate=1e-3, model=None, 
+    def from_draw(cls, size,
+                      rate=None,
+                      source=None,
+                      model=None, 
                       magabs=None, magscatter=None,
                       zmin=0, zmax=None,
                       tstart=None, tstop=None,
                       **kwargs):
         """ loads an instance from a sncosmo TimeSeriesSource source and draws trasient parameters
         (see https://sncosmo.readthedocs.io/en/stable/source-list.html#list-of-built-in-sources)
```

### Comparing `skysurvey-0.7.1/skysurvey/template.py` & `skysurvey-0.7.3/skysurvey/template.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.1/skysurvey/tools/snana.py` & `skysurvey-0.7.3/skysurvey/tools/snana.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.1/skysurvey/tools/utils.py` & `skysurvey-0.7.3/skysurvey/tools/utils.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.1/skysurvey.egg-info/PKG-INFO` & `skysurvey-0.7.3/skysurvey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skysurvey
-Version: 0.7.1
+Version: 0.7.3
 Summary: Simulating Transient in the sky and how to observe them
 Home-page: https://github.com/MickaelRigault/skysurvey
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: Apache Software License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `skysurvey-0.7.1/skysurvey.egg-info/SOURCES.txt` & `skysurvey-0.7.3/skysurvey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

