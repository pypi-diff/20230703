# Comparing `tmp/starcatalogquery-0.1.7-py3-none-any.whl.zip` & `tmp/starcatalogquery-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 27073 bytes, number of entries: 17
+Zip file size: 27770 bytes, number of entries: 17
 -rw-r--r--  2.0 unx       33 b- defN 23-May-08 07:01 starcatalogquery/__init__.py
--rw-r--r--  2.0 unx     6048 b- defN 23-May-09 01:27 starcatalogquery/catalog_check.py
--rw-r--r--  2.0 unx     6716 b- defN 23-May-09 01:26 starcatalogquery/catalog_download.py
--rw-r--r--  2.0 unx    15124 b- defN 23-May-08 13:32 starcatalogquery/catalog_query.py
--rw-r--r--  2.0 unx    51243 b- defN 23-Jun-16 03:40 starcatalogquery/classes.py
+-rw-r--r--  2.0 unx     6049 b- defN 23-Jun-18 09:44 starcatalogquery/catalog_check.py
+-rw-r--r--  2.0 unx     6727 b- defN 23-Jun-18 09:49 starcatalogquery/catalog_download.py
+-rw-r--r--  2.0 unx    16654 b- defN 23-Jul-03 08:08 starcatalogquery/catalog_query.py
+-rw-r--r--  2.0 unx    51269 b- defN 23-Jun-19 23:39 starcatalogquery/classes.py
 -rw-r--r--  2.0 unx     3078 b- defN 23-May-12 08:00 starcatalogquery/invariantfeatures.py
--rw-r--r--  2.0 unx     5624 b- defN 23-May-10 03:48 starcatalogquery/tiles_draw.py
+-rw-r--r--  2.0 unx     5684 b- defN 23-Jul-03 14:28 starcatalogquery/tiles_draw.py
 -rw-r--r--  2.0 unx     1978 b- defN 23-May-30 08:00 starcatalogquery/wcs.py
 -rw-r--r--  2.0 unx        1 b- defN 23-May-11 04:20 starcatalogquery/utils/__init__.py
 -rw-r--r--  2.0 unx      612 b- defN 23-May-09 08:08 starcatalogquery/utils/df2info.py
--rw-r--r--  2.0 unx     4272 b- defN 23-May-09 08:33 starcatalogquery/utils/starcatalog_statistic.py
+-rw-r--r--  2.0 unx     4274 b- defN 23-Jun-18 09:43 starcatalogquery/utils/starcatalog_statistic.py
 -rw-r--r--  2.0 unx      477 b- defN 23-May-09 08:06 starcatalogquery/utils/try_download.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jun-16 03:53 starcatalogquery-0.1.7.dist-info/LICENSE
--rw-r--r--  2.0 unx    12259 b- defN 23-Jun-16 03:53 starcatalogquery-0.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 03:53 starcatalogquery-0.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jun-16 03:53 starcatalogquery-0.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1510 b- defN 23-Jun-16 03:53 starcatalogquery-0.1.7.dist-info/RECORD
-17 files, 110152 bytes uncompressed, 24553 bytes compressed:  77.7%
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jul-03 14:47 starcatalogquery-0.1.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12582 b- defN 23-Jul-03 14:47 starcatalogquery-0.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 14:47 starcatalogquery-0.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jul-03 14:47 starcatalogquery-0.1.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1510 b- defN 23-Jul-03 14:47 starcatalogquery-0.1.8.dist-info/RECORD
+17 files, 112105 bytes uncompressed, 25250 bytes compressed:  77.5%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: starcatalogquery/utils/starcatalog_statistic.py
 Comment: 
 
 Filename: starcatalogquery/utils/try_download.py
 Comment: 
 
-Filename: starcatalogquery-0.1.7.dist-info/LICENSE
+Filename: starcatalogquery-0.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: starcatalogquery-0.1.7.dist-info/METADATA
+Filename: starcatalogquery-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: starcatalogquery-0.1.7.dist-info/WHEEL
+Filename: starcatalogquery-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: starcatalogquery-0.1.7.dist-info/top_level.txt
+Filename: starcatalogquery-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: starcatalogquery-0.1.7.dist-info/RECORD
+Filename: starcatalogquery-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## starcatalogquery/catalog_check.py

```diff
@@ -75,15 +75,15 @@
 
     Usage:
         >>> dir_from = '/Volumes/TOSHIBA/starcatalogs/raw/ucac5/res2/'
         >>> tile_size = 2 # in [deg]
         >>> dir_from,dir_size,file_num,validity = catalog_check(scname,tile_size,dir_from)
 
     Inputs:
-        scname -> [str] Name of the starcatalog. Available starcatalogs include 'hygv3', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
+        scname -> [str] Name of the starcatalog. Available starcatalogs include 'hygv35', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
         tile_size -> [int] size of tile in [deg]
         dir_from -> [str,optional,default=None] Path of the starcatalog tile files. 
 
     Outputs:
         dir_from -> [str] Path of the starcatalog tile files. If None, the path is assigned to 'starcatalogs/raw/<scname>/<resx>/' by default.
         dir_size -> [float] The size of the star catalog.
         file_num -> [int] Total number of the tile files.
```

## starcatalogquery/catalog_download.py

```diff
@@ -11,15 +11,15 @@
     """
     Download starcatalog tile files from https://outerspace.stsci.edu/display/GC
 
     Usage: 
         >>> dir_to,tile_size = catalog_download('gsc12')
 
     Inputs:
-        scname -> [str] Name of the starcatalog to download. Available starcatalogs include 'hygv3', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
+        scname -> [str] Name of the starcatalog to download. Available starcatalogs include 'hygv35', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
         tile_size -> [int,optinal,default=None] size of tile in [deg]
         dir_to -> [str,optional,default=None] Download path of the starcatalog
 
     Outputs: 
         dir_to -> [str] Path of the starcatalog tile files. If None, the path is assigned to 'starcatalogs/raw/<scname>/<resx>/' by default.
         tile_size -> [int] Size of tile in [deg]. If None, the size of the tile is automatically assigned a feasible maximum according to the name of the star catalog.
 
@@ -81,62 +81,63 @@
     print('Downloading the catalog tile files for {:s}'.format(scname),end = '...')  
     os.system('cat url_{:s}.txt | xargs -P 16 -n 2 wget -c -O'.format(scname))
     print('Finished')  
     os.remove(url_file)
 
     return dir_to,tile_size  
 
-def hygv3_download(tile_size=None,dir_to=None):
+def hygv35_download(tile_size=None,dir_to=None):
     """
-    Download the HYG v3 database and convert it to the tile mode.
+    Download the HYG v35 database and convert it to the tile mode.
 
     Usage: 
-        >>> dir_to,tile_size = hygv3_download(5)
+        >>> dir_to,tile_size = hygv35_download(5)
 
     Inputs:
         tile_size -> [int,optinal,default=None] size of tile in [deg]
         dir_to -> [str,optional,default=None] Download path of the starcatalog    
 
     Outputs: 
-        dir_to -> [str] Path of the starcatalog tile files. If None, the path is assigned to 'starcatalogs/raw/hygv3/<resx>/' by default.
+        dir_to -> [str] Path of the starcatalog tile files. If None, the path is assigned to 'starcatalogs/raw/hygv35/<resx>/' by default.
         dir_size -> [float] The size of the star catalog.
         file_num -> [int] Total number of the tile files.
         validity -> [bool] The validity of the star catalog. 
         tile_size -> [int] Size of tile in [deg]. If None, default = 2.
     """
 
     if tile_size is None:
         tile_size = 2
     else:    
         # for pyshtools, N = 180//tile_size must be even.
         if tile_size not in [1,2,3,5,6,9,10]: raise Exception('tile size must be in [1,2,3,5,6,9,10] deg')  
 
     raw_dir_to = str(Path.home()) + '/src/starcatalogs/data/'
-    raw_file = 'hygdata_v3.csv'
+    raw_file = 'hygdata_v35.csv'
     raw_dir_file = raw_dir_to + raw_file
 
-    url = 'https://astronexus.com/downloads/catalogs/hygdata_v3.csv.gz'
+    url = 'https://astronexus.com/downloads/catalogs/hygdata_v35.csv.gz'
+
     raw_dir_file_gz = raw_dir_to + url.split('/')[-1]
 
     if not os.path.exists(raw_dir_to): os.makedirs(raw_dir_to)
     if not os.path.exists(raw_dir_file):
-        desc = "Downloading the HYG v3 database '{:s}' from The Astronomy Nexus.".format(raw_file)
+        desc = "Downloading the HYG v35 database '{:s}' from The Astronomy Nexus.".format(raw_file)
         wget_out = wget_download(url,raw_dir_file_gz,desc)
         g_file = GzipFile(wget_out)
         open(raw_dir_file, "wb").write(g_file.read())
         g_file.close()
         os.remove(wget_out) 
 
     else:
         print("Star catalog file '{:s}' is already in {:s}".format(raw_file,raw_dir_to)) 
 
     # Now divide the entire star catalog file into multiple tile files
     print('Divide the entire star catalog file into multiple tile files',end='...')
     if dir_to is None:
-        dir_to = 'starcatalogs/raw/hygv3/res{:d}/'.format(tile_size)  
+        dir_to = 'starcatalogs/raw/hygv35/res{:d}/'.format(tile_size)  
     Path(dir_to).mkdir(parents=True, exist_ok=True) 
 
     df = pd.read_csv(raw_dir_file,skiprows=[1]) # remove the sun
     ra,dec = df['ra']*15,df['dec']  
 
     count_ra = 360//tile_size
     count_dec = 180//tile_size
@@ -147,15 +148,15 @@
             
             ra_flag = np.abs(ra - (ra_min + ra_max)/2) < (ra_max - ra_min)/2
             dec_flag = np.abs(dec- (dec_min + dec_max)/2) < (dec_max - dec_min)/2
             
             flag = ra_flag & dec_flag 
             df_sec = df[flag]
 
-            fn = open(dir_to+'hygv3-{:d}.csv'.format(count_ra *i+j), 'w')
+            fn = open(dir_to+'hygv35-{:d}.csv'.format(count_ra *i+j), 'w')
             fn.write('#Objects found : {:d}\n'.format(len(df_sec)))
             df_sec.to_csv(fn,index=False)   
             fn.close() 
     print('Finished')         
 
     # calculate total size and numbers of tile files    
     file_num,dir_size,validity = tiles_statistic(dir_to,tile_size)
```

## starcatalogquery/catalog_query.py

```diff
@@ -1,13 +1,61 @@
 import os
 import numpy as np
 import pandas as pd
-import pyshtools as pysh
 from astropy.coordinates import SkyCoord
 
+def from_cap(theta,clat,clon,lmax):
+    """
+    Mask grid points using spherical cap.
+    Reference: https://github.com/SHTOOLS/SHTOOLS/blob/master/pyshtools/shclasses/shgrid.py
+
+    Usage:
+        >>> mask_cap = from_cap(theta,clat,clon,lmax])
+    Inputs:
+        theta -> [float] The angular radius of the spherical cap in [deg]
+        clat, clon -> [float] Latitude and longitude of the center of the spherical cap in [deg]
+        lmax -> [int] The maximum spherical harmonic degree resolvable by the grid
+    Outputs:
+        mask_cap -> [numpy array] Grid points with spherical cap masked 
+    """
+    step = 90/(lmax+1)
+    lats = np.deg2rad(np.arange(90,-90,-step))
+    lons = np.deg2rad(np.arange(0,360,step))
+    nlat,nlon = len(lats),len(lons)
+    array = np.zeros((nlat, nlon))
+
+    theta = np.deg2rad(theta)
+    clat = np.deg2rad(clat)
+    clon = np.deg2rad(clon)
+
+    # Set array equal to 1 within the cap
+    imin = np.inf
+    imax = 0
+    for i, lat in enumerate(lats):
+        if lat <= clat + theta:
+            if i <= imin: imin = i
+        if lat >= clat - theta:
+            if i >= imax: imax = i
+
+    x = np.cos(clat) * np.cos(clon)
+    y = np.cos(clat) * np.sin(clon)
+    z = np.sin(clat)
+
+    coslon = np.cos(lons)
+    sinlon = np.sin(lons)
+    costheta = np.cos(theta)
+
+    for i in range(imin, imax+1):
+        coslat = np.cos(lats[i])
+        sinlat = np.sin(lats[i])
+        for j in range(0, nlon):
+            dist = coslat * (x * coslon[j] + y * sinlon[j]) + z * sinlat
+            if dist >= costheta: array[i, j] = 1
+    return array
+
 def seq2radec(seq,tile_size):
     """
     Given the indices of star catalog tile files, calculate the spherical rectangles corresponding to the indices.
 
     Usage:
         >>> radec_box,box_center = seq2radec(100,3)
         >>> radec_box,box_center = seq2radec([120,130],5)
@@ -91,30 +139,30 @@
         seqs -> [array of int] Indices of the star catalog tile files over the cone search area.
     """
     count_lon = 360//tile_size
     radius += tile_size*1.5 # buffer of boundary
     N = int(180/tile_size)
     if N%2: raise Exception('tile_size must satisfy the condition that 180/tile_size is even.')
     L = int(N/2) - 1
-    mask_circle = pysh.SHGrid.from_cap(radius, dec_c, ra_c, L,extend=False)
-    dec_index,ra_index = np.where(mask_circle.data)
+    mask_cap = from_cap(radius, dec_c, ra_c, L)
+    dec_index,ra_index = np.where(mask_cap)
     seqs = dec_index * count_lon + ra_index
     return seqs    
 
 def _load_files(sc_indices,sc_path,sc_name,_mode):
     """
     Build a generator for loading multiple star catalog tile files.
 
     Usage:
-        >>> _load_files([10,15,178,3430,8009,10002],'starcatalogs/raw/hygv3/res5/','hygv3,'raw')
+        >>> _load_files([10,15,178,3430,8009,10002],'starcatalogs/raw/hygv35/res5/','hygv35,'raw')
 
     Inputs:
         sc_indices -> [array of int] Indices of the star catalog tile files to load.  
-        sc_path -> [str] Path of starcatalog tile files, such as 'starcatalogs/raw/hygv3/res5/'
-        sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv3', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
+        sc_path -> [str] Path of starcatalog tile files, such as 'starcatalogs/raw/hygv35/res5/'
+        sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv35', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
         _mode -> [str] Types of star catalogs, including 'raw', 'reduced', 'simplified', where
             'raw' represents the original star catalog, which contains all information about the star
             'reduced' represents the reduced star catalog, which contains the position, proper motion, apparent magnitude, epoch of the star
             'simplified' represents the minimalist star catalog, which only includes the position and apparent magnitude of stars
     Outputs:
         A generator
     """
@@ -129,24 +177,24 @@
         if os.path.getsize(filename) > 25: yield pd.read_csv(filename,skiprows=skiprows,dtype=str) 
         
 def search_box_magpm(radec_box,sc_path,sc_name,tile_size,_mode,mag_threshold,t_pm):
     """
     Perform a rectangle search of stars on the reduced star catalog.
 
     Usage:
-        >>> df = search_box([20,30,30,40],'starcatalogs/reduced/hygv3/res5/','hygv3',5,'reduced',8,2023.5)
+        >>> df = search_box([20,30,30,40],'starcatalogs/reduced/hygv35/res5/','hygv35',5,'reduced',8,2023.5)
 
     Inputs:
         radec_box -> [int,array_like] Rectangular search area in format of [ra_min,dec_min,ra_max,dec_max], where
             ra_min -> [float] Left border of RA in [deg].
             dec_min -> [float] Lower border of DEC in [deg].
             ra_max -> [float] Right border of RA in [deg].
             dec_max -> [float] Upper border of DEC in [deg].
-        sc_path -> [str] Path of starcatalog tile files, such as 'starcatalogs/reduced/hygv3/'
-        sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv3', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
+        sc_path -> [str] Path of starcatalog tile files, such as 'starcatalogs/reduced/hygv35/'
+        sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv35', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
         tile_size -> [int] Size of the tile in [deg]
         _mode -> [str] Types of star catalogs, including 'raw', 'reduced', 'simplified', where
             'raw' represents the original star catalog, which contains all information about the star
             'reduced' represents the reduced star catalog, which contains the position, proper motion, apparent magnitude, epoch of the star
             'simplified' represents the minimalist star catalog, which only includes the position and apparent magnitude of stars
         mag_threshold -> [float] Apparent magnitude limit of the detector  
         t_pm -> [float] The epoch when the search was performed
@@ -188,23 +236,23 @@
     return df.reset_index(drop=True)   
 
 def search_cone_magpm(center,radius,sc_path,sc_name,tile_size,_mode,mag_threshold,t_pm):
     """
     Perform a cone search of stars on the reduced star catalog.
 
     Usage:
-        >>> df = search_cone([20,30],10,'starcatalogs/reduced/hygv3/res5/','hygv3',5,'reduced',8,2023.5)
+        >>> df = search_cone([20,30],10,'starcatalogs/reduced/hygv35/res5/','hygv35',5,'reduced',8,2023.5)
 
     Inputs:
         center -> [int,array_like] Center of the cap in format of [ra_c,dec_c], where
             ra_c -> [float] RA, in [deg].
             dec_c -> [float] DEC, in [deg].
         radius -> [float] Angular radius of the cap, in [deg].
-        sc_path -> [str] Path of starcatalog tile files, such as 'starcatalogs/reduced/hygv3/'
-        sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv3', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
+        sc_path -> [str] Path of starcatalog tile files, such as 'starcatalogs/reduced/hygv35/'
+        sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv35', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
         tile_size -> [int] Size of the tile in [deg]. Avaliable values are 1,2,3,5,6,9,10.
         _mode -> [str] Types of star catalogs, including 'raw', 'reduced', 'simplified', where
             'raw' represents the original star catalog, which contains all information about the star
             'reduced' represents the reduced star catalog, which contains the position, proper motion, apparent magnitude, epoch of the star
             'simplified' represents the minimalist star catalog, which only includes the position and apparent magnitude of stars
         mag_threshold -> [float] Apparent magnitude limit of the detector  
         t_pm -> [float] The epoch when the search was performed
@@ -246,24 +294,24 @@
     return df.reset_index(drop=True)   
 
 def search_box(radec_box,sc_path,sc_name,tile_size,_mode):
     """
     Perform a rectangle search of stars on the simplified star catalog.
 
     Usage:
-        >>> df = search_box([20,30,30,40],'starcatalogs/simplified/hygv3/res5/mag8.0/epoch2023.0/','hygv3',5,'simplified')
+        >>> df = search_box([20,30,30,40],'starcatalogs/simplified/hygv35/res5/mag8.0/epoch2023.0/','hygv35',5,'simplified')
 
     Inputs:
         radec_box -> [int,array_like] Rectangular search area in format of [ra_min,dec_min,ra_max,dec_max], where
             ra_min -> [float] Left border of RA in [deg].
             dec_min -> [float] Lower border of DEC in [deg].
             ra_max -> [float] Right border of RA in [deg].
             dec_max -> [float] Upper border of DEC in [deg].
-        sc_path -> [str] Path of starcatalog tile files, such as 'starcatalogs/reduced/hygv3/'
-        sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv3', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
+        sc_path -> [str] Path of starcatalog tile files, such as 'starcatalogs/reduced/hygv35/'
+        sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv35', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
         tile_size -> [int] Size of the tile in [deg]
         _mode -> [str] Types of star catalogs, including 'raw', 'reduced', 'simplified', where
             'raw' represents the original star catalog, which contains all information about the star
             'reduced' represents the reduced star catalog, which contains the position, proper motion, apparent magnitude, epoch of the star
             'simplified' represents the minimalist star catalog, which only includes the position and apparent magnitude of stars
 
     Outputs:
@@ -285,23 +333,23 @@
     return df.reset_index(drop=True)   
 
 def search_cone(center,radius,sc_path,sc_name,tile_size,_mode):
     """
     Perform a cone search of stars on the simplified star catalog.
 
     Usage:
-        >>> df = search_cone([20,30],10,'starcatalogs/simplified/hygv3/res5/mag8.0/epoch2023.0/','hygv3',5,'simplified')
+        >>> df = search_cone([20,30],10,'starcatalogs/simplified/hygv35/res5/mag8.0/epoch2023.0/','hygv35',5,'simplified')
 
     Inputs:
         center -> [int,array_like] Center of the cap in format of [ra_c,dec_c], where
             ra_c -> [float] RA, in [deg].
             dec_c -> [float] DEC, in [deg].
         radius -> [float] Angular radius of the cap, in [deg].
-        sc_path -> [str] Path of starcatalog tile files, such as 'starcatalogs/reduced/hygv3/'
-        sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv3', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
+        sc_path -> [str] Path of starcatalog tile files, such as 'starcatalogs/reduced/hygv35/'
+        sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv35', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
         tile_size -> [int] Size of the tile in [deg]. Avaliable values are 1,2,3,5,6,9,10.
         _mode -> [str] Types of star catalogs, including 'raw', 'reduced', 'simplified', where
             'raw' represents the original star catalog, which contains all information about the star
             'reduced' represents the reduced star catalog, which contains the position, proper motion, apparent magnitude, epoch of the star
             'simplified' represents the minimalist star catalog, which only includes the position and apparent magnitude of stars
 
     Outputs:
```

## starcatalogquery/classes.py

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 from astropy.time import Time
 from astropy.coordinates import SkyCoord
 from colorama import Fore
 import healpy as hp
 from scipy.spatial import KDTree
 
-from .catalog_download import catalog_download,hygv3_download
+from .catalog_download import catalog_download,hygv35_download
 from .catalog_check import catalog_check
 from .utils.starcatalog_statistic import tiles_statistic,starcatalog_info
 from .utils.df2info import df2info
 from .catalog_query import search_box,search_cone,search_box_magpm,search_cone_magpm,box2seqs,cone2seqs,_load_files
 from .tiles_draw import search_draw
 from .wcs import xy_catalog
 from .invariantfeatures import _generate_invariants
@@ -25,23 +25,23 @@
         Grab star catalog data files from a remote server.
 
         Usage:
             >>> from starcatalogquery import StarCatalog
             >>> gaiadr3_raw = StarCatalog.get('gaiadr3',2)
 
         Inputs:
-            sc_name -> [str] Name of the starcatalog to download. Available starcatalogs include 'hygv3', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
+            sc_name -> [str] Name of the starcatalog to download. Available starcatalogs include 'hygv35', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
             tile_size -> [int,optinal,default=None] size of the tile in [deg]. If None, the size of the tile is automatically assigned a feasible maximum according to the name of the star catalog.
             dir_to -> [str,optional,default=None] The download path of the star catalog files. If None, the path is automatically assigned to a suitable directory by default.
 
         Outputs:
             Instance of class StarCatalogRaw
         """
-        if sc_name == 'hygv3': # for HYG v3 star catalog
-            dir_to,dir_size,file_num,validity,tile_size = hygv3_download(tile_size,dir_to) 
+        if sc_name == 'hygv35': # for HYG v35 star catalog
+            dir_to,dir_size,file_num,validity,tile_size = hygv35_download(tile_size,dir_to) 
 
         else: # for other star catalogs
 
             if dir_to is None:
                 dir_to = 'starcatalogs/raw/{:s}/res{:d}/'.format(sc_name,tile_size) 
 
             if os.path.exists(dir_to):
@@ -84,15 +84,15 @@
         _mode,sc_name,tile_size = dir_from.split('starcatalogs/')[1].split('/')[:3]
         tile_size = int(tile_size[3:])
 
         # _mode -> [str] Types of star catalogs, including 'raw', 'reduced', 'simplified', where
         # 'raw' represents the original star catalog, which contains all information about the star
         # 'reduced' represents the reduced star catalog, which contains the position, proper motion, apparent magnitude, epoch of the star
         # 'simplified' represents the minimalist star catalog, which only includes the position and apparent magnitude of stars at a specific epoch
-        # sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv3', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
+        # sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv35', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
         # tile_size -> [int] Size of the tile in [deg]
 
         if _mode == 'raw':
             starcatalog = StarCatalogRaw.load(sc_name,tile_size,dir_from)
         elif _mode == 'reduced':
             starcatalog = StarCatalogReduced.load(sc_name,tile_size,dir_from)
         elif _mode == 'simplified':    
@@ -103,15 +103,15 @@
 
     def read_h5_indices(infile):
         """
         Read in h5-formatted star catalog file, which records the center pointing of each sky area, the pixel coordinates of the stars, the triangle invariants and the asterism indices.
 
         Usage:
             >>> from starcatalogquery import StarCatalog
-            >>> infile_h5 = 'starcatalogs/indices/hygv3/fov20_mag8_mcp40_2023.0.h5'
+            >>> infile_h5 = 'starcatalogs/indices/hygv35/fov20_mag8_mcp40_2023.0.h5'
             >>> fp_radecs,stars_xy,stars_invariants,stars_asterisms = read_h5_indices(infile_h5)
         
         Inputs:
             infile_h5 -> [str] h5-formatted star catalog file  
 
         Outputs:
             fp_radecs -> [2d array of float] The center pointing of each sky area in format of [[RA0,DEC0],..[RAn,DECn]] in [deg]
@@ -138,15 +138,15 @@
     Class StarCatalogRaw
 
     Attributes:
         - tiles_path: Path of the starcatalog tile files. 
         - sc_size: The size of the star catalog.
         - tiles_num: Total number of the tile files.
         - validity: The validity of the star catalog.
-        - sc_name: Name of the starcatalog. Available starcatalogs include 'hygv3', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
+        - sc_name: Name of the starcatalog. Available starcatalogs include 'hygv35', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
         - tile_size: Size of the tile in [deg]
         - _mode: Types of star catalogs, including 'raw', 'reduced', 'simplified', where
             'raw' represents the original star catalog, which contains all information about the star
             'reduced' represents the reduced star catalog, which contains the position, proper motion, apparent magnitude, epoch of the star
             'simplified' represents the minimalist star catalog, which only includes the position and apparent magnitude of stars
         - stars_num: Total number of stars in the catalog
         - mag: Apparent magnitude of stars in the catalog
@@ -177,15 +177,15 @@
         Usage:
             >>> from starcatalogquery import StarCatalogRaw
             >>> # load the raw star catalog GAIADR3
             >>> dir_from_raw = '/Volumes/TOSHIBA/starcatalog/raw/gaiadr3/res2/'
             >>> gaiadr3_raw = StarCatalogRaw.load('raw','gaiadr3',2,dir_from_raw)
 
         Inputs:
-            sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv3', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
+            sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv35', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
             tile_size -> [int] Size of the tile in [deg]
             dir_from -> [str,optional,default=None] The loading path of the star catalog files. If None, the path is automatically assigned to a suitable directory by default.
 
         Outputs:
             Instance of class StarCatalogRaw
         """
         if dir_from is None: dir_from = 'starcatalogs/raw/{:s}/res{:d}/'.format(sc_name,tile_size)    
@@ -224,15 +224,15 @@
             dir_reduced = tiles_path.replace('raw','reduced')
         Path(dir_reduced).mkdir(parents=True, exist_ok=True)    
 
         file_list = glob(tiles_path+'*') 
         sc_name = self.sc_name
         print('Reducing the star catalog {:s}, which may take a considerable amount of time'.format(sc_name))  
 
-        if sc_name == 'hygv3':
+        if sc_name == 'hygv35':
             j = 1
             for tile_file in file_list:
                 desc = 'Reducing {:s}{:d}{:s} of {:d}'.format(Fore.BLUE,j,Fore.RESET,self.tiles_num)
                 print(desc,end='\r')
 
                 df = pd.read_csv(tile_file,skiprows=1,dtype=str)
                 # units: ra->hourangle, dec->deg, pmra->mas/a, pmdec->mas/a, epoch->2000.0 
@@ -356,15 +356,15 @@
         ra_min,dec_min,ra_max,dec_max = radec_box
         tile_size = int(self.tile_size.split()[0])
         sc_path,sc_name = self.tiles_path,self.sc_name
         sc_indices = box2seqs(radec_box,tile_size) 
 
         df = pd.concat(_load_files(sc_indices,sc_path,sc_name,self._mode))
 
-        if sc_name == 'hygv3':
+        if sc_name == 'hygv35':
             df['ra'] = (df['ra'].astype(float)*15).round(6) # Convert hourangle to deg
             df['epoch'] = 2000.0
         elif sc_name == 'gsc12':
             columns_dict = {'RApm':'pmra', 'Decpm':'pmdec', 'Epoch':'epoch'}
             df.rename(columns=columns_dict, inplace=True)
             # Convert to standard proper motion in mas/a
             df['pmra'] = (df['pmra'].astype(float)*1e4).round(2) 
@@ -439,15 +439,15 @@
         ra_c,dec_c = center
         tile_size = int(self.tile_size.split()[0])
         sc_path,sc_name = self.tiles_path,self.sc_name
         sc_indices = cone2seqs(ra_c,dec_c,radius,tile_size) 
 
         df = pd.concat(_load_files(sc_indices,sc_path,sc_name,self._mode))
 
-        if sc_name == 'hygv3':
+        if sc_name == 'hygv35':
             df['ra'] = (df['ra'].astype(float)*15).round(6) # Convert hourangle to deg
             df['epoch'] = 2000.0
         elif sc_name == 'gsc12':
             columns_dict = {'RApm':'pmra', 'Decpm':'pmdec', 'Epoch':'epoch'}
             df.rename(columns=columns_dict, inplace=True)
             # Convert to standard proper motion in mas/a
             df['pmra'] = (df['pmra'].astype(float)*1e4).round(2) 
@@ -532,15 +532,15 @@
     Class StarCatalogReduced
 
     Attributes:
         - tiles_path: Path of the starcatalog tile files. 
         - sc_size: The size of the star catalog.
         - tiles_num: Total number of the tile files.
         - validity: The validity of the star catalog.
-        - sc_name: Name of the starcatalog. Available starcatalogs include 'hygv3', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
+        - sc_name: Name of the starcatalog. Available starcatalogs include 'hygv35', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
         - tile_size: Size of the tile in [deg]
         - _mode: Types of star catalogs, including 'raw', 'reduced', 'simplified', where
             'raw' represents the original star catalog, which contains all information about the star
             'reduced' represents the reduced star catalog, which contains the position, proper motion, apparent magnitude, epoch of the star
             'simplified' represents the minimalist star catalog, which only includes the position and apparent magnitude of stars
         - stars_num: Total number of stars in the catalog
         - mag: Apparent magnitude of stars in the catalog
@@ -571,15 +571,15 @@
         Usage:
             >>> from starcatalogquery import StarCatalogReduced
             >>> # load the reduced star catalog GAIADR3
             >>> dir_from_reduced = '/Volumes/TOSHIBA/starcatalog/reduced/gaiadr3/res2/'
             >>> gaiadr3_reduced = StarCatalogReduced.load('reduced','gaiadr3',2,dir_from_reduced)
 
         Inputs:
-            sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv3', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
+            sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv35', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
             tile_size -> [int] Size of the tile in [deg]
             dir_from -> [str,optional,default=None] The loading path of the star catalog files. If None, the path is automatically assigned to a suitable directory by default.
 
         Outputs:
             Instance of class StarCatalogReduced
         """
         if dir_from is None: dir_from = 'starcatalogs/reduced/{:s}/res{:d}/'.format(sc_name,tile_size)    
@@ -600,15 +600,15 @@
         Simplify the reduced star catalog so that the simplified star catalog only contains key information: the position and apparent magnitude of stars.
 
         Usage:
             >>> from starcatalogquery import StarCatalogReduced
             >>> # load the reduced star catalog GAIADR3
             >>> dir_from_reduced = '/Volumes/TOSHIBA/starcatalog/reduced/gaiadr3/res2/'
             >>> gaiadr3_reduced = StarCatalogReduced.load('reduced','gaiadr3',2,dir_from_reduced)
-            >>> gaiadr3_simplified = gaiadr3_reduced.simplify()
+            >>> gaiadr3_simplified = gaiadr3_reduced.simplify(9.0,2022.0)
 
         Inputs:
             mag_threshold -> [float] Apparent magnitude limit of the detector  
             t_pm -> [float] The epoch when the search was performed
             dir_simplified -> [str,optional,default=None] The path of the simplified star catalog files to store. If None, the path is automatically assigned to a suitable directory by default.
 
         Outputs:
@@ -759,15 +759,15 @@
     Class StarCatalogSimplified
 
     Attributes:
         - tiles_path: Path of the starcatalog tile files. 
         - sc_size: The size of the star catalog.
         - tiles_num: Total number of the tile files.
         - validity: The validity of the star catalog.
-        - sc_name: Name of the starcatalog. Available starcatalogs include 'hygv3', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
+        - sc_name: Name of the starcatalog. Available starcatalogs include 'hygv35', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
         - tile_size: Size of the tile in [deg]
         - _mode: Types of star catalogs, including 'raw', 'reduced', 'simplified', where
             'raw' represents the original star catalog, which contains all information about the star
             'reduced' represents the reduced star catalog, which contains the position, proper motion, apparent magnitude, epoch of the star
             'simplified' represents the minimalist star catalog, which only includes the position and apparent magnitude of stars
         - stars_num: Total number of stars in the catalog
         - mag: Apparent magnitude of stars in the catalog
@@ -798,15 +798,15 @@
         Usage:
             >>> from starcatalogquery import StarCatalogSimplified
             >>> # load the simplified star catalog GAIADR3
             >>> dir_from_simplified = '/Volumes/TOSHIBA/starcatalog/simplified/gaiadr3/res2/'
             >>> gaiadr3_simplified = StarCatalogSimplified.load('simplified','gaiadr3',2,dir_from_simplified)
 
         Inputs:
-            sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv3', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
+            sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv35', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
             tile_size -> [int] Size of the tile in [deg]
             mag_cutoff -> [float] The truncated magnitude of the simplified star catalog
             epoch -> [float] The epoch of the simplified star catalog
             dir_from -> [str,optional,default=None] The loading path of the star catalog files. If None, the path is automatically assigned to a suitable directory by default.
 
         Outputs:
             Instance of class StarCatalogSimplified
```

## starcatalogquery/tiles_draw.py

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import cartopy.crs as ccrs
 from matplotlib.patches import Rectangle
-from pyshtools.utils import MakeCircleCoord
+from astropy.visualization.wcsaxes import SphericalCircle
+from astropy import units as u
 
 from .catalog_query import cone2seqs,box2seqs,seq2radec  
 
 def search_draw(tile_size,kwargs):
     """
     Visualize the scope of the search area and the coverage of the corresponding tiles.
 
@@ -46,15 +47,14 @@
 
 def plot_circle_PlateCarree(radec_boxes,ra_c,dec_c,r):
     """
     Plot the scope of the cap search area and the coverage of the corresponding tiles.         
     """
     region = left_ra, right_ra, lower_dec, upper_dec = ra_c-1.5*r, ra_c+1.5*r, dec_c-1.5*r, dec_c+1.5*r 
     ra_span = dec_span = 3*r
-    circle = MakeCircleCoord(dec_c,ra_c,r)
         
     # set the map projection
     proj = ccrs.PlateCarree(central_longitude=ra_c)
    
     # plot
     plt.clf()
     fig = plt.figure(dpi=300)
@@ -68,15 +68,16 @@
     if right_ra > 180:
         block_flags = xlocs > 180
         xlocs[block_flags] -= 360
 
     gl = ax.gridlines(xlocs = xlocs, ylocs = ylocs,draw_labels=True,linestyle='--',alpha=0.7)
     gl.xlabel_style = {'size': 7, 'color': 'gray'}
     gl.ylabel_style = {'size': 7, 'color': 'gray'}
-    ax.plot(circle[:,1], circle[:,0], color='m',lw=1.5,transform=ccrs.Geodetic())
+    circle = SphericalCircle((ra_c*u.deg, dec_c*u.deg), r*u.deg,fc='none',ec='m',lw=1.5,transform=ccrs.Geodetic())
+    ax.add_patch(circle)
     
     for radec_box in radec_boxes:
         ra_min,dec_min,ra_max,dec_max = radec_box
         width = ra_max - ra_min
         height = dec_max - dec_min
     
         ax.add_patch(Rectangle((ra_min,dec_min),width, height, ec ='g',lw = 1,transform=ccrs.PlateCarree(),alpha=0.3))
```

## starcatalogquery/utils/starcatalog_statistic.py

```diff
@@ -41,22 +41,22 @@
     """
     Given a star catalog name, get basic information about the catalog.
 
     Usage:
         >>> star_num,mag,description = starcatalog_info('2mass')
 
     Inputs:
-        sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv3', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
+        sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv35', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
 
     Outputs:
         star_num -> [str] The total number of stars contained in the catalog
         mag -> [str] The magnitude range of the star catalog
         description -> [str] A brief description of the catalog      
     """
-    if sc_name == 'hygv3':
+    if sc_name == 'hygv35':
         star_num = '~ 0.12 Million'
         mag = '< 9'    
         description = 'The database is a subset of the data in three major catalogs: the Hipparcos Catalog,the Yale Bright Star Catalog (5th Edition), and the Gliese Catalog of Nearby Stars (3rd Edition).'
     elif sc_name == 'gsc12':
         star_num = '~ 19 Million'
         mag = '6 ~ 15' 
         description = 'The GSC(Guide Star Catalog) I is primarily based on an all-sky, single-epoch collection of Schmidt plates.'
```

## Comparing `starcatalogquery-0.1.7.dist-info/LICENSE` & `starcatalogquery-0.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `starcatalogquery-0.1.7.dist-info/METADATA` & `starcatalogquery-0.1.8.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starcatalogquery
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package to establish an offline star catalog query database
 Home-page: https://github.com/lcx366/STARQUERY
 Author: Chunxiao Li
 Author-email: lcx366@126.com
 License: MIT
 Keywords: StarCatalog
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
-Requires-Dist: pyshtools
 Requires-Dist: astropy (>=4.3.1)
 Requires-Dist: pandas
 Requires-Dist: h5py
 Requires-Dist: colorama
 Requires-Dist: healpy
 Requires-Dist: cartopy
 Requires-Dist: wget
@@ -52,30 +51,30 @@
 ```
 
 ## How to use
 
 ### Build an offline star catalog database
 
 Get the star catalog data from the remote server ([MIKULSKI ARCHIVE&
-SPACE TELESCOPES](https://archive.stsci.edu)) , and build an offline star catalog database locally. Currently, available star catalogs include 'hygv3', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
+SPACE TELESCOPES](https://archive.stsci.edu)) , and build an offline star catalog database locally. Currently, available star catalogs include 'hygv35', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
 
 ```python
 >>> from starcatalogquery import StarCatalog
 >>> # Get the star catalog GAIADR3 with the tile size of 2 deg
 >>> gaiadr3_raw = StarCatalog.get('gaiadr3',2)
 ```
 
 We get an instance of class StarCatalogRaw with
 
     Attributes:
         - tiles_path: Path of the starcatalog tile files. 
         - sc_size: The size of the star catalog.
         - tiles_num: Total number of the tile files.
         - validity: The validity of the star catalog.
-        - sc_name: Name of the starcatalog. Available starcatalogs include 'hygv3', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
+        - sc_name: Name of the starcatalog. Available starcatalogs include 'hygv35', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
         - tile_size: Size of the tile in [deg]
         - _mode: Types of star catalogs, including 'raw', 'reduced', 'simplified', where
             'raw' represents the original star catalog, which contains all information about the star
             'reduced' represents the reduced star catalog, which contains the position, proper motion, apparent magnitude, epoch of the star
             'simplified' represents the minimalist star catalog, which only includes the position and apparent magnitude of stars
         - stars_num: Total number of stars in the catalog
         - mag: Apparent magnitude of stars in the catalog
@@ -98,15 +97,16 @@
 The reduced star catalog only contains the celestial position, proper motion, apparent magnitude, and epoch of stars.
 
 ### Simplify the reduced star catalogs
 
 In order to further reduce the size of the star catalog and improve its query efficiency, we filter out the reduced star catalog according to the limit magnitude of the detector, and make proper motion corrections to obtain a minimalist star catalog.
 
 ```python
->>> gaiadr3_simplified = gaiadr3_reduced.simplify()
+>>> mag_threshold, t_pm = 9.0,2022.0 
+>>> gaiadr3_simplified = gaiadr3_reduced.simplify(mag_threshold,t_pm)
 ```
 
 The simplified(minimalist) star catalog only includes the celetial position and apparent magnitude of stars at a specific epoch.
 
 ### Query information about stars in a specific sky area
 
 Perform a cone search of stars on the raw or reduced star catalog.
@@ -219,43 +219,49 @@
 
 A h5-formatted star catalog file `outh5`is generated, which records the center pointing of each sky area, the pixel coordinates, the triangle invariants and the asterism indices of the stars.
 
 ### Read in h5-formatted star catalog file
 
 ```python
 >>> from starcatalogquery import StarCatalog
->>> infile_h5 = 'starcatalogs/indices/hygv3/fov20_mag8_mcp40_2023.0.h5'
+>>> infile_h5 = 'starcatalogs/indices/hygv35/fov20_mag8_mcp40_2023.0.h5'
 >>> fp_radecs,stars_xy,stars_invariants,stars_asterisms = StarCatalog.read_h5_indices(infile_h5)
 ```
 
 ### Load the local offline star catalog database
 
 #### Load the raw or reduced star catalog
 
 ```python
 >>> from starcatalogquery import StarCatalog
->>> dir_from_raw = '/Volumes/TOSHIBA/starcatalogs/raw/hygv3/res2/' # Path of the raw starcatalog
->>> hygv3_raw = StarCatalog.load(dir_from_raw)
->>> # dir_from_reduced = '/Volumes/TOSHIBA/starcatalogs/reduced/hygv3/res2/' # Path of the reduced starcatalog
->>> # hygv3_reduced = StarCatalog.load(dir_from_reduced)
+>>> dir_from_raw = '/Volumes/TOSHIBA/starcatalogs/raw/hygv35/res2/' # Path of the raw starcatalog
+>>> hygv35_raw = StarCatalog.load(dir_from_raw)
+>>> # dir_from_reduced = '/Volumes/TOSHIBA/starcatalogs/reduced/hygv35/res2/' # Path of the reduced starcatalog
+>>> # hygv35_reduced = StarCatalog.load(dir_from_reduced)
 ```
 
 #### Load the simplified star catalog
 
 ```python
 >>> from starcatalogquery import StarCatalog
->>> dir_from_simplified = '/Volumes/TOSHIBA/starcatalogs/raw/hygv3/res5/mag8.0/epoch2023.0/' # Path of the starcatalog
->>> hygv3_raw = StarCatalog.load(dir_from_simplified)
+>>> dir_from_simplified = '/Volumes/TOSHIBA/starcatalogs/simplified/hygv35/res5/mag8.0/epoch2023.0/' # Path of the starcatalog
+>>> hygv35_simplified = StarCatalog.load(dir_from_simplified)
 ```
 
 ## Change log
 
+- **0.1.8 — Jul 03, 2023**
+  
+  - Get rid of dependency on **pyshtools**
+    - Added function `from_cap` to replace `pysh.SHGrid.from_cap` in *catalog_query.py*
+    - Using `SphericalCircle` in *astropy* to replace `MakeCircleCoord` in *pyshtools.utils* 
+
 - **0.1.7 — Jun 16, 2023**
   
-  - Simplified the loading of star catalogs by `StarCatalog.load` .
+  - Simplified parameter input of `StarCatalog.load` for star catalog loading.
 
 - **0.1.5 — May 13, 2023**
   
   - Add method `.invariantfeatures()` to class `Stars`, which calculates the triangle invariants and constructs a 2D Tree; and records the asterism indices for each triangle.
 
 - **0.1.0 — May 10,  2023**
```

## Comparing `starcatalogquery-0.1.7.dist-info/RECORD` & `starcatalogquery-0.1.8.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 starcatalogquery/__init__.py,sha256=F5XhiD_gjaRsVVK_KfSD9ZkmgQnoNiJQqIMoMsceHRY,33
-starcatalogquery/catalog_check.py,sha256=r6B-MtO3bq3NVRHkyq0xnZxBvTRf8Epmn-thBD53gHo,6048
-starcatalogquery/catalog_download.py,sha256=gDFjQEtwKX56Sdwv7L53YIZKLrLy_3CtbvE3tfyxrvQ,6716
-starcatalogquery/catalog_query.py,sha256=kBY8F25jt_WiLLY_SNJWseHCx0XWVti-b7ToL17csV4,15124
-starcatalogquery/classes.py,sha256=B7olOsvZkxDhWpQjheXhZjsjlI5e-1Sr5R83Deono58,51243
+starcatalogquery/catalog_check.py,sha256=GIjZgERg7Q6qhwyfzHOxut95KjmJGwq-M0SJVUFMLY8,6049
+starcatalogquery/catalog_download.py,sha256=sy316_xRn5CBVsqQAYmXSOSXx5bvBaU9Ewmwxt24vOM,6727
+starcatalogquery/catalog_query.py,sha256=HOilEP_Xyxo9BRDW06gFfu1YgyIO60FZinOBy1bIfDg,16654
+starcatalogquery/classes.py,sha256=ZL5ImjCW2p8Xo05gHXHgqNMJjdzs9iZt7Z4llf1K57s,51269
 starcatalogquery/invariantfeatures.py,sha256=iJG2K3R4BcbAqkX0I-P0nQYR4Xeo2UpPaQuEqx4CP58,3078
-starcatalogquery/tiles_draw.py,sha256=zsL2lOnfOrb-fWXDSSmdGwdfYWNIL08D84Kvk8Lvc0E,5624
+starcatalogquery/tiles_draw.py,sha256=GGFtw8GNY67eTS-RzOG_RH-amS0wjlm8Dx844LblYXI,5684
 starcatalogquery/wcs.py,sha256=gtHOyg7Y51Icc3uAfA_uX3YznXqYbhtSKwVDcO1gIcg,1978
 starcatalogquery/utils/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 starcatalogquery/utils/df2info.py,sha256=_eQENb_DxX5Q5EGxbanJuo9nQKBm-A6Tz8pEsLFinxI,612
-starcatalogquery/utils/starcatalog_statistic.py,sha256=xnyKAJFuduuXo3dKkO0B1YoeTlvu-j-BtNtgrRMvZIY,4272
+starcatalogquery/utils/starcatalog_statistic.py,sha256=LSjhB0jEsxzZmkXcB7NoVDXOorWB71DAPYg1HWWUREQ,4274
 starcatalogquery/utils/try_download.py,sha256=cTfNaevU_ELwKP3R9SpYQsiGtEvoBETnsi__EdkLSVE,477
-starcatalogquery-0.1.7.dist-info/LICENSE,sha256=1mo8gGwn9nEfzoruoWYAD1ttN40DofMYGQNef1rsytY,1068
-starcatalogquery-0.1.7.dist-info/METADATA,sha256=jcgH9FSfcKRF45k6nA9w8cij4gLlgtdFRXRs7qEHlgA,12259
-starcatalogquery-0.1.7.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-starcatalogquery-0.1.7.dist-info/top_level.txt,sha256=xZmWsZTK993L9eaiWI9PM0exXZiKw-64leh_79J2M9U,17
-starcatalogquery-0.1.7.dist-info/RECORD,,
+starcatalogquery-0.1.8.dist-info/LICENSE,sha256=1mo8gGwn9nEfzoruoWYAD1ttN40DofMYGQNef1rsytY,1068
+starcatalogquery-0.1.8.dist-info/METADATA,sha256=JdBIPuVw2qAhdBr2tYdwf2_wo1NseYgqZ4lAmk6OC9k,12582
+starcatalogquery-0.1.8.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+starcatalogquery-0.1.8.dist-info/top_level.txt,sha256=xZmWsZTK993L9eaiWI9PM0exXZiKw-64leh_79J2M9U,17
+starcatalogquery-0.1.8.dist-info/RECORD,,
```

