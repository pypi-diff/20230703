# Comparing `tmp/scoobi-0.0.1.5.tar.gz` & `tmp/scoobi-0.0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoobi-0.0.1.5.tar", last modified: Sun May  7 20:36:40 2023, max compression
+gzip compressed data, was "scoobi-0.0.1.6.tar", last modified: Sun Jul  2 22:06:26 2023, max compression
```

## Comparing `scoobi-0.0.1.5.tar` & `scoobi-0.0.1.6.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:36:40.509817 scoobi-0.0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-07 20:36:27.000000 scoobi-0.0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-05-07 20:36:40.509817 scoobi-0.0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-07 20:36:27.000000 scoobi-0.0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-07 20:36:40.509817 scoobi-0.0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-07 20:36:27.000000 scoobi-0.0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:36:40.505818 scoobi-0.0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:36:40.509817 scoobi-0.0.1.5/src/scoobi/
--rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-05-07 20:36:27.000000 scoobi-0.0.1.5/src/scoobi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-05-07 20:36:27.000000 scoobi-0.0.1.5/src/scoobi/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:36:40.509817 scoobi-0.0.1.5/src/scoobi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-05-07 20:36:40.000000 scoobi-0.0.1.5/src/scoobi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-07 20:36:40.000000 scoobi-0.0.1.5/src/scoobi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:36:40.000000 scoobi-0.0.1.5/src/scoobi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-07 20:36:40.000000 scoobi-0.0.1.5/src/scoobi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-07 20:36:40.000000 scoobi-0.0.1.5/src/scoobi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 20:36:40.000000 scoobi-0.0.1.5/src/scoobi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:26.888028 scoobi-0.0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-02 22:06:11.000000 scoobi-0.0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-02 22:06:26.888028 scoobi-0.0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-02 22:06:11.000000 scoobi-0.0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-02 22:06:26.888028 scoobi-0.0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-02 22:06:11.000000 scoobi-0.0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:26.880028 scoobi-0.0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:26.884028 scoobi-0.0.1.6/src/scoobi/
+-rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-07-02 22:06:11.000000 scoobi-0.0.1.6/src/scoobi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-07-02 22:06:11.000000 scoobi-0.0.1.6/src/scoobi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-02 22:06:11.000000 scoobi-0.0.1.6/src/scoobi/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-07-02 22:06:11.000000 scoobi-0.0.1.6/src/scoobi/fitscubetofits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:26.888028 scoobi-0.0.1.6/src/scoobi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-02 22:06:26.000000 scoobi-0.0.1.6/src/scoobi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-02 22:06:26.000000 scoobi-0.0.1.6/src/scoobi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 22:06:26.000000 scoobi-0.0.1.6/src/scoobi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-02 22:06:26.000000 scoobi-0.0.1.6/src/scoobi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-02 22:06:26.000000 scoobi-0.0.1.6/src/scoobi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 22:06:26.000000 scoobi-0.0.1.6/src/scoobi.egg-info/top_level.txt
```

### Comparing `scoobi-0.0.1.5/LICENSE` & `scoobi-0.0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scoobi-0.0.1.5/PKG-INFO` & `scoobi-0.0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoobi
-Version: 0.0.1.5
+Version: 0.0.1.6
 Summary: Solar Conventionality-based Organizing Observation data ( SCOOBI )
 Home-page: https://github.com/avialxee/scoobi
 Author: Avinash Kumar
 Author-email: avialxee@gmail.com
 Project-URL: Bug Tracker, https://github.com/avialxee/scoobi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -17,41 +17,43 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # scoobi
 Solar Conventionality-based Organizing Observation data ( SCOOBI )
 
 ```bash
-usage: scoobi [-h] [-f FITS_FOLDER] [-t TIFF_FOLDER] [-o OUTPUT_FILE] [-c CONFIG_FILE] [-hdr HEADER] [-hf HEADER_FILE]
-              [-hfo HEADER_FILE_OUTPUT] [-mm MONTH] [-dd DAYS] [--no-datedfolder] [-rt] [-ct] [-rc] [-cc] [-do] [-th]
+age: scoobi [-h] [-f FITS_FOLDER] [-t TIFF_FOLDER] [-r RAW_FOLDER] [-o OUTPUT_FILE] [-c CONFIG_FILE] [-hdr HEADER] [-hf HEADER_FILE] [-hfo HEADER_FILE_OUTPUT]
+              [-mm MONTH] [-dd DAYS] [--no-datedfolder] [-rt] [-ct] [-rc] [-cc] [-do] [-th]
 
 Solar Conventionality-based Organizing Observation data ( SCOOBI )
 
 optional arguments:
   -h, --help            show this help message and exit
   -f FITS_FOLDER, --fits_folder FITS_FOLDER
                         source
   -t TIFF_FOLDER, --tiff_folder TIFF_FOLDER
-                        tiff folder path
+                        RAW TIFF folder path
+  -r RAW_FOLDER, --raw_folder RAW_FOLDER
+                        RAW FITS folder path
   -o OUTPUT_FILE, --output_file OUTPUT_FILE
                         complete path for output csv or log file.
   -c CONFIG_FILE, --config_file CONFIG_FILE
                         complete path for config file with inputs
   -mm MONTH, --month MONTH
                         comma separated month names
   -dd DAYS, --days DAYS
                         comma separated month names for range(a,b) Ex --days='1,32'
   --no-datedfolder      if not needed to create dated folder
   -rt, --read-time      reads time from a tiff file
   -ct, --compare-time   compares time from a fits file to a tiff file
   -rc, --read-config    read config, bool
   -cc, --create-config  create config, if called with rc would modify from and to the CONFIG_FILE path
-  -do, --do-conversion  create fits from tiff file and take care of the folder structure. Requires tiff_folder path
-  -th, --thumbnail      True/False for creating thumbnails; The fits folder path is required but should be more specific
-                        e.g atleaset including the /processed; should not be used with -do
+  -do, --do-conversion  create fits from tiff/fits raw file and take care of the folder structure. Requires tiff_folder or raw_folder path
+  -th, --thumbnail      True/False for creating thumbnails; The fits folder path is required but should be more specific e.g atleaset including the /processed; should
+                        not be used with -do
 
 header:
   Parameters for injecting and printing headers.
   [[Work in Progress]]
 
   -hdr HEADER, --header HEADER
                         Comma separated input headers to inject to the raw file.
@@ -70,25 +72,25 @@
 
 ### Folder structure
 
 - solar_data
     - final
         > contains fits files and thumbnails
         - YEAR (int[4])
-          - MONTH (int[2])
-             - DAY (int[2])
+          - MONTH (str[3])
+             - DAY (int[8])
                 - .fits file
                 - thumbnails/
                     - .fits file path.stem + 'jpg'
         
     - processed
         > contains fits files
         - YEAR (int[4])
-           - MONTH (int[2])
-             - DAY (int[2])
+           - MONTH (str[3])
+             - DAY (int[8])
                 - .fits file
                     
     - raw
         > raw telescope data
       - YEAR (int[4])
           - Month (int[2])
               - Day (int[2])
```

### Comparing `scoobi-0.0.1.5/README.md` & `scoobi-0.0.1.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 # scoobi
 Solar Conventionality-based Organizing Observation data ( SCOOBI )
 
 ```bash
-usage: scoobi [-h] [-f FITS_FOLDER] [-t TIFF_FOLDER] [-o OUTPUT_FILE] [-c CONFIG_FILE] [-hdr HEADER] [-hf HEADER_FILE]
-              [-hfo HEADER_FILE_OUTPUT] [-mm MONTH] [-dd DAYS] [--no-datedfolder] [-rt] [-ct] [-rc] [-cc] [-do] [-th]
+age: scoobi [-h] [-f FITS_FOLDER] [-t TIFF_FOLDER] [-r RAW_FOLDER] [-o OUTPUT_FILE] [-c CONFIG_FILE] [-hdr HEADER] [-hf HEADER_FILE] [-hfo HEADER_FILE_OUTPUT]
+              [-mm MONTH] [-dd DAYS] [--no-datedfolder] [-rt] [-ct] [-rc] [-cc] [-do] [-th]
 
 Solar Conventionality-based Organizing Observation data ( SCOOBI )
 
 optional arguments:
   -h, --help            show this help message and exit
   -f FITS_FOLDER, --fits_folder FITS_FOLDER
                         source
   -t TIFF_FOLDER, --tiff_folder TIFF_FOLDER
-                        tiff folder path
+                        RAW TIFF folder path
+  -r RAW_FOLDER, --raw_folder RAW_FOLDER
+                        RAW FITS folder path
   -o OUTPUT_FILE, --output_file OUTPUT_FILE
                         complete path for output csv or log file.
   -c CONFIG_FILE, --config_file CONFIG_FILE
                         complete path for config file with inputs
   -mm MONTH, --month MONTH
                         comma separated month names
   -dd DAYS, --days DAYS
                         comma separated month names for range(a,b) Ex --days='1,32'
   --no-datedfolder      if not needed to create dated folder
   -rt, --read-time      reads time from a tiff file
   -ct, --compare-time   compares time from a fits file to a tiff file
   -rc, --read-config    read config, bool
   -cc, --create-config  create config, if called with rc would modify from and to the CONFIG_FILE path
-  -do, --do-conversion  create fits from tiff file and take care of the folder structure. Requires tiff_folder path
-  -th, --thumbnail      True/False for creating thumbnails; The fits folder path is required but should be more specific
-                        e.g atleaset including the /processed; should not be used with -do
+  -do, --do-conversion  create fits from tiff/fits raw file and take care of the folder structure. Requires tiff_folder or raw_folder path
+  -th, --thumbnail      True/False for creating thumbnails; The fits folder path is required but should be more specific e.g atleaset including the /processed; should
+                        not be used with -do
 
 header:
   Parameters for injecting and printing headers.
   [[Work in Progress]]
 
   -hdr HEADER, --header HEADER
                         Comma separated input headers to inject to the raw file.
@@ -51,25 +53,25 @@
 
 ### Folder structure
 
 - solar_data
     - final
         > contains fits files and thumbnails
         - YEAR (int[4])
-          - MONTH (int[2])
-             - DAY (int[2])
+          - MONTH (str[3])
+             - DAY (int[8])
                 - .fits file
                 - thumbnails/
                     - .fits file path.stem + 'jpg'
         
     - processed
         > contains fits files
         - YEAR (int[4])
-           - MONTH (int[2])
-             - DAY (int[2])
+           - MONTH (str[3])
+             - DAY (int[8])
                 - .fits file
                     
     - raw
         > raw telescope data
       - YEAR (int[4])
           - Month (int[2])
               - Day (int[2])
```

### Comparing `scoobi-0.0.1.5/setup.py` & `scoobi-0.0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as rdme:
     desc = rdme.read()
 
 setup(
     name = 'scoobi',
-    version = '0.0.1.5',
+    version = '0.0.1.6',
     url='https://github.com/avialxee/scoobi',
     author='Avinash Kumar',
     author_email='avialxee@gmail.com',
     description='Solar Conventionality-based Organizing Observation data ( SCOOBI )',
     py_modules = ["scoobi"],
     package_dir={'':'src'},
     classifiers=["Programming Language :: Python :: 3",
```

### Comparing `scoobi-0.0.1.5/src/scoobi/__init__.py` & `scoobi-0.0.1.6/src/scoobi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from astropy.io import fits
 from astropy.time import Time
 import astropy.units as u
 from collections import defaultdict
 import csv
 import datetime
 import shutil
+from scoobi.config import usemagick, thumbnails, thumbnails_root, rootfolder
 
 
 class SCOOBI():
     def __init__():
         pass
 
 # Helper
@@ -69,48 +70,49 @@
     }
     header_params.update(kwargs)
     with fits.open(fitsfile, 'update') as f:
         for hdu in f:
             hdu.header.update(header_params)
             hdu.header['FILENAME'] = tifpath.name
 
-def build_foldername(fitsname, **kwargs):
+def build_foldername(filename,createdir=True, **kwargs):
     """
     Builds folder name taking input of the fitsfile name i.e
     destfolder + 
 
     *Parameters*
     
-    :fitsname: 
+    :filename: 
         (str) (Required)
 
         This is the conventional name of the fitsfile which will be used to build the folder path.
         Ex. S-2022-11-01T02:02:20.001-HA.fits
 
     :destfolder: 
-        (str) (Optional) (Default:None)
+        (str) (Optional) (Default:'')
 
         The destination folder name where all the files will get saved.
 
     *Return*
     
-        (str) complete path for the fitsfile.
+        (str) complete path for the file.
 
     """
-    params={'destfolder': 'processed/',
+    params={'destfolder': '',
     }
     params.update(kwargs)
-        
-    dcf=fitsname.split('-')
-    dcf_date=dcf[3].split('T')[0]
-    #currentfolder=f'{params["rootfolder"]}{params["destfolder"]}{dcf[1]}/{dcf[1]}{dcf[2]}{dcf_date}/'
-    currentfolder=f'{params["destfolder"]}/{dcf[1]}/{dcf[2]}/{dcf_date}/'
-    if not Path(currentfolder).exists():
-        Path(currentfolder).mkdir(parents=True,exist_ok=True)
-    return f'{currentfolder}{fitsname}'
+    if not params['destfolder']: params['destfolder']=f"{params['fits_folder']}"
+    dbf=filename.split('-') # date-wise build foldername
+    dbf_date=dbf[3].split('T')[0]
+    # YEAR[int4]/MONTH[str3]/yyyymmdd/S-yyyy-mm-ddTtime.fits
+    mm_str=datetime.datetime.strptime(dbf[2],"%m").strftime("%b").capitalize()
+    builtfolder=f'{params["destfolder"]}{dbf[1]}/{mm_str}/{dbf[1]}{dbf[2]}{dbf_date}/'
+    if not Path(builtfolder).exists() and createdir:
+        Path(builtfolder).mkdir(parents=True,exist_ok=True)
+    return f'{builtfolder}{filename}'
         
 def fits_to_fits(fitsfile_i, header=None, **kwargs):
     """
     *Parameters*
     
     :fitsfile_i:
         (str) (Required)
@@ -149,34 +151,40 @@
     """
     params={'fitsname':None, 'telescope':'HA', 'initial':'S'}
     params.update(kwargs)
     fitsfile_o=None
     
     if header:
         pass
-    print(f'{fitsfile_i}')
     with fits.open(fitsfile_i, 'readonly',) as hdul:
+        print('fits opned')
         if len(hdul[0].data.shape)==3:hdul[0].data=hdul[0].data[0]
         date=hdul[0].header['DATE-OBS']
+        print(f'read date:{date}')
         for hdu in hdul:
             hdu.header.update(header)
             hdu.header['TELESCOP']=params['telescope']
             hdu.header['FILENAME']=Path(fitsfile_i).name
             
         if params['fitsname'] is None:
             # name convention : *S + DATETIME + TELESCOPE*
+            print('building foldername:')
+
             fitsfile_o=f"{params['initial']}-{date}-{params['telescope']}.fits"
             fitsfile_o=build_foldername(fitsfile_o, **kwargs)
+            print(fitsfile_o)
         else:
+            
             fitsfile_o=build_foldername(params['fitsname'])
+            
         hdul.writeto(fitsfile_o, overwrite=True)
     return fitsfile_o
     # data,hdrdata=scidata[0][0], scidata[1] # taking data[0] as data is 3D
     
-def tif_to_fits(tiffile, magick=True, header=None, **kwargs):
+def tif_to_fits(tiffile, magick=usemagick, header=None, **kwargs):
     """
     *Parameters*
     
     :tiffile:
         (str) (Required)
 
         Full path of the TIFF file that needs to be converted to FITS.
@@ -234,30 +242,47 @@
             fitspath = Path(fitsfile)
             hdu.header.update(header)
             hdu.header['TELESCOP']=params['telescope']
             hdu.header['FILENAME']=fitspath.name
             hdu.header['HISTORY']=f'{tiffile}'
             hdu.header['HISTORY']=f'scoobi'
 
-def thumb_gen(fits_folder, out_folder=None, thumb_folder="Thumbnails", force=False):
+def thumbgen(fitsfile, out_folder=None, thumb_folder=thumbnails, force=False):
     """
     Creates thumbnails for the fits file provided in the fits_folder path.
+    depends on build_foldername 
+    else if thumb_folder is specified with out_folder jpgfile is created accordingly.
+    ex. out_folder,thumb_foler='/data/solardata/','Thumbnails/'
+
+    """
+    if fitsfile:        
+        jpgfile_name=f"{Path(fitsfile).stem}.jpg"
+        if out_folder is None:out_folder=Path(fitsfile).parent
+        jpgfile=f'{out_folder}/{thumb_folder}/{jpgfile_name}'
+        if not Path(jpgfile).exists(): Path(jpgfile).parent.mkdir(parents=True,exist_ok=True)
+        if not Path(jpgfile).exists() or force: subprocess.run(["convert", fitsfile,"-linear-stretch","1x1","-resize", "56%", jpgfile ])
+        return jpgfile
+
+def thumbgen_bulk(fits_folder, thumb_folder=thumbnails, thumb_root=thumbnails_root, force=False, **kwargs):
+    """
+    calls thumb_gen for converting fits to jpg and then copies to a directory specified by :thumb_root:
     """
-    if fits_folder:
-        allfile=search_file(f"{fits_folder}/",'.fits', recursive=True)
+    
+    allfile=search_file(f"{fits_folder}/",'.fits', recursive=True)
+    for fitsfile in allfile:
+        jpgfile=thumbgen(fitsfile,thumb_folder=thumb_folder,force=force)
+
+        outfolder_root=build_foldername(Path(fitsfile).name,createdir=False, destfolder='/')
+        jpgfile_root=f"{thumb_root}/{Path(outfolder_root).parent}/{Path(jpgfile).name}"
         
-        for fitsfile in allfile:
-            print(f"{fitsfile} is read")
-            out_folder=Path(fitsfile).parent
-            jpgfolder=f"{out_folder}/{thumb_folder}"
-            jpgfile=f"{jpgfolder}/{Path(fitsfile).stem}.jpg"
-            print(f"jpgfolder:{jpgfolder}")
-            if not Path(jpgfolder).exists(): Path(jpgfolder).mkdir(parents=True,exist_ok=True)
-            if not Path(jpgfile).exists() or force: subprocess.run(["convert", fitsfile,"-linear-stretch","1x1","-resize", "56%", jpgfile ])
+        if not Path(jpgfile_root).exists() or force: 
+            Path(jpgfile_root).parent.mkdir(parents=True,exist_ok=True)
+            shutil.copy(str(jpgfile), str(jpgfile_root))
 
+            
 def fits2fits_bulk(fitsfolderlist, **kwargs):
     """
     takes input as list of string fits folder paths and executes fits_to_fits() using for loop to each folder path.
     see *fits_to_fits()* for the list of parameters.
     If fits to fits conversion fails, the file is saved in "corrupt/" (can be changed from call) folder at the tiff source folder.
     """
     params={'failed_folder':'corrupt/'}
```

### Comparing `scoobi-0.0.1.5/src/scoobi/cli.py` & `scoobi-0.0.1.6/src/scoobi/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
-from scoobi import compare_datetime, read_tif, Time, tif2fits_bulk, tif_to_fits, compare_datetime_nofolder, thumb_gen,fits2fits_bulk,fits_to_fits
+from scoobi import compare_datetime, read_tif, Time, tif2fits_bulk, tif_to_fits, compare_datetime_nofolder, thumbgen_bulk,fits2fits_bulk,fits_to_fits
 from collections import defaultdict
 from pathlib import Path
+from scoobi.config import rootfolder,processedfolder,processed,thumbnails_root,rawfolder,hc,lc,darks,flat,corrupted_folder
 
 def read_configfile(filepath):
     with open(filepath,'r') as f:
         params = defaultdict(list)
         pr=f.read().splitlines()
         for i in range(len(pr)):
             if '#' in pr[i]:
@@ -18,18 +19,19 @@
                     dd=v.split(',')
                     params[k]=range(int(dd[0]),int(dd[1])) 
                 else:
                     params[k]=v
     return params
 
 def default_params():
-    return {'fits_folder':'/data/solar_data/processed', 
-        'csv_file':'/data/solar_data/raw/log.csv',
-        'tiff_folder':'/data/solar_data/raw/',
-        'raw_folder':'/data/solar_data/raw/', 
+    return {'fits_folder':processedfolder,
+        'csv_file':f'{rootfolder}log.csv',
+        'tiff_folder':rawfolder,
+        'raw_folder':rawfolder, 
+        'rootfolder':rootfolder,
         'month':'Jan,Feb,Mar,Apr,May,June,July,Aug,Sept,Oct,Nov,Dec', 
         'days':'1,32'}
 
 def create_config(params, out='.config'):
     with open(out, 'w') as o:
         for k,v in params.items():
             if isinstance(v,list) : 
@@ -117,11 +119,11 @@
             else:
                 print(tif_to_fits(params['tiff_folder'], destfolder=params['fits_folder']))
         if args.raw_folder:
             if not any(fts in params['raw_folder'] for fts in ['.fits', '.fts']): 
                 print(fits2fits_bulk(params['raw_folder'].split(','), destfolder=params['fits_folder']))
             else:
                 print(fits_to_fits(params['raw_folder'], destfolder=params['fits_folder']))
-    if args.th: thumb_gen(params['fits_folder'])
+    if args.th: print(thumbgen_bulk(params['fits_folder'],rootfolder=params['rootfolder']))
         
 if __name__=='__main__':
     cli()
```

### Comparing `scoobi-0.0.1.5/src/scoobi.egg-info/PKG-INFO` & `scoobi-0.0.1.6/src/scoobi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoobi
-Version: 0.0.1.5
+Version: 0.0.1.6
 Summary: Solar Conventionality-based Organizing Observation data ( SCOOBI )
 Home-page: https://github.com/avialxee/scoobi
 Author: Avinash Kumar
 Author-email: avialxee@gmail.com
 Project-URL: Bug Tracker, https://github.com/avialxee/scoobi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -17,41 +17,43 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # scoobi
 Solar Conventionality-based Organizing Observation data ( SCOOBI )
 
 ```bash
-usage: scoobi [-h] [-f FITS_FOLDER] [-t TIFF_FOLDER] [-o OUTPUT_FILE] [-c CONFIG_FILE] [-hdr HEADER] [-hf HEADER_FILE]
-              [-hfo HEADER_FILE_OUTPUT] [-mm MONTH] [-dd DAYS] [--no-datedfolder] [-rt] [-ct] [-rc] [-cc] [-do] [-th]
+age: scoobi [-h] [-f FITS_FOLDER] [-t TIFF_FOLDER] [-r RAW_FOLDER] [-o OUTPUT_FILE] [-c CONFIG_FILE] [-hdr HEADER] [-hf HEADER_FILE] [-hfo HEADER_FILE_OUTPUT]
+              [-mm MONTH] [-dd DAYS] [--no-datedfolder] [-rt] [-ct] [-rc] [-cc] [-do] [-th]
 
 Solar Conventionality-based Organizing Observation data ( SCOOBI )
 
 optional arguments:
   -h, --help            show this help message and exit
   -f FITS_FOLDER, --fits_folder FITS_FOLDER
                         source
   -t TIFF_FOLDER, --tiff_folder TIFF_FOLDER
-                        tiff folder path
+                        RAW TIFF folder path
+  -r RAW_FOLDER, --raw_folder RAW_FOLDER
+                        RAW FITS folder path
   -o OUTPUT_FILE, --output_file OUTPUT_FILE
                         complete path for output csv or log file.
   -c CONFIG_FILE, --config_file CONFIG_FILE
                         complete path for config file with inputs
   -mm MONTH, --month MONTH
                         comma separated month names
   -dd DAYS, --days DAYS
                         comma separated month names for range(a,b) Ex --days='1,32'
   --no-datedfolder      if not needed to create dated folder
   -rt, --read-time      reads time from a tiff file
   -ct, --compare-time   compares time from a fits file to a tiff file
   -rc, --read-config    read config, bool
   -cc, --create-config  create config, if called with rc would modify from and to the CONFIG_FILE path
-  -do, --do-conversion  create fits from tiff file and take care of the folder structure. Requires tiff_folder path
-  -th, --thumbnail      True/False for creating thumbnails; The fits folder path is required but should be more specific
-                        e.g atleaset including the /processed; should not be used with -do
+  -do, --do-conversion  create fits from tiff/fits raw file and take care of the folder structure. Requires tiff_folder or raw_folder path
+  -th, --thumbnail      True/False for creating thumbnails; The fits folder path is required but should be more specific e.g atleaset including the /processed; should
+                        not be used with -do
 
 header:
   Parameters for injecting and printing headers.
   [[Work in Progress]]
 
   -hdr HEADER, --header HEADER
                         Comma separated input headers to inject to the raw file.
@@ -70,25 +72,25 @@
 
 ### Folder structure
 
 - solar_data
     - final
         > contains fits files and thumbnails
         - YEAR (int[4])
-          - MONTH (int[2])
-             - DAY (int[2])
+          - MONTH (str[3])
+             - DAY (int[8])
                 - .fits file
                 - thumbnails/
                     - .fits file path.stem + 'jpg'
         
     - processed
         > contains fits files
         - YEAR (int[4])
-           - MONTH (int[2])
-             - DAY (int[2])
+           - MONTH (str[3])
+             - DAY (int[8])
                 - .fits file
                     
     - raw
         > raw telescope data
       - YEAR (int[4])
           - Month (int[2])
               - Day (int[2])
```

