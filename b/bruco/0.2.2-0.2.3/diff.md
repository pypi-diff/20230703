# Comparing `tmp/bruco-0.2.2.tar.gz` & `tmp/bruco-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bruco-0.2.2.tar", last modified: Mon Jan 30 13:22:01 2023, max compression
+gzip compressed data, was "bruco-0.2.3.tar", last modified: Mon Jul  3 08:51:07 2023, max compression
```

## Comparing `bruco-0.2.2.tar` & `bruco-0.2.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-01-30 13:22:01.391423 bruco-0.2.2/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    35147 2020-12-11 06:07:29.000000 bruco-0.2.2/LICENSE
--rw-r--r--   0 duncan    (1000) duncan    (1000)      120 2020-12-11 06:07:29.000000 bruco-0.2.2/MANIFEST.in
--rw-r--r--   0 duncan    (1000) duncan    (1000)      815 2023-01-30 13:22:01.391423 bruco-0.2.2/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6668 2022-06-23 12:47:33.000000 bruco-0.2.2/README.md
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-01-30 13:22:01.381423 bruco-0.2.2/bin/
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)       36 2020-12-11 06:07:29.000000 bruco-0.2.2/bin/bruco
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-01-30 13:22:01.381423 bruco-0.2.2/bruco/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      188 2023-01-30 13:21:49.000000 bruco-0.2.2/bruco/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8398 2022-06-23 12:47:33.000000 bruco-0.2.2/bruco/__main__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    17805 2023-01-30 13:21:49.000000 bruco-0.2.2/bruco/coherence.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8737 2022-06-23 12:47:33.000000 bruco-0.2.2/bruco/functions.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-01-30 13:22:01.381423 bruco-0.2.2/bruco/html/
--rw-r--r--   0 duncan    (1000) duncan    (1000)       88 2020-12-11 06:07:29.000000 bruco-0.2.2/bruco/html/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    20950 2020-12-11 06:07:29.000000 bruco-0.2.2/bruco/html/markup.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3390 2022-06-23 12:47:33.000000 bruco-0.2.2/bruco/ligodata.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6728 2022-06-23 12:47:33.000000 bruco-0.2.2/bruco/parameters.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7041 2022-06-23 12:47:33.000000 bruco-0.2.2/bruco/report.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-01-30 13:22:01.381423 bruco-0.2.2/bruco.egg-info/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      815 2023-01-30 13:22:01.000000 bruco-0.2.2/bruco.egg-info/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)      664 2023-01-30 13:22:01.000000 bruco-0.2.2/bruco.egg-info/SOURCES.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2023-01-30 13:22:01.000000 bruco-0.2.2/bruco.egg-info/dependency_links.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)       54 2023-01-30 13:22:01.000000 bruco-0.2.2/bruco.egg-info/requires.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)        6 2023-01-30 13:22:01.000000 bruco-0.2.2/bruco.egg-info/top_level.txt
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-01-30 13:22:01.381423 bruco-0.2.2/debian/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1224 2022-06-23 12:47:33.000000 bruco-0.2.2/debian/changelog
--rw-r--r--   0 duncan    (1000) duncan    (1000)        2 2020-12-11 06:07:29.000000 bruco-0.2.2/debian/compat
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1196 2022-06-23 12:47:33.000000 bruco-0.2.2/debian/control
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1143 2020-12-11 06:07:29.000000 bruco-0.2.2/debian/copyright
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)      306 2022-06-23 12:47:33.000000 bruco-0.2.2/debian/rules
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-01-30 13:22:01.381423 bruco-0.2.2/debian/source/
--rw-r--r--   0 duncan    (1000) duncan    (1000)       12 2020-12-11 06:07:29.000000 bruco-0.2.2/debian/source/format
--rw-r--r--   0 duncan    (1000) duncan    (1000)       73 2023-01-30 13:22:01.391423 bruco-0.2.2/setup.cfg
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1970 2023-01-30 13:21:49.000000 bruco-0.2.2/setup.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-01-30 13:22:01.381423 bruco-0.2.2/share/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      448 2023-01-30 13:21:49.000000 bruco-0.2.2/share/asc_modulations.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1292 2022-06-23 12:47:33.000000 bruco-0.2.2/share/excluded_channels.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)   538850 2020-12-11 06:07:29.000000 bruco-0.2.2/share/lho_cal_deltal_calibration.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)      697 2021-10-19 12:42:06.000000 bruco-0.2.2/share/lho_excluded_channels_O3.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)      809 2023-01-30 13:21:49.000000 bruco-0.2.2/share/lho_excluded_channels_O4.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)      595 2021-10-05 07:22:59.000000 bruco-0.2.2/share/llo_excluded_channels.txt
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-07-03 08:51:07.630846 bruco-0.2.3/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    35147 2020-12-11 06:07:29.000000 bruco-0.2.3/LICENSE
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      120 2020-12-11 06:07:29.000000 bruco-0.2.3/MANIFEST.in
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      815 2023-07-03 08:51:07.630846 bruco-0.2.3/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6668 2022-06-23 12:47:33.000000 bruco-0.2.3/README.md
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-07-03 08:51:07.620846 bruco-0.2.3/bin/
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)       36 2020-12-11 06:07:29.000000 bruco-0.2.3/bin/bruco
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-07-03 08:51:07.620846 bruco-0.2.3/bruco/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      188 2023-07-03 08:50:52.000000 bruco-0.2.3/bruco/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8404 2023-07-03 08:50:52.000000 bruco-0.2.3/bruco/__main__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    17805 2023-01-30 13:21:49.000000 bruco-0.2.3/bruco/coherence.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8737 2022-06-23 12:47:33.000000 bruco-0.2.3/bruco/functions.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-07-03 08:51:07.620846 bruco-0.2.3/bruco/html/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       88 2020-12-11 06:07:29.000000 bruco-0.2.3/bruco/html/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    20950 2020-12-11 06:07:29.000000 bruco-0.2.3/bruco/html/markup.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3390 2022-06-23 12:47:33.000000 bruco-0.2.3/bruco/ligodata.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6728 2022-06-23 12:47:33.000000 bruco-0.2.3/bruco/parameters.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6845 2023-07-03 08:50:52.000000 bruco-0.2.3/bruco/report.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-07-03 08:51:07.620846 bruco-0.2.3/bruco.egg-info/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      815 2023-07-03 08:51:07.000000 bruco-0.2.3/bruco.egg-info/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      664 2023-07-03 08:51:07.000000 bruco-0.2.3/bruco.egg-info/SOURCES.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2023-07-03 08:51:07.000000 bruco-0.2.3/bruco.egg-info/dependency_links.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       47 2023-07-03 08:51:07.000000 bruco-0.2.3/bruco.egg-info/requires.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        6 2023-07-03 08:51:07.000000 bruco-0.2.3/bruco.egg-info/top_level.txt
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-07-03 08:51:07.620846 bruco-0.2.3/debian/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1396 2023-07-03 08:50:52.000000 bruco-0.2.3/debian/changelog
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        2 2020-12-11 06:07:29.000000 bruco-0.2.3/debian/compat
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1196 2022-06-23 12:47:33.000000 bruco-0.2.3/debian/control
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1143 2020-12-11 06:07:29.000000 bruco-0.2.3/debian/copyright
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)      306 2022-06-23 12:47:33.000000 bruco-0.2.3/debian/rules
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-07-03 08:51:07.620846 bruco-0.2.3/debian/source/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       12 2020-12-11 06:07:29.000000 bruco-0.2.3/debian/source/format
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       73 2023-07-03 08:51:07.630846 bruco-0.2.3/setup.cfg
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1953 2023-07-03 08:50:52.000000 bruco-0.2.3/setup.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-07-03 08:51:07.630846 bruco-0.2.3/share/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      448 2023-01-30 13:21:49.000000 bruco-0.2.3/share/asc_modulations.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1292 2022-06-23 12:47:33.000000 bruco-0.2.3/share/excluded_channels.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)   538850 2020-12-11 06:07:29.000000 bruco-0.2.3/share/lho_cal_deltal_calibration.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      697 2021-10-19 12:42:06.000000 bruco-0.2.3/share/lho_excluded_channels_O3.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      827 2023-07-03 08:50:52.000000 bruco-0.2.3/share/lho_excluded_channels_O4.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      595 2021-10-05 07:22:59.000000 bruco-0.2.3/share/llo_excluded_channels.txt
```

### Comparing `bruco-0.2.2/LICENSE` & `bruco-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bruco-0.2.2/PKG-INFO` & `bruco-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bruco
-Version: 0.2.2
+Version: 0.2.3
 Summary: Brute force coherence
 Home-page: https://git.ligo.org/gabriele-vajente/bruco
 Author: Gabriele Vajente
 License: GPLv3+
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `bruco-0.2.2/README.md` & `bruco-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `bruco-0.2.2/bruco/__main__.py` & `bruco-0.2.3/bruco/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Brute force coherence (Gabriele Vajente, 2022-02-08)
 
 import numpy
 import os
 import multiprocessing
-import pickle
 
 from scipy.signal import resample_poly, resample, detrend
 import scipy.stats
 
 from . import __version__, __date__
 from .functions import *
 from .html import markup
@@ -129,15 +128,15 @@
         mod_data, mod_fs = getRawData(modulations, opt['gpsb'], opt['gpse'], opt['aux_source'])
         # create array of resampled data
         mod_channels = numpy.zeros((len(modulations)+1, (opt['gpse']-opt['gpsb'])*opt['outfs']))
         mod_channels[0,:] = 1   # including constant
         for i,m in enumerate(modulations):
             if mod_fs[m] < opt['outfs']:
                 mod_channels[i+1,:] = resample_poly(mod_data[m], up=opt['outfs']//mod_fs[m], down=1)
-            elif fs[m] > opt['outfs']:
+            elif mod_fs[m] > opt['outfs']:
                 mod_channels[i+1,:] = resample_poly(mod_data[m], up=1, down=mod_fs[m]//opt['outfs'])
             else:
                 mod_channels[i+1,:] = mod_data[m]
         mod_channels[i,:] = detrend(mod_channels[i,:])
         # add empty string to list of modulation channels, to represent unmodulated channel
         modulations = ['No modulation'] + modulations
     else:
@@ -182,17 +181,17 @@
         results = [parallelized_coherence(args[0])]
 
     # when we get here, all the computations are concluded
     print(">>>>> Parallel processes finished...")
 
     ## Put all the results together ###############################################################
 
-    cohtab, idxtab, modtab = collect_results(results, opt)
+    cohtab, idxtab, modtab, timing = collect_results(results, opt)
 
     ## Write the HTML report ######################################################################
 
-    generate_report(opt, cohtab, idxtab, modtab, channels, modulations)
+    generate_report(opt, cohtab, idxtab, modtab, channels, modulations, timing)
 
 
 if __name__ == '__main__':
     # execute the main function when called from command line
     bruco()
```

### Comparing `bruco-0.2.2/bruco/coherence.py` & `bruco-0.2.3/bruco/coherence.py`

 * *Files identical despite different names*

### Comparing `bruco-0.2.2/bruco/functions.py` & `bruco-0.2.3/bruco/functions.py`

 * *Files identical despite different names*

### Comparing `bruco-0.2.2/bruco/html/markup.py` & `bruco-0.2.3/bruco/html/markup.py`

 * *Files identical despite different names*

### Comparing `bruco-0.2.2/bruco/ligodata.py` & `bruco-0.2.3/bruco/ligodata.py`

 * *Files identical despite different names*

### Comparing `bruco-0.2.2/bruco/parameters.py` & `bruco-0.2.3/bruco/parameters.py`

 * *Files identical despite different names*

### Comparing `bruco-0.2.2/bruco/report.py` & `bruco-0.2.3/bruco/report.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Brute force coherence (Gabriele Vajente, 2022-02-08)
 
 import numpy
 import os
-import pickle
 import gpstime
 import sys
 import time
 
 from . import __version__, __date__
 from .functions import *
 from .html import markup
@@ -33,19 +32,15 @@
     """
 
     # first step, concatenate the tables
     x = list(zip(*results))
     cohtab = numpy.concatenate(x[0], axis=1)
     idxtab = numpy.concatenate(x[1], axis=1)
     modtab = numpy.concatenate(x[2], axis=1)
-
-    # save timing info
     timing = x[4]
-    with open(opt['dir'] + '/timing.pickle', 'wb') as timingfile:
-        pickle.dump(timing, timingfile)
 
     # list of channels with errors
     errchannellist = numpy.concatenate(x[5],axis=0)
     numpy.savetxt(opt['dir']+'/channels_error.txt', errchannellist, fmt='%s')
 
     # then sort in order of descending coherence for each bin
     for j in numpy.arange(cohtab.shape[0]):
@@ -61,17 +56,17 @@
     idxtab = idxtab[:,-opt['ntop']:]
     modtab = modtab[:,-opt['ntop']:]
     # save the coherence tables to files
     numpy.savetxt(opt['dir'] + '/cohtab.txt', cohtab)
     numpy.savetxt(opt['dir'] + '/idxtab.txt', idxtab)
     numpy.savetxt(opt['dir'] + '/modtab.txt', modtab)
 
-    return cohtab, idxtab, modtab
+    return cohtab, idxtab, modtab, timing
 
-def generate_report(opt, cohtab, idxtab, modtab, channels, modulations):
+def generate_report(opt, cohtab, idxtab, modtab, channels, modulations, timing):
     """
     Generate the HTML report page.
 
     Parameters
     ----------
     opt: dict
         parsed command line arguments
@@ -182,15 +177,14 @@
 
     # That's the end, save the HTML page
     with open(opt['dir']  + '/index.html', 'w') as fileid:
         print(page, file=fileid)
 
     # timing info
     dt['report'] = dt['report'] + time.time()
-    timing = pickle.load(open(opt['dir'] + '/timing.pickle', 'rb'))
     for t in timing:
         for k in t.keys():
             dt[k] += t[k]
     label = {'data':'Read data','decim':'Resampling','fft':'FFT','plot':'Plotting','tot':'Total', 'report':'Write report'}
     print()
     print('Task           Time  Time/nproc  Percent')
     print('----------------------------------------')
```

### Comparing `bruco-0.2.2/bruco.egg-info/PKG-INFO` & `bruco-0.2.3/bruco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bruco
-Version: 0.2.2
+Version: 0.2.3
 Summary: Brute force coherence
 Home-page: https://git.ligo.org/gabriele-vajente/bruco
 Author: Gabriele Vajente
 License: GPLv3+
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `bruco-0.2.2/bruco.egg-info/SOURCES.txt` & `bruco-0.2.3/bruco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bruco-0.2.2/debian/changelog` & `bruco-0.2.3/debian/changelog`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-bruco (0.2.1-1) unstable; urgency=low
+bruco (0.2.3-1) unstable; urgency=low
+
+  * minor bug fixes, removed pickle requirement
+
+ -- Gabriele Vajente <gabriele.vajente@ligo.org>  Mon, 1 May 2023 00:00:00 +0000
+ 
+ bruco (0.2.1-1) unstable; urgency=low
 
   * minor bug fixes
 
  -- Gabriele Vajente <gabriele.vajente@ligo.org>  Tue, 16 Jun 2022 00:00:00 +0000
 
 bruco (0.2.0-1) unstable; urgency=low
```

### Comparing `bruco-0.2.2/debian/control` & `bruco-0.2.3/debian/control`

 * *Files identical despite different names*

### Comparing `bruco-0.2.2/debian/copyright` & `bruco-0.2.3/debian/copyright`

 * *Files identical despite different names*

### Comparing `bruco-0.2.2/setup.py` & `bruco-0.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     install_requires=[
         'numpy',
         'scipy',
         'matplotlib',
         'gwdatafind',
         'gwpy',
         'gpstime',
-        'pickle'
     ],
     # content
     packages=find_packages(),
     scripts=[os.path.join('bin', 'bruco')],
     data_files=[
         (os.path.join('share', 'bruco'),
          list(glob.glob(os.path.join('share', '*.txt'))),
```

### Comparing `bruco-0.2.2/share/excluded_channels.txt` & `bruco-0.2.3/share/excluded_channels.txt`

 * *Files identical despite different names*

### Comparing `bruco-0.2.2/share/lho_cal_deltal_calibration.txt` & `bruco-0.2.3/share/lho_cal_deltal_calibration.txt`

 * *Files identical despite different names*

### Comparing `bruco-0.2.2/share/lho_excluded_channels_O3.txt` & `bruco-0.2.3/share/lho_excluded_channels_O3.txt`

 * *Files identical despite different names*

### Comparing `bruco-0.2.2/share/lho_excluded_channels_O4.txt` & `bruco-0.2.3/share/lho_excluded_channels_O4.txt`

 * *Files 8% similar despite different names*

```diff
@@ -53,7 +53,9 @@
 ASC-AS_A_RF45_Q_SUM_OUT_DQ
 *TIDAL*
 *GPS*
 OAF-CLEAN*
 OAF-CAL_DELTAL*
 OMZ*
 BOS*
+OAF*
+SUS-PI_PROC*
```

### Comparing `bruco-0.2.2/share/llo_excluded_channels.txt` & `bruco-0.2.3/share/llo_excluded_channels.txt`

 * *Files identical despite different names*

