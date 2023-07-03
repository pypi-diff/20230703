# Comparing `tmp/scoobi-0.0.1.6.tar.gz` & `tmp/scoobi-0.0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoobi-0.0.1.6.tar", last modified: Sun Jul  2 22:06:26 2023, max compression
+gzip compressed data, was "scoobi-0.0.1.7.tar", last modified: Mon Jul  3 09:45:16 2023, max compression
```

## Comparing `scoobi-0.0.1.6.tar` & `scoobi-0.0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:26.888028 scoobi-0.0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-02 22:06:11.000000 scoobi-0.0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-02 22:06:26.888028 scoobi-0.0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-02 22:06:11.000000 scoobi-0.0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-02 22:06:26.888028 scoobi-0.0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-02 22:06:11.000000 scoobi-0.0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:26.880028 scoobi-0.0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:26.884028 scoobi-0.0.1.6/src/scoobi/
--rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-07-02 22:06:11.000000 scoobi-0.0.1.6/src/scoobi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-07-02 22:06:11.000000 scoobi-0.0.1.6/src/scoobi/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-02 22:06:11.000000 scoobi-0.0.1.6/src/scoobi/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-07-02 22:06:11.000000 scoobi-0.0.1.6/src/scoobi/fitscubetofits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:26.888028 scoobi-0.0.1.6/src/scoobi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-02 22:06:26.000000 scoobi-0.0.1.6/src/scoobi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-02 22:06:26.000000 scoobi-0.0.1.6/src/scoobi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 22:06:26.000000 scoobi-0.0.1.6/src/scoobi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-02 22:06:26.000000 scoobi-0.0.1.6/src/scoobi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-02 22:06:26.000000 scoobi-0.0.1.6/src/scoobi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 22:06:26.000000 scoobi-0.0.1.6/src/scoobi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:45:16.822983 scoobi-0.0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-03 09:45:06.000000 scoobi-0.0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-03 09:45:16.822983 scoobi-0.0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-03 09:45:06.000000 scoobi-0.0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-03 09:45:16.822983 scoobi-0.0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-03 09:45:06.000000 scoobi-0.0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:45:16.822983 scoobi-0.0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:45:16.822983 scoobi-0.0.1.7/src/scoobi/
+-rw-r--r--   0 runner    (1001) docker     (123)    17897 2023-07-03 09:45:06.000000 scoobi-0.0.1.7/src/scoobi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-07-03 09:45:06.000000 scoobi-0.0.1.7/src/scoobi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-03 09:45:06.000000 scoobi-0.0.1.7/src/scoobi/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-07-03 09:45:06.000000 scoobi-0.0.1.7/src/scoobi/fitscubetofits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:45:16.822983 scoobi-0.0.1.7/src/scoobi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-03 09:45:16.000000 scoobi-0.0.1.7/src/scoobi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-03 09:45:16.000000 scoobi-0.0.1.7/src/scoobi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 09:45:16.000000 scoobi-0.0.1.7/src/scoobi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-03 09:45:16.000000 scoobi-0.0.1.7/src/scoobi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-03 09:45:16.000000 scoobi-0.0.1.7/src/scoobi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 09:45:16.000000 scoobi-0.0.1.7/src/scoobi.egg-info/top_level.txt
```

### Comparing `scoobi-0.0.1.6/LICENSE` & `scoobi-0.0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scoobi-0.0.1.6/PKG-INFO` & `scoobi-0.0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoobi
-Version: 0.0.1.6
+Version: 0.0.1.7
 Summary: Solar Conventionality-based Organizing Observation data ( SCOOBI )
 Home-page: https://github.com/avialxee/scoobi
 Author: Avinash Kumar
 Author-email: avialxee@gmail.com
 Project-URL: Bug Tracker, https://github.com/avialxee/scoobi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `scoobi-0.0.1.6/README.md` & `scoobi-0.0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `scoobi-0.0.1.6/setup.py` & `scoobi-0.0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as rdme:
     desc = rdme.read()
 
 setup(
     name = 'scoobi',
-    version = '0.0.1.6',
+    version = '0.0.1.7',
     url='https://github.com/avialxee/scoobi',
     author='Avinash Kumar',
     author_email='avialxee@gmail.com',
     description='Solar Conventionality-based Organizing Observation data ( SCOOBI )',
     py_modules = ["scoobi"],
     package_dir={'':'src'},
     classifiers=["Programming Language :: Python :: 3",
```

### Comparing `scoobi-0.0.1.6/src/scoobi/__init__.py` & `scoobi-0.0.1.7/src/scoobi/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from astropy.time import Time
 import astropy.units as u
 from collections import defaultdict
 import csv
 import datetime
 import shutil
 from scoobi.config import usemagick, thumbnails, thumbnails_root, rootfolder
+from scoobi.config import  dark,dark_cadence,dark_initial,flat,flat_cadence,flat_initial,hc,hc_cadence,hc_initial,lc,lc_cadence,lc_initial
 
 
 class SCOOBI():
     def __init__():
         pass
 
 # Helper
@@ -145,44 +146,66 @@
 
         The destination folder name where all the files will get saved.
 
     :telescope:
         (str) (Optional) (Default:HA)
         The Telescope name is used to create the header info and filename
     """
+    if header:
+        pass
     params={'fitsname':None, 'telescope':'HA', 'initial':'S'}
     params.update(kwargs)
     fitsfile_o=None
-    
-    if header:
-        pass
-    with fits.open(fitsfile_i, 'readonly',) as hdul:
-        print('fits opned')
-        if len(hdul[0].data.shape)==3:hdul[0].data=hdul[0].data[0]
-        date=hdul[0].header['DATE-OBS']
-        print(f'read date:{date}')
+    def __writefilefromhdul(hdul,date):
+        """
+        internal function to read hdul and date to fill headers and generate fitsfile name creating directory where necessary.
+        """
+        date=date.strftime('%Y-%m-%dT%H:%M:%S.%f')
         for hdu in hdul:
             hdu.header.update(header)
             hdu.header['TELESCOP']=params['telescope']
             hdu.header['FILENAME']=Path(fitsfile_i).name
             
         if params['fitsname'] is None:
             # name convention : *S + DATETIME + TELESCOPE*
             print('building foldername:')
 
             fitsfile_o=f"{params['initial']}-{date}-{params['telescope']}.fits"
             fitsfile_o=build_foldername(fitsfile_o, **kwargs)
-            print(fitsfile_o)
         else:
-            
             fitsfile_o=build_foldername(params['fitsname'])
-            
         hdul.writeto(fitsfile_o, overwrite=True)
+        return fitsfile_o
+    
+    with fits.open(fitsfile_i, 'readonly',) as hdul:
+        date=hdul[0].header['DATE-OBS']
+        date=datetime.datetime.strptime(date,'%Y-%m-%dT%H:%M:%S.%f')
+        cadence=0
+        if dark in fitsfile_i:
+            params['initial']=dark_initial
+            cadence=dark_cadence
+        elif flat in fitsfile_i:
+            params['initial']=flat_initial
+            cadence=flat_cadence
+        elif hc in fitsfile_i:
+            params['initial']=hc_initial
+            cadence=hc_cadence
+        elif lc in fitsfile_i:
+            params['initial']=lc_initial
+            cadence=lc_cadence
+            
+
+        if len(hdul[0].data.shape)==3:                                  # checks if data is cube
+            for i, hdul_slice in enumerate(hdul[0].data):
+                td=datetime.timedelta(seconds=cadence*i)
+                date=date+td
+                fitsfile_o=__writefilefromhdul(hdul_slice,date)
+        else:
+            fitsfile_o=__writefilefromhdul(hdul,date)
     return fitsfile_o
-    # data,hdrdata=scidata[0][0], scidata[1] # taking data[0] as data is 3D
     
 def tif_to_fits(tiffile, magick=usemagick, header=None, **kwargs):
     """
     *Parameters*
     
     :tiffile:
         (str) (Required)
```

### Comparing `scoobi-0.0.1.6/src/scoobi/cli.py` & `scoobi-0.0.1.7/src/scoobi/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 from scoobi import compare_datetime, read_tif, Time, tif2fits_bulk, tif_to_fits, compare_datetime_nofolder, thumbgen_bulk,fits2fits_bulk,fits_to_fits
 from collections import defaultdict
 from pathlib import Path
-from scoobi.config import rootfolder,processedfolder,processed,thumbnails_root,rawfolder,hc,lc,darks,flat,corrupted_folder
+from scoobi.config import rootfolder,processedfolder,rawfolder,config
 
 def read_configfile(filepath):
     with open(filepath,'r') as f:
         params = defaultdict(list)
         pr=f.read().splitlines()
         for i in range(len(pr)):
             if '#' in pr[i]:
@@ -15,36 +15,48 @@
                 k,v=pr[i].split('=')
                 if 'month' in k:
                     params[k]=v.split(',')
                 elif 'days' in k:
                     dd=v.split(',')
                     params[k]=range(int(dd[0]),int(dd[1])) 
                 else:
+                    try:
+                        v=int(v)
+                    except:
+                        v=str(v)
+                        if 'True' in v: v=v.lower()=='true'
+                        elif 'False' in v:v=v.lower()=='true'
+                    
                     params[k]=v
     return params
 
 def default_params():
-    return {'fits_folder':processedfolder,
+    params= {'fits_folder':processedfolder,
         'csv_file':f'{rootfolder}log.csv',
         'tiff_folder':rawfolder,
         'raw_folder':rawfolder, 
         'rootfolder':rootfolder,
         'month':'Jan,Feb,Mar,Apr,May,June,July,Aug,Sept,Oct,Nov,Dec', 
         'days':'1,32'}
+    params.update(config)
+    return params
 
-def create_config(params, out='.config'):
+def create_config(params, out='config.py'):
+    # if Path(out).exists():
+    
     with open(out, 'w') as o:
         for k,v in params.items():
             if isinstance(v,list) : 
                 o.write(f'{k}={",".join(v)}\n')
             elif isinstance(v, range):
                 o.write(f'{k}={v.start},{v.stop}\n')
             else:
                 o.write(f'{k}={v}\n')
     return f'configfile:{out}'
+    
 
 parser = argparse.ArgumentParser('scoobi',description="""
 Solar Conventionality-based Organizing Observation data ( SCOOBI )""", formatter_class=argparse.RawDescriptionHelpFormatter)
 
 # pa = parser.add_subparsers(help='compare datetimes') # subparser is used like $pip "install"
 
 parser.add_argument('-f','--fits_folder', help='source') #positionals
@@ -105,15 +117,17 @@
     if mm: params['month']=mm.split(',')
     params['days']=range(int(dd[0]),int(dd[1]))    
     params={k: v for k, v in params.items() if v is not None}
     if Path(configfile).exists() and args.rc: params.update(read_configfile(configfile))
 
     if args.ct and not args.no_datedfolder: compare_datetime(**params)
     if args.no_datedfolder and args.ct: compare_datetime_nofolder(**params)
-    if args.rc: print(read_configfile(configfile))
+    if args.rc: 
+        params.update(read_configfile(configfile))
+        print(params)
     if args.cc: print(create_config(params,configfile))
     if args.rt: print(str(read_tif(params['tiff_folder'])['Image DateTime'].values))
     if args.do: 
         if args.tiff_folder:
             if '.tif' not in params['tiff_folder']: 
                 print(tif2fits_bulk(params['tiff_folder'].split(','), destfolder=params['fits_folder']))
             else:
```

### Comparing `scoobi-0.0.1.6/src/scoobi/fitscubetofits.py` & `scoobi-0.0.1.7/src/scoobi/fitscubetofits.py`

 * *Files identical despite different names*

### Comparing `scoobi-0.0.1.6/src/scoobi.egg-info/PKG-INFO` & `scoobi-0.0.1.7/src/scoobi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoobi
-Version: 0.0.1.6
+Version: 0.0.1.7
 Summary: Solar Conventionality-based Organizing Observation data ( SCOOBI )
 Home-page: https://github.com/avialxee/scoobi
 Author: Avinash Kumar
 Author-email: avialxee@gmail.com
 Project-URL: Bug Tracker, https://github.com/avialxee/scoobi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

