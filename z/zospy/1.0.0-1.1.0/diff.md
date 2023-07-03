# Comparing `tmp/zospy-1.0.0.tar.gz` & `tmp/zospy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zospy-1.0.0.tar", last modified: Fri May  5 14:30:15 2023, max compression
+gzip compressed data, was "zospy-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `zospy-1.0.0.tar` & `zospy-1.1.0.tar`

### file list

```diff
@@ -1,105 +1,107 @@
--rw-r--r--   0        0        0    35149 2023-05-05 14:30:02.620558 zospy-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     6956 2023-05-05 14:30:02.620558 zospy-1.0.0/README.md
--rw-r--r--   0        0        0     1940 2023-05-05 14:30:02.856561 zospy-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      430 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/__init__.py
--rw-r--r--   0        0        0      265 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/analyses/__init__.py
--rw-r--r--   0        0        0    19416 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/analyses/base.py
--rw-r--r--   0        0        0     7810 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/analyses/mtf.py
--rw-r--r--   0        0        0     5771 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/analyses/psf.py
--rwxr-xr-x   0        0        0    12892 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/analyses/raysandspots.py
--rw-r--r--   0        0        0    34758 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/analyses/reports.py
--rw-r--r--   0        0        0     7204 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/analyses/surface.py
--rw-r--r--   0        0        0     8770 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/analyses/wavefront.py
--rw-r--r--   0        0        0       88 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI.py
--rw-r--r--   0        0        0    17150 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Data/__init__.pyi
--rw-r--r--   0        0        0     7459 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/PhysicalOptics/__init__.pyi
--rw-r--r--   0        0        0     1500 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/RayTracing/__init__.pyi
--rw-r--r--   0        0        0    13181 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Aberrations/__init__.pyi
--rw-r--r--   0        0        0     7370 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/DiffractionEfficiency/__init__.pyi
--rw-r--r--   0        0        0     6951 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/EncircledEnergy/__init__.pyi
--rw-r--r--   0        0        0     8224 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/ExtendedScene/__init__.pyi
--rw-r--r--   0        0        0     1710 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Fans/__init__.pyi
--rw-r--r--   0        0        0     3185 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Materials/__init__.pyi
--rw-r--r--   0        0        0    20338 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Mtf/__init__.pyi
--rw-r--r--   0        0        0     3248 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/NSCSurface/__init__.pyi
--rw-r--r--   0        0        0     6857 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Psf/__init__.pyi
--rw-r--r--   0        0        0      289 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/RMS/RMSField/__init__.pyi
--rw-r--r--   0        0        0      309 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/RMS/RMSFieldMap/__init__.pyi
--rw-r--r--   0        0        0     9314 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/RMS/__init__.pyi
--rw-r--r--   0        0        0     6028 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/RayTracing/__init__.pyi
--rw-r--r--   0        0        0     2847 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Spot/__init__.pyi
--rw-r--r--   0        0        0    10174 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Surface/__init__.pyi
--rw-r--r--   0        0        0     2748 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Wavefront/__init__.pyi
--rw-r--r--   0        0        0    12350 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/__init__.pyi
--rw-r--r--   0        0        0     1276 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Tolerancing/QuickYield/__init__.pyi
--rw-r--r--   0        0        0     3789 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Tolerancing/__init__.pyi
--rw-r--r--   0        0        0    29718 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/__init__.pyi
--rw-r--r--   0        0        0     7010 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Common/__init__.pyi
--rw-r--r--   0        0        0   221316 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Editors/LDE/__init__.pyi
--rw-r--r--   0        0        0     4886 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Editors/MCE/__init__.pyi
--rw-r--r--   0        0        0    10272 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Editors/MFE/__init__.pyi
--rw-r--r--   0        0        0   321725 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/Editors/NCE/__init__.pyi
--rw-r--r--   0        0        0     5024 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/Editors/TDE/__init__.pyi
--rw-r--r--   0        0        0    15871 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/Editors/__init__.pyi
--rw-r--r--   0        0        0     4438 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/Preferences/__init__.pyi
--rw-r--r--   0        0        0    21244 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/SystemData/__init__.pyi
--rw-r--r--   0        0        0    19510 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/Tools/General/__init__.pyi
--rw-r--r--   0        0        0    22251 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/Tools/LMx/__init__.pyi
--rw-r--r--   0        0        0     5075 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/Tools/Optimization/__init__.pyi
--rw-r--r--   0        0        0    16386 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/Tools/RayTrace/__init__.pyi
--rw-r--r--   0        0        0    18928 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/Tools/Tolerancing/__init__.pyi
--rw-r--r--   0        0        0    16271 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/Tools/__init__.pyi
--rw-r--r--   0        0        0    26695 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/Wizards/__init__.pyi
--rw-r--r--   0        0        0    12760 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/py.typed
--rw-r--r--   0        0        0       93 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants.py
--rw-r--r--   0        0        0     1477 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/PhysicalOptics/__init__.pyi
--rw-r--r--   0        0        0      358 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/RayTracing/__init__.pyi
--rw-r--r--   0        0        0     1325 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Aberrations/__init__.pyi
--rw-r--r--   0        0        0      655 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/EncircledEnergy/__init__.pyi
--rw-r--r--   0        0        0      613 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/ExtendedScene/__init__.pyi
--rw-r--r--   0        0        0      395 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Fans/__init__.pyi
--rw-r--r--   0        0        0      768 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Mtf/__init__.pyi
--rw-r--r--   0        0        0      517 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/NSCSurface/__init__.pyi
--rw-r--r--   0        0        0      626 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Psf/__init__.pyi
--rw-r--r--   0        0        0      282 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/RMS/RMSField/__init__.pyi
--rw-r--r--   0        0        0      302 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/RMS/RMSFieldMap/__init__.pyi
--rw-r--r--   0        0        0     2589 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/RMS/__init__.pyi
--rw-r--r--   0        0        0      548 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Spot/__init__.pyi
--rw-r--r--   0        0        0      744 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Wavefront/__init__.pyi
--rw-r--r--   0        0        0     1982 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/__init__.pyi
--rw-r--r--   0        0        0      637 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Tolerancing/QuickYield/__init__.pyi
--rw-r--r--   0        0        0      560 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Tolerancing/__init__.pyi
--rw-r--r--   0        0        0    11188 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/__init__.pyi
--rw-r--r--   0        0        0      937 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Common/__init__.pyi
--rw-r--r--   0        0        0     9011 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Editors/LDE/__init__.pyi
--rw-r--r--   0        0        0     1792 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Editors/MCE/__init__.pyi
--rw-r--r--   0        0        0     6853 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Editors/MFE/__init__.pyi
--rw-r--r--   0        0        0    11143 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Editors/NCE/__init__.pyi
--rw-r--r--   0        0        0     1158 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Editors/TDE/__init__.pyi
--rw-r--r--   0        0        0     1854 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Editors/__init__.pyi
--rw-r--r--   0        0        0      522 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Preferences/__init__.pyi
--rw-r--r--   0        0        0     3392 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/SystemData/__init__.pyi
--rw-r--r--   0        0        0     2561 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Tools/General/__init__.pyi
--rw-r--r--   0        0        0      254 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Tools/LMx/__init__.pyi
--rw-r--r--   0        0        0      680 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Tools/Optimization/__init__.pyi
--rw-r--r--   0        0        0     1330 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Tools/RayTrace/__init__.pyi
--rw-r--r--   0        0        0     3821 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Tools/Tolerancing/__init__.pyi
--rw-r--r--   0        0        0     1742 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Tools/__init__.pyi
--rw-r--r--   0        0        0     1224 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Wizards/__init__.pyi
--rw-r--r--   0        0        0     1461 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/py.typed
--rw-r--r--   0        0        0        0 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/__init__.py
--rw-r--r--   0        0        0     5642 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/apisupport.py
--rw-r--r--   0        0        0      254 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/config.py
--rw-r--r--   0        0        0     3996 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/constants.py
--rw-r--r--   0        0        0       49 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/functions/__init__.py
--rw-r--r--   0        0        0     1997 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/functions/lde.py
--rw-r--r--   0        0        0     1169 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/functions/nce.py
--rw-r--r--   0        0        0     6119 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/solvers/__init__.py
--rw-r--r--   0        0        0       97 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/utils/__init__.py
--rw-r--r--   0        0        0     3689 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/utils/clrutils.py
--rw-r--r--   0        0        0     1338 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/utils/pyutils.py
--rw-r--r--   0        0        0     4471 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/utils/zputils.py
--rw-r--r--   0        0        0    14957 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/zpcore.py
--rw-r--r--   0        0        0     7998 1970-01-01 00:00:00.000000 zospy-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-03 15:08:14.477806 zospy-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     7109 2023-07-03 15:08:14.485806 zospy-1.1.0/README.md
+-rw-r--r--   0        0        0     1914 2023-07-03 15:08:14.721811 zospy-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      430 2023-07-03 15:08:14.737811 zospy-1.1.0/zospy/__init__.py
+-rw-r--r--   0        0        0      407 2023-07-03 15:08:14.737811 zospy-1.1.0/zospy/analyses/__init__.py
+-rw-r--r--   0        0        0    19416 2023-07-03 15:08:14.737811 zospy-1.1.0/zospy/analyses/base.py
+-rw-r--r--   0        0        0     9108 2023-07-03 15:08:14.737811 zospy-1.1.0/zospy/analyses/mtf.py
+-rw-r--r--   0        0        0    16774 2023-07-03 15:08:14.737811 zospy-1.1.0/zospy/analyses/polarization.py
+-rw-r--r--   0        0        0     5771 2023-07-03 15:08:14.737811 zospy-1.1.0/zospy/analyses/psf.py
+-rwxr-xr-x   0        0        0    12898 2023-07-03 15:08:14.737811 zospy-1.1.0/zospy/analyses/raysandspots.py
+-rw-r--r--   0        0        0    34758 2023-07-03 15:08:14.737811 zospy-1.1.0/zospy/analyses/reports.py
+-rw-r--r--   0        0        0     7204 2023-07-03 15:08:14.737811 zospy-1.1.0/zospy/analyses/surface.py
+-rw-r--r--   0        0        0     9093 2023-07-03 15:08:14.737811 zospy-1.1.0/zospy/analyses/systemviewers.py
+-rw-r--r--   0        0        0     8770 2023-07-03 15:08:14.737811 zospy-1.1.0/zospy/analyses/wavefront.py
+-rw-r--r--   0        0        0       88 2023-07-03 15:08:14.737811 zospy-1.1.0/zospy/api/_ZOSAPI.py
+-rw-r--r--   0        0        0    17150 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Data/__init__.pyi
+-rw-r--r--   0        0        0     7459 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/PhysicalOptics/__init__.pyi
+-rw-r--r--   0        0        0     1500 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/RayTracing/__init__.pyi
+-rw-r--r--   0        0        0    13181 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/Aberrations/__init__.pyi
+-rw-r--r--   0        0        0     7370 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/DiffractionEfficiency/__init__.pyi
+-rw-r--r--   0        0        0     6951 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/EncircledEnergy/__init__.pyi
+-rw-r--r--   0        0        0     8224 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/ExtendedScene/__init__.pyi
+-rw-r--r--   0        0        0     1710 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/Fans/__init__.pyi
+-rw-r--r--   0        0        0     3185 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/Materials/__init__.pyi
+-rw-r--r--   0        0        0    20338 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/Mtf/__init__.pyi
+-rw-r--r--   0        0        0     3248 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/NSCSurface/__init__.pyi
+-rw-r--r--   0        0        0     6857 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/Psf/__init__.pyi
+-rw-r--r--   0        0        0      289 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/RMS/RMSField/__init__.pyi
+-rw-r--r--   0        0        0      309 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/RMS/RMSFieldMap/__init__.pyi
+-rw-r--r--   0        0        0     9314 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/RMS/__init__.pyi
+-rw-r--r--   0        0        0     6028 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/RayTracing/__init__.pyi
+-rw-r--r--   0        0        0     2847 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/Spot/__init__.pyi
+-rw-r--r--   0        0        0    10174 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/Surface/__init__.pyi
+-rw-r--r--   0        0        0     2748 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/Wavefront/__init__.pyi
+-rw-r--r--   0        0        0    12350 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/__init__.pyi
+-rw-r--r--   0        0        0     1276 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Tolerancing/QuickYield/__init__.pyi
+-rw-r--r--   0        0        0     3789 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Tolerancing/__init__.pyi
+-rw-r--r--   0        0        0    29718 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/__init__.pyi
+-rw-r--r--   0        0        0     7010 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Common/__init__.pyi
+-rw-r--r--   0        0        0   221316 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Editors/LDE/__init__.pyi
+-rw-r--r--   0        0        0     4886 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Editors/MCE/__init__.pyi
+-rw-r--r--   0        0        0    10272 2023-07-03 15:08:14.741812 zospy-1.1.0/zospy/api/_ZOSAPI/Editors/MFE/__init__.pyi
+-rw-r--r--   0        0        0   321725 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI/Editors/NCE/__init__.pyi
+-rw-r--r--   0        0        0     5024 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI/Editors/TDE/__init__.pyi
+-rw-r--r--   0        0        0    15871 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI/Editors/__init__.pyi
+-rw-r--r--   0        0        0     4438 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI/Preferences/__init__.pyi
+-rw-r--r--   0        0        0    21244 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI/SystemData/__init__.pyi
+-rw-r--r--   0        0        0    19510 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI/Tools/General/__init__.pyi
+-rw-r--r--   0        0        0    22251 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI/Tools/LMx/__init__.pyi
+-rw-r--r--   0        0        0     5075 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI/Tools/Optimization/__init__.pyi
+-rw-r--r--   0        0        0    16386 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI/Tools/RayTrace/__init__.pyi
+-rw-r--r--   0        0        0    18928 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI/Tools/Tolerancing/__init__.pyi
+-rw-r--r--   0        0        0    16271 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI/Tools/__init__.pyi
+-rw-r--r--   0        0        0    26695 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI/Wizards/__init__.pyi
+-rw-r--r--   0        0        0    12760 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI/py.typed
+-rw-r--r--   0        0        0       93 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants.py
+-rw-r--r--   0        0        0     1477 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/PhysicalOptics/__init__.pyi
+-rw-r--r--   0        0        0      358 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/RayTracing/__init__.pyi
+-rw-r--r--   0        0        0     1325 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Aberrations/__init__.pyi
+-rw-r--r--   0        0        0      655 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/EncircledEnergy/__init__.pyi
+-rw-r--r--   0        0        0      613 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/ExtendedScene/__init__.pyi
+-rw-r--r--   0        0        0      395 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Fans/__init__.pyi
+-rw-r--r--   0        0        0      768 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Mtf/__init__.pyi
+-rw-r--r--   0        0        0      517 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/NSCSurface/__init__.pyi
+-rw-r--r--   0        0        0      626 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Psf/__init__.pyi
+-rw-r--r--   0        0        0      282 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/RMS/RMSField/__init__.pyi
+-rw-r--r--   0        0        0      302 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/RMS/RMSFieldMap/__init__.pyi
+-rw-r--r--   0        0        0     2589 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/RMS/__init__.pyi
+-rw-r--r--   0        0        0      548 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Spot/__init__.pyi
+-rw-r--r--   0        0        0      744 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Wavefront/__init__.pyi
+-rw-r--r--   0        0        0     1982 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/__init__.pyi
+-rw-r--r--   0        0        0      637 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Tolerancing/QuickYield/__init__.pyi
+-rw-r--r--   0        0        0      560 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Tolerancing/__init__.pyi
+-rw-r--r--   0        0        0    11188 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/__init__.pyi
+-rw-r--r--   0        0        0      937 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Common/__init__.pyi
+-rw-r--r--   0        0        0     9011 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Editors/LDE/__init__.pyi
+-rw-r--r--   0        0        0     1792 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Editors/MCE/__init__.pyi
+-rw-r--r--   0        0        0     6853 2023-07-03 15:08:14.745812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Editors/MFE/__init__.pyi
+-rw-r--r--   0        0        0    11143 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Editors/NCE/__init__.pyi
+-rw-r--r--   0        0        0     1158 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Editors/TDE/__init__.pyi
+-rw-r--r--   0        0        0     1854 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Editors/__init__.pyi
+-rw-r--r--   0        0        0      522 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Preferences/__init__.pyi
+-rw-r--r--   0        0        0     3392 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/SystemData/__init__.pyi
+-rw-r--r--   0        0        0     2561 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Tools/General/__init__.pyi
+-rw-r--r--   0        0        0      254 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Tools/LMx/__init__.pyi
+-rw-r--r--   0        0        0      680 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Tools/Optimization/__init__.pyi
+-rw-r--r--   0        0        0     1330 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Tools/RayTrace/__init__.pyi
+-rw-r--r--   0        0        0     3821 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Tools/Tolerancing/__init__.pyi
+-rw-r--r--   0        0        0     1742 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Tools/__init__.pyi
+-rw-r--r--   0        0        0     1224 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/Wizards/__init__.pyi
+-rw-r--r--   0        0        0     1461 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/api/_ZOSAPI_constants/py.typed
+-rw-r--r--   0        0        0        0 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/api/__init__.py
+-rw-r--r--   0        0        0     5642 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/api/apisupport.py
+-rw-r--r--   0        0        0      320 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/api/config.py
+-rw-r--r--   0        0        0     3996 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/api/constants.py
+-rw-r--r--   0        0        0       49 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/functions/__init__.py
+-rw-r--r--   0        0        0     4250 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/functions/lde.py
+-rw-r--r--   0        0        0     3588 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/functions/nce.py
+-rw-r--r--   0        0        0     6119 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/solvers/__init__.py
+-rw-r--r--   0        0        0       97 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/utils/__init__.py
+-rw-r--r--   0        0        0     3689 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/utils/clrutils.py
+-rw-r--r--   0        0        0     5140 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/utils/pyutils.py
+-rw-r--r--   0        0        0     4471 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/utils/zputils.py
+-rw-r--r--   0        0        0    15151 2023-07-03 15:08:14.749812 zospy-1.1.0/zospy/zpcore.py
+-rw-r--r--   0        0        0     8182 1970-01-01 00:00:00.000000 zospy-1.1.0/PKG-INFO
```

### Comparing `zospy-1.0.0/LICENSE.txt` & `zospy-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/README.md` & `zospy-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,18 +47,20 @@
 > :warning: Version 1.0.0 introduced some breaking changes. See
 > the [release notes](https://github.com/MREYE-LUMC/ZOSPy/releases/tag/v1.0.0) for more information.
 
 ZOSPy is tested with the following versions of Python and Ansys Zemax OpticStudio:
 
 | Zemax       | 20.3.2 | 23.0.1 |
 |-------------|--------|--------|
-| Python 3.8  | -      | ✔      |
-| Python 3.9  | -      | ✔      |
-| Python 3.10 | -      | ✔      |
-| Python 3.11 | ✔      | ✔      |
+| Python 3.9  | ⚠      | ✔      |
+| Python 3.10 | ⚠      | ✔      |
+| Python 3.11 | ⚠      | ✔      |
+
+✔: This version works without problems.
+⚠: This version works, but the output of analyses can differ slightly from the used reference version (currently **OpticStudio 23 R1.01**).
 
 ## Referencing
 
 When publishing results obtained with this package, please cite the paper in which the package was first used:<br>
 van Vught L, Que I, Luyten GPM and Beenakker JWM.
 _Effect of anatomical differences and intraocular lens design on Negative Dysphotopsia._
 JCRS: Sep 06, 2022.
```

### Comparing `zospy-1.0.0/pyproject.toml` & `zospy-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     "Programming Language :: Python :: 3",
     "Typing :: Typed"
 ]
 requires-python = ">=3.9,<3.12"
 dependencies = [
     "pythonnet ~= 3.0.1",
     "pandas",
-    "numpy"
+    "numpy",
+    "semver ~= 3.0.0"
 ]
 dynamic = ["version"]
 
 [project.urls]
 Source = "https://github.com/MREYE-LUMC/ZOSPy"
 Documentation = "https://mreye-lumc.github.io/ZOSPy"
 
@@ -78,20 +79,18 @@
 # Rule sets for linting
 select = [
     "F",    # pyflakes
     "E",    # pycodestyle error
     "W",    # pycodestyle warning
     "I",    # isort
     "D",    # pydocstyle
-    "TCH",  # flake8 type checking
     "NPY",  # numpy-specific
 ]
 
 ignore = [
-    "TCH001",
     "D100",
     "D101",
     "D102",
     "D103",
     "D104",
     "D105",
     "D401"
```

### Comparing `zospy-1.0.0/zospy/analyses/base.py` & `zospy-1.1.0/zospy/analyses/base.py`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/analyses/mtf.py` & `zospy-1.1.0/zospy/analyses/mtf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,54 @@
 """Zemax OpticStudio analyses from the MTF category."""
 
 from __future__ import annotations
 
+import os
+from tempfile import mkstemp
+
 import pandas as pd
 
 from zospy import utils
 from zospy.analyses.base import AnalysisResult, OnComplete, new_analysis
 from zospy.api import constants
 from zospy.zpcore import OpticStudioSystem
 
 
+def _correct_fft_through_focus_mtftype_api_bug(oss, analysis, mtftype) -> None:
+    """Correction for an API bug in OpticStudio versions < 21.2.
+
+    In these versions, the MTF Type cannot be set through the ZOS-API for the FFT Through Focus MTF
+    See also: https://community.zemax.com/zos-api-12/zos-api-setting-mtf-property-type-not-working-730
+
+    Parameters
+    ----------
+    oss: zospy.core.OpticStudioSystem
+        A ZOSPy OpticStudioSystem instance. Should be sequential.
+    analysis: Analysis
+        An FFT Through Focus MTF analysis.
+    mtftype: zospy.constants.Analysis.Settings.Mtf.MtfTypes.Modulation
+
+    Returns
+    -------
+    None
+    """
+    if oss._ZOS.version < "21.2.0":
+        fd, cfgoutfile = mkstemp(suffix=".CFG", prefix="zospy_")
+        os.close(fd)
+        analysis.Settings.SaveTo(cfgoutfile)
+
+        analysis.Settings.ModifySettings(
+            cfgoutfile,
+            "TFM_TYPE",
+            str(int(constants.process_constant(constants.Analysis.Settings.Mtf.MtfTypes, mtftype))),
+        )
+        analysis.Settings.LoadFrom(cfgoutfile)
+        os.remove(cfgoutfile)
+
+
 def fft_through_focus_mtf(
     oss: OpticStudioSystem,
     sampling: str | int = "64x64",
     deltafocus: float = 0.1,
     frequency: float = 0,
     numberofsteps: int = 5,
     wavelength: str | int = "All",
@@ -73,14 +108,17 @@
     analysis.Settings.NumberOfSteps = numberofsteps
     analysis.set_wavelength(wavelength)
     analysis.set_field(field)
     analysis.Settings.Type = constants.process_constant(constants.Analysis.Settings.Mtf.MtfTypes, mtftype)
     analysis.Settings.UsePolarization = use_polarization
     analysis.Settings.UseDashes = use_dashes
 
+    # Correct an API bug in setting API type for OpticStudio version <21.2
+    _correct_fft_through_focus_mtftype_api_bug(oss, analysis, mtftype)
+
     # Calculate
     analysis.ApplyAndWaitForCompletion()
 
     # Get headerdata, metadata and messages
     headerdata = analysis.get_header_data()
     metadata = analysis.get_metadata()
     messages = analysis.get_messages()
```

### Comparing `zospy-1.0.0/zospy/analyses/psf.py` & `zospy-1.1.0/zospy/analyses/psf.py`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/analyses/raysandspots.py` & `zospy-1.1.0/zospy/analyses/raysandspots.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             target2 = order_of_appearance[order_of_appearance.index(target) + 1]
             section_end = inds[target2]["rnum"]
 
         # Read as dataframe
         df = pd.read_csv(
             StringIO("".join(line_list[section_start:section_end]).replace(" ", "")),
             delimiter="\t",
-            decimal=_config.DECIMAL,
+            decimal=_config.DECIMAL_POINT,
         )
 
         # Recover case of target
         keyname = inds[target]["name"].replace(" ", "")
 
         # Add to result dictionary
         res[keyname] = df
```

### Comparing `zospy-1.0.0/zospy/analyses/reports.py` & `zospy-1.1.0/zospy/analyses/reports.py`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/analyses/surface.py` & `zospy-1.1.0/zospy/analyses/surface.py`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/analyses/wavefront.py` & `zospy-1.1.0/zospy/analyses/wavefront.py`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Data/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/PhysicalOptics/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/PhysicalOptics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/RayTracing/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/RayTracing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Aberrations/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/Aberrations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/DiffractionEfficiency/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/DiffractionEfficiency/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/EncircledEnergy/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/EncircledEnergy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/ExtendedScene/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/ExtendedScene/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Fans/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/Fans/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Materials/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/Materials/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Mtf/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/Mtf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/NSCSurface/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/NSCSurface/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Psf/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/Psf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/RMS/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/RMS/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/RayTracing/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/RayTracing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Spot/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/Spot/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Surface/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/Surface/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Wavefront/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/Wavefront/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Settings/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Tolerancing/QuickYield/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Tolerancing/QuickYield/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Tolerancing/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/Tolerancing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Analysis/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Common/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Common/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Editors/LDE/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Editors/LDE/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Editors/MCE/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Editors/MCE/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Editors/MFE/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Editors/MFE/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Editors/NCE/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Editors/NCE/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Editors/TDE/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Editors/TDE/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Editors/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Editors/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Preferences/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Preferences/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/SystemData/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/SystemData/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Tools/General/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Tools/General/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Tools/LMx/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Tools/LMx/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Tools/Optimization/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Tools/Optimization/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Tools/RayTrace/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Tools/RayTrace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Tools/Tolerancing/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Tools/Tolerancing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Tools/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Tools/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/Wizards/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/Wizards/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/PhysicalOptics/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/PhysicalOptics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Aberrations/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Aberrations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/EncircledEnergy/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/EncircledEnergy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/ExtendedScene/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/ExtendedScene/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Mtf/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Mtf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/NSCSurface/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/NSCSurface/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Psf/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Psf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/RMS/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/RMS/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Spot/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Spot/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Wavefront/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Wavefront/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Tolerancing/QuickYield/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Tolerancing/QuickYield/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Tolerancing/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/Tolerancing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Analysis/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Common/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Common/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Editors/LDE/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Editors/LDE/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Editors/MCE/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Editors/MCE/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Editors/MFE/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Editors/MFE/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Editors/NCE/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Editors/NCE/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Editors/TDE/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Editors/TDE/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Editors/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Editors/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Preferences/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Preferences/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/SystemData/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/SystemData/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Tools/General/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Tools/General/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Tools/Optimization/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Tools/Optimization/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Tools/RayTrace/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Tools/RayTrace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Tools/Tolerancing/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Tools/Tolerancing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Tools/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Tools/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/Wizards/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/Wizards/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/_ZOSAPI_constants/__init__.pyi` & `zospy-1.1.0/zospy/api/_ZOSAPI_constants/__init__.pyi`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/apisupport.py` & `zospy-1.1.0/zospy/api/apisupport.py`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/api/constants.py` & `zospy-1.1.0/zospy/api/constants.py`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/solvers/__init__.py` & `zospy-1.1.0/zospy/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/utils/clrutils.py` & `zospy-1.1.0/zospy/utils/clrutils.py`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/utils/zputils.py` & `zospy-1.1.0/zospy/utils/zputils.py`

 * *Files identical despite different names*

### Comparing `zospy-1.0.0/zospy/zpcore.py` & `zospy-1.1.0/zospy/zpcore.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 import logging
 import warnings
 import weakref
 
+from semver.version import Version
+
 from zospy.api import _ZOSAPI, constants
 from zospy.api.apisupport import load_zosapi, load_zosapi_nethelper
 
 logger = logging.getLogger(__name__)
 
 
 class OpticStudioSystem:
@@ -433,14 +435,18 @@
         raise ValueError("Can only create a new system when using a standalone connection.")
 
     def get_primary_system(self) -> OpticStudioSystem:
         opticstudiosystem = self.Application.PrimarySystem
         return self._OpticStudioSystem(zos_instance=self, system_instance=opticstudiosystem)
 
     def get_system(self, pos: int = 0) -> OpticStudioSystem:
-        warnings.warn("ZOS.get_system() has not been tested yet")
-        # ToDo test
-        opticstudiosystem = self.Application.PrimarySystem.GetSystemAt(pos)
+        opticstudiosystem = self.Application.GetSystemAt(pos)
         return self._OpticStudioSystem(zos_instance=self, system_instance=opticstudiosystem)
 
-    def licence_check(self):
-        pass
+    @property
+    def version(self) -> Version:
+        """Returns the OpticStudio version as Version object."""
+        return Version(
+            major=self.Application.ZOSMajorVersion,
+            minor=self.Application.ZOSMinorVersion,
+            patch=self.Application.ZOSSPVersion,
+        )
```

### Comparing `zospy-1.0.0/PKG-INFO` & `zospy-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: zospy
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python package used to communicate with Zemax OpticStudio through the API
 Keywords: Zemax,OpticStudio,API,ZOSAPI
 Author-email: Luc van Vught <l.van_vught@lumc.nl>, Jan-Willem Beenakker <j.w.m.beenakker@lumc.nl>, Corné Haasjes <c.haasjes@lumc.nl>
 Requires-Python: >=3.9,<3.12
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
 Requires-Dist: pythonnet ~= 3.0.1
 Requires-Dist: pandas
 Requires-Dist: numpy
+Requires-Dist: semver ~= 3.0.0
 Requires-Dist: zospy[test] ; extra == "dev"
 Requires-Dist: black[jupyter] == 23.3.0 ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: pydantic ; extra == "dev"
 Requires-Dist: ruff ; extra == "dev"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: tox ; extra == "test"
@@ -73,18 +74,20 @@
 > :warning: Version 1.0.0 introduced some breaking changes. See
 > the [release notes](https://github.com/MREYE-LUMC/ZOSPy/releases/tag/v1.0.0) for more information.
 
 ZOSPy is tested with the following versions of Python and Ansys Zemax OpticStudio:
 
 | Zemax       | 20.3.2 | 23.0.1 |
 |-------------|--------|--------|
-| Python 3.8  | -      | ✔      |
-| Python 3.9  | -      | ✔      |
-| Python 3.10 | -      | ✔      |
-| Python 3.11 | ✔      | ✔      |
+| Python 3.9  | ⚠      | ✔      |
+| Python 3.10 | ⚠      | ✔      |
+| Python 3.11 | ⚠      | ✔      |
+
+✔: This version works without problems.
+⚠: This version works, but the output of analyses can differ slightly from the used reference version (currently **OpticStudio 23 R1.01**).
 
 ## Referencing
 
 When publishing results obtained with this package, please cite the paper in which the package was first used:<br>
 van Vught L, Que I, Luyten GPM and Beenakker JWM.
 _Effect of anatomical differences and intraocular lens design on Negative Dysphotopsia._
 JCRS: Sep 06, 2022.
```

